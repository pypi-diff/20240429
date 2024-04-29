# Comparing `tmp/dataframe_short-0.1.3.tar.gz` & `tmp/dataframe_short-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataframe_short-0.1.3.tar", last modified: Mon Apr 29 03:46:48 2024, max compression
+gzip compressed data, was "dataframe_short-0.1.4.tar", last modified: Mon Apr 29 04:42:19 2024, max compression
```

## Comparing `dataframe_short-0.1.3.tar` & `dataframe_short-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 03:46:48.900497 dataframe_short-0.1.3/
--rw-rw-rw-   0        0        0      255 2024-04-29 03:46:48.899501 dataframe_short-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 03:46:48.891522 dataframe_short-0.1.3/dataframe_short/
--rw-rw-rw-   0        0        0      119 2024-04-29 03:46:02.000000 dataframe_short-0.1.3/dataframe_short/__init__.py
--rw-rw-rw-   0        0        0     7711 2024-03-17 03:24:34.000000 dataframe_short-0.1.3/dataframe_short/dataframe_test.py
--rw-rw-rw-   0        0        0     2803 2024-03-11 03:40:50.000000 dataframe_short-0.1.3/dataframe_short/func_24_Feb.py
--rw-rw-rw-   0        0        0    49343 2024-04-29 03:45:09.000000 dataframe_short-0.1.3/dataframe_short/lib02_dataframe.py
-drwxrwxrwx   0        0        0        0 2024-04-29 03:46:48.898503 dataframe_short-0.1.3/dataframe_short.egg-info/
--rw-rw-rw-   0        0        0      255 2024-04-29 03:46:48.000000 dataframe_short-0.1.3/dataframe_short.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-29 03:46:48.000000 dataframe_short-0.1.3/dataframe_short.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 03:46:48.000000 dataframe_short-0.1.3/dataframe_short.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-29 03:46:48.000000 dataframe_short-0.1.3/dataframe_short.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 03:46:48.901496 dataframe_short-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      362 2024-04-29 03:45:52.000000 dataframe_short-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:42:19.654199 dataframe_short-0.1.4/
+-rw-rw-rw-   0        0        0      333 2024-04-29 04:42:19.654199 dataframe_short-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 04:42:19.644225 dataframe_short-0.1.4/dataframe_short/
+-rw-rw-rw-   0        0        0      119 2024-04-29 04:42:11.000000 dataframe_short-0.1.4/dataframe_short/__init__.py
+-rw-rw-rw-   0        0        0     7713 2024-04-29 04:40:51.000000 dataframe_short-0.1.4/dataframe_short/dataframe_test.py
+-rw-rw-rw-   0        0        0     2803 2024-03-11 03:40:50.000000 dataframe_short-0.1.4/dataframe_short/func_24_Feb.py
+-rw-rw-rw-   0        0        0    49373 2024-04-29 04:41:04.000000 dataframe_short-0.1.4/dataframe_short/lib02_dataframe.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:42:19.652203 dataframe_short-0.1.4/dataframe_short.egg-info/
+-rw-rw-rw-   0        0        0      333 2024-04-29 04:42:19.000000 dataframe_short-0.1.4/dataframe_short.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-29 04:42:19.000000 dataframe_short-0.1.4/dataframe_short.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 04:42:19.000000 dataframe_short-0.1.4/dataframe_short.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-29 04:42:19.000000 dataframe_short-0.1.4/dataframe_short.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 04:42:19.654199 dataframe_short-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      379 2024-04-29 04:42:00.000000 dataframe_short-0.1.4/setup.py
```

### Comparing `dataframe_short-0.1.3/dataframe_short/dataframe_test.py` & `dataframe_short-0.1.4/dataframe_short/dataframe_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-import lib02_dataframe as ds
+# import lib02_dataframe as ds
 import pandas as pd
 
 class Test_df_value_index(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         # Setup data once for all tests in this class
         cls.dict01 = {'A': [1, 2, 3], 'B': [4, 5, 1], 'C': [7, 1, 9]}
```

### Comparing `dataframe_short-0.1.3/dataframe_short/func_24_Feb.py` & `dataframe_short-0.1.4/dataframe_short/func_24_Feb.py`

 * *Files identical despite different names*

### Comparing `dataframe_short-0.1.3/dataframe_short/lib02_dataframe.py` & `dataframe_short-0.1.4/dataframe_short/lib02_dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import pandas as pd
 import numpy as np
 from itertools import product
 from collections import defaultdict
 import sys
 
 # from lib01_xgb import *
-import string_01 as pst
-
+# import string_01 as pst
+import py_string_tool as pst
 
 def indexAlignedAppend(df1, df2, col_name):
     # it works: medium tested
     import pandas as pd
     """
     Appends rows from df2 to df1 based on a specific column (col_name).
     And readjust the index in each episode via (col_name)
```

