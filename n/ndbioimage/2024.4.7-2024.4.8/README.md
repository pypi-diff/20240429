# Comparing `tmp/ndbioimage-2024.4.7.tar.gz` & `tmp/ndbioimage-2024.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndbioimage-2024.4.7.tar", max compression
+gzip compressed data, was "ndbioimage-2024.4.8.tar", max compression
```

## Comparing `ndbioimage-2024.4.7.tar` & `ndbioimage-2024.4.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.4.7/LICENSE
--rw-r--r--   0        0        0     2603 2024-04-12 15:46:18.729984 ndbioimage-2024.4.7/README.md
--rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.4.7/ndbioimage/.DS_Store
--rwxr-xr-x   0        0        0    54330 2024-04-19 14:08:16.717040 ndbioimage-2024.4.7/ndbioimage/__init__.py
--rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.4.7/ndbioimage/jvm.py
--rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.4.7/ndbioimage/readers/__init__.py
--rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.4.7/ndbioimage/readers/bfread.py
--rw-r--r--   0        0        0    28169 2024-04-24 15:10:18.268539 ndbioimage-2024.4.7/ndbioimage/readers/cziread.py
--rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.4.7/ndbioimage/readers/fijiread.py
--rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.4.7/ndbioimage/readers/ndread.py
--rw-r--r--   0        0        0     6405 2024-04-12 14:01:22.758103 ndbioimage-2024.4.7/ndbioimage/readers/seqread.py
--rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.4.7/ndbioimage/readers/tifread.py
--rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.4.7/ndbioimage/transform.txt
--rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.4.7/ndbioimage/transforms.py
--rw-r--r--   0        0        0     1248 2024-04-24 15:11:52.416478 ndbioimage-2024.4.7/pyproject.toml
--rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 ndbioimage-2024.4.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.4.8/LICENSE
+-rw-r--r--   0        0        0     2603 2024-04-12 15:46:18.729984 ndbioimage-2024.4.8/README.md
+-rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.4.8/ndbioimage/.DS_Store
+-rwxr-xr-x   0        0        0    54330 2024-04-19 14:08:16.717040 ndbioimage-2024.4.8/ndbioimage/__init__.py
+-rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.4.8/ndbioimage/jvm.py
+-rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.4.8/ndbioimage/readers/__init__.py
+-rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.4.8/ndbioimage/readers/bfread.py
+-rw-r--r--   0        0        0    28254 2024-04-29 11:09:41.232812 ndbioimage-2024.4.8/ndbioimage/readers/cziread.py
+-rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.4.8/ndbioimage/readers/fijiread.py
+-rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.4.8/ndbioimage/readers/ndread.py
+-rw-r--r--   0        0        0     6405 2024-04-12 14:01:22.758103 ndbioimage-2024.4.8/ndbioimage/readers/seqread.py
+-rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.4.8/ndbioimage/readers/tifread.py
+-rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.4.8/ndbioimage/transform.txt
+-rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.4.8/ndbioimage/transforms.py
+-rw-r--r--   0        0        0     1248 2024-04-29 11:13:48.376671 ndbioimage-2024.4.8/pyproject.toml
+-rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 ndbioimage-2024.4.8/PKG-INFO
```

### Comparing `ndbioimage-2024.4.7/LICENSE` & `ndbioimage-2024.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.7/README.md` & `ndbioimage-2024.4.8/README.md`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.7/ndbioimage/.DS_Store` & `ndbioimage-2024.4.8/ndbioimage/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.7/ndbioimage/__init__.py` & `ndbioimage-2024.4.8/ndbioimage/__init__.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.7/ndbioimage/jvm.py` & `ndbioimage-2024.4.8/ndbioimage/jvm.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.7/ndbioimage/readers/bfread.py` & `ndbioimage-2024.4.8/ndbioimage/readers/bfread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.7/ndbioimage/readers/cziread.py` & `ndbioimage-2024.4.8/ndbioimage/readers/cziread.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,14 +257,17 @@
         self.get_instruments()
         self.get_detectors()
         self.get_objectives()
         self.get_tubelenses()
         self.get_light_sources()
         self.get_filters()
         self.get_pixels()
+        self.get_channels()
+        self.get_planes()
+        self.get_annotations()
 
     @staticmethod
     def text(item: Optional[Element], default: str = "") -> str:
         return default if item is None else item.text
 
     @staticmethod
     def def_list(item: Any) -> list[Any]:
```

### Comparing `ndbioimage-2024.4.7/ndbioimage/readers/fijiread.py` & `ndbioimage-2024.4.8/ndbioimage/readers/fijiread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.7/ndbioimage/readers/ndread.py` & `ndbioimage-2024.4.8/ndbioimage/readers/ndread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.7/ndbioimage/readers/seqread.py` & `ndbioimage-2024.4.8/ndbioimage/readers/seqread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.7/ndbioimage/readers/tifread.py` & `ndbioimage-2024.4.8/ndbioimage/readers/tifread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.7/ndbioimage/transforms.py` & `ndbioimage-2024.4.8/ndbioimage/transforms.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.7/pyproject.toml` & `ndbioimage-2024.4.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ndbioimage"
-version = "2024.4.7"
+version = "2024.4.8"
 description = "Bio image reading, metadata and some affine registration."
 authors = ["W. Pomp <w.pomp@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["bioformats", "imread", "numpy", "metadata"]
 include = ["transform.txt"]
 repository = "https://github.com/wimpomp/ndbioimage"
```

### Comparing `ndbioimage-2024.4.7/PKG-INFO` & `ndbioimage-2024.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndbioimage
-Version: 2024.4.7
+Version: 2024.4.8
 Summary: Bio image reading, metadata and some affine registration.
 Home-page: https://github.com/wimpomp/ndbioimage
 License: GPLv3
 Keywords: bioformats,imread,numpy,metadata
 Author: W. Pomp
 Author-email: w.pomp@nki.nl
 Requires-Python: >=3.10,<4.0
```

