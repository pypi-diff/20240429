# Comparing `tmp/abstract_pandas-0.0.0.1.tar.gz` & `tmp/abstract_pandas-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_pandas-0.0.0.1.tar", last modified: Sun Apr 28 17:19:24 2024, max compression
+gzip compressed data, was "abstract_pandas-0.0.0.2.tar", last modified: Mon Apr 29 21:25:29 2024, max compression
```

## Comparing `abstract_pandas-0.0.0.1.tar` & `abstract_pandas-0.0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 17:19:24.366597 abstract_pandas-0.0.0.1/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-04-28 17:19:24.366597 abstract_pandas-0.0.0.1/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.1/README.md
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-28 17:19:24.366597 abstract_pandas-0.0.0.1/setup.cfg
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      979 2024-04-28 17:17:02.000000 abstract_pandas-0.0.0.1/setup.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 17:19:24.362597 abstract_pandas-0.0.0.1/src/
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 17:19:24.362597 abstract_pandas-0.0.0.1/src/abstract_pandas/
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.1/src/abstract_pandas/__init__.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      285 2024-04-28 05:06:34.000000 abstract_pandas-0.0.0.1/src/abstract_pandas/class_manager.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    20479 2024-04-24 17:55:36.000000 abstract_pandas-0.0.0.1/src/abstract_pandas/excel_gui.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)    15285 2024-04-17 21:20:16.000000 abstract_pandas-0.0.0.1/src/abstract_pandas/excel_module.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     3227 2024-04-17 09:26:10.000000 abstract_pandas-0.0.0.1/src/abstract_pandas/general_functions.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5664 2024-04-26 19:59:40.000000 abstract_pandas-0.0.0.1/src/abstract_pandas/geo_pandas.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     1464 2024-04-26 00:28:54.000000 abstract_pandas-0.0.0.1/src/abstract_pandas/geo_spec.py
--rw-rw-r--   0 gamook    (1000) gamook    (1000)     5426 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.1/src/abstract_pandas/time_module.py
-drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-28 17:19:24.366597 abstract_pandas-0.0.0.1/src/abstract_pandas.egg-info/
--rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-04-28 17:19:24.000000 abstract_pandas-0.0.0.1/src/abstract_pandas.egg-info/PKG-INFO
--rw-rw-r--   0 gamook    (1000) gamook    (1000)      512 2024-04-28 17:19:24.000000 abstract_pandas-0.0.0.1/src/abstract_pandas.egg-info/SOURCES.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-28 17:19:24.000000 abstract_pandas-0.0.0.1/src/abstract_pandas.egg-info/dependency_links.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-04-28 17:19:24.000000 abstract_pandas-0.0.0.1/src/abstract_pandas.egg-info/requires.txt
--rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-04-28 17:19:24.000000 abstract_pandas-0.0.0.1/src/abstract_pandas.egg-info/top_level.txt
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 21:25:29.910421 abstract_pandas-0.0.0.2/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-04-29 21:25:29.910421 abstract_pandas-0.0.0.2/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       49 2024-04-08 17:04:50.000000 abstract_pandas-0.0.0.2/README.md
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       38 2024-04-29 21:25:29.910421 abstract_pandas-0.0.0.2/setup.cfg
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      979 2024-04-29 21:25:21.000000 abstract_pandas-0.0.0.2/setup.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 21:25:29.910421 abstract_pandas-0.0.0.2/src/
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 21:25:29.910421 abstract_pandas-0.0.0.2/src/abstract_pandas/
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        0 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/__init__.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      285 2024-04-28 05:06:34.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/class_manager.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    20479 2024-04-24 17:55:36.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/excel_gui.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)    15784 2024-04-29 21:25:11.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/excel_module.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     3227 2024-04-17 09:26:10.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/general_functions.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5664 2024-04-26 19:59:40.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/geo_pandas.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     1464 2024-04-26 00:28:54.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/geo_spec.py
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)     5426 2024-04-08 17:04:56.000000 abstract_pandas-0.0.0.2/src/abstract_pandas/time_module.py
+drwxrwxr-x   0 gamook    (1000) gamook    (1000)        0 2024-04-29 21:25:29.910421 abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/
+-rw-r--r--   0 gamook    (1000) gamook    (1000)      610 2024-04-29 21:25:29.000000 abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/PKG-INFO
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)      512 2024-04-29 21:25:29.000000 abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)        1 2024-04-29 21:25:29.000000 abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       62 2024-04-29 21:25:29.000000 abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/requires.txt
+-rw-rw-r--   0 gamook    (1000) gamook    (1000)       16 2024-04-29 21:25:29.000000 abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/top_level.txt
```

### Comparing `abstract_pandas-0.0.0.1/PKG-INFO` & `abstract_pandas-0.0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.0.1
+Version: 0.0.0.2
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.0.1/setup.py` & `abstract_pandas-0.0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name='abstract_pandas',
-    version='0.0.0.1',
+    version='0.0.0.2',
     author='putkoff',
     author_email='partners@abstractendeavors.com',
     description="",
     long_description=long_description,
     long_description_content_type='text/markdown',
     classifiers=[
           'Development Status :: 3 - Alpha',
```

### Comparing `abstract_pandas-0.0.0.1/src/abstract_pandas/excel_gui.py` & `abstract_pandas-0.0.0.2/src/abstract_pandas/excel_gui.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.1/src/abstract_pandas/excel_module.py` & `abstract_pandas-0.0.0.2/src/abstract_pandas/excel_module.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,30 @@
 from odf import text, teletype
 from odf.opendocument import load
 from .general_functions import *
 from datetime import datetime
 from itertools import permutations
 from difflib import get_close_matches
 from datetime import datetime
+import pandas as pd
+from pyxlsb import open_workbook
+
+
+
+# Example usage
+
+print(df)
+def read_xlsb_to_dataframe(file_path, sheet_name):
+    data = []
+    with open_workbook(file_path) as wb:
+        with wb.get_sheet(sheet_name) as sheet:
+            for row in sheet.rows():
+                data.append([cell.v for cell in row])
+    # Create a DataFrame
+    return pd.DataFrame(data)
 def safe_excel_save(df,original_file_path,index=False, engine='openpyxl'):
     with tempfile.NamedTemporaryFile(delete=False, suffix='.xlsx') as tmp:
         temp_file_name = tmp.name
         df.to_excel(tmp.name, index=index, engine=engine)  # Save your DataFrame to the temp file
     if os.path.getsize(temp_file_name) > 0:
         shutil.move(temp_file_name, original_file_path)
     else:
@@ -166,15 +182,16 @@
                 return pd.read_csv(source)
             elif file_ext == '.ods':
                 return read_ods(source)
             elif file_ext in ('.xlsx', '.xls'):
                 return pd.read_excel(source, engine='openpyxl')
             elif file_ext == '.tsv':  # Handle TSV files
                 return pd.read_csv(source, sep='\t')
-
+            elif file_ext=='.xlsb':
+                return read_xlsb_to_dataframe(source, 'Sheet1')
         except Exception as e:
             print(f"Failed to read file: {e}")
     elif isinstance(source, FileStorage):  # Check if source is a FileStorage object
         try:
             # Read the file directly from the file object
             return pd.read_excel(source)
         except Exception as e:
```

### Comparing `abstract_pandas-0.0.0.1/src/abstract_pandas/general_functions.py` & `abstract_pandas-0.0.0.2/src/abstract_pandas/general_functions.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.1/src/abstract_pandas/geo_pandas.py` & `abstract_pandas-0.0.0.2/src/abstract_pandas/geo_pandas.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.1/src/abstract_pandas/geo_spec.py` & `abstract_pandas-0.0.0.2/src/abstract_pandas/geo_spec.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.1/src/abstract_pandas/time_module.py` & `abstract_pandas-0.0.0.2/src/abstract_pandas/time_module.py`

 * *Files identical despite different names*

### Comparing `abstract_pandas-0.0.0.1/src/abstract_pandas.egg-info/PKG-INFO` & `abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_pandas
-Version: 0.0.0.1
+Version: 0.0.0.2
 Author: putkoff
 Author-email: partners@abstractendeavors.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `abstract_pandas-0.0.0.1/src/abstract_pandas.egg-info/SOURCES.txt` & `abstract_pandas-0.0.0.2/src/abstract_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

