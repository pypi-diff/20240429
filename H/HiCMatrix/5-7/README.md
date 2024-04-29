# Comparing `tmp/HiCMatrix-5.tar.gz` & `tmp/HiCMatrix-7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/HiCMatrix-5.tar", last modified: Thu Dec  6 11:16:43 2018, max compression
+gzip compressed data, was "dist/HiCMatrix-7.tar", last modified: Wed Feb 13 11:15:44 2019, max compression
```

## Comparing `HiCMatrix-5.tar` & `HiCMatrix-7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 wolffj    (1000) wolffj    (1000)        0 2018-12-06 11:16:43.000000 HiCMatrix-5/
-drwxrwxr-x   0 wolffj    (1000) wolffj    (1000)        0 2018-12-06 11:16:43.000000 HiCMatrix-5/HiCMatrix.egg-info/
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)      106 2018-12-06 11:16:43.000000 HiCMatrix-5/HiCMatrix.egg-info/requires.txt
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)       10 2018-12-06 11:16:43.000000 HiCMatrix-5/HiCMatrix.egg-info/top_level.txt
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     1205 2018-12-06 11:16:43.000000 HiCMatrix-5/HiCMatrix.egg-info/PKG-INFO
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)        1 2018-12-06 11:16:43.000000 HiCMatrix-5/HiCMatrix.egg-info/dependency_links.txt
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)      514 2018-12-06 11:16:43.000000 HiCMatrix-5/HiCMatrix.egg-info/SOURCES.txt
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)        1 2018-09-03 10:11:00.000000 HiCMatrix-5/HiCMatrix.egg-info/not-zip-safe
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     1205 2018-12-06 11:16:43.000000 HiCMatrix-5/PKG-INFO
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     3848 2018-09-25 10:33:47.000000 HiCMatrix-5/setup.py
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)       38 2018-12-06 11:16:43.000000 HiCMatrix-5/setup.cfg
-drwxrwxr-x   0 wolffj    (1000) wolffj    (1000)        0 2018-12-06 11:16:43.000000 HiCMatrix-5/hicmatrix/
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)       55 2018-12-06 11:12:11.000000 HiCMatrix-5/hicmatrix/__init__.py
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)       61 2018-12-06 11:12:22.000000 HiCMatrix-5/hicmatrix/_version.py
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     2911 2018-09-25 10:33:47.000000 HiCMatrix-5/hicmatrix/utilities.py
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)    40777 2018-12-06 11:12:22.000000 HiCMatrix-5/hicmatrix/HiCMatrix.py
-drwxrwxr-x   0 wolffj    (1000) wolffj    (1000)        0 2018-12-06 11:16:43.000000 HiCMatrix-5/hicmatrix/lib/
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     2265 2018-12-06 11:12:22.000000 HiCMatrix-5/hicmatrix/lib/homer.py
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     7396 2018-12-06 11:12:22.000000 HiCMatrix-5/hicmatrix/lib/h5.py
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)       63 2018-09-25 10:33:46.000000 HiCMatrix-5/hicmatrix/lib/__init__.py
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)    10343 2018-12-06 11:12:22.000000 HiCMatrix-5/hicmatrix/lib/cool.py
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     1035 2018-09-25 10:33:46.000000 HiCMatrix-5/hicmatrix/lib/ginteractions.py
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     1223 2018-09-25 10:33:46.000000 HiCMatrix-5/hicmatrix/lib/hicpro.py
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     2234 2018-12-06 11:12:22.000000 HiCMatrix-5/hicmatrix/lib/matrixFileHandler.py
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)      870 2018-09-25 10:33:46.000000 HiCMatrix-5/hicmatrix/lib/matrixFile.py
--rw-rw-r--   0 wolffj    (1000) wolffj    (1000)      527 2018-12-06 11:12:22.000000 HiCMatrix-5/README.rst
+drwxrwxr-x   0 wolffj    (1000) wolffj    (1000)        0 2019-02-13 11:15:44.000000 HiCMatrix-7/
+drwxrwxr-x   0 wolffj    (1000) wolffj    (1000)        0 2019-02-13 11:15:44.000000 HiCMatrix-7/HiCMatrix.egg-info/
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)      105 2019-02-13 11:15:44.000000 HiCMatrix-7/HiCMatrix.egg-info/requires.txt
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)       10 2019-02-13 11:15:44.000000 HiCMatrix-7/HiCMatrix.egg-info/top_level.txt
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     1171 2019-02-13 11:15:44.000000 HiCMatrix-7/HiCMatrix.egg-info/PKG-INFO
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)        1 2019-02-13 11:15:44.000000 HiCMatrix-7/HiCMatrix.egg-info/dependency_links.txt
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)      514 2019-02-13 11:15:44.000000 HiCMatrix-7/HiCMatrix.egg-info/SOURCES.txt
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)        1 2019-02-13 11:15:44.000000 HiCMatrix-7/HiCMatrix.egg-info/not-zip-safe
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     1171 2019-02-13 11:15:44.000000 HiCMatrix-7/PKG-INFO
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     3847 2019-02-13 11:15:01.000000 HiCMatrix-7/setup.py
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)       38 2019-02-13 11:15:44.000000 HiCMatrix-7/setup.cfg
+drwxrwxr-x   0 wolffj    (1000) wolffj    (1000)        0 2019-02-13 11:15:44.000000 HiCMatrix-7/hicmatrix/
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)       55 2019-02-13 11:15:01.000000 HiCMatrix-7/hicmatrix/__init__.py
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)       61 2019-02-13 11:15:01.000000 HiCMatrix-7/hicmatrix/_version.py
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     2911 2019-02-13 11:15:01.000000 HiCMatrix-7/hicmatrix/utilities.py
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)    40777 2019-02-13 11:15:01.000000 HiCMatrix-7/hicmatrix/HiCMatrix.py
+drwxrwxr-x   0 wolffj    (1000) wolffj    (1000)        0 2019-02-13 11:15:44.000000 HiCMatrix-7/hicmatrix/lib/
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     2265 2019-02-13 11:15:01.000000 HiCMatrix-7/hicmatrix/lib/homer.py
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     7396 2019-02-13 11:15:01.000000 HiCMatrix-7/hicmatrix/lib/h5.py
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)       63 2019-02-13 11:15:01.000000 HiCMatrix-7/hicmatrix/lib/__init__.py
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)    10705 2019-02-13 11:15:01.000000 HiCMatrix-7/hicmatrix/lib/cool.py
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     1035 2019-02-13 11:15:01.000000 HiCMatrix-7/hicmatrix/lib/ginteractions.py
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     1223 2019-02-13 11:15:01.000000 HiCMatrix-7/hicmatrix/lib/hicpro.py
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)     2234 2019-02-13 11:15:01.000000 HiCMatrix-7/hicmatrix/lib/matrixFileHandler.py
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)      870 2019-02-13 11:15:01.000000 HiCMatrix-7/hicmatrix/lib/matrixFile.py
+-rw-rw-r--   0 wolffj    (1000) wolffj    (1000)      527 2019-02-13 11:15:01.000000 HiCMatrix-7/README.rst
```

### Comparing `HiCMatrix-5/HiCMatrix.egg-info/PKG-INFO` & `HiCMatrix-7/HiCMatrix.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: HiCMatrix
-Version: 5
+Version: 7
 Summary: Helper package which implements HiCMatrix class for HiCExplorer and pyGenomeTracks
 Home-page: https://github.com/deeptools/HiCMatrix
 Author: Fidel Ramirez, Vivek Bhardwaj, Björn Grüning, Joachim Wolff
 Author-email: deeptools@googlegroups.com
 License: LICENSE.txt
-Description-Content-Type: UNKNOWN
 Description: HiCMatrix
         ===========
         
         This library implements the central class of HiCExplorer to manage Hi-C interaction matrices. It is separated from the main project to enable to use of Hi-C matrices
         in other project without the dependency to HiCExplorer. Moreover, it enables us to use the already separated pyGenomeTracks (former hicPlotTADs) to be used in HiCExplorer
         because mutual dependencies are resolved.
```

### Comparing `HiCMatrix-5/HiCMatrix.egg-info/SOURCES.txt` & `HiCMatrix-7/HiCMatrix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HiCMatrix-5/PKG-INFO` & `HiCMatrix-7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: HiCMatrix
-Version: 5
+Version: 7
 Summary: Helper package which implements HiCMatrix class for HiCExplorer and pyGenomeTracks
 Home-page: https://github.com/deeptools/HiCMatrix
 Author: Fidel Ramirez, Vivek Bhardwaj, Björn Grüning, Joachim Wolff
 Author-email: deeptools@googlegroups.com
 License: LICENSE.txt
-Description-Content-Type: UNKNOWN
 Description: HiCMatrix
         ===========
         
         This library implements the central class of HiCExplorer to manage Hi-C interaction matrices. It is separated from the main project to enable to use of Hi-C matrices
         in other project without the dependency to HiCExplorer. Moreover, it enables us to use the already separated pyGenomeTracks (former hicPlotTADs) to be used in HiCExplorer
         because mutual dependencies are resolved.
```

### Comparing `HiCMatrix-5/setup.py` & `HiCMatrix-7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
 
 install_requires_py = ["numpy >= 1.13.*",
                        "scipy >= 1.1.*",
                        "tables >= 3.4.*",
                        "pandas >= 0.23.*",
                        "future >= 0.16.*",
-                       "cooler == 0.7.11",
+                       "cooler == 0.8.2",
                        "intervaltree == 2.1.*"
                        ]
 
 setup(
     name='HiCMatrix',
     version=get_version(),
     author='Fidel Ramirez, Vivek Bhardwaj, Björn Grüning, Joachim Wolff',
```

### Comparing `HiCMatrix-5/hicmatrix/utilities.py` & `HiCMatrix-7/hicmatrix/utilities.py`

 * *Files identical despite different names*

### Comparing `HiCMatrix-5/hicmatrix/HiCMatrix.py` & `HiCMatrix-7/hicmatrix/HiCMatrix.py`

 * *Files identical despite different names*

### Comparing `HiCMatrix-5/hicmatrix/lib/homer.py` & `HiCMatrix-7/hicmatrix/lib/homer.py`

 * *Files identical despite different names*

### Comparing `HiCMatrix-5/hicmatrix/lib/h5.py` & `HiCMatrix-7/hicmatrix/lib/h5.py`

 * *Files identical despite different names*

### Comparing `HiCMatrix-5/hicmatrix/lib/cool.py` & `HiCMatrix-7/hicmatrix/lib/cool.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import cooler
 import logging
 import numpy as np
 from scipy.sparse import triu, csr_matrix
 import pandas as pd
 from past.builtins import zip
 from builtins import super
@@ -32,15 +33,15 @@
             log.info('No matrix is initalized')
 
         try:
             cooler_file = cooler.Cooler(self.matrixFileName)
         except Exception:
             log.info("Could not open cooler file. Maybe the path is wrong or the given node is not available.")
             log.info('The following file was tried to open: {}'.format(self.matrixFileName))
-            log.info("The following nodes are available: {}".format(cooler.io.ls(self.matrixFileName.split("::")[0])))
+            log.info("The following nodes are available: {}".format(cooler.fileops.list_coolers(self.matrixFileName.split("::")[0])))
             exit()
 
         if self.chrnameList is None:
             matrixDataFrame = cooler_file.matrix(balance=False, sparse=True, as_pixels=True)
             used_dtype = np.int32
             if np.iinfo(np.int32).max < cooler_file.info['nbins']:
                 used_dtype = np.int64
@@ -50,17 +51,18 @@
             features = np.empty(cooler_file.info['nnz'], dtype=used_dtype)
             i = 0
             size = cooler_file.info['nbins'] // 32
             if size == 0:
                 size = 1
             start_pos = 0
             while i < cooler_file.info['nbins']:
-                _data = matrixDataFrame[i:i + size]['count'].values.astype(count_dtype).T
-                _instances = matrixDataFrame[i:i + size]['bin1_id'].values.astype(used_dtype).T
-                _features = matrixDataFrame[i:i + size]['bin2_id'].values.astype(used_dtype).T
+                matrixDataFrameChunk = matrixDataFrame[i:i + size]
+                _data = matrixDataFrameChunk['count'].values.astype(count_dtype)
+                _instances = matrixDataFrameChunk['bin1_id'].values.astype(used_dtype)
+                _features = matrixDataFrameChunk['bin2_id'].values.astype(used_dtype)
 
                 data[start_pos:start_pos + len(_data)] = _data
                 instances[start_pos:start_pos + len(_instances)] = _instances
                 features[start_pos:start_pos + len(_features)] = _features
                 start_pos += len(_features)
                 i += size
 
@@ -226,12 +228,20 @@
             log.warning("Writing non-standard cooler matrix. Datatype of matrix['count'] is: {}".format(self.matrix.dtype))
             dtype_pixel['count'] = self.matrix.dtype
         split_factor = 1
         if len(self.matrix.data) > 1e7:
             split_factor = 1e4
             matrix_data_frame = np.array_split(matrix_data_frame, split_factor)
 
-        cooler.io.create(cool_uri=pFileName,
-                         bins=bins_data_frame,
-                         pixels=matrix_data_frame,
-                         append=self.appendData,
-                         dtype=dtype_pixel)
+        if self.appendData:
+            self.appendData = 'a'
+        else:
+            self.appendData = 'w'
+
+        local_temp_dir = os.path.dirname(os.path.realpath(pFileName))
+        cooler.create_cooler(cool_uri=pFileName,
+                             bins=bins_data_frame,
+                             pixels=matrix_data_frame,
+                             mode=self.appendData,
+                             dtypes=dtype_pixel,
+                             ordered=True,
+                             temp_dir=local_temp_dir)
```

### Comparing `HiCMatrix-5/hicmatrix/lib/ginteractions.py` & `HiCMatrix-7/hicmatrix/lib/ginteractions.py`

 * *Files identical despite different names*

### Comparing `HiCMatrix-5/hicmatrix/lib/hicpro.py` & `HiCMatrix-7/hicmatrix/lib/hicpro.py`

 * *Files identical despite different names*

### Comparing `HiCMatrix-5/hicmatrix/lib/matrixFileHandler.py` & `HiCMatrix-7/hicmatrix/lib/matrixFileHandler.py`

 * *Files identical despite different names*

### Comparing `HiCMatrix-5/hicmatrix/lib/matrixFile.py` & `HiCMatrix-7/hicmatrix/lib/matrixFile.py`

 * *Files identical despite different names*

### Comparing `HiCMatrix-5/README.rst` & `HiCMatrix-7/README.rst`

 * *Files identical despite different names*

