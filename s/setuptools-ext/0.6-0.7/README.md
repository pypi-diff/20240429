# Comparing `tmp/setuptools_ext-0.6.tar.gz` & `tmp/setuptools_ext-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools_ext-0.6.tar", last modified: Wed Apr 17 22:01:50 2024, max compression
+gzip compressed data, was "setuptools_ext-0.7.tar", last modified: Mon Apr 29 02:03:21 2024, max compression
```

## Comparing `setuptools_ext-0.6.tar` & `setuptools_ext-0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-04-17 22:01:50.788884 setuptools_ext-0.6/
--rw-r--r--   0 wim        (501) staff       (20)     1066 2022-04-20 07:49:46.000000 setuptools_ext-0.6/LICENSE
--rw-r--r--   0 wim        (501) staff       (20)     9207 2024-04-17 22:01:50.788585 setuptools_ext-0.6/PKG-INFO
--rw-r--r--   0 wim        (501) staff       (20)     8751 2022-10-27 07:06:15.000000 setuptools_ext-0.6/README.rst
--rw-r--r--   0 wim        (501) staff       (20)      564 2024-04-17 22:01:11.000000 setuptools_ext-0.6/pyproject.toml
--rw-r--r--   0 wim        (501) staff       (20)       38 2024-04-17 22:01:50.789125 setuptools_ext-0.6/setup.cfg
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-04-17 22:01:50.788323 setuptools_ext-0.6/setuptools_ext.egg-info/
--rw-r--r--   0 wim        (501) staff       (20)     9207 2024-04-17 22:01:50.000000 setuptools_ext-0.6/setuptools_ext.egg-info/PKG-INFO
--rw-r--r--   0 wim        (501) staff       (20)      269 2024-04-17 22:01:50.000000 setuptools_ext-0.6/setuptools_ext.egg-info/SOURCES.txt
--rw-r--r--   0 wim        (501) staff       (20)        1 2024-04-17 22:01:50.000000 setuptools_ext-0.6/setuptools_ext.egg-info/dependency_links.txt
--rw-r--r--   0 wim        (501) staff       (20)       53 2024-04-17 22:01:50.000000 setuptools_ext-0.6/setuptools_ext.egg-info/requires.txt
--rw-r--r--   0 wim        (501) staff       (20)       15 2024-04-17 22:01:50.000000 setuptools_ext-0.6/setuptools_ext.egg-info/top_level.txt
--rw-r--r--   0 wim        (501) staff       (20)     4246 2024-04-17 22:01:11.000000 setuptools_ext-0.6/setuptools_ext.py
-drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-04-17 22:01:50.787951 setuptools_ext-0.6/tests/
--rw-r--r--   0 wim        (501) staff       (20)     3316 2024-04-17 22:01:11.000000 setuptools_ext-0.6/tests/test_setuptools_ext.py
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-04-29 02:03:21.251917 setuptools_ext-0.7/
+-rw-r--r--   0 wim        (501) staff       (20)     1066 2022-04-20 07:49:46.000000 setuptools_ext-0.7/LICENSE
+-rw-r--r--   0 wim        (501) staff       (20)     9207 2024-04-29 02:03:21.251639 setuptools_ext-0.7/PKG-INFO
+-rw-r--r--   0 wim        (501) staff       (20)     8751 2024-04-17 23:32:21.000000 setuptools_ext-0.7/README.rst
+-rw-r--r--   0 wim        (501) staff       (20)      564 2024-04-29 02:03:12.000000 setuptools_ext-0.7/pyproject.toml
+-rw-r--r--   0 wim        (501) staff       (20)       38 2024-04-29 02:03:21.251967 setuptools_ext-0.7/setup.cfg
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-04-29 02:03:21.251356 setuptools_ext-0.7/setuptools_ext.egg-info/
+-rw-r--r--   0 wim        (501) staff       (20)     9207 2024-04-29 02:03:21.000000 setuptools_ext-0.7/setuptools_ext.egg-info/PKG-INFO
+-rw-r--r--   0 wim        (501) staff       (20)      269 2024-04-29 02:03:21.000000 setuptools_ext-0.7/setuptools_ext.egg-info/SOURCES.txt
+-rw-r--r--   0 wim        (501) staff       (20)        1 2024-04-29 02:03:21.000000 setuptools_ext-0.7/setuptools_ext.egg-info/dependency_links.txt
+-rw-r--r--   0 wim        (501) staff       (20)       53 2024-04-29 02:03:21.000000 setuptools_ext-0.7/setuptools_ext.egg-info/requires.txt
+-rw-r--r--   0 wim        (501) staff       (20)       15 2024-04-29 02:03:21.000000 setuptools_ext-0.7/setuptools_ext.egg-info/top_level.txt
+-rw-r--r--   0 wim        (501) staff       (20)     8174 2024-04-29 02:03:12.000000 setuptools_ext-0.7/setuptools_ext.py
+drwxr-xr-x   0 wim        (501) staff       (20)        0 2024-04-29 02:03:21.250992 setuptools_ext-0.7/tests/
+-rw-r--r--   0 wim        (501) staff       (20)     3614 2024-04-18 05:48:36.000000 setuptools_ext-0.7/tests/test_setuptools_ext.py
```

### Comparing `setuptools_ext-0.6/LICENSE` & `setuptools_ext-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools_ext-0.6/PKG-INFO` & `setuptools_ext-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-ext
-Version: 0.6
+Version: 0.7
 Summary: Extension of setuptools to support all core metadata fields
 Author: Wim Glenn
 Author-email: hey@wimglenn.com
 License: MIT
 Project-URL: Homepage, https://github.com/wimglenn/setuptools-ext
 Keywords: setuptools,packaging,metadata
 Requires-Python: >=3.7
```

### Comparing `setuptools_ext-0.6/README.rst` & `setuptools_ext-0.7/README.rst`

 * *Files identical despite different names*

### Comparing `setuptools_ext-0.6/pyproject.toml` & `setuptools_ext-0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "setuptools-ext"
-version = "0.6"
+version = "0.7"
 requires-python = ">= 3.7"
 description = "Extension of setuptools to support all core metadata fields"
 authors = [
     {name = "Wim Glenn"},
     {email = "hey@wimglenn.com"},
 ]
 readme = "README.rst"
```

### Comparing `setuptools_ext-0.6/setuptools_ext.egg-info/PKG-INFO` & `setuptools_ext-0.7/setuptools_ext.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-ext
-Version: 0.6
+Version: 0.7
 Summary: Extension of setuptools to support all core metadata fields
 Author: Wim Glenn
 Author-email: hey@wimglenn.com
 License: MIT
 Project-URL: Homepage, https://github.com/wimglenn/setuptools-ext
 Keywords: setuptools,packaging,metadata
 Requires-Python: >=3.7
```

### Comparing `setuptools_ext-0.6/tests/test_setuptools_ext.py` & `setuptools_ext-0.7/tests/test_setuptools_ext.py`

 * *Files 11% similar despite different names*

```diff
@@ -128,7 +128,29 @@
 def test_build_wheel_setup_cfg(in_source_tree):
     in_source_tree.joinpath("pyproject.toml").write_text(example_pyproject_minimal)
     in_source_tree.joinpath("setup.cfg").write_text(example_setup_cfg)
     whl = setuptools_ext.build_wheel(wheel_directory=str(in_source_tree))
     with zipfile.ZipFile(str(in_source_tree / whl)) as zf:
         txt = zf.read("example_proj-0.1.dist-info/METADATA").decode()
     assert txt.rstrip() == expected_metadata.rstrip()
+
+
+in_bytes = b"""\
+Metadata-Version: 2.1
+Name: foo
+Platform: UNKNOWN
+Version: 1.0
+
+"""
+
+
+expected_out_bytes = b"""\
+Metadata-Version: 2.1
+Name: foo
+Version: 1.0
+
+"""
+
+
+def test_drop_unknown():
+    out_bytes = setuptools_ext.rewrite_metadata(in_bytes, {})
+    assert out_bytes == expected_out_bytes
```

