# Comparing `tmp/crypt_r-3.13.0.tar.gz` & `tmp/crypt_r-3.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypt_r-3.13.0.tar", last modified: Mon Apr 29 12:24:21 2024, max compression
+gzip compressed data, was "crypt_r-3.13.1.tar", last modified: Mon Apr 29 12:54:24 2024, max compression
```

## Comparing `crypt_r-3.13.0.tar` & `crypt_r-3.13.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 churchyard  (1000) churchyard  (1000)        0 2024-04-29 12:24:21.495149 crypt_r-3.13.0/
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)    13936 2024-04-25 13:06:15.000000 crypt_r-3.13.0/LICENSE
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)       86 2024-04-29 07:56:18.000000 crypt_r-3.13.0/MANIFEST.in
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)    24245 2024-04-29 12:24:21.495149 crypt_r-3.13.0/PKG-INFO
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)     7264 2024-04-29 12:23:04.000000 crypt_r-3.13.0/README.rst
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)     1082 2024-04-29 12:23:04.000000 crypt_r-3.13.0/pyproject.toml
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)       38 2024-04-29 12:24:21.495149 crypt_r-3.13.0/setup.cfg
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)      264 2024-04-29 07:56:18.000000 crypt_r-3.13.0/setup.py
-drwxr-xr-x   0 churchyard  (1000) churchyard  (1000)        0 2024-04-29 12:24:21.494150 crypt_r-3.13.0/src/
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)     2906 2024-04-29 07:56:18.000000 crypt_r-3.13.0/src/_crypt_r.c
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)      120 2024-04-29 07:56:18.000000 crypt_r-3.13.0/src/crypt.py
-drwxr-xr-x   0 churchyard  (1000) churchyard  (1000)        0 2024-04-29 12:24:21.495149 crypt_r-3.13.0/src/crypt_r.egg-info/
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)    24245 2024-04-29 12:24:21.000000 crypt_r-3.13.0/src/crypt_r.egg-info/PKG-INFO
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)      267 2024-04-29 12:24:21.000000 crypt_r-3.13.0/src/crypt_r.egg-info/SOURCES.txt
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)        1 2024-04-29 12:24:21.000000 crypt_r-3.13.0/src/crypt_r.egg-info/dependency_links.txt
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)       23 2024-04-29 12:24:21.000000 crypt_r-3.13.0/src/crypt_r.egg-info/top_level.txt
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)     3785 2024-04-29 07:56:18.000000 crypt_r-3.13.0/src/crypt_r.py
-drwxr-xr-x   0 churchyard  (1000) churchyard  (1000)        0 2024-04-29 12:24:21.494150 crypt_r-3.13.0/tests/
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)     3831 2024-04-29 07:56:18.000000 crypt_r-3.13.0/tests/test_crypt_r.py
--rw-r--r--   0 churchyard  (1000) churchyard  (1000)      120 2024-04-29 07:56:18.000000 crypt_r-3.13.0/tox.ini
+drwxr-xr-x   0 churchyard  (1000) churchyard  (1000)        0 2024-04-29 12:54:24.845875 crypt_r-3.13.1/
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)    13936 2024-04-25 13:06:15.000000 crypt_r-3.13.1/LICENSE
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)       86 2024-04-29 07:56:18.000000 crypt_r-3.13.1/MANIFEST.in
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)    24318 2024-04-29 12:54:24.845875 crypt_r-3.13.1/PKG-INFO
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)     7337 2024-04-29 12:50:00.000000 crypt_r-3.13.1/README.rst
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)     1082 2024-04-29 12:49:24.000000 crypt_r-3.13.1/pyproject.toml
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)       38 2024-04-29 12:54:24.845875 crypt_r-3.13.1/setup.cfg
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)      264 2024-04-29 07:56:18.000000 crypt_r-3.13.1/setup.py
+drwxr-xr-x   0 churchyard  (1000) churchyard  (1000)        0 2024-04-29 12:54:24.844875 crypt_r-3.13.1/src/
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)     2919 2024-04-29 12:48:58.000000 crypt_r-3.13.1/src/_crypt_r.c
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)      120 2024-04-29 07:56:18.000000 crypt_r-3.13.1/src/crypt.py
+drwxr-xr-x   0 churchyard  (1000) churchyard  (1000)        0 2024-04-29 12:54:24.845875 crypt_r-3.13.1/src/crypt_r.egg-info/
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)    24318 2024-04-29 12:54:24.000000 crypt_r-3.13.1/src/crypt_r.egg-info/PKG-INFO
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)      267 2024-04-29 12:54:24.000000 crypt_r-3.13.1/src/crypt_r.egg-info/SOURCES.txt
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)        1 2024-04-29 12:54:24.000000 crypt_r-3.13.1/src/crypt_r.egg-info/dependency_links.txt
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)       23 2024-04-29 12:54:24.000000 crypt_r-3.13.1/src/crypt_r.egg-info/top_level.txt
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)     3785 2024-04-29 07:56:18.000000 crypt_r-3.13.1/src/crypt_r.py
+drwxr-xr-x   0 churchyard  (1000) churchyard  (1000)        0 2024-04-29 12:54:24.845875 crypt_r-3.13.1/tests/
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)     3831 2024-04-29 07:56:18.000000 crypt_r-3.13.1/tests/test_crypt_r.py
+-rw-r--r--   0 churchyard  (1000) churchyard  (1000)      175 2024-04-29 12:48:58.000000 crypt_r-3.13.1/tox.ini
```

### Comparing `crypt_r-3.13.0/LICENSE` & `crypt_r-3.13.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crypt_r-3.13.0/PKG-INFO` & `crypt_r-3.13.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypt_r
-Version: 3.13.0
+Version: 3.13.1
 Summary: A copy of the `crypt` module that was removed in Python 3.13
 Author-email: "Steven D. Majewski" <sdm7g@virginia.edu>
 Maintainer-email: Miro Hrončok <miro@hroncok.cz>, Petr Viktorin <encukou@gmail.com>, Tomáš Hrnčiar <tomas.hrnciar@me.com>, Karolina Surma <ksurma@redhat.com>
 License: A. HISTORY OF THE SOFTWARE
         ==========================
         
         Python was created in the early 1990s by Guido van Rossum at Stichting
@@ -479,14 +479,20 @@
 
 --------------
 
 
 Changelog
 ---------
 
+3.13.1
+^^^^^^
+
+* Fix build with ``-Werror=incompatible-pointer-types``
+
+
 3.13.0
 ^^^^^^
 
 * Initial fork from CPython 3.12.3
 * Always uses the `crypt_r(3)`_ function, never `crypt(3)`_
 * Renamed the Python modules to ``crypt_r`` and ``_crypt_r``
```

### Comparing `crypt_r-3.13.0/README.rst` & `crypt_r-3.13.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -183,14 +183,20 @@
 
 --------------
 
 
 Changelog
 ---------
 
+3.13.1
+^^^^^^
+
+* Fix build with ``-Werror=incompatible-pointer-types``
+
+
 3.13.0
 ^^^^^^
 
 * Initial fork from CPython 3.12.3
 * Always uses the `crypt_r(3)`_ function, never `crypt(3)`_
 * Renamed the Python modules to ``crypt_r`` and ``_crypt_r``
```

### Comparing `crypt_r-3.13.0/pyproject.toml` & `crypt_r-3.13.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crypt_r"
-version = "3.13.0"
+version = "3.13.1"
 authors = [
     {name = "Steven D. Majewski", email = "sdm7g@virginia.edu"},
 ]
 maintainers = [
     {name = "Miro Hrončok", email = "miro@hroncok.cz"},
     {name = "Petr Viktorin", email = "encukou@gmail.com"},
     {name = "Tomáš Hrnčiar", email = "tomas.hrnciar@me.com"},
```

### Comparing `crypt_r-3.13.0/src/_crypt_r.c` & `crypt_r-3.13.1/src/_crypt_r.c`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         return PyErr_SetFromErrno(PyExc_OSError);
     }
     return PyUnicode_FromString(crypt_result);
 }
 
 
 static PyMethodDef crypt_r_methods[] = {
-    {"crypt", crypt_r_crypt, METH_FASTCALL, crypt_r_crypt__doc__},
+    {"crypt", (PyCFunction)crypt_r_crypt, METH_FASTCALL, crypt_r_crypt__doc__},
     {NULL,              NULL}           /* sentinel */
 };
 
 static PyModuleDef_Slot _crypt_r_slots[] = {
 #ifdef Py_MOD_PER_INTERPRETER_GIL_SUPPORTED
     {Py_mod_multiple_interpreters, Py_MOD_PER_INTERPRETER_GIL_SUPPORTED},
 #endif
```

### Comparing `crypt_r-3.13.0/src/crypt_r.egg-info/PKG-INFO` & `crypt_r-3.13.1/src/crypt_r.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypt_r
-Version: 3.13.0
+Version: 3.13.1
 Summary: A copy of the `crypt` module that was removed in Python 3.13
 Author-email: "Steven D. Majewski" <sdm7g@virginia.edu>
 Maintainer-email: Miro Hrončok <miro@hroncok.cz>, Petr Viktorin <encukou@gmail.com>, Tomáš Hrnčiar <tomas.hrnciar@me.com>, Karolina Surma <ksurma@redhat.com>
 License: A. HISTORY OF THE SOFTWARE
         ==========================
         
         Python was created in the early 1990s by Guido van Rossum at Stichting
@@ -479,14 +479,20 @@
 
 --------------
 
 
 Changelog
 ---------
 
+3.13.1
+^^^^^^
+
+* Fix build with ``-Werror=incompatible-pointer-types``
+
+
 3.13.0
 ^^^^^^
 
 * Initial fork from CPython 3.12.3
 * Always uses the `crypt_r(3)`_ function, never `crypt(3)`_
 * Renamed the Python modules to ``crypt_r`` and ``_crypt_r``
```

### Comparing `crypt_r-3.13.0/src/crypt_r.py` & `crypt_r-3.13.1/src/crypt_r.py`

 * *Files identical despite different names*

### Comparing `crypt_r-3.13.0/tests/test_crypt_r.py` & `crypt_r-3.13.1/tests/test_crypt_r.py`

 * *Files identical despite different names*

