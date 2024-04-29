# Comparing `tmp/cdklabs.aws_data_solutions_framework-1.5.0.tar.gz` & `tmp/cdklabs.aws_data_solutions_framework-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.aws_data_solutions_framework-1.5.0.tar", last modified: Fri Apr 19 16:15:58 2024, max compression
+gzip compressed data, was "cdklabs.aws_data_solutions_framework-1.6.0.tar", last modified: Mon Apr 29 17:40:15 2024, max compression
```

## Comparing `cdklabs.aws_data_solutions_framework-1.5.0.tar` & `cdklabs.aws_data_solutions_framework-1.6.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:15:58.535133 cdklabs.aws_data_solutions_framework-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-04-19 16:15:48.000000 cdklabs.aws_data_solutions_framework-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-19 16:15:48.000000 cdklabs.aws_data_solutions_framework-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-19 16:15:58.535133 cdklabs.aws_data_solutions_framework-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-19 16:15:48.000000 cdklabs.aws_data_solutions_framework-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-19 16:15:48.000000 cdklabs.aws_data_solutions_framework-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 16:15:58.535133 cdklabs.aws_data_solutions_framework-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-19 16:15:48.000000 cdklabs.aws_data_solutions_framework-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:15:58.523133 cdklabs.aws_data_solutions_framework-1.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:15:58.523133 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:15:58.527133 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 16:15:48.000000 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:15:58.527133 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-19 16:15:48.000000 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  3744819 2024-04-19 16:15:48.000000 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/_jsii/aws-data-solutions-framework@1.5.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:15:58.531133 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/consumption/
--rw-r--r--   0 runner    (1001) docker     (127)   158969 2024-04-19 16:15:48.000000 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/consumption/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:15:58.531133 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/governance/
--rw-r--r--   0 runner    (1001) docker     (127)    45726 2024-04-19 16:15:48.000000 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/governance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:15:58.531133 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/processing/
--rw-r--r--   0 runner    (1001) docker     (127)   259729 2024-04-19 16:15:48.000000 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:15:48.000000 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:15:58.531133 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/storage/
--rw-r--r--   0 runner    (1001) docker     (127)    86274 2024-04-19 16:15:48.000000 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:15:58.535133 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)    93221 2024-04-19 16:15:48.000000 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/streaming/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:15:58.535133 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    97649 2024-04-19 16:15:48.000000 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:15:58.527133 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs.aws_data_solutions_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-19 16:15:58.000000 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs.aws_data_solutions_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-19 16:15:58.000000 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs.aws_data_solutions_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:15:58.000000 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs.aws_data_solutions_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-19 16:15:58.000000 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs.aws_data_solutions_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 16:15:58.000000 cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs.aws_data_solutions_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11392 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.658992 cdklabs.aws_data_solutions_framework-1.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.658992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.658992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.662992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3947535 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/_jsii/aws-data-solutions-framework@1.6.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/consumption/
+-rw-r--r--   0 runner    (1001) docker     (127)   249288 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/consumption/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/governance/
+-rw-r--r--   0 runner    (1001) docker     (127)    45726 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/governance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)   259729 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)    86274 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)    93221 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/streaming/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.666992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    97649 2024-04-29 17:40:05.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 17:40:15.658992 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-29 17:40:15.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-29 17:40:15.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 17:40:15.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-29 17:40:15.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 17:40:15.000000 cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/top_level.txt
```

### Comparing `cdklabs.aws_data_solutions_framework-1.5.0/LICENSE` & `cdklabs.aws_data_solutions_framework-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.5.0/PKG-INFO` & `cdklabs.aws_data_solutions_framework-1.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.aws_data_solutions_framework
-Version: 1.5.0
+Version: 1.6.0
 Summary: L3 CDK Constructs used to build data solutions with AWS
 Home-page: https://awslabs.github.io/data-solutions-framework-on-aws/
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/data-solutions-framework-on-aws.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.aws_data_solutions_framework-1.5.0/setup.py` & `cdklabs.aws_data_solutions_framework-1.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.aws_data_solutions_framework",
-    "version": "1.5.0",
+    "version": "1.6.0",
     "description": "L3 CDK Constructs used to build data solutions with AWS",
     "license": "Apache-2.0",
     "url": "https://awslabs.github.io/data-solutions-framework-on-aws/",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -28,15 +28,15 @@
         "cdklabs.aws_data_solutions_framework.processing",
         "cdklabs.aws_data_solutions_framework.storage",
         "cdklabs.aws_data_solutions_framework.streaming",
         "cdklabs.aws_data_solutions_framework.utils"
     ],
     "package_data": {
         "cdklabs.aws_data_solutions_framework._jsii": [
-            "aws-data-solutions-framework@1.5.0.jsii.tgz"
+            "aws-data-solutions-framework@1.6.0.jsii.tgz"
         ],
         "cdklabs.aws_data_solutions_framework": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/__init__.py` & `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/_jsii/__init__.py` & `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/_jsii/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import aws_cdk.lambda_layer_kubectl_v27._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@cdklabs/aws-data-solutions-framework",
-    "1.5.0",
+    "1.6.0",
     __name__[0:-6],
-    "aws-data-solutions-framework@1.5.0.jsii.tgz",
+    "aws-data-solutions-framework@1.6.0.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/governance/__init__.py` & `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/governance/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/processing/__init__.py` & `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/storage/__init__.py` & `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/streaming/__init__.py` & `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs/aws_data_solutions_framework/utils/__init__.py` & `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs/aws_data_solutions_framework/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs.aws_data_solutions_framework.egg-info/PKG-INFO` & `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.aws-data-solutions-framework
-Version: 1.5.0
+Version: 1.6.0
 Summary: L3 CDK Constructs used to build data solutions with AWS
 Home-page: https://awslabs.github.io/data-solutions-framework-on-aws/
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/data-solutions-framework-on-aws.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.aws_data_solutions_framework-1.5.0/src/cdklabs.aws_data_solutions_framework.egg-info/SOURCES.txt` & `cdklabs.aws_data_solutions_framework-1.6.0/src/cdklabs.aws_data_solutions_framework.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 src/cdklabs.aws_data_solutions_framework.egg-info/SOURCES.txt
 src/cdklabs.aws_data_solutions_framework.egg-info/dependency_links.txt
 src/cdklabs.aws_data_solutions_framework.egg-info/requires.txt
 src/cdklabs.aws_data_solutions_framework.egg-info/top_level.txt
 src/cdklabs/aws_data_solutions_framework/__init__.py
 src/cdklabs/aws_data_solutions_framework/py.typed
 src/cdklabs/aws_data_solutions_framework/_jsii/__init__.py
-src/cdklabs/aws_data_solutions_framework/_jsii/aws-data-solutions-framework@1.5.0.jsii.tgz
+src/cdklabs/aws_data_solutions_framework/_jsii/aws-data-solutions-framework@1.6.0.jsii.tgz
 src/cdklabs/aws_data_solutions_framework/consumption/__init__.py
 src/cdklabs/aws_data_solutions_framework/governance/__init__.py
 src/cdklabs/aws_data_solutions_framework/processing/__init__.py
 src/cdklabs/aws_data_solutions_framework/storage/__init__.py
 src/cdklabs/aws_data_solutions_framework/streaming/__init__.py
 src/cdklabs/aws_data_solutions_framework/utils/__init__.py
```

