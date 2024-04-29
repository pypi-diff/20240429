# Comparing `tmp/static_analysis_script-0.1.6.tar.gz` & `tmp/static_analysis_script-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static_analysis_script-0.1.6.tar", last modified: Mon Apr 29 06:28:22 2024, max compression
+gzip compressed data, was "static_analysis_script-0.1.7.tar", last modified: Mon Apr 29 06:36:22 2024, max compression
```

## Comparing `static_analysis_script-0.1.6.tar` & `static_analysis_script-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 06:28:22.491471 static_analysis_script-0.1.6/
--rw-rw-rw-   0        0        0     2318 2024-04-29 06:28:22.490471 static_analysis_script-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     1579 2024-04-29 06:24:40.000000 static_analysis_script-0.1.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 06:28:22.491471 static_analysis_script-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1603 2024-04-29 06:27:06.000000 static_analysis_script-0.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 06:28:22.472962 static_analysis_script-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 06:28:22.490471 static_analysis_script-0.1.6/src/static_analysis_script.egg-info/
--rw-rw-rw-   0        0        0     2318 2024-04-29 06:28:22.000000 static_analysis_script-0.1.6/src/static_analysis_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      320 2024-04-29 06:28:22.000000 static_analysis_script-0.1.6/src/static_analysis_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 06:28:22.000000 static_analysis_script-0.1.6/src/static_analysis_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-29 06:28:22.000000 static_analysis_script-0.1.6/src/static_analysis_script.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-04-29 06:28:22.000000 static_analysis_script-0.1.6/src/static_analysis_script.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 06:28:22.000000 static_analysis_script-0.1.6/src/static_analysis_script.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 06:36:22.450041 static_analysis_script-0.1.7/
+-rw-rw-rw-   0        0        0     2318 2024-04-29 06:36:22.449039 static_analysis_script-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1579 2024-04-29 06:33:06.000000 static_analysis_script-0.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 06:36:22.450041 static_analysis_script-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2024-04-29 06:34:59.000000 static_analysis_script-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 06:36:22.421015 static_analysis_script-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 06:36:22.432527 static_analysis_script-0.1.7/src/analysis/
+-rw-rw-rw-   0        0        0        0 2024-04-29 06:33:06.000000 static_analysis_script-0.1.7/src/analysis/__init__.py
+-rw-rw-rw-   0        0        0    11695 2024-04-29 06:33:06.000000 static_analysis_script-0.1.7/src/analysis/main.py
+drwxrwxrwx   0        0        0        0 2024-04-29 06:36:22.449039 static_analysis_script-0.1.7/src/static_analysis_script.egg-info/
+-rw-rw-rw-   0        0        0     2318 2024-04-29 06:36:22.000000 static_analysis_script-0.1.7/src/static_analysis_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2024-04-29 06:36:22.000000 static_analysis_script-0.1.7/src/static_analysis_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 06:36:22.000000 static_analysis_script-0.1.7/src/static_analysis_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-29 06:36:22.000000 static_analysis_script-0.1.7/src/static_analysis_script.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2024-04-29 06:36:22.000000 static_analysis_script-0.1.7/src/static_analysis_script.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 06:36:22.000000 static_analysis_script-0.1.7/src/static_analysis_script.egg-info/top_level.txt
```

### Comparing `static_analysis_script-0.1.6/PKG-INFO` & `static_analysis_script-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-analysis-script
-Version: 0.1.6
+Version: 0.1.7
 Summary: A utility to perform static analysis on files.
 Home-page: https://github.com/perzibel/static-analysis-script
 Author: Perzibel
 Author-email: perzibel@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Security
```

### Comparing `static_analysis_script-0.1.6/README.md` & `static_analysis_script-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `static_analysis_script-0.1.6/setup.py` & `static_analysis_script-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Used for the long_description. It's nice to have this in the setup file so
 # that the distribution will have a more comprehensive description.
 def read(file_name):
     return open(os.path.join(os.path.dirname(__file__), file_name)).read()
 
 setup(
     name='static-analysis-script',
-    version='0.1.6',
+    version='0.1.7',
     author='Perzibel',
     author_email='perzibel@outlook.com',
     description='A utility to perform static analysis on files.',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',  # This is important for rendering Markdown from README
     url='https://github.com/perzibel/static-analysis-script',
     packages=find_packages(where="src"),
```

### Comparing `static_analysis_script-0.1.6/src/static_analysis_script.egg-info/PKG-INFO` & `static_analysis_script-0.1.7/src/static_analysis_script.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-analysis-script
-Version: 0.1.6
+Version: 0.1.7
 Summary: A utility to perform static analysis on files.
 Home-page: https://github.com/perzibel/static-analysis-script
 Author: Perzibel
 Author-email: perzibel@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Security
```

