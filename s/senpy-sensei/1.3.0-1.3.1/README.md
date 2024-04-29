# Comparing `tmp/senpy_sensei-1.3.0-py3-none-any.whl.zip` & `tmp/senpy_sensei-1.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 20459 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat      136 b- defN 24-Apr-29 12:13 senpy/__init__.py
+Zip file size: 20458 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat      138 b- defN 24-Apr-29 12:51 senpy/__init__.py
 -rw-rw-rw-  2.0 fat     9839 b- defN 24-Apr-29 00:17 senpy/confidence.py
 -rw-rw-rw-  2.0 fat     4362 b- defN 24-Apr-29 00:17 senpy/log_logistic_funcs.py
 -rw-rw-rw-  2.0 fat     4591 b- defN 24-Apr-29 00:17 senpy/logistic_funcs.py
 -rw-rw-rw-  2.0 fat    30018 b- defN 24-Apr-29 00:17 senpy/neyer.py
 -rw-rw-rw-  2.0 fat     5255 b- defN 24-Apr-29 00:17 senpy/norm_funcs.py
 -rw-rw-rw-  2.0 fat     4269 b- defN 24-Apr-29 00:17 senpy/plotting.py
 -rw-rw-rw-  2.0 fat     1964 b- defN 24-Apr-29 00:17 senpy/utils.py
--rw-rw-rw-  2.0 fat     1086 b- defN 24-Apr-29 12:39 senpy_sensei-1.3.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2427 b- defN 24-Apr-29 12:39 senpy_sensei-1.3.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-29 12:39 senpy_sensei-1.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-29 12:39 senpy_sensei-1.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1016 b- defN 24-Apr-29 12:39 senpy_sensei-1.3.0.dist-info/RECORD
-13 files, 65061 bytes uncompressed, 18781 bytes compressed:  71.1%
+-rw-rw-rw-  2.0 fat     1086 b- defN 24-Apr-29 12:52 senpy_sensei-1.3.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2427 b- defN 24-Apr-29 12:52 senpy_sensei-1.3.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-29 12:52 senpy_sensei-1.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 24-Apr-29 12:52 senpy_sensei-1.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1016 b- defN 24-Apr-29 12:52 senpy_sensei-1.3.1.dist-info/RECORD
+13 files, 65063 bytes uncompressed, 18780 bytes compressed:  71.1%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: senpy/plotting.py
 Comment: 
 
 Filename: senpy/utils.py
 Comment: 
 
-Filename: senpy_sensei-1.3.0.dist-info/LICENSE
+Filename: senpy_sensei-1.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: senpy_sensei-1.3.0.dist-info/METADATA
+Filename: senpy_sensei-1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: senpy_sensei-1.3.0.dist-info/WHEEL
+Filename: senpy_sensei-1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: senpy_sensei-1.3.0.dist-info/top_level.txt
+Filename: senpy_sensei-1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: senpy_sensei-1.3.0.dist-info/RECORD
+Filename: senpy_sensei-1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## senpy/__init__.py

```diff
@@ -3,8 +3,8 @@
 Created on Sun Mar 22 17:28:13 2020
 
 @author: alexc
 """
 
 from . import neyer
 
-__version__ = 1.3.0
+__version__ = "1.3.1"
```

## Comparing `senpy_sensei-1.3.0.dist-info/LICENSE` & `senpy_sensei-1.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `senpy_sensei-1.3.0.dist-info/METADATA` & `senpy_sensei-1.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: senpy-sensei
-Version: 1.3.0
+Version: 1.3.1
 Summary: A python package of algorithms for sensitivity testing.
 Project-URL: Repository, https://github.com/ACasey13/senpy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

