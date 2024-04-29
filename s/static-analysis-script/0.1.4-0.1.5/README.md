# Comparing `tmp/static_analysis_script-0.1.4.tar.gz` & `tmp/static_analysis_script-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static_analysis_script-0.1.4.tar", last modified: Mon Apr 29 06:02:33 2024, max compression
+gzip compressed data, was "static_analysis_script-0.1.5.tar", last modified: Mon Apr 29 06:16:23 2024, max compression
```

## Comparing `static_analysis_script-0.1.4.tar` & `static_analysis_script-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 06:02:33.219274 static_analysis_script-0.1.4/
--rw-rw-rw-   0        0        0     2318 2024-04-29 06:02:33.219274 static_analysis_script-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1579 2024-04-29 05:41:48.000000 static_analysis_script-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-29 06:02:33.219274 static_analysis_script-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1594 2024-04-29 06:00:31.000000 static_analysis_script-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 06:02:33.186508 static_analysis_script-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 06:02:33.189074 static_analysis_script-0.1.4/src/analysis/
--rw-rw-rw-   0        0        0        0 2024-04-29 05:41:48.000000 static_analysis_script-0.1.4/src/analysis/__init__.py
--rw-rw-rw-   0        0        0    11695 2024-04-29 05:41:48.000000 static_analysis_script-0.1.4/src/analysis/main.py
-drwxrwxrwx   0        0        0        0 2024-04-29 06:02:33.201761 static_analysis_script-0.1.4/src/bin/
--rwxrwxrwx   0        0        0   370056 2024-04-29 05:41:48.000000 static_analysis_script-0.1.4/src/bin/strings.exe
-drwxrwxrwx   0        0        0        0 2024-04-29 06:02:33.218282 static_analysis_script-0.1.4/src/static_analysis_script.egg-info/
--rw-rw-rw-   0        0        0     2318 2024-04-29 06:02:33.000000 static_analysis_script-0.1.4/src/static_analysis_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      398 2024-04-29 06:02:33.000000 static_analysis_script-0.1.4/src/static_analysis_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 06:02:33.000000 static_analysis_script-0.1.4/src/static_analysis_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-29 06:02:33.000000 static_analysis_script-0.1.4/src/static_analysis_script.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-04-29 06:02:33.000000 static_analysis_script-0.1.4/src/static_analysis_script.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 06:02:33.000000 static_analysis_script-0.1.4/src/static_analysis_script.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 06:16:23.001525 static_analysis_script-0.1.5/
+-rw-rw-rw-   0        0        0     2318 2024-04-29 06:16:23.001525 static_analysis_script-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1579 2024-04-29 05:41:48.000000 static_analysis_script-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 06:16:23.002525 static_analysis_script-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1603 2024-04-29 06:15:33.000000 static_analysis_script-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 06:16:22.976108 static_analysis_script-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 06:16:22.978682 static_analysis_script-0.1.5/src/analysis/
+-rw-rw-rw-   0        0        0        0 2024-04-29 05:41:48.000000 static_analysis_script-0.1.5/src/analysis/__init__.py
+-rw-rw-rw-   0        0        0    11695 2024-04-29 05:41:48.000000 static_analysis_script-0.1.5/src/analysis/main.py
+drwxrwxrwx   0        0        0        0 2024-04-29 06:16:22.979617 static_analysis_script-0.1.5/src/bin/
+-rwxrwxrwx   0        0        0   370056 2024-04-29 05:41:48.000000 static_analysis_script-0.1.5/src/bin/strings.exe
+drwxrwxrwx   0        0        0        0 2024-04-29 06:16:23.000526 static_analysis_script-0.1.5/src/static_analysis_script.egg-info/
+-rw-rw-rw-   0        0        0     2318 2024-04-29 06:16:22.000000 static_analysis_script-0.1.5/src/static_analysis_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2024-04-29 06:16:22.000000 static_analysis_script-0.1.5/src/static_analysis_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 06:16:22.000000 static_analysis_script-0.1.5/src/static_analysis_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-29 06:16:22.000000 static_analysis_script-0.1.5/src/static_analysis_script.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2024-04-29 06:16:22.000000 static_analysis_script-0.1.5/src/static_analysis_script.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-29 06:16:22.000000 static_analysis_script-0.1.5/src/static_analysis_script.egg-info/top_level.txt
```

### Comparing `static_analysis_script-0.1.4/PKG-INFO` & `static_analysis_script-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-analysis-script
-Version: 0.1.4
+Version: 0.1.5
 Summary: A utility to perform static analysis on files.
 Home-page: https://github.com/perzibel/static-analysis-script
 Author: Perzibel
 Author-email: perzibel@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Security
```

### Comparing `static_analysis_script-0.1.4/README.md` & `static_analysis_script-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `static_analysis_script-0.1.4/setup.py` & `static_analysis_script-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Used for the long_description. It's nice to have this in the setup file so
 # that the distribution will have a more comprehensive description.
 def read(file_name):
     return open(os.path.join(os.path.dirname(__file__), file_name)).read()
 
 setup(
     name='static-analysis-script',
-    version='0.1.4',
+    version='0.1.5',
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
-        "analysis": ["../bin/strings.exe"],  # Make sure the path matches your structure
+        "analysis": ["../analysis/bin/strings.exe"],  # Make sure the path matches your structure
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Information Technology',
         'Topic :: Security',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

### Comparing `static_analysis_script-0.1.4/src/analysis/main.py` & `static_analysis_script-0.1.5/src/analysis/main.py`

 * *Files identical despite different names*

### Comparing `static_analysis_script-0.1.4/src/bin/strings.exe` & `static_analysis_script-0.1.5/src/bin/strings.exe`

 * *Files identical despite different names*

### Comparing `static_analysis_script-0.1.4/src/static_analysis_script.egg-info/PKG-INFO` & `static_analysis_script-0.1.5/src/static_analysis_script.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-analysis-script
-Version: 0.1.4
+Version: 0.1.5
 Summary: A utility to perform static analysis on files.
 Home-page: https://github.com/perzibel/static-analysis-script
 Author: Perzibel
 Author-email: perzibel@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Security
```

