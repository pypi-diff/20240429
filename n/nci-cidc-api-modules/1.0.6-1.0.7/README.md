# Comparing `tmp/nci_cidc_api_modules-1.0.6.tar.gz` & `tmp/nci_cidc_api_modules-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nci_cidc_api_modules-1.0.6.tar", last modified: Thu Apr 18 15:13:23 2024, max compression
+gzip compressed data, was "nci_cidc_api_modules-1.0.7.tar", last modified: Mon Apr 29 20:05:03 2024, max compression
```

## Comparing `nci_cidc_api_modules-1.0.6.tar` & `nci_cidc_api_modules-1.0.7.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.391672 nci_cidc_api_modules-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    40323 2024-04-18 15:13:23.387672 nci_cidc_api_modules-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    39309 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.383672 nci_cidc_api_modules-1.0.6/cidc_api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.383672 nci_cidc_api_modules-1.0.6/cidc_api/config/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/config/db.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/config/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/config/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/config/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.383672 nci_cidc_api_modules-1.0.6/cidc_api/csms/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/csms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/csms/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.387672 nci_cidc_api_modules-1.0.6/cidc_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31664 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/csms_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.387672 nci_cidc_api_modules-1.0.6/cidc_api/models/files/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62309 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/files/details.py
--rw-r--r--   0 runner    (1001) docker     (127)    29172 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/files/facets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)   120820 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/models/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.387672 nci_cidc_api_modules-1.0.6/cidc_api/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/shared/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/shared/emails.py
--rw-r--r--   0 runner    (1001) docker     (127)    33746 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/shared/gcloud_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/cidc_api/shared/rest_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.387672 nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40323 2024-04-18 15:13:23.000000 nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-18 15:13:23.000000 nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:13:23.000000 nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 15:13:23.000000 nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-18 15:13:23.000000 nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 15:13:23.000000 nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/requirements.modules.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 15:13:23.391672 nci_cidc_api_modules-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 15:13:23.387672 nci_cidc_api_modules-1.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    17127 2024-04-18 15:13:16.000000 nci_cidc_api_modules-1.0.6/tests/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:05:03.492677 nci_cidc_api_modules-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    40323 2024-04-29 20:05:03.492677 nci_cidc_api_modules-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    39309 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:05:03.484677 nci_cidc_api_modules-1.0.7/cidc_api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:05:03.488677 nci_cidc_api_modules-1.0.7/cidc_api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/config/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/config/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/config/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/config/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:05:03.488677 nci_cidc_api_modules-1.0.7/cidc_api/csms/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/csms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/csms/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:05:03.488677 nci_cidc_api_modules-1.0.7/cidc_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31664 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/models/csms_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:05:03.488677 nci_cidc_api_modules-1.0.7/cidc_api/models/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/models/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62309 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/models/files/details.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29172 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/models/files/facets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/models/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120820 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/models/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:05:03.492677 nci_cidc_api_modules-1.0.7/cidc_api/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11647 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/shared/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/shared/emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33746 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/shared/gcloud_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/cidc_api/shared/rest_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:05:03.492677 nci_cidc_api_modules-1.0.7/nci_cidc_api_modules.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40323 2024-04-29 20:05:03.000000 nci_cidc_api_modules-1.0.7/nci_cidc_api_modules.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-29 20:05:03.000000 nci_cidc_api_modules-1.0.7/nci_cidc_api_modules.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:05:03.000000 nci_cidc_api_modules-1.0.7/nci_cidc_api_modules.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 20:05:03.000000 nci_cidc_api_modules-1.0.7/nci_cidc_api_modules.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-29 20:05:03.000000 nci_cidc_api_modules-1.0.7/nci_cidc_api_modules.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 20:05:03.000000 nci_cidc_api_modules-1.0.7/nci_cidc_api_modules.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/requirements.modules.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 20:05:03.492677 nci_cidc_api_modules-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 20:05:03.492677 nci_cidc_api_modules-1.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    17127 2024-04-29 20:04:59.000000 nci_cidc_api_modules-1.0.7/tests/test_api.py
```

### Comparing `nci_cidc_api_modules-1.0.6/LICENSE` & `nci_cidc_api_modules-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/PKG-INFO` & `nci_cidc_api_modules-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_api_modules
-Version: 1.0.6
+Version: 1.0.7
 Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
 Home-page: https://github.com/NCI-CIDC/cidc-api-gae
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: werkzeug==2.3.8
@@ -21,15 +21,15 @@
 Requires-Dist: google-api-python-client==2.64.0
 Requires-Dist: packaging>=20.0.0
 Requires-Dist: pyarrow==14.0.1
 Requires-Dist: pandas<2,>=1
 Requires-Dist: python-dotenv==0.10.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: jinja2==3.1.3
-Requires-Dist: nci-cidc-schemas==0.26.29
+Requires-Dist: nci-cidc-schemas==0.26.32
 
 # NCI CIDC API <!-- omit in TOC -->
 
 The next generation of the CIDC API, reworked to use Google Cloud-managed services. This API is built with the Flask REST API framework backed by Google Cloud SQL, running on Google App Engine.
 
 ## Development <!-- omit in TOC -->
```

### Comparing `nci_cidc_api_modules-1.0.6/README.md` & `nci_cidc_api_modules-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/cidc_api/config/db.py` & `nci_cidc_api_modules-1.0.7/cidc_api/config/db.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/cidc_api/config/logging.py` & `nci_cidc_api_modules-1.0.7/cidc_api/config/logging.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/cidc_api/config/secrets.py` & `nci_cidc_api_modules-1.0.7/cidc_api/config/secrets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/cidc_api/config/settings.py` & `nci_cidc_api_modules-1.0.7/cidc_api/config/settings.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/cidc_api/csms/auth.py` & `nci_cidc_api_modules-1.0.7/cidc_api/csms/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/cidc_api/models/csms_api.py` & `nci_cidc_api_modules-1.0.7/cidc_api/models/csms_api.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/cidc_api/models/files/details.py` & `nci_cidc_api_modules-1.0.7/cidc_api/models/files/details.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/cidc_api/models/files/facets.py` & `nci_cidc_api_modules-1.0.7/cidc_api/models/files/facets.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/cidc_api/models/migrations.py` & `nci_cidc_api_modules-1.0.7/cidc_api/models/migrations.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/cidc_api/models/models.py` & `nci_cidc_api_modules-1.0.7/cidc_api/models/models.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/cidc_api/models/schemas.py` & `nci_cidc_api_modules-1.0.7/cidc_api/models/schemas.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/cidc_api/shared/auth.py` & `nci_cidc_api_modules-1.0.7/cidc_api/shared/auth.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/cidc_api/shared/emails.py` & `nci_cidc_api_modules-1.0.7/cidc_api/shared/emails.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/cidc_api/shared/gcloud_client.py` & `nci_cidc_api_modules-1.0.7/cidc_api/shared/gcloud_client.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/cidc_api/shared/rest_utils.py` & `nci_cidc_api_modules-1.0.7/cidc_api/shared/rest_utils.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/PKG-INFO` & `nci_cidc_api_modules-1.0.7/nci_cidc_api_modules.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nci_cidc_api_modules
-Version: 1.0.6
+Version: 1.0.7
 Summary: SQLAlchemy data models and configuration tools used in the NCI CIDC API
 Home-page: https://github.com/NCI-CIDC/cidc-api-gae
 License: MIT license
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: werkzeug==2.3.8
@@ -21,15 +21,15 @@
 Requires-Dist: google-api-python-client==2.64.0
 Requires-Dist: packaging>=20.0.0
 Requires-Dist: pyarrow==14.0.1
 Requires-Dist: pandas<2,>=1
 Requires-Dist: python-dotenv==0.10.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: jinja2==3.1.3
-Requires-Dist: nci-cidc-schemas==0.26.29
+Requires-Dist: nci-cidc-schemas==0.26.32
 
 # NCI CIDC API <!-- omit in TOC -->
 
 The next generation of the CIDC API, reworked to use Google Cloud-managed services. This API is built with the Flask REST API framework backed by Google Cloud SQL, running on Google App Engine.
 
 ## Development <!-- omit in TOC -->
```

### Comparing `nci_cidc_api_modules-1.0.6/nci_cidc_api_modules.egg-info/SOURCES.txt` & `nci_cidc_api_modules-1.0.7/nci_cidc_api_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/pyproject.toml` & `nci_cidc_api_modules-1.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/setup.py` & `nci_cidc_api_modules-1.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `nci_cidc_api_modules-1.0.6/tests/test_api.py` & `nci_cidc_api_modules-1.0.7/tests/test_api.py`

 * *Files identical despite different names*

