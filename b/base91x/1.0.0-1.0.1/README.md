# Comparing `tmp/base91x-1.0.0.tar.gz` & `tmp/base91x-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "base91x-1.0.0.tar", last modified: Sun Feb 19 09:46:28 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `base91x-1.0.0.tar` & `base91x-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 09:46:28.613418 base91x-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-19 09:45:39.000000 base91x-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-02-19 09:46:28.613418 base91x-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-02-19 09:45:39.000000 base91x-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-02-19 09:45:39.000000 base91x-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-19 09:46:28.613418 base91x-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-19 09:45:39.000000 base91x-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 09:46:28.609418 base91x-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 09:46:28.609418 base91x-1.0.0/src/base91x/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-02-19 09:45:39.000000 base91x-1.0.0/src/base91x/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-02-19 09:45:39.000000 base91x-1.0.0/src/base91x/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-02-19 09:45:39.000000 base91x-1.0.0/src/base91x/base91x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 09:46:28.613418 base91x-1.0.0/src/base91x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-02-19 09:46:28.000000 base91x-1.0.0/src/base91x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-19 09:46:28.000000 base91x-1.0.0/src/base91x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 09:46:28.000000 base91x-1.0.0/src/base91x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-19 09:46:28.000000 base91x-1.0.0/src/base91x.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-19 09:46:28.000000 base91x-1.0.0/src/base91x.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 09:46:28.613418 base91x-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-02-19 09:45:39.000000 base91x-1.0.0/tests/test_base91x.py
+-rw-r--r--   0        0        0    14266 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeCache.txt
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeLists.txt
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 base91x-1.0.1/CTestTestfile.cmake
+-rw-r--r--   0        0        0    10930 2020-02-02 00:00:00.000000 base91x-1.0.1/Makefile
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 base91x-1.0.1/SECURITY.md
+-rwxr-xr-x   0        0        0    32080 2020-02-02 00:00:00.000000 base91x-1.0.1/base91x
+-rw-r--r--   0        0        0     2403 2020-02-02 00:00:00.000000 base91x-1.0.1/cmake_install.cmake
+-rwxr-xr-x   0        0        0    22248 2020-02-02 00:00:00.000000 base91x-1.0.1/perf_base91x
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 base91x-1.0.1/requirements.txt
+-rwxr-xr-x   0        0        0    35224 2020-02-02 00:00:00.000000 base91x-1.0.1/test_base91x
+-rw-r--r--   0        0        0    60736 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/CMakeConfigureLog.yaml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/CMakeDirectoryInformation.cmake
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/CMakeRuleHashes.txt
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/Makefile.cmake
+-rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/Makefile2
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/TargetDirectories.txt
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/cmake.check_cache
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/progress.marks
+-rw-r--r--   0        0        0     2750 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/3.29.2/CMakeCCompiler.cmake
+-rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/3.29.2/CMakeCXXCompiler.cmake
+-rwxr-xr-x   0        0        0    15968 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/3.29.2/CMakeDetermineCompilerABI_C.bin
+-rwxr-xr-x   0        0        0    15992 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/3.29.2/CMakeDetermineCompilerABI_CXX.bin
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/3.29.2/CMakeSystem.cmake
+-rw-r--r--   0        0        0    27496 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/3.29.2/CompilerIdC/CMakeCCompilerId.c
+-rwxr-xr-x   0        0        0    16088 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/3.29.2/CompilerIdC/a.out
+-rw-r--r--   0        0        0    27064 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/3.29.2/CompilerIdCXX/CMakeCXXCompilerId.cpp
+-rwxr-xr-x   0        0        0    16096 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/3.29.2/CompilerIdCXX/a.out
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/base91x.dir/DependInfo.cmake
+-rw-r--r--   0        0        0     4471 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/base91x.dir/build.make
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/base91x.dir/cmake_clean.cmake
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/base91x.dir/compiler_depend.make
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/base91x.dir/compiler_depend.ts
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/base91x.dir/depend.make
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/base91x.dir/flags.make
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/base91x.dir/link.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/base91x.dir/progress.make
+-rw-r--r--   0        0        0    26896 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/base91x.dir/src/base91x.cpp.o
+-rw-r--r--   0        0        0     9867 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/base91x.dir/src/base91x.cpp.o.d
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf.dir/DependInfo.cmake
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf.dir/build.make
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf.dir/cmake_clean.cmake
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf.dir/compiler_depend.make
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf.dir/compiler_depend.ts
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf.dir/progress.make
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf_base91x.dir/DependInfo.cmake
+-rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf_base91x.dir/build.make
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf_base91x.dir/cmake_clean.cmake
+-rw-r--r--   0        0        0    11452 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf_base91x.dir/compiler_depend.internal
+-rw-r--r--   0        0        0    23684 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf_base91x.dir/compiler_depend.make
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf_base91x.dir/compiler_depend.ts
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf_base91x.dir/depend.make
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf_base91x.dir/flags.make
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf_base91x.dir/link.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf_base91x.dir/progress.make
+-rw-r--r--   0        0        0    18104 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf_base91x.dir/perf/perf_base91x.cpp.o
+-rw-r--r--   0        0        0    11743 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/perf_base91x.dir/perf/perf_base91x.cpp.o.d
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/test_base91x.dir/DependInfo.cmake
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/test_base91x.dir/build.make
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/test_base91x.dir/cmake_clean.cmake
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/test_base91x.dir/compiler_depend.make
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/test_base91x.dir/compiler_depend.ts
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/test_base91x.dir/depend.make
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/test_base91x.dir/flags.make
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/test_base91x.dir/link.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/test_base91x.dir/progress.make
+-rw-r--r--   0        0        0    46216 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/test_base91x.dir/tests/test_base91x.cpp.o
+-rw-r--r--   0        0        0    11745 2020-02-02 00:00:00.000000 base91x-1.0.1/CMakeFiles/test_base91x.dir/tests/test_base91x.cpp.o.d
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 base91x-1.0.1/Testing/Temporary/CTestCostData.txt
+-rw-r--r--   0        0        0     8410 2020-02-02 00:00:00.000000 base91x-1.0.1/Testing/Temporary/LastTest.log
+-rw-r--r--   0        0        0     8035 2020-02-02 00:00:00.000000 base91x-1.0.1/include/base91x.hpp
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 base91x-1.0.1/perf/__main__.py
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 base91x-1.0.1/perf/perf_base91x.cpp
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 base91x-1.0.1/src/base91x.cpp
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 base91x-1.0.1/src/base91x/__init__.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 base91x-1.0.1/src/base91x/__main__.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 base91x-1.0.1/src/base91x/base91x.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 base91x-1.0.1/src/base91x/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 base91x-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     8376 2020-02-02 00:00:00.000000 base91x-1.0.1/tests/test_base91x.cpp
+-rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 base91x-1.0.1/tests/test_base91x.py
+-rw-r--r--   0        0        0     4062 2020-02-02 00:00:00.000000 base91x-1.0.1/xmlcov/coverage.xml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 base91x-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 base91x-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 base91x-1.0.1/README.md
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 base91x-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 base91x-1.0.1/PKG-INFO
```

### Comparing `base91x-1.0.0/LICENSE` & `base91x-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `base91x-1.0.0/PKG-INFO` & `base91x-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,36 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: base91x
-Version: 1.0.0
+Version: 1.0.1
 Summary: base91x encoding/decoding library
+Project-URL: Homepage, https://github.com/babenek/base91x
+Project-URL: Bug Tracker, https://github.com/babenek/base91x/issues
 Author-email: Roman Babenko <babenek@users.noreply.github.com>
-Project-URL: Homepage, https://github.com/babenek/base91
-Project-URL: Bug Tracker, https://github.com/babenek/base91/issues
-Keywords: encode,decode,base91x
-Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+Keywords: base91x,decode,encode
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # base91x
+https://pypi.org/project/base91x/
+
+
+[![Test](https://github.com/babenek/base91x/actions/workflows/main.yml/badge.svg)](https://github.com/babenek/base91x/actions/workflows/main.yml)
+[![codecov](https://codecov.io/gh/babenek/base91x/branch/main/graph/badge.svg)](https://codecov.io/gh/babenek/base91x)
+[![GitHub release (latestSemVer)](https://img.shields.io/github/v/release/babenek/base91x)](https://github.com/babenek/base91x/releases)
+[![PyPI](https://img.shields.io/pypi/v/base91x)](https://pypi.org/project/base91x/)
+[![License](https://img.shields.io/badge/licence-MIT-green.svg?style=flat)](LICENSE)
+[![Python](https://img.shields.io/pypi/pyversions/base91x.svg)](https://badge.fury.io/py/base91x)
 
 This base91x method provides data encoding and decoding 
 using numeric system of base 91 with specific alphabet that does not require
 escaping any symbols in C, C++ (and many other languages?) string.
 'x' - means the alphabet was obtained with XOR function.
```

### Comparing `base91x-1.0.0/README.md` & `base91x-1.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,17 @@
 # base91x
+https://pypi.org/project/base91x/
+
+
+[![Test](https://github.com/babenek/base91x/actions/workflows/main.yml/badge.svg)](https://github.com/babenek/base91x/actions/workflows/main.yml)
+[![codecov](https://codecov.io/gh/babenek/base91x/branch/main/graph/badge.svg)](https://codecov.io/gh/babenek/base91x)
+[![GitHub release (latestSemVer)](https://img.shields.io/github/v/release/babenek/base91x)](https://github.com/babenek/base91x/releases)
+[![PyPI](https://img.shields.io/pypi/v/base91x)](https://pypi.org/project/base91x/)
+[![License](https://img.shields.io/badge/licence-MIT-green.svg?style=flat)](LICENSE)
+[![Python](https://img.shields.io/pypi/pyversions/base91x.svg)](https://badge.fury.io/py/base91x)
 
 This base91x method provides data encoding and decoding 
 using numeric system of base 91 with specific alphabet that does not require
 escaping any symbols in C, C++ (and many other languages?) string.
 'x' - means the alphabet was obtained with XOR function.
```

### Comparing `base91x-1.0.0/src/base91x/__main__.py` & `base91x-1.0.1/src/base91x/__main__.py`

 * *Files identical despite different names*

### Comparing `base91x-1.0.0/src/base91x/base91x.py` & `base91x-1.0.1/src/base91x/base91x.py`

 * *Files identical despite different names*

### Comparing `base91x-1.0.0/tests/test_base91x.py` & `base91x-1.0.1/tests/test_base91x.py`

 * *Files identical despite different names*

