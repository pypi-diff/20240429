# Comparing `tmp/mars_similarity_tools-0.2.0.tar.gz` & `tmp/mars_similarity_tools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mars_similarity_tools-0.2.0.tar", max compression
+gzip compressed data, was "mars_similarity_tools-0.2.1.tar", max compression
```

## Comparing `mars_similarity_tools-0.2.0.tar` & `mars_similarity_tools-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4101 2024-03-13 15:40:12.272797 mars_similarity_tools-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-13 13:47:44.899763 mars_similarity_tools-0.2.0/mars_similarity_tools/__init__.py
--rw-r--r--   0        0        0     5188 2024-03-25 14:57:42.004257 mars_similarity_tools-0.2.0/mars_similarity_tools/augmentation/__init__.py
--rw-r--r--   0        0        0      466 2024-03-25 15:23:29.681015 mars_similarity_tools-0.2.0/mars_similarity_tools/models/__init__.py
--rw-r--r--   0        0        0     4572 2024-03-28 13:27:21.537761 mars_similarity_tools-0.2.0/mars_similarity_tools/services/__init__.py
--rw-r--r--   0        0        0     4011 2024-03-28 13:25:48.344437 mars_similarity_tools-0.2.0/mars_similarity_tools/storages/__init__.py
--rw-r--r--   0        0        0      384 2024-03-28 13:27:04.550853 mars_similarity_tools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4763 1970-01-01 00:00:00.000000 mars_similarity_tools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4101 2024-03-13 15:40:12.272797 mars_similarity_tools-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-13 13:47:44.899763 mars_similarity_tools-0.2.1/mars_similarity_tools/__init__.py
+-rw-r--r--   0        0        0     5188 2024-03-25 14:57:42.004257 mars_similarity_tools-0.2.1/mars_similarity_tools/augmentation/__init__.py
+-rw-r--r--   0        0        0      466 2024-03-25 15:23:29.681015 mars_similarity_tools-0.2.1/mars_similarity_tools/models/__init__.py
+-rw-r--r--   0        0        0     4572 2024-03-28 13:27:21.537761 mars_similarity_tools-0.2.1/mars_similarity_tools/services/__init__.py
+-rw-r--r--   0        0        0     4011 2024-03-28 13:25:48.344437 mars_similarity_tools-0.2.1/mars_similarity_tools/storages/__init__.py
+-rw-r--r--   0        0        0      384 2024-04-29 13:46:18.328943 mars_similarity_tools-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4763 1970-01-01 00:00:00.000000 mars_similarity_tools-0.2.1/PKG-INFO
```

### Comparing `mars_similarity_tools-0.2.0/README.md` & `mars_similarity_tools-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mars_similarity_tools-0.2.0/mars_similarity_tools/augmentation/__init__.py` & `mars_similarity_tools-0.2.1/mars_similarity_tools/augmentation/__init__.py`

 * *Files identical despite different names*

### Comparing `mars_similarity_tools-0.2.0/mars_similarity_tools/services/__init__.py` & `mars_similarity_tools-0.2.1/mars_similarity_tools/services/__init__.py`

 * *Files identical despite different names*

### Comparing `mars_similarity_tools-0.2.0/mars_similarity_tools/storages/__init__.py` & `mars_similarity_tools-0.2.1/mars_similarity_tools/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `mars_similarity_tools-0.2.0/PKG-INFO` & `mars_similarity_tools-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: mars-similarity-tools
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Author: znittzel
 Author-email: rikard@ourstudio.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dill (>=0.3.8,<0.4.0)
-Requires-Dist: mars-vectorizer-sdk (>=0.1.9,<0.2.0)
+Requires-Dist: mars-vectorizer-sdk (>=0.2.0,<0.3.0)
 Requires-Dist: maz (>=0.0.12,<0.0.13)
 Requires-Dist: more-itertools (>=10.2.0,<11.0.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Mars Similarity Tools
 A small tools library for getting vector similarity measurement working in no time.
```

