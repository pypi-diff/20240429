# Comparing `tmp/trace_attributes-3.0.4.tar.gz` & `tmp/trace_attributes-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trace_attributes-3.0.4.tar", last modified: Sun Apr 28 02:18:20 2024, max compression
+gzip compressed data, was "trace_attributes-3.0.5.tar", last modified: Sun Apr 28 18:22:31 2024, max compression
```

## Comparing `trace_attributes-3.0.4.tar` & `trace_attributes-3.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:18:20.538860 trace_attributes-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-28 02:18:08.000000 trace_attributes-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-28 02:18:20.538860 trace_attributes-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    47682 2024-04-28 02:18:08.000000 trace_attributes-3.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 02:18:20.538860 trace_attributes-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-28 02:18:08.000000 trace_attributes-3.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:18:20.534860 trace_attributes-3.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:18:20.534860 trace_attributes-3.0.4/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:18:20.538860 trace_attributes-3.0.4/src/python/langtrace/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 02:18:08.000000 trace_attributes-3.0.4/src/python/langtrace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:18:20.538860 trace_attributes-3.0.4/src/python/langtrace/trace_attributes/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-28 02:18:08.000000 trace_attributes-3.0.4/src/python/langtrace/trace_attributes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:18:20.538860 trace_attributes-3.0.4/src/python/langtrace/trace_attributes/models/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 02:18:08.000000 trace_attributes-3.0.4/src/python/langtrace/trace_attributes/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-28 02:18:08.000000 trace_attributes-3.0.4/src/python/langtrace/trace_attributes/models/database_span_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-28 02:18:08.000000 trace_attributes-3.0.4/src/python/langtrace/trace_attributes/models/framework_span_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-28 02:18:08.000000 trace_attributes-3.0.4/src/python/langtrace/trace_attributes/models/llm_span_attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 02:18:20.538860 trace_attributes-3.0.4/src/python/trace_attributes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-28 02:18:20.000000 trace_attributes-3.0.4/src/python/trace_attributes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-28 02:18:20.000000 trace_attributes-3.0.4/src/python/trace_attributes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 02:18:20.000000 trace_attributes-3.0.4/src/python/trace_attributes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-28 02:18:20.000000 trace_attributes-3.0.4/src/python/trace_attributes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-28 02:18:20.000000 trace_attributes-3.0.4/src/python/trace_attributes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:22:31.308807 trace_attributes-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-28 18:22:15.000000 trace_attributes-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-28 18:22:31.308807 trace_attributes-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    47682 2024-04-28 18:22:15.000000 trace_attributes-3.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 18:22:31.308807 trace_attributes-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-28 18:22:15.000000 trace_attributes-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:22:31.304807 trace_attributes-3.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:22:31.304807 trace_attributes-3.0.5/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:22:31.304807 trace_attributes-3.0.5/src/python/langtrace/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 18:22:15.000000 trace_attributes-3.0.5/src/python/langtrace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:22:31.304807 trace_attributes-3.0.5/src/python/langtrace/trace_attributes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-28 18:22:15.000000 trace_attributes-3.0.5/src/python/langtrace/trace_attributes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:22:31.304807 trace_attributes-3.0.5/src/python/langtrace/trace_attributes/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-28 18:22:15.000000 trace_attributes-3.0.5/src/python/langtrace/trace_attributes/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-28 18:22:15.000000 trace_attributes-3.0.5/src/python/langtrace/trace_attributes/models/database_span_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-28 18:22:15.000000 trace_attributes-3.0.5/src/python/langtrace/trace_attributes/models/framework_span_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-28 18:22:15.000000 trace_attributes-3.0.5/src/python/langtrace/trace_attributes/models/llm_span_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 18:22:31.308807 trace_attributes-3.0.5/src/python/trace_attributes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-28 18:22:31.000000 trace_attributes-3.0.5/src/python/trace_attributes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-28 18:22:31.000000 trace_attributes-3.0.5/src/python/trace_attributes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 18:22:31.000000 trace_attributes-3.0.5/src/python/trace_attributes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-28 18:22:31.000000 trace_attributes-3.0.5/src/python/trace_attributes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-28 18:22:31.000000 trace_attributes-3.0.5/src/python/trace_attributes.egg-info/top_level.txt
```

### Comparing `trace_attributes-3.0.4/LICENSE` & `trace_attributes-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `trace_attributes-3.0.4/PKG-INFO` & `trace_attributes-3.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trace-attributes
-Version: 3.0.4
+Version: 3.0.5
 Summary: LangTrace - Trace Attributes
 Home-page: https://github.com/Scale3-Labs/langtrace-trace-attributes
 Author: Karthik Kalyanaraman
 Author-email: karthik@scale3labs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trace_attributes-3.0.4/README.md` & `trace_attributes-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `trace_attributes-3.0.4/setup.py` & `trace_attributes-3.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='trace-attributes',  # Choose a unique name for PyPI
-    version='3.0.4',
+    version='3.0.5',
     author='Karthik Kalyanaraman',
     author_email='karthik@scale3labs.com',
     description='LangTrace - Trace Attributes',
     long_description="LangTrace - Trace Attributes",
     long_description_content_type='text/markdown',
     url='https://github.com/Scale3-Labs/langtrace-trace-attributes',  # Project home page
     package_dir={'': 'src/python'},
```

### Comparing `trace_attributes-3.0.4/src/python/langtrace/trace_attributes/models/database_span_attributes.py` & `trace_attributes-3.0.5/src/python/langtrace/trace_attributes/models/database_span_attributes.py`

 * *Files identical despite different names*

### Comparing `trace_attributes-3.0.4/src/python/langtrace/trace_attributes/models/framework_span_attributes.py` & `trace_attributes-3.0.5/src/python/langtrace/trace_attributes/models/framework_span_attributes.py`

 * *Files identical despite different names*

### Comparing `trace_attributes-3.0.4/src/python/langtrace/trace_attributes/models/llm_span_attributes.py` & `trace_attributes-3.0.5/src/python/langtrace/trace_attributes/models/llm_span_attributes.py`

 * *Files identical despite different names*

### Comparing `trace_attributes-3.0.4/src/python/trace_attributes.egg-info/PKG-INFO` & `trace_attributes-3.0.5/src/python/trace_attributes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trace-attributes
-Version: 3.0.4
+Version: 3.0.5
 Summary: LangTrace - Trace Attributes
 Home-page: https://github.com/Scale3-Labs/langtrace-trace-attributes
 Author: Karthik Kalyanaraman
 Author-email: karthik@scale3labs.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trace_attributes-3.0.4/src/python/trace_attributes.egg-info/SOURCES.txt` & `trace_attributes-3.0.5/src/python/trace_attributes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

