# Comparing `tmp/pathlib_next-0.1.5.tar.gz` & `tmp/pathlib_next-0.1.6.tar.gz`

## Comparing `pathlib_next-0.1.5.tar` & `pathlib_next-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/example.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/pathlib_next/__init__.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/pathlib_next/fspath.py
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/pathlib_next/mempath.py
--rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/pathlib_next/path.py
--rw-r--r--   0        0        0    15459 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/pathlib_next/uri/__init__.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/pathlib_next/uri/query.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/pathlib_next/uri/source.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/pathlib_next/uri/schemes/__init__.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/pathlib_next/uri/schemes/file.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/pathlib_next/uri/schemes/http.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/pathlib_next/uri/schemes/sftp.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/pathlib_next/utils/__init__.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/pathlib_next/utils/glob.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/pathlib_next/utils/stat.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/src/pathlib_next/utils/sync.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/tests/test_local.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/tests/test_uri.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/LICENSE
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pathlib_next-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/example.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/__init__.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/fspath.py
+-rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/mempath.py
+-rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/path.py
+-rw-r--r--   0        0        0    15459 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/uri/__init__.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/uri/query.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/uri/source.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/uri/schemes/__init__.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/uri/schemes/file.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/uri/schemes/http.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/uri/schemes/sftp.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/utils/__init__.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/utils/glob.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/utils/stat.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/utils/sync.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/tests/test_local.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/tests/test_uri.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/LICENSE
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/PKG-INFO
```

### Comparing `pathlib_next-0.1.5/src/example.py` & `pathlib_next-0.1.6/src/example.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/src/pathlib_next/fspath.py` & `pathlib_next-0.1.6/src/pathlib_next/fspath.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/src/pathlib_next/mempath.py` & `pathlib_next-0.1.6/src/pathlib_next/mempath.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
             else:
                 parent = parent[path]
 
         return parent, name
 
     def _mkdir(self, mode: int):
         parent, name = self._parent_container()
-        if name in parent:
+        if not name or name in parent:
             raise FileExistsError(name)
         parent[name] = {}
 
     def rmdir(self):
         parent, name = self._parent_container()
         if not name:
             raise FileNotFoundError(self)
```

### Comparing `pathlib_next-0.1.5/src/pathlib_next/path.py` & `pathlib_next-0.1.6/src/pathlib_next/path.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/src/pathlib_next/uri/__init__.py` & `pathlib_next-0.1.6/src/pathlib_next/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/src/pathlib_next/uri/query.py` & `pathlib_next-0.1.6/src/pathlib_next/uri/query.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/src/pathlib_next/uri/source.py` & `pathlib_next-0.1.6/src/pathlib_next/uri/source.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/src/pathlib_next/uri/schemes/file.py` & `pathlib_next-0.1.6/src/pathlib_next/uri/schemes/file.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/src/pathlib_next/uri/schemes/http.py` & `pathlib_next-0.1.6/src/pathlib_next/uri/schemes/http.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/src/pathlib_next/uri/schemes/sftp.py` & `pathlib_next-0.1.6/src/pathlib_next/uri/schemes/sftp.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/src/pathlib_next/utils/__init__.py` & `pathlib_next-0.1.6/src/pathlib_next/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/src/pathlib_next/utils/glob.py` & `pathlib_next-0.1.6/src/pathlib_next/utils/glob.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/src/pathlib_next/utils/stat.py` & `pathlib_next-0.1.6/src/pathlib_next/utils/stat.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/src/pathlib_next/utils/sync.py` & `pathlib_next-0.1.6/src/pathlib_next/utils/sync.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/tests/test_local.py` & `pathlib_next-0.1.6/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/tests/test_uri.py` & `pathlib_next-0.1.6/tests/test_uri.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/LICENSE` & `pathlib_next-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.5/pyproject.toml` & `pathlib_next-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pathlib_next"
-version = "0.1.5"
+version = "0.1.6"
 authors = [{ name = "Jose A" }]
 description = "Generic Path Protocol based pathlib"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pathlib_next-0.1.5/PKG-INFO` & `pathlib_next-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pathlib_next
-Version: 0.1.5
+Version: 0.1.6
 Summary: Generic Path Protocol based pathlib
 Project-URL: Homepage, https://github.com/jose-pr/pathlib_next/
 Project-URL: Issues, https://github.com/jose-pr/pathlib_next/issues
 Author: Jose A
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

