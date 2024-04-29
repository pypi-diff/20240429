# Comparing `tmp/simple_aws_wrapper-2.7.5.tar.gz` & `tmp/simple_aws_wrapper-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aws_wrapper-2.7.5.tar", last modified: Tue Mar  5 15:03:20 2024, max compression
+gzip compressed data, was "simple_aws_wrapper-2.8.0.tar", last modified: Mon Apr 29 13:41:59 2024, max compression
```

## Comparing `simple_aws_wrapper-2.7.5.tar` & `simple_aws_wrapper-2.8.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:03:20.704501 simple_aws_wrapper-2.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-05 15:03:20.704501 simple_aws_wrapper-2.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-05 15:03:20.704501 simple_aws_wrapper-2.7.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:03:20.700501 simple_aws_wrapper-2.7.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:03:20.700501 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:03:20.704501 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/const/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/const/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/const/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/const/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:03:20.704501 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/exceptions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/resource_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:03:20.704501 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/services/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/services/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/services/parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/services/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/services/sqs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:03:20.704501 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-05 15:03:20.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-05 15:03:20.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 15:03:20.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-05 15:03:20.000000 simple_aws_wrapper-2.7.5/src/simple_aws_wrapper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:03:20.704501 simple_aws_wrapper-2.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/tests/test_dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/tests/test_parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-03-05 15:03:14.000000 simple_aws_wrapper-2.7.5/tests/test_s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:41:59.247840 simple_aws_wrapper-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-29 13:41:59.247840 simple_aws_wrapper-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-29 13:41:59.247840 simple_aws_wrapper-2.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:41:59.243839 simple_aws_wrapper-2.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:41:59.243839 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:41:59.247840 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/const/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/const/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/const/services.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:41:59.247840 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/exceptions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/resource_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:41:59.247840 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/services/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/services/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3349 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/services/parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7059 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/services/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/services/sqs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:41:59.247840 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-29 13:41:59.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-29 13:41:59.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:41:59.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 13:41:59.000000 simple_aws_wrapper-2.8.0/src/simple_aws_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:41:59.247840 simple_aws_wrapper-2.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/tests/test_dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/tests/test_parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-29 13:41:53.000000 simple_aws_wrapper-2.8.0/tests/test_s3.py
```

### Comparing `simple_aws_wrapper-2.7.5/LICENSE` & `simple_aws_wrapper-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_aws_wrapper-2.7.5/PKG-INFO` & `simple_aws_wrapper-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_aws_wrapper
-Version: 2.7.5
+Version: 2.8.0
 Summary: Implementazione minimale per la gestione delle risorse in cloud di AWS
 Author-email: Andrea Trupia <andrea.trupia.96@gmail.com>
 Project-URL: Homepage, https://github.com/AndreaTrupia/simple_aws_wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `simple_aws_wrapper-2.7.5/pyproject.toml` & `simple_aws_wrapper-2.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=40.8.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "simple_aws_wrapper"
-version = "2.7.5"
+version = "2.8.0"
 authors = [
     { name="Andrea Trupia", email="andrea.trupia.96@gmail.com"}
 ]
 description = "Implementazione minimale per la gestione delle risorse in cloud di AWS"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/config.py` & `simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,16 @@
         return self.__configured
 
     def set_region(self, region: Region):
         """
         Imposta la regione in cui si vuole utilizzare il ResourceManager
         :param region: regione in cui si vuole utilizzare il ResourceManager
         """
-        if not isinstance(region, Region):
-            raise TypeError("region must be a Region")
+        if not isinstance(region, Region) and isinstance(region, str):
+            region = Region(region)
         if region == "":
             raise ValueError("region cannot be empty")
         self.__region = region
         self.__configured = True
         return self
 
     def set_endpoint_url(self, endpoint_url: str | None):
```

### Comparing `simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/const/regions.py` & `simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/const/regions.py`

 * *Files identical despite different names*

### Comparing `simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/resource_manager.py` & `simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/resource_manager.py`

 * *Files identical despite different names*

### Comparing `simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/services/aws_lambda.py` & `simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/services/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/services/dynamodb.py` & `simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/services/dynamodb.py`

 * *Files identical despite different names*

### Comparing `simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/services/parameter_store.py` & `simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/services/parameter_store.py`

 * *Files identical despite different names*

### Comparing `simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/services/s3.py` & `simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/services/s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,8 +165,18 @@
             raise GenericException(traceback.format_exc())
 
     def bucket_exists(self, bucket_name: str) -> bool:
         try:
             self.client.head_bucket(Bucket=bucket_name)
             return True
         except Exception:
-            return False
+            return False
+
+    def list_object_keys(self, bucket_name: str) -> list[str]:
+        try:
+            result = self.client.list_objects(Bucket=bucket_name, Delimiter='/')
+            output_list: list[str] = []
+            for object in result["Contents"]:
+                output_list.append(object["Key"])
+            return output_list
+        except Exception:
+            return []
```

### Comparing `simple_aws_wrapper-2.7.5/src/simple_aws_wrapper/services/sqs.py` & `simple_aws_wrapper-2.8.0/src/simple_aws_wrapper/services/sqs.py`

 * *Files identical despite different names*

### Comparing `simple_aws_wrapper-2.7.5/src/simple_aws_wrapper.egg-info/PKG-INFO` & `simple_aws_wrapper-2.8.0/src/simple_aws_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_aws_wrapper
-Version: 2.7.5
+Version: 2.8.0
 Summary: Implementazione minimale per la gestione delle risorse in cloud di AWS
 Author-email: Andrea Trupia <andrea.trupia.96@gmail.com>
 Project-URL: Homepage, https://github.com/AndreaTrupia/simple_aws_wrapper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `simple_aws_wrapper-2.7.5/src/simple_aws_wrapper.egg-info/SOURCES.txt` & `simple_aws_wrapper-2.8.0/src/simple_aws_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_wrapper-2.7.5/tests/test_dynamodb.py` & `simple_aws_wrapper-2.8.0/tests/test_dynamodb.py`

 * *Files identical despite different names*

### Comparing `simple_aws_wrapper-2.7.5/tests/test_parameter_store.py` & `simple_aws_wrapper-2.8.0/tests/test_parameter_store.py`

 * *Files identical despite different names*

### Comparing `simple_aws_wrapper-2.7.5/tests/test_s3.py` & `simple_aws_wrapper-2.8.0/tests/test_s3.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
         ).set_aws_session_token(
             "test"
         )
         self.s3 = S3()
         self.bucket_name = f"test-bucket-{random.randint(0, 1000)}"
         self.test_string: str = "Hello World!"
         self.object_key = "test.txt"
+        self.object_key_for_listing = "test2.txt"
         self.destination_bucket_name = f"test-bucket-{random.randint(0, 1000)}"
         self.destination_object_key = "test-destination.txt"
 
     def test_put_object(self):
         self.s3.create_bucket(self.bucket_name)
         upload_status: bool = self.s3.put_object(
             self.test_string, self.bucket_name, self.object_key
@@ -91,8 +92,15 @@
         self.s3.delete_object(self.bucket_name, self.object_key)
         self.s3.delete_bucket(self.bucket_name)
 
     def test_bucket_exists(self):
         self.s3.create_bucket(self.bucket_name)
         self.assertTrue(self.s3.bucket_exists(self.bucket_name))
         self.s3.delete_bucket(self.bucket_name)
-        self.assertFalse(self.s3.bucket_exists(self.bucket_name))
+        self.assertFalse(self.s3.bucket_exists(self.bucket_name))
+
+    def test_list_objects(self):
+        self.s3.create_bucket(self.bucket_name)
+        self.s3.put_object(self.test_string, bucket_name=self.bucket_name, object_key=self.object_key)
+        self.s3.put_object(self.test_string, bucket_name=self.bucket_name, object_key=self.object_key_for_listing)
+        object_key_list: list[str] = self.s3.list_object_keys(self.bucket_name)
+        self.assertTrue(self.object_key in object_key_list and self.object_key_for_listing in object_key_list)
```

