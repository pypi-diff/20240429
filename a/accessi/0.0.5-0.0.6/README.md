# Comparing `tmp/accessi-0.0.5.tar.gz` & `tmp/accessi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accessi-0.0.5.tar", last modified: Thu Apr 25 19:12:46 2024, max compression
+gzip compressed data, was "accessi-0.0.6.tar", last modified: Mon Apr 29 18:53:41 2024, max compression
```

## Comparing `accessi-0.0.5.tar` & `accessi-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:12:46.061027 accessi-0.0.5/
--rw-rw-rw-   0 root         (0) root         (0)     1070 2024-04-25 18:49:29.000000 accessi-0.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1477 2024-04-25 19:12:46.061027 accessi-0.0.5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      889 2024-04-25 18:49:29.000000 accessi-0.0.5/README.md
--rw-rw-rw-   0 root         (0) root         (0)      570 2024-04-25 19:12:13.000000 accessi-0.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-25 19:12:46.061027 accessi-0.0.5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:12:46.057027 accessi-0.0.5/src/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-25 19:12:13.000000 accessi-0.0.5/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:12:46.057027 accessi-0.0.5/src/accessi.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1477 2024-04-25 19:12:46.000000 accessi-0.0.5/src/accessi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      218 2024-04-25 19:12:46.000000 accessi-0.0.5/src/accessi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-25 19:12:46.000000 accessi-0.0.5/src/accessi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-25 19:12:46.000000 accessi-0.0.5/src/accessi.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    35905 2024-04-25 18:49:29.000000 accessi-0.0.5/src/accessi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-25 19:12:46.057027 accessi-0.0.5/tests/
--rw-rw-rw-   0 root         (0) root         (0)     6311 2024-04-25 18:49:29.000000 accessi-0.0.5/tests/tests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:53:41.094946 accessi-0.0.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1070 2024-04-29 18:53:29.000000 accessi-0.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-04-29 18:53:41.090946 accessi-0.0.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      831 2024-04-29 18:53:29.000000 accessi-0.0.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      578 2024-04-29 18:53:29.000000 accessi-0.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-29 18:53:41.094946 accessi-0.0.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:53:41.090946 accessi-0.0.6/src/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 18:53:29.000000 accessi-0.0.6/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:53:41.090946 accessi-0.0.6/src/accessi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-04-29 18:53:41.000000 accessi-0.0.6/src/accessi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      218 2024-04-29 18:53:41.000000 accessi-0.0.6/src/accessi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 18:53:41.000000 accessi-0.0.6/src/accessi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-29 18:53:41.000000 accessi-0.0.6/src/accessi.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    35905 2024-04-29 18:53:29.000000 accessi-0.0.6/src/accessi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 18:53:41.090946 accessi-0.0.6/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6311 2024-04-29 18:53:29.000000 accessi-0.0.6/tests/tests.py
```

### Comparing `accessi-0.0.5/LICENSE` & `accessi-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `accessi-0.0.5/PKG-INFO` & `accessi-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: accessi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library for Siemens Access-i MR Scanner Interface to integrate and control the MR Scanner.
 Author-email: Martin Reinok <m.reinok@student.utwente.nl>
-Project-URL: Homepage, https://github.com/martinreinok/accessi-library
-Project-URL: Issues, https://github.com/martinreinok/accessi-library/issues
+Project-URL: Homepage, https://gitlab.utwente.nl/s2981416/accessi-library
+Project-URL: Issues, https://gitlab.utwente.nl/s2981416/accessi-library/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,15 +18,15 @@
 ## Install
 ```
 pip install accessi
 ```
 
 ## Siemens Documentation
 The library is based on this document:
-[Access-i Dev Guide NX V1.1.2](https://github.com/martinreinok/accessi-library/blob/main/documentation/Access-i_Dev_Guide_NX_V1.1.2.pdf)
+[Access-i Dev Guide NX V1.1.2](documentation/Access-i_Dev_Guide_NX_V1.1.2.pdf)
 
 ## Usage guide
 A sample test suite (tests.py) has been created which demonstrates basic Access-i usage.  
 The tests.py requires Access-i simulator to be running on the background, on the same local computer.  
 The tests.py demonstrates most of the implemented methods, as well as receiving images over websocket.  
 
 ## Collaborating
```

### Comparing `accessi-0.0.5/README.md` & `accessi-0.0.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 ## Install
 ```
 pip install accessi
 ```
 
 ## Siemens Documentation
 The library is based on this document:
-[Access-i Dev Guide NX V1.1.2](https://github.com/martinreinok/accessi-library/blob/main/documentation/Access-i_Dev_Guide_NX_V1.1.2.pdf)
+[Access-i Dev Guide NX V1.1.2](documentation/Access-i_Dev_Guide_NX_V1.1.2.pdf)
 
 ## Usage guide
 A sample test suite (tests.py) has been created which demonstrates basic Access-i usage.  
 The tests.py requires Access-i simulator to be running on the background, on the same local computer.  
 The tests.py demonstrates most of the implemented methods, as well as receiving images over websocket.  
 
 ## Collaborating
```

### Comparing `accessi-0.0.5/src/accessi.egg-info/PKG-INFO` & `accessi-0.0.6/src/accessi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: accessi
-Version: 0.0.5
+Version: 0.0.6
 Summary: Library for Siemens Access-i MR Scanner Interface to integrate and control the MR Scanner.
 Author-email: Martin Reinok <m.reinok@student.utwente.nl>
-Project-URL: Homepage, https://github.com/martinreinok/accessi-library
-Project-URL: Issues, https://github.com/martinreinok/accessi-library/issues
+Project-URL: Homepage, https://gitlab.utwente.nl/s2981416/accessi-library
+Project-URL: Issues, https://gitlab.utwente.nl/s2981416/accessi-library/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -18,15 +18,15 @@
 ## Install
 ```
 pip install accessi
 ```
 
 ## Siemens Documentation
 The library is based on this document:
-[Access-i Dev Guide NX V1.1.2](https://github.com/martinreinok/accessi-library/blob/main/documentation/Access-i_Dev_Guide_NX_V1.1.2.pdf)
+[Access-i Dev Guide NX V1.1.2](documentation/Access-i_Dev_Guide_NX_V1.1.2.pdf)
 
 ## Usage guide
 A sample test suite (tests.py) has been created which demonstrates basic Access-i usage.  
 The tests.py requires Access-i simulator to be running on the background, on the same local computer.  
 The tests.py demonstrates most of the implemented methods, as well as receiving images over websocket.  
 
 ## Collaborating
```

### Comparing `accessi-0.0.5/src/accessi.py` & `accessi-0.0.6/src/accessi.py`

 * *Files identical despite different names*

### Comparing `accessi-0.0.5/tests/tests.py` & `accessi-0.0.6/tests/tests.py`

 * *Files identical despite different names*

