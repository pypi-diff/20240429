# Comparing `tmp/pycentroids-0.2.0rc2.tar.gz` & `tmp/pycentroids-0.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycentroids-0.2.0rc2.tar", last modified: Mon Jun 22 02:07:47 2020, max compression
+gzip compressed data, was "pycentroids-0.2.0rc3.tar", last modified: Mon Apr 29 15:47:05 2024, max compression
```

## Comparing `pycentroids-0.2.0rc2.tar` & `pycentroids-0.2.0rc3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2020-06-22 02:07:47.000000 pycentroids-0.2.0rc2/
--rw-r--r--   0 mrakitin   (501) staff       (20)     1637 2020-06-15 15:18:46.000000 pycentroids-0.2.0rc2/CMakeLists.txt
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2020-06-22 02:07:47.000000 pycentroids-0.2.0rc2/LICENSE/
--rw-r--r--   0 mrakitin   (501) staff       (20)     1537 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/LICENSE/LICENSE
--rw-r--r--   0 mrakitin   (501) staff       (20)     1558 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/LICENSE/LICENSE_LMFIT
--rw-r--r--   0 mrakitin   (501) staff       (20)      536 2020-06-22 02:05:34.000000 pycentroids-0.2.0rc2/MANIFEST.in
--rw-r--r--   0 mrakitin   (501) staff       (20)     2052 2020-06-22 02:07:47.000000 pycentroids-0.2.0rc2/PKG-INFO
--rw-r--r--   0 mrakitin   (501) staff       (20)     1458 2020-06-22 02:06:12.000000 pycentroids-0.2.0rc2/README.md
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2020-06-22 02:07:47.000000 pycentroids-0.2.0rc2/cmake/
--rw-r--r--   0 mrakitin   (501) staff       (20)      288 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/cmake/FindSphinx.cmake
--rw-r--r--   0 mrakitin   (501) staff       (20)      607 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/cmake/PreventInSourceBuilds.cmake
--rw-r--r--   0 mrakitin   (501) staff       (20)     5916 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/cmake/cpplint.cmake
--rw-r--r--   0 mrakitin   (501) staff       (20)     1317 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/cmake/version.cmake
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2020-06-22 02:07:46.000000 pycentroids-0.2.0rc2/docs/
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2020-06-22 02:07:47.000000 pycentroids-0.2.0rc2/docs/doxygen/
--rw-r--r--   0 mrakitin   (501) staff       (20)      696 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/docs/doxygen/CMakeLists.txt
--rw-r--r--   0 mrakitin   (501) staff       (20)   110739 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/docs/doxygen/Doxyfile.in
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2020-06-22 02:07:47.000000 pycentroids-0.2.0rc2/docs/sphinx/
--rw-r--r--   0 mrakitin   (501) staff       (20)      712 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/docs/sphinx/CMakeLists.txt
--rw-r--r--   0 mrakitin   (501) staff       (20)      339 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/docs/sphinx/api.rst
--rw-r--r--   0 mrakitin   (501) staff       (20)     8087 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/docs/sphinx/conf.py.in
--rw-r--r--   0 mrakitin   (501) staff       (20)    54289 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/docs/sphinx/first_pass.png
--rw-r--r--   0 mrakitin   (501) staff       (20)     2142 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/docs/sphinx/first_pass.rst
--rw-r--r--   0 mrakitin   (501) staff       (20)      505 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/docs/sphinx/index.rst
--rw-r--r--   0 mrakitin   (501) staff       (20)     5781 2020-06-15 15:18:58.000000 pycentroids-0.2.0rc2/docs/sphinx/second_pass.rst
--rw-r--r--   0 mrakitin   (501) staff       (20)      833 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/docs/sphinx/theory.rst
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2020-06-22 02:07:47.000000 pycentroids-0.2.0rc2/lib/
--rw-r--r--   0 mrakitin   (501) staff       (20)     2746 2020-06-15 15:18:46.000000 pycentroids-0.2.0rc2/lib/CMakeLists.txt
--rw-r--r--   0 mrakitin   (501) staff       (20)      123 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/lib/centroids-config.cmake.in
--rw-r--r--   0 mrakitin   (501) staff       (20)     5158 2020-06-22 02:05:34.000000 pycentroids-0.2.0rc2/lib/centroids.h
--rw-r--r--   0 mrakitin   (501) staff       (20)    35771 2020-06-22 02:05:34.000000 pycentroids-0.2.0rc2/lib/photons.cpp
--rw-r--r--   0 mrakitin   (501) staff       (20)     6016 2020-06-22 02:05:34.000000 pycentroids-0.2.0rc2/lib/photons.h
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2020-06-22 02:07:47.000000 pycentroids-0.2.0rc2/lmfit/
--rw-r--r--   0 mrakitin   (501) staff       (20)     4745 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/lmfit/lminvert.c
--rw-r--r--   0 mrakitin   (501) staff       (20)      451 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/lmfit/lminvert.h
--rw-r--r--   0 mrakitin   (501) staff       (20)    46613 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/lmfit/lmmin.c
--rw-r--r--   0 mrakitin   (501) staff       (20)     3593 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/lmfit/lmmin.h
--rw-r--r--   0 mrakitin   (501) staff       (20)     3562 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/lmfit/lmstruct.h
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2020-06-22 02:07:47.000000 pycentroids-0.2.0rc2/pycentroids/
--rw-r--r--   0 mrakitin   (501) staff       (20)      195 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/pycentroids/__init__.py
--rw-r--r--   0 mrakitin   (501) staff       (20)      500 2020-06-22 02:07:47.000000 pycentroids-0.2.0rc2/pycentroids/_version.py
--rw-r--r--   0 mrakitin   (501) staff       (20)     5462 2020-06-22 02:05:34.000000 pycentroids-0.2.0rc2/pycentroids/pycentroids.py
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2020-06-22 02:07:47.000000 pycentroids-0.2.0rc2/pycentroids/tests/
--rw-r--r--   0 mrakitin   (501) staff       (20)        0 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/pycentroids/tests/__init__.py
--rw-r--r--   0 mrakitin   (501) staff       (20)      219 2020-06-15 15:18:46.000000 pycentroids-0.2.0rc2/pycentroids/tests/test_install.py
--rw-r--r--   0 mrakitin   (501) staff       (20)     8222 2020-06-22 02:05:34.000000 pycentroids-0.2.0rc2/pycentroids/tests/test_photons.py
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2020-06-22 02:07:47.000000 pycentroids-0.2.0rc2/pycentroids.egg-info/
--rw-r--r--   0 mrakitin   (501) staff       (20)     2052 2020-06-22 02:07:46.000000 pycentroids-0.2.0rc2/pycentroids.egg-info/PKG-INFO
--rw-r--r--   0 mrakitin   (501) staff       (20)     1067 2020-06-22 02:07:46.000000 pycentroids-0.2.0rc2/pycentroids.egg-info/SOURCES.txt
--rw-r--r--   0 mrakitin   (501) staff       (20)        1 2020-06-22 02:07:46.000000 pycentroids-0.2.0rc2/pycentroids.egg-info/dependency_links.txt
--rw-r--r--   0 mrakitin   (501) staff       (20)        1 2020-06-22 02:07:46.000000 pycentroids-0.2.0rc2/pycentroids.egg-info/not-zip-safe
--rw-r--r--   0 mrakitin   (501) staff       (20)       30 2020-06-22 02:07:46.000000 pycentroids-0.2.0rc2/pycentroids.egg-info/requires.txt
--rw-r--r--   0 mrakitin   (501) staff       (20)       25 2020-06-22 02:07:46.000000 pycentroids-0.2.0rc2/pycentroids.egg-info/top_level.txt
-drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2020-06-22 02:07:47.000000 pycentroids-0.2.0rc2/python/
--rw-r--r--   0 mrakitin   (501) staff       (20)      699 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/python/CMakeLists.txt
--rw-r--r--   0 mrakitin   (501) staff       (20)    12590 2020-06-22 02:05:34.000000 pycentroids-0.2.0rc2/python/binding.cpp
--rw-r--r--   0 mrakitin   (501) staff       (20)       29 2020-06-22 02:05:34.000000 pycentroids-0.2.0rc2/requirements.txt
--rw-r--r--   0 mrakitin   (501) staff       (20)      331 2020-06-22 02:07:47.000000 pycentroids-0.2.0rc2/setup.cfg
--rw-r--r--   0 mrakitin   (501) staff       (20)     3852 2020-06-15 15:18:46.000000 pycentroids-0.2.0rc2/setup.py
--rw-r--r--   0 mrakitin   (501) staff       (20)    68611 2020-06-12 20:09:24.000000 pycentroids-0.2.0rc2/versioneer.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2024-04-29 15:47:05.615288 pycentroids-0.2.0rc3/
+-rw-r--r--   0 mrakitin   (501) staff       (20)     1637 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/CMakeLists.txt
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2024-04-29 15:47:05.585117 pycentroids-0.2.0rc3/LICENSE/
+-rw-r--r--   0 mrakitin   (501) staff       (20)     1537 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/LICENSE/LICENSE
+-rw-r--r--   0 mrakitin   (501) staff       (20)     1558 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/LICENSE/LICENSE_LMFIT
+-rw-r--r--   0 mrakitin   (501) staff       (20)      536 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/MANIFEST.in
+-rw-r--r--   0 mrakitin   (501) staff       (20)     1940 2024-04-29 15:47:05.614842 pycentroids-0.2.0rc3/PKG-INFO
+-rw-r--r--   0 mrakitin   (501) staff       (20)     1558 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/README.md
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2024-04-29 15:47:05.587388 pycentroids-0.2.0rc3/cmake/
+-rw-r--r--   0 mrakitin   (501) staff       (20)      288 2020-02-13 19:58:45.000000 pycentroids-0.2.0rc3/cmake/FindSphinx.cmake
+-rw-r--r--   0 mrakitin   (501) staff       (20)      607 2020-02-13 19:58:45.000000 pycentroids-0.2.0rc3/cmake/PreventInSourceBuilds.cmake
+-rw-r--r--   0 mrakitin   (501) staff       (20)     5916 2020-02-13 19:58:45.000000 pycentroids-0.2.0rc3/cmake/cpplint.cmake
+-rw-r--r--   0 mrakitin   (501) staff       (20)     1317 2020-02-13 19:58:45.000000 pycentroids-0.2.0rc3/cmake/version.cmake
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2024-04-29 15:47:05.578470 pycentroids-0.2.0rc3/docs/
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2024-04-29 15:47:05.588469 pycentroids-0.2.0rc3/docs/doxygen/
+-rw-r--r--   0 mrakitin   (501) staff       (20)      696 2020-02-13 19:58:45.000000 pycentroids-0.2.0rc3/docs/doxygen/CMakeLists.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)   110739 2020-02-13 19:58:45.000000 pycentroids-0.2.0rc3/docs/doxygen/Doxyfile.in
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2024-04-29 15:47:05.593277 pycentroids-0.2.0rc3/docs/sphinx/
+-rw-r--r--   0 mrakitin   (501) staff       (20)      712 2020-02-13 19:58:45.000000 pycentroids-0.2.0rc3/docs/sphinx/CMakeLists.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)      339 2020-02-13 19:58:45.000000 pycentroids-0.2.0rc3/docs/sphinx/api.rst
+-rw-r--r--   0 mrakitin   (501) staff       (20)     8087 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/docs/sphinx/conf.py.in
+-rw-r--r--   0 mrakitin   (501) staff       (20)    54289 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/docs/sphinx/first_pass.png
+-rw-r--r--   0 mrakitin   (501) staff       (20)     2142 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/docs/sphinx/first_pass.rst
+-rw-r--r--   0 mrakitin   (501) staff       (20)      505 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/docs/sphinx/index.rst
+-rw-r--r--   0 mrakitin   (501) staff       (20)     5781 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/docs/sphinx/second_pass.rst
+-rw-r--r--   0 mrakitin   (501) staff       (20)      833 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/docs/sphinx/theory.rst
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2024-04-29 15:47:05.596224 pycentroids-0.2.0rc3/lib/
+-rw-r--r--   0 mrakitin   (501) staff       (20)     2746 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/lib/CMakeLists.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)      123 2020-02-13 19:58:45.000000 pycentroids-0.2.0rc3/lib/centroids-config.cmake.in
+-rw-r--r--   0 mrakitin   (501) staff       (20)     5158 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/lib/centroids.h
+-rw-r--r--   0 mrakitin   (501) staff       (20)    35771 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/lib/photons.cpp
+-rw-r--r--   0 mrakitin   (501) staff       (20)     6016 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/lib/photons.h
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2024-04-29 15:47:05.600340 pycentroids-0.2.0rc3/lmfit/
+-rw-r--r--   0 mrakitin   (501) staff       (20)     4745 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/lmfit/lminvert.c
+-rw-r--r--   0 mrakitin   (501) staff       (20)      451 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/lmfit/lminvert.h
+-rw-r--r--   0 mrakitin   (501) staff       (20)    46613 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/lmfit/lmmin.c
+-rw-r--r--   0 mrakitin   (501) staff       (20)     3593 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/lmfit/lmmin.h
+-rw-r--r--   0 mrakitin   (501) staff       (20)     3562 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/lmfit/lmstruct.h
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2024-04-29 15:47:05.617576 pycentroids-0.2.0rc3/pycentroids/
+-rw-r--r--   0 mrakitin   (501) staff       (20)      195 2020-02-13 19:58:45.000000 pycentroids-0.2.0rc3/pycentroids/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)      500 2024-04-29 15:47:05.617766 pycentroids-0.2.0rc3/pycentroids/_version.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     5462 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/pycentroids/pycentroids.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2024-04-29 15:47:05.610582 pycentroids-0.2.0rc3/pycentroids/tests/
+-rw-r--r--   0 mrakitin   (501) staff       (20)        0 2020-02-13 19:58:45.000000 pycentroids-0.2.0rc3/pycentroids/tests/__init__.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)      219 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/pycentroids/tests/test_install.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)     8222 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/pycentroids/tests/test_photons.py
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2024-04-29 15:47:05.613360 pycentroids-0.2.0rc3/pycentroids.egg-info/
+-rw-r--r--   0 mrakitin   (501) staff       (20)     1940 2024-04-29 15:47:05.000000 pycentroids-0.2.0rc3/pycentroids.egg-info/PKG-INFO
+-rw-r--r--   0 mrakitin   (501) staff       (20)     1067 2024-04-29 15:47:05.000000 pycentroids-0.2.0rc3/pycentroids.egg-info/SOURCES.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)        1 2024-04-29 15:47:05.000000 pycentroids-0.2.0rc3/pycentroids.egg-info/dependency_links.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)        1 2024-04-29 15:47:05.000000 pycentroids-0.2.0rc3/pycentroids.egg-info/not-zip-safe
+-rw-r--r--   0 mrakitin   (501) staff       (20)       30 2024-04-29 15:47:05.000000 pycentroids-0.2.0rc3/pycentroids.egg-info/requires.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)       25 2024-04-29 15:47:05.000000 pycentroids-0.2.0rc3/pycentroids.egg-info/top_level.txt
+drwxr-xr-x   0 mrakitin   (501) staff       (20)        0 2024-04-29 15:47:05.612316 pycentroids-0.2.0rc3/python/
+-rw-r--r--   0 mrakitin   (501) staff       (20)      699 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/python/CMakeLists.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)    12590 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/python/binding.cpp
+-rw-r--r--   0 mrakitin   (501) staff       (20)       29 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/requirements.txt
+-rw-r--r--   0 mrakitin   (501) staff       (20)      331 2024-04-29 15:47:05.616860 pycentroids-0.2.0rc3/setup.cfg
+-rw-r--r--   0 mrakitin   (501) staff       (20)     3852 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/setup.py
+-rw-r--r--   0 mrakitin   (501) staff       (20)    68573 2024-04-29 15:35:58.000000 pycentroids-0.2.0rc3/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pycentroids-0.2.0rc2/CMakeLists.txt` & `pycentroids-0.2.0rc3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/LICENSE/LICENSE` & `pycentroids-0.2.0rc3/LICENSE/LICENSE`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/LICENSE/LICENSE_LMFIT` & `pycentroids-0.2.0rc3/LICENSE/LICENSE_LMFIT`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/MANIFEST.in` & `pycentroids-0.2.0rc3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/PKG-INFO` & `pycentroids-0.2.0rc3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 Metadata-Version: 2.1
 Name: pycentroids
-Version: 0.2.0rc2
+Version: 0.2.0rc3
 Summary: Centroiding algorithms for CCD Single Photon Counting
 Home-page: https://github.com/NSLS-II/centroids
 Author: Stuart B. Wilkins
 Author-email: swilkins@bnl.gov
 License: BSD (3-clause)
-Description: # centroids
-        
-        ## Build Status
-        
-        
-        | Build Type | Result |
-        |---|:-----:|
-        | **Python Linux Builds** | [![Build Status](https://dev.azure.com/nsls-ii/centroids/_apis/build/status/NSLS-II.centroids?branchName=master&jobName=BuildPython)](https://dev.azure.com/nsls-ii/centroids/_build/latest?definitionId=3&branchName=master) |
-        | **CXX Lib Linux Builds** | [![Build Status](https://dev.azure.com/nsls-ii/centroids/_apis/build/status/NSLS-II.centroids?branchName=master&jobName=BuildLib)](https://dev.azure.com/nsls-ii/centroids/_build/latest?definitionId=3&branchName=master) |
-        | **Documentation Build** | [![Build Status](https://dev.azure.com/nsls-ii/centroids/_apis/build/status/NSLS-II.centroids?branchName=master&jobName=BuildDocs)](https://dev.azure.com/nsls-ii/centroids/_build/latest?definitionId=3&branchName=master) |
-        
-        ## Introduction
-        
-        Routines for performing single photon counting and centroiding of CCD data
-        
-        ## Documentation
-        
-        The documentation can be found [online](https://nsls-ii.github.io/centroids/).
-        
-        ## Changes
-        
-        ### v0.2.0rc1
-        
-        Release candidate for v0.2.
-        
-        * Changed `MANIFEST.in` to allow for building with `pip`.
-        
-        ### v0.1.11
-        
-        * Fixed bug in standard error for 2D fits calculations. Incorrect number of data points was used.
-        * Added range option to fitting parameters for _sigma_ and _position_
-        * Modified CI to report tests and coverage
-        * Improved unit tests to cover parameter range selection
-        * Added debug output to unit tests
-        * Updated docs
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: cpplint
+Requires-Dist: pybind11
+
+# centroids
+
+## Build Status
+
+
+| Build Type | Result |
+|---|:-----:|
+| **Python Linux Builds** | [![Build Status](https://dev.azure.com/nsls-ii/centroids/_apis/build/status/NSLS-II.centroids?branchName=master&jobName=BuildPython)](https://dev.azure.com/nsls-ii/centroids/_build/latest?definitionId=3&branchName=master) |
+| **CXX Lib Linux Builds** | [![Build Status](https://dev.azure.com/nsls-ii/centroids/_apis/build/status/NSLS-II.centroids?branchName=master&jobName=BuildLib)](https://dev.azure.com/nsls-ii/centroids/_build/latest?definitionId=3&branchName=master) |
+| **Documentation Build** | [![Build Status](https://dev.azure.com/nsls-ii/centroids/_apis/build/status/NSLS-II.centroids?branchName=master&jobName=BuildDocs)](https://dev.azure.com/nsls-ii/centroids/_build/latest?definitionId=3&branchName=master) |
+
+## Introduction
+
+Routines for performing single photon counting and centroiding of CCD data
+
+## Documentation
+
+The documentation can be found [online](https://nsls-ii.github.io/centroids/).
+
+## Changes
+
+### v0.2.0rc2
+
+* Exposed Pixel Lookup Table to python interface
+* Added weights for 1D and 2D Fits
+
+### v0.2.0rc1
+
+Release candidate for v0.2.
+
+* Changed `MANIFEST.in` to allow for building with `pip`.
+
+### v0.1.11
+
+* Fixed bug in standard error for 2D fits calculations. Incorrect number of data points was used.
+* Added range option to fitting parameters for _sigma_ and _position_
+* Modified CI to report tests and coverage
+* Improved unit tests to cover parameter range selection
+* Added debug output to unit tests
+* Updated docs
```

### Comparing `pycentroids-0.2.0rc2/README.md` & `pycentroids-0.2.0rc3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 
 ## Documentation
 
 The documentation can be found [online](https://nsls-ii.github.io/centroids/).
 
 ## Changes
 
+### v0.2.0rc2
+
+* Exposed Pixel Lookup Table to python interface
+* Added weights for 1D and 2D Fits
+
 ### v0.2.0rc1
 
 Release candidate for v0.2.
 
 * Changed `MANIFEST.in` to allow for building with `pip`.
 
 ### v0.1.11
```

### Comparing `pycentroids-0.2.0rc2/cmake/PreventInSourceBuilds.cmake` & `pycentroids-0.2.0rc3/cmake/PreventInSourceBuilds.cmake`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/cmake/cpplint.cmake` & `pycentroids-0.2.0rc3/cmake/cpplint.cmake`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/cmake/version.cmake` & `pycentroids-0.2.0rc3/cmake/version.cmake`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/docs/doxygen/CMakeLists.txt` & `pycentroids-0.2.0rc3/docs/doxygen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/docs/doxygen/Doxyfile.in` & `pycentroids-0.2.0rc3/docs/doxygen/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/docs/sphinx/CMakeLists.txt` & `pycentroids-0.2.0rc3/docs/sphinx/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/docs/sphinx/conf.py.in` & `pycentroids-0.2.0rc3/docs/sphinx/conf.py.in`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/docs/sphinx/first_pass.png` & `pycentroids-0.2.0rc3/docs/sphinx/first_pass.png`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/docs/sphinx/first_pass.rst` & `pycentroids-0.2.0rc3/docs/sphinx/first_pass.rst`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/docs/sphinx/second_pass.rst` & `pycentroids-0.2.0rc3/docs/sphinx/second_pass.rst`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/docs/sphinx/theory.rst` & `pycentroids-0.2.0rc3/docs/sphinx/theory.rst`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/lib/CMakeLists.txt` & `pycentroids-0.2.0rc3/lib/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/lib/centroids.h` & `pycentroids-0.2.0rc3/lib/centroids.h`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/lib/photons.cpp` & `pycentroids-0.2.0rc3/lib/photons.cpp`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/lib/photons.h` & `pycentroids-0.2.0rc3/lib/photons.h`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/lmfit/lminvert.c` & `pycentroids-0.2.0rc3/lmfit/lminvert.c`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/lmfit/lmmin.c` & `pycentroids-0.2.0rc3/lmfit/lmmin.c`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/lmfit/lmmin.h` & `pycentroids-0.2.0rc3/lmfit/lmmin.h`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/lmfit/lmstruct.h` & `pycentroids-0.2.0rc3/lmfit/lmstruct.h`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/pycentroids/pycentroids.py` & `pycentroids-0.2.0rc3/pycentroids/pycentroids.py`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/pycentroids/tests/test_photons.py` & `pycentroids-0.2.0rc3/pycentroids/tests/test_photons.py`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/pycentroids.egg-info/PKG-INFO` & `pycentroids-0.2.0rc3/pycentroids.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 Metadata-Version: 2.1
 Name: pycentroids
-Version: 0.2.0rc2
+Version: 0.2.0rc3
 Summary: Centroiding algorithms for CCD Single Photon Counting
 Home-page: https://github.com/NSLS-II/centroids
 Author: Stuart B. Wilkins
 Author-email: swilkins@bnl.gov
 License: BSD (3-clause)
-Description: # centroids
-        
-        ## Build Status
-        
-        
-        | Build Type | Result |
-        |---|:-----:|
-        | **Python Linux Builds** | [![Build Status](https://dev.azure.com/nsls-ii/centroids/_apis/build/status/NSLS-II.centroids?branchName=master&jobName=BuildPython)](https://dev.azure.com/nsls-ii/centroids/_build/latest?definitionId=3&branchName=master) |
-        | **CXX Lib Linux Builds** | [![Build Status](https://dev.azure.com/nsls-ii/centroids/_apis/build/status/NSLS-II.centroids?branchName=master&jobName=BuildLib)](https://dev.azure.com/nsls-ii/centroids/_build/latest?definitionId=3&branchName=master) |
-        | **Documentation Build** | [![Build Status](https://dev.azure.com/nsls-ii/centroids/_apis/build/status/NSLS-II.centroids?branchName=master&jobName=BuildDocs)](https://dev.azure.com/nsls-ii/centroids/_build/latest?definitionId=3&branchName=master) |
-        
-        ## Introduction
-        
-        Routines for performing single photon counting and centroiding of CCD data
-        
-        ## Documentation
-        
-        The documentation can be found [online](https://nsls-ii.github.io/centroids/).
-        
-        ## Changes
-        
-        ### v0.2.0rc1
-        
-        Release candidate for v0.2.
-        
-        * Changed `MANIFEST.in` to allow for building with `pip`.
-        
-        ### v0.1.11
-        
-        * Fixed bug in standard error for 2D fits calculations. Incorrect number of data points was used.
-        * Added range option to fitting parameters for _sigma_ and _position_
-        * Modified CI to report tests and coverage
-        * Improved unit tests to cover parameter range selection
-        * Added debug output to unit tests
-        * Updated docs
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: cpplint
+Requires-Dist: pybind11
+
+# centroids
+
+## Build Status
+
+
+| Build Type | Result |
+|---|:-----:|
+| **Python Linux Builds** | [![Build Status](https://dev.azure.com/nsls-ii/centroids/_apis/build/status/NSLS-II.centroids?branchName=master&jobName=BuildPython)](https://dev.azure.com/nsls-ii/centroids/_build/latest?definitionId=3&branchName=master) |
+| **CXX Lib Linux Builds** | [![Build Status](https://dev.azure.com/nsls-ii/centroids/_apis/build/status/NSLS-II.centroids?branchName=master&jobName=BuildLib)](https://dev.azure.com/nsls-ii/centroids/_build/latest?definitionId=3&branchName=master) |
+| **Documentation Build** | [![Build Status](https://dev.azure.com/nsls-ii/centroids/_apis/build/status/NSLS-II.centroids?branchName=master&jobName=BuildDocs)](https://dev.azure.com/nsls-ii/centroids/_build/latest?definitionId=3&branchName=master) |
+
+## Introduction
+
+Routines for performing single photon counting and centroiding of CCD data
+
+## Documentation
+
+The documentation can be found [online](https://nsls-ii.github.io/centroids/).
+
+## Changes
+
+### v0.2.0rc2
+
+* Exposed Pixel Lookup Table to python interface
+* Added weights for 1D and 2D Fits
+
+### v0.2.0rc1
+
+Release candidate for v0.2.
+
+* Changed `MANIFEST.in` to allow for building with `pip`.
+
+### v0.1.11
+
+* Fixed bug in standard error for 2D fits calculations. Incorrect number of data points was used.
+* Added range option to fitting parameters for _sigma_ and _position_
+* Modified CI to report tests and coverage
+* Improved unit tests to cover parameter range selection
+* Added debug output to unit tests
+* Updated docs
```

### Comparing `pycentroids-0.2.0rc2/pycentroids.egg-info/SOURCES.txt` & `pycentroids-0.2.0rc3/pycentroids.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/python/CMakeLists.txt` & `pycentroids-0.2.0rc3/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/python/binding.cpp` & `pycentroids-0.2.0rc3/python/binding.cpp`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/setup.py` & `pycentroids-0.2.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `pycentroids-0.2.0rc2/versioneer.py` & `pycentroids-0.2.0rc3/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,17 +335,16 @@
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise EnvironmentError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
     setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
-    with open(setup_cfg, "r") as f:
-        parser.readfp(f)
+    parser = configparser.ConfigParser()
+    parser.read(setup_cfg)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
     cfg = VersioneerConfig()
```

