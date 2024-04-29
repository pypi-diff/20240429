# Comparing `tmp/way2dssat-0.0.2.tar.gz` & `tmp/way2dssat-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "way2dssat-0.0.2.tar", last modified: Sun Apr 28 20:15:01 2024, max compression
+gzip compressed data, was "way2dssat-0.0.3.tar", last modified: Mon Apr 29 04:10:27 2024, max compression
```

## Comparing `way2dssat-0.0.2.tar` & `way2dssat-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-28 20:15:01.626786 way2dssat-0.0.2/
--rw-rw-rw-   0        0        0      668 2024-04-28 20:15:01.626786 way2dssat-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       67 2024-04-28 03:48:31.000000 way2dssat-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-28 20:15:01.550647 way2dssat-0.0.2/Way2DSSAT/
--rw-rw-rw-   0        0        0       45 2024-04-28 05:36:43.000000 way2dssat-0.0.2/Way2DSSAT/__init__.py
--rw-rw-rw-   0        0        0     6836 2024-04-28 06:15:03.000000 way2dssat-0.0.2/Way2DSSAT/gssurgo2soil.py
-drwxrwxrwx   0        0        0        0 2024-04-28 20:15:01.626786 way2dssat-0.0.2/Way2DSSAT.egg-info/
--rw-rw-rw-   0        0        0      668 2024-04-28 20:15:01.000000 way2dssat-0.0.2/Way2DSSAT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-28 20:15:01.000000 way2dssat-0.0.2/Way2DSSAT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-28 20:15:01.000000 way2dssat-0.0.2/Way2DSSAT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-28 20:15:01.000000 way2dssat-0.0.2/Way2DSSAT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-28 20:15:01.000000 way2dssat-0.0.2/Way2DSSAT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      699 2024-04-28 20:14:05.000000 way2dssat-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-28 20:15:01.641797 way2dssat-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      476 2024-04-28 06:04:18.000000 way2dssat-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:10:27.589323 way2dssat-0.0.3/
+-rw-rw-rw-   0        0        0      668 2024-04-29 04:10:27.587499 way2dssat-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2024-04-28 03:48:31.000000 way2dssat-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 04:10:27.548720 way2dssat-0.0.3/Way2DSSAT/
+-rw-rw-rw-   0        0        0      803 2024-04-29 04:00:36.000000 way2dssat-0.0.3/Way2DSSAT/__init__.py
+-rw-rw-rw-   0        0        0     6847 2024-04-29 04:03:05.000000 way2dssat-0.0.3/Way2DSSAT/gssurgo2soil.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:10:27.579969 way2dssat-0.0.3/Way2DSSAT.egg-info/
+-rw-rw-rw-   0        0        0      668 2024-04-29 04:10:27.000000 way2dssat-0.0.3/Way2DSSAT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-29 04:10:27.000000 way2dssat-0.0.3/Way2DSSAT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 04:10:27.000000 way2dssat-0.0.3/Way2DSSAT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-29 04:10:27.000000 way2dssat-0.0.3/Way2DSSAT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-29 04:10:27.000000 way2dssat-0.0.3/Way2DSSAT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      699 2024-04-29 04:09:30.000000 way2dssat-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 04:10:27.589323 way2dssat-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      476 2024-04-28 06:04:18.000000 way2dssat-0.0.3/setup.py
```

### Comparing `way2dssat-0.0.2/PKG-INFO` & `way2dssat-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Way2DSSAT
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package to handle input output files
 Author: Manavjot Singh
 Author-email: Manavjot <manavjotsingh97@gmail.com>
 Project-URL: Homepage, https://github.com/ManavjotSingh97/Way2DSSAT
 Project-URL: Issues, https://github.com/ManavjotSingh97/Way2DSSAT/issues
 Keywords: python,DSSAT,Input,gSSURGO
 Classifier: Programming Language :: Python :: 3
```

### Comparing `way2dssat-0.0.2/Way2DSSAT/gssurgo2soil.py` & `way2dssat-0.0.3/Way2DSSAT/gssurgo2soil.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 def SOL(path,path2):
     import pandas
     import math
-    """
+"""
     Converts gSSURGO format into DSSAT .SOL format.
     
     Inputs
     ------
         path: string
             path to your .csv file containing the data from gSSURGO. Must have the following columns(and other related depths)
             WC15Bar_DCP_0to5
@@ -17,20 +17,22 @@
             Db3rdbar_DCP_0to5
             Ksat_DCP_0to5
             OrgMatter_DCP_0to5
             MUKEY_DCP_0to5
         
         path2: string
             path where u want to save files
-        Example: 
+            
+    Example 
+    -------
             path = 'Username/pathtothecsv'
             path2 = 'Username/pathtosavingfolder'
             ssurgo2soil(path,path2)
             
-    """
+"""
     #Reading csv  
     
     df_soil = pandas.read_csv(path)
     #Returns list of columns not required with specific keyword
     # data from ssurgo contains columns suchas pct_Silt** which aren't required
     # Removing those columns form the dataframe
     # These have column name are duplicate of the required soil properties with additional pct in 
@@ -105,15 +107,14 @@
     # SCEC     Cation exchange capacity, cmol kg-1                                 
     # SADC     Anion adsorption coefficient (reduced nitrate flow), cm3 
     # Writing lines to the text documents
 
     #Initialize empty string
     Soil=''
 
-
     for j in range(0,len(df)):
         Mukey = df[Mukey_columns].loc[j,Mukey_columns[0]]
         # Appending teh empty string
         Soil+=line1
         Soil+=line2
         Soil+=f'*IIE{Mukey:>7}  SSURGO      CL         200 seriesname can have spaces upto this length but ca\n'
         Soil+=line4
@@ -130,23 +131,23 @@
         SLNI = '-99'
         SLHB= '-99'
         SADC = '-99'
 
         for i in range(0,len(SLCL_columns)):
             SLB =int(SLCL_columns[i].split('to')[1]) #DEPTH
 
-            SLLL=round(df[SLLL_columns].loc[0,SLLL_columns[i]]/100,3) 
-            SDUL=round(df[SDUL_columns].loc[0,SDUL_columns[i]]/100,3)
-            SLCL=round(df[SLCL_columns].loc[0,SLCL_columns[i]],1)
-            SLSI=round(df[SLSI_columns].loc[0,SLSI_columns[i]],1)
+            SLLL=round(df[SLLL_columns].loc[j,SLLL_columns[i]]/100,3) 
+            SDUL=round(df[SDUL_columns].loc[j,SDUL_columns[i]]/100,3)
+            SLCL=round(df[SLCL_columns].loc[j,SLCL_columns[i]],1)
+            SLSI=round(df[SLSI_columns].loc[j,SLSI_columns[i]],1)
             SSAT= round(0.3332 + (-0.000725)*(SLSI)+0.12768*math.log10(SLCL) , 3) #from DSSAT mannual
-            SLHW=round(df[SLHW_columns].loc[0,SLHW_columns[i]],3)
-            SCEC=round(df[SCEC_columns].loc[0,SCEC_columns[i]],3)
-            SBDM= round(df[SBDM_columns].loc[0,SBDM_columns[i]],3)
-            SSKS=round(df[SSKS_columns].loc[0,SSKS_columns[i]]*0.36,2) #from micrometer /second to cm /hour
-            SLOC=round(df[SLOC_columns].loc[0,SLOC_columns[i]],3)
+            SLHW=round(df[SLHW_columns].loc[j,SLHW_columns[i]],3)
+            SCEC=round(df[SCEC_columns].loc[j,SCEC_columns[i]],3)
+            SBDM= round(df[SBDM_columns].loc[j,SBDM_columns[i]],3)
+            SSKS=round(df[SSKS_columns].loc[j,SSKS_columns[i]]*0.36,2) #from micrometer /second to cm /hour
+            SLOC=round(df[SLOC_columns].loc[j,SLOC_columns[i]],3)
             Soil+= f'{SLB:>6}{SLMH:>6}{SLLL:>6}{SDUL:>6}{SSAT:>6}{SRGF:>6}{SSKS:>6}{SBDM:>6}{SLOC:>6}{SLCL:>6}{SLSI:>6}{SLCF:>6}{SLNI:>6}{SLHW:>6}{SLHB:>6}{SCEC:>6}{SADC:>6}\n'
         Soil+='\n'     
     # Write to a .SOL file
     destination=path2
     with open(f'{destination}SG.SOL', 'w') as file:
         file.write(Soil)
```

### Comparing `way2dssat-0.0.2/Way2DSSAT.egg-info/PKG-INFO` & `way2dssat-0.0.3/Way2DSSAT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Way2DSSAT
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package to handle input output files
 Author: Manavjot Singh
 Author-email: Manavjot <manavjotsingh97@gmail.com>
 Project-URL: Homepage, https://github.com/ManavjotSingh97/Way2DSSAT
 Project-URL: Issues, https://github.com/ManavjotSingh97/Way2DSSAT/issues
 Keywords: python,DSSAT,Input,gSSURGO
 Classifier: Programming Language :: Python :: 3
```

### Comparing `way2dssat-0.0.2/pyproject.toml` & `way2dssat-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0","pandas"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dependencies = [ "pandas"]
 name = "Way2DSSAT"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Manavjot", email="manavjotsingh97@gmail.com" },
 ]
 description = "Package to handle input output files"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

