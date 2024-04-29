# Comparing `tmp/jr_connection-0.1.3.tar.gz` & `tmp/jr_connection-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jr_connection-0.1.3.tar", last modified: Wed Apr 24 18:55:08 2024, max compression
+gzip compressed data, was "jr_connection-0.1.4.tar", last modified: Mon Apr 29 16:26:49 2024, max compression
```

## Comparing `jr_connection-0.1.3.tar` & `jr_connection-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:55:08.946612 jr_connection-0.1.3/
--rw-r--r--   0 felipeburry   (501) staff       (20)     1072 2024-04-17 14:52:47.000000 jr_connection-0.1.3/LICENSE
--rw-r--r--   0 felipeburry   (501) staff       (20)     2536 2024-04-24 18:55:08.946233 jr_connection-0.1.3/PKG-INFO
--rw-r--r--   0 felipeburry   (501) staff       (20)       16 2024-04-17 14:49:29.000000 jr_connection-0.1.3/README.md
--rw-r--r--   0 felipeburry   (501) staff       (20)     1148 2024-04-24 18:55:00.000000 jr_connection-0.1.3/pyproject.toml
--rw-r--r--   0 felipeburry   (501) staff       (20)       38 2024-04-24 18:55:08.946700 jr_connection-0.1.3/setup.cfg
--rw-r--r--   0 felipeburry   (501) staff       (20)      737 2024-04-24 18:54:36.000000 jr_connection-0.1.3/setup.py
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:55:08.934636 jr_connection-0.1.3/src/
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:55:08.937730 jr_connection-0.1.3/src/jr_connection/
--rw-r--r--   0 felipeburry   (501) staff       (20)      156 2024-04-24 18:54:23.000000 jr_connection-0.1.3/src/jr_connection/__init__.py
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:55:08.944582 jr_connection-0.1.3/src/jr_connection/classes/
--rw-r--r--   0 felipeburry   (501) staff       (20)      104 2024-04-24 18:51:26.000000 jr_connection-0.1.3/src/jr_connection/classes/__init__.py
--rw-r--r--   0 felipeburry   (501) staff       (20)     7506 2024-04-24 18:51:19.000000 jr_connection-0.1.3/src/jr_connection/classes/connection_class.py
--rw-r--r--   0 felipeburry   (501) staff       (20)     5504 2024-04-17 19:15:46.000000 jr_connection-0.1.3/src/jr_connection/classes/data_handler_class.py
--rw-r--r--   0 felipeburry   (501) staff       (20)      421 2024-04-24 18:38:17.000000 jr_connection-0.1.3/src/jr_connection/classes/dbconfig_class.py
--rwxr-xr-x   0 felipeburry   (501) staff       (20)     2932 2024-04-24 18:38:27.000000 jr_connection-0.1.3/src/jr_connection/first_run.py
--rw-r--r--   0 felipeburry   (501) staff       (20)      154 2024-04-17 18:00:05.000000 jr_connection-0.1.3/src/jr_connection/other_constants.py
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:55:08.941879 jr_connection-0.1.3/src/jr_connection.egg-info/
--rw-r--r--   0 felipeburry   (501) staff       (20)     2536 2024-04-24 18:55:08.000000 jr_connection-0.1.3/src/jr_connection.egg-info/PKG-INFO
--rw-r--r--   0 felipeburry   (501) staff       (20)      627 2024-04-24 18:55:08.000000 jr_connection-0.1.3/src/jr_connection.egg-info/SOURCES.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)        1 2024-04-24 18:55:08.000000 jr_connection-0.1.3/src/jr_connection.egg-info/dependency_links.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)       59 2024-04-24 18:55:08.000000 jr_connection-0.1.3/src/jr_connection.egg-info/entry_points.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)      347 2024-04-24 18:55:08.000000 jr_connection-0.1.3/src/jr_connection.egg-info/requires.txt
--rw-r--r--   0 felipeburry   (501) staff       (20)       14 2024-04-24 18:55:08.000000 jr_connection-0.1.3/src/jr_connection.egg-info/top_level.txt
-drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-24 18:55:08.945322 jr_connection-0.1.3/tests/
--rw-r--r--   0 felipeburry   (501) staff       (20)     2007 2024-04-17 18:31:52.000000 jr_connection-0.1.3/tests/test_connection_class.py
--rw-r--r--   0 felipeburry   (501) staff       (20)     2503 2024-04-17 18:48:40.000000 jr_connection-0.1.3/tests/test_data_handler_class.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-29 16:26:49.307803 jr_connection-0.1.4/
+-rw-r--r--   0 felipeburry   (501) staff       (20)     1072 2024-04-17 14:52:47.000000 jr_connection-0.1.4/LICENSE
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2536 2024-04-29 16:26:49.307358 jr_connection-0.1.4/PKG-INFO
+-rw-r--r--   0 felipeburry   (501) staff       (20)       16 2024-04-17 14:49:29.000000 jr_connection-0.1.4/README.md
+-rw-r--r--   0 felipeburry   (501) staff       (20)     1148 2024-04-29 16:24:18.000000 jr_connection-0.1.4/pyproject.toml
+-rw-r--r--   0 felipeburry   (501) staff       (20)       38 2024-04-29 16:26:49.307896 jr_connection-0.1.4/setup.cfg
+-rw-r--r--   0 felipeburry   (501) staff       (20)      737 2024-04-29 16:24:20.000000 jr_connection-0.1.4/setup.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-29 16:26:49.300171 jr_connection-0.1.4/src/
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-29 16:26:49.302837 jr_connection-0.1.4/src/jr_connection/
+-rw-r--r--   0 felipeburry   (501) staff       (20)      156 2024-04-24 18:54:23.000000 jr_connection-0.1.4/src/jr_connection/__init__.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-29 16:26:49.305969 jr_connection-0.1.4/src/jr_connection/classes/
+-rw-r--r--   0 felipeburry   (501) staff       (20)      104 2024-04-24 18:51:26.000000 jr_connection-0.1.4/src/jr_connection/classes/__init__.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)     7506 2024-04-24 18:51:19.000000 jr_connection-0.1.4/src/jr_connection/classes/connection_class.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)     5504 2024-04-17 19:15:46.000000 jr_connection-0.1.4/src/jr_connection/classes/data_handler_class.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)      421 2024-04-24 18:38:17.000000 jr_connection-0.1.4/src/jr_connection/classes/dbconfig_class.py
+-rwxr-xr-x   0 felipeburry   (501) staff       (20)     2932 2024-04-24 18:38:27.000000 jr_connection-0.1.4/src/jr_connection/first_run.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)      154 2024-04-17 18:00:05.000000 jr_connection-0.1.4/src/jr_connection/other_constants.py
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-29 16:26:49.304725 jr_connection-0.1.4/src/jr_connection.egg-info/
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2536 2024-04-29 16:26:49.000000 jr_connection-0.1.4/src/jr_connection.egg-info/PKG-INFO
+-rw-r--r--   0 felipeburry   (501) staff       (20)      627 2024-04-29 16:26:49.000000 jr_connection-0.1.4/src/jr_connection.egg-info/SOURCES.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)        1 2024-04-29 16:26:49.000000 jr_connection-0.1.4/src/jr_connection.egg-info/dependency_links.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)       59 2024-04-29 16:26:49.000000 jr_connection-0.1.4/src/jr_connection.egg-info/entry_points.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)      347 2024-04-29 16:26:49.000000 jr_connection-0.1.4/src/jr_connection.egg-info/requires.txt
+-rw-r--r--   0 felipeburry   (501) staff       (20)       14 2024-04-29 16:26:49.000000 jr_connection-0.1.4/src/jr_connection.egg-info/top_level.txt
+drwxr-xr-x   0 felipeburry   (501) staff       (20)        0 2024-04-29 16:26:49.306542 jr_connection-0.1.4/tests/
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2007 2024-04-17 18:31:52.000000 jr_connection-0.1.4/tests/test_connection_class.py
+-rw-r--r--   0 felipeburry   (501) staff       (20)     2503 2024-04-17 18:48:40.000000 jr_connection-0.1.4/tests/test_data_handler_class.py
```

### Comparing `jr_connection-0.1.3/LICENSE` & `jr_connection-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jr_connection-0.1.3/PKG-INFO` & `jr_connection-0.1.4/src/jr_connection.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jr_connection
-Version: 0.1.3
+Name: jr-connection
+Version: 0.1.4
 Summary: A simple python package to connect to JR servers and get the data
 Home-page: https://github.com/faburry23/JR_Connection
 Author: Felipe Burry
 Author-email: Felipe Burry <felipe.burry@jriveros.cl>
 License: MIT License
         
         Copyright (c) [2024] [Felipe Burry]
@@ -30,29 +30,29 @@
 Project-URL: Issues, https://github.com/faburry23/JR_Connection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cramjam==2.8.3
-Requires-Dist: et-xmlfile==1.1.0
-Requires-Dist: fastparquet==2024.2.0
-Requires-Dist: fsspec==2024.3.1
-Requires-Dist: numpy==1.26.4
-Requires-Dist: openpyxl==3.1.2
-Requires-Dist: packaging==24.0
-Requires-Dist: pandas==2.2.1
-Requires-Dist: pyarrow==15.0.2
-Requires-Dist: pyodbc==5.1.0
-Requires-Dist: python-dateutil==2.9.0.post0
-Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: pytz==2024.1
-Requires-Dist: six==1.16.0
-Requires-Dist: SQLAlchemy==2.0.29
-Requires-Dist: typing_extensions==4.10.0
-Requires-Dist: tzdata==2024.1
-Requires-Dist: pytest==7.4.3
-Requires-Dist: pytest-mock==3.14.0
-Requires-Dist: pymssql==2.2.11
+Requires-Dist: cramjam>=2.8.3
+Requires-Dist: et-xmlfile>=1.1.0
+Requires-Dist: fastparquet>=2024.2.0
+Requires-Dist: fsspec>=2024.3.1
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: openpyxl>=3.1.2
+Requires-Dist: packaging>=24.0
+Requires-Dist: pandas>=2.2.1
+Requires-Dist: pyarrow>=15.0.2
+Requires-Dist: pyodbc>=5.1.0
+Requires-Dist: python-dateutil>=2.9.0.post0
+Requires-Dist: python-dotenv>=1.0.1
+Requires-Dist: pytz>=2024.1
+Requires-Dist: six>=1.16.0
+Requires-Dist: SQLAlchemy>=2.0.29
+Requires-Dist: typing_extensions>=4.10.0
+Requires-Dist: tzdata>=2024.1
+Requires-Dist: pytest>=7.4.3
+Requires-Dist: pytest-mock>=3.14.0
+Requires-Dist: pymssql>=2.2.11
 
 # JR_Connection
```

### Comparing `jr_connection-0.1.3/pyproject.toml` & `jr_connection-0.1.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jr_connection"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Felipe Burry", email="felipe.burry@jriveros.cl" },
 ]
 description = "A simple python package to connect to JR servers and get the data"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
-    "cramjam==2.8.3",
-    "et-xmlfile==1.1.0",
-    "fastparquet==2024.2.0",
-    "fsspec==2024.3.1",
-    "numpy==1.26.4",
-    "openpyxl==3.1.2",
-    "packaging==24.0",
-    "pandas==2.2.1",
-    "pyarrow==15.0.2",
-    "pyodbc==5.1.0",
-    "python-dateutil==2.9.0.post0",
-    "python-dotenv==1.0.1",
-    "pytz==2024.1",
-    "six==1.16.0",
-    "SQLAlchemy==2.0.29",
-    "typing_extensions==4.10.0",
-    "tzdata==2024.1",
-    "pytest==7.4.3",
-    "pytest-mock==3.14.0",
-    "pymssql==2.2.11",
+    "cramjam>=2.8.3",
+    "et-xmlfile>=1.1.0",
+    "fastparquet>=2024.2.0",
+    "fsspec>=2024.3.1",
+    "numpy>=1.26.4",
+    "openpyxl>=3.1.2",
+    "packaging>=24.0",
+    "pandas>=2.2.1",
+    "pyarrow>=15.0.2",
+    "pyodbc>=5.1.0",
+    "python-dateutil>=2.9.0.post0",
+    "python-dotenv>=1.0.1",
+    "pytz>=2024.1",
+    "six>=1.16.0",
+    "SQLAlchemy>=2.0.29",
+    "typing_extensions>=4.10.0",
+    "tzdata>=2024.1",
+    "pytest>=7.4.3",
+    "pytest-mock>=3.14.0",
+    "pymssql>=2.2.11",
 ]
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
```

### Comparing `jr_connection-0.1.3/setup.py` & `jr_connection-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="jr_connection",
-    version="0.1.3",
+    version="0.1.4",
     description="A simple python package to connect to JR servers and get the data",
     long_description="lalala",
     url="https://github.com/faburry23/JR_Connection",
     author="Felipe Burry",
     author_email="felipe.burry@jriveros.cl",
     license="MIT",
     package_dir={"": "src"},
```

### Comparing `jr_connection-0.1.3/src/jr_connection/classes/connection_class.py` & `jr_connection-0.1.4/src/jr_connection/classes/connection_class.py`

 * *Files identical despite different names*

### Comparing `jr_connection-0.1.3/src/jr_connection/classes/data_handler_class.py` & `jr_connection-0.1.4/src/jr_connection/classes/data_handler_class.py`

 * *Files identical despite different names*

### Comparing `jr_connection-0.1.3/src/jr_connection/first_run.py` & `jr_connection-0.1.4/src/jr_connection/first_run.py`

 * *Files identical despite different names*

### Comparing `jr_connection-0.1.3/src/jr_connection.egg-info/PKG-INFO` & `jr_connection-0.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jr-connection
-Version: 0.1.3
+Name: jr_connection
+Version: 0.1.4
 Summary: A simple python package to connect to JR servers and get the data
 Home-page: https://github.com/faburry23/JR_Connection
 Author: Felipe Burry
 Author-email: Felipe Burry <felipe.burry@jriveros.cl>
 License: MIT License
         
         Copyright (c) [2024] [Felipe Burry]
@@ -30,29 +30,29 @@
 Project-URL: Issues, https://github.com/faburry23/JR_Connection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: cramjam==2.8.3
-Requires-Dist: et-xmlfile==1.1.0
-Requires-Dist: fastparquet==2024.2.0
-Requires-Dist: fsspec==2024.3.1
-Requires-Dist: numpy==1.26.4
-Requires-Dist: openpyxl==3.1.2
-Requires-Dist: packaging==24.0
-Requires-Dist: pandas==2.2.1
-Requires-Dist: pyarrow==15.0.2
-Requires-Dist: pyodbc==5.1.0
-Requires-Dist: python-dateutil==2.9.0.post0
-Requires-Dist: python-dotenv==1.0.1
-Requires-Dist: pytz==2024.1
-Requires-Dist: six==1.16.0
-Requires-Dist: SQLAlchemy==2.0.29
-Requires-Dist: typing_extensions==4.10.0
-Requires-Dist: tzdata==2024.1
-Requires-Dist: pytest==7.4.3
-Requires-Dist: pytest-mock==3.14.0
-Requires-Dist: pymssql==2.2.11
+Requires-Dist: cramjam>=2.8.3
+Requires-Dist: et-xmlfile>=1.1.0
+Requires-Dist: fastparquet>=2024.2.0
+Requires-Dist: fsspec>=2024.3.1
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: openpyxl>=3.1.2
+Requires-Dist: packaging>=24.0
+Requires-Dist: pandas>=2.2.1
+Requires-Dist: pyarrow>=15.0.2
+Requires-Dist: pyodbc>=5.1.0
+Requires-Dist: python-dateutil>=2.9.0.post0
+Requires-Dist: python-dotenv>=1.0.1
+Requires-Dist: pytz>=2024.1
+Requires-Dist: six>=1.16.0
+Requires-Dist: SQLAlchemy>=2.0.29
+Requires-Dist: typing_extensions>=4.10.0
+Requires-Dist: tzdata>=2024.1
+Requires-Dist: pytest>=7.4.3
+Requires-Dist: pytest-mock>=3.14.0
+Requires-Dist: pymssql>=2.2.11
 
 # JR_Connection
```

### Comparing `jr_connection-0.1.3/src/jr_connection.egg-info/SOURCES.txt` & `jr_connection-0.1.4/src/jr_connection.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jr_connection-0.1.3/tests/test_connection_class.py` & `jr_connection-0.1.4/tests/test_connection_class.py`

 * *Files identical despite different names*

### Comparing `jr_connection-0.1.3/tests/test_data_handler_class.py` & `jr_connection-0.1.4/tests/test_data_handler_class.py`

 * *Files identical despite different names*

