# Comparing `tmp/pykwl-0.0.6.tar.gz` & `tmp/pykwl-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykwl-0.0.6.tar", last modified: Thu Apr 18 11:30:58 2024, max compression
+gzip compressed data, was "pykwl-0.0.7.tar", last modified: Mon Apr 29 10:31:46 2024, max compression
```

## Comparing `pykwl-0.0.6.tar` & `pykwl-0.0.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-18 11:30:48.000000 pykwl-0.0.6/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-18 11:30:48.000000 pykwl-0.0.6/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-18 11:30:48.000000 pykwl-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-18 11:30:48.000000 pykwl-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 11:30:58.489852 pykwl-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-18 11:30:48.000000 pykwl-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.485851 pykwl-0.0.6/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-18 11:30:48.000000 pykwl-0.0.6/cmake/configure_ccache.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.485851 pykwl-0.0.6/dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-18 11:30:48.000000 pykwl-0.0.6/dependencies/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.485851 pykwl-0.0.6/dependencies/pybind11/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-18 11:30:48.000000 pykwl-0.0.6/dependencies/pybind11/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.485851 pykwl-0.0.6/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/include/wl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/include/wl/details/
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-18 11:30:48.000000 pykwl-0.0.6/include/wl/details/graph.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-18 11:30:48.000000 pykwl-0.0.6/include/wl/details/weisfeiler_leman.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-18 11:30:48.000000 pykwl-0.0.6/include/wl/wl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-18 11:30:48.000000 pykwl-0.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.485851 pykwl-0.0.6/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/python/src/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-18 11:30:48.000000 pykwl-0.0.6/python/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-18 11:30:48.000000 pykwl-0.0.6/python/src/main.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/python/src/pykwl/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-18 11:30:48.000000 pykwl-0.0.6/python/src/pykwl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-18 11:30:48.000000 pykwl-0.0.6/python/src/pykwl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-18 11:30:48.000000 pykwl-0.0.6/python/src/pykwl/bindings.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/python/src/pykwl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-18 11:30:58.000000 pykwl-0.0.6/python/src/pykwl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-18 11:30:58.000000 pykwl-0.0.6/python/src/pykwl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:30:58.000000 pykwl-0.0.6/python/src/pykwl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:30:58.000000 pykwl-0.0.6/python/src/pykwl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-18 11:30:58.000000 pykwl-0.0.6/python/src/pykwl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-18 11:30:58.000000 pykwl-0.0.6/python/src/pykwl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 11:30:58.489852 pykwl-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-18 11:30:48.000000 pykwl-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-18 11:30:48.000000 pykwl-0.0.6/src/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-18 11:30:48.000000 pykwl-0.0.6/src/graph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8961 2024-04-18 11:30:48.000000 pykwl-0.0.6/src/weisfeiler_leman.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:48.000000 pykwl-0.0.6/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:58.489852 pykwl-0.0.6/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:48.000000 pykwl-0.0.6/tests/unit/CMakeLists copy.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:30:48.000000 pykwl-0.0.6/tests/unit/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-29 10:31:36.000000 pykwl-0.0.7/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-29 10:31:36.000000 pykwl-0.0.7/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 10:31:36.000000 pykwl-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-29 10:31:36.000000 pykwl-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-29 10:31:46.184571 pykwl-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-29 10:31:36.000000 pykwl-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-29 10:31:36.000000 pykwl-0.0.7/cmake/configure_ccache.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 10:31:36.000000 pykwl-0.0.7/dependencies/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/dependencies/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-29 10:31:36.000000 pykwl-0.0.7/dependencies/pybind11/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.180570 pykwl-0.0.7/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/include/wl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/include/wl/details/
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-29 10:31:36.000000 pykwl-0.0.7/include/wl/details/graph.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-29 10:31:36.000000 pykwl-0.0.7/include/wl/details/weisfeiler_leman.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-29 10:31:36.000000 pykwl-0.0.7/include/wl/wl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-29 10:31:36.000000 pykwl-0.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.180570 pykwl-0.0.7/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/python/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-29 10:31:36.000000 pykwl-0.0.7/python/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-29 10:31:36.000000 pykwl-0.0.7/python/src/main.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/python/src/pykwl/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 10:31:36.000000 pykwl-0.0.7/python/src/pykwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-29 10:31:36.000000 pykwl-0.0.7/python/src/pykwl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-29 10:31:36.000000 pykwl-0.0.7/python/src/pykwl/bindings.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/python/src/pykwl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-29 10:31:46.000000 pykwl-0.0.7/python/src/pykwl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-29 10:31:46.000000 pykwl-0.0.7/python/src/pykwl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:31:46.000000 pykwl-0.0.7/python/src/pykwl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:31:46.000000 pykwl-0.0.7/python/src/pykwl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 10:31:46.000000 pykwl-0.0.7/python/src/pykwl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 10:31:46.000000 pykwl-0.0.7/python/src/pykwl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:31:46.184571 pykwl-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-29 10:31:36.000000 pykwl-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-29 10:31:36.000000 pykwl-0.0.7/src/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-29 10:31:36.000000 pykwl-0.0.7/src/graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10117 2024-04-29 10:31:36.000000 pykwl-0.0.7/src/weisfeiler_leman.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:36.000000 pykwl-0.0.7/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:46.184571 pykwl-0.0.7/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:36.000000 pykwl-0.0.7/tests/unit/CMakeLists copy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:31:36.000000 pykwl-0.0.7/tests/unit/CMakeLists.txt
```

### Comparing `pykwl-0.0.6/CMakeLists.txt` & `pykwl-0.0.7/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.6/Config.cmake.in` & `pykwl-0.0.7/Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.6/LICENSE` & `pykwl-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.6/README.md` & `pykwl-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.6/cmake/configure_ccache.cmake` & `pykwl-0.0.7/cmake/configure_ccache.cmake`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.6/dependencies/pybind11/CMakeLists.txt` & `pykwl-0.0.7/dependencies/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.6/include/wl/details/graph.hpp` & `pykwl-0.0.7/include/wl/details/graph.hpp`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.6/pyproject.toml` & `pykwl-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.6/python/src/pykwl/bindings.cpp` & `pykwl-0.0.7/python/src/pykwl/bindings.cpp`

 * *Files 27% similar despite different names*

```diff
@@ -17,9 +17,12 @@
     py::class_<Graph>(m, "Graph")  //
         .def(py::init<bool>())
         .def("add_node", &Graph::add_node, py::arg("label") = 0)
         .def("add_edge", &Graph::add_edge, py::arg("src_node"), py::arg("dst_node"), py::arg("label") = 0);
 
     py::class_<WeisfeilerLeman>(m, "WeisfeilerLeman")  //
         .def(py::init<int>())
+        .def(py::init<int, bool>())
+        .def("get_k", &WeisfeilerLeman::get_k)
+        .def("get_ignore_counting", &WeisfeilerLeman::get_ignore_counting)
         .def("compute_coloring", &WeisfeilerLeman::compute_coloring);
 }
```

### Comparing `pykwl-0.0.6/python/src/pykwl.egg-info/SOURCES.txt` & `pykwl-0.0.7/python/src/pykwl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.6/setup.py` & `pykwl-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import multiprocessing
 
 from pathlib import Path
 
 from setuptools import setup, find_packages, Extension
 from setuptools.command.build_ext import build_ext
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 HERE = Path(__file__).resolve().parent
 
 
 # A CMakeExtension needs a sourcedir instead of a file list.
 # The name must be the _single_ output extension from the CMake build.
 # If you need multiple extensions, see scikit-build.
 class CMakeExtension(Extension):
```

### Comparing `pykwl-0.0.6/src/CMakeLists.txt` & `pykwl-0.0.7/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pykwl-0.0.6/src/graph.cpp` & `pykwl-0.0.7/src/graph.cpp`

 * *Files identical despite different names*

