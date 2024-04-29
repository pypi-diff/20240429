# Comparing `tmp/spinsfast-2022.4.5.tar.gz` & `tmp/spinsfast-2022.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spinsfast-2022.4.5.tar", last modified: Mon Mar 11 12:49:48 2024, max compression
+gzip compressed data, was "spinsfast-2022.4.6.tar", last modified: Mon Apr 29 18:58:23 2024, max compression
```

## Comparing `spinsfast-2022.4.5.tar` & `spinsfast-2022.4.6.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:49:48.910098 spinsfast-2022.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)    35122 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-11 12:49:48.910098 spinsfast-2022.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/README
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:49:48.906098 spinsfast-2022.4.5/code/
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/alm.c
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/dump_cimage.c
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/healpix_convert.c
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/module.mk
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/spinsfast_backward_Gmm.c
--rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/spinsfast_backward_Gmm_alm2iqu.c
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/spinsfast_backward_transform.c
--rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/spinsfast_forward_Imm.c
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/spinsfast_forward_Jmm.c
--rw-r--r--   0 runner    (1001) docker     (127)     6201 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/spinsfast_forward_transform.c
--rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/spinsfast_forward_transform_eo.c
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/spinsfast_forward_transform_from_Imm.c
--rw-r--r--   0 runner    (1001) docker     (127)     9771 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/spinsfast_forward_transform_iqu2alm.c
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/wigner_d_halfpi_Risbo.c
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/wigner_d_halfpi_TN.c
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/code/wigner_d_halfpi_methods.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:49:48.906098 spinsfast-2022.4.5/example/
--rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/example/example_iqu.c
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/example/example_multispin.c
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/example/example_spin.c
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/example/example_spin.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/example/module.mk
--rw-r--r--   0 runner    (1001) docker     (127)  1406131 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/example/spinsfast.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:49:48.910098 spinsfast-2022.4.5/include/
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/include/alm.h
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/include/fftw.h
--rw-r--r--   0 runner    (1001) docker     (127)    31394 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/include/fftw3.h
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/include/healpix_convert.h
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/include/inline.h
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/include/restrict.h
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/include/spinsfast_backward.h
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/include/spinsfast_forward.h
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/include/wigner_d_halfpi.h
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/include/wigner_d_halfpi_Risbo.h
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/include/wigner_d_halfpi_TN.h
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/include/wigner_d_halfpi_methods.h
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-03-11 12:49:40.000000 spinsfast-2022.4.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:49:48.910098 spinsfast-2022.4.5/python/
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-03-11 12:49:40.000000 spinsfast-2022.4.5/python/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1624 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/python/build_macosx_wheels.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2692 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/python/build_manylinux_wheels.sh
--rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/python/cextension.c
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/python/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-11 12:49:39.000000 spinsfast-2022.4.5/python/module.mk
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 12:49:48.910098 spinsfast-2022.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-03-11 12:49:40.000000 spinsfast-2022.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 12:49:48.910098 spinsfast-2022.4.5/spinsfast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-11 12:49:48.000000 spinsfast-2022.4.5/spinsfast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-11 12:49:48.000000 spinsfast-2022.4.5/spinsfast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 12:49:48.000000 spinsfast-2022.4.5/spinsfast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-11 12:49:48.000000 spinsfast-2022.4.5/spinsfast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:58:23.057866 spinsfast-2022.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)    35122 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-29 18:58:23.057866 spinsfast-2022.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/README
+-rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:58:23.049866 spinsfast-2022.4.6/code/
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/alm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/dump_cimage.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/healpix_convert.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/module.mk
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/spinsfast_backward_Gmm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6398 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/spinsfast_backward_Gmm_alm2iqu.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/spinsfast_backward_transform.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12218 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/spinsfast_forward_Imm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/spinsfast_forward_Jmm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6201 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/spinsfast_forward_transform.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/spinsfast_forward_transform_eo.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/spinsfast_forward_transform_from_Imm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9771 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/spinsfast_forward_transform_iqu2alm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/wigner_d_halfpi_Risbo.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/wigner_d_halfpi_TN.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/code/wigner_d_halfpi_methods.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:58:23.049866 spinsfast-2022.4.6/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/example/example_iqu.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/example/example_multispin.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/example/example_spin.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/example/example_spin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/example/module.mk
+-rw-r--r--   0 runner    (1001) docker     (127)  1406131 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/example/spinsfast.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:58:23.053866 spinsfast-2022.4.6/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/include/alm.h
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/include/fftw.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31394 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/include/fftw3.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/include/healpix_convert.h
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/include/inline.h
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/include/restrict.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/include/spinsfast_backward.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/include/spinsfast_forward.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/include/wigner_d_halfpi.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/include/wigner_d_halfpi_Risbo.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/include/wigner_d_halfpi_TN.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/include/wigner_d_halfpi_methods.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-29 18:58:19.000000 spinsfast-2022.4.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:58:23.053866 spinsfast-2022.4.6/python/
+-rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-04-29 18:58:19.000000 spinsfast-2022.4.6/python/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1624 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/python/build_macosx_wheels.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2692 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/python/build_manylinux_wheels.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     9311 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/python/cextension.c
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/python/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-29 18:58:18.000000 spinsfast-2022.4.6/python/module.mk
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 18:58:23.057866 spinsfast-2022.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-29 18:58:19.000000 spinsfast-2022.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:58:23.053866 spinsfast-2022.4.6/spinsfast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-29 18:58:22.000000 spinsfast-2022.4.6/spinsfast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-29 18:58:23.000000 spinsfast-2022.4.6/spinsfast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:58:22.000000 spinsfast-2022.4.6/spinsfast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 18:58:22.000000 spinsfast-2022.4.6/spinsfast.egg-info/top_level.txt
```

### Comparing `spinsfast-2022.4.5/COPYING` & `spinsfast-2022.4.6/COPYING`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/LICENSE` & `spinsfast-2022.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/Makefile` & `spinsfast-2022.4.6/Makefile`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/PKG-INFO` & `spinsfast-2022.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: spinsfast
-Version: 2022.4.5
+Version: 2022.4.6
 Summary: Fast and exact spin-s spherical-harmonic transforms
 Home-page: https://github.com/moble/spinsfast
 Maintainer: Mike Boyle
 Maintainer-email: mob22@cornell.edu
 License: UNKNOWN
 Description: This module is a lightly modified version of the code originally written by Huffenberger and
         Wandelt.  It enables the user to transform between modes of a spin-weighted spherical-harmonic
```

### Comparing `spinsfast-2022.4.5/README` & `spinsfast-2022.4.6/README`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/spinsfast.svg)](https://anaconda.org/conda-forge/spinsfast)
 [![GPL-3.0 License](https://img.shields.io/github/license/moble/spinsfast.svg)](https://github.com/moble/spinsfast/blob/main/LICENSE)
 [![DOI](https://zenodo.org/badge/30340582.svg)](https://zenodo.org/badge/latestdoi/30340582)
 
 # spinsfast
 Fast and exact spin-s spherical-harmonic transforms
 
-This code is a lightly modified version of the code hosted
+This code is a modified version of the code hosted
 [here](http://astrophysics.physics.fsu.edu/~huffenbe/research/spinsfast/index.html)
-by Huffenberger, based on work by
-[Huffenberger and Wandelt](http://stacks.iop.org/0067-0049/189/255).
+by Huffenberger, based on work by [Huffenberger and
+Wandelt](http://stacks.iop.org/0067-0049/189/255).
 
-My modifications mostly deal with the user interface:
+My (@moble's) modifications mostly deal with the user interface:
 
   * add `multi_map2salm` and `multi_salm2map` for running many similar transformations efficiently;
   * create python wrappers for the `map2salm` and `salm2map` functions to deal with any (reasonable)
     type or shape of input data, including multi-dimensional;
   * add python 3.x compatibility to `python/spinsfast_module.c`;
   * fix segfaults due to use of `free` instead of `fftw_free` when `fftw_malloc` was used;
   * make it easier to install as a python module by trying to detect paths to
@@ -28,36 +28,39 @@
     ([see below](#installation));
   * add integration with [conda](https://conda.io/docs/)
     and [anaconda.org](https://anaconda.org/moble/spinsfast), for easiest installation
     ([see below](#installation)).
 
 # License
 
-The original work is licensed under GPL, so that's what I have to license this
-under as well.  (I usually go for the more liberal MIT license, but GPL is
-fine.)  See the `LICENSE` file in this directory for more details.
-
-I based my work on Huffenberger and Wandelt's "Revision 104, 13 Apr 2012",
-which is current as of this writing (August 2015).  Whenever I notice updates
-on their end, I will gladly update this code, so feel free to open an
-[issue](https://github.com/moble/spinsfast/issues) to notify me.  To see more
-specifically what I've added, look through the
-[commits](https://github.com/moble/spinsfast/commits/master); my contributions
-are just everything since the initial commit.
+The original work is licensed under GPL, so that's what I have to
+license this under as well.  (I usually go for the more liberal MIT
+license, but GPL is fine.)  See the `LICENSE` file in this directory
+for more details.
+
+I based my work on Huffenberger and Wandelt's "Revision 104, 13 Apr
+2012", which is current as of this writing (August 2015).  Whenever I
+notice updates on their end, I will gladly update this code, so feel
+free to open an [issue](https://github.com/moble/spinsfast/issues) to
+notify me.  To see more specifically what I've added, look through the
+[commits](https://github.com/moble/spinsfast/commits/master); my
+contributions are just everything since the initial commit.
 
 
 # Example Usage
 
-A convenient ipython/jupyter notebook is found in the `example` directory, and
-can also be
-[viewed directly online](http://nbviewer.ipython.org/github/moble/spinsfast/blob/master/example/spinsfast.ipynb).
-It shows some example python code that can be used to run this module, and
-explains some of the conventions established by the `spinsfast` authors.
+A convenient ipython/jupyter notebook is found in the `example`
+directory, and can also be [viewed directly
+online](http://nbviewer.ipython.org/github/moble/spinsfast/blob/master/example/spinsfast.ipynb).
+It shows some example python code that can be used to run this module,
+and explains some of the conventions established by the `spinsfast`
+authors.
 
-In the interests of a very short, explicit example, here is one using random `(ell,m)` modes:
+In the interests of a very short, explicit example, here is one using
+random `(ell,m)` modes:
 
 ```python
 from numpy.random import normal, seed
 import spinsfast
 
 # Some boilerplate for setting things up:
 s = 1  # spin weight of the field
@@ -79,23 +82,25 @@
 ```
 
 
 # Installation
 
 ## Anaconda
 
-Though manual installation is possible, the best way by far to satisfy these
-dependencies is to use the [`anaconda`](http://continuum.io/downloads)
-distribution.  This distribution can co-exist with your system python with no
-trouble -- you simply add the path to anaconda before your system executables.
-It installs into your home directory, so it doesn't require root access.  It
-can be uninstalled easily, since it exists entirely inside its own directory.
-And updates are trivial.
+Though manual installation is possible, the best way by far to satisfy
+these dependencies is to use the
+[`anaconda`](http://continuum.io/downloads) distribution.  This
+distribution can co-exist with your system python with no trouble --
+you simply add the path to anaconda before your system executables.
+It installs into your home directory, so it doesn't require root
+access.  It can be uninstalled easily, since it exists entirely inside
+its own directory.  And updates are trivial.
 
-Once `anaconda` is installed, this package may be installed with the command
+Once `anaconda` is installed, this package may be installed with the
+command
 
 ```bash
 conda install --channel conda-forge spinsfast
 ```
 
 Note this may also install `numpy` and `fftw` automatically.
 
@@ -104,64 +109,74 @@
 
 While generally less robust, this package is also available via `pip`:
 
 ```bash
 python -m pip install spinsfast
 ```
 
-Unfortunately, maintaining binary distributions on pip is very complicated, so `pip` may try to
-compile the source code for you, in which case you will need to have FFTW and a compiler installed.
-But `pip` has no good way of handling these dependencies.  See below for environment variables you
-may need to set to get compilation working properly.
-
-It may be helpful to install `pyfftw` first.  Or, on MacOS, you may have better luck installing FFTW
-via homebrew and adding flags like `CFLAGS=" -L/opt/homebrew/lib " python -m pip install spinsfast`.
+Unfortunately, maintaining binary distributions on pip is very
+complicated, so `pip` may try to compile the source code for you, in
+which case you will need to have FFTW and a compiler installed.  But
+`pip` has no good way of handling these dependencies.  See below for
+environment variables you may need to set to get compilation working
+properly.
+
+It may be helpful to install `pyfftw` first.  Or, on MacOS, you may
+have better luck installing FFTW via homebrew and adding flags like
+`CFLAGS=" -L/opt/homebrew/lib " python -m pip install spinsfast`.
 
 
 ## Manual installation
 
-Manual installation of this package is slightly more delicate.  The [FFTW
-package](http://www.fftw.org/) must be installed first.  This is usually very simple.  But the
-resulting header and library must be found by the compilation step for this package.  You can first
-simply try to run
+Manual installation of this package is slightly more delicate.  The
+[FFTW package](http://www.fftw.org/) must be installed first.  This is
+usually very simple.  But the resulting header and library must be
+found by the compilation step for this package.  You can first simply
+try to run
 
 ```bash
 python -m pip install .
 ```
 
-from the top directory of the `spinsfast` code.  This attempts to find the `fftw` header or library
-for you, using some common defaults checked by code in `setup.py`.
-
-If this doesn't work, you can read the error message, but the most likely problem is that the
-compiler cannot find the `fftw` header, or the linker cannot find the `fftw` library.  To solve
-these problems, you will need to run something more like this:
+from the top directory of the `spinsfast` code.  This attempts to find
+the `fftw` header or library for you, using some common defaults
+checked by code in `setup.py`.
+
+If this doesn't work, you can read the error message, but the most
+likely problem is that the compiler cannot find the `fftw` header, or
+the linker cannot find the `fftw` library.  To solve these problems,
+you will need to run something more like this:
 
 ```bash
 export LIBRARY_PATH=/path/to/fftw/lib
 export C_INCLUDE_PATH=/path/to/fftw/include
 python -m pip install .
 ```
 
-Alternatively, you could try to alter `setup.py` to point to the right paths.
+Alternatively, you could try to alter `setup.py` to point to the right
+paths.
 
 
 # Original installation instructions
 
-Though these are not necessary for installing the python module, the following
-are the instructions in the original source code for building the C code.
+Though these are not necessary for installing the python module, the
+following are the instructions in the original source code for
+building the C code.
 
 Get the latest version at:
 
     http://www.physics.miami.edu/~huffenbe/research/spinsfast/
 
 ## Compilation instructions
 
-  1. Edit the file (or make a new file) called build/config.mk so that the proper locations for header and library files are included.
+  1. Edit the file (or make a new file) called build/config.mk so that
+     the proper locations for header and library files are included.
 
-  2. Set the environment variable "build" so that it points to that file. I.e., in bash, say
+  2. Set the environment variable "build" so that it points to that
+     file. I.e., in bash, say
 
         export build=build/config.mk 
 
   3. Build the library and example codes with 
 
         make
```

### Comparing `spinsfast-2022.4.5/README.md` & `spinsfast-2022.4.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/spinsfast.svg)](https://anaconda.org/conda-forge/spinsfast)
 [![GPL-3.0 License](https://img.shields.io/github/license/moble/spinsfast.svg)](https://github.com/moble/spinsfast/blob/main/LICENSE)
 [![DOI](https://zenodo.org/badge/30340582.svg)](https://zenodo.org/badge/latestdoi/30340582)
 
 # spinsfast
 Fast and exact spin-s spherical-harmonic transforms
 
-This code is a lightly modified version of the code hosted
+This code is a modified version of the code hosted
 [here](http://astrophysics.physics.fsu.edu/~huffenbe/research/spinsfast/index.html)
-by Huffenberger, based on work by
-[Huffenberger and Wandelt](http://stacks.iop.org/0067-0049/189/255).
+by Huffenberger, based on work by [Huffenberger and
+Wandelt](http://stacks.iop.org/0067-0049/189/255).
 
-My modifications mostly deal with the user interface:
+My (@moble's) modifications mostly deal with the user interface:
 
   * add `multi_map2salm` and `multi_salm2map` for running many similar transformations efficiently;
   * create python wrappers for the `map2salm` and `salm2map` functions to deal with any (reasonable)
     type or shape of input data, including multi-dimensional;
   * add python 3.x compatibility to `python/spinsfast_module.c`;
   * fix segfaults due to use of `free` instead of `fftw_free` when `fftw_malloc` was used;
   * make it easier to install as a python module by trying to detect paths to
@@ -28,36 +28,39 @@
     ([see below](#installation));
   * add integration with [conda](https://conda.io/docs/)
     and [anaconda.org](https://anaconda.org/moble/spinsfast), for easiest installation
     ([see below](#installation)).
 
 # License
 
-The original work is licensed under GPL, so that's what I have to license this
-under as well.  (I usually go for the more liberal MIT license, but GPL is
-fine.)  See the `LICENSE` file in this directory for more details.
-
-I based my work on Huffenberger and Wandelt's "Revision 104, 13 Apr 2012",
-which is current as of this writing (August 2015).  Whenever I notice updates
-on their end, I will gladly update this code, so feel free to open an
-[issue](https://github.com/moble/spinsfast/issues) to notify me.  To see more
-specifically what I've added, look through the
-[commits](https://github.com/moble/spinsfast/commits/master); my contributions
-are just everything since the initial commit.
+The original work is licensed under GPL, so that's what I have to
+license this under as well.  (I usually go for the more liberal MIT
+license, but GPL is fine.)  See the `LICENSE` file in this directory
+for more details.
+
+I based my work on Huffenberger and Wandelt's "Revision 104, 13 Apr
+2012", which is current as of this writing (August 2015).  Whenever I
+notice updates on their end, I will gladly update this code, so feel
+free to open an [issue](https://github.com/moble/spinsfast/issues) to
+notify me.  To see more specifically what I've added, look through the
+[commits](https://github.com/moble/spinsfast/commits/master); my
+contributions are just everything since the initial commit.
 
 
 # Example Usage
 
-A convenient ipython/jupyter notebook is found in the `example` directory, and
-can also be
-[viewed directly online](http://nbviewer.ipython.org/github/moble/spinsfast/blob/master/example/spinsfast.ipynb).
-It shows some example python code that can be used to run this module, and
-explains some of the conventions established by the `spinsfast` authors.
+A convenient ipython/jupyter notebook is found in the `example`
+directory, and can also be [viewed directly
+online](http://nbviewer.ipython.org/github/moble/spinsfast/blob/master/example/spinsfast.ipynb).
+It shows some example python code that can be used to run this module,
+and explains some of the conventions established by the `spinsfast`
+authors.
 
-In the interests of a very short, explicit example, here is one using random `(ell,m)` modes:
+In the interests of a very short, explicit example, here is one using
+random `(ell,m)` modes:
 
 ```python
 from numpy.random import normal, seed
 import spinsfast
 
 # Some boilerplate for setting things up:
 s = 1  # spin weight of the field
@@ -79,23 +82,25 @@
 ```
 
 
 # Installation
 
 ## Anaconda
 
-Though manual installation is possible, the best way by far to satisfy these
-dependencies is to use the [`anaconda`](http://continuum.io/downloads)
-distribution.  This distribution can co-exist with your system python with no
-trouble -- you simply add the path to anaconda before your system executables.
-It installs into your home directory, so it doesn't require root access.  It
-can be uninstalled easily, since it exists entirely inside its own directory.
-And updates are trivial.
+Though manual installation is possible, the best way by far to satisfy
+these dependencies is to use the
+[`anaconda`](http://continuum.io/downloads) distribution.  This
+distribution can co-exist with your system python with no trouble --
+you simply add the path to anaconda before your system executables.
+It installs into your home directory, so it doesn't require root
+access.  It can be uninstalled easily, since it exists entirely inside
+its own directory.  And updates are trivial.
 
-Once `anaconda` is installed, this package may be installed with the command
+Once `anaconda` is installed, this package may be installed with the
+command
 
 ```bash
 conda install --channel conda-forge spinsfast
 ```
 
 Note this may also install `numpy` and `fftw` automatically.
 
@@ -104,64 +109,74 @@
 
 While generally less robust, this package is also available via `pip`:
 
 ```bash
 python -m pip install spinsfast
 ```
 
-Unfortunately, maintaining binary distributions on pip is very complicated, so `pip` may try to
-compile the source code for you, in which case you will need to have FFTW and a compiler installed.
-But `pip` has no good way of handling these dependencies.  See below for environment variables you
-may need to set to get compilation working properly.
-
-It may be helpful to install `pyfftw` first.  Or, on MacOS, you may have better luck installing FFTW
-via homebrew and adding flags like `CFLAGS=" -L/opt/homebrew/lib " python -m pip install spinsfast`.
+Unfortunately, maintaining binary distributions on pip is very
+complicated, so `pip` may try to compile the source code for you, in
+which case you will need to have FFTW and a compiler installed.  But
+`pip` has no good way of handling these dependencies.  See below for
+environment variables you may need to set to get compilation working
+properly.
+
+It may be helpful to install `pyfftw` first.  Or, on MacOS, you may
+have better luck installing FFTW via homebrew and adding flags like
+`CFLAGS=" -L/opt/homebrew/lib " python -m pip install spinsfast`.
 
 
 ## Manual installation
 
-Manual installation of this package is slightly more delicate.  The [FFTW
-package](http://www.fftw.org/) must be installed first.  This is usually very simple.  But the
-resulting header and library must be found by the compilation step for this package.  You can first
-simply try to run
+Manual installation of this package is slightly more delicate.  The
+[FFTW package](http://www.fftw.org/) must be installed first.  This is
+usually very simple.  But the resulting header and library must be
+found by the compilation step for this package.  You can first simply
+try to run
 
 ```bash
 python -m pip install .
 ```
 
-from the top directory of the `spinsfast` code.  This attempts to find the `fftw` header or library
-for you, using some common defaults checked by code in `setup.py`.
-
-If this doesn't work, you can read the error message, but the most likely problem is that the
-compiler cannot find the `fftw` header, or the linker cannot find the `fftw` library.  To solve
-these problems, you will need to run something more like this:
+from the top directory of the `spinsfast` code.  This attempts to find
+the `fftw` header or library for you, using some common defaults
+checked by code in `setup.py`.
+
+If this doesn't work, you can read the error message, but the most
+likely problem is that the compiler cannot find the `fftw` header, or
+the linker cannot find the `fftw` library.  To solve these problems,
+you will need to run something more like this:
 
 ```bash
 export LIBRARY_PATH=/path/to/fftw/lib
 export C_INCLUDE_PATH=/path/to/fftw/include
 python -m pip install .
 ```
 
-Alternatively, you could try to alter `setup.py` to point to the right paths.
+Alternatively, you could try to alter `setup.py` to point to the right
+paths.
 
 
 # Original installation instructions
 
-Though these are not necessary for installing the python module, the following
-are the instructions in the original source code for building the C code.
+Though these are not necessary for installing the python module, the
+following are the instructions in the original source code for
+building the C code.
 
 Get the latest version at:
 
     http://www.physics.miami.edu/~huffenbe/research/spinsfast/
 
 ## Compilation instructions
 
-  1. Edit the file (or make a new file) called build/config.mk so that the proper locations for header and library files are included.
+  1. Edit the file (or make a new file) called build/config.mk so that
+     the proper locations for header and library files are included.
 
-  2. Set the environment variable "build" so that it points to that file. I.e., in bash, say
+  2. Set the environment variable "build" so that it points to that
+     file. I.e., in bash, say
 
         export build=build/config.mk 
 
   3. Build the library and example codes with 
 
         make
```

### Comparing `spinsfast-2022.4.5/code/alm.c` & `spinsfast-2022.4.6/code/alm.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/code/dump_cimage.c` & `spinsfast-2022.4.6/code/dump_cimage.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/code/healpix_convert.c` & `spinsfast-2022.4.6/code/healpix_convert.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/code/module.mk` & `spinsfast-2022.4.6/code/module.mk`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/code/spinsfast_backward_Gmm.c` & `spinsfast-2022.4.6/code/spinsfast_backward_Gmm.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/code/spinsfast_backward_Gmm_alm2iqu.c` & `spinsfast-2022.4.6/code/spinsfast_backward_Gmm_alm2iqu.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/code/spinsfast_backward_transform.c` & `spinsfast-2022.4.6/code/spinsfast_backward_transform.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/code/spinsfast_forward_Imm.c` & `spinsfast-2022.4.6/code/spinsfast_forward_Imm.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/code/spinsfast_forward_Jmm.c` & `spinsfast-2022.4.6/code/spinsfast_forward_Jmm.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/code/spinsfast_forward_transform.c` & `spinsfast-2022.4.6/code/spinsfast_forward_transform.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/code/spinsfast_forward_transform_eo.c` & `spinsfast-2022.4.6/code/spinsfast_forward_transform_eo.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/code/spinsfast_forward_transform_from_Imm.c` & `spinsfast-2022.4.6/code/spinsfast_forward_transform_from_Imm.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/code/spinsfast_forward_transform_iqu2alm.c` & `spinsfast-2022.4.6/code/spinsfast_forward_transform_iqu2alm.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/code/wigner_d_halfpi_Risbo.c` & `spinsfast-2022.4.6/code/wigner_d_halfpi_Risbo.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/code/wigner_d_halfpi_TN.c` & `spinsfast-2022.4.6/code/wigner_d_halfpi_TN.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/code/wigner_d_halfpi_methods.c` & `spinsfast-2022.4.6/code/wigner_d_halfpi_methods.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/example/example_iqu.c` & `spinsfast-2022.4.6/example/example_iqu.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/example/example_multispin.c` & `spinsfast-2022.4.6/example/example_multispin.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/example/example_spin.c` & `spinsfast-2022.4.6/example/example_spin.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/example/example_spin.py` & `spinsfast-2022.4.6/example/example_spin.py`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/example/spinsfast.ipynb` & `spinsfast-2022.4.6/example/spinsfast.ipynb`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/include/alm.h` & `spinsfast-2022.4.6/include/alm.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/include/fftw3.h` & `spinsfast-2022.4.6/include/fftw3.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/include/healpix_convert.h` & `spinsfast-2022.4.6/include/healpix_convert.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/include/spinsfast_backward.h` & `spinsfast-2022.4.6/include/spinsfast_backward.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/include/spinsfast_forward.h` & `spinsfast-2022.4.6/include/spinsfast_forward.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/include/wigner_d_halfpi.h` & `spinsfast-2022.4.6/include/wigner_d_halfpi.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/include/wigner_d_halfpi_Risbo.h` & `spinsfast-2022.4.6/include/wigner_d_halfpi_Risbo.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/include/wigner_d_halfpi_TN.h` & `spinsfast-2022.4.6/include/wigner_d_halfpi_TN.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/include/wigner_d_halfpi_methods.h` & `spinsfast-2022.4.6/include/wigner_d_halfpi_methods.h`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/pyproject.toml` & `spinsfast-2022.4.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [tool.poetry]
 name = "spinsfast"
-version = "2022.4.5"
+version = "2022.4.6"
 description = "Fast and exact spin-s spherical-harmonic transforms"
 readme = "README.md"
 license = "GPL-3.0-only"
 authors = ["Michael Boyle <mob22@cornell.edu>"]
 homepage = "https://github.com/moble/spinsfast"
 
 [tool.cibuildwheel]
 # See pyfftw for a good example: https://github.com/pyFFTW/pyFFTW/blob/master/.github/workflows/wheel_tests_and_release.yml
+# See also numpy: https://github.com/numpy/numpy/blob/main/pyproject.toml#L137
+# And scipy: https://github.com/scipy/scipy/blob/main/pyproject.toml#L123
 # SciPy and NumPy don't support musllinux
 # SciPy and NumPy don't support 32-bit Linux from Python 3.10 and onwards
 # Numpy only supports pypy38 x86_64 on Linux
 #skip = "cp36-* cp37-* pp37-* pp38-*i686 pp38-macos* pp39-* *musl* *-win*"
-skip = "*p36-* *p37-* pp38-*i686 pp39-* pp310-* *musl* *-win* cp310-manylinux_i686 cp311-manylinux_i686 cp312-manylinux_i686"
+#skip = "cp36-* cp37-* cp-38* pp37-* *-manylinux_i686 *_ppc64le *_s390x *_universal2"
+#skip = "cp36-* cp37-* cp38-* pp* *_ppc64le *_i686 *_s390x"
+skip = "cp36-* cp37-* cp-38* pp3* *musl* *-win* *-manylinux_i686 *_ppc64le *_s390x *_universal2"
 # before-build = "python -m pip install --no-cache-dir --force-reinstall oldest-supported-numpy"
 
 [tool.cibuildwheel.environment]
 # this makes sure that we build only on platforms that have a corresponding numpy wheel
 PIP_ONLY_BINARY = ":all:"
 
 [tool.cibuildwheel.macos]
```

### Comparing `spinsfast-2022.4.5/python/__init__.py` & `spinsfast-2022.4.6/python/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 """
 
 from __future__ import absolute_import
 
 # NOTE: Don't change the following line; it is modified automatically in the
 # github actions build step, based on the version given in pyproject.toml
-__version__ = "2022.4.5"
+__version__ = "2022.4.6"
 
 # explicitly import functions with underscores (which will be wrapped)
 from .cextension import (
     N_lm, _ind_lm, _lm_ind,
     _salm2map, _multi_salm2map, _map2salm, _multi_map2salm,
     _f_extend_MW, _f_extend_old, _Imm, _quadrature_weights
 )
```

### Comparing `spinsfast-2022.4.5/python/build_macosx_wheels.sh` & `spinsfast-2022.4.6/python/build_macosx_wheels.sh`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/python/build_manylinux_wheels.sh` & `spinsfast-2022.4.6/python/build_manylinux_wheels.sh`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/python/cextension.c` & `spinsfast-2022.4.6/python/cextension.c`

 * *Files identical despite different names*

### Comparing `spinsfast-2022.4.5/setup.py` & `spinsfast-2022.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os.path import isdir, join, dirname, realpath
 from setuptools import setup, Extension
 from distutils.sysconfig import get_python_lib
 
 
 # NOTE: Don't change the following line; it is modified automatically in the
 # github actions build step, based on the version given in pyproject.toml
-version = "2022.4.5"
+version = "2022.4.6"
 
 try:
     import numpy
     numpy_inc = numpy.get_include()
 except:
     numpy_inc = os.path.join(get_python_lib(plat_specific=1), 'numpy', 'core', 'include')
```

### Comparing `spinsfast-2022.4.5/spinsfast.egg-info/PKG-INFO` & `spinsfast-2022.4.6/spinsfast.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: spinsfast
-Version: 2022.4.5
+Version: 2022.4.6
 Summary: Fast and exact spin-s spherical-harmonic transforms
 Home-page: https://github.com/moble/spinsfast
 Maintainer: Mike Boyle
 Maintainer-email: mob22@cornell.edu
 License: UNKNOWN
 Description: This module is a lightly modified version of the code originally written by Huffenberger and
         Wandelt.  It enables the user to transform between modes of a spin-weighted spherical-harmonic
```

### Comparing `spinsfast-2022.4.5/spinsfast.egg-info/SOURCES.txt` & `spinsfast-2022.4.6/spinsfast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

