# Comparing `tmp/dknovautils-0.2.7.tar.gz` & `tmp/dknovautils-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dknovautils-0.2.7.tar", last modified: Mon Apr 29 03:20:09 2024, max compression
+gzip compressed data, was "dknovautils-0.2.8.tar", last modified: Mon Apr 29 12:34:18 2024, max compression
```

## Comparing `dknovautils-0.2.7.tar` & `dknovautils-0.2.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 03:20:09.719024 dknovautils-0.2.7/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1091 2023-05-19 02:33:35.000000 dknovautils-0.2.7/LICENSE
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      914 2024-04-29 03:20:09.718015 dknovautils-0.2.7/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      169 2024-02-02 04:40:13.000000 dknovautils-0.2.7/README.md
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2398 2024-04-29 03:20:01.000000 dknovautils-0.2.7/pyproject.toml
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2024-04-29 03:20:09.719024 dknovautils-0.2.7/setup.cfg
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 03:20:09.673016 dknovautils-0.2.7/src/
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 03:20:09.699007 dknovautils-0.2.7/src/dknovautils/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      326 2024-01-25 15:30:10.000000 dknovautils-0.2.7/src/dknovautils/__init__.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      134 2024-01-25 15:30:06.000000 dknovautils-0.2.7/src/dknovautils/__main__.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2907 2024-02-01 04:42:06.000000 dknovautils-0.2.7/src/dknovautils/commons.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1229 2024-04-29 03:20:01.000000 dknovautils-0.2.7/src/dknovautils/dk_imports.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     6828 2024-01-25 19:13:32.000000 dknovautils-0.2.7/src/dknovautils/dk_lang_etc_util.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)    17331 2024-04-29 03:20:01.000000 dknovautils-0.2.7/src/dknovautils/dkat.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     3332 2024-04-29 02:00:28.000000 dknovautils-0.2.7/src/dknovautils/dkfiles.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1447 2024-04-19 11:27:14.000000 dknovautils-0.2.7/src/dknovautils/dkipy.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     4052 2024-04-29 02:59:04.000000 dknovautils-0.2.7/src/dknovautils/dkprocess.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      618 2024-01-25 09:56:51.000000 dknovautils-0.2.7/src/dknovautils/example.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      282 2024-01-25 09:56:22.000000 dknovautils-0.2.7/src/dknovautils/myadd.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      314 2024-01-25 15:05:17.000000 dknovautils-0.2.7/src/dknovautils/mysubtract.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-01-25 17:59:24.000000 dknovautils-0.2.7/src/dknovautils/py.typed
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 03:20:09.717018 dknovautils-0.2.7/src/dknovautils.egg-info/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      914 2024-04-29 03:20:09.000000 dknovautils-0.2.7/src/dknovautils.egg-info/PKG-INFO
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      677 2024-04-29 03:20:09.000000 dknovautils-0.2.7/src/dknovautils.egg-info/SOURCES.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2024-04-29 03:20:09.000000 dknovautils-0.2.7/src/dknovautils.egg-info/dependency_links.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       43 2024-04-29 03:20:09.000000 dknovautils-0.2.7/src/dknovautils.egg-info/entry_points.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       14 2024-04-29 03:20:09.000000 dknovautils-0.2.7/src/dknovautils.egg-info/requires.txt
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2024-04-29 03:20:09.000000 dknovautils-0.2.7/src/dknovautils.egg-info/top_level.txt
-drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 03:20:09.715020 dknovautils-0.2.7/tests/
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      172 2024-01-26 10:01:40.000000 dknovautils-0.2.7/tests/test_b.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)      220 2024-01-26 10:01:52.000000 dknovautils-0.2.7/tests/test_c.py
--rwxrwxrwx   0 dknova    (1000) dknova    (1000)     3700 2024-04-29 03:16:44.000000 dknovautils-0.2.7/tests/test_d.py
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 12:34:18.831507 dknovautils-0.2.8/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1091 2023-05-19 02:33:35.000000 dknovautils-0.2.8/LICENSE
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      914 2024-04-29 12:34:18.829337 dknovautils-0.2.8/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      169 2024-02-02 04:40:13.000000 dknovautils-0.2.8/README.md
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2398 2024-04-29 12:34:04.000000 dknovautils-0.2.8/pyproject.toml
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       38 2024-04-29 12:34:18.831507 dknovautils-0.2.8/setup.cfg
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 12:34:18.785828 dknovautils-0.2.8/src/
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 12:34:18.813326 dknovautils-0.2.8/src/dknovautils/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      326 2024-01-25 15:30:10.000000 dknovautils-0.2.8/src/dknovautils/__init__.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      134 2024-01-25 15:30:06.000000 dknovautils-0.2.8/src/dknovautils/__main__.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     2907 2024-02-01 04:42:06.000000 dknovautils-0.2.8/src/dknovautils/commons.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1229 2024-04-29 12:34:04.000000 dknovautils-0.2.8/src/dknovautils/dk_imports.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     6828 2024-01-25 19:13:32.000000 dknovautils-0.2.8/src/dknovautils/dk_lang_etc_util.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)    17331 2024-04-29 12:34:04.000000 dknovautils-0.2.8/src/dknovautils/dkat.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     4856 2024-04-29 12:30:42.000000 dknovautils-0.2.8/src/dknovautils/dkfiles.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     1447 2024-04-19 11:27:14.000000 dknovautils-0.2.8/src/dknovautils/dkipy.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     4035 2024-04-29 03:22:31.000000 dknovautils-0.2.8/src/dknovautils/dkprocess.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      618 2024-01-25 09:56:51.000000 dknovautils-0.2.8/src/dknovautils/example.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      282 2024-01-25 09:56:22.000000 dknovautils-0.2.8/src/dknovautils/myadd.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      314 2024-01-25 15:05:17.000000 dknovautils-0.2.8/src/dknovautils/mysubtract.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-01-25 17:59:24.000000 dknovautils-0.2.8/src/dknovautils/py.typed
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 12:34:18.828326 dknovautils-0.2.8/src/dknovautils.egg-info/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      914 2024-04-29 12:34:18.000000 dknovautils-0.2.8/src/dknovautils.egg-info/PKG-INFO
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      677 2024-04-29 12:34:18.000000 dknovautils-0.2.8/src/dknovautils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)        1 2024-04-29 12:34:18.000000 dknovautils-0.2.8/src/dknovautils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       43 2024-04-29 12:34:18.000000 dknovautils-0.2.8/src/dknovautils.egg-info/entry_points.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       14 2024-04-29 12:34:18.000000 dknovautils-0.2.8/src/dknovautils.egg-info/requires.txt
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)       12 2024-04-29 12:34:18.000000 dknovautils-0.2.8/src/dknovautils.egg-info/top_level.txt
+drwxrwxrwx   0 dknova    (1000) dknova    (1000)        0 2024-04-29 12:34:18.827325 dknovautils-0.2.8/tests/
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      172 2024-01-26 10:01:40.000000 dknovautils-0.2.8/tests/test_b.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)      220 2024-01-26 10:01:52.000000 dknovautils-0.2.8/tests/test_c.py
+-rwxrwxrwx   0 dknova    (1000) dknova    (1000)     3700 2024-04-29 03:16:44.000000 dknovautils-0.2.8/tests/test_d.py
```

### Comparing `dknovautils-0.2.7/LICENSE` & `dknovautils-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.7/PKG-INFO` & `dknovautils-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.2.7
+Version: 0.2.8
 Summary: A small example package
 Author-email: dknova <dikisite@outlook.com>, dknova2 <dikisite2@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://example.com/xxx
 Project-URL: Documentation, https://readthedocs.org/xxx
 Project-URL: Repository, https://github.com/me/xxx.git
 Project-URL: Issues, https://github.com/me/xxx/issues
```

### Comparing `dknovautils-0.2.7/pyproject.toml` & `dknovautils-0.2.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # 之所以改成setuptools build 是因为要配置 py.typed参数 而如果用hatch工具不知道如何配置
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dknovautils"
-version = '0.2.7'
+version = '0.2.8'
 dependencies = [
     "numpy",
     "ipython"
 ]
 authors = [
   { name="dknova", email="dikisite@outlook.com" },
   { name="dknova2", email="dikisite2@outlook.com" },
```

### Comparing `dknovautils-0.2.7/src/dknovautils/commons.py` & `dknovautils-0.2.8/src/dknovautils/commons.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.7/src/dknovautils/dk_imports.py` & `dknovautils-0.2.8/src/dknovautils/dk_imports.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.7/src/dknovautils/dk_lang_etc_util.py` & `dknovautils-0.2.8/src/dknovautils/dk_lang_etc_util.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.7/src/dknovautils/dkat.py` & `dknovautils-0.2.8/src/dknovautils/dkat.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import dknovautils
 
 # from dknovautils.dk_imports import *
 from dknovautils.commons import *
 
 
-DkAppVer = '0.2.7'
+DkAppVer = '0.2.8'
 
 _unknown_err = "_unknown_err4035"
 
 T = TypeVar("T")
 
 
 class staticproperty(property):
```

### Comparing `dknovautils-0.2.7/src/dknovautils/dkipy.py` & `dknovautils-0.2.8/src/dknovautils/dkipy.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.7/src/dknovautils/dkprocess.py` & `dknovautils-0.2.8/src/dknovautils/dkprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,17 @@
         cmd: str,
         *,
         splitLines: bool = False,
         throwOnErrReturnCode: bool = False,
         strip: bool = True,
         _debug: bool = False,
         encoding: Any = None,
-        errors:Any=None,
+        errors: Any = None,
     ) -> Tuple[int, str, str]:
-        """ 
-        
-        """
+        """ """
         # Tuple[int, str|List,str|List]
         cmdid = DKProcessUtil._cmdid
         DKProcessUtil._cmdid += 1
 
         AT.assert_(not splitLines, "err51042 no splitlines")
 
         if _debug:
```

### Comparing `dknovautils-0.2.7/src/dknovautils/example.py` & `dknovautils-0.2.8/src/dknovautils/example.py`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.7/src/dknovautils.egg-info/PKG-INFO` & `dknovautils-0.2.8/src/dknovautils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dknovautils
-Version: 0.2.7
+Version: 0.2.8
 Summary: A small example package
 Author-email: dknova <dikisite@outlook.com>, dknova2 <dikisite2@outlook.com>
 License: MIT License
 Project-URL: Homepage, https://example.com/xxx
 Project-URL: Documentation, https://readthedocs.org/xxx
 Project-URL: Repository, https://github.com/me/xxx.git
 Project-URL: Issues, https://github.com/me/xxx/issues
```

### Comparing `dknovautils-0.2.7/src/dknovautils.egg-info/SOURCES.txt` & `dknovautils-0.2.8/src/dknovautils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dknovautils-0.2.7/tests/test_d.py` & `dknovautils-0.2.8/tests/test_d.py`

 * *Files identical despite different names*

