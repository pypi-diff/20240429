# Comparing `tmp/vlite-0.2.5.tar.gz` & `tmp/vlite-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlite-0.2.5.tar", last modified: Mon Apr 29 03:18:43 2024, max compression
+gzip compressed data, was "vlite-0.2.6.tar", last modified: Mon Apr 29 07:20:13 2024, max compression
```

## Comparing `vlite-0.2.5.tar` & `vlite-0.2.6.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-29 03:18:43.088370 vlite-0.2.5/
--rw-r--r--   0 sdan       (501) staff       (20)    34523 2024-03-27 04:16:34.000000 vlite-0.2.5/LICENSE
--rw-r--r--   0 sdan       (501) staff       (20)      595 2024-04-29 03:18:43.088235 vlite-0.2.5/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)     3247 2024-04-18 04:36:43.000000 vlite-0.2.5/README.md
--rw-r--r--   0 sdan       (501) staff       (20)       38 2024-04-29 03:18:43.088411 vlite-0.2.5/setup.cfg
--rw-r--r--   0 sdan       (501) staff       (20)     1043 2024-04-29 03:18:23.000000 vlite-0.2.5/setup.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-29 03:18:43.085956 vlite-0.2.5/tests/
--rw-r--r--   0 sdan       (501) staff       (20)     6320 2024-04-03 19:37:27.000000 vlite-0.2.5/tests/test_server.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-29 03:18:43.087375 vlite-0.2.5/vlite/
--rw-r--r--   0 sdan       (501) staff       (20)       57 2024-04-17 20:14:36.000000 vlite-0.2.5/vlite/__init__.py
--rw-r--r--   0 sdan       (501) staff       (20)     6744 2024-04-17 09:21:55.000000 vlite-0.2.5/vlite/ctx.py
--rw-r--r--   0 sdan       (501) staff       (20)     1331 2024-04-26 00:57:11.000000 vlite-0.2.5/vlite/index.py
--rw-r--r--   0 sdan       (501) staff       (20)    13527 2024-04-29 03:14:09.000000 vlite-0.2.5/vlite/main.py
--rw-r--r--   0 sdan       (501) staff       (20)     4484 2024-04-17 09:30:24.000000 vlite-0.2.5/vlite/model.py
--rw-r--r--   0 sdan       (501) staff       (20)     7781 2024-04-17 20:14:19.000000 vlite-0.2.5/vlite/server.py
--rw-r--r--   0 sdan       (501) staff       (20)     7980 2024-04-14 22:49:23.000000 vlite-0.2.5/vlite/utils.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-29 03:18:43.088033 vlite-0.2.5/vlite.egg-info/
--rw-r--r--   0 sdan       (501) staff       (20)      595 2024-04-29 03:18:43.000000 vlite-0.2.5/vlite.egg-info/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)      297 2024-04-29 03:18:43.000000 vlite-0.2.5/vlite.egg-info/SOURCES.txt
--rw-r--r--   0 sdan       (501) staff       (20)        1 2024-04-29 03:18:43.000000 vlite-0.2.5/vlite.egg-info/dependency_links.txt
--rw-r--r--   0 sdan       (501) staff       (20)      154 2024-04-29 03:18:43.000000 vlite-0.2.5/vlite.egg-info/requires.txt
--rw-r--r--   0 sdan       (501) staff       (20)        6 2024-04-29 03:18:43.000000 vlite-0.2.5/vlite.egg-info/top_level.txt
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-29 07:20:13.725481 vlite-0.2.6/
+-rw-r--r--   0 sdan       (501) staff       (20)    34523 2024-03-27 04:16:34.000000 vlite-0.2.6/LICENSE
+-rw-r--r--   0 sdan       (501) staff       (20)      595 2024-04-29 07:20:13.725367 vlite-0.2.6/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)     3247 2024-04-18 04:36:43.000000 vlite-0.2.6/README.md
+-rw-r--r--   0 sdan       (501) staff       (20)       38 2024-04-29 07:20:13.725523 vlite-0.2.6/setup.cfg
+-rw-r--r--   0 sdan       (501) staff       (20)     1062 2024-04-29 07:20:09.000000 vlite-0.2.6/setup.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-29 07:20:13.723529 vlite-0.2.6/tests/
+-rw-r--r--   0 sdan       (501) staff       (20)     6320 2024-04-03 19:37:27.000000 vlite-0.2.6/tests/test_server.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-29 07:20:13.724602 vlite-0.2.6/vlite/
+-rw-r--r--   0 sdan       (501) staff       (20)       57 2024-04-17 20:14:36.000000 vlite-0.2.6/vlite/__init__.py
+-rw-r--r--   0 sdan       (501) staff       (20)     1706 2024-04-29 06:46:56.000000 vlite-0.2.6/vlite/constants.py
+-rw-r--r--   0 sdan       (501) staff       (20)     7758 2024-04-29 07:14:45.000000 vlite-0.2.6/vlite/ctx.py
+-rw-r--r--   0 sdan       (501) staff       (20)     1331 2024-04-26 00:57:11.000000 vlite-0.2.6/vlite/index.py
+-rw-r--r--   0 sdan       (501) staff       (20)    14036 2024-04-29 07:15:10.000000 vlite-0.2.6/vlite/main.py
+-rw-r--r--   0 sdan       (501) staff       (20)     4484 2024-04-17 09:30:24.000000 vlite-0.2.6/vlite/model.py
+-rw-r--r--   0 sdan       (501) staff       (20)     7781 2024-04-17 20:14:19.000000 vlite-0.2.6/vlite/server.py
+-rw-r--r--   0 sdan       (501) staff       (20)     7980 2024-04-14 22:49:23.000000 vlite-0.2.6/vlite/utils.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-29 07:20:13.725180 vlite-0.2.6/vlite.egg-info/
+-rw-r--r--   0 sdan       (501) staff       (20)      595 2024-04-29 07:20:13.000000 vlite-0.2.6/vlite.egg-info/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)      316 2024-04-29 07:20:13.000000 vlite-0.2.6/vlite.egg-info/SOURCES.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        1 2024-04-29 07:20:13.000000 vlite-0.2.6/vlite.egg-info/dependency_links.txt
+-rw-r--r--   0 sdan       (501) staff       (20)      162 2024-04-29 07:20:13.000000 vlite-0.2.6/vlite.egg-info/requires.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        6 2024-04-29 07:20:13.000000 vlite-0.2.6/vlite.egg-info/top_level.txt
```

### Comparing `vlite-0.2.5/LICENSE` & `vlite-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vlite-0.2.5/PKG-INFO` & `vlite-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlite
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple and blazing fast vector database
 Author: Surya Dantuluri
 Author-email: surya@suryad.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `vlite-0.2.5/README.md` & `vlite-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `vlite-0.2.5/setup.py` & `vlite-0.2.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.2.5'
+__version__ = '0.2.6'
 
 setup(
     name='vlite',
     version=__version__,
     author='Surya Dantuluri',
     author_email='surya@suryad.com',
     description='A simple and blazing fast vector database',
@@ -17,14 +17,15 @@
         'requests',
         'beautifulsoup4',
         'huggingface_hub',
         'tiktoken',
         'torch==2.2.2',
         'transformers==4.39.0',
         'tokenizers==0.15.2',
+        'posthog',
     ],
     extras_require={
         'ocr': ['surya-ocr-vlite']
     },
     python_requires='>=3.10',
     classifiers=[
         'Development Status :: 4 - Beta',
```

### Comparing `vlite-0.2.5/tests/test_server.py` & `vlite-0.2.6/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `vlite-0.2.5/vlite/ctx.py` & `vlite-0.2.6/vlite/ctx.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import os
 import struct
 import json
 from enum import Enum
 from typing import List, Dict, Union
 import numpy as np
 import logging
-
+from posthog import Posthog
+from constants import Constants
+import uuid
 
 logging.basicConfig(level=logging.WARNING, format='%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
+posthog = Posthog(project_api_key=Constants.TELEMETRY_POSTHOG, host=Constants.TELEMETRY_POSTHOG_HOST, disable_geoip=False)
 
 class CtxSectionType(Enum):
     HEADER = 0
     EMBEDDINGS = 1
     CONTEXTS = 2
     METADATA = 3
 
@@ -27,14 +30,16 @@
             "embedding_size": 0,
             "embedding_dtype": "float32",
             "context_length": 0,
         }
         self.embeddings = []
         self.contexts = []
         self.metadata = {}
+        # Anonymized telemetry
+        self.anon_user_id = uuid.uuid4().hex if not os.path.exists(f"./contexts/{uuid.uuid4().hex}.telm") else open(f"./contexts/{uuid.uuid4().hex}.telm", "r").read()
 
     def set_header(self, embedding_model: str, embedding_size: int, embedding_dtype: str, context_length: int):
         self.header["embedding_model"] = embedding_model
         self.header["embedding_size"] = embedding_size
         self.header["embedding_dtype"] = embedding_dtype
         self.header["context_length"] = context_length
 
@@ -45,14 +50,18 @@
         self.contexts.append(context)
 
     def add_metadata(self, key: str, value: Union[int, float, str]):
         self.metadata[key] = value
         
     def save(self):
         with open(self.file_path, "wb") as file:
+            # Anonymized telemetry
+            if not os.path.exists(f"./contexts/{self.anon_user_id}.telm"): open(f"./contexts/{self.anon_user_id}.telm", "w").write(self.anon_user_id)            
+            posthog.capture(self.anon_user_id,'ctx_save',{'file_path': self.file_path,'header': self.header})
+            
             file.write(self.MAGIC_NUMBER)
             file.write(struct.pack("<I", self.VERSION))
 
             header_json = json.dumps(self.header).encode("utf-8")
             file.write(struct.pack("<II", CtxSectionType.HEADER.value, len(header_json)))
             file.write(header_json)
 
@@ -72,14 +81,18 @@
             file.write(struct.pack("<II", CtxSectionType.METADATA.value, len(metadata_json)))
             file.write(metadata_json)
         
 
     def load(self):
         try:
             with open(self.file_path, "rb") as file:
+                # Anonymized telemetry
+                if not os.path.exists(f"./contexts/{self.anon_user_id}.telm"): open(f"./contexts/{self.anon_user_id}.telm", "w").write(self.anon_user_id)
+                posthog.capture(self.anon_user_id,'ctx_load',{'file_path': self.file_path})
+                
                 # Read and verify header
                 magic_number = file.read(len(self.MAGIC_NUMBER))
                 if magic_number != self.MAGIC_NUMBER:
                     raise ValueError(f"Invalid magic number: {magic_number}")
 
                 version = struct.unpack("<I", file.read(4))[0]
                 if version != self.VERSION:
```

### Comparing `vlite-0.2.5/vlite/index.py` & `vlite-0.2.6/vlite/index.py`

 * *Files identical despite different names*

### Comparing `vlite-0.2.5/vlite/main.py` & `vlite-0.2.6/vlite/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,30 @@
 from .utils import check_cuda_available, check_mps_available
 from .model import EmbeddingModel
 from .utils import chop_and_chunk
 import datetime
 from .ctx import Ctx
 import time
 import logging
+from posthog import Posthog
+from constants import Constants
+import os
 
 # Configure logging
 logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
-
+posthog = Posthog(project_api_key=Constants.TELEMETRY_POSTHOG, host=Constants.TELEMETRY_POSTHOG_HOST, disable_geoip=False)
 
 class VLite:
     def __init__(self, collection=None, device=None, model_name='mixedbread-ai/mxbai-embed-large-v1'):
         start_time = time.time()
+        # Anonymized telemetry
+        self.anon_user_id = uuid4().hex if not os.path.exists(f"./contexts/{uuid4().hex}.telm") else open(f"./contexts/{uuid4().hex}.telm", "r").read()
+        posthog.capture(self.anon_user_id,'vlite_init',{'collection': collection,'device': device,'model_name': model_name})
+        
         if device is None:
             if check_cuda_available():
                 device = 'cuda'
             elif check_mps_available():
                 device = 'mps'
             else:
                 device = 'cpu'
```

### Comparing `vlite-0.2.5/vlite/model.py` & `vlite-0.2.6/vlite/model.py`

 * *Files identical despite different names*

### Comparing `vlite-0.2.5/vlite/server.py` & `vlite-0.2.6/vlite/server.py`

 * *Files identical despite different names*

### Comparing `vlite-0.2.5/vlite/utils.py` & `vlite-0.2.6/vlite/utils.py`

 * *Files identical despite different names*

### Comparing `vlite-0.2.5/vlite.egg-info/PKG-INFO` & `vlite-0.2.6/vlite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlite
-Version: 0.2.5
+Version: 0.2.6
 Summary: A simple and blazing fast vector database
 Author: Surya Dantuluri
 Author-email: surya@suryad.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

