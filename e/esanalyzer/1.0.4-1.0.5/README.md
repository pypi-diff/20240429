# Comparing `tmp/esanalyzer-1.0.4.tar.gz` & `tmp/esanalyzer-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esanalyzer-1.0.4.tar", last modified: Fri Apr 26 05:23:47 2024, max compression
+gzip compressed data, was "esanalyzer-1.0.5.tar", last modified: Mon Apr 29 10:20:22 2024, max compression
```

## Comparing `esanalyzer-1.0.4.tar` & `esanalyzer-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-26 05:23:47.811939 esanalyzer-1.0.4/
--rw-rw-rw-   0        0        0     1074 2024-04-25 11:23:48.000000 esanalyzer-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1479 2024-04-26 05:23:47.809917 esanalyzer-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      581 2024-04-26 05:20:35.000000 esanalyzer-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-26 05:23:47.789211 esanalyzer-1.0.4/esanalyzer/
-drwxrwxrwx   0        0        0        0 2024-04-26 05:23:47.803924 esanalyzer-1.0.4/esanalyzer/src/
-drwxrwxrwx   0        0        0        0 2024-04-26 05:23:47.807919 esanalyzer-1.0.4/esanalyzer/src/esanalyzer.egg-info/
--rw-rw-rw-   0        0        0     1479 2024-04-26 05:23:47.000000 esanalyzer-1.0.4/esanalyzer/src/esanalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2024-04-26 05:23:47.000000 esanalyzer-1.0.4/esanalyzer/src/esanalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-26 05:23:47.000000 esanalyzer-1.0.4/esanalyzer/src/esanalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2024-04-26 05:23:47.000000 esanalyzer-1.0.4/esanalyzer/src/esanalyzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-26 05:23:47.000000 esanalyzer-1.0.4/esanalyzer/src/esanalyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    23767 2024-04-25 13:08:05.000000 esanalyzer-1.0.4/esanalyzer/src/esanalyzer.py
--rw-rw-rw-   0        0        0       42 2024-04-26 05:23:47.811939 esanalyzer-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1724 2024-04-26 05:20:06.000000 esanalyzer-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:20:22.973442 esanalyzer-1.0.5/
+-rw-rw-rw-   0        0        0     1074 2024-04-25 11:23:48.000000 esanalyzer-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1545 2024-04-29 10:20:22.972475 esanalyzer-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1030 2024-04-29 06:24:51.000000 esanalyzer-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 10:20:22.946068 esanalyzer-1.0.5/esanalyzer/
+drwxrwxrwx   0        0        0        0 2024-04-29 10:20:22.964467 esanalyzer-1.0.5/esanalyzer/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 10:20:22.969452 esanalyzer-1.0.5/esanalyzer/src/esanalyzer.egg-info/
+-rw-rw-rw-   0        0        0     1545 2024-04-29 10:20:22.000000 esanalyzer-1.0.5/esanalyzer/src/esanalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2024-04-29 10:20:22.000000 esanalyzer-1.0.5/esanalyzer/src/esanalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 10:20:22.000000 esanalyzer-1.0.5/esanalyzer/src/esanalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2024-04-29 10:20:22.000000 esanalyzer-1.0.5/esanalyzer/src/esanalyzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-29 10:20:22.000000 esanalyzer-1.0.5/esanalyzer/src/esanalyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    23767 2024-04-25 13:08:05.000000 esanalyzer-1.0.5/esanalyzer/src/esanalyzer.py
+-rw-rw-rw-   0        0        0       42 2024-04-29 10:20:22.974438 esanalyzer-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1790 2024-04-29 10:19:26.000000 esanalyzer-1.0.5/setup.py
```

### Comparing `esanalyzer-1.0.4/LICENSE` & `esanalyzer-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `esanalyzer-1.0.4/PKG-INFO` & `esanalyzer-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: esanalyzer
-Version: 1.0.4
+Version: 1.0.5
 Summary: Emotion("fear", "anger", "surprise", "sadness", "disgust", "joy") and Sentiment("Positive","Negative") Analysis
-Home-page: https://github.com/ajaysingh111444/python/tree/esanalyzer/esanalyzer
+Home-page: https://github.com/ajaysingh111444/python/tree/esanalyzer/esanalyzer/version/1.0.5
 Author: Ajay Singh Rajput
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: nrclex
-Requires-Dist: datasets
-Requires-Dist: scikit-learn
-Requires-Dist: pandas
-Requires-Dist: numpy
+Requires-Dist: nrclex==3.0.0
+Requires-Dist: datasets==2.16.1
+Requires-Dist: scikit-learn==1.3.2
+Requires-Dist: pandas==2.1.4
+Requires-Dist: numpy==1.26.3
 Requires-Dist: googletrans==4.0.0-rc1
-Requires-Dist: transformers
-Requires-Dist: nltk
+Requires-Dist: transformers==4.36.2
+Requires-Dist: nltk==3.8.1
 
 # esanalyzer
 
     The Python Emotion and Sentiment Analysis library you've been looking for.
 
     ## Services
     - Emotion Analysis("fear", "anger", "surprise", "sadness", "disgust", "joy")
```

### Comparing `esanalyzer-1.0.4/esanalyzer/src/esanalyzer.egg-info/PKG-INFO` & `esanalyzer-1.0.5/esanalyzer/src/esanalyzer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: esanalyzer
-Version: 1.0.4
+Version: 1.0.5
 Summary: Emotion("fear", "anger", "surprise", "sadness", "disgust", "joy") and Sentiment("Positive","Negative") Analysis
-Home-page: https://github.com/ajaysingh111444/python/tree/esanalyzer/esanalyzer
+Home-page: https://github.com/ajaysingh111444/python/tree/esanalyzer/esanalyzer/version/1.0.5
 Author: Ajay Singh Rajput
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: nrclex
-Requires-Dist: datasets
-Requires-Dist: scikit-learn
-Requires-Dist: pandas
-Requires-Dist: numpy
+Requires-Dist: nrclex==3.0.0
+Requires-Dist: datasets==2.16.1
+Requires-Dist: scikit-learn==1.3.2
+Requires-Dist: pandas==2.1.4
+Requires-Dist: numpy==1.26.3
 Requires-Dist: googletrans==4.0.0-rc1
-Requires-Dist: transformers
-Requires-Dist: nltk
+Requires-Dist: transformers==4.36.2
+Requires-Dist: nltk==3.8.1
 
 # esanalyzer
 
     The Python Emotion and Sentiment Analysis library you've been looking for.
 
     ## Services
     - Emotion Analysis("fear", "anger", "surprise", "sadness", "disgust", "joy")
```

### Comparing `esanalyzer-1.0.4/esanalyzer/src/esanalyzer.py` & `esanalyzer-1.0.5/esanalyzer/src/esanalyzer.py`

 * *Files identical despite different names*

### Comparing `esanalyzer-1.0.4/setup.py` & `esanalyzer-1.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='esanalyzer',
-    version='1.0.4',
+    version='1.0.5',
     author='Ajay Singh Rajput',
     description='Emotion("fear", "anger", "surprise", "sadness", "disgust", "joy") and Sentiment("Positive","Negative") Analysis',
-    url='https://github.com/ajaysingh111444/python/tree/esanalyzer/esanalyzer',
+    url='https://github.com/ajaysingh111444/python/tree/esanalyzer/esanalyzer/version/1.0.5',
     long_description="""# esanalyzer
 
     The Python Emotion and Sentiment Analysis library you've been looking for.
 
     ## Services
     - Emotion Analysis("fear", "anger", "surprise", "sadness", "disgust", "joy")
     - Sentiment Analysis("Positive","Negative")
@@ -38,19 +38,19 @@
     
     """,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
     py_modules=["esanalyzer"],
     packages=find_packages(),
     install_requires=[
-        'nrclex',
-        'datasets',
-        'scikit-learn',
-        'pandas',
-        'numpy',
+        'nrclex==3.0.0',
+        'datasets==2.16.1',
+        'scikit-learn==1.3.2',
+        'pandas==2.1.4',
+        'numpy==1.26.3',
         'googletrans==4.0.0-rc1',
-        'transformers',
-        'nltk'
+        'transformers==4.36.2',
+        'nltk==3.8.1'
     ],
     package_dir={'':'esanalyzer/src'}
     # Include other metadata like description, author, etc.
 )
```

