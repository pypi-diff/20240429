# Comparing `tmp/bagelML-0.0.13.tar.gz` & `tmp/bagelML-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bagelML-0.0.13.tar", last modified: Thu Apr 18 08:29:17 2024, max compression
+gzip compressed data, was "bagelML-0.0.14.tar", last modified: Mon Apr 29 10:07:22 2024, max compression
```

## Comparing `bagelML-0.0.13.tar` & `bagelML-0.0.14.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-18 08:29:17.081661 bagelML-0.0.13/
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     6713 2024-04-18 08:29:17.081434 bagelML-0.0.13/PKG-INFO
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     5638 2024-04-02 18:31:43.000000 bagelML-0.0.13/README.md
-drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-18 08:29:17.078238 bagelML-0.0.13/bagel/
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      376 2024-04-18 08:27:45.000000 bagelML-0.0.13/bagel/__init__.py
-drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-18 08:29:17.079555 bagelML-0.0.13/bagel/api/
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    15205 2024-04-02 18:31:43.000000 bagelML-0.0.13/bagel/api/Cluster.py
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    13969 2024-04-18 08:27:54.000000 bagelML-0.0.13/bagel/api/__init__.py
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    22393 2024-04-18 08:27:54.000000 bagelML-0.0.13/bagel/api/fastapi.py
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    11570 2024-02-22 02:33:19.000000 bagelML-0.0.13/bagel/api/types.py
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     5965 2024-02-22 02:33:19.000000 bagelML-0.0.13/bagel/config.py
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      683 2024-02-22 02:33:19.000000 bagelML-0.0.13/bagel/errors.py
-drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-18 08:29:17.079881 bagelML-0.0.13/bagel/utils/
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)        0 2024-02-22 02:33:19.000000 bagelML-0.0.13/bagel/utils/__init__.py
-drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-18 08:29:17.080533 bagelML-0.0.13/bagelML.egg-info/
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     6713 2024-04-18 08:29:17.000000 bagelML-0.0.13/bagelML.egg-info/PKG-INFO
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      383 2024-04-18 08:29:17.000000 bagelML-0.0.13/bagelML.egg-info/SOURCES.txt
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)        1 2024-04-18 08:29:17.000000 bagelML-0.0.13/bagelML.egg-info/dependency_links.txt
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      267 2024-04-18 08:29:17.000000 bagelML-0.0.13/bagelML.egg-info/requires.txt
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)       11 2024-04-18 08:29:17.000000 bagelML-0.0.13/bagelML.egg-info/top_level.txt
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)       38 2024-04-18 08:29:17.081712 bagelML-0.0.13/setup.cfg
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     1217 2024-04-18 08:27:54.000000 bagelML-0.0.13/setup.py
-drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-18 08:29:17.081042 bagelML-0.0.13/test/
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)        0 2024-02-22 02:33:19.000000 bagelML-0.0.13/test/__init__.py
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     2717 2024-04-02 18:31:43.000000 bagelML-0.0.13/test/client_test.py
--rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     2332 2024-02-22 02:33:19.000000 bagelML-0.0.13/test/opt_test.py
+drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-29 10:07:22.526587 bagelML-0.0.14/
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     6713 2024-04-29 10:07:22.526392 bagelML-0.0.14/PKG-INFO
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     5638 2024-04-02 18:31:43.000000 bagelML-0.0.14/README.md
+drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-29 10:07:22.523285 bagelML-0.0.14/bagel/
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      376 2024-04-18 08:27:45.000000 bagelML-0.0.14/bagel/__init__.py
+drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-29 10:07:22.524492 bagelML-0.0.14/bagel/api/
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    15205 2024-04-02 18:31:43.000000 bagelML-0.0.14/bagel/api/Cluster.py
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    14224 2024-04-29 10:06:57.000000 bagelML-0.0.14/bagel/api/__init__.py
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    23695 2024-04-29 10:06:57.000000 bagelML-0.0.14/bagel/api/fastapi.py
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)    11570 2024-02-22 02:33:19.000000 bagelML-0.0.14/bagel/api/types.py
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     5965 2024-02-22 02:33:19.000000 bagelML-0.0.14/bagel/config.py
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      683 2024-02-22 02:33:19.000000 bagelML-0.0.14/bagel/errors.py
+drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-29 10:07:22.524838 bagelML-0.0.14/bagel/utils/
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)        0 2024-02-22 02:33:19.000000 bagelML-0.0.14/bagel/utils/__init__.py
+drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-29 10:07:22.525414 bagelML-0.0.14/bagelML.egg-info/
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     6713 2024-04-29 10:07:22.000000 bagelML-0.0.14/bagelML.egg-info/PKG-INFO
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      383 2024-04-29 10:07:22.000000 bagelML-0.0.14/bagelML.egg-info/SOURCES.txt
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)        1 2024-04-29 10:07:22.000000 bagelML-0.0.14/bagelML.egg-info/dependency_links.txt
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)      267 2024-04-29 10:07:22.000000 bagelML-0.0.14/bagelML.egg-info/requires.txt
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)       11 2024-04-29 10:07:22.000000 bagelML-0.0.14/bagelML.egg-info/top_level.txt
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)       38 2024-04-29 10:07:22.526629 bagelML-0.0.14/setup.cfg
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     1217 2024-04-29 10:06:57.000000 bagelML-0.0.14/setup.py
+drwxr-xr-x   0 rashedulhasanrijul   (501) staff       (20)        0 2024-04-29 10:07:22.525887 bagelML-0.0.14/test/
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)        0 2024-02-22 02:33:19.000000 bagelML-0.0.14/test/__init__.py
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     2717 2024-04-02 18:31:43.000000 bagelML-0.0.14/test/client_test.py
+-rw-r--r--   0 rashedulhasanrijul   (501) staff       (20)     2332 2024-02-22 02:33:19.000000 bagelML-0.0.14/test/opt_test.py
```

### Comparing `bagelML-0.0.13/PKG-INFO` & `bagelML-0.0.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagelML
-Version: 0.0.13
+Version: 0.0.14
 Summary: BagelML is a Python library for interacting with the Bagel inference and vector embedding API.
 Home-page: https://github.com/BagelNetwork/Client
 Author: Bidhan Roy
 Author-email: bidhan@bagel.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bagelML-0.0.13/README.md` & `bagelML-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.13/bagel/api/Cluster.py` & `bagelML-0.0.14/bagel/api/Cluster.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.13/bagel/api/__init__.py` & `bagelML-0.0.14/bagel/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -453,8 +453,18 @@
             self,
             dataset_id: str,
             file_path: Optional[str] = "",
             api_key: Optional[str] = None
     ) -> str:  
         """Download the full dataset."""
         pass
+    
+    @abstractmethod
+    def download_dataset_files(
+            self,
+            dataset_id: str, 
+            target_dir: str,
+            file_path: Optional[str] = "",
+            api_key: Optional[str] = None
+            ) -> bool:
+        pass
```

### Comparing `bagelML-0.0.13/bagel/api/fastapi.py` & `bagelML-0.0.14/bagel/api/fastapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -649,14 +649,52 @@
         # raise_bagel_error(resp)
         
         file_content = resp.content
         file_name = resp.headers.get('Content-Disposition', '').split('filename=')[1].strip('"')
         file_type = resp.headers.get('Content-Type', '')
         
         return file_content, file_name, file_type
+    
+    @override
+    def download_dataset_files(
+            self, 
+            dataset_id: str, 
+            target_dir: str,
+            file_path: Optional[str] = "",
+            api_key: Optional[str] = None
+            ) -> bool:
+        
+        headers = self._popuate_headers_with_api_key(api_key)
+
+        os.makedirs(target_dir, exist_ok=True)
+        
+        dataset_info = self.get_dataset_info(dataset_id, file_path)
+        file_types = ["file", "dir"]
+
+        dataset_id = dataset_info['dataset_id']
+        repo_info = dataset_info['repo_info']
+        files = repo_info['files']
+
+        for file_info in files:
+            file_path = file_info['path']
+            if file_info['type'] == file_types[0]:
+                file_content, file_name, file_type = self.download_dataset(
+                    dataset_id=dataset_id,
+                    file_path=file_path
+                )
+
+                file_path = os.path.join(target_dir, file_name)
+                with open(file_path, "wb") as file:
+                    file.write(file_content)
+
+            elif file_info['type'] == file_types[1]:
+                dataset_dir_info = self.get_dataset_info(dataset_id, file_path)
+                self.download_dataset_files(dataset_dir_info, target_dir)
+        
+        return True
 
 
 def raise_bagel_error(resp: requests.Response) -> None:
     """Raises an error if the response is not ok, using a BagelError if possible"""
     if resp.ok:
         return
```

### Comparing `bagelML-0.0.13/bagel/api/types.py` & `bagelML-0.0.14/bagel/api/types.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.13/bagel/config.py` & `bagelML-0.0.14/bagel/config.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.13/bagel/errors.py` & `bagelML-0.0.14/bagel/errors.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.13/bagelML.egg-info/PKG-INFO` & `bagelML-0.0.14/bagelML.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bagelML
-Version: 0.0.13
+Version: 0.0.14
 Summary: BagelML is a Python library for interacting with the Bagel inference and vector embedding API.
 Home-page: https://github.com/BagelNetwork/Client
 Author: Bidhan Roy
 Author-email: bidhan@bagel.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bagelML-0.0.13/setup.py` & `bagelML-0.0.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bagelML",
-    version="0.0.13",
+    version="0.0.14",
     description="BagelML is a Python library for interacting with the Bagel inference and vector embedding API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Bidhan Roy",
     author_email="bidhan@bagel.net",
     url="https://github.com/BagelNetwork/Client",
     packages=find_packages(),
```

### Comparing `bagelML-0.0.13/test/client_test.py` & `bagelML-0.0.14/test/client_test.py`

 * *Files identical despite different names*

### Comparing `bagelML-0.0.13/test/opt_test.py` & `bagelML-0.0.14/test/opt_test.py`

 * *Files identical despite different names*

