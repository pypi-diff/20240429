# Comparing `tmp/label-studio-tools-0.0.3.tar.gz` & `tmp/label-studio-tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/label-studio-tools-0.0.3.tar", last modified: Fri Aug 25 01:13:01 2023, max compression
+gzip compressed data, was "dist/label-studio-tools-0.0.4.tar", last modified: Mon Apr 29 12:32:33 2024, max compression
```

## Comparing `label-studio-tools-0.0.3.tar` & `label-studio-tools-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 01:13:01.000000 label-studio-tools-0.0.3/
--rwxr-xr-x   0 runner    (1001) docker     (999)    11341 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)       25 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)      507 2023-08-25 01:13:01.000000 label-studio-tools-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)       33 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 01:13:01.000000 label-studio-tools-0.0.3/label_studio_tools/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/label_studio_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 01:13:01.000000 label-studio-tools-0.0.3/label_studio_tools/core/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/label_studio_tools/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5757 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/label_studio_tools/core/label_config.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 01:13:01.000000 label-studio-tools-0.0.3/label_studio_tools/core/utils/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/label_studio_tools/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)       66 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/label_studio_tools/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (999)     3989 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/label_studio_tools/core/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (999)     1244 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/label_studio_tools/core/utils/params.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 01:13:01.000000 label-studio-tools-0.0.3/label_studio_tools/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/label_studio_tools/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3490 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/label_studio_tools/postprocessing/video.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 01:13:01.000000 label-studio-tools-0.0.3/label_studio_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/label_studio_tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4353 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/label_studio_tools/tests/test_core_label_config.py
--rw-r--r--   0 runner    (1001) docker     (999)    14391 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/label_studio_tools/tests/test_postprocessing_video.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 01:13:01.000000 label-studio-tools-0.0.3/label_studio_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)      507 2023-08-25 01:13:01.000000 label-studio-tools-0.0.3/label_studio_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      764 2023-08-25 01:13:01.000000 label-studio-tools-0.0.3/label_studio_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-25 01:13:01.000000 label-studio-tools-0.0.3/label_studio_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       27 2023-08-25 01:13:01.000000 label-studio-tools-0.0.3/label_studio_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       19 2023-08-25 01:13:01.000000 label-studio-tools-0.0.3/label_studio_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)       26 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-25 01:13:01.000000 label-studio-tools-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)      956 2023-08-25 01:12:47.000000 label-studio-tools-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:32:33.000000 label-studio-tools-0.0.4/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11341 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-29 12:32:33.000000 label-studio-tools-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:32:33.000000 label-studio-tools-0.0.4/label_studio_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/label_studio_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:32:33.000000 label-studio-tools-0.0.4/label_studio_tools/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/label_studio_tools/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/label_studio_tools/core/label_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:32:33.000000 label-studio-tools-0.0.4/label_studio_tools/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/label_studio_tools/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/label_studio_tools/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/label_studio_tools/core/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/label_studio_tools/core/utils/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:32:33.000000 label-studio-tools-0.0.4/label_studio_tools/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/label_studio_tools/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/label_studio_tools/postprocessing/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:32:33.000000 label-studio-tools-0.0.4/label_studio_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/label_studio_tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/label_studio_tools/tests/test_core_label_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/label_studio_tools/tests/test_get_local_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14391 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/label_studio_tools/tests/test_postprocessing_video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:32:33.000000 label-studio-tools-0.0.4/label_studio_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-29 12:32:33.000000 label-studio-tools-0.0.4/label_studio_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-29 12:32:33.000000 label-studio-tools-0.0.4/label_studio_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:32:33.000000 label-studio-tools-0.0.4/label_studio_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 12:32:33.000000 label-studio-tools-0.0.4/label_studio_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 12:32:33.000000 label-studio-tools-0.0.4/label_studio_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:32:33.000000 label-studio-tools-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-29 12:32:18.000000 label-studio-tools-0.0.4/setup.py
```

### Comparing `label-studio-tools-0.0.3/LICENSE` & `label-studio-tools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `label-studio-tools-0.0.3/label_studio_tools/core/label_config.py` & `label-studio-tools-0.0.4/label_studio_tools/core/label_config.py`

 * *Files identical despite different names*

### Comparing `label-studio-tools-0.0.3/label_studio_tools/core/utils/params.py` & `label-studio-tools-0.0.4/label_studio_tools/core/utils/params.py`

 * *Files identical despite different names*

### Comparing `label-studio-tools-0.0.3/label_studio_tools/postprocessing/video.py` & `label-studio-tools-0.0.4/label_studio_tools/postprocessing/video.py`

 * *Files identical despite different names*

### Comparing `label-studio-tools-0.0.3/label_studio_tools/tests/test_core_label_config.py` & `label-studio-tools-0.0.4/label_studio_tools/tests/test_core_label_config.py`

 * *Files identical despite different names*

### Comparing `label-studio-tools-0.0.3/label_studio_tools/tests/test_postprocessing_video.py` & `label-studio-tools-0.0.4/label_studio_tools/tests/test_postprocessing_video.py`

 * *Files identical despite different names*

### Comparing `label-studio-tools-0.0.3/label_studio_tools.egg-info/SOURCES.txt` & `label-studio-tools-0.0.4/label_studio_tools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 label_studio_tools/core/utils/exceptions.py
 label_studio_tools/core/utils/io.py
 label_studio_tools/core/utils/params.py
 label_studio_tools/postprocessing/__init__.py
 label_studio_tools/postprocessing/video.py
 label_studio_tools/tests/__init__.py
 label_studio_tools/tests/test_core_label_config.py
+label_studio_tools/tests/test_get_local_path.py
 label_studio_tools/tests/test_postprocessing_video.py
```

### Comparing `label-studio-tools-0.0.3/setup.py` & `label-studio-tools-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Module dependencies
 requirements_file = os.path.join(os.path.dirname(__file__), 'requirements.txt')
 with open(requirements_file, 'r') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name='label-studio-tools',
-    version='0.0.3',
+    version='0.0.4',
     author='Heartex',
     author_email="hello@heartex.ai",
     description='Label studio common tools',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/heartexlabs/label-studio-tools',
     packages=setuptools.find_packages(),
```

