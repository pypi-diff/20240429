# Comparing `tmp/OpenGeodeWeb-Back-4.0.0rc1.tar.gz` & `tmp/opengeodeweb_back-4.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenGeodeWeb-Back-4.0.0rc1.tar", last modified: Wed Feb 28 15:21:07 2024, max compression
+gzip compressed data, was "opengeodeweb_back-4.1.0rc1.tar", last modified: Mon Apr 29 12:53:53 2024, max compression
```

## Comparing `OpenGeodeWeb-Back-4.0.0rc1.tar` & `opengeodeweb_back-4.1.0rc1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:21:07.182220 OpenGeodeWeb-Back-4.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-02-28 15:21:07.182220 OpenGeodeWeb-Back-4.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-02-28 15:20:53.000000 OpenGeodeWeb-Back-4.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 15:21:07.182220 OpenGeodeWeb-Back-4.0.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:21:07.178220 OpenGeodeWeb-Back-4.0.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:21:07.182220 OpenGeodeWeb-Back-4.0.0rc1/src/OpenGeodeWeb_Back.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-02-28 15:21:07.000000 OpenGeodeWeb-Back-4.0.0rc1/src/OpenGeodeWeb_Back.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-02-28 15:21:07.000000 OpenGeodeWeb-Back-4.0.0rc1/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 15:21:07.000000 OpenGeodeWeb-Back-4.0.0rc1/src/OpenGeodeWeb_Back.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-28 15:21:07.000000 OpenGeodeWeb-Back-4.0.0rc1/src/OpenGeodeWeb_Back.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-28 15:21:07.000000 OpenGeodeWeb-Back-4.0.0rc1/src/OpenGeodeWeb_Back.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:21:07.178220 OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/geode_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    20319 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/geode_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    15911 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/inspector_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:21:07.182220 OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/routes/
--rw-r--r--   0 runner    (1001) docker     (127)     5189 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/routes/blueprint_routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:21:07.182220 OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/routes/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/routes/schemas/allowed_files.json
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/routes/schemas/allowed_objects.json
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/routes/schemas/geode_objects_and_output_extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/routes/schemas/geographic_coordinate_systems.json
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/routes/schemas/missing_files.json
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/routes/schemas/upload_file.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 15:21:07.182220 OpenGeodeWeb-Back-4.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    12428 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-02-28 15:20:52.000000 OpenGeodeWeb-Back-4.0.0rc1/tests/test_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:53.632957 opengeodeweb_back-4.1.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-29 12:53:53.628957 opengeodeweb_back-4.1.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-29 12:53:45.000000 opengeodeweb_back-4.1.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:53:53.632957 opengeodeweb_back-4.1.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:53.624957 opengeodeweb_back-4.1.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:53.628957 opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-29 12:53:53.000000 opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-29 12:53:53.000000 opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:53:53.000000 opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-29 12:53:53.000000 opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 12:53:53.000000 opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:53.628957 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/geode_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20286 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/geode_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:53.628957 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/blueprint_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:53.628957 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/allowed_files.json
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/allowed_objects.json
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/geode_objects_and_output_extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/geographic_coordinate_systems.json
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/inspect_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/missing_files.json
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/schemas/upload_file.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:53:53.628957 opengeodeweb_back-4.1.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14349 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-29 12:53:39.000000 opengeodeweb_back-4.1.0rc1/tests/test_routes.py
```

### Comparing `OpenGeodeWeb-Back-4.0.0rc1/LICENSE` & `opengeodeweb_back-4.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Back-4.0.0rc1/PKG-INFO` & `opengeodeweb_back-4.1.0rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Back
-Version: 4.0.0rc1
+Version: 4.1.0rc1
 Summary: OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 Author-email: Geode-solutions <team-web@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Back
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Back/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: asgiref==3.7.2
+Requires-Dist: asgiref==3.8.1
 Requires-Dist: attrs==23.2.0
-Requires-Dist: blinker==1.7.0
+Requires-Dist: blinker==1.8.1
 Requires-Dist: click==8.1.7
-Requires-Dist: colorama==0.4.6
-Requires-Dist: flask[async]==3.0.1
+Requires-Dist: flask[async]==3.0.3
 Requires-Dist: flask-cors==4.0.0
-Requires-Dist: geode-background==7.7.1
-Requires-Dist: geode-common==30.1.2
-Requires-Dist: geode-conversion==5.2.1
-Requires-Dist: geode-explicit==4.4.3
-Requires-Dist: geode-implicit==2.6.1
-Requires-Dist: geode-numerics==4.3.0
-Requires-Dist: geode-simplex==6.5.1
-Requires-Dist: geode-viewables==2.2.0
-Requires-Dist: importlib-metadata==7.0.1
-Requires-Dist: itsdangerous==2.1.2
+Requires-Dist: geode-background==7.9.8
+Requires-Dist: geode-common==31.0.8
+Requires-Dist: geode-conversion==5.2.8
+Requires-Dist: geode-explicit==4.7.5
+Requires-Dist: geode-implicit==2.8.6
+Requires-Dist: geode-numerics==4.3.3
+Requires-Dist: geode-simplex==6.7.4
+Requires-Dist: geode-viewables==2.2.2
+Requires-Dist: itsdangerous==2.2.0
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: jsonschema==4.21.1
 Requires-Dist: jsonschema-specifications==2023.12.1
-Requires-Dist: markupsafe==2.1.4
-Requires-Dist: opengeode-core==14.13.2
-Requires-Dist: opengeode-geosciences==7.4.0
-Requires-Dist: opengeode-geosciencesio==4.6.0
-Requires-Dist: opengeode-inspector==4.0.6
-Requires-Dist: opengeode-io==6.4.0
-Requires-Dist: referencing==0.33.0
-Requires-Dist: rpds-py==0.17.1
-Requires-Dist: typing-extensions==4.9.0
-Requires-Dist: werkzeug==3.0.1
-Requires-Dist: zipp==3.17.0
+Requires-Dist: markupsafe==2.1.5
+Requires-Dist: opengeode-core==14.19.2
+Requires-Dist: opengeode-geosciences==7.6.4
+Requires-Dist: opengeode-geosciencesio==4.7.6
+Requires-Dist: opengeode-inspector==5.1.3
+Requires-Dist: opengeode-io==6.5.1
+Requires-Dist: referencing==0.35.0
+Requires-Dist: rpds-py==0.18.0
+Requires-Dist: werkzeug==3.0.2
 
 <h1 align="center">OpenGeodeWeb-Back<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">OpenSource Python framework based on OpenGeode</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeodeWeb-Back/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/OpenGeodeWeb-Back/workflows/CD/badge.svg" alt="Deploy Status">
```

### Comparing `OpenGeodeWeb-Back-4.0.0rc1/README.md` & `opengeodeweb_back-4.1.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `OpenGeodeWeb-Back-4.0.0rc1/pyproject.toml` & `opengeodeweb_back-4.1.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "OpenGeodeWeb-Back"
-version = "4.0.0-rc.1"
+version = "4.1.0-rc.1"
 dynamic = ["dependencies"]
 authors = [
   { name="Geode-solutions", email="team-web@geode-solutions.com" },
 ]
 description = "OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `OpenGeodeWeb-Back-4.0.0rc1/src/OpenGeodeWeb_Back.egg-info/PKG-INFO` & `opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 Metadata-Version: 2.1
 Name: OpenGeodeWeb-Back
-Version: 4.0.0rc1
+Version: 4.1.0rc1
 Summary: OpenGeodeWeb-Back is an open source framework that proposes handy python functions and wrappers for the OpenGeode ecosystem
 Author-email: Geode-solutions <team-web@geode-solutions.com>
 Project-URL: Homepage, https://github.com/Geode-solutions/OpenGeodeWeb-Back
 Project-URL: Bug Tracker, https://github.com/Geode-solutions/OpenGeodeWeb-Back/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: asgiref==3.7.2
+Requires-Dist: asgiref==3.8.1
 Requires-Dist: attrs==23.2.0
-Requires-Dist: blinker==1.7.0
+Requires-Dist: blinker==1.8.1
 Requires-Dist: click==8.1.7
-Requires-Dist: colorama==0.4.6
-Requires-Dist: flask[async]==3.0.1
+Requires-Dist: flask[async]==3.0.3
 Requires-Dist: flask-cors==4.0.0
-Requires-Dist: geode-background==7.7.1
-Requires-Dist: geode-common==30.1.2
-Requires-Dist: geode-conversion==5.2.1
-Requires-Dist: geode-explicit==4.4.3
-Requires-Dist: geode-implicit==2.6.1
-Requires-Dist: geode-numerics==4.3.0
-Requires-Dist: geode-simplex==6.5.1
-Requires-Dist: geode-viewables==2.2.0
-Requires-Dist: importlib-metadata==7.0.1
-Requires-Dist: itsdangerous==2.1.2
+Requires-Dist: geode-background==7.9.8
+Requires-Dist: geode-common==31.0.8
+Requires-Dist: geode-conversion==5.2.8
+Requires-Dist: geode-explicit==4.7.5
+Requires-Dist: geode-implicit==2.8.6
+Requires-Dist: geode-numerics==4.3.3
+Requires-Dist: geode-simplex==6.7.4
+Requires-Dist: geode-viewables==2.2.2
+Requires-Dist: itsdangerous==2.2.0
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: jsonschema==4.21.1
 Requires-Dist: jsonschema-specifications==2023.12.1
-Requires-Dist: markupsafe==2.1.4
-Requires-Dist: opengeode-core==14.13.2
-Requires-Dist: opengeode-geosciences==7.4.0
-Requires-Dist: opengeode-geosciencesio==4.6.0
-Requires-Dist: opengeode-inspector==4.0.6
-Requires-Dist: opengeode-io==6.4.0
-Requires-Dist: referencing==0.33.0
-Requires-Dist: rpds-py==0.17.1
-Requires-Dist: typing-extensions==4.9.0
-Requires-Dist: werkzeug==3.0.1
-Requires-Dist: zipp==3.17.0
+Requires-Dist: markupsafe==2.1.5
+Requires-Dist: opengeode-core==14.19.2
+Requires-Dist: opengeode-geosciences==7.6.4
+Requires-Dist: opengeode-geosciencesio==4.7.6
+Requires-Dist: opengeode-inspector==5.1.3
+Requires-Dist: opengeode-io==6.5.1
+Requires-Dist: referencing==0.35.0
+Requires-Dist: rpds-py==0.18.0
+Requires-Dist: werkzeug==3.0.2
 
 <h1 align="center">OpenGeodeWeb-Back<sup><i>by Geode-solutions</i></sup></h1>
 <h3 align="center">OpenSource Python framework based on OpenGeode</h3>
 
 <p align="center">
   <img src="https://github.com/Geode-solutions/OpenGeodeWeb-Back/workflows/CI/badge.svg" alt="Build Status">
   <img src="https://github.com/Geode-solutions/OpenGeodeWeb-Back/workflows/CD/badge.svg" alt="Deploy Status">
```

### Comparing `OpenGeodeWeb-Back-4.0.0rc1/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt` & `opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 src/OpenGeodeWeb_Back.egg-info/SOURCES.txt
 src/OpenGeodeWeb_Back.egg-info/dependency_links.txt
 src/OpenGeodeWeb_Back.egg-info/requires.txt
 src/OpenGeodeWeb_Back.egg-info/top_level.txt
 src/opengeodeweb_back/__init__.py
 src/opengeodeweb_back/geode_functions.py
 src/opengeodeweb_back/geode_objects.py
-src/opengeodeweb_back/inspector_functions.py
 src/opengeodeweb_back/routes/blueprint_routes.py
 src/opengeodeweb_back/routes/schemas/allowed_files.json
 src/opengeodeweb_back/routes/schemas/allowed_objects.json
 src/opengeodeweb_back/routes/schemas/geode_objects_and_output_extensions.json
 src/opengeodeweb_back/routes/schemas/geographic_coordinate_systems.json
+src/opengeodeweb_back/routes/schemas/inspect_file.json
 src/opengeodeweb_back/routes/schemas/missing_files.json
 src/opengeodeweb_back/routes/schemas/upload_file.json
 tests/test_functions.py
 tests/test_routes.py
```

### Comparing `OpenGeodeWeb-Back-4.0.0rc1/src/OpenGeodeWeb_Back.egg-info/requires.txt` & `opengeodeweb_back-4.1.0rc1/src/OpenGeodeWeb_Back.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,27 @@
-asgiref==3.7.2
+asgiref==3.8.1
 attrs==23.2.0
-blinker==1.7.0
+blinker==1.8.1
 click==8.1.7
-colorama==0.4.6
-flask[async]==3.0.1
+flask[async]==3.0.3
 flask-cors==4.0.0
-geode-background==7.7.1
-geode-common==30.1.2
-geode-conversion==5.2.1
-geode-explicit==4.4.3
-geode-implicit==2.6.1
-geode-numerics==4.3.0
-geode-simplex==6.5.1
-geode-viewables==2.2.0
-importlib-metadata==7.0.1
-itsdangerous==2.1.2
+geode-background==7.9.8
+geode-common==31.0.8
+geode-conversion==5.2.8
+geode-explicit==4.7.5
+geode-implicit==2.8.6
+geode-numerics==4.3.3
+geode-simplex==6.7.4
+geode-viewables==2.2.2
+itsdangerous==2.2.0
 jinja2==3.1.3
 jsonschema==4.21.1
 jsonschema-specifications==2023.12.1
-markupsafe==2.1.4
-opengeode-core==14.13.2
-opengeode-geosciences==7.4.0
-opengeode-geosciencesio==4.6.0
-opengeode-inspector==4.0.6
-opengeode-io==6.4.0
-referencing==0.33.0
-rpds-py==0.17.1
-typing-extensions==4.9.0
-werkzeug==3.0.1
-zipp==3.17.0
+markupsafe==2.1.5
+opengeode-core==14.19.2
+opengeode-geosciences==7.6.4
+opengeode-geosciencesio==4.7.6
+opengeode-inspector==5.1.3
+opengeode-io==6.5.1
+referencing==0.35.0
+rpds-py==0.18.0
+werkzeug==3.0.2
```

### Comparing `OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/geode_functions.py` & `opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/geode_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     return geode_object_value(geode_object)["is_3D"]
 
 
 def is_viewable(geode_object: str):
     return geode_object_value(geode_object)["is_viewable"]
 
 
-def inspector(geode_object: str, data):
+def inspect(geode_object: str, data):
     return geode_object_value(geode_object)["inspector"](data)
 
 
 def save_viewable(geode_object: str, data, folder_absolute_path: str, id: str):
     return geode_object_value(geode_object)["save_viewable"](
         data, os.path.join(folder_absolute_path, id)
     )
@@ -170,14 +170,40 @@
         parent_geode_object = geode_object_value(geode_object)["parent"]
         geode_objects_output_extensions_dict.update(
             geode_objects_output_extensions(parent_geode_object, data)
         )
     return geode_objects_output_extensions_dict
 
 
+def get_inspector_children(obj):
+    new_object = {}
+
+    if "inspection_type" in dir(obj):
+        new_object["title"] = obj.inspection_type()
+        new_object["nb_issues"] = 0
+        new_object["children"] = []
+        for child in dir(obj):
+            if not child.startswith("__") and not child in [
+                "inspection_type",
+                "string",
+            ]:
+                child_instance = obj.__getattribute__(child)
+                child_object = get_inspector_children(child_instance)
+                new_object["children"].append(child_object)
+                new_object["nb_issues"] += child_object["nb_issues"]
+    else:
+        new_object["title"] = obj.description()
+        nb_issues = obj.nb_issues()
+        new_object["nb_issues"] = nb_issues
+        if nb_issues > 0:
+            issues = obj.string().split("\n")
+            new_object["issues"] = issues
+    return new_object
+
+
 def versions(list_packages: list):
     list_with_versions = []
     for package in list_packages:
         list_with_versions.append(
             {
                 "package": package,
                 "version": pkg_resources.get_distribution(package).version,
```

### Comparing `OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/geode_objects.py` & `opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/geode_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                 "convert": og_gs.convert_brep_coordinate_reference_system,
                 "create": og.create_brep_coordinate_system,
             },
             "is_model": True,
             "is_3D": True,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_brep,
-            "inspector": og_inspector.BRepInspector,
+            "inspector": og_inspector.inspect_brep,
         },
         "CrossSection": {
             "parent": "Section",
             "input_factory": og_gs.CrossSectionInputFactory,
             "output_factory": og_gs.CrossSectionOutputFactory,
             "missing_files": og_gs.check_cross_section_missing_files,
             "is_loadable": og_gs.is_cross_section_loadable,
@@ -43,15 +43,15 @@
                 "convert": og_gs.convert_section_coordinate_reference_system,
                 "create": og.create_section_coordinate_system,
             },
             "is_model": True,
             "is_3D": False,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_cross_section,
-            "inspector": og_inspector.SectionInspector,
+            "inspector": og_inspector.inspect_section,
         },
         "EdgedCurve2D": {
             "input_factory": og.EdgedCurveInputFactory2D,
             "output_factory": og.EdgedCurveOutputFactory2D,
             "missing_files": og.check_edged_curve_missing_files2D,
             "is_loadable": og.is_edged_curve_loadable2D,
             "load": og.load_edged_curve2D,
@@ -63,15 +63,15 @@
                 "convert": og_gs.convert_edged_curve_coordinate_reference_system2D,
                 "create": og.create_edged_curve_coordinate_system2D,
             },
             "is_model": False,
             "is_3D": False,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_edged_curve2D,
-            "inspector": og_inspector.EdgedCurveInspector2D,
+            "inspector": og_inspector.inspect_edgedcurve2D,
         },
         "EdgedCurve3D": {
             "input_factory": og.EdgedCurveInputFactory3D,
             "output_factory": og.EdgedCurveOutputFactory3D,
             "missing_files": og.check_edged_curve_missing_files3D,
             "is_loadable": og.is_edged_curve_loadable3D,
             "load": og.load_edged_curve3D,
@@ -83,15 +83,15 @@
                 "convert": og_gs.convert_edged_curve_coordinate_reference_system3D,
                 "create": og.create_edged_curve_coordinate_system3D,
             },
             "is_model": False,
             "is_3D": True,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_edged_curve3D,
-            "inspector": og_inspector.EdgedCurveInspector3D,
+            "inspector": og_inspector.inspect_edgedcurve3D,
         },
         "Graph": {
             "input_factory": og.GraphInputFactory,
             "output_factory": og.GraphOutputFactory,
             "missing_files": og.check_graph_missing_files,
             "is_loadable": og.is_graph_loadable,
             "load": og.load_graph,
@@ -116,15 +116,15 @@
                 "convert": og_gs.convert_solid_mesh_coordinate_reference_system3D,
                 "create": og.create_solid_mesh_coordinate_system3D,
             },
             "is_model": False,
             "is_3D": True,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_hybrid_solid3D,
-            "inspector": og_inspector.SolidMeshInspector3D,
+            "inspector": og_inspector.inspect_solid3D,
         },
         "LightRegularGrid2D": {
             "input_factory": og.LightRegularGridInputFactory2D,
             "output_factory": og.LightRegularGridOutputFactory2D,
             "missing_files": og.check_light_regular_grid_missing_files2D,
             "is_loadable": og.is_light_regular_grid_loadable2D,
             "load": og.load_light_regular_grid2D,
@@ -162,15 +162,15 @@
                 "convert": og_gs.convert_point_set_coordinate_reference_system2D,
                 "create": og.create_point_set_coordinate_system2D,
             },
             "is_model": False,
             "is_3D": False,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_point_set2D,
-            "inspector": og_inspector.PointSetInspector2D,
+            "inspector": og_inspector.inspect_pointset2D,
         },
         "PointSet3D": {
             "input_factory": og.PointSetInputFactory3D,
             "output_factory": og.PointSetOutputFactory3D,
             "missing_files": og.check_point_set_missing_files3D,
             "is_loadable": og.is_point_set_loadable3D,
             "load": og.load_point_set3D,
@@ -182,15 +182,15 @@
                 "convert": og_gs.convert_point_set_coordinate_reference_system3D,
                 "create": og.create_point_set_coordinate_system3D,
             },
             "is_model": False,
             "is_3D": True,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_point_set3D,
-            "inspector": og_inspector.PointSetInspector3D,
+            "inspector": og_inspector.inspect_pointset3D,
         },
         "PolygonalSurface2D": {
             "input_factory": og.PolygonalSurfaceInputFactory2D,
             "output_factory": og.PolygonalSurfaceOutputFactory2D,
             "missing_files": og.check_polygonal_surface_missing_files2D,
             "is_loadable": og.is_polygonal_surface_loadable2D,
             "load": og.load_polygonal_surface2D,
@@ -202,15 +202,15 @@
                 "convert": og_gs.convert_surface_mesh_coordinate_reference_system2D,
                 "create": og.create_surface_mesh_coordinate_system2D,
             },
             "is_model": False,
             "is_3D": False,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_polygonal_surface2D,
-            "inspector": og_inspector.SurfaceMeshInspector2D,
+            "inspector": og_inspector.inspect_surface2D,
         },
         "PolygonalSurface3D": {
             "input_factory": og.PolygonalSurfaceInputFactory3D,
             "output_factory": og.PolygonalSurfaceOutputFactory3D,
             "missing_files": og.check_polygonal_surface_missing_files3D,
             "is_loadable": og.is_polygonal_surface_loadable3D,
             "load": og.load_polygonal_surface3D,
@@ -222,15 +222,15 @@
                 "convert": og_gs.convert_surface_mesh_coordinate_reference_system3D,
                 "create": og.create_surface_mesh_coordinate_system3D,
             },
             "is_model": False,
             "is_3D": True,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_polygonal_surface3D,
-            "inspector": og_inspector.SurfaceMeshInspector3D,
+            "inspector": og_inspector.inspect_surface3D,
         },
         "PolyhedralSolid3D": {
             "input_factory": og.PolyhedralSolidInputFactory3D,
             "output_factory": og.PolyhedralSolidOutputFactory3D,
             "missing_files": og.check_polyhedral_solid_missing_files3D,
             "is_loadable": og.is_polyhedral_solid_loadable3D,
             "load": og.load_polyhedral_solid3D,
@@ -242,15 +242,15 @@
                 "convert": og_gs.convert_solid_mesh_coordinate_reference_system3D,
                 "create": og.create_solid_mesh_coordinate_system3D,
             },
             "is_model": False,
             "is_3D": True,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_polyhedral_solid3D,
-            "inspector": og_inspector.SolidMeshInspector3D,
+            "inspector": og_inspector.inspect_solid3D,
         },
         "RasterImage2D": {
             "input_factory": og.RasterImageInputFactory2D,
             "output_factory": og.RasterImageOutputFactory2D,
             "missing_files": og.check_raster_image_missing_files2D,
             "is_loadable": og.is_raster_image_loadable2D,
             "load": og.load_raster_image2D,
@@ -326,15 +326,15 @@
                 "convert": og_gs.convert_section_coordinate_reference_system,
                 "create": og.create_section_coordinate_system,
             },
             "is_model": True,
             "is_3D": False,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_section,
-            "inspector": og_inspector.SectionInspector,
+            "inspector": og_inspector.inspect_section,
         },
         "StructuralModel": {
             "parent": "BRep",
             "input_factory": og_gs.StructuralModelInputFactory,
             "output_factory": og_gs.StructuralModelOutputFactory,
             "missing_files": og_gs.check_structural_model_missing_files,
             "is_loadable": og_gs.is_structural_model_loadable,
@@ -347,15 +347,15 @@
                 "convert": og_gs.convert_brep_coordinate_reference_system,
                 "create": og.create_brep_coordinate_system,
             },
             "is_model": True,
             "is_3D": True,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_structural_model,
-            "inspector": og_inspector.BRepInspector,
+            "inspector": og_inspector.inspect_brep,
         },
         "TetrahedralSolid3D": {
             "input_factory": og.TetrahedralSolidInputFactory3D,
             "output_factory": og.TetrahedralSolidOutputFactory3D,
             "missing_files": og.check_tetrahedral_solid_missing_files3D,
             "is_loadable": og.is_tetrahedral_solid_loadable3D,
             "load": og.load_tetrahedral_solid3D,
@@ -367,15 +367,15 @@
                 "convert": og_gs.convert_solid_mesh_coordinate_reference_system3D,
                 "create": og.create_solid_mesh_coordinate_system3D,
             },
             "is_model": False,
             "is_3D": True,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_tetrahedral_solid3D,
-            "inspector": og_inspector.SolidMeshInspector3D,
+            "inspector": og_inspector.inspect_solid3D,
         },
         "TriangulatedSurface2D": {
             "input_factory": og.TriangulatedSurfaceInputFactory2D,
             "output_factory": og.TriangulatedSurfaceOutputFactory2D,
             "missing_files": og.check_triangulated_surface_missing_files2D,
             "is_loadable": og.is_triangulated_surface_loadable2D,
             "load": og.load_triangulated_surface2D,
@@ -387,15 +387,15 @@
                 "convert": og_gs.convert_surface_mesh_coordinate_reference_system2D,
                 "create": og.create_surface_mesh_coordinate_system2D,
             },
             "is_model": False,
             "is_3D": False,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_triangulated_surface2D,
-            "inspector": og_inspector.TriangulatedSurfaceInspector2D,
+            "inspector": og_inspector.inspect_triangulated_surface2D,
         },
         "TriangulatedSurface3D": {
             "input_factory": og.TriangulatedSurfaceInputFactory3D,
             "output_factory": og.TriangulatedSurfaceOutputFactory3D,
             "missing_files": og.check_triangulated_surface_missing_files3D,
             "is_loadable": og.is_triangulated_surface_loadable3D,
             "load": og.load_triangulated_surface3D,
@@ -407,15 +407,15 @@
                 "convert": og_gs.convert_surface_mesh_coordinate_reference_system3D,
                 "create": og.create_surface_mesh_coordinate_system3D,
             },
             "is_model": False,
             "is_3D": True,
             "is_viewable": True,
             "save_viewable": g_v.save_viewable_triangulated_surface3D,
-            "inspector": og_inspector.TriangulatedSurfaceInspector3D,
+            "inspector": og_inspector.inspect_triangulated_surface3D,
         },
         "VertexSet": {
             "input_factory": og.VertexSetInputFactory,
             "output_factory": og.VertexSetOutputFactory,
             "missing_files": og.check_vertex_set_missing_files,
             "is_loadable": og.is_vertex_set_loadable,
             "load": og.load_vertex_set,
```

### Comparing `OpenGeodeWeb-Back-4.0.0rc1/src/opengeodeweb_back/routes/blueprint_routes.py` & `opengeodeweb_back-4.1.0rc1/src/opengeodeweb_back/routes/blueprint_routes.py`

 * *Files 8% similar despite different names*

```diff
@@ -147,14 +147,39 @@
         crs["authority"] = info.authority
         crs_list.append(crs)
 
     return flask.make_response({"crs_list": crs_list}, 200)
 
 
 with open(
+    os.path.join(schemas, "inspect_file.json"),
+    "r",
+) as file:
+    inspect_file_json = json.load(file)
+
+
+@routes.route(
+    inspect_file_json["route"],
+    methods=inspect_file_json["methods"],
+)
+def inspect_file():
+    UPLOAD_FOLDER = flask.current_app.config["UPLOAD_FOLDER"]
+    geode_functions.validate_request(flask.request, inspect_file_json)
+
+    secure_filename = werkzeug.utils.secure_filename(flask.request.json["filename"])
+    file_path = os.path.abspath(os.path.join(UPLOAD_FOLDER, secure_filename))
+    data = geode_functions.load(flask.request.json["input_geode_object"], file_path)
+    class_inspector = geode_functions.inspect(
+        flask.request.json["input_geode_object"], data
+    )
+    inspection_result = geode_functions.get_inspector_children(class_inspector)
+    return flask.make_response({"inspection_result": inspection_result}, 200)
+
+
+with open(
     os.path.join(schemas, "geode_objects_and_output_extensions.json"),
     "r",
 ) as file:
     geode_objects_and_output_extensions_json = json.load(file)
 
 
 @routes.route(
```

### Comparing `OpenGeodeWeb-Back-4.0.0rc1/tests/test_functions.py` & `opengeodeweb_back-4.1.0rc1/tests/test_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import os
 import uuid
 from src.opengeodeweb_back import geode_functions, geode_objects
 
 
+data_folder = os.path.join(os.path.dirname(__file__), "data")
+
+
 def test_geode_object_value():
     for geode_object, value in geode_objects.geode_objects_dict().items():
         geode_object_value = geode_functions.geode_object_value(geode_object)
         assert type(geode_object_value) is dict
 
 
 def test_input_factory():
@@ -35,15 +38,15 @@
             assert type(output) is str
 
 
 def test_missing_files():
     for geode_object, value in geode_objects.geode_objects_dict().items():
         input_extensions = geode_functions.geode_object_input_extensions(geode_object)
         for input_extension in input_extensions:
-            file_absolute_path = os.path.abspath(f"tests/data/test.{input_extension}")
+            file_absolute_path = os.path.join(data_folder, f"test.{input_extension}")
             missing_files = geode_functions.missing_files(
                 geode_object, file_absolute_path
             )
             has_missing_files = missing_files.has_missing_files()
             assert type(has_missing_files) is bool
             mandatory_files = missing_files.mandatory_files
             assert type(mandatory_files) is list
@@ -51,37 +54,37 @@
             assert type(additional_files) is list
 
 
 def test_is_loadable():
     for geode_object, value in geode_objects.geode_objects_dict().items():
         input_extensions = geode_functions.geode_object_input_extensions(geode_object)
         for input_extension in input_extensions:
-            file_absolute_path = os.path.abspath(f"tests/data/test.{input_extension}")
+            file_absolute_path = os.path.join(data_folder, f"test.{input_extension}")
             is_loadable = geode_functions.is_loadable(geode_object, file_absolute_path)
             assert type(is_loadable) is bool
 
 
 def test_load():
     for geode_object, value in geode_objects.geode_objects_dict().items():
         print(f"\n{geode_object=}")
         input_extensions = geode_functions.geode_object_input_extensions(geode_object)
         for input_extension in input_extensions:
             print(f"\t{input_extension=}")
+            file_absolute_path = os.path.join(data_folder, f"test.{input_extension}")
             missing_files = geode_functions.missing_files(
-                geode_object, f"tests/data/test.{input_extension}"
+                geode_object, file_absolute_path
             )
             has_missing_files = missing_files.has_missing_files()
             if has_missing_files:
                 mandatory_files = missing_files.mandatory_files
                 print(f"\t\t{mandatory_files=}")
                 additional_files = missing_files.additional_files
                 print(f"\t\t{additional_files=}")
-            file_apsolute_path = os.path.abspath(f"tests/data/test.{input_extension}")
-            if geode_functions.is_loadable(geode_object, file_apsolute_path):
-                data = geode_functions.load(geode_object, file_apsolute_path)
+            if geode_functions.is_loadable(geode_object, file_absolute_path):
+                data = geode_functions.load(geode_object, file_absolute_path)
                 if "save_viewable" in value:
                     uu_id = str(uuid.uuid4()).replace("-", "")
                     viewable_file_path = geode_functions.save_viewable(
                         geode_object,
                         data,
                         os.path.abspath(f"./output"),
                         uu_id,
@@ -145,24 +148,25 @@
 
 def test_geode_object_output_extensions():
     for geode_object, value in geode_objects.geode_objects_dict().items():
         print(f"\n{geode_object=}")
         input_extensions = geode_functions.geode_object_input_extensions(geode_object)
         for input_extension in input_extensions:
             print(f"\t{input_extension=}")
+            file_absolute_path = os.path.join(data_folder, f"test.{input_extension}")
             missing_files = geode_functions.missing_files(
-                geode_object, f"tests/data/test.{input_extension}"
+                geode_object, file_absolute_path
             )
             has_missing_files = missing_files.has_missing_files()
             if has_missing_files:
                 mandatory_files = missing_files.mandatory_files
                 print(f"\t\t{mandatory_files=}")
                 additional_files = missing_files.additional_files
                 print(f"\t\t{additional_files=}")
-            file_absolute_path = os.path.abspath(f"tests/data/test.{input_extension}")
+            file_absolute_path = os.path.join(data_folder, f"test.{input_extension}")
             if geode_functions.is_loadable(geode_object, file_absolute_path):
                 data = geode_functions.load(geode_object, file_absolute_path)
                 geode_objets_and_output_extensions = (
                     geode_functions.geode_objects_output_extensions(geode_object, data)
                 )
                 assert type(geode_objets_and_output_extensions) is dict
                 for (
@@ -173,14 +177,50 @@
                         output_extension,
                         output_extension_value,
                     ) in output_geode_object_value.items():
                         assert type(output_extension) is str
                         assert type(output_extension_value["is_saveable"]) is bool
 
 
+def test_get_inspector_children():
+    for geode_object, value in geode_objects.geode_objects_dict().items():
+        if "inspector" in value:
+            print(f"\n{geode_object=}", flush=True)
+            input_extensions = geode_functions.geode_object_input_extensions(
+                geode_object
+            )
+            for input_extension in input_extensions:
+                print(f"\t{input_extension=}", flush=True)
+                file_absolute_path = os.path.join(
+                    data_folder, f"test.{input_extension}"
+                )
+                missing_files = geode_functions.missing_files(
+                    geode_object, file_absolute_path
+                )
+                has_missing_files = missing_files.has_missing_files()
+                if has_missing_files:
+                    mandatory_files = missing_files.mandatory_files
+                    print(f"\t\t{mandatory_files=}", flush=True)
+                    additional_files = missing_files.additional_files
+                    print(f"\t\t{additional_files=}", flush=True)
+                file_absolute_path = os.path.join(
+                    data_folder, f"test.{input_extension}"
+                )
+                if geode_functions.is_loadable(geode_object, file_absolute_path):
+                    data = geode_functions.load(geode_object, file_absolute_path)
+                    class_inspector = geode_functions.inspect(geode_object, data)
+                    assert "InspectionResult" in class_inspector.__class__.__name__
+                    inspection_result = geode_functions.get_inspector_children(
+                        class_inspector
+                    )
+
+                    print(f"\t\t{inspection_result=}", flush=True)
+                    assert type(inspection_result) is dict
+
+
 def test_filter_geode_objects():
     filters_list = ["", "crs", "inspector", None]
 
     for filter in filters_list:
         geode_objects_filtered_list = geode_functions.filter_geode_objects(filter)
         assert type(geode_objects_filtered_list) is list
         for geode_object in geode_objects_filtered_list:
@@ -223,16 +263,16 @@
     for test in test_list:
         key = test["key"]
         invalid_geode_objects = test["invalid_geode_objects"]
 
         input_extensions = geode_functions.list_input_extensions(key)
         for geode_object, value in geode_objects.geode_objects_dict().items():
             for input_extension in input_extensions:
-                file_absolute_path = os.path.abspath(
-                    f"tests/data/test.{input_extension}"
+                file_absolute_path = os.path.join(
+                    data_folder, f"test.{input_extension}"
                 )
                 return_dict = geode_functions.list_geode_objects(
                     file_absolute_path, key
                 )
                 assert type(return_dict) is dict
 
                 if key != None:
@@ -250,15 +290,15 @@
                             assert type(input_extension_value) is bool
 
 
 def test_geode_objects_output_extensions():
     for geode_object, value in geode_objects.geode_objects_dict().items():
         input_extensions = geode_functions.geode_object_input_extensions(geode_object)
         for input_extension in input_extensions:
-            file_absolute_path = f"tests/data/test.{input_extension}"
+            file_absolute_path = os.path.join(data_folder, f"test.{input_extension}")
             if geode_functions.is_loadable(geode_object, file_absolute_path):
                 data = geode_functions.load(geode_object, file_absolute_path)
                 geode_objects_and_output_extensions = (
                     geode_functions.geode_objects_output_extensions(geode_object, data)
                 )
                 assert type(geode_objects_and_output_extensions) is dict
                 for (
```

### Comparing `OpenGeodeWeb-Back-4.0.0rc1/tests/test_routes.py` & `opengeodeweb_back-4.1.0rc1/tests/test_routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -96,14 +96,40 @@
     assert response.status_code == 400
     error_message = response.json["description"]
     assert (
         error_message == "Validation error: 'input_geode_object' is a required property"
     )
 
 
+def test_inspect_file(client):
+    route = f"/inspect_file"
+
+    def get_full_data():
+        return {
+            "input_geode_object": "BRep",
+            "filename": "corbi.og_brep",
+        }
+
+    json = get_full_data()
+
+    # Normal test with geode_object 'BRep'
+    response = client.post(route, json=json)
+    assert response.status_code == 200
+    inspection_result = response.json["inspection_result"]
+    assert type(inspection_result) is dict
+
+    for key, value in get_full_data().items():
+        json = get_full_data()
+        json.pop(key)
+        response = client.post(route, json=json)
+        assert response.status_code == 400
+        error_description = response.json["description"]
+        assert error_description == f"Validation error: '{key}' is a required property"
+
+
 def test_geode_objects_and_output_extensions(client):
     route = "/geode_objects_and_output_extensions"
 
     def get_full_data():
         return {
             "input_geode_object": "BRep",
             "filename": "corbi.og_brep",
```

