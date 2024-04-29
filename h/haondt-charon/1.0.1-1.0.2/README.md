# Comparing `tmp/haondt_charon-1.0.1.tar.gz` & `tmp/haondt_charon-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haondt_charon-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "haondt_charon-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `haondt_charon-1.0.1.tar` & `haondt_charon-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       39 2024-04-28 02:50:20.846986 haondt_charon-1.0.1/.gitignore
--rw-r--r--   0        0        0      169 2024-04-27 13:55:39.003551 haondt_charon-1.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0      196 2024-04-28 03:00:11.413730 haondt_charon-1.0.1/Dockerfile
--rw-r--r--   0        0        0     1081 2024-04-28 02:50:20.850987 haondt_charon-1.0.1/LICENSE
--rw-r--r--   0        0        0     5423 2024-04-28 02:50:20.850987 haondt_charon-1.0.1/README.md
--rw-r--r--   0        0        0     1054 2024-04-27 13:55:39.003551 haondt_charon-1.0.1/charon.yml
--rw-r--r--   0        0        0        0 2024-04-28 12:24:26.124303 haondt_charon-1.0.1/charon/__init__.py
--rw-r--r--   0        0        0     1395 2024-04-28 02:50:20.850987 haondt_charon-1.0.1/charon/__main__.py
--rw-r--r--   0        0        0       45 2024-04-28 02:50:20.850987 haondt_charon-1.0.1/charon/destinations/__init__.py
--rw-r--r--   0        0        0     1794 2024-04-28 02:50:20.850987 haondt_charon-1.0.1/charon/destinations/gcp_bucket.py
--rw-r--r--   0        0        0     1164 2024-04-28 02:50:20.850987 haondt_charon-1.0.1/charon/destinations/local.py
--rw-r--r--   0        0        0       50 2024-04-28 02:50:20.850987 haondt_charon-1.0.1/charon/requirements.txt
--rw-r--r--   0        0        0     2532 2024-04-28 02:50:20.850987 haondt_charon-1.0.1/charon/scheduling.py
--rw-r--r--   0        0        0     2369 2024-04-28 02:50:20.850987 haondt_charon-1.0.1/charon/shared.py
--rw-r--r--   0        0        0      107 2024-04-28 02:50:20.850987 haondt_charon-1.0.1/charon/sources/__init__.py
--rw-r--r--   0        0        0     2145 2024-04-28 02:50:20.850987 haondt_charon-1.0.1/charon/sources/http.py
--rw-r--r--   0        0        0     2010 2024-04-28 02:50:20.850987 haondt_charon-1.0.1/charon/sources/lib.py
--rw-r--r--   0        0        0     1350 2024-04-28 02:50:20.850987 haondt_charon-1.0.1/charon/sources/local.py
--rw-r--r--   0        0        0     1312 2024-04-28 02:50:20.850987 haondt_charon-1.0.1/charon/styx.py
--rw-r--r--   0        0        0      314 2024-04-27 14:17:35.041418 haondt_charon-1.0.1/docker-compose.yml
--rw-r--r--   0        0        0      367 2024-04-28 12:24:07.692114 haondt_charon-1.0.1/pipeline.yml
--rw-r--r--   0        0        0      632 2024-04-28 12:24:26.552308 haondt_charon-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      493 2024-04-28 02:50:20.850987 haondt_charon-1.0.1/tests/charon.test.yml
--rwxr-xr-x   0        0        0      561 2024-04-28 02:50:20.854987 haondt_charon-1.0.1/tests/test.sh
--rwxr-xr-x   0        0        0      787 2024-04-28 02:50:20.854987 haondt_charon-1.0.1/tests/test2.sh
--rw-r--r--   0        0        0     5828 1970-01-01 00:00:00.000000 haondt_charon-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-04-28 02:50:20.846986 haondt_charon-1.0.2/.gitignore
+-rw-r--r--   0        0        0      169 2024-04-27 13:55:39.003551 haondt_charon-1.0.2/.gitlab-ci.yml
+-rw-r--r--   0        0        0      196 2024-04-28 03:00:11.413730 haondt_charon-1.0.2/Dockerfile
+-rw-r--r--   0        0        0     1081 2024-04-28 02:50:20.850987 haondt_charon-1.0.2/LICENSE
+-rw-r--r--   0        0        0     5423 2024-04-28 02:50:20.850987 haondt_charon-1.0.2/README.md
+-rw-r--r--   0        0        0     1054 2024-04-27 13:55:39.003551 haondt_charon-1.0.2/charon.yml
+-rw-r--r--   0        0        0        0 2024-04-28 13:17:55.887544 haondt_charon-1.0.2/charon/__init__.py
+-rw-r--r--   0        0        0     1395 2024-04-28 02:50:20.850987 haondt_charon-1.0.2/charon/__main__.py
+-rw-r--r--   0        0        0       45 2024-04-28 02:50:20.850987 haondt_charon-1.0.2/charon/destinations/__init__.py
+-rw-r--r--   0        0        0     1794 2024-04-28 02:50:20.850987 haondt_charon-1.0.2/charon/destinations/gcp_bucket.py
+-rw-r--r--   0        0        0     1164 2024-04-28 02:50:20.850987 haondt_charon-1.0.2/charon/destinations/local.py
+-rw-r--r--   0        0        0       50 2024-04-28 02:50:20.850987 haondt_charon-1.0.2/charon/requirements.txt
+-rw-r--r--   0        0        0     2532 2024-04-28 02:50:20.850987 haondt_charon-1.0.2/charon/scheduling.py
+-rw-r--r--   0        0        0     2369 2024-04-28 02:50:20.850987 haondt_charon-1.0.2/charon/shared.py
+-rw-r--r--   0        0        0      107 2024-04-28 02:50:20.850987 haondt_charon-1.0.2/charon/sources/__init__.py
+-rw-r--r--   0        0        0     2145 2024-04-28 02:50:20.850987 haondt_charon-1.0.2/charon/sources/http.py
+-rw-r--r--   0        0        0     2010 2024-04-28 02:50:20.850987 haondt_charon-1.0.2/charon/sources/lib.py
+-rw-r--r--   0        0        0     1350 2024-04-28 02:50:20.850987 haondt_charon-1.0.2/charon/sources/local.py
+-rw-r--r--   0        0        0     1312 2024-04-28 02:50:20.850987 haondt_charon-1.0.2/charon/styx.py
+-rw-r--r--   0        0        0      314 2024-04-27 14:17:35.041418 haondt_charon-1.0.2/docker-compose.yml
+-rw-r--r--   0        0        0      465 2024-04-28 13:17:35.863272 haondt_charon-1.0.2/pipeline.yml
+-rw-r--r--   0        0        0      742 2024-04-28 13:17:56.311549 haondt_charon-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      493 2024-04-28 02:50:20.850987 haondt_charon-1.0.2/tests/charon.test.yml
+-rwxr-xr-x   0        0        0      561 2024-04-28 02:50:20.854987 haondt_charon-1.0.2/tests/test.sh
+-rwxr-xr-x   0        0        0      787 2024-04-28 02:50:20.854987 haondt_charon-1.0.2/tests/test2.sh
+-rw-r--r--   0        0        0     5968 1970-01-01 00:00:00.000000 haondt_charon-1.0.2/PKG-INFO
```

### Comparing `haondt_charon-1.0.1/LICENSE` & `haondt_charon-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.1/README.md` & `haondt_charon-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.1/charon.yml` & `haondt_charon-1.0.2/charon.yml`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.1/charon/__main__.py` & `haondt_charon-1.0.2/charon/__main__.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.1/charon/destinations/gcp_bucket.py` & `haondt_charon-1.0.2/charon/destinations/gcp_bucket.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.1/charon/destinations/local.py` & `haondt_charon-1.0.2/charon/destinations/local.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.1/charon/scheduling.py` & `haondt_charon-1.0.2/charon/scheduling.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.1/charon/shared.py` & `haondt_charon-1.0.2/charon/shared.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.1/charon/sources/http.py` & `haondt_charon-1.0.2/charon/sources/http.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.1/charon/sources/lib.py` & `haondt_charon-1.0.2/charon/sources/lib.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.1/charon/sources/local.py` & `haondt_charon-1.0.2/charon/sources/local.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.1/charon/styx.py` & `haondt_charon-1.0.2/charon/styx.py`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.1/pyproject.toml` & `haondt_charon-1.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 requires = [ "flit_core >=3.2,<4",]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "haondt_charon"
 classifiers = [ "License :: OSI Approved :: MIT License",]
 description = "charon is a utility for backing up data from one location to another at regular intervals."
-version = "1.0.1"
+version = "1.0.2"
 readme = "README.md"
 keywords = [ "backup", "recovery",]
+dependencies = [ "croniter>=2.0.5", "PyYAML>=6.0.1", "cryptography>=42.0.5", "google-cloud-storage>=2.16.0",]
 [[project.authors]]
 name = "haondt"
 
 [project.license]
 file = "LICENSE"
 
 [project.scripts]
```

### Comparing `haondt_charon-1.0.1/tests/test.sh` & `haondt_charon-1.0.2/tests/test.sh`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.1/tests/test2.sh` & `haondt_charon-1.0.2/tests/test2.sh`

 * *Files identical despite different names*

### Comparing `haondt_charon-1.0.1/PKG-INFO` & `haondt_charon-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 Metadata-Version: 2.1
 Name: haondt_charon
-Version: 1.0.1
+Version: 1.0.2
 Summary: charon is a utility for backing up data from one location to another at regular intervals.
 Keywords: backup,recovery
 Author: haondt
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
+Requires-Dist: croniter>=2.0.5
+Requires-Dist: PyYAML>=6.0.1
+Requires-Dist: cryptography>=42.0.5
+Requires-Dist: google-cloud-storage>=2.16.0
 Project-URL: Homepage, https://gitlab.com/haondt/charon
 Project-URL: Repository, https://gitlab.com/haondt/charon
 
 # charon
 
 charon is a utility for backing up data from one location to another at regular intervals.
```

