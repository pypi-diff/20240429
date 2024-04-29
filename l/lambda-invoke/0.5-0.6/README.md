# Comparing `tmp/lambda_invoke-0.5.tar.gz` & `tmp/lambda_invoke-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambda_invoke-0.5.tar", last modified: Tue Apr 16 15:37:28 2024, max compression
+gzip compressed data, was "lambda_invoke-0.6.tar", last modified: Mon Apr 29 15:43:35 2024, max compression
```

## Comparing `lambda_invoke-0.5.tar` & `lambda_invoke-0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tox       (1000) tox       (1000)        0 2024-04-16 15:37:28.534296 lambda_invoke-0.5/
--rw-r--r--   0 tox       (1000) tox       (1000)      156 2021-12-13 02:14:12.000000 lambda_invoke-0.5/AUTHORS.rst
--rw-r--r--   0 tox       (1000) tox       (1000)     1073 2021-12-13 02:31:40.000000 lambda_invoke-0.5/LICENSE
--rw-r--r--   0 tox       (1000) tox       (1000)     1637 2024-04-16 15:37:28.534296 lambda_invoke-0.5/PKG-INFO
--rw-r--r--   0 tox       (1000) tox       (1000)      471 2021-12-14 03:30:11.000000 lambda_invoke-0.5/README.rst
-drwxr-xr-x   0 tox       (1000) tox       (1000)        0 2024-04-16 15:37:28.534296 lambda_invoke-0.5/lambda_invoke/
--rw-r--r--   0 tox       (1000) tox       (1000)       70 2021-12-14 03:40:14.000000 lambda_invoke-0.5/lambda_invoke/__init__.py
--rw-r--r--   0 tox       (1000) tox       (1000)     4687 2024-04-16 15:23:10.000000 lambda_invoke-0.5/lambda_invoke/simple_proxy.py
-drwxr-xr-x   0 tox       (1000) tox       (1000)        0 2024-04-16 15:37:28.534296 lambda_invoke-0.5/lambda_invoke.egg-info/
--rw-r--r--   0 tox       (1000) tox       (1000)     1637 2024-04-16 15:37:28.000000 lambda_invoke-0.5/lambda_invoke.egg-info/PKG-INFO
--rw-r--r--   0 tox       (1000) tox       (1000)      358 2024-04-16 15:37:28.000000 lambda_invoke-0.5/lambda_invoke.egg-info/SOURCES.txt
--rw-r--r--   0 tox       (1000) tox       (1000)        1 2024-04-16 15:37:28.000000 lambda_invoke-0.5/lambda_invoke.egg-info/dependency_links.txt
--rw-r--r--   0 tox       (1000) tox       (1000)        1 2024-04-16 15:27:37.000000 lambda_invoke-0.5/lambda_invoke.egg-info/not-zip-safe
--rw-r--r--   0 tox       (1000) tox       (1000)       99 2024-04-16 15:37:28.000000 lambda_invoke-0.5/lambda_invoke.egg-info/requires.txt
--rw-r--r--   0 tox       (1000) tox       (1000)       14 2024-04-16 15:37:28.000000 lambda_invoke-0.5/lambda_invoke.egg-info/top_level.txt
--rw-r--r--   0 tox       (1000) tox       (1000)       90 2021-12-13 02:27:07.000000 lambda_invoke-0.5/pyproject.toml
--rw-r--r--   0 tox       (1000) tox       (1000)     1014 2024-04-16 15:37:28.534296 lambda_invoke-0.5/setup.cfg
-drwxr-xr-x   0 tox       (1000) tox       (1000)        0 2024-04-16 15:37:28.534296 lambda_invoke-0.5/tests/
--rw-r--r--   0 tox       (1000) tox       (1000)     7154 2024-04-16 15:23:10.000000 lambda_invoke-0.5/tests/test_simple_proxy.py
+drwxr-xr-x   0 tox       (1000) tox       (1000)        0 2024-04-29 15:43:35.286606 lambda_invoke-0.6/
+-rw-r--r--   0 tox       (1000) tox       (1000)      156 2021-12-13 02:14:12.000000 lambda_invoke-0.6/AUTHORS.rst
+-rw-r--r--   0 tox       (1000) tox       (1000)     1073 2021-12-13 02:31:40.000000 lambda_invoke-0.6/LICENSE
+-rw-r--r--   0 tox       (1000) tox       (1000)     1637 2024-04-29 15:43:35.286606 lambda_invoke-0.6/PKG-INFO
+-rw-r--r--   0 tox       (1000) tox       (1000)      471 2021-12-14 03:30:11.000000 lambda_invoke-0.6/README.rst
+drwxr-xr-x   0 tox       (1000) tox       (1000)        0 2024-04-29 15:43:35.282606 lambda_invoke-0.6/lambda_invoke/
+-rw-r--r--   0 tox       (1000) tox       (1000)       70 2021-12-14 03:40:14.000000 lambda_invoke-0.6/lambda_invoke/__init__.py
+-rw-r--r--   0 tox       (1000) tox       (1000)     4516 2024-04-29 15:37:54.000000 lambda_invoke-0.6/lambda_invoke/simple_proxy.py
+drwxr-xr-x   0 tox       (1000) tox       (1000)        0 2024-04-29 15:43:35.282606 lambda_invoke-0.6/lambda_invoke.egg-info/
+-rw-r--r--   0 tox       (1000) tox       (1000)     1637 2024-04-29 15:43:35.000000 lambda_invoke-0.6/lambda_invoke.egg-info/PKG-INFO
+-rw-r--r--   0 tox       (1000) tox       (1000)      358 2024-04-29 15:43:35.000000 lambda_invoke-0.6/lambda_invoke.egg-info/SOURCES.txt
+-rw-r--r--   0 tox       (1000) tox       (1000)        1 2024-04-29 15:43:35.000000 lambda_invoke-0.6/lambda_invoke.egg-info/dependency_links.txt
+-rw-r--r--   0 tox       (1000) tox       (1000)        1 2024-04-16 15:27:37.000000 lambda_invoke-0.6/lambda_invoke.egg-info/not-zip-safe
+-rw-r--r--   0 tox       (1000) tox       (1000)       99 2024-04-29 15:43:35.000000 lambda_invoke-0.6/lambda_invoke.egg-info/requires.txt
+-rw-r--r--   0 tox       (1000) tox       (1000)       14 2024-04-29 15:43:35.000000 lambda_invoke-0.6/lambda_invoke.egg-info/top_level.txt
+-rw-r--r--   0 tox       (1000) tox       (1000)       90 2021-12-13 02:27:07.000000 lambda_invoke-0.6/pyproject.toml
+-rw-r--r--   0 tox       (1000) tox       (1000)     1014 2024-04-29 15:43:35.286606 lambda_invoke-0.6/setup.cfg
+drwxr-xr-x   0 tox       (1000) tox       (1000)        0 2024-04-29 15:43:35.282606 lambda_invoke-0.6/tests/
+-rw-r--r--   0 tox       (1000) tox       (1000)     7251 2024-04-29 15:37:54.000000 lambda_invoke-0.6/tests/test_simple_proxy.py
```

### Comparing `lambda_invoke-0.5/LICENSE` & `lambda_invoke-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lambda_invoke-0.5/PKG-INFO` & `lambda_invoke-0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda-invoke
-Version: 0.5
+Version: 0.6
 Summary: Conveniently invoke lambda mimicking a proxy invocation
 Home-page: https://github.com/IlyaSukhanov/lambda-invoke
 Author: Ilya Sukhanov
 Author-email: ilya@sukhanov.net
 License: MIT license
 Keywords: aws,lambda-invoke
 Classifier: Intended Audience :: Developers
```

### Comparing `lambda_invoke-0.5/lambda_invoke/simple_proxy.py` & `lambda_invoke-0.6/lambda_invoke/simple_proxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,29 +70,22 @@
         host_parts = self.url.hostname.split(".")
         if len(host_parts) > 1:
             return f"{host_parts[-1]}:{host_parts[-2]}"
         return host_parts[0]
 
     @property
     def request_query_string(self):
-        qs = {
+        return {
             "queryStringParameters": {
-                key: value[0]
-                for key, value in parse_qs(self.url.query).items()
-                if len(value) == 1
-            }
+                key: value[0] for key, value in parse_qs(self.url.query).items()
+            },
+            "multiValueQueryStringParameters": {
+                key: value for key, value in parse_qs(self.url.query).items()
+            },
         }
-        multi_value_qs = {
-            key: value
-            for key, value in parse_qs(self.url.query).items()
-            if len(value) > 1
-        }
-        if multi_value_qs:
-            qs["multiValueQueryStringParameters"] = multi_value_qs
-        return qs
 
     @property
     def request_body(self):
         if not self.body:
             return False, None
         try:
             if isinstance(self.body, str):
```

### Comparing `lambda_invoke-0.5/lambda_invoke.egg-info/PKG-INFO` & `lambda_invoke-0.6/lambda_invoke.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda-invoke
-Version: 0.5
+Version: 0.6
 Summary: Conveniently invoke lambda mimicking a proxy invocation
 Home-page: https://github.com/IlyaSukhanov/lambda-invoke
 Author: Ilya Sukhanov
 Author-email: ilya@sukhanov.net
 License: MIT license
 Keywords: aws,lambda-invoke
 Classifier: Intended Audience :: Developers
```

### Comparing `lambda_invoke-0.5/setup.cfg` & `lambda_invoke-0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lambda-invoke
-version = 0.5
+version = 0.6
 author = Ilya Sukhanov
 author_email = ilya@sukhanov.net
 license = MIT license
 description = Conveniently invoke lambda mimicking a proxy invocation
 keywords = 
 	aws
 	lambda-invoke
```

### Comparing `lambda_invoke-0.5/tests/test_simple_proxy.py` & `lambda_invoke-0.6/tests/test_simple_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -113,40 +113,44 @@
         )
         response = proxy.send(self.mock_client)
         assert response.status_code == 200
         sent_payload = json.loads(
             self.mock_client.invoke.call_args.kwargs.get("Payload")
         )
         assert sent_payload.get("queryStringParameters") == {"a": "1", "b": "2"}
-        assert "multiValueQueryStringParameters" not in sent_payload.keys()
+        assert sent_payload.get("multiValueQueryStringParameters") == {
+            "a": ["1"],
+            "b": ["2"],
+        }
 
     def test_mix_multi_value_query_string(self):
         proxy = LambdaSimpleProxy(
             "us-east-1", "get", "http://example/?a=1&b=2&a=bob", {}, None
         )
         response = proxy.send(self.mock_client)
         assert response.status_code == 200
         sent_payload = json.loads(
             self.mock_client.invoke.call_args.kwargs.get("Payload")
         )
-        assert sent_payload.get("queryStringParameters") == {"b": "2"}
+        assert sent_payload.get("queryStringParameters") == {"a": "1", "b": "2"}
         assert sent_payload.get("multiValueQueryStringParameters") == {
-            "a": ["1", "bob"]
+            "a": ["1", "bob"],
+            "b": ["2"],
         }
 
     def test_only_multi_value_query_string(self):
         proxy = LambdaSimpleProxy(
             "us-east-1", "get", "http://example/?a=1&a=bob", {}, None
         )
         response = proxy.send(self.mock_client)
         assert response.status_code == 200
         sent_payload = json.loads(
             self.mock_client.invoke.call_args.kwargs.get("Payload")
         )
-        assert sent_payload.get("queryStringParameters") == {}
+        assert sent_payload.get("queryStringParameters") == {"a": "1"}
         assert sent_payload.get("multiValueQueryStringParameters") == {
             "a": ["1", "bob"]
         }
 
 
 class TestSimpleProxyAsync(IsolatedAsyncioTestCase):
     async def test_200_ok_async(self):
```

