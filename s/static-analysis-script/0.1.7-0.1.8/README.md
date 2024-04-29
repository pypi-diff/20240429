# Comparing `tmp/static_analysis_script-0.1.7.tar.gz` & `tmp/static_analysis_script-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static_analysis_script-0.1.7.tar", last modified: Mon Apr 29 06:36:22 2024, max compression
+gzip compressed data, was "static_analysis_script-0.1.8.tar", last modified: Mon Apr 29 06:40:09 2024, max compression
```

## Comparing `static_analysis_script-0.1.7.tar` & `static_analysis_script-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 06:36:22.450041 static_analysis_script-0.1.7/
--rw-rw-rw-   0        0        0     2318 2024-04-29 06:36:22.449039 static_analysis_script-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1579 2024-04-29 06:33:06.000000 static_analysis_script-0.1.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 06:36:22.450041 static_analysis_script-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1603 2024-04-29 06:34:59.000000 static_analysis_script-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 06:36:22.421015 static_analysis_script-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 06:36:22.432527 static_analysis_script-0.1.7/src/analysis/
--rw-rw-rw-   0        0        0        0 2024-04-29 06:33:06.000000 static_analysis_script-0.1.7/src/analysis/__init__.py
--rw-rw-rw-   0        0        0    11695 2024-04-29 06:33:06.000000 static_analysis_script-0.1.7/src/analysis/main.py
-drwxrwxrwx   0        0        0        0 2024-04-29 06:36:22.449039 static_analysis_script-0.1.7/src/static_analysis_script.egg-info/
--rw-rw-rw-   0        0        0     2318 2024-04-29 06:36:22.000000 static_analysis_script-0.1.7/src/static_analysis_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      366 2024-04-29 06:36:22.000000 static_analysis_script-0.1.7/src/static_analysis_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 06:36:22.000000 static_analysis_script-0.1.7/src/static_analysis_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-29 06:36:22.000000 static_analysis_script-0.1.7/src/static_analysis_script.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-04-29 06:36:22.000000 static_analysis_script-0.1.7/src/static_analysis_script.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 06:36:22.000000 static_analysis_script-0.1.7/src/static_analysis_script.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 06:40:09.217847 static_analysis_script-0.1.8/
+-rw-rw-rw-   0        0        0     2318 2024-04-29 06:40:09.216847 static_analysis_script-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1579 2024-04-29 06:33:06.000000 static_analysis_script-0.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 06:40:09.217847 static_analysis_script-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1594 2024-04-29 06:38:58.000000 static_analysis_script-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 06:40:09.200339 static_analysis_script-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 06:40:09.201338 static_analysis_script-0.1.8/src/analysis/
+-rw-rw-rw-   0        0        0        0 2024-04-29 06:33:06.000000 static_analysis_script-0.1.8/src/analysis/__init__.py
+-rw-rw-rw-   0        0        0    11695 2024-04-29 06:33:06.000000 static_analysis_script-0.1.8/src/analysis/main.py
+drwxrwxrwx   0        0        0        0 2024-04-29 06:40:09.202338 static_analysis_script-0.1.8/src/bin/
+-rwxrwxrwx   0        0        0   370056 2024-04-29 06:33:06.000000 static_analysis_script-0.1.8/src/bin/strings.exe
+drwxrwxrwx   0        0        0        0 2024-04-29 06:40:09.216847 static_analysis_script-0.1.8/src/static_analysis_script.egg-info/
+-rw-rw-rw-   0        0        0     2318 2024-04-29 06:40:09.000000 static_analysis_script-0.1.8/src/static_analysis_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2024-04-29 06:40:09.000000 static_analysis_script-0.1.8/src/static_analysis_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 06:40:09.000000 static_analysis_script-0.1.8/src/static_analysis_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-29 06:40:09.000000 static_analysis_script-0.1.8/src/static_analysis_script.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2024-04-29 06:40:09.000000 static_analysis_script-0.1.8/src/static_analysis_script.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 06:40:09.000000 static_analysis_script-0.1.8/src/static_analysis_script.egg-info/top_level.txt
```

### Comparing `static_analysis_script-0.1.7/PKG-INFO` & `static_analysis_script-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-analysis-script
-Version: 0.1.7
+Version: 0.1.8
 Summary: A utility to perform static analysis on files.
 Home-page: https://github.com/perzibel/static-analysis-script
 Author: Perzibel
 Author-email: perzibel@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Security
```

### Comparing `static_analysis_script-0.1.7/README.md` & `static_analysis_script-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `static_analysis_script-0.1.7/setup.py` & `static_analysis_script-0.1.8/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Used for the long_description. It's nice to have this in the setup file so
 # that the distribution will have a more comprehensive description.
 def read(file_name):
     return open(os.path.join(os.path.dirname(__file__), file_name)).read()
 
 setup(
     name='static-analysis-script',
-    version='0.1.7',
+    version='0.1.8',
     author='Perzibel',
     author_email='perzibel@outlook.com',
     description='A utility to perform static analysis on files.',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',  # This is important for rendering Markdown from README
     url='https://github.com/perzibel/static-analysis-script',
     packages=find_packages(where="src"),
@@ -26,15 +26,15 @@
     install_requires=[
         'PyPDF2',
         'tqdm',
         'numpy'   
     ],
     include_package_data=True,
     package_data={
-        "analysis": ["../analysis/bin/strings.exe"],  # Make sure the path matches your structure
+        "analysis": ["../bin/strings.exe"],  # Make sure the path matches your structure
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Information Technology',
         'Topic :: Security',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

### Comparing `static_analysis_script-0.1.7/src/analysis/main.py` & `static_analysis_script-0.1.8/src/analysis/main.py`

 * *Files identical despite different names*

### Comparing `static_analysis_script-0.1.7/src/static_analysis_script.egg-info/PKG-INFO` & `static_analysis_script-0.1.8/src/static_analysis_script.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-analysis-script
-Version: 0.1.7
+Version: 0.1.8
 Summary: A utility to perform static analysis on files.
 Home-page: https://github.com/perzibel/static-analysis-script
 Author: Perzibel
 Author-email: perzibel@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Security
```

