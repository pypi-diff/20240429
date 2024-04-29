# Comparing `tmp/static_analysis_script-0.1.2.tar.gz` & `tmp/static_analysis_script-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static_analysis_script-0.1.2.tar", last modified: Sat Apr 27 03:11:04 2024, max compression
+gzip compressed data, was "static_analysis_script-0.1.3.tar", last modified: Mon Apr 29 05:47:25 2024, max compression
```

## Comparing `static_analysis_script-0.1.2.tar` & `static_analysis_script-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 03:11:04.476005 static_analysis_script-0.1.2/
--rw-rw-rw-   0        0        0     2318 2024-04-27 03:11:04.475005 static_analysis_script-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1579 2024-04-27 02:59:43.000000 static_analysis_script-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-27 03:11:04.476005 static_analysis_script-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1592 2024-04-27 03:09:27.000000 static_analysis_script-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 03:11:04.449660 static_analysis_script-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-27 03:11:04.451777 static_analysis_script-0.1.2/src/analysis/
--rw-rw-rw-   0        0        0        0 2024-04-27 02:59:43.000000 static_analysis_script-0.1.2/src/analysis/__init__.py
--rw-rw-rw-   0        0        0    11695 2024-04-27 02:57:52.000000 static_analysis_script-0.1.2/src/analysis/main.py
-drwxrwxrwx   0        0        0        0 2024-04-27 03:11:04.454776 static_analysis_script-0.1.2/src/bin/
--rwxrwxrwx   0        0        0   370056 2024-04-27 02:59:43.000000 static_analysis_script-0.1.2/src/bin/strings.exe
-drwxrwxrwx   0        0        0        0 2024-04-27 03:11:04.475005 static_analysis_script-0.1.2/src/static_analysis_script.egg-info/
--rw-rw-rw-   0        0        0     2318 2024-04-27 03:11:04.000000 static_analysis_script-0.1.2/src/static_analysis_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2024-04-27 03:11:04.000000 static_analysis_script-0.1.2/src/static_analysis_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 03:11:04.000000 static_analysis_script-0.1.2/src/static_analysis_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-27 03:11:04.000000 static_analysis_script-0.1.2/src/static_analysis_script.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-04-27 03:11:04.000000 static_analysis_script-0.1.2/src/static_analysis_script.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-27 03:11:04.000000 static_analysis_script-0.1.2/src/static_analysis_script.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 05:47:25.032721 static_analysis_script-0.1.3/
+-rw-rw-rw-   0        0        0     2318 2024-04-29 05:47:25.032721 static_analysis_script-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1579 2024-04-29 05:41:48.000000 static_analysis_script-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 05:47:25.033720 static_analysis_script-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1591 2024-04-29 05:45:46.000000 static_analysis_script-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 05:47:25.006171 static_analysis_script-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 05:47:25.012609 static_analysis_script-0.1.3/src/analysis/
+-rw-rw-rw-   0        0        0        0 2024-04-29 05:41:48.000000 static_analysis_script-0.1.3/src/analysis/__init__.py
+-rw-rw-rw-   0        0        0    11695 2024-04-29 05:41:48.000000 static_analysis_script-0.1.3/src/analysis/main.py
+drwxrwxrwx   0        0        0        0 2024-04-29 05:47:25.031721 static_analysis_script-0.1.3/src/static_analysis_script.egg-info/
+-rw-rw-rw-   0        0        0     2318 2024-04-29 05:47:24.000000 static_analysis_script-0.1.3/src/static_analysis_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      366 2024-04-29 05:47:25.000000 static_analysis_script-0.1.3/src/static_analysis_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 05:47:24.000000 static_analysis_script-0.1.3/src/static_analysis_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-29 05:47:24.000000 static_analysis_script-0.1.3/src/static_analysis_script.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2024-04-29 05:47:24.000000 static_analysis_script-0.1.3/src/static_analysis_script.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 05:47:24.000000 static_analysis_script-0.1.3/src/static_analysis_script.egg-info/top_level.txt
```

### Comparing `static_analysis_script-0.1.2/PKG-INFO` & `static_analysis_script-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-analysis-script
-Version: 0.1.2
+Version: 0.1.3
 Summary: A utility to perform static analysis on files.
 Home-page: https://github.com/perzibel/static-analysis-script
 Author: Perzibel
 Author-email: perzibel@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Security
```

### Comparing `static_analysis_script-0.1.2/README.md` & `static_analysis_script-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `static_analysis_script-0.1.2/setup.py` & `static_analysis_script-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Used for the long_description. It's nice to have this in the setup file so
 # that the distribution will have a more comprehensive description.
 def read(file_name):
     return open(os.path.join(os.path.dirname(__file__), file_name)).read()
 
 setup(
     name='static-analysis-script',
-    version='0.1.2',
+    version='0.1.3',
     author='Perzibel',
     author_email='perzibel@outlook.com',
     description='A utility to perform static analysis on files.',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',  # This is important for rendering Markdown from README
     url='https://github.com/perzibel/static-analysis-script',
     packages=find_packages(where="src"),
@@ -26,20 +26,20 @@
     install_requires=[
         'PyPDF2',
         'tqdm',
         'numpy'   
     ],
     include_package_data=True,
     package_data={
-        "analysis": ["../bin/strings.exe"],  # Make sure the path matches your structure
+        "analysis": ["bin/strings.exe"],  # Make sure the path matches your structure
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Information Technology',
         'Topic :: Security',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
-)
+)
```

### Comparing `static_analysis_script-0.1.2/src/analysis/main.py` & `static_analysis_script-0.1.3/src/analysis/main.py`

 * *Files identical despite different names*

### Comparing `static_analysis_script-0.1.2/src/static_analysis_script.egg-info/PKG-INFO` & `static_analysis_script-0.1.3/src/static_analysis_script.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-analysis-script
-Version: 0.1.2
+Version: 0.1.3
 Summary: A utility to perform static analysis on files.
 Home-page: https://github.com/perzibel/static-analysis-script
 Author: Perzibel
 Author-email: perzibel@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Security
```

