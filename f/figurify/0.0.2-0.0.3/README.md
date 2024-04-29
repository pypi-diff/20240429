# Comparing `tmp/figurify-0.0.2.tar.gz` & `tmp/figurify-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figurify-0.0.2.tar", last modified: Mon Apr 29 17:49:49 2024, max compression
+gzip compressed data, was "figurify-0.0.3.tar", last modified: Mon Apr 29 17:54:28 2024, max compression
```

## Comparing `figurify-0.0.2.tar` & `figurify-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 17:49:49.400425 figurify-0.0.2/
--rw-r--r--   0 julian    (1000) julian    (1000)     1068 2024-04-28 15:07:49.000000 figurify-0.0.2/LICENSE
--rw-r--r--   0 julian    (1000) julian    (1000)       60 2024-04-29 12:55:00.000000 figurify-0.0.2/MANIFEST.in
--rw-r--r--   0 julian    (1000) julian    (1000)    11525 2024-04-29 17:49:49.400425 figurify-0.0.2/PKG-INFO
--rw-r--r--   0 julian    (1000) julian    (1000)     1945 2024-04-29 16:03:47.000000 figurify-0.0.2/README.md
--rw-r--r--   0 julian    (1000) julian    (1000)        5 2024-04-29 17:46:37.000000 figurify-0.0.2/VERSION.txt
--rw-r--r--   0 julian    (1000) julian    (1000)    11005 2024-04-29 16:31:38.000000 figurify-0.0.2/documentation.md
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 17:49:49.400425 figurify-0.0.2/figurify/
--rw-r--r--   0 julian    (1000) julian    (1000)     1329 2024-04-28 16:20:13.000000 figurify-0.0.2/figurify/__init__.py
--rw-r--r--   0 julian    (1000) julian    (1000)      824 2024-04-28 06:24:04.000000 figurify-0.0.2/figurify/material_properties.py
--rw-r--r--   0 julian    (1000) julian    (1000)     2114 2024-04-28 06:52:47.000000 figurify-0.0.2/figurify/units.py
-drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 17:49:49.400425 figurify-0.0.2/figurify.egg-info/
--rw-r--r--   0 julian    (1000) julian    (1000)    11525 2024-04-29 17:49:49.000000 figurify-0.0.2/figurify.egg-info/PKG-INFO
--rw-r--r--   0 julian    (1000) julian    (1000)      266 2024-04-29 17:49:49.000000 figurify-0.0.2/figurify.egg-info/SOURCES.txt
--rw-r--r--   0 julian    (1000) julian    (1000)        1 2024-04-29 17:49:49.000000 figurify-0.0.2/figurify.egg-info/dependency_links.txt
--rw-r--r--   0 julian    (1000) julian    (1000)        9 2024-04-29 17:49:49.000000 figurify-0.0.2/figurify.egg-info/top_level.txt
--rw-r--r--   0 julian    (1000) julian    (1000)       38 2024-04-29 17:49:49.400425 figurify-0.0.2/setup.cfg
--rw-r--r--   0 julian    (1000) julian    (1000)      817 2024-04-29 16:02:25.000000 figurify-0.0.2/setup.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 17:54:28.483768 figurify-0.0.3/
+-rw-r--r--   0 julian    (1000) julian    (1000)     1068 2024-04-28 15:07:49.000000 figurify-0.0.3/LICENSE
+-rw-r--r--   0 julian    (1000) julian    (1000)       60 2024-04-29 12:55:00.000000 figurify-0.0.3/MANIFEST.in
+-rw-r--r--   0 julian    (1000) julian    (1000)    11470 2024-04-29 17:54:28.483768 figurify-0.0.3/PKG-INFO
+-rw-r--r--   0 julian    (1000) julian    (1000)     1945 2024-04-29 16:03:47.000000 figurify-0.0.3/README.md
+-rw-r--r--   0 julian    (1000) julian    (1000)        5 2024-04-29 17:53:44.000000 figurify-0.0.3/VERSION.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)    11005 2024-04-29 16:31:38.000000 figurify-0.0.3/documentation.md
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 17:54:28.483768 figurify-0.0.3/figurify/
+-rw-r--r--   0 julian    (1000) julian    (1000)     1329 2024-04-28 16:20:13.000000 figurify-0.0.3/figurify/__init__.py
+-rw-r--r--   0 julian    (1000) julian    (1000)      824 2024-04-28 06:24:04.000000 figurify-0.0.3/figurify/material_properties.py
+-rw-r--r--   0 julian    (1000) julian    (1000)     2114 2024-04-28 06:52:47.000000 figurify-0.0.3/figurify/units.py
+drwxr-xr-x   0 julian    (1000) julian    (1000)        0 2024-04-29 17:54:28.483768 figurify-0.0.3/figurify.egg-info/
+-rw-r--r--   0 julian    (1000) julian    (1000)    11470 2024-04-29 17:54:28.000000 figurify-0.0.3/figurify.egg-info/PKG-INFO
+-rw-r--r--   0 julian    (1000) julian    (1000)      266 2024-04-29 17:54:28.000000 figurify-0.0.3/figurify.egg-info/SOURCES.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)        1 2024-04-29 17:54:28.000000 figurify-0.0.3/figurify.egg-info/dependency_links.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)        9 2024-04-29 17:54:28.000000 figurify-0.0.3/figurify.egg-info/top_level.txt
+-rw-r--r--   0 julian    (1000) julian    (1000)       38 2024-04-29 17:54:28.483768 figurify-0.0.3/setup.cfg
+-rw-r--r--   0 julian    (1000) julian    (1000)      762 2024-04-29 17:52:07.000000 figurify-0.0.3/setup.py
```

### Comparing `figurify-0.0.2/LICENSE` & `figurify-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `figurify-0.0.2/PKG-INFO` & `figurify-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: figurify
-Version: 0.0.2
+Version: 0.0.3
 Summary: With figurify you can calculate figures, surfaces and physics.
-Home-page: https://github.com/julian-hess/Figurify.git
 Author: Julian Hess
 Project-URL: Source, https://github.com/julian-hess/Figurify.git
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
```

### Comparing `figurify-0.0.2/README.md` & `figurify-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `figurify-0.0.2/documentation.md` & `figurify-0.0.3/documentation.md`

 * *Files identical despite different names*

### Comparing `figurify-0.0.2/figurify/__init__.py` & `figurify-0.0.3/figurify/__init__.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.2/figurify/material_properties.py` & `figurify-0.0.3/figurify/material_properties.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.2/figurify/units.py` & `figurify-0.0.3/figurify/units.py`

 * *Files identical despite different names*

### Comparing `figurify-0.0.2/figurify.egg-info/PKG-INFO` & `figurify-0.0.3/figurify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Metadata-Version: 2.1
 Name: figurify
-Version: 0.0.2
+Version: 0.0.3
 Summary: With figurify you can calculate figures, surfaces and physics.
-Home-page: https://github.com/julian-hess/Figurify.git
 Author: Julian Hess
 Project-URL: Source, https://github.com/julian-hess/Figurify.git
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
```

### Comparing `figurify-0.0.2/setup.py` & `figurify-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 setup(
     name='figurify',
     version=get_version(),
     author='Julian Hess',
     description='With figurify you can calculate figures, surfaces and physics.',
     long_description=open("documentation.md").read(),
     long_description_content_type="text/markdown",
-    url='https://github.com/julian-hess/Figurify.git',
     packages=find_packages(),
     project_urls={
         "Source": "https://github.com/julian-hess/Figurify.git"
     },
     classifiers=[
         'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
```

