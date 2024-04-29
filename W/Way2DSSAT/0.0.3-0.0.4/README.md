# Comparing `tmp/way2dssat-0.0.3.tar.gz` & `tmp/way2dssat-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "way2dssat-0.0.3.tar", last modified: Mon Apr 29 04:10:27 2024, max compression
+gzip compressed data, was "way2dssat-0.0.4.tar", last modified: Mon Apr 29 04:30:51 2024, max compression
```

## Comparing `way2dssat-0.0.3.tar` & `way2dssat-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 04:10:27.589323 way2dssat-0.0.3/
--rw-rw-rw-   0        0        0      668 2024-04-29 04:10:27.587499 way2dssat-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       67 2024-04-28 03:48:31.000000 way2dssat-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 04:10:27.548720 way2dssat-0.0.3/Way2DSSAT/
--rw-rw-rw-   0        0        0      803 2024-04-29 04:00:36.000000 way2dssat-0.0.3/Way2DSSAT/__init__.py
--rw-rw-rw-   0        0        0     6847 2024-04-29 04:03:05.000000 way2dssat-0.0.3/Way2DSSAT/gssurgo2soil.py
-drwxrwxrwx   0        0        0        0 2024-04-29 04:10:27.579969 way2dssat-0.0.3/Way2DSSAT.egg-info/
--rw-rw-rw-   0        0        0      668 2024-04-29 04:10:27.000000 way2dssat-0.0.3/Way2DSSAT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-29 04:10:27.000000 way2dssat-0.0.3/Way2DSSAT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 04:10:27.000000 way2dssat-0.0.3/Way2DSSAT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-29 04:10:27.000000 way2dssat-0.0.3/Way2DSSAT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-29 04:10:27.000000 way2dssat-0.0.3/Way2DSSAT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      699 2024-04-29 04:09:30.000000 way2dssat-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 04:10:27.589323 way2dssat-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      476 2024-04-28 06:04:18.000000 way2dssat-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:30:51.517830 way2dssat-0.0.4/
+-rw-rw-rw-   0        0        0      668 2024-04-29 04:30:51.511809 way2dssat-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2024-04-28 03:48:31.000000 way2dssat-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 04:30:51.469609 way2dssat-0.0.4/Way2DSSAT/
+-rw-rw-rw-   0        0        0      811 2024-04-29 04:27:57.000000 way2dssat-0.0.4/Way2DSSAT/__init__.py
+-rw-rw-rw-   0        0        0     6858 2024-04-29 04:27:54.000000 way2dssat-0.0.4/Way2DSSAT/gssurgo2soil.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:30:51.511809 way2dssat-0.0.4/Way2DSSAT.egg-info/
+-rw-rw-rw-   0        0        0      668 2024-04-29 04:30:51.000000 way2dssat-0.0.4/Way2DSSAT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-29 04:30:51.000000 way2dssat-0.0.4/Way2DSSAT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 04:30:51.000000 way2dssat-0.0.4/Way2DSSAT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-29 04:30:51.000000 way2dssat-0.0.4/Way2DSSAT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-29 04:30:51.000000 way2dssat-0.0.4/Way2DSSAT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      699 2024-04-29 04:29:31.000000 way2dssat-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 04:30:51.517830 way2dssat-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      476 2024-04-28 06:04:18.000000 way2dssat-0.0.4/setup.py
```

### Comparing `way2dssat-0.0.3/PKG-INFO` & `way2dssat-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Way2DSSAT
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package to handle input output files
 Author: Manavjot Singh
 Author-email: Manavjot <manavjotsingh97@gmail.com>
 Project-URL: Homepage, https://github.com/ManavjotSingh97/Way2DSSAT
 Project-URL: Issues, https://github.com/ManavjotSingh97/Way2DSSAT/issues
 Keywords: python,DSSAT,Input,gSSURGO
 Classifier: Programming Language :: Python :: 3
```

### Comparing `way2dssat-0.0.3/Way2DSSAT/__init__.py` & `way2dssat-0.0.4/Way2DSSAT/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #init funciton
 
 from .gssurgo2soil import SOL
 
-"""
+    """
     Converts gSSURGO format into DSSAT .SOL format.
     
     Inputs
     ------
         path: string
             path to your .csv file containing the data from gSSURGO. Must have the following columns(and other related depths)
             WC15Bar_DCP_0to5
@@ -24,8 +24,8 @@
             path where u want to save files
     Example:
     --------
             path = 'Username/pathtothecsv'
             path2 = 'Username/pathtosavingfolder'
             ssurgo2soil(path,path2)
             
-"""
+    """
```

### Comparing `way2dssat-0.0.3/Way2DSSAT/gssurgo2soil.py` & `way2dssat-0.0.4/Way2DSSAT/gssurgo2soil.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 def SOL(path,path2):
+    
     import pandas
     import math
-"""
+    """
     Converts gSSURGO format into DSSAT .SOL format.
     
     Inputs
     ------
         path: string
             path to your .csv file containing the data from gSSURGO. Must have the following columns(and other related depths)
             WC15Bar_DCP_0to5
@@ -24,18 +25,18 @@
             
     Example 
     -------
             path = 'Username/pathtothecsv'
             path2 = 'Username/pathtosavingfolder'
             ssurgo2soil(path,path2)
             
-"""
+    """
     #Reading csv  
     
-    df_soil = pandas.read_csv(path)
+    df_soil=pandas.read_csv(path)
     #Returns list of columns not required with specific keyword
     # data from ssurgo contains columns suchas pct_Silt** which aren't required
     # Removing those columns form the dataframe
     # These have column name are duplicate of the required soil properties with additional pct in 
     # the name. Thus posing difficulty in calling the column name with keyword
     columns_not_req = list(df_soil.columns.array[list(df_soil.columns.str.contains('pct'))])
```

### Comparing `way2dssat-0.0.3/Way2DSSAT.egg-info/PKG-INFO` & `way2dssat-0.0.4/Way2DSSAT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Way2DSSAT
-Version: 0.0.3
+Version: 0.0.4
 Summary: Package to handle input output files
 Author: Manavjot Singh
 Author-email: Manavjot <manavjotsingh97@gmail.com>
 Project-URL: Homepage, https://github.com/ManavjotSingh97/Way2DSSAT
 Project-URL: Issues, https://github.com/ManavjotSingh97/Way2DSSAT/issues
 Keywords: python,DSSAT,Input,gSSURGO
 Classifier: Programming Language :: Python :: 3
```

### Comparing `way2dssat-0.0.3/pyproject.toml` & `way2dssat-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0","pandas"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = [ "pandas"]
 name = "Way2DSSAT"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Manavjot", email="manavjotsingh97@gmail.com" },
 ]
 description = "Package to handle input output files"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

