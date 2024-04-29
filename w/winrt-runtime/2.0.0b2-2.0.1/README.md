# Comparing `tmp/winrt-runtime-2.0.0b2.tar.gz` & `tmp/winrt_runtime-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "winrt-runtime-2.0.0b2.tar", last modified: Sat Dec  2 18:19:13 2023, max compression
+gzip compressed data, was "winrt_runtime-2.0.1.tar", last modified: Sun Apr 28 21:04:19 2024, max compression
```

## Comparing `winrt-runtime-2.0.0b2.tar` & `winrt_runtime-2.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-12-02 18:19:13.507195 winrt-runtime-2.0.0b2/
--rw-rw-rw-   0        0        0      735 2023-12-02 18:19:13.507195 winrt-runtime-2.0.0b2/PKG-INFO
--rw-rw-rw-   0        0        0       97 2023-12-02 18:17:35.000000 winrt-runtime-2.0.0b2/README.md
--rw-rw-rw-   0        0        0     9639 2023-12-02 18:17:35.000000 winrt-runtime-2.0.0b2/_winrt.cpp
--rw-rw-rw-   0        0        0    17255 2023-12-02 18:17:35.000000 winrt-runtime-2.0.0b2/_winrt_array.cpp
--rw-rw-rw-   0        0        0     1419 2023-12-02 18:17:35.000000 winrt-runtime-2.0.0b2/pyproject.toml
--rw-rw-rw-   0        0        0       12 2023-12-02 18:17:35.000000 winrt-runtime-2.0.0b2/pywinrt-version.txt
--rw-rw-rw-   0        0        0    10715 2023-12-02 18:17:35.000000 winrt-runtime-2.0.0b2/runtime.cpp
--rw-rw-rw-   0        0        0       42 2023-12-02 18:19:13.507195 winrt-runtime-2.0.0b2/setup.cfg
--rw-rw-rw-   0        0        0      461 2023-12-02 18:17:35.000000 winrt-runtime-2.0.0b2/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-02 18:19:13.491569 winrt-runtime-2.0.0b2/src/
-drwxrwxrwx   0        0        0        0 2023-12-02 18:19:13.507195 winrt-runtime-2.0.0b2/src/winrt/
--rw-rw-rw-   0        0        0     3991 2023-12-02 18:17:35.000000 winrt-runtime-2.0.0b2/src/winrt/_winrt.pyi
--rw-rw-rw-   0        0        0        0 2023-12-02 18:17:35.000000 winrt-runtime-2.0.0b2/src/winrt/py.typed
-drwxrwxrwx   0        0        0        0 2023-12-02 18:19:13.507195 winrt-runtime-2.0.0b2/src/winrt/system/
--rw-rw-rw-   0        0        0     4166 2023-12-02 18:17:35.000000 winrt-runtime-2.0.0b2/src/winrt/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-02 18:19:13.507195 winrt-runtime-2.0.0b2/src/winrt_runtime.egg-info/
--rw-rw-rw-   0        0        0      735 2023-12-02 18:19:12.000000 winrt-runtime-2.0.0b2/src/winrt_runtime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-12-02 18:19:13.000000 winrt-runtime-2.0.0b2/src/winrt_runtime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-02 18:19:12.000000 winrt-runtime-2.0.0b2/src/winrt_runtime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-12-02 18:19:12.000000 winrt-runtime-2.0.0b2/src/winrt_runtime.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-28 21:04:19.468763 winrt_runtime-2.0.1/
+-rw-rw-rw-   0        0        0      733 2024-04-28 21:04:19.468763 winrt_runtime-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       97 2024-04-28 21:03:17.000000 winrt_runtime-2.0.1/README.md
+-rw-rw-rw-   0        0        0     9639 2024-04-28 21:03:17.000000 winrt_runtime-2.0.1/_winrt.cpp
+-rw-rw-rw-   0        0        0    17252 2024-04-28 21:03:17.000000 winrt_runtime-2.0.1/_winrt_array.cpp
+-rw-rw-rw-   0        0        0     1470 2024-04-28 21:03:17.000000 winrt_runtime-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0        5 2024-04-28 21:03:17.000000 winrt_runtime-2.0.1/pywinrt-version.txt
+-rw-rw-rw-   0        0        0    10715 2024-04-28 21:03:17.000000 winrt_runtime-2.0.1/runtime.cpp
+-rw-rw-rw-   0        0        0       42 2024-04-28 21:04:19.468763 winrt_runtime-2.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1019 2024-04-28 21:03:17.000000 winrt_runtime-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-28 21:04:19.453138 winrt_runtime-2.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-28 21:04:19.468763 winrt_runtime-2.0.1/src/winrt/
+-rw-rw-rw-   0        0        0     3991 2024-04-28 21:03:17.000000 winrt_runtime-2.0.1/src/winrt/_winrt.pyi
+-rw-rw-rw-   0        0        0        0 2024-04-28 21:03:17.000000 winrt_runtime-2.0.1/src/winrt/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-28 21:04:19.468763 winrt_runtime-2.0.1/src/winrt/system/
+-rw-rw-rw-   0        0        0     4166 2024-04-28 21:03:17.000000 winrt_runtime-2.0.1/src/winrt/system/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-28 21:04:19.468763 winrt_runtime-2.0.1/src/winrt_runtime.egg-info/
+-rw-rw-rw-   0        0        0      733 2024-04-28 21:04:19.000000 winrt_runtime-2.0.1/src/winrt_runtime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2024-04-28 21:04:19.000000 winrt_runtime-2.0.1/src/winrt_runtime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 21:04:19.000000 winrt_runtime-2.0.1/src/winrt_runtime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-28 21:04:19.000000 winrt_runtime-2.0.1/src/winrt_runtime.egg-info/top_level.txt
```

### Comparing `winrt-runtime-2.0.0b2/PKG-INFO` & `winrt_runtime-2.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winrt-runtime
-Version: 2.0.0b2
+Version: 2.0.1
 Summary: Python projection of Windows Runtime (WinRT) APIs
 License: MIT
 Project-URL: Documentation, https://pywinrt.readthedocs.io
 Project-URL: Repository, https://github.com/pywinrt/pywinrt
 Project-URL: Changelog, https://github.com/pywinrt/pywinrt/blob/main/CHANGELOG.md
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
```

### Comparing `winrt-runtime-2.0.0b2/_winrt.cpp` & `winrt_runtime-2.0.1/_winrt.cpp`

 * *Files identical despite different names*

### Comparing `winrt-runtime-2.0.0b2/_winrt_array.cpp` & `winrt_runtime-2.0.1/_winrt_array.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         }
 
         pyobj_handle self_handle{reinterpret_cast<PyObject*>(self)};
 
         PyObject* arg0;
         PyObject* arg1 = nullptr;
 
-        if (PyArg_UnpackTuple(args, "Array", 1, 2, &arg0, &arg1) < 0)
+        if (!PyArg_UnpackTuple(args, "Array", 1, 2, &arg0, &arg1))
         {
             return nullptr;
         }
 
         std::unique_ptr<py::Array> array;
 
         if (PyUnicode_Check(arg0))
```

### Comparing `winrt-runtime-2.0.0b2/pyproject.toml` & `winrt_runtime-2.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # WARNING: Please don't edit this file. It was automatically generated.
 
 [build-system]
-requires = ["setuptools", "setuptools-scm", "winrt-sdk"]
+requires = ["setuptools", "winrt-sdk"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "winrt-runtime"
 description = "Python projection of Windows Runtime (WinRT) APIs"
 readme = "README.md"
 license = { text = "MIT" }
@@ -27,21 +27,22 @@
 [tool.setuptools.dynamic]
 version = { file = "pywinrt-version.txt" }
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.package-data]
-winrt = ["*.pyi", "py.typed"]
+"*" = ["*.pyi", "py.typed"]
 
 [tool.cibuildwheel]
 # use local winrt-sdk build dependency
 environment = { PYTHONPATH="../winrt-sdk/src" }
 # don't install winrt-sdk from PyPI
 build-frontend = { name = "build", args = ["--skip-dependency-check", "--no-isolation"] }
 # don't build for PyPy
 skip = "pp*"
 # suppress warnings about ARM64 testing
 test-skip = "*-win_arm64"
 
 [tool.cibuildwheel.windows]
 archs = ["x86", "AMD64", "ARM64"]
+repair-wheel-command = "python scripts/add_dlls.py {wheel} {dest_dir}"
```

### Comparing `winrt-runtime-2.0.0b2/runtime.cpp` & `winrt_runtime-2.0.1/runtime.cpp`

 * *Files identical despite different names*

### Comparing `winrt-runtime-2.0.0b2/src/winrt/_winrt.pyi` & `winrt_runtime-2.0.1/src/winrt/_winrt.pyi`

 * *Files identical despite different names*

### Comparing `winrt-runtime-2.0.0b2/src/winrt/system/__init__.py` & `winrt_runtime-2.0.1/src/winrt/system/__init__.py`

 * *Files identical despite different names*

### Comparing `winrt-runtime-2.0.0b2/src/winrt_runtime.egg-info/PKG-INFO` & `winrt_runtime-2.0.1/src/winrt_runtime.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: winrt-runtime
-Version: 2.0.0b2
+Version: 2.0.1
 Summary: Python projection of Windows Runtime (WinRT) APIs
 License: MIT
 Project-URL: Documentation, https://pywinrt.readthedocs.io
 Project-URL: Repository, https://github.com/pywinrt/pywinrt
 Project-URL: Changelog, https://github.com/pywinrt/pywinrt/blob/main/CHANGELOG.md
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
```

