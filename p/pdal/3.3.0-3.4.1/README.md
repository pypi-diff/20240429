# Comparing `tmp/pdal-3.3.0.tar.gz` & `tmp/pdal-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdal-3.3.0.tar", last modified: Wed Jan  3 20:08:48 2024, max compression
+gzip compressed data, was "pdal-3.4.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `pdal-3.3.0.tar` & `pdal-3.4.1.tar`

### file list

```diff
@@ -1,58 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:08:48.273786 pdal-3.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:08:48.265787 pdal-3.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-03 20:07:09.000000 pdal-3.3.0/.github/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:08:48.265787 pdal-3.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-01-03 20:07:09.000000 pdal-3.3.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-03 20:07:09.000000 pdal-3.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-01-03 20:07:09.000000 pdal-3.3.0/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-01-03 20:07:09.000000 pdal-3.3.0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-01-03 20:07:09.000000 pdal-3.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16484 2024-01-03 20:08:48.273786 pdal-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11908 2024-01-03 20:07:09.000000 pdal-3.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:08:48.265787 pdal-3.3.0/_skbuild/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:08:48.265787 pdal-3.3.0/_skbuild/linux-x86_64-3.12/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:08:48.265787 pdal-3.3.0/_skbuild/linux-x86_64-3.12/cmake-install/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:08:48.269786 pdal-3.3.0/_skbuild/linux-x86_64-3.12/cmake-install/pdal/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-01-03 20:08:26.000000 pdal-3.3.0/_skbuild/linux-x86_64-3.12/cmake-install/pdal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-01-03 20:08:26.000000 pdal-3.3.0/_skbuild/linux-x86_64-3.12/cmake-install/pdal/drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)   346256 2024-01-03 20:08:26.000000 pdal-3.3.0/_skbuild/linux-x86_64-3.12/cmake-install/pdal/libpdalpython.cpython-312-x86_64-linux-gnu.so
--rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-01-03 20:08:26.000000 pdal-3.3.0/_skbuild/linux-x86_64-3.12/cmake-install/pdal/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:08:48.269786 pdal-3.3.0/pdal/
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-01-03 20:07:09.000000 pdal-3.3.0/pdal/PyArray.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-01-03 20:07:09.000000 pdal-3.3.0/pdal/PyArray.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-01-03 20:07:09.000000 pdal-3.3.0/pdal/PyDimension.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12455 2024-01-03 20:07:09.000000 pdal-3.3.0/pdal/PyPipeline.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-01-03 20:07:09.000000 pdal-3.3.0/pdal/PyPipeline.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-01-03 20:07:09.000000 pdal-3.3.0/pdal/StreamableExecutor.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-01-03 20:07:09.000000 pdal-3.3.0/pdal/StreamableExecutor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-01-03 20:07:09.000000 pdal-3.3.0/pdal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-01-03 20:07:09.000000 pdal-3.3.0/pdal/drivers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-01-03 20:07:09.000000 pdal-3.3.0/pdal/libpdalpython.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8308 2024-01-03 20:07:09.000000 pdal-3.3.0/pdal/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:08:48.273786 pdal-3.3.0/pdal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16484 2024-01-03 20:08:48.000000 pdal-3.3.0/pdal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-01-03 20:08:48.000000 pdal-3.3.0/pdal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-03 20:08:48.000000 pdal-3.3.0/pdal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-03 20:08:48.000000 pdal-3.3.0/pdal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-03 20:08:48.000000 pdal-3.3.0/pdal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-01-03 20:07:09.000000 pdal-3.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-03 20:08:48.273786 pdal-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-01-03 20:07:09.000000 pdal-3.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:08:48.269786 pdal-3.3.0/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-03 20:08:48.273786 pdal-3.3.0/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)    36439 2024-01-03 20:07:09.000000 pdal-3.3.0/test/data/1.2-with-color.las
--rw-r--r--   0 runner    (1001) docker     (127)    37417 2024-01-03 20:07:09.000000 pdal-3.3.0/test/data/autzen-utm.las
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-01-03 20:07:09.000000 pdal-3.3.0/test/data/bad.json
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-03 20:07:09.000000 pdal-3.3.0/test/data/bad.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-01-03 20:07:09.000000 pdal-3.3.0/test/data/chip.json
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-03 20:07:09.000000 pdal-3.3.0/test/data/chip.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-01-03 20:07:09.000000 pdal-3.3.0/test/data/mesh.json
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-01-03 20:07:09.000000 pdal-3.3.0/test/data/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-03 20:07:09.000000 pdal-3.3.0/test/data/range.json
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-03 20:07:09.000000 pdal-3.3.0/test/data/range.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-01-03 20:07:09.000000 pdal-3.3.0/test/data/reproject.json
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-03 20:07:09.000000 pdal-3.3.0/test/data/reproject.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-01-03 20:07:09.000000 pdal-3.3.0/test/data/sort.json
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-03 20:07:09.000000 pdal-3.3.0/test/data/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-03 20:07:09.000000 pdal-3.3.0/test/data/test3d.npy
--rw-r--r--   0 runner    (1001) docker     (127)    22155 2024-01-03 20:07:09.000000 pdal-3.3.0/test/test_pipeline.py
+-rw-r--r--   0        0        0       97 2022-11-09 12:37:21.000000 pdal-3.4.1/.gitignore
+-rw-r--r--   0        0        0     3724 2022-11-09 12:37:21.000000 pdal-3.4.1/CHANGES.txt
+-rw-r--r--   0        0        0     1385 2022-11-09 12:37:21.000000 pdal-3.4.1/CMakeLists.txt
+-rw-r--r--   0        0        0     1898 2022-11-09 12:37:21.000000 pdal-3.4.1/LICENSE.txt
+-rw-r--r--   0        0        0    12093 2022-11-09 12:37:21.000000 pdal-3.4.1/README.rst
+-rw-r--r--   0        0        0     1660 2022-11-09 12:37:21.000000 pdal-3.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1467 2022-11-09 12:37:21.000000 pdal-3.4.1/setup.py.off
+-rw-r--r--   0        0        0     6228 2022-11-09 12:37:21.000000 pdal-3.4.1/src/pdal/PyArray.cpp
+-rw-r--r--   0        0        0     3283 2022-11-09 12:37:21.000000 pdal-3.4.1/src/pdal/PyArray.hpp
+-rw-r--r--   0        0        0     3219 2022-11-09 12:37:21.000000 pdal-3.4.1/src/pdal/PyDimension.hpp
+-rw-r--r--   0        0        0    11691 2022-11-09 12:37:21.000000 pdal-3.4.1/src/pdal/PyPipeline.cpp
+-rw-r--r--   0        0        0     3486 2022-11-09 12:37:21.000000 pdal-3.4.1/src/pdal/PyPipeline.hpp
+-rw-r--r--   0        0        0     6947 2022-11-09 12:37:21.000000 pdal-3.4.1/src/pdal/StreamableExecutor.cpp
+-rw-r--r--   0        0        0     3294 2022-11-09 12:37:21.000000 pdal-3.4.1/src/pdal/StreamableExecutor.hpp
+-rw-r--r--   0        0        0      375 2022-11-09 12:37:21.000000 pdal-3.4.1/src/pdal/__init__.py
+-rw-r--r--   0        0        0     2222 2022-11-09 12:37:21.000000 pdal-3.4.1/src/pdal/__main__.py
+-rw-r--r--   0        0        0     2576 2022-11-09 12:37:21.000000 pdal-3.4.1/src/pdal/drivers.py
+-rw-r--r--   0        0        0    11626 2022-11-09 12:37:21.000000 pdal-3.4.1/src/pdal/libpdalpython.cpp
+-rw-r--r--   0        0        0     8308 2022-11-09 12:37:21.000000 pdal-3.4.1/src/pdal/pipeline.py
+-rw-r--r--   0        0        0    36439 2022-11-09 12:37:21.000000 pdal-3.4.1/test/data/1.2-with-color.las
+-rw-r--r--   0        0        0    37417 2022-11-09 12:37:21.000000 pdal-3.4.1/test/data/autzen-utm.las
+-rw-r--r--   0        0        0      111 2022-11-09 12:37:21.000000 pdal-3.4.1/test/data/bad.json
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 pdal-3.4.1/test/data/bad.py
+-rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 pdal-3.4.1/test/data/chip.json
+-rw-r--r--   0        0        0      102 2022-11-09 12:37:21.000000 pdal-3.4.1/test/data/chip.py
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 pdal-3.4.1/test/data/mesh.json
+-rw-r--r--   0        0        0       90 2022-11-09 12:37:21.000000 pdal-3.4.1/test/data/mesh.py
+-rw-r--r--   0        0        0      105 2022-11-09 12:37:21.000000 pdal-3.4.1/test/data/range.json
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 pdal-3.4.1/test/data/range.py
+-rw-r--r--   0        0        0      724 2022-11-09 12:37:21.000000 pdal-3.4.1/test/data/reproject.json
+-rw-r--r--   0        0        0      678 2022-11-09 12:37:21.000000 pdal-3.4.1/test/data/reproject.py
+-rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 pdal-3.4.1/test/data/sort.json
+-rw-r--r--   0        0        0       68 2022-11-09 12:37:21.000000 pdal-3.4.1/test/data/sort.py
+-rw-r--r--   0        0        0      368 2022-11-09 12:37:21.000000 pdal-3.4.1/test/data/test3d.npy
+-rw-r--r--   0        0        0    22155 2022-11-09 12:37:21.000000 pdal-3.4.1/test/test_pipeline.py
+-rw-r--r--   0        0        0    15489 2022-11-09 12:37:21.000000 pdal-3.4.1/PKG-INFO
```

### Comparing `pdal-3.3.0/CHANGES.txt` & `pdal-3.4.1/CHANGES.txt`

 * *Files identical despite different names*

### Comparing `pdal-3.3.0/LICENSE.txt` & `pdal-3.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pdal-3.3.0/PKG-INFO` & `pdal-3.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,93 @@
 Metadata-Version: 2.1
 Name: pdal
-Version: 3.3.0
+Version: 3.4.1
 Summary: Point cloud data processing
+Keywords: point,cloud,spatial
 Home-page: https://pdal.io
 Author: Howard Butler
-Author-email: howard@hobu.co
-Maintainer: Howard Butler
-Maintainer-email: howard@hobu.co
-License: BSD
-Keywords: point cloud spatial
+Author-Email: Unknown <howard@hobu.co>
+Maintainer-Email: Howard Butler <howard@hobu.co>
+License: Unless otherwise indicated, all files in the PDAL distribution are
+        
+          Copyright (c) 2017, Hobu, Inc. (howard@hobu.co)
+        
+        and are released under the terms of the BSD open source license.
+        
+        This file contains the license terms of all files within PDAL.
+        
+        
+        Overall PDAL license (BSD)
+        ===========================
+        
+         Copyright (c) 2017, Hobu, Inc. (howard@hobu.co)
+        
+         All rights reserved.
+        
+         Redistribution and use in source and binary forms, with or without
+         modification, are permitted provided that the following
+         conditions are met:
+        
+             * Redistributions of source code must retain the above copyright
+               notice, this list of conditions and the following disclaimer.
+             * Redistributions in binary form must reproduce the above copyright
+               notice, this list of conditions and the following disclaimer in
+               the documentation and/or other materials provided
+               with the distribution.
+             * Neither the name of Hobu, Inc. or Flaxen Consulting LLC nor the
+               names of its contributors may be used to endorse or promote
+               products derived from this software without specific prior
+               written permission.
+        
+         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+         "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+         LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
+         FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
+         COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
+         INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING,
+         BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS
+         OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED
+         AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
+         OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY
+         OF SUCH DAMAGE.
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: GIS
+Project-URL: Homepage, https://pdal.io
+Project-URL: Documentation, https://pdal.io
+Project-URL: Repository, https://github.com/PDAL/Python
+Project-URL: Changelog, https://github.com/PDAL/python/blob/main/README.rst
+Requires-Python: >=3.9
+Requires-Dist: numpy>=1.22
+Requires-Dist: pandas; extra == "test"
+Requires-Dist: meshio; extra == "test"
+Provides-Extra: test
 Description-Content-Type: text/x-rst
-License-File: LICENSE.txt
-Requires-Dist: numpy
 
 ================================================================================
 PDAL
 ================================================================================
 
 PDAL Python support allows you to process data with PDAL into `Numpy`_ arrays.
 It provides a PDAL extension module to control Python interaction with PDAL.
 Additionally, you can use it to fetch `schema`_ and `metadata`_ from PDAL operations.
 
 Installation
 --------------------------------------------------------------------------------
 
+**Note** The PDAL Python bindings require the PDAL base library installed. Source code can be found at https://pdal.io and `GitHub <https://github.com/PDAL/PDAL>`__.
+
 PyPI
 ................................................................................
 
 PDAL Python support is installable via PyPI:
 
 .. code-block::
 
@@ -328,126 +378,12 @@
 
 .. image:: https://github.com/PDAL/python/workflows/Build/badge.svg
    :target: https://github.com/PDAL/python/actions?query=workflow%3ABuild
 
 Requirements
 ================================================================================
 
-* PDAL 2.5+
+* PDAL 2.6+
 * Python >=3.9
 * Pybind11 (eg :code:`pip install pybind11[global]`)
-* Numpy (eg :code:`pip install numpy`)
-* scikit-build (eg :code:`pip install scikit-build`)
-
-
-Changes
---------------------------------------------------------------------------------
-
-
-3.2.3
-................................................................................
-
-Do not build and include wheels in distro
-
-
-3.2.2
-................................................................................
-
-* Implement move ctor to satisfy MSVC 2019 https://github.com/PDAL/python/commit/667f56bd0ee465f55a14636986e80b0a9cefcf14
-
-
-3.2.1
-................................................................................
-
-* implement #129, add pandas DataFrame i/o for convenience by @hobu in
-  https://github.com/PDAL/python/pull/130
-* harden getMetadata and related calls from getting non-utf-8 'json'  by @hobu
-  in https://github.com/PDAL/python/pull/140
-* ignore DataFrame test if not GeoPandas, give up on Python 3.7 builds by @hobu
-  in https://github.com/PDAL/python/pull/137
-
-3.2.0
-................................................................................
-
-* PDAL base library 2.4.0+ is required
-
-* CMake project name updated to pdal-python
-
-* `srswkt2` property added to allow fetching of SRS info
-
-* pip builds require cmake >= 3.11
-
-* CMAKE_CXX_STANDARD set to c++17 to match PDAL 2.4.x
-
-* Driver and options *actually* uses the library instead of
-  shelling out to `pdal` application :)
-
-* _get_json renamed to toJSON and made public
-
-* Fix #119, 'json' optional kwarg put back for now
-
-* DEVELOPMENT_COMPONENT in CMake FindPython skipped on OSX
-
-* Make sure 'type' gets set when serializing to JSON
-
-3.1.0
-................................................................................
-
-* **Breaking change** – pipeline.metadata now returns a dictionary from
-  json.loads instead of a string.
-
-* pipeline.quickinfo will fetch the PDAL preview() information for a data source.
-  You can use this to fetch header or other information without reading data.
-  https://github.com/PDAL/python/pull/109
-
-* PDAL driver and option collection now uses the PDAL library directly rather
-  than shelling out to the pdal command https://github.com/PDAL/python/pull/107
-
-* Pipelines now support pickling for use with things like Dask
-  https://github.com/PDAL/python/pull/110
-
-
-
-3.0.0
-................................................................................
-
-* Pythonic pipeline creation https://github.com/PDAL/python/pull/91
-
-* Support streaming pipeline execution https://github.com/PDAL/python/pull/94
-
-* Replace Cython with PyBind11 https://github.com/PDAL/python/pull/102
-
-* Remove pdal.pio module https://github.com/PDAL/python/pull/101
-
-* Move readers.numpy and filters.python to separate repository https://github.com/PDAL/python/pull/104
-
-* Miscellaneous refactorings and cleanups
-
-2.3.5
-................................................................................
-
-* Fix memory leak https://github.com/PDAL/python/pull/74
-
-* Handle metadata with invalid unicode by erroring https://github.com/PDAL/python/pull/74
-
-2.3.0
-................................................................................
-
-* PDAL Python support 2.3.0 requires PDAL 2.1+. Older PDAL base libraries
-  likely will not work.
-
-* Python support built using scikit-build
-
-* readers.numpy and filters.python are installed along with the extension.
-
-* Pipeline can take in a list of arrays that are passed to readers.numpy
-
-* readers.numpy now supports functions that return arrays. See
-  https://pdal.io/stages/readers.numpy.html for more detail.
-
-2.0.0
-................................................................................
-
-* PDAL Python extension is now in its own repository on its own release
-  schedule at https://github.com/PDAL/python
-
-* Extension now builds and works under PDAL OSGeo4W64 on Windows.
+* Numpy >= 1.22 (eg :code:`pip install numpy`)
+* scikit-build-core (eg :code:`pip install scikit-build-core`)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pdal-3.3.0/README.rst` & `pdal-3.4.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 PDAL Python support allows you to process data with PDAL into `Numpy`_ arrays.
 It provides a PDAL extension module to control Python interaction with PDAL.
 Additionally, you can use it to fetch `schema`_ and `metadata`_ from PDAL operations.
 
 Installation
 --------------------------------------------------------------------------------
 
+**Note** The PDAL Python bindings require the PDAL base library installed. Source code can be found at https://pdal.io and `GitHub <https://github.com/PDAL/PDAL>`__.
+
 PyPI
 ................................................................................
 
 PDAL Python support is installable via PyPI:
 
 .. code-block::
 
@@ -303,12 +305,12 @@
 
 .. image:: https://github.com/PDAL/python/workflows/Build/badge.svg
    :target: https://github.com/PDAL/python/actions?query=workflow%3ABuild
 
 Requirements
 ================================================================================
 
-* PDAL 2.5+
+* PDAL 2.6+
 * Python >=3.9
 * Pybind11 (eg :code:`pip install pybind11[global]`)
-* Numpy (eg :code:`pip install numpy`)
-* scikit-build (eg :code:`pip install scikit-build`)
+* Numpy >= 1.22 (eg :code:`pip install numpy`)
+* scikit-build-core (eg :code:`pip install scikit-build-core`)
```

### Comparing `pdal-3.3.0/_skbuild/linux-x86_64-3.12/cmake-install/pdal/drivers.py` & `pdal-3.4.1/src/pdal/drivers.py`

 * *Files identical despite different names*

### Comparing `pdal-3.3.0/_skbuild/linux-x86_64-3.12/cmake-install/pdal/pipeline.py` & `pdal-3.4.1/src/pdal/pipeline.py`

 * *Files identical despite different names*

### Comparing `pdal-3.3.0/pdal/PyArray.cpp` & `pdal-3.4.1/src/pdal/PyArray.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -88,17 +88,14 @@
 }
 
 } // unnamed namespace
 
 
 Array::Array(PyArrayObject* array) : m_array(array), m_rowMajor(true)
 {
-    if (_import_array() < 0)
-        throw pdal_error("Could not import numpy.core.multiarray.");
-
     Py_XINCREF(array);
 
     PyArray_Descr *dtype = PyArray_DTYPE(m_array);
     npy_intp ndims = PyArray_NDIM(m_array);
     npy_intp *shape = PyArray_SHAPE(m_array);
     int numFields = (dtype->fields == Py_None) ?
         0 :
```

### Comparing `pdal-3.3.0/pdal/PyArray.hpp` & `pdal-3.4.1/src/pdal/PyArray.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -31,16 +31,25 @@
 * OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY
 * OF SUCH DAMAGE.
 ****************************************************************************/
 
 #pragma once
 
 #include <pdal/PointView.hpp>
+
+#define NPY_TARGET_VERSION NPY_1_22_API_VERSION
+#define NPY_NO_DEPRECATED_API NPY_1_22_API_VERSION
+
+#define NO_IMPORT_ARRAY
+#define PY_ARRAY_UNIQUE_SYMBOL PDAL_ARRAY_API
+
 #include <pdal/io/MemoryViewReader.hpp>
+
 #include <numpy/ndarraytypes.h>
+#include <numpy/arrayobject.h>
 
 #include <vector>
 #include <memory>
 
 namespace pdal
 {
 namespace python
```

### Comparing `pdal-3.3.0/pdal/PyDimension.hpp` & `pdal-3.4.1/src/pdal/PyDimension.hpp`

 * *Files identical despite different names*

### Comparing `pdal-3.3.0/pdal/PyPipeline.cpp` & `pdal-3.4.1/src/pdal/PyPipeline.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -207,24 +207,15 @@
     std::stringstream strm;
     pdal::Utils::toJSON(summary, strm);
     return strm.str();
 }
 
 void PipelineExecutor::addArrayReaders(std::vector<std::shared_ptr<Array>> arrays)
 {
-    // Make the symbols in pdal_base global so that they're accessible
-    // to PDAL plugins.  Python dlopen's this extension with RTLD_LOCAL,
-    // which means that without this, symbols in libpdal_base aren't available
-    // for resolution of symbols on future runtime linking.  This is an issue
-    // on Alpine and other Linux variants that don't use UNIQUE symbols
-    // for C++ template statics only.  Without this, you end up with multiple
-    // copies of template statics.
-#ifndef _WIN32
-    ::dlopen("libpdal_base.so", RTLD_NOLOAD | RTLD_GLOBAL);
-#endif
+
     if (arrays.empty())
         return;
 
     std::vector<Stage *> roots = m_manager.roots();
     if (roots.size() != 1)
         throw pdal_error("Filter pipeline must contain a single root stage.");
 
@@ -316,16 +307,14 @@
     PyDict_SetItemString(dtype_dict, "formats", formats);
     return dtype_dict;
 }
 
 
 PyArrayObject* viewToNumpyArray(PointViewPtr view)
 {
-    if (_import_array() < 0)
-        throw pdal_error("Could not import numpy.core.multiarray.");
 
     PyObject* dtype_dict = buildNumpyDescriptor(view->layout());
     PyArray_Descr *dtype = nullptr;
     if (PyArray_DescrConverter(dtype_dict, &dtype) == NPY_FAIL)
         throw pdal_error("Unable to build numpy dtype");
     Py_XDECREF(dtype_dict);
 
@@ -340,17 +329,14 @@
         view->getPackedPoint(types, idx, (char *)PyArray_GETPTR1(array, idx));
     return array;
 }
 
 
 PyArrayObject* meshToNumpyArray(const TriangularMesh* mesh)
 {
-    if (_import_array() < 0)
-        throw pdal_error("Could not import numpy.core.multiarray.");
-
     // Build up a numpy dtype dictionary
     //
     // {'formats': ['f8', 'f8', 'f8', 'u2', 'u1', 'u1', 'u1', 'u1', 'u1',
     //              'f4', 'u1', 'u2', 'f8', 'u2', 'u2', 'u2'],
     // 'names': ['X', 'Y', 'Z', 'Intensity', 'ReturnNumber',
     //           'NumberOfReturns', 'ScanDirectionFlag', 'EdgeOfFlightLine',
     //           'Classification', 'ScanAngleRank', 'UserData',
```

### Comparing `pdal-3.3.0/pdal/PyPipeline.hpp` & `pdal-3.4.1/src/pdal/PyPipeline.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -31,14 +31,21 @@
 * OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY
 * OF SUCH DAMAGE.
 ****************************************************************************/
 
 #pragma once
 
 #include <pdal/PipelineManager.hpp>
+
+#define NPY_TARGET_VERSION NPY_1_22_API_VERSION
+#define NPY_NO_DEPRECATED_API NPY_1_22_API_VERSION
+
+#define NO_IMPORT_ARRAY
+#define PY_ARRAY_UNIQUE_SYMBOL PDAL_ARRAY_API
+
 #include <numpy/arrayobject.h>
 
 namespace pdal
 {
 namespace python
 {
```

### Comparing `pdal-3.3.0/pdal/StreamableExecutor.cpp` & `pdal-3.4.1/src/pdal/StreamableExecutor.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 * OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY
 * OF SUCH DAMAGE.
 ****************************************************************************/
 
 #include "PyPipeline.hpp"
 #include "StreamableExecutor.hpp"
 
+#define NO_IMPORT_ARRAY
+#define PY_ARRAY_UNIQUE_SYMBOL PDAL_ARRAY_API
+
 #include <Python.h>
 #include <numpy/arrayobject.h>
 
 #include <pdal/Stage.hpp>
 #include <pdal/pdal_features.hpp>
 
 namespace pdal
@@ -63,16 +66,15 @@
 
 void PythonPointTable::finalize()
 {
     BasePointTable::finalize();
 
     // create dtype
     auto gil = PyGILState_Ensure();
-    if (_import_array() < 0)
-        std::cerr << "Could not import array!\n";
+
     PyObject *dtype_dict = buildNumpyDescriptor(&m_layout);
     if (PyArray_DescrConverter(dtype_dict, &m_dtype) == NPY_FAIL)
         throw pdal_error("Unable to create numpy dtype");
     Py_XDECREF(dtype_dict);
     PyGILState_Release(gil);
 
     py_createArray();
@@ -98,16 +100,16 @@
     // copy the non-skipped elements to the beginning
     npy_intp dest_idx = 0;
     for (PointId src_idx = 0; src_idx < numPoints(); src_idx++)
         if (!skip(src_idx))
         {
             if (src_idx != dest_idx)
             {
-                PyObject* src_item = PyArray_GETITEM(m_curArray, PyArray_GETPTR1(m_curArray, src_idx));
-                PyArray_SETITEM(m_curArray, PyArray_GETPTR1(m_curArray, dest_idx), src_item);
+                PyObject* src_item = PyArray_GETITEM(m_curArray, (const char*) PyArray_GETPTR1(m_curArray, src_idx));
+                PyArray_SETITEM(m_curArray, (char*) PyArray_GETPTR1(m_curArray, dest_idx), src_item);
                 Py_XDECREF(src_item);
             }
             dest_idx++;
         }
     PyArray_Resize(m_curArray, &dims, true, NPY_CORDER);
     PyGILState_Release(gil);
 }
```

### Comparing `pdal-3.3.0/pdal/StreamableExecutor.hpp` & `pdal-3.4.1/src/pdal/StreamableExecutor.hpp`

 * *Files identical despite different names*

### Comparing `pdal-3.3.0/pdal/libpdalpython.cpp` & `pdal-3.4.1/src/pdal/libpdalpython.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 #include <pybind11/numpy.h>
 #include <pybind11/stl/filesystem.h>
 #include <iostream>
 
 #include <pdal/pdal_config.hpp>
 #include <pdal/StageFactory.hpp>
 
+#define NPY_TARGET_VERSION NPY_1_22_API_VERSION
+#define NPY_NO_DEPRECATED_API NPY_1_22_API_VERSION
+
+#define PY_ARRAY_UNIQUE_SYMBOL PDAL_ARRAY_API
+
+#include <numpy/arrayobject.h>
+
 #include "PyArray.hpp"
 #include "PyDimension.hpp"
 #include "PyPipeline.hpp"
 #include "StreamableExecutor.hpp"
 
 namespace py = pybind11;
 
@@ -26,15 +33,14 @@
                 "debug"_a = pdal::Config::debugInformation(),
                 "sha1"_a = pdal::Config::sha1(),
                 "plugin"_a = pdal::Config::pluginInstallPath()
         );
     };
 
    std::vector<py::dict> getDrivers() {
-        py::gil_scoped_acquire acquire;
         std::vector<py::dict> drivers;
 
         pdal::StageFactory f(false);
         pdal::PluginManager<pdal::Stage>::loadAll();
         pdal::StringList stages = pdal::PluginManager<pdal::Stage>::names();
 
         pdal::StageExtensions& extensions = pdal::PluginManager<pdal::Stage>::extensions();
@@ -55,15 +61,14 @@
             drivers.push_back(std::move(d));
         }
         return drivers;
 
     };
 
    py::object getOptions() {
-        py::gil_scoped_acquire acquire;
         py::object json = py::module_::import("json");
         py::dict stageOptions;
 
         pdal::StageFactory f;
         pdal::PluginManager<pdal::Stage>::loadAll();
         pdal::StringList stages = pdal::PluginManager<pdal::Stage>::names();
 
@@ -90,15 +95,14 @@
             stageOptions[pybind11::cast(name)] = std::move(j);
        }
         return stageOptions;
 
     };
 
     std::vector<py::dict> getDimensions() {
-        py::gil_scoped_acquire acquire;
         py::object np = py::module_::import("numpy");
         py::object dtype = np.attr("dtype");
         std::vector<py::dict> dims;
         for (const auto& dim: getValidDimensions())
         {
             py::dict d(
                 "name"_a=dim.name,
@@ -108,21 +112,19 @@
             dims.push_back(std::move(d));
         }
         return dims;
     };
 
     std::string getReaderDriver(std::filesystem::path const& p)
     {
-        py::gil_scoped_acquire acquire;
         return StageFactory::inferReaderDriver(p.string());
     }
 
     std::string getWriterDriver(std::filesystem::path const& p)
     {
-        py::gil_scoped_acquire acquire;
         return StageFactory::inferWriterDriver(p.string());
     }
 
     using pdal::python::PipelineExecutor;
     using pdal::python::StreamableExecutor;
 
     class PipelineIterator : public StreamableExecutor {
@@ -138,15 +140,14 @@
             if (!arr)
                 throw py::stop_iteration();
 
             return py::reinterpret_steal<py::array>((PyObject*)arr);
         }
 
         py::object getMetadata() {
-            py::gil_scoped_acquire acquire;
             py::object json = py::module_::import("json");
 
             std::stringstream strm;
             MetadataNode root = (StreamableExecutor::getMetadata()).clone("metadata");
             pdal::Utils::toJSON(root, strm);
 
 
@@ -186,15 +187,14 @@
         std::unique_ptr<PipelineIterator> iterator(int chunk_size, int prefetch) {
             return std::unique_ptr<PipelineIterator>(new PipelineIterator(
                 getJson(), _inputs, _loglevel, chunk_size, prefetch
             ));
         }
 
         void setInputs(std::vector<py::array> ndarrays) {
-            py::gil_scoped_acquire acquire;
             _inputs.clear();
             for (const auto& ndarray: ndarrays) {
                 PyArrayObject* ndarray_ptr = (PyArrayObject*)ndarray.ptr();
                 _inputs.push_back(std::make_shared<pdal::python::Array>(ndarray_ptr));
             }
             delExecutor();
         }
@@ -205,15 +205,14 @@
 
         std::string getLog() { return getExecutor()->getLog(); }
 
         std::string getPipeline() { return getExecutor()->getPipeline(); }
         std::string getSrsWKT2() { return getExecutor()->getSrsWKT2(); }
 
         py::object getQuickInfo() {
-            py::gil_scoped_acquire acquire;
             py::object json = py::module_::import("json");
 
             std::string response;
             {
                 py::gil_scoped_release release;
                 response = getExecutor()->getQuickInfo();
             }
@@ -271,37 +270,46 @@
         bool hasInputs() { return !_inputs.empty(); }
 
         void copyInputs(const Pipeline& other) { _inputs = other._inputs; }
 
         void delExecutor() { _executor.reset(); }
 
         PipelineExecutor* getExecutor() {
+            // We need to acquire the GIL before we create the executor
+            // because this method does Python init stuff but pybind11 doesn't
+            // automatically encapsulate it with a gil_scoped_acquire like it
+            // does for all of the other methods it knows about
             py::gil_scoped_acquire acquire;
             if (!_executor)
                 _executor.reset(new PipelineExecutor(getJson(), _inputs, _loglevel));
             return _executor.get();
         }
 
     private:
         std::unique_ptr<PipelineExecutor> _executor;
         std::vector<std::shared_ptr<pdal::python::Array>> _inputs;
         int _loglevel;
     };
 
+
+
     PYBIND11_MODULE(libpdalpython, m)
     {
+        _import_array();
+
     py::class_<PipelineIterator>(m, "PipelineIterator")
         .def("__iter__", [](PipelineIterator &it) -> PipelineIterator& { return it; })
         .def("__next__", &PipelineIterator::executeNext)
         .def_property_readonly("log", &PipelineIterator::getLog)
         .def_property_readonly("schema", &PipelineIterator::getSchema)
         .def_property_readonly("srswkt2", &PipelineIterator::getSrsWKT2)
         .def_property_readonly("pipeline", &PipelineIterator::getPipeline)
         .def_property_readonly("metadata", &PipelineIterator::getMetadata);
 
+
     py::class_<Pipeline>(m, "Pipeline")
         .def(py::init<>())
         .def("execute", &Pipeline::execute)
         .def("execute_streaming", &Pipeline::executeStream, "chunk_size"_a=10000)
         .def("iterator", &Pipeline::iterator, "chunk_size"_a=10000, "prefetch"_a=0)
         .def_property("inputs", nullptr, &Pipeline::setInputs)
         .def_property("loglevel", &Pipeline::getLoglevel, &Pipeline::setLogLevel)
@@ -319,10 +327,16 @@
         .def("_del_executor", &Pipeline::delExecutor);
     m.def("getInfo", &getInfo);
     m.def("getDrivers", &getDrivers);
     m.def("getOptions", &getOptions);
     m.def("getDimensions", &getDimensions);
     m.def("infer_reader_driver", &getReaderDriver);
     m.def("infer_writer_driver", &getWriterDriver);
+
+    if (pdal::Config::versionMajor() < 2)
+        throw pybind11::import_error("PDAL version must be >= 2.6");
+
+    if (pdal::Config::versionMajor() == 2 && pdal::Config::versionMinor() < 6)
+        throw pybind11::import_error("PDAL version must be >= 2.6");
     };
 
 }; // namespace pdal
```

### Comparing `pdal-3.3.0/setup.py` & `pdal-3.4.1/setup.py.off`

 * *Files identical despite different names*

### Comparing `pdal-3.3.0/test/data/1.2-with-color.las` & `pdal-3.4.1/test/data/1.2-with-color.las`

 * *Files identical despite different names*

### Comparing `pdal-3.3.0/test/data/autzen-utm.las` & `pdal-3.4.1/test/data/autzen-utm.las`

 * *Files identical despite different names*

### Comparing `pdal-3.3.0/test/data/reproject.json` & `pdal-3.4.1/test/data/reproject.json`

 * *Files identical despite different names*

### Comparing `pdal-3.3.0/test/data/reproject.py` & `pdal-3.4.1/test/data/reproject.py`

 * *Files identical despite different names*

### Comparing `pdal-3.3.0/test/test_pipeline.py` & `pdal-3.4.1/test/test_pipeline.py`

 * *Files identical despite different names*

