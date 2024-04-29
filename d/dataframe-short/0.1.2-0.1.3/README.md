# Comparing `tmp/dataframe_short-0.1.2.tar.gz` & `tmp/dataframe_short-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataframe_short-0.1.2.tar", last modified: Mon Apr 29 03:37:57 2024, max compression
+gzip compressed data, was "dataframe_short-0.1.3.tar", last modified: Mon Apr 29 03:46:48 2024, max compression
```

## Comparing `dataframe_short-0.1.2.tar` & `dataframe_short-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 03:37:57.877388 dataframe_short-0.1.2/
--rw-rw-rw-   0        0        0      255 2024-04-29 03:37:57.876391 dataframe_short-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-29 03:37:57.863426 dataframe_short-0.1.2/dataframe_short/
--rw-rw-rw-   0        0        0      119 2024-04-29 03:35:00.000000 dataframe_short-0.1.2/dataframe_short/__init__.py
--rw-rw-rw-   0        0        0     7711 2024-03-17 03:24:34.000000 dataframe_short-0.1.2/dataframe_short/dataframe_test.py
--rw-rw-rw-   0        0        0     2803 2024-03-11 03:40:50.000000 dataframe_short-0.1.2/dataframe_short/func_24_Feb.py
--rw-rw-rw-   0        0        0    49641 2024-04-29 01:56:48.000000 dataframe_short-0.1.2/dataframe_short/lib02_dataframe.py
-drwxrwxrwx   0        0        0        0 2024-04-29 03:37:57.874396 dataframe_short-0.1.2/dataframe_short.egg-info/
--rw-rw-rw-   0        0        0      255 2024-04-29 03:37:57.000000 dataframe_short-0.1.2/dataframe_short.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-29 03:37:57.000000 dataframe_short-0.1.2/dataframe_short.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 03:37:57.000000 dataframe_short-0.1.2/dataframe_short.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-29 03:37:57.000000 dataframe_short-0.1.2/dataframe_short.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-29 03:37:57.877388 dataframe_short-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      362 2024-04-29 03:34:55.000000 dataframe_short-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:46:48.900497 dataframe_short-0.1.3/
+-rw-rw-rw-   0        0        0      255 2024-04-29 03:46:48.899501 dataframe_short-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-29 03:46:48.891522 dataframe_short-0.1.3/dataframe_short/
+-rw-rw-rw-   0        0        0      119 2024-04-29 03:46:02.000000 dataframe_short-0.1.3/dataframe_short/__init__.py
+-rw-rw-rw-   0        0        0     7711 2024-03-17 03:24:34.000000 dataframe_short-0.1.3/dataframe_short/dataframe_test.py
+-rw-rw-rw-   0        0        0     2803 2024-03-11 03:40:50.000000 dataframe_short-0.1.3/dataframe_short/func_24_Feb.py
+-rw-rw-rw-   0        0        0    49343 2024-04-29 03:45:09.000000 dataframe_short-0.1.3/dataframe_short/lib02_dataframe.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:46:48.898503 dataframe_short-0.1.3/dataframe_short.egg-info/
+-rw-rw-rw-   0        0        0      255 2024-04-29 03:46:48.000000 dataframe_short-0.1.3/dataframe_short.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-29 03:46:48.000000 dataframe_short-0.1.3/dataframe_short.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 03:46:48.000000 dataframe_short-0.1.3/dataframe_short.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-29 03:46:48.000000 dataframe_short-0.1.3/dataframe_short.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 03:46:48.901496 dataframe_short-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      362 2024-04-29 03:45:52.000000 dataframe_short-0.1.3/setup.py
```

### Comparing `dataframe_short-0.1.2/dataframe_short/dataframe_test.py` & `dataframe_short-0.1.3/dataframe_short/dataframe_test.py`

 * *Files identical despite different names*

### Comparing `dataframe_short-0.1.2/dataframe_short/func_24_Feb.py` & `dataframe_short-0.1.3/dataframe_short/func_24_Feb.py`

 * *Files identical despite different names*

### Comparing `dataframe_short-0.1.2/dataframe_short/lib02_dataframe.py` & `dataframe_short-0.1.3/dataframe_short/lib02_dataframe.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @author: Heng2020
 """
 import pandas as pd
 import numpy as np
 from itertools import product
 from collections import defaultdict
 import sys
-sys.path.append(r"C:\Users\Heng2020\OneDrive\Python MyLib\Python MyLib 01\11 String")
+
 # from lib01_xgb import *
 import string_01 as pst
 
 
 def indexAlignedAppend(df1, df2, col_name):
     # it works: medium tested
     import pandas as pd
@@ -79,19 +79,16 @@
 
         ):
     import pandas as pd
     import re
     import os
 
     import sys
-    sys.path.append(r'C:\Users\Heng2020\OneDrive\Python MyLib\Python MyLib 01\02 DataFrame')
-    sys.path.append(r'C:\Users\Heng2020\OneDrive\Python MyLib\Python MyLib 01\10 OS')
+    import os_toolkit as ost
 
-    import os_01 as ost
-    import lib02_dataframe as ds
     
     if not os.path.isdir(folder_path):
         print("This is not the correct folder path")
         return False
 
 
     path_list = ost.get_full_filename(folder_path,extension=[".xlsx",".csv"])
@@ -103,15 +100,15 @@
 
         if extract_pattern is None:
             name_filter = filename
         else:
             name_filter = re.search(extract_pattern, filename).group()
         # curr_df.columns.values[0] = 'NoSentence'
         curr_df[filename_col_name] = name_filter
-        ds.pd_move_col_front(curr_df, filename_col_name)
+        pd_move_col_front(curr_df, filename_col_name)
         out_df = pd.concat([out_df,curr_df])
 
     return out_df
 
 
 # ########################################## imported from work Mar 17, 2024 #######################################################################
 def df_to_str_decimal(df,cols,decimal_place = 1, inplace = True, except_level = []):
```

