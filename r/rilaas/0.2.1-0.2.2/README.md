# Comparing `tmp/rilaas-0.2.1.tar.gz` & `tmp/rilaas-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rilaas-0.2.1.tar", last modified: Thu Apr 18 13:49:40 2024, max compression
+gzip compressed data, was "rilaas-0.2.2.tar", last modified: Mon Apr 29 10:21:17 2024, max compression
```

## Comparing `rilaas-0.2.1.tar` & `rilaas-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 13:49:40.102779 rilaas-0.2.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2024-03-08 10:28:21.000000 rilaas-0.2.1/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1639 2024-04-18 13:49:40.102779 rilaas-0.2.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1294 2024-04-18 13:49:03.000000 rilaas-0.2.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 13:49:40.102779 rilaas-0.2.1/rilaas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16524 2024-04-18 13:44:51.000000 rilaas-0.2.1/rilaas/Client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-08 10:28:21.000000 rilaas-0.2.1/rilaas/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      690 2024-04-18 13:45:02.000000 rilaas-0.2.1/rilaas/get_file_type.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-18 13:49:40.102779 rilaas-0.2.1/rilaas.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1639 2024-04-18 13:49:39.000000 rilaas-0.2.1/rilaas.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2024-04-18 13:49:40.000000 rilaas-0.2.1/rilaas.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-18 13:49:39.000000 rilaas-0.2.1/rilaas.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2024-04-18 13:49:39.000000 rilaas-0.2.1/rilaas.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2024-04-18 13:49:39.000000 rilaas-0.2.1/rilaas.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-18 13:49:40.102779 rilaas-0.2.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      688 2024-04-18 13:47:01.000000 rilaas-0.2.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 10:21:17.056291 rilaas-0.2.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1074 2024-03-08 10:28:21.000000 rilaas-0.2.2/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1639 2024-04-29 10:21:17.056291 rilaas-0.2.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1294 2024-04-18 13:49:03.000000 rilaas-0.2.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 10:21:17.052291 rilaas-0.2.2/rilaas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18994 2024-04-29 10:17:29.000000 rilaas-0.2.2/rilaas/Client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-08 10:28:21.000000 rilaas-0.2.2/rilaas/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      690 2024-04-18 13:45:02.000000 rilaas-0.2.2/rilaas/get_file_type.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-29 10:21:17.052291 rilaas-0.2.2/rilaas.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1639 2024-04-29 10:21:16.000000 rilaas-0.2.2/rilaas.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      235 2024-04-29 10:21:16.000000 rilaas-0.2.2/rilaas.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-29 10:21:16.000000 rilaas-0.2.2/rilaas.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       34 2024-04-29 10:21:16.000000 rilaas-0.2.2/rilaas.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2024-04-29 10:21:16.000000 rilaas-0.2.2/rilaas.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-29 10:21:17.056291 rilaas-0.2.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      688 2024-04-29 10:20:49.000000 rilaas-0.2.2/setup.py
```

### Comparing `rilaas-0.2.1/LICENSE` & `rilaas-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rilaas-0.2.1/PKG-INFO` & `rilaas-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rilaas
-Version: 0.2.1
+Version: 0.2.2
 Summary: This is a package for getting a response from the EC2 server for the models deployed for ServeLine
 Home-page: https://github.com/ahfahad96/rilaas
 Author: Abdul Hafeez Fahad
 Author-email: ah.fahad@redbuffer.net
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rilaas-0.2.1/README.md` & `rilaas-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `rilaas-0.2.1/rilaas/Client.py` & `rilaas-0.2.2/rilaas/Client.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,137 +4,148 @@
 current_dir = os.path.dirname(os.path.abspath(__file__))
 sys.path.append(current_dir)
 
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 from get_file_type import get_mime_type
 import requests
 import json
+import aiohttp
 
 class Client:
     def __init__(self, api_key, **kwargs):
         self.ptr_id = kwargs.get('id', None)
         self.model_name = kwargs.get('name', None)
         self.api_key = api_key
         self.api_url = 'https://n4kh6hh8p3.execute-api.us-east-1.amazonaws.com/rilaas_client_get_metadata'
         self.endpoint_params = None
         self.model_predictor = None
         self.selected_endpoint = None
         self.response_metadata = None
 
-    def get_endpoints(self):
+    async def get_endpoints(self):
         if self.ptr_id is not None:
             if self.endpoint_params:
                 return self.endpoint_params
             
             request_type = 'endpoints'
-            
             headers = {
                 'Content-Type': 'application/json',
                 'API_KEY': self.api_key
             }
 
             data = {
                 'ptr_id': self.ptr_id,
                 'request_type': request_type
             }
-
-            try:
-                response = requests.post(self.api_url, headers=headers, json=data)
-                self.response_metadata = response.json()
-                self.endpoint_params = self.response_metadata[0]
-                return self.endpoint_params
-        
-            except requests.RequestException as e:
-                print(f"Error during request: {e}")
-                return None
+            async with aiohttp.ClientSession() as session:
+                try:
+                    async with session.post(self.api_url, headers=headers, json=data) as response:
+                        self.response_metadata = await response.json()
+                        self.endpoint_params = self.response_metadata[0]
+                        return self.endpoint_params
+            
+                except aiohttp.ClientError as e:
+                    print(f"Error during request: {e}")
+                    return None
         else:
             return None
         
-    def get_ptr_id(self):
+    async def get_ptr_id(self):
         if self.ptr_id is None:
             if self.model_name is not None:
                 request_type = 'get_ptr_id'
                 
                 headers = {
                     'Content-Type': 'application/json',
                     'API_KEY': self.api_key
                 }
 
                 data = {
                     'name': self.model_name,
                     'request_type': request_type
                 }
-
-                try:
-                    response = requests.post(self.api_url, headers=headers, json=data)
-                    self.ptr_id = response.text
-                    return response.text
-            
-                except requests.RequestException as e:
-                    print(f"Error during request: {e}")
-                    return None
+                async with aiohttp.ClientSession() as session:
+                    try:
+                        async with session.post(self.api_url, headers=headers, json=data) as response:
+                        # response = requests.post(self.api_url, headers=headers, json=data)
+                            self.ptr_id = await response.text()
+                            return response.text
+                
+                    except requests.RequestException as e:
+                        print(f"Error during request: {e}")
+                        return None
             else:
                 return None
         else:
             return self.ptr_id
         
-    def get_parameters(self, endpoint):
+    async def get_parameters(self, endpoint):
         if self.endpoint_params and endpoint in self.endpoint_params:
             self.selected_endpoint = endpoint
             return self.endpoint_params[endpoint]
         else:
             print(f"Endpoint '{endpoint}' not found or failed to fetch endpoints.")
             return None
     
-    def init_model_predictor(self):
+    async def init_model_predictor(self):
         if self.response_metadata[2].lower() in 'yolov5':
             self.model_predictor = Yolov5_Client(self.ptr_id, self.api_key, self.selected_endpoint)
         elif self.response_metadata[2].lower() in ["diffusers_sd", "diffusers_sdxl", "sdxl_turbo"]:
             self.model_predictor = Diffusers_Client(self.ptr_id, self.api_key, self.selected_endpoint)
         elif self.response_metadata[2].lower() in 'llms':
             self.model_predictor = Llms_Client(self.ptr_id, self.api_key, self.selected_endpoint)
         elif self.response_metadata[2].lower() in 'transformers':
             self.model_predictor = Transformers_Client(self.ptr_id, self.api_key, self.selected_endpoint, self.response_metadata[3])
+        elif self.response_metadata[2].lower() in 'custom':
+            self.model_predictor = CustomModel_Client(self.ptr_id, self.api_key, self.selected_endpoint, self.response_metadata[3])
         else:
             print ("Wrong Model Input")
             
-    def predict(self, **kwargs):
+    async def predict(self, **kwargs):
         if not self.model_predictor:
-            self.init_model_predictor()
+            await self.init_model_predictor()
 
-        return self.model_predictor.predict(**kwargs)
+        return await self.model_predictor.predict(**kwargs)
         
 
 class Yolov5_Client():
     def __init__(self, ptr_id, api_key, selected_endpoint):
         self.initial_url = 'https://n4kh6hh8p3.execute-api.us-east-1.amazonaws.com/'
         self.ptr_id = ptr_id
         self.api_key = api_key 
         self.selected_endpoint = selected_endpoint
     
-    def predict(self, **kwargs):
+    async def predict(self, **kwargs):
         url = os.path.join(self.initial_url, self.ptr_id, "inference", self.selected_endpoint)
         
         payload = {}
         img_path = kwargs.get('image_path', None)
-        files=[('img',(os.path.basename(img_path),open(img_path,'rb'),'image/jpeg'))]
+        # files=[('img',(os.path.basename(img_path),open(img_path,'rb'),'image/jpeg'))]
         headers = {
         'API_KEY': self.api_key
         }
-        response = requests.request("POST", url, headers=headers, data=payload, files=files)
-        return response
+        async with aiohttp.ClientSession() as session:
+            try:
+                with open(img_path, 'rb') as file:
+                    files = {'img': file}
+                    data = {**payload, **files}
+                    async with session.post(url, headers=headers, data=data) as response:
+                        return await response.read()
+            except aiohttp.ClientError as e:
+                print(f"Error during request: {e}")
+                return None
 
 class Diffusers_Client():
     def __init__(self, ptr_id, api_key, selected_endpoint):
         self.initial_url = 'https://n4kh6hh8p3.execute-api.us-east-1.amazonaws.com/'
         self.ptr_id = ptr_id
         self.api_key = api_key
         self.selected_endpoint = selected_endpoint
     
-    def predict(self, **kwargs):
+    async def predict(self, **kwargs):
         url = os.path.join(self.initial_url, self.ptr_id, "inference", self.selected_endpoint)
         
         if "txt2img" == self.selected_endpoint.lower():
             
             data = {
                 "prompt": kwargs.get('prompt', None),
                 "negative_prompt": kwargs.get('negative_prompt', None),
@@ -150,22 +161,21 @@
             multipart_encoder = MultipartEncoder(fields=fields)
     
             headers = {
                 'accept': 'image/jpeg',
                 'Content-Type': multipart_encoder.content_type,
                 'API_KEY': self.api_key
             }
-            
-            response = requests.request(
-                method="POST",
-                url=url,
-                headers=headers,
-                data=multipart_encoder.to_string()
-            )
-            return response
+            async with aiohttp.ClientSession() as session:
+                try:
+                    async with session.post(url = url, headers=headers, data=multipart_encoder.to_string()) as response:
+                        return await response.read()
+                except aiohttp.ClientError as e:
+                    print(f"Error during request: {e}")
+                    return None
             
         elif "img2img" == self.selected_endpoint.lower():
             
             data = {
                 "prompt": kwargs.get('prompt', None),
                 "negative_prompt": kwargs.get('negative_prompt', None),
                 "height": kwargs.get('height', None),
@@ -181,22 +191,21 @@
             multipart_encoder = MultipartEncoder(fields=fields)
     
             headers = {
                 'accept': 'image/jpeg',
                 'Content-Type': multipart_encoder.content_type,
                 'API_KEY': self.api_key
             }
-            
-            response = requests.request(
-                method="POST",
-                url=url,
-                headers=headers,
-                data=multipart_encoder.to_string()
-            )
-            return response
+            async with aiohttp.ClientSession() as session:
+                try:
+                    async with session.post(url = url, headers=headers, data=multipart_encoder.to_string()) as response:
+                        return await response.read()
+                except aiohttp.ClientError as e:
+                    print(f"Error during request: {e}")
+                    return None
             
         elif "inpaint" == self.selected_endpoint.lower():
             
             data = {
                 "prompt": kwargs.get('prompt', None),
                 "negative_prompt": kwargs.get('negative_prompt', None),
                 "height": kwargs.get('height', None),
@@ -213,35 +222,32 @@
             multipart_encoder = MultipartEncoder(fields=fields)
     
             headers = {
                 'accept': 'image/jpeg',
                 'Content-Type': multipart_encoder.content_type,
                 'API_KEY': self.api_key
             }
-            
-            response = requests.request(
-                method="POST",
-                url=url,
-                headers=headers,
-                data=multipart_encoder.to_string()
-            )
-            return response
-            
+            async with aiohttp.ClientSession() as session:
+                try:
+                    async with session.post(url = url, headers=headers, data=multipart_encoder.to_string()) as response:
+                        return await response.read()
+                except aiohttp.ClientError as e:
+                    print(f"Error during request: {e}")
+                    return None
         else:
             return "Endpoint does not exists"
         
 class Llms_Client():
-    # need to fix the payload input
     def __init__(self, ptr_id, api_key, selected_endpoint):
         self.initial_url = 'https://n4kh6hh8p3.execute-api.us-east-1.amazonaws.com/'
         self.ptr_id = ptr_id
         self.api_key = api_key 
         self.selected_endpoint = selected_endpoint
     
-    def predict(self, **kwargs):
+    async def predict(self, **kwargs):
         url = os.path.join(self.initial_url, self.ptr_id, "inference", self.selected_endpoint)
         
         sampling_params = {
             "temperature": kwargs.get("sampling_params", {}).get("temperature"),
             "logprobs": kwargs.get("sampling_params", {}).get("logprobs")
         }
         data = {
@@ -255,54 +261,52 @@
             }
         multipart_encoder = MultipartEncoder(fields=fields)
         headers = {
                 'accept': 'image/jpeg',
                 'Content-Type': multipart_encoder.content_type,
                 'API_KEY': self.api_key
             }
-        
-        response = requests.request(
-                method="POST",
-                url=url,
-                headers=headers,
-                data=multipart_encoder.to_string()
-            )
-        return response
+        async with aiohttp.ClientSession() as session:
+                try:
+                    async with session.post(url = url, headers=headers, data=multipart_encoder.to_string()) as response:
+                        return await response.read()
+                except aiohttp.ClientError as e:
+                    print(f"Error during request: {e}")
+                    return None
     
 class Transformers_Client():
     def __init__(self, ptr_id, api_key, selected_endpoint, model_sub_category):
         self.initial_url = 'https://n4kh6hh8p3.execute-api.us-east-1.amazonaws.com/'
         self.ptr_id = ptr_id
         self.api_key = api_key 
         self.selected_endpoint = selected_endpoint
         self.model_sub_category = model_sub_category
     
-    def predict(self, **kwargs):
+    async def predict(self, **kwargs):
         url = os.path.join(self.initial_url, self.ptr_id, "inference", self.selected_endpoint)
         if self.model_sub_category.lower() == "summarization" or self.model_sub_category.lower() == "token-classification" or self.model_sub_category.lower() == "text-classification" or self.model_sub_category.lower() == "text2text-generation":
             data = {
                     "inputs": kwargs.get('inputs', None)
                 }
             fields = {
                     'data': json.dumps(data)
                 }
             multipart_encoder = MultipartEncoder(fields=fields)
             headers = {
                     'accept': 'image/jpeg',
                     'Content-Type': multipart_encoder.content_type,
                     'API_KEY': self.api_key
                 }
-            
-            response = requests.request(
-                    method="POST",
-                    url=url,
-                    headers=headers,
-                    data=multipart_encoder.to_string()
-                )
-            return response
+            async with aiohttp.ClientSession() as session:
+                try:
+                    async with session.post(url = url, headers=headers, data=multipart_encoder.to_string()) as response:
+                        return await response.read()
+                except aiohttp.ClientError as e:
+                    print(f"Error during request: {e}")
+                    return None
         
         elif self.model_sub_category.lower() == "question-answering":
             data = {
                     "question": kwargs.get("question",None),
                     "context": kwargs.get("context",None),
                 }
             fields = {
@@ -310,22 +314,21 @@
                 }
             multipart_encoder = MultipartEncoder(fields=fields)
             headers = {
                     'accept': 'image/jpeg',
                     'Content-Type': multipart_encoder.content_type,
                     'API_KEY': self.api_key
                 }
-            
-            response = requests.request(
-                    method="POST",
-                    url=url,
-                    headers=headers,
-                    data=multipart_encoder.to_string()
-                )
-            return response
+            async with aiohttp.ClientSession() as session:
+                try:
+                    async with session.post(url = url, headers=headers, data=multipart_encoder.to_string()) as response:
+                        return await response.read()
+                except aiohttp.ClientError as e:
+                    print(f"Error during request: {e}")
+                    return None
         
         elif self.model_sub_category.lower() == "translation":
             data = {
                     "inputs": kwargs.get("inputs",None),
                     "src_lang": kwargs.get("src_lang",None),
                     "tgt_lang": kwargs.get("tgt_lang",None)
                 }
@@ -334,22 +337,22 @@
                 }
             multipart_encoder = MultipartEncoder(fields=fields)
             headers = {
                     'accept': 'image/jpeg',
                     'Content-Type': multipart_encoder.content_type,
                     'API_KEY': self.api_key
                 }
-            
-            response = requests.request(
-                    method="POST",
-                    url=url,
-                    headers=headers,
-                    data=multipart_encoder.to_string()
-                )
-            return response
+            async with aiohttp.ClientSession() as session:
+                try:
+                    async with session.post(url = url, headers=headers, data=multipart_encoder.to_string()) as response:
+                        return await response.read()
+                except aiohttp.ClientError as e:
+                    print(f"Error during request: {e}")
+                    return None
+                
         elif self.model_sub_category.lower() == "table-question-answering":
             inputs = {
                     "query": kwargs.get("inputs", {}).get("query"),
                     "table": kwargs.get("inputs", {}).get("table"),
                 }
             payload = {
                 "inputs": inputs
@@ -360,21 +363,22 @@
             multipart_encoder = MultipartEncoder(fields=fields)
             headers = {
                     'accept': 'image/jpeg',
                     'Content-Type': multipart_encoder.content_type,
                     'API_KEY': self.api_key
                 }
             
-            response = requests.request(
-                    method="POST",
-                    url=url,
-                    headers=headers,
-                    data=multipart_encoder.to_string()
-                )
-            return response
+            async with aiohttp.ClientSession() as session:
+                try:
+                    async with session.post(url = url, headers=headers, data=multipart_encoder.to_string()) as response:
+                        return await response.read()
+                except aiohttp.ClientError as e:
+                    print(f"Error during request: {e}")
+                    return None
+                
         elif self.model_sub_category.lower() == "zero-shot-classification":
             data = {
                     "inputs": kwargs.get("inputs",None),
                     "candidate_labels": kwargs.get("candidate_labels",None)
                 }
             fields = {
                     'data': json.dumps(data)
@@ -382,30 +386,31 @@
             multipart_encoder = MultipartEncoder(fields=fields)
             headers = {
                     'accept': 'image/jpeg',
                     'Content-Type': multipart_encoder.content_type,
                     'API_KEY': self.api_key
                 }
             
-            response = requests.request(
-                    method="POST",
-                    url=url,
-                    headers=headers,
-                    data=multipart_encoder.to_string()
-                )
-            return response
+            async with aiohttp.ClientSession() as session:
+                try:
+                    async with session.post(url = url, headers=headers, data=multipart_encoder.to_string()) as response:
+                        return await response.read()
+                except aiohttp.ClientError as e:
+                    print(f"Error during request: {e}")
+                    return None
         
 class CustomModel_Client():
     def __init__(self, ptr_id, api_key, selected_endpoint):
         self.initial_url = 'https://n4kh6hh8p3.execute-api.us-east-1.amazonaws.com/'
         self.ptr_id = ptr_id
         self.api_key = api_key
         self.selected_endpoint = selected_endpoint
     
-    def predict(self, **kwargs):
+    async def predict(self, **kwargs):
+        print ('hrel')
         url = os.path.join(self.initial_url, self.ptr_id, "inference", self.selected_endpoint)
         fields = {}
     
         if 'text' in kwargs:
             fields['text'] = json.dumps(kwargs['text'])
         
         if 'json' in kwargs:
@@ -426,14 +431,14 @@
         multipart_encoder = MultipartEncoder(fields=fields)
         headers = {
             'accept': 'image/jpeg',
             'Content-Type': multipart_encoder.content_type,
             'API_KEY': self.api_key
         }
         
-        response = requests.request(
-            method="POST",
-            url=url,
-            headers=headers,
-            data=multipart_encoder.to_string()
-        )
-        return response
+        async with aiohttp.ClientSession() as session:
+            try:
+                async with session.post(url = url, headers=headers, data=multipart_encoder.to_string()) as response:
+                    return await response.read()
+            except aiohttp.ClientError as e:
+                print(f"Error during request: {e}")
+                return None
```

### Comparing `rilaas-0.2.1/rilaas/get_file_type.py` & `rilaas-0.2.2/rilaas/get_file_type.py`

 * *Files identical despite different names*

### Comparing `rilaas-0.2.1/rilaas.egg-info/PKG-INFO` & `rilaas-0.2.2/rilaas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rilaas
-Version: 0.2.1
+Version: 0.2.2
 Summary: This is a package for getting a response from the EC2 server for the models deployed for ServeLine
 Home-page: https://github.com/ahfahad96/rilaas
 Author: Abdul Hafeez Fahad
 Author-email: ah.fahad@redbuffer.net
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rilaas-0.2.1/setup.py` & `rilaas-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rilaas',
-    version='0.2.1',
+    version='0.2.2',
     packages=find_packages(),
     # package_data={'config': ['*.yaml']},
     install_requires=[
         'requests',
         'pyyaml',
         'requests-toolbelt'
```

