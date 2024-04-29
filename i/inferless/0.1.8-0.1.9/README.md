# Comparing `tmp/inferless-0.1.8.tar.gz` & `tmp/inferless-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inferless-0.1.8.tar", max compression
+gzip compressed data, was "inferless-0.1.9.tar", max compression
```

## Comparing `inferless-0.1.8.tar` & `inferless-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2196 2024-04-25 13:52:25.406985 inferless-0.1.8/README.md
--rw-r--r--   0        0        0      114 2023-12-18 13:10:49.190353 inferless-0.1.8/inferless/__init__.py
--rw-r--r--   0        0        0     2489 2024-04-25 14:13:33.435568 inferless-0.1.8/inferless/api.py
--rw-r--r--   0        0        0       59 2024-04-25 13:52:25.407586 inferless-0.1.8/inferless/utils/__init__.py
--rw-r--r--   0        0        0     2124 2024-04-25 13:52:25.407890 inferless-0.1.8/inferless/utils/inputs.py
--rw-r--r--   0        0        0      282 2024-04-25 13:52:25.408278 inferless-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 inferless-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2295 2024-04-29 11:21:49.363335 inferless-0.1.9/README.md
+-rw-r--r--   0        0        0      114 2024-04-29 11:24:54.430704 inferless-0.1.9/inferless/__init__.py
+-rw-r--r--   0        0        0     2742 2024-04-29 11:18:42.233009 inferless-0.1.9/inferless/api.py
+-rw-r--r--   0        0        0       59 2024-04-26 09:38:11.712037 inferless-0.1.9/inferless/utils/__init__.py
+-rw-r--r--   0        0        0     2193 2024-04-29 11:17:52.288828 inferless-0.1.9/inferless/utils/inputs.py
+-rw-r--r--   0        0        0      282 2024-04-29 11:24:48.742915 inferless-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2828 1970-01-01 00:00:00.000000 inferless-0.1.9/PKG-INFO
```

### Comparing `inferless-0.1.8/README.md` & `inferless-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -78,7 +78,10 @@
 print(t2 - t1)
 ```
 Output
 ```console
 time taken: 0:00:00.000141
 ```
 It can be seen that the program continues without waiting for the response. The response is written to a file by the callback function after it is received.
+
+### Batch call
+If the model is configured for batch processing, `is_batch` should be set to `True`
```

### Comparing `inferless-0.1.8/inferless/api.py` & `inferless-0.1.9/inferless/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import os
 from typing import Optional, Any
 import json
 import threading
 from .utils import create_data
 
 
-def call(url: str, workspace_api_key: Optional[str] = None, data: Optional[dict] = None, callback: Optional[Any] = None, inputs: Optional[dict] = None):
+def call(url: str, workspace_api_key: Optional[str] = None, data: Optional[dict] = None, callback: Optional[Any] = None,
+         inputs: Optional[dict] = None, is_batch: Optional[bool] = False):
     """
     Call Inferless API
     :param url: Inferless Model API URL
     :param workspace_api_key: Inferless Workspace API Key
     :param data: Model Input Data as a dictionary, example: {"question": "What is the capital of France?", "context": "Paris is the capital of France."}
     :param callback: Callback function to be called after the response is received
     :param inputs: Model Input Data in inferless format
+    :param is_batch: Whether the input is a batch of inputs, default is False
     :return: Response from the API call
     """
     try:
         if inputs is not None and data is not None:
             raise Exception("Cannot provide both data and inputs")
 
         if data is not None:
-            inputs = create_data(data)
+            inputs = create_data(data, is_batch)
 
         import requests
         if workspace_api_key is None:
             workspace_api_key = os.environ.get("INFERLESS_API_KEY")
         headers = {"Content-Type": "application/json",
                    "Authorization": f"Bearer {workspace_api_key}"}
         if inputs is None:
@@ -40,20 +42,21 @@
         if callback is not None:
             callback(e, None)
         else:
             raise e
 
 
 def call_async(url: str, workspace_api_key: Optional[str] = None, data: Optional[dict] = None,
-               callback: Any = None, inputs: Optional[dict] = None):
+               callback: Any = None, inputs: Optional[dict] = None, is_batch: Optional[bool] = False):
     """
     Call Inferless API
     :param url: Inferless Model API URL
     :param workspace_api_key: Inferless Workspace API Key
     :param data: Model Input Data as a dictionary, example: {"question": "What is the capital of France?", "context": "Paris is the capital of France."}
     :param callback: Callback function to be called after the response is received
     :param inputs: Model Input Data in inferless format
+    :param is_batch: Whether the input is a batch of inputs, default is False
     :return: Response from the API call
     """
-    thread = threading.Thread(target=call, args=(url, workspace_api_key, data, callback, inputs))
+    thread = threading.Thread(target=call, args=(url, workspace_api_key, data, callback, inputs, is_batch))
     thread.start()
     return thread
```

### Comparing `inferless-0.1.8/inferless/utils/inputs.py` & `inferless-0.1.9/inferless/utils/inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,20 +11,22 @@
     np.dtype('int64'): "INT64",
     np.dtype('float16'): "FP16",
     np.dtype('float32'): "FP32",
     np.dtype('float64'): "FP64"
 }
 
 
-def create_data(prompts):
+def create_data(prompts, is_batch=False):
     inputs = {
         "inputs": []
     }
     for key, value in prompts.items():
         data, data_type, shape = extract_data(value)
+        if is_batch:
+            shape = [1] + shape
         inputs["inputs"].append(
             {
                 "data": data,
                 "name": key,
                 "shape": shape,
                 "datatype": data_type,
             }
```

### Comparing `inferless-0.1.8/PKG-INFO` & `inferless-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inferless
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Inferless
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -95,7 +95,9 @@
 ```
 Output
 ```console
 time taken: 0:00:00.000141
 ```
 It can be seen that the program continues without waiting for the response. The response is written to a file by the callback function after it is received.
 
+### Batch call
+If the model is configured for batch processing, `is_batch` should be set to `True`
```

