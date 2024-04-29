# Comparing `tmp/napari_conidie-1.0.0.tar.gz` & `tmp/napari_conidie-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_conidie-1.0.0.tar", last modified: Mon Apr 29 12:34:05 2024, max compression
+gzip compressed data, was "napari_conidie-1.0.1.tar", last modified: Mon Apr 29 12:36:11 2024, max compression
```

## Comparing `napari_conidie-1.0.0.tar` & `napari_conidie-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 12:34:05.229738 napari_conidie-1.0.0/
--rw-rw-rw-   0        0        0     1520 2024-04-29 07:13:55.000000 napari_conidie-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      101 2024-04-29 07:13:55.000000 napari_conidie-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5445 2024-04-29 12:34:05.229738 napari_conidie-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3706 2024-04-29 12:31:10.000000 napari_conidie-1.0.0/README.md
--rw-rw-rw-   0        0        0      192 2024-04-29 07:13:55.000000 napari_conidie-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1796 2024-04-29 12:34:05.231737 napari_conidie-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1348 2024-04-29 12:33:31.000000 napari_conidie-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-29 12:34:05.186457 napari_conidie-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 12:34:05.207803 napari_conidie-1.0.0/src/napari_conidie/
--rw-rw-rw-   0        0        0      191 2024-04-29 12:33:42.000000 napari_conidie-1.0.0/src/napari_conidie/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 12:34:05.225737 napari_conidie-1.0.0/src/napari_conidie/_tests/
--rw-rw-rw-   0        0        0        0 2024-04-29 07:13:55.000000 napari_conidie-1.0.0/src/napari_conidie/_tests/__init__.py
--rw-rw-rw-   0        0        0       84 2024-04-29 07:13:55.000000 napari_conidie-1.0.0/src/napari_conidie/_tests/test_widget.py
--rw-rw-rw-   0        0        0    20449 2024-04-29 12:31:10.000000 napari_conidie-1.0.0/src/napari_conidie/_widget.py
--rw-rw-rw-   0        0        0     1191 2024-04-29 08:03:42.000000 napari_conidie-1.0.0/src/napari_conidie/ilastik_search.py
--rw-rw-rw-   0        0        0      591 2024-04-29 12:31:10.000000 napari_conidie-1.0.0/src/napari_conidie/napari.yaml
--rw-rw-rw-   0        0        0      413 2024-04-29 08:04:52.000000 napari_conidie-1.0.0/src/napari_conidie/path.py
-drwxrwxrwx   0        0        0        0 2024-04-29 12:34:05.227736 napari_conidie-1.0.0/src/napari_conidie.egg-info/
--rw-rw-rw-   0        0        0     5445 2024-04-29 12:34:05.000000 napari_conidie-1.0.0/src/napari_conidie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2024-04-29 12:34:05.000000 napari_conidie-1.0.0/src/napari_conidie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 12:34:05.000000 napari_conidie-1.0.0/src/napari_conidie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-29 12:34:05.000000 napari_conidie-1.0.0/src/napari_conidie.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2024-04-29 12:34:05.000000 napari_conidie-1.0.0/src/napari_conidie.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-29 12:34:05.000000 napari_conidie-1.0.0/src/napari_conidie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 12:36:11.772249 napari_conidie-1.0.1/
+-rw-rw-rw-   0        0        0     1520 2024-04-29 07:13:55.000000 napari_conidie-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-04-29 07:13:55.000000 napari_conidie-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5445 2024-04-29 12:36:11.772249 napari_conidie-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3706 2024-04-29 12:31:10.000000 napari_conidie-1.0.1/README.md
+-rw-rw-rw-   0        0        0      192 2024-04-29 07:13:55.000000 napari_conidie-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1796 2024-04-29 12:36:11.774757 napari_conidie-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2024-04-29 12:35:53.000000 napari_conidie-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:36:11.730999 napari_conidie-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 12:36:11.750945 napari_conidie-1.0.1/src/napari_conidie/
+-rw-rw-rw-   0        0        0      191 2024-04-29 12:36:02.000000 napari_conidie-1.0.1/src/napari_conidie/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:36:11.769247 napari_conidie-1.0.1/src/napari_conidie/_tests/
+-rw-rw-rw-   0        0        0        0 2024-04-29 07:13:55.000000 napari_conidie-1.0.1/src/napari_conidie/_tests/__init__.py
+-rw-rw-rw-   0        0        0       84 2024-04-29 07:13:55.000000 napari_conidie-1.0.1/src/napari_conidie/_tests/test_widget.py
+-rw-rw-rw-   0        0        0    20449 2024-04-29 12:31:10.000000 napari_conidie-1.0.1/src/napari_conidie/_widget.py
+-rw-rw-rw-   0        0        0     1191 2024-04-29 08:03:42.000000 napari_conidie-1.0.1/src/napari_conidie/ilastik_search.py
+-rw-rw-rw-   0        0        0      591 2024-04-29 12:31:10.000000 napari_conidie-1.0.1/src/napari_conidie/napari.yaml
+-rw-rw-rw-   0        0        0      413 2024-04-29 08:04:52.000000 napari_conidie-1.0.1/src/napari_conidie/path.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:36:11.770246 napari_conidie-1.0.1/src/napari_conidie.egg-info/
+-rw-rw-rw-   0        0        0     5445 2024-04-29 12:36:11.000000 napari_conidie-1.0.1/src/napari_conidie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      552 2024-04-29 12:36:11.000000 napari_conidie-1.0.1/src/napari_conidie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 12:36:11.000000 napari_conidie-1.0.1/src/napari_conidie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-29 12:36:11.000000 napari_conidie-1.0.1/src/napari_conidie.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2024-04-29 12:36:11.000000 napari_conidie-1.0.1/src/napari_conidie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-29 12:36:11.000000 napari_conidie-1.0.1/src/napari_conidie.egg-info/top_level.txt
```

### Comparing `napari_conidie-1.0.0/LICENSE` & `napari_conidie-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_conidie-1.0.0/PKG-INFO` & `napari_conidie-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-conidie
-Version: 1.0.0
+Version: 1.0.1
 Summary: A segmentation tool to get conidie and hyphe
 Home-page: https://github.com/hereariim/napari-conidie
 Author: Herearii Metuarea
 Author-email: herearii.metuarea@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/hereariim/napari-conidie/issues
 Project-URL: Documentation, https://github.com/hereariim/napari-conidie#README.md
```

### Comparing `napari_conidie-1.0.0/README.md` & `napari_conidie-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `napari_conidie-1.0.0/setup.cfg` & `napari_conidie-1.0.1/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6170 6172 692d 636f 6e69 6469   = napari-conidi
 00000020: 650d 0a76 6572 7369 6f6e 203d 2031 2e30  e..version = 1.0
-00000030: 2e30 0d0a 6465 7363 7269 7074 696f 6e20  .0..description 
+00000030: 2e31 0d0a 6465 7363 7269 7074 696f 6e20  .1..description 
 00000040: 3d20 4120 7365 676d 656e 7461 7469 6f6e  = A segmentation
 00000050: 2074 6f6f 6c20 746f 2067 6574 2063 6f6e   tool to get con
 00000060: 6964 6965 2061 6e64 2068 7970 6865 0d0a  idie and hyphe..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
 00000090: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
 000000a0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
```

### Comparing `napari_conidie-1.0.0/setup.py` & `napari_conidie-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r", encoding="utf-8") as fh: 
      long_description = fh.read() 
 setup(    
     author="Herearii Metuarea",    
     author_email="herearii.metuarea@gmail.com",
     name='napari-conidie', 
     description='A segmentation tool to get conidie and hyphe',  
-    version="1.0.0",    
+    version="1.0.1",    
     long_description=long_description, 
     long_description_content_type="text/markdown",  
     url='https://github.com/hereariim/napari-conidie', 
     packages=find_packages(),
     python_requires=">=3.8",
     install_requires=['numpy',
     'magicgui',
```

### Comparing `napari_conidie-1.0.0/src/napari_conidie/_widget.py` & `napari_conidie-1.0.1/src/napari_conidie/_widget.py`

 * *Files identical despite different names*

### Comparing `napari_conidie-1.0.0/src/napari_conidie/ilastik_search.py` & `napari_conidie-1.0.1/src/napari_conidie/ilastik_search.py`

 * *Files identical despite different names*

### Comparing `napari_conidie-1.0.0/src/napari_conidie/napari.yaml` & `napari_conidie-1.0.1/src/napari_conidie/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari_conidie-1.0.0/src/napari_conidie.egg-info/PKG-INFO` & `napari_conidie-1.0.1/src/napari_conidie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-conidie
-Version: 1.0.0
+Version: 1.0.1
 Summary: A segmentation tool to get conidie and hyphe
 Home-page: https://github.com/hereariim/napari-conidie
 Author: Herearii Metuarea
 Author-email: herearii.metuarea@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/hereariim/napari-conidie/issues
 Project-URL: Documentation, https://github.com/hereariim/napari-conidie#README.md
```

### Comparing `napari_conidie-1.0.0/src/napari_conidie.egg-info/SOURCES.txt` & `napari_conidie-1.0.1/src/napari_conidie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

