# Comparing `tmp/altinn3_test_lib-0.0.7.tar.gz` & `tmp/altinn3_test_lib-0.0.8.tar.gz`

## Comparing `altinn3_test_lib-0.0.7.tar` & `altinn3_test_lib-0.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/CODEOWNERS
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/__init__.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/hello_test.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/plugins.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/fixtures/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/fixtures/factories/__init__.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/fixtures/factories/altinn_factory.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/fixtures/factories/file_factory.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/fixtures/factories/gcp_factories.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/fixtures/mocking/__init__.py
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/fixtures/mocking/environment_vars.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/fixtures/mocking/mock_assist.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/resources/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/resources/mocking.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/test_files/instance.json
--rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/test_files/instance_json_in.json
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/test_files/instance_json_out.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/test_files/simple_prefill.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/utils/__init__.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/src/altinn3_test_lib/utils/fileutils.py
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/LICENSE
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/README.md
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/CODEOWNERS
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/__init__.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/hello_test.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/plugins.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/fixtures/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/fixtures/factories/__init__.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/fixtures/factories/altinn_factory.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/fixtures/factories/file_factory.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/fixtures/factories/gcp_factories.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/fixtures/mocking/__init__.py
+-rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/fixtures/mocking/environment_vars.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/fixtures/mocking/mock_assist.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/resources/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/resources/mocking.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/test_files/instance.json
+-rw-r--r--   0        0        0     4316 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/test_files/instance_json_in.json
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/test_files/instance_json_out.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/test_files/simple_prefill.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/utils/__init__.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/src/altinn3_test_lib/utils/fileutils.py
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/LICENSE
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/README.md
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 altinn3_test_lib-0.0.8/PKG-INFO
```

### Comparing `altinn3_test_lib-0.0.7/src/altinn3_test_lib/plugins.py` & `altinn3_test_lib-0.0.8/src/altinn3_test_lib/plugins.py`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.7/src/altinn3_test_lib/fixtures/factories/altinn_factory.py` & `altinn3_test_lib-0.0.8/src/altinn3_test_lib/fixtures/factories/altinn_factory.py`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.7/src/altinn3_test_lib/fixtures/factories/file_factory.py` & `altinn3_test_lib-0.0.8/src/altinn3_test_lib/fixtures/factories/file_factory.py`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.7/src/altinn3_test_lib/fixtures/factories/gcp_factories.py` & `altinn3_test_lib-0.0.8/src/altinn3_test_lib/fixtures/factories/gcp_factories.py`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.7/src/altinn3_test_lib/fixtures/mocking/environment_vars.py` & `altinn3_test_lib-0.0.8/src/altinn3_test_lib/fixtures/mocking/environment_vars.py`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.7/src/altinn3_test_lib/fixtures/mocking/mock_assist.py` & `altinn3_test_lib-0.0.8/src/altinn3_test_lib/fixtures/mocking/mock_assist.py`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.7/src/altinn3_test_lib/test_files/instance.json` & `altinn3_test_lib-0.0.8/src/altinn3_test_lib/test_files/instance.json`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.7/src/altinn3_test_lib/test_files/instance_json_in.json` & `altinn3_test_lib-0.0.8/src/altinn3_test_lib/test_files/instance_json_in.json`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.7/src/altinn3_test_lib/test_files/instance_json_out.json` & `altinn3_test_lib-0.0.8/src/altinn3_test_lib/test_files/instance_json_out.json`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.7/src/altinn3_test_lib/test_files/simple_prefill.txt` & `altinn3_test_lib-0.0.8/src/altinn3_test_lib/test_files/simple_prefill.txt`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.7/.gitignore` & `altinn3_test_lib-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.7/LICENSE` & `altinn3_test_lib-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `altinn3_test_lib-0.0.7/pyproject.toml` & `altinn3_test_lib-0.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "altinn3-test-lib"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     { name="Anders Hagen", email="nhk@ssb.no" },
     { name="Rannveig Aasen", email="rsa@ssb.no" }
 ]
 description = "A POC project for modular test tools"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `altinn3_test_lib-0.0.7/PKG-INFO` & `altinn3_test_lib-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: altinn3-test-lib
-Version: 0.0.7
+Version: 0.0.8
 Summary: A POC project for modular test tools
 Author-email: Anders Hagen <nhk@ssb.no>, Rannveig Aasen <rsa@ssb.no>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
```

