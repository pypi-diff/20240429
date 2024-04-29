# Comparing `tmp/opinf-0.5.1.tar.gz` & `tmp/opinf-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opinf-0.5.1.tar", last modified: Wed Jan 24 16:55:00 2024, max compression
+gzip compressed data, was "opinf-0.5.2.tar", last modified: Mon Apr 29 19:25:13 2024, max compression
```

## Comparing `opinf-0.5.1.tar` & `opinf-0.5.2.tar`

### file list

```diff
@@ -1,66 +1,72 @@
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.065600 opinf-0.5.1/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1079 2023-10-10 16:21:43.000000 opinf-0.5.1/LICENSE
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     4929 2024-01-24 16:55:00.065149 opinf-0.5.1/PKG-INFO
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1800 2023-10-10 16:21:43.000000 opinf-0.5.1/README.md
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1884 2024-01-24 16:53:31.000000 opinf-0.5.1/pyproject.toml
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       38 2024-01-24 16:55:00.065651 opinf-0.5.1/setup.cfg
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      161 2023-10-10 16:21:43.000000 opinf-0.5.1/setup.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.025969 opinf-0.5.1/src/
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.033276 opinf-0.5.1/src/opinf/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      394 2024-01-24 16:53:26.000000 opinf-0.5.1/src/opinf/__init__.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.048683 opinf-0.5.1/src/opinf/basis/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      105 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/basis/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     4577 2023-12-01 18:52:21.000000 opinf-0.5.1/src/opinf/basis/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    13111 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/basis/_linear.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    36457 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/basis/_pod.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.050280 opinf-0.5.1/src/opinf/ddt/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       99 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/ddt/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7766 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/ddt/_finite_difference.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      557 2024-01-24 16:53:26.000000 opinf-0.5.1/src/opinf/errors.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.052322 opinf-0.5.1/src/opinf/lift/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      134 2024-01-24 16:53:26.000000 opinf-0.5.1/src/opinf/lift/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5011 2024-01-24 16:53:26.000000 opinf-0.5.1/src/opinf/lift/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5660 2024-01-24 16:53:26.000000 opinf-0.5.1/src/opinf/lift/_polynomial.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.053996 opinf-0.5.1/src/opinf/lstsq/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     2764 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/lstsq/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7622 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/lstsq/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    18912 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/lstsq/_tikhonov.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      936 2023-12-01 18:52:21.000000 opinf-0.5.1/src/opinf/lstsq/_total.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.054503 opinf-0.5.1/src/opinf/models/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      142 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/models/__init__.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.056002 opinf-0.5.1/src/opinf/models/mono/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      183 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/models/mono/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    12644 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/models/mono/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    42164 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/models/mono/_nonparametric.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    55664 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/models/mono/_parametric.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.057502 opinf-0.5.1/src/opinf/models/multi/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      185 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/models/multi/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      106 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/models/multi/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      105 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/models/multi/_nonparametric.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       99 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/models/multi/_parametric.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.059056 opinf-0.5.1/src/opinf/operators/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      178 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/operators/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    22795 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/operators/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    35035 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/operators/_interpolate.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    51328 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/operators/_nonparametric.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.059790 opinf-0.5.1/src/opinf/post/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      111 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/post/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7005 2023-12-01 18:52:21.000000 opinf-0.5.1/src/opinf/post/_errors.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.060971 opinf-0.5.1/src/opinf/pre/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      112 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/pre/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7381 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/pre/_base.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    36339 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/pre/_shiftscale.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.062263 opinf-0.5.1/src/opinf/roms/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      168 2024-01-12 21:51:13.000000 opinf-0.5.1/src/opinf/roms/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3734 2024-01-13 00:03:24.000000 opinf-0.5.1/src/opinf/roms/_nonparametric.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       52 2024-01-12 21:52:14.000000 opinf-0.5.1/src/opinf/roms/_parametric.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.063431 opinf-0.5.1/src/opinf/utils/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       69 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/utils/__init__.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     4011 2023-12-18 16:40:20.000000 opinf-0.5.1/src/opinf/utils/_hdf5.py
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3856 2023-12-01 18:52:21.000000 opinf-0.5.1/src/opinf/utils/_reprojection.py
-drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-01-24 16:55:00.064230 opinf-0.5.1/src/opinf.egg-info/
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     4929 2024-01-24 16:55:00.000000 opinf-0.5.1/src/opinf.egg-info/PKG-INFO
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1361 2024-01-24 16:55:00.000000 opinf-0.5.1/src/opinf.egg-info/SOURCES.txt
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        1 2024-01-24 16:55:00.000000 opinf-0.5.1/src/opinf.egg-info/dependency_links.txt
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      311 2024-01-24 16:55:00.000000 opinf-0.5.1/src/opinf.egg-info/requires.txt
--rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        6 2024-01-24 16:55:00.000000 opinf-0.5.1/src/opinf.egg-info/top_level.txt
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.548803 opinf-0.5.2/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1079 2023-10-10 16:21:43.000000 opinf-0.5.2/LICENSE
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5032 2024-04-29 19:25:13.548303 opinf-0.5.2/PKG-INFO
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1800 2023-10-10 16:21:43.000000 opinf-0.5.2/README.md
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1937 2024-04-29 19:15:32.000000 opinf-0.5.2/pyproject.toml
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       38 2024-04-29 19:25:13.548852 opinf-0.5.2/setup.cfg
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      161 2023-10-10 16:21:43.000000 opinf-0.5.2/setup.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.506054 opinf-0.5.2/src/
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.510612 opinf-0.5.2/src/opinf/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      394 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/__init__.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.515875 opinf-0.5.2/src/opinf/basis/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      148 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/basis/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     9891 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/basis/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    10006 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/basis/_linear.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    20882 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/basis/_multi.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    42659 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/basis/_pod.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.517420 opinf-0.5.2/src/opinf/ddt/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       99 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/ddt/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7766 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/ddt/_finite_difference.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      565 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/errors.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.519588 opinf-0.5.2/src/opinf/lift/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      134 2024-02-05 19:42:33.000000 opinf-0.5.2/src/opinf/lift/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5092 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/lift/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5660 2024-01-24 16:53:26.000000 opinf-0.5.2/src/opinf/lift/_polynomial.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.524587 opinf-0.5.2/src/opinf/lstsq/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     2764 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/lstsq/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7622 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/lstsq/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    18912 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/lstsq/_tikhonov.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      936 2023-12-01 18:52:21.000000 opinf-0.5.2/src/opinf/lstsq/_total.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.525257 opinf-0.5.2/src/opinf/models/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      142 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/__init__.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.527552 opinf-0.5.2/src/opinf/models/mono/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      183 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/mono/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    12644 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/mono/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    42164 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/mono/_nonparametric.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    55664 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/mono/_parametric.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.530203 opinf-0.5.2/src/opinf/models/multi/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      185 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/multi/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      106 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/multi/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      105 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/multi/_nonparametric.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       99 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/models/multi/_parametric.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.533974 opinf-0.5.2/src/opinf/operators/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      178 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/operators/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    22275 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/operators/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    35032 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/operators/_interpolate.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    51458 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/operators/_nonparametric.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.537141 opinf-0.5.2/src/opinf/post/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      111 2023-12-18 16:40:20.000000 opinf-0.5.2/src/opinf/post/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     7938 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/post/_errors.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.540806 opinf-0.5.2/src/opinf/pre/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      155 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/pre/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    11547 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/pre/_base.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    18031 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/pre/_multi.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)    27382 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/pre/_shiftscale.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.542135 opinf-0.5.2/src/opinf/roms/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      168 2024-01-12 21:51:13.000000 opinf-0.5.2/src/opinf/roms/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3734 2024-01-13 00:03:24.000000 opinf-0.5.2/src/opinf/roms/_nonparametric.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)       52 2024-01-12 21:52:14.000000 opinf-0.5.2/src/opinf/roms/_parametric.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.546136 opinf-0.5.2/src/opinf/utils/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      178 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/utils/__init__.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     4070 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/utils/_hdf5.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      784 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/utils/_mpl_config.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      355 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/utils/_repr.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3856 2023-12-01 18:52:21.000000 opinf-0.5.2/src/opinf/utils/_reprojection.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1015 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/utils/_requires.py
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     3089 2024-04-29 19:15:32.000000 opinf-0.5.2/src/opinf/utils/_timer.py
+drwxr-xr-x   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        0 2024-04-29 19:25:13.546964 opinf-0.5.2/src/opinf.egg-info/
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     5032 2024-04-29 19:25:13.000000 opinf-0.5.2/src/opinf.egg-info/PKG-INFO
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)     1522 2024-04-29 19:25:13.000000 opinf-0.5.2/src/opinf.egg-info/SOURCES.txt
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        1 2024-04-29 19:25:13.000000 opinf-0.5.2/src/opinf.egg-info/dependency_links.txt
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)      350 2024-04-29 19:25:13.000000 opinf-0.5.2/src/opinf.egg-info/requires.txt
+-rw-r--r--   0 smcquar  (97406) SANDIA\Domain Users (1049671531)        6 2024-04-29 19:25:13.000000 opinf-0.5.2/src/opinf.egg-info/top_level.txt
```

### Comparing `opinf-0.5.1/LICENSE` & `opinf-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opinf-0.5.1/PKG-INFO` & `opinf-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opinf
-Version: 0.5.1
+Version: 0.5.2
 Summary: Operator Inference for data-driven model reduction of dynamical systems.
 Author-email: Willcox Research Group <kwillcox@oden.utexas.edu>
 Maintainer-email: "Shane A. McQuarrie" <shanemcq@utexas.edu>
 License: MIT License
         
         Copyright (c) 2023 Willcox Research Group
         
@@ -48,15 +48,17 @@
 Provides-Extra: tests
 Requires-Dist: pytest>=6.0.2; extra == "tests"
 Requires-Dist: pytest-cov>=2.12.1; extra == "tests"
 Requires-Dist: black>=23.10.0; extra == "tests"
 Requires-Dist: flake8>=3.9.0; extra == "tests"
 Requires-Dist: pre-commit>=3.5.0; extra == "tests"
 Provides-Extra: docs
+Requires-Dist: bibtexparser>=2.0.0b7; extra == "docs"
 Requires-Dist: chardet>=5.0; extra == "docs"
+Requires-Dist: docutils==0.17.1; extra == "docs"
 Requires-Dist: jupyter-book<0.15.0,>=0.14.0; extra == "docs"
 Requires-Dist: jupyterlab>=4.0.9; extra == "docs"
 Requires-Dist: numpydoc>=1.2; extra == "docs"
 Requires-Dist: pandas>=2.0.3; extra == "docs"
 Requires-Dist: sphinx-design>=0.1.0; extra == "docs"
 Requires-Dist: sphinxcontrib-mermaid>=0.7.1; extra == "docs"
```

### Comparing `opinf-0.5.1/README.md` & `opinf-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `opinf-0.5.1/pyproject.toml` & `opinf-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,17 @@
     "pytest>=6.0.2",
     "pytest-cov>=2.12.1",
     "black>=23.10.0",
     "flake8>=3.9.0",
     "pre-commit>=3.5.0",
 ]
 docs = [
+    "bibtexparser>=2.0.0b7",
     "chardet>=5.0",
+    "docutils==0.17.1",
     "jupyter-book>=0.14.0,<0.15.0",
     "jupyterlab>=4.0.9",
     "numpydoc>=1.2",
     "pandas>=2.0.3",
     "sphinx-design>=0.1.0",
     "sphinxcontrib-mermaid>=0.7.1",
 ]
```

### Comparing `opinf-0.5.1/src/opinf/basis/_pod.py` & `opinf-0.5.2/src/opinf/basis/_pod.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,1014 +1,1234 @@
-# pre/basis/_pod.py
-"""Tools for basis computation and reduced-dimension selection."""
+# basis/_pod.py
+"""Dimensionality reduction with Proper Orthogonal Decomposition (POD)."""
 
 __all__ = [
     "PODBasis",
-    "PODBasisMulti",
     "pod_basis",
     "svdval_decay",
     "cumulative_energy",
     "residual_energy",
-    "projection_error",
 ]
 
-import h5py
+import types
+import warnings
 import numpy as np
 import scipy.linalg as la
+import scipy.sparse as sparse
 import sklearn.utils.extmath as sklmath
 import matplotlib.pyplot as plt
 
-from ..errors import LoadfileFormatError
-from ..utils import hdf5_savehandle, hdf5_loadhandle
-from ._linear import LinearBasis, LinearBasisMulti
+from .. import errors, utils
+from ._base import BasisTemplate
+from ._linear import LinearBasis
 
 
+# Helper functions ============================================================
+requires_svdvals = utils.requires2(
+    "svdvals",
+    "no singular value data, call fit()",
+)
+
+
+def _Wmult(W, arr):
+    """Matrix multiply ``W`` and ``arr``, where ``W`` may be a one-dimensional
+    array representing diagonals or a two-dimensional array.
+    """
+    if W.ndim == 1:
+        if arr.ndim == 1:
+            return W * arr
+        elif arr.ndim == 2:
+            return W.reshape((-1, 1)) * arr
+        else:
+            raise ValueError("expected one- or two-dimensional array")
+    return W @ arr
+
+
+# Main class ==================================================================
 class PODBasis(LinearBasis):
-    r"""Proper othogonal decomposition basis, derived from the principal left
-    singular vectors of a collection of states :math:`\Q`:
+    r"""Proper othogonal decomposition basis, consisting of the principal left
+    singular vectors of a collection of states.
 
     .. math::
-       \text{svd}(\Q) = \V\Sigma\W\trp
+       \text{svd}(\Q) = \bfPhi\bfSigma\bfPsi\trp
        \qquad\Longrightarrow\qquad
-       \text{pod}(\Q, r) = \V_{:,:r}
+       \text{pod}(\Q, r) = \bfPhi_{:,:r}
 
-    The low-dimensional approximation is linear:
-
-    .. math::
-       \q \approx \Vr\qhat = \sum_{i=1}^r \hat{q}_i \v_i
+    The low-dimensional approximation is linear, see :class:`LinearBasis`.
+    Here, :math:`\Q\in\mathbb{R}^{n\times k}` is a collection of states,
+    the only argument of :meth:`fit`.
+
+    The POD basis entries :math:`\Vr = \bfPhi_{:,:r}\in\RR^{n\times r}`
+    are always orthogonal, i.e., :math:`\Vr\trp\Vr = \I`. If a weight matrix
+    :math:`\W` is specified, a weighted SVD is computed so that
+    :math:`\Vr\trp\W\Vr = \I`.
+
+    The number of left singular vectors :math:`r` is the dimension of the
+    reduced state and is set by specifying exactly one of the constructor
+    arguments ``num_vectors``, ``svdval_threshold``, ``residual_energy``,
+    ``cumulative_energy``, or ``projection_error``. Once the basis entries are
+    set by calling :meth:`fit`, the reduced state dimension :math:`r` can be
+    updated by calling :meth:`set_dimension`.
+
+    The POD singular values, which are used to select :math:`r`, are the
+    diagonals of :math:`\bfSigma` and are denoted
+    :math:`\sigma_1,\ldots,\sigma_k`.
 
     Parameters
     ----------
-    economize : bool
-        If ``True``, throw away basis vectors beyond the first ``r`` whenever
-        the ``r`` attribute is changed.
+    num_vectors : int
+        Set the reduced state dimension :math:`r` to ``num_vectors``.
+    svdval_threshold : float
+        Choose :math:`r` as the number of normalized POD singular values that
+        are greater than the given threshold, i.e.,
+        :math:`\sigma_{i}/\sigma_{1} \ge` ``svdval_threshold`` for
+        :math:`i=1,\ldots,r`.
+    cumulative_energy : float
+        Choose :math:`r` as the smallest integer such that
+        :math:`\sum_{i=1}^{r}\sigma_i^2\big/\sum_{j=1}^{k}\sigma_j^2`
+        is greater than or equal to ``cumulative_energy``.
+    residual_energy : float
+        Choose :math:`r` as the smallest integer such that
+        :math:`\sum_{i=r+1}^k\sigma_i^2\big/\sum_{j=1}^k\sigma_j^2`
+        is less than or equal to ``residual_energy``.
+    projection_error : float
+        Choose :math:`r` as the smallest integer such that
+        :math:`\|\Q - \Vr\Vr\trp\Q\|_F \big/ \|\Q\|_F`
+        is less than or equal to ``projection_error``.
+    max_vectors : int
+        Maximum number of POD basis vectors to store. After calling
+        :meth:`fit`, the ``reduced_state_dimension`` can be increased up to
+        ``max_vectors``. If not given (default), record all :math:`k` left
+        singular vectors.
+    svdsolver : str or callable
+        Strategy for computing the thin SVD of the states.
+
+        **Options:**
+
+        * ``"dense"`` (default): Use ``scipy.linalg.svd()`` to compute the SVD.
+          May be inefficient for very large state matrices.
+        * ``"randomized"``: Compute an approximate SVD with a randomized
+          approach via ``sklearn.utils.extmath.randomized_svd()``.
+          May be more efficient but less accurate for very large state
+          matrices. **NOTE**: it is highly recommended to set ``max_vectors``
+          to limit the number of computed singular vectors. In this case,
+          only ``max_vectors`` singular *values* are computed as well, meaning
+          the cumulative and residual energies cannot be computed exactly.
+        * callable: If this argument is a callable function, use it for the
+          SVD computation. The signature must match ``scipy.linalg.svd()``,
+          i.e., ``U, s, Vh = svdsolver(states, **svdsolver_options)``
+    weights : (n, n) ndarray or (n,) ndarray None
+        Weight matrix :math:`\W` or its diagonals.
+        When provided, a weighted singular value decomposition of the states
+        is used to ensure that the left singular vectors are orthogonal with
+        respect to the weight matrix, i.e., :math:`\bfPhi\trp\W\bfPhi = \I`.
+        If ``None`` (default), set :math:`\W` to the identity.
+    name : str
+        Label for the state variable that this basis approximates.
+    svdsolver_options : dict
+        Options to pass to the SVD solver.
     """
 
-    def __init__(self, economize=False):
-        """Initialize an empty basis."""
-        self.__r = None
-        self.__entries = None
-        self.__svdvals = None
-        self.__dual = None
-        # self.__spatialweights = None
-        self.economize = bool(economize)
-        LinearBasis.__init__(self)
+    # Valid SVD solvers.
+    __SVDSOLVERS = types.MappingProxyType(
+        {
+            "dense": la.svd,
+            "randomized": sklmath.randomized_svd,
+            # "streaming":  # TODO
+        }
+    )
 
-    # Dimension selection -----------------------------------------------------
-    def __shrink_stored_entries_to(self, r):
-        if self.entries is not None and r is not None:
-            self.__entries = self.__entries[:, :r].copy()
-            self.__dual = self.__dual[:, :r].copy()
+    # Constructors ------------------------------------------------------------
+    def __init__(
+        self,
+        num_vectors: int = None,
+        svdval_threshold: float = None,
+        cumulative_energy: float = None,
+        residual_energy: float = None,
+        projection_error: float = None,
+        max_vectors: int = None,
+        svdsolver: str = "dense",
+        weights: np.ndarray = None,
+        name: str = None,
+        **svdsolver_options,
+    ):
+        """Initialize an empty basis."""
+        # Superclass constructor.
+        LinearBasis.__init__(self, entries=None, weights=weights, name=name)
 
-    @property
-    def r(self):
-        """Dimension of the basis, i.e., the number of basis vectors."""
-        return self.__r
-
-    @r.setter
-    def r(self, r):
-        """Set the reduced dimension."""
-        if r is None:
-            self.__r = None
-            return
-        if self.entries is None:
-            raise AttributeError("empty basis (call fit() first)")
-        if self.__entries.shape[1] < r:
-            raise ValueError(
-                f"only {self.__entries.shape[1]:d} " "basis vectors stored"
-            )
-        self.__r = r
+        # Store dimension selection criteria.
+        self._set_dimension_selection_criterion(
+            num_vectors=num_vectors,
+            svdval_threshold=svdval_threshold,
+            cumulative_energy=cumulative_energy,
+            residual_energy=residual_energy,
+            projection_error=projection_error,
+        )
+        self.__energy_is_being_estimated = False
 
-        # Forget higher-order basis vectors.
-        if self.economize:
-            self.__shrink_stored_entries_to(r)
+        # Initialize hyperparameter properties.
+        if max_vectors is not None:
+            max_vectors = int(max_vectors)
+            if max_vectors <= 0:
+                raise ValueError("max_vectors must be a positive integer")
+        self.__max_vectors_desired = max_vectors
+        self.svdsolver = svdsolver
+        self.svdsolver_options = svdsolver_options
 
-    @property
-    def economize(self):
-        """If True, throw away basis vectors beyond the first `r` whenever
-        the `r` attribute is changed."""
-        return self.__economize
-
-    @economize.setter
-    def economize(self, econ):
-        """Set the economize flag."""
-        self.__economize = bool(econ)
-        if self.__economize:
-            self.__shrink_stored_entries_to(self.r)
+        # Initialize entry properties.
+        self.__leftvecs = None
+        self.__svdvals = None
+        self.__rightvecs = None
+        self.__cumulative_energy = None
+        self.__residual_energy = None
+
+        # Store weights (separate from LinearBasis.__weights)
+        if weights is not None:
+            if weights.ndim == 1:
+                self.__sqrt_weights = np.sqrt(weights)
+            else:  # (weights.ndim == 2, checked by LinearBasis)
+                self.__sqrt_weights = la.sqrtm(weights)
+                self.__sqrt_weights_cho = la.cho_factor(self.__sqrt_weights)
 
-    def set_dimension(
-        self, r=None, cumulative_energy=None, residual_energy=None
+    @classmethod
+    def from_svd(
+        cls,
+        leftvecs: np.ndarray,
+        svdvals: np.ndarray,
+        rightvecs: np.ndarray = None,
+        num_vectors: int = None,
+        svdval_threshold: float = None,
+        residual_energy: float = None,
+        cumulative_energy: float = None,
+        projection_error: float = None,
+        max_vectors: int = None,
+        weights: np.ndarray = None,
+        name: str = None,
     ):
-        """Set the basis dimension, i.e., the number of basis vectors.
+        r"""Initialize a :class:`PODBasis` from the singular value
+        decomposition of an :math:`n\times k` matrix.
 
         Parameters
         ----------
-        r : int or None
-            Number of basis vectors to include in the basis.
-        cumulative_energy : float or None
-            Cumulative energy threshold. If provided and r=None, choose the
-            smallest number of basis vectors so that the cumulative singular
-            value energy exceeds the given threshold.
-        residual_energy : float or None
-            Residual energy threshold. If provided, r=None, and
-            cumulative_energy=None, choose the smallest number of basis vectors
-            so that the residual singular value energy is less than the given
-            threshold.
+        leftvecs : (n, r) ndarray
+            Left singular vectors.
+        svdvals : (r,) ndarray
+            Singular values.
+        rightvecs : (k, r) ndarray or None
+            Right singular vectors. Each *column* is a singular vector.
 
         Returns
         -------
-        r : int
-            Selected basis dimension.
+        Initialized :class:`PODBasis` object.
+
+        Notes
+        -----
+        See :class:`PODBasis` for details on other arguments.
         """
-        if r is None:
-            self._check_svdvals_exist()
-            svdvals2 = self.svdvals**2
-            cum_energy = np.cumsum(svdvals2) / np.sum(svdvals2)
-            if cumulative_energy is not None:
-                r = int(np.searchsorted(cum_energy, cumulative_energy)) + 1
-            elif residual_energy is not None:
-                r = np.count_nonzero(1 - cum_energy > residual_energy) + 1
-            else:
-                r = self.entries.shape[1]
-        self.r = r
+        # Default dimensionality criterion: use all left singular vectors.
+        if all(
+            arg is None
+            for arg in (
+                num_vectors,
+                svdval_threshold,
+                residual_energy,
+                cumulative_energy,
+                projection_error,
+            )
+        ):
+            num_vectors = leftvecs.shape[1]
+
+        basis = cls(
+            num_vectors=num_vectors,
+            svdval_threshold=svdval_threshold,
+            residual_energy=residual_energy,
+            cumulative_energy=cumulative_energy,
+            projection_error=projection_error,
+            max_vectors=max_vectors,
+            weights=weights,
+            name=name,
+        )
+        basis._store_svd(leftvecs, svdvals, rightvecs)
+        basis._set_dimension_from_criterion()
 
+        return basis
+
+    # Properties: hyperparameters ---------------------------------------------
     @property
-    def rmax(self):
-        """Total number of stored basis vectors, i.e., the maximum value of r.
-        Always the same as the dimension r if economize=True.
+    def svdsolver(self) -> str:
+        """Strategy for computing the thin SVD of the states, either
+        ``'dense'``, ``'randomized'``, or ``'custom'``.
         """
-        return None if self.__entries is None else self.__entries.shape[1]
+        return self.__svdsolverlabel
+
+    @svdsolver.setter
+    def svdsolver(self, s):
+        if callable(s):
+            self.__svdsolverlabel = "custom"
+            self.__svdengine = s
+            return
+
+        if s not in self.__SVDSOLVERS:
+            raise AttributeError(
+                f"invalid svdsolver '{s}', options: "
+                + ", ".join(self.__SVDSOLVERS.keys())
+            )
+        self.__svdsolverlabel = s
+        self.__svdengine = self.__SVDSOLVERS[s]
 
-    # Properties --------------------------------------------------------------
     @property
-    def entries(self):
-        """Entries of the basis."""
-        return None if self.__entries is None else self.__entries[:, : self.r]
+    def svdsolver_options(self) -> dict:
+        """Options to pass to the SVD solver."""
+        return self.__svdsolver_options
+
+    @svdsolver_options.setter
+    def svdsolver_options(self, options):
+        if options is None:
+            options = dict()
+        if not isinstance(options, dict):
+            raise TypeError("svdsolver_options must be a dictionary")
+        self.__svdsolver_options = options
 
+    # Properties: entries -----------------------------------------------------
     @property
-    def shape(self):
-        """Dimensions of the basis (state_dimension, reduced_dimension)."""
-        return None if self.entries is None else (self.n, self.r)
+    def leftvecs(self):
+        """Leading left singular vectors of the training data."""
+        return self.__leftvecs
+
+    @property
+    def max_vectors(self) -> int:
+        """Number of POD basis vectors stored in memory.
+        The ``reduced_state_dimension`` may be increased up to ``max_vectors``.
+        """
+        return None if self.leftvecs is None else self.leftvecs.shape[1]
 
     @property
     def svdvals(self):
-        """Singular values of the training data."""
+        """Normalized singular values of the training data."""
         return self.__svdvals
 
     @property
-    def dual(self):
-        """Leading *right* singular vectors."""
-        return None if self.__dual is None else self.__dual[:, : self.r]
-
-    # @property
-    # def spatialweights(self):
-    #     """Symmetric positive definite weighting matrix for the inner
-    #     product. """
-    #     return self.__spatialweights
-
-    # @spatialweights.setter
-    # def spatialweights(self, weights):
-    #     """Set the spatial weights, checking dimension."""
-    #     if weights is not None and self.n is not None:
-    #         if weights.shape[0] != self.n:
-    #             raise ValueError(f"{weights.shape} spatialweights "
-    #                              f"not aligned with dimension n = {self.n}")
-    #     self.__spatialweights = weights
-
-    # def _spatial_weighting(self, state, weights):
-    #     """Weight a state or a collection of states (spatially)."""
-    #     if weights is not None:
-    #         if weights.ndim == 1:
-    #             if state.ndim == 2:
-    #                 weights = weights.reshape(-1, 1)
-    #             return weights * state
-    #         return weights @ state
-    #     return state
-
-    # Dimension reduction -----------------------------------------------------
-    # def compress(self, state):
-    #     """Map high-dimensional states to low-dimensional latent coordinates.
-
-    #     Parameters
-    #     ----------
-    #     state : (n,) or (n, k) ndarray
-    #         High-dimensional state vector, or a collection of k such vectors
-    #         organized as the columns of a matrix.
-
-    #     Returns
-    #     -------
-    #     state_ : (r,) or (r, k) ndarray
-    #         Low-dimensional latent coordinate vector, or a collection of k
-    #         such vectors organized as the columns of a matrix.
-    #     """
-    #     # if self.spatialweights.ndim == 1 and
-    #     # # state.ndim == 2 and state.shape[1] < self.r:
-    #     #     return self._spatial_weighting(self.entries,
-    #     #                                 self.spatialweights).T @ state
-    #     return self.entries.T @ self._spatial_weighting(state,
-    #                                                     self.spatialweights)
+    def rightvecs(self):
+        """Leading *right* singular vectors of the training data."""
+        return self.__rightvecs
 
-    # Fitting -----------------------------------------------------------------
-    @staticmethod
-    def _validate_rank(states, r):
-        """Validate the rank `r` (if given)."""
-        rmax = min(states.shape)
-        if r is not None and (r > rmax or r < 1):
-            raise ValueError(f"invalid POD rank r = {r} (need 1 ≤ r ≤ {rmax})")
+    @property
+    def cumulative_energy(self) -> float:
+        r"""Amount of singular value energy captured by the basis,
+        :math:`\sum_{i=1}^r\sigma_i^2\big/\sum_{j=1}^k\sigma_j^2`.
+        """
+        return self.__cumulative_energy
 
-    def _store_svd(self, V, svals, Wt):
-        """Store SVD components as private attributes."""
-        self.__entries = V
-        self.__svdvals = np.sort(svals)[::-1] if svals is not None else None
-        self.__dual = Wt.T if Wt is not None else None
+    @property
+    def residual_energy(self) -> float:
+        r"""Amount of singular value energy *not* captured by the basis,
+        :math:`\sum_{i=r+1}^k\sigma_i^2\big/\sum_{j=1}^k\sigma_j^2`.
+        """
+        return self.__residual_energy
+
+    def __str__(self):
+        """String representation: class, dimensions, and
+        singular value energies.
+        """
+        out = [LinearBasis.__str__(self)]
+
+        if (ce := self.cumulative_energy) is not None:
+            if self.__energy_is_being_estimated:
+                out.append(f"Approximate cumulative energy: {ce:%}")
+            else:
+                out.append(f"Cumulative energy: {ce:%}")
+
+        if (re := self.residual_energy) is not None:
+            if self.__energy_is_being_estimated:
+                out.append(f"Approximate residual energy:   {re:.4e}")
+            else:
+                out.append(f"Residual energy:   {re:.4e}")
 
-    def _fit(
-        self, driver, states, r, cumulative_energy, residual_energy, **options
+        if (mv := self.max_vectors) is not None:
+            out.append(f"{mv:d} basis vectors available")
+
+        if self.__svdsolverlabel == "dense":
+            out.append("SVD solver: scipy.linalg.svd()")
+        elif self.__svdsolverlabel == "randomized":
+            out.append("SVD solver: sklearn.utils.extmath.randomized_svd()")
+        elif self.__svdsolverlabel == "custom":
+            if (name := self.__svdengine.__name__) == "<lambda>":
+                out.append("SVD solver: custom lambda function")
+            else:
+                out.append(f"SVD solver: {name}()")
+
+        return "\n  ".join(out)
+
+    # Dimension selection -----------------------------------------------------
+    def _set_dimension_selection_criterion(
+        self,
+        num_vectors: int = None,
+        svdval_threshold: float = None,
+        cumulative_energy: float = None,
+        residual_energy: float = None,
+        projection_error: float = None,
     ):
-        """Compute the POD basis of rank r corresponding to the states using
-        `driver()` to compute the SVD.
+        args = [
+            ("num_vectors", num_vectors),
+            ("svdval_threshold", svdval_threshold),
+            ("cumulative_energy", cumulative_energy),
+            ("residual_energy", residual_energy),
+            ("projection_error", projection_error),
+        ]
+        provided = [(arg[1] is not None) for arg in args]
+
+        # More than one argument provided.
+        if sum(provided) > 1:
+            firstarg = args[np.argmax(provided)]
+            warnings.warn(
+                "received multiple dimension selection criteria, using "
+                f"{firstarg[0]}={firstarg[1]}",
+                errors.UsageWarning,
+            )
+            self.__criterion = firstarg
+            return
 
-        Parameters
-        ----------
-        driver : callable
-            Function that computes the SVD of the given states.
-        states : (n, k) ndarray
-            Matrix of k snapshots. Each column is a single snapshot of
-            dimension n.
-        r : int or None
-            Number of vectors to include in the basis.
-            If None, use the largest possible basis (r = min{n, k}).
-        cumulative_energy : float or None
-            Cumulative energy threshold. If provided and r=None, choose the
-            smallest number of basis vectors so that the cumulative singular
-            value energy exceeds the given threshold.
-        residual_energy : float or None
-            Residual energy threshold. If provided, r=None, and
-            cumulative_energy=None, choose the smallest number of basis vectors
-            so that the residual singular value energy is less than the given
-            threshold.
-        options
-            Additional parameters for scipy.linalg.svd().
+        # Return the one provided argument.
+        for name, val in args:
+            if val is not None:
+                self.__criterion = (name, val)
+                return
+
+        # No arguments provided.
+        raise ValueError(
+            "exactly one dimension selection criterion must be provided"
+        )
 
-        Notes
-        -----
-        This method computes the full singular value decomposition of `states`.
-        The method fit_randomized() uses a randomized SVD.
+    @BasisTemplate.reduced_state_dimension.setter
+    def reduced_state_dimension(self, r):
+        """Set the reduced state dimension :math:`r`. If there is SVD data,
+        set the basis entries to the first r left singular vectors.
+
+        If r > max_vectors, set r = max_vectors and raise a warning.
         """
-        #  spatialweights, temporalweights, **options):
-        if np.ndim(states) == 3:
-            # Concatenate list of states.
-            states = np.hstack(states)
-        self._validate_rank(states, r)
+        r = int(r)
 
-        # # Weight the states.
-        # if spatialweights is not None:
-        #     if spatialweights.ndim == 1:
-        #         root_weights = np.sqrt(spatialweights)
-        #         inv_root_weights = 1 / root_weights
-        #     elif spatialweights.ndim == 2:
-        #         root_weights = la.sqrtm(spatialweights)
-        #         inv_root_weights = la.inv(root_weights)
-        #     else:
-        #         raise ValueError("1D spatial weights only")
-        #     states = self._spatial_weighting(states, root_weights)
+        # No basis data yet, but when fit() is called there will be r vectors.
+        if self.svdvals is None:
+            self._set_dimension_selection_criterion(num_vectors=r)
+            BasisTemplate.reduced_state_dimension.fset(self, r)
+            return
 
-        # Compute the SVD.
-        V, svdvals, Wt = driver(states, **options)
+        # Basis data already exists, change the dimension and update.
+        if r > (k := self.max_vectors):
+            warnings.warn(
+                "selected reduced dimension exceeds number of stored vectors, "
+                f"setting reduced_state_dimension = max_vectors = {k:d}",
+                errors.UsageWarning,
+            )
+            r = self.max_vectors
+        BasisTemplate.reduced_state_dimension.fset(self, r)
 
-        # Unweight the basis vectors.
-        # if spatialweights is not None:
-        #     if spatialweights.ndim == 1:
-        #         V *= np.reshape(1 / root_weights, (-1, 1))
-        #     elif spatialweights.ndim == 2:
-        #         V = inv_root_weights @ V
+        # Update singular value energies.
+        r = self.reduced_state_dimension
+        svdvals2 = self.svdvals**2
+        self.__cumulative_energy = np.sum(svdvals2[:r]) / np.sum(svdvals2)
+        self.__residual_energy = 1 - self.__cumulative_energy
 
-        # Store the results.
-        self._store_svd(V, svdvals, Wt)
-        self.set_dimension(r, cumulative_energy, residual_energy)
-        # self.spatialweights = spatialweights
+        # Update entries.
+        LinearBasis.__init__(
+            self,
+            entries=self.__leftvecs[:, :r],
+            weights=self.weights,
+            check_orthogonality=True,
+            name=self.name,
+        )
 
-        return self
+    def _set_dimension_from_criterion(self):
+        """Set the dimension by interpreting the ``__criterion`` attribute."""
+        criterion, value = self.__criterion
+        svdvals2 = self.svdvals**2
+        nsvdvals = svdvals2.size
+        energy = np.cumsum(svdvals2) / np.sum(svdvals2)
+
+        if criterion == "num_vectors":
+            r = value
+        elif criterion == "svdval_threshold":
+            r = np.count_nonzero(self.svdvals >= value)
+        elif criterion == "cumulative_energy":
+            r = int(np.searchsorted(energy, value)) + 1
+            if self.__energy_is_being_estimated:
+                warnings.warn(
+                    "cumulative energy is being estimated from only "
+                    f"{nsvdvals:d} singular values",
+                    errors.UsageWarning,
+                )
+        elif criterion == "residual_energy":
+            r = np.count_nonzero(1 - energy >= value) + 1
+            if self.__energy_is_being_estimated:
+                warnings.warn(
+                    "residual energy is being estimated from only "
+                    f"{nsvdvals:d} singular values",
+                    errors.UsageWarning,
+                )
+        elif criterion == "projection_error":
+            r = np.count_nonzero(np.sqrt(1 - energy) >= value) + 1
+            if self.__energy_is_being_estimated:
+                warnings.warn(
+                    "projection error is being estimated from only "
+                    f"{nsvdvals:d} singular values",
+                    errors.UsageWarning,
+                )
+
+        self.reduced_state_dimension = r
 
-    def fit(
+    def set_dimension(
         self,
-        states,
-        r=None,
-        cumulative_energy=None,
-        residual_energy=None,
-        **options,
+        num_vectors: int = None,
+        svdval_threshold: float = None,
+        cumulative_energy: float = None,
+        residual_energy: float = None,
+        projection_error: float = None,
     ):
-        """Compute the POD basis of rank r corresponding to the states
-        via the compact/thin singular value decomposition (scipy.linalg.svd()).
+        r"""Set the reduced state dimension :math:`r`.
+        Exactly one argument should be specified
 
         Parameters
         ----------
-        states : (n, k) ndarray
-            Matrix of k snapshots. Each column is a single snapshot of
-            dimension n.
-        r : int or None
-            Number of vectors to include in the basis.
-            If None, use the largest possible basis (r = min{n, k}).
-        cumulative_energy : float or None
-            Cumulative energy threshold. If provided and r=None, choose the
-            smallest number of basis vectors so that the cumulative singular
-            value energy exceeds the given threshold.
-        residual_energy : float or None
-            Residual energy threshold. If provided, r=None, and
-            cumulative_energy=None, choose the smallest number of basis vectors
-            so that the residual singular value energy is less than the given
-            threshold.
-        options
-            Additional parameters for scipy.linalg.svd().
-
-        Notes
-        -----
-        This method computes the full singular value decomposition of `states`.
-        The method fit_randomized() uses a randomized SVD.
+        num_vectors : int
+            Set :math:`r` to ``num_vectors``.
+        svdval_threshold : float
+            Choose :math:`r` as the number of normalized POD singular values
+            that are greater than the given threshold, i.e.,
+            :math:`\sigma_{i}/\sigma_{1} \ge` ``svdval_threshold`` for
+            :math:`i=1,\ldots,r`.
+        cumulative_energy : float
+            Choose :math:`r` as the smallest integer such that
+            :math:`\sum_{i=1}^{r}\sigma_i^2\big/\sum_{j=1}^{k}\sigma_j^2`
+            is greater than or equal to ``cumulative_energy``.
+        residual_energy : float
+            Choose :math:`r` as the smallest integer such that
+            :math:`\sum_{i=r+1}^k\sigma_i^2\big/\sum_{j=1}^k\sigma_j^2`
+            is less than or equal to ``residual_energy``.
+        projection_error : float
+            Choose :math:`r` as the smallest integer such that
+            :math:`\|\Q - \Vr\Vr\trp\Q\|_F \big/ \|\Q\|_F`
+            is less than or equal to ``projection_error``.
         """
-        # spatialweights=None, temporalweights=None, **options):
-        options["full_matrices"] = False
-
-        return self._fit(
-            la.svd, states, r, cumulative_energy, residual_energy, **options
+        self._set_dimension_selection_criterion(
+            num_vectors=num_vectors,
+            svdval_threshold=svdval_threshold,
+            residual_energy=residual_energy,
+            cumulative_energy=cumulative_energy,
+            projection_error=projection_error,
         )
 
-    def fit_randomized(self, states, r, **options):
-        """Compute the POD basis of rank r corresponding to the states
-        via the randomized singular value decomposition
-        (sklearn.utils.extmath.randomized_svd()).
+        # No basis data yet, do nothing.
+        if self.svdvals is None:
+            return
+
+        # Basis data exists, set the dimension and update.
+        self._set_dimension_from_criterion()
+
+    # Fitting -----------------------------------------------------------------
+    def _store_svd(self, left, svdvals, right):
+        """Store the singular value decomposition, normalizing the singular
+        values.
+        """
+        self.__leftvecs = left
+        svdvals = np.sort(svdvals)[::-1]
+        self.__svdvals = svdvals / svdvals[0]
+        self.__rightvecs = right
+
+    def fit(self, states):
+        """Compute the POD basis entries by taking the SVD of the states.
 
         Parameters
         ----------
         states : (n, k) ndarray
-            Matrix of k snapshots. Each column is a single snapshot of
-            dimension n.
-        r : int
-            Number of vectors to include in the basis.
-        options
-            Additional parameters for sklearn.utils.extmath.randomized_svd().
+            Matrix of :math:`k` :math:`n`-dimensional snapshots.
+        """
+        if np.ndim(states) == 3:
+            states = np.hstack(states)
 
-        Notes
-        -----
-        This method uses an iterative method to approximate a partial singular
-        value decomposition, which can be useful for very large n.
-        The method fit() computes the full singular value decomposition.
-        """
-        # spatialweights=None, temporalweights=None, **options):
-        if "random_state" not in options:
-            options["random_state"] = None
-        options["n_components"] = r
-
-        return self._fit(
-            sklmath.randomized_svd,
-            states,
-            r,
-            None,
-            None,
-            # spatialweights, temporalweights,
-            **options,
+        # Limit maximum number of vectors if needed.
+        rmax = min(states.shape)
+        keep = self.__max_vectors_desired
+        if keep is None:
+            keep = rmax
+        elif keep > rmax:
+            warnings.warn(
+                f"only {rmax:d} singular vectors can be extracted "
+                f"from ({states.shape[0]:d} x {states.shape[1]:d}) snapshots, "
+                f"setting max_vectors={rmax:d}",
+                errors.UsageWarning,
+            )
+            keep = rmax
+
+        # SVD solver settings.
+        self.__energy_is_being_estimated = False
+        options = self.svdsolver_options.copy()
+
+        if self.__svdsolverlabel == "dense":
+            options["full_matrices"] = False
+        elif self.__svdsolverlabel == "randomized":
+            options["n_components"] = keep
+            if "random_state" not in options:
+                options["random_state"] = None
+            if keep < rmax:
+                self.__energy_is_being_estimated = True
+
+        # Weight the states.
+        if self.weights is not None:
+            if states.shape[0] != (nW := self.__sqrt_weights.shape[0]):
+                raise errors.DimensionalityError(
+                    f"states not aligned with weights, should have {nW:d} rows"
+                )
+            states = _Wmult(self.__sqrt_weights, states)
+
+        # Compute the SVD.
+        V, svdvals, Wt = self.__svdengine(states, **options)
+
+        # Unweight the basis.
+        if self.weights is not None:
+            if self.__sqrt_weights.ndim == 1:
+                V = _Wmult(1 / self.__sqrt_weights, V)
+            else:
+                V = la.cho_solve(self.__sqrt_weights_cho, V)
+                # V = la.solve(sqrtW, V)
+
+        # Store the results.
+        self._store_svd(
+            left=V[:, :keep],
+            svdvals=svdvals,
+            right=Wt[:keep, :].T,
         )
+        self._set_dimension_from_criterion()
+
+        return self
 
     # Visualization -----------------------------------------------------------
-    def _check_svdvals_exist(self):
-        """Raise an AttributeError if there are no singular values stored."""
-        if self.svdvals is None:
-            raise AttributeError("no singular value data (call fit() first)")
+    @requires_svdvals
+    def _plot_single(self, plotter, **kwargs):
+        """Execute a single plotting routine."""
+        plotter(self.svdvals, **kwargs)
+        return ax if (ax := kwargs.get("ax")) is not None else plt.gca()
 
-    def plot_svdval_decay(self, threshold=None, normalize=True, ax=None):
+    def plot_svdval_decay(
+        self,
+        threshold=None,
+        right=None,
+        ax=None,
+        **options,
+    ):
         """Plot the normalized singular value decay.
 
         Parameters
         ----------
-        threshold : float or None
-            Cutoff value to mark on the plot.
-        normalize : bool
-            If True, normalize so that the maximum singular value is 1.
+        threshold : float or list[floats] or None
+            Cutoff value(s) to mark on the plot.
+        right : int or None
+            Maximum singular value index to plot (``plt.xlim(right=right)``).
         ax : plt.Axes or None
-            Matplotlib Axes to plot on. If None, a new figure is created.
+            Matplotlib Axes to plot on.
+            If ``None`` (default), a new single-axes figure is created.
+        options : dict
+            Additional arguments to pass to ``plt.semilogy()``.
 
         Returns
         -------
         ax : plt.Axes
             Matplotlib Axes for the plot.
         """
-        self._check_svdvals_exist()
-        if ax is None:
-            ax = plt.figure().add_subplot(111)
-
-        singular_values = self.svdvals
-        if normalize:
-            singular_values = singular_values / singular_values[0]
-        j = np.arange(1, singular_values.size + 1)
-        ax.semilogy(j, singular_values, "k*", ms=10, mew=0, zorder=3)
-        ax.set_xlim((0, j.size))
+        kwargs = dict(threshold=threshold, plot=True, right=right, ax=ax)
+        kwargs.update(options)
+        return self._plot_single(svdval_decay, **kwargs)
 
-        if threshold is not None:
-            rank = np.count_nonzero(singular_values > threshold)
-            ax.axhline(threshold, color="gray", linewidth=0.5)
-            ax.axvline(rank, color="gray", linewidth=0.5)
-            # TODO: label lines with text.
-
-        ax.set_xlabel("Singular value index")
-        ax.set_ylabel(("Normalized s" if normalize else "") + "ingular values")
+    def plot_cumulative_energy(
+        self,
+        threshold=None,
+        right=None,
+        ax=None,
+        **options,
+    ):
+        r"""Plot the cumulative singular value energy.
 
-        return ax
+        The cumulative energy of :math:`r` singular values is defined by
 
-    def plot_residual_energy(self, threshold=None, ax=None):
-        """Plot the residual singular value energy decay, defined by
+        .. math::
+           \kappa_r = \sum_{i=1}^r\sigma_i^2 \bigg/ \sum_{j=1}^k\sigma_j^2.
 
-            residual_j = sum(svdvals[j+1:]**2) / sum(svdvals**2).
+        This method plots :math:`\kappa_r` as a function of :math:`r`.
 
         Parameters
         ----------
-        threshold : 0 ≤ float ≤ 1 or None
-            Cutoff value to mark on the plot.
+        threshold : float or list[floats] or None
+            Threshold energy value(s) to mark on the plot.
+        right : int or None
+            Maximum singular value index to plot (``plt.xlim(right=right)``).
         ax : plt.Axes or None
-            Matplotlib Axes to plot on. If None, a new figure is created.
+            Matplotlib Axes to plot on.
+            If ``None`` (default), a new single-axes figure is created.
+        kwargs : dict
+            Additional arguments to pass to ``plt.semilogy()``.
 
         Returns
         -------
         ax : plt.Axes
             Matplotlib Axes for the plot.
         """
-        self._check_svdvals_exist()
-        if ax is None:
-            ax = plt.figure().add_subplot(111)
-
-        svdvals2 = self.svdvals**2
-        res_energy = 1 - (np.cumsum(svdvals2) / np.sum(svdvals2))
-        j = np.arange(1, svdvals2.size + 1)
-        ax.semilogy(j, res_energy, "C0.-", ms=10, lw=1, zorder=3)
-        ax.set_xlim(0, j.size)
+        kwargs = dict(threshold=threshold, plot=True, right=right, ax=ax)
+        kwargs.update(options)
+        return self._plot_single(cumulative_energy, **kwargs)
 
-        if threshold is not None:
-            rank = np.count_nonzero(res_energy > threshold) + 1
-            ax.axhline(threshold, color="gray", linewidth=0.5)
-            ax.axvline(rank, color="gray", linewidth=0.5)
-            # TODO: label lines with text.
-
-        ax.set_xlabel("Singular value index")
-        ax.set_ylabel("Residual energy")
+    def plot_residual_energy(
+        self,
+        threshold=None,
+        right=None,
+        ax=None,
+        **options,
+    ):
+        r"""Plot the residual singular value energy.
 
-        return ax
+        The residual energy of :math:`r` singular values is defined by
 
-    def plot_cumulative_energy(self, threshold=None, ax=None):
-        """Plot the cumulative singular value energy, defined by
+        .. math::
+           \epsilon_r
+           = \sum_{i=r+1}^k\sigma_i^2 \bigg/ \sum_{j=1}^k\sigma_j^2
+           = 1 - \left(
+           \sum_{i=1}^r\sigma_i^2 \bigg/ \sum_{j=1}^k\sigma_j^2
+           \right)
 
-            energy_j = sum(svdvals[:j]**2) / sum(svdvals**2).
+        This method plots :math:`\epsilon_r` as a function of :math:`r`.
 
         Parameters
         ----------
-        threshold : 0 ≤ float ≤ 1 or None
-            Cutoff value to mark on the plot.
+        threshold : float or list[floats] or None
+            Cutoff value(s) to mark on the plot.
+        right : int or None
+            Maximum singular value index to plot (``plt.xlim(right=right)``).
         ax : plt.Axes or None
-            Matplotlib Axes to plot on. If None, a new figure is created.
+            Matplotlib Axes to plot on.
+            If ``None`` (default), a new single-axes figure is created.
+        options : dict
+            Additional arguments to pass to ``plt.semilogy()``.
 
         Returns
         -------
         ax : plt.Axes
             Matplotlib Axes for the plot.
         """
-        self._check_svdvals_exist()
-        if ax is None:
-            ax = plt.figure().add_subplot(111)
+        kwargs = dict(threshold=threshold, plot=True, right=right, ax=ax)
+        kwargs.update(options)
+        return self._plot_single(residual_energy, **kwargs)
+
+    @requires_svdvals
+    def plot_energy(self, right=None):
+        """Plot the normalized singular values and the cumulative and residual
+        energies.
 
-        svdvals2 = self.svdvals**2
-        cum_energy = np.cumsum(svdvals2) / np.sum(svdvals2)
-        j = np.arange(1, svdvals2.size + 1)
-        ax.plot(j, cum_energy, "C0.-", ms=10, lw=1, zorder=3)
-        ax.set_xlim(0, j.size)
+        Parameters
+        ----------
+        right : int or None
+            Maximum singular value index to plot (``plt.xlim(right=right)``).
+        """
+        r = self.reduced_state_dimension
 
-        if threshold is not None:
-            rank = int(np.searchsorted(cum_energy, threshold)) + 1
-            ax.axhline(threshold, color="gray", linewidth=0.5)
-            ax.axvline(rank, color="gray", linewidth=0.5)
-            # TODO: label lines with text.
+        def _rline(ax, ymin):
+            ax.axvline(r, color="gray", linewidth=0.5, zorder=1)
+            ax.text(
+                r + 0.5,
+                ymin,
+                f"r = {r}",
+                color="gray",
+                horizontalalignment="left",
+                verticalalignment="bottom",
+            )
 
-        ax.set_xlabel(r"Singular value index")
-        ax.set_ylabel(r"Residual energy")
+        fig, axes = plt.subplots(1, 2, figsize=(13.44, 4.8))
 
-        return ax
+        ax = self.plot_svdval_decay(right=right, ax=axes[0])
+        ax.set_title("POD singular values")
+        _rline(ax, 1.05 * ax.get_ylim()[0])
+
+        ax = self.plot_residual_energy(right=right, ax=axes[1])
+        ax.set_ylabel("Residual energy", color="C1")
+        ax.spines["right"].set_visible(True)
+        ax.tick_params(axis="y", which="both", color="C1", labelcolor="C1")
+        ax.set_title("POD singular value energy")
+
+        ax = self.plot_cumulative_energy(
+            right=right,
+            ax=axes[1].twinx(),
+            color="C0",
+        )
+        ax.spines["left"].set_visible(True)
+        ax.set_ylabel("Cumulative energy", color="C0")
+        ax.tick_params(axis="y", which="both", color="C0", labelcolor="C0")
+        _rline(ax, 0.01 + ax.get_ylim()[0])
 
-    def plot_energy(self):
-        """Plot the normalized singular value and residual energy decay."""
-        self._check_svdvals_exist()
-
-        fig, axes = plt.subplots(1, 2, figsize=(8, 3))
-        self.plot_svdval_decay(ax=axes[0])
-        self.plot_residual_energy(ax=axes[1])
         fig.tight_layout()
 
-        return fig, axes
-
     # Persistence -------------------------------------------------------------
     def save(self, savefile, overwrite=False):
         """Save the basis to an HDF5 file.
 
         Parameters
         ----------
         savefile : str
-            Path of the file to save the basis in.
+            Path of the file to save the basis to.
         overwrite : bool
-            If True, overwrite the file if it already exists. If False
-            (default), raise a FileExistsError if the file already exists.
+            If ``True``, overwrite the file if it already exists.
+            If ``False`` (default), raise a ``FileExistsError`` if the file
+            already exists.
         """
-        with hdf5_savehandle(savefile, overwrite) as hf:
+        with utils.hdf5_savehandle(savefile, overwrite) as hf:
             meta = hf.create_dataset("meta", shape=(0,))
-            meta.attrs["economize"] = int(self.economize)
-            if self.r is not None:
-                meta.attrs["r"] = self.r
-
-            if self.entries is not None:
-                hf.create_dataset("entries", data=self.__entries)
-                hf.create_dataset("svdvals", data=self.__svdvals)
-                hf.create_dataset("dual", data=self.__dual)
-
-    @classmethod
-    def load(cls, loadfile, rmax=None):
-        """Load a basis from an HDF5 file.
-
-        Parameters
-        ----------
-        loadfile : str
-            Path to the file where the basis was stored (via save()).
-        rmax : int or None
-            Maximum number of POD modes to load. If None (default), load all.
-
-        Returns
-        -------
-        PODBasis object
-        """
-        entries, svdvals, dualT, r = None, None, None, rmax
-        with hdf5_loadhandle(loadfile) as hf:
-            if "meta" not in hf:
-                raise LoadfileFormatError(
-                    "invalid save format " "(meta/ not found)"
-                )
-            economize = bool(hf["meta"].attrs["economize"])
-            if "r" in hf["meta"].attrs:
-                r = int(hf["meta"].attrs["r"])
-                if rmax is not None:
-                    r = min(r, rmax)
-
-            if "entries" in hf:
-                entries = hf["entries"][:, :rmax]
-                svdvals = hf["svdvals"][:rmax]
-                dualT = hf["dual"][:, :rmax].T
-
-        out = cls(economize=economize)
-        out._store_svd(entries, svdvals, dualT)
-        out.r = r
-        return out
-
-
-class PODBasisMulti(LinearBasisMulti):
-    r"""Block-diagonal proper othogonal decomposition basis, derived from the
-    principal left singular vectors of a collection of states grouped into
-    blocks.
-
-    .. math::
-       \Q = \left[\begin{array}{c}
-       \Q_1 \\ \vdots \\ \Q_{n_\text{vars}}
-       \end{array}\right]
-       \qquad\Longrightarrow\qquad
-       \text{pod\_multi}(\Q; r_1,\ldots,r_{n_\text{vars}})
-       = \left[\begin{array}{ccc}
-       \V_1 & & \\
-       & \ddots & \\
-       & & \V_{n_\text{vars}}
-       \end{array}\right]
-
-    where :math:`\V_i = \text{pod}(\Q_i;r_i), i=1,\ldots,n_\text{vars}`.
-
-    The low-dimensional approximation is linear (see :class:`PODBasis`).
-
-    Parameters
-    ----------
-    num_variables : int
-        Number of variables represented in a single snapshot (number of
-        individual bases to learn). The dimension `n` of the snapshots
-        must be evenly divisible by num_variables; for example,
-        num_variables=3 means the first n entries of a snapshot correspond to
-        the first variable, and the next n entries correspond to the second
-        variable, and the last n entries correspond to the third variable.
-    economize : bool
-        If True, throw away basis vectors beyond the first `r` whenever
-        the `r` attribute is changed.
-    variable_names : list of num_variables strings, optional
-        Names for each of the `num_variables` variables.
-        Defaults to "variable 1", "variable 2", ....
-    """
-    _BasisClass = PODBasis
+            if self.name:
+                meta.attrs["name"] = self.name
 
-    def __init__(self, num_variables, economize=False, variable_names=None):
-        """Initialize an empty basis."""
-        # Store dimensions.
-        LinearBasisMulti.__init__(
-            self, num_variables, variable_names=variable_names
-        )
-        self.economize = bool(economize)
+            meta.attrs["criterion_type"] = self.__criterion[0]
+            hf.create_dataset("criterion_value", data=[self.__criterion[1]])
 
-    # Properties -------------------------------------------------------------
-    @property
-    def rs(self):
-        """Dimensions for each diagonal basis block, i.e., `rs[i]` is the
-        number of basis vectors in the representation for state variable `i`.
-        """
-        rs = [basis.r for basis in self.bases]
-        return rs if any(rs) else None
-
-    @rs.setter
-    def rs(self, rs):
-        """Reset the basis dimensions."""
-        if len(rs) != self.num_variables:
-            raise ValueError(f"rs must have length {self.num_variables}")
-
-        # This will raise an AttributeError if the entries are not set.
-        for basis, r in zip(self.bases, rs):
-            basis.r = r  # Economization is also taken care of here.
-
-        self._set_entries()
-
-    @property
-    def economize(self):
-        """If True, throw away basis vectors beyond the first `r` whenever
-        the `r` attribute is changed."""
-        return self.__economize
-
-    @economize.setter
-    def economize(self, econ):
-        """Set the economize flag."""
-        econ = bool(econ)
-        for basis in self.bases:
-            basis.economize = econ
-        self.__economize = econ
-
-    # Main routines -----------------------------------------------------------
-    def fit(
-        self,
-        states,
-        rs=None,
-        cumulative_energy=None,
-        residual_energy=None,
-        **options,
-    ):
-        """Fit the basis to the data.
-
-        Parameters
-        ----------
-        states : (n, k) ndarray
-            Matrix of k snapshots. Each column is a single snapshot of
-            dimension n.
-        rs : list(int) or None
-            Number of basis vectors for each state variable.
-            If None, use the largest possible bases (ri = min{ni, k}).
-        cumulative_energy : float or None
-            Cumulative energy threshold. If provided and rs=None, choose the
-            smallest number of basis vectors so that the cumulative singular
-            value energy exceeds the given threshold.
-        residual_energy : float or None
-            Residual energy threshold. If provided, rs=None, and
-            cumulative_energy=None, choose the smallest number of basis vectors
-            so that the residual singular value energy is less than the given
-            threshold.
-        options
-            Additional parameters for scipy.linalg.svd().
-        """
-        # Split the state and compute the basis for each variable.
-        if rs is None:
-            rs = [None] * self.num_variables
-        for basis, r, var in zip(
-            self.bases, rs, np.split(states, self.num_variables, axis=0)
-        ):
-            basis.fit(var, r, cumulative_energy, residual_energy, **options)
-
-        self._set_entries()
-        return self
-
-    def fit_randomized(self, states, rs, **options):
-        """Compute the POD basis of rank r corresponding to the states
-        via the randomized singular value decomposition
-        (sklearn.utils.extmath.randomized_svd()).
-
-        Parameters
-        ----------
-        states : (n, k) ndarray
-            Matrix of k snapshots. Each column is a single snapshot of
-            dimension n.
-        rs : list(int) or None
-            Number of basis vectors for each state variable.
-        options
-            Additional parameters for sklearn.utils.extmath.randomized_svd().
-
-        Notes
-        -----
-        This method uses an iterative method to approximate a partial singular
-        value decomposition, which can be useful for very large n.
-        The method fit() computes the full singular value decomposition.
-        """
-        # Fit the individual bases.
-        if not isinstance(rs, list) or len(rs) != self.num_variables:
-            raise TypeError(f"rs must be list of length {self.num_variables}")
-        for basis, r, var in zip(
-            self.bases, rs, np.split(states, self.num_variables, axis=0)
-        ):
-            basis.fit_randomized(var, r, **options)
-
-        self._set_entries()
-        return self
-
-    # Persistence -------------------------------------------------------------
-    def save(self, savefile, overwrite=False):
-        """Save the basis to an HDF5 file.
+            if self.__max_vectors_desired is not None:
+                hf.create_dataset(
+                    "max_vectors",
+                    data=[self.__max_vectors_desired],
+                )
 
-        Parameters
-        ----------
-        savefile : str
-            Path of the file to save the basis in.
-        overwrite : bool
-            If True, overwrite the file if it already exists. If False
-            (default), raise a FileExistsError if the file already exists.
-        """
-        LinearBasisMulti.save(self, savefile, overwrite)
-        with h5py.File(savefile, "a") as hf:
-            hf["meta"].attrs["economize"] = self.economize
+            if (w := self.weights) is not None:
+                if isinstance(w, sparse.dia_array):
+                    w = w.data[0]
+                hf.create_dataset("weights", data=w)
+
+            if self.leftvecs is not None:
+                hf.create_dataset("leftvecs", data=self.leftvecs)
+                hf.create_dataset("svdvals", data=self.svdvals)
+                hf.create_dataset("rightvecs", data=self.rightvecs)
 
     @classmethod
-    def load(cls, loadfile):
+    def load(cls, loadfile, max_vectors=None):
         """Load a basis from an HDF5 file.
 
         Parameters
         ----------
         loadfile : str
-            Path to the file where the basis was stored (via save()).
+            Path to the file where the basis was stored via :meth:`save`.
+        max_vectors : int or None
+            Maximum number of POD vectors to load. If None (default), load all.
 
         Returns
         -------
         PODBasis object
         """
-        # basis = LinearBasisMulti.load(cls, loadfile)
-        basis = super(cls, cls).load(loadfile)
-        with h5py.File(loadfile, "r") as hf:
-            basis.economize = hf["meta"].attrs["economize"]
-        return basis
+        kwargs = {}
+        with utils.hdf5_loadhandle(loadfile) as hf:
+            attrs = hf["meta"].attrs
+
+            if "name" in attrs:
+                kwargs["name"] = attrs["name"]
+
+            kwargs[attrs["criterion_type"]] = hf["criterion_value"][0]
+
+            if "max_vectors" in hf:
+                kwargs["max_vectors"] = hf["max_vectors"][0]
+
+            if "weights" in hf:
+                kwargs["weights"] = hf["weights"][:]
+
+            if "leftvecs" in hf:
+                if (r := max_vectors) is not None:
+                    r = min(r, hf["leftvecs"].shape[1])
+                    if "num_vectors" in kwargs:
+                        kwargs["num_vectors"] = r
+                kwargs["leftvecs"] = hf["leftvecs"][:, :r]
+                kwargs["svdvals"] = hf["svdvals"][:]
+                kwargs["rightvecs"] = hf["rightvecs"][:, :r]
+                return cls.from_svd(**kwargs)
+
+            return cls(**kwargs)
 
 
 # Functional API ==============================================================
 def pod_basis(
     states,
-    r: int = None,
-    mode: str = "dense",
-    return_W: bool = False,
-    **options,
+    num_vectors: int = None,
+    svdval_threshold: float = None,
+    cumulative_energy: float = None,
+    residual_energy: float = None,
+    projection_error: float = None,
+    svdsolver: str = "dense",
+    weights: np.ndarray = None,
+    return_rightvecs: bool = False,
+    **svdsolver_options,
 ):
-    """Compute the POD basis of rank r corresponding to the states.
+    r"""Compute a POD basis from the given states.
 
     Parameters
     ----------
     states : (n, k) ndarray
-        Matrix of k snapshots. Each column is a single snapshot of dimension n.
-    r : int or None
-        Number of POD basis vectors and singular values to compute.
-        If None (default), compute the full SVD.
-    mode : str
-        Strategy to use for computing the truncated SVD of the states. Options:
-
-        * "dense" (default): Use scipy.linalg.svd() to compute the SVD.
-            May be inefficient for very large matrices.
-        * "randomized": Compute an approximate SVD with a randomized approach
-            using sklearn.utils.extmath.randomized_svd(). This gives faster
-            results at the cost of some accuracy.
-
-    return_W : bool
-        If True, also return the first r *right* singular vectors.
-    options
-        Additional parameters for the SVD solver, which depends on `mode`:
-
-        * "dense": scipy.linalg.svd()
-        * "randomized": sklearn.utils.extmath.randomized_svd()
+        Matrix of :math:`k` :math:`n`-dimensional snapshots.
+    return_rightvec : bool
+        If ``True``, return the right singular vectors as well.
 
     Returns
     -------
     basis : (n, r) ndarray
-        First r POD basis vectors (left singular vectors).
-        Each column is a single basis vector of dimension n.
+        POD basis matrix, the first :math:`r` left singular vectors of the
+        states.
     svdvals : (n,), (k,), or (r,) ndarray
-        Singular values in descending order. Always returns as many as are
-        calculated: r for mode="randomize", min(n, k) for "dense".
-    W : (k, r) ndarray
-        First r **right** singular vectors, as columns.
-        **Only returned if return_W=True.**
+        Normalized singular values in descending order.
+        Always returns as many as are calculated:
+        :math:`\min\{n, k\}` for ``svdsolver="dense"``,
+        :math:`r` for ``svdsolver="randomized"``.
+    rightvecs : (k, r) ndarray
+        First :math:`r` **right** singular vectors, as columns.
+        **NOTE**: only returned if ``return_rightvecs=True``.
+
+    Notes
+    -----
+    See :class:`PODBasis` for the mathematical definition of POD and for
+    details on other constructor arguments.
     """
-    # Validate the rank.
-    rmax = min(states.shape)
-    if r is None:
-        r = rmax
-    if r > rmax or r < 1:
-        raise ValueError(f"invalid POD rank r = {r} (need 1 ≤ r ≤ {rmax})")
-
-    if mode == "dense" or mode == "simple":
-        V, svdvals, Wt = la.svd(states, full_matrices=False, **options)
-        W = Wt.T
-
-    elif mode == "randomized":
-        if "random_state" not in options:
-            options["random_state"] = None
-        V, svdvals, Wt = sklmath.randomized_svd(states, r, **options)
-        W = Wt.T
-
-    else:
-        raise NotImplementedError(f"invalid mode '{mode}'")
-
-    if return_W:
-        return V[:, :r], svdvals, W[:, :r]
-    return V[:, :r], svdvals
+    # If no criteria given, use the maximum dimension based on the states.
+    criteria = {
+        num_vectors,
+        svdval_threshold,
+        cumulative_energy,
+        residual_energy,
+        projection_error,
+    }
+    if len(criteria) == 1 and criteria.pop() is None:
+        num_vectors = min(states.shape)
+
+    basis = PODBasis(
+        num_vectors=num_vectors,
+        svdval_threshold=svdval_threshold,
+        cumulative_energy=cumulative_energy,
+        residual_energy=residual_energy,
+        projection_error=projection_error,
+        svdsolver=svdsolver,
+        weights=weights,
+        **svdsolver_options,
+    ).fit(states)
+
+    if return_rightvecs:
+        r = basis.reduced_state_dimension
+        return basis.entries, basis.svdvals, basis.rightvecs[:, :r]
+
+    return basis.entries, basis.svdvals
 
 
 def svdval_decay(
     singular_values,
-    tol: float = 1e-8,
-    normalize: bool = True,
+    threshold: float = 1e-8,
     plot: bool = True,
+    right=None,
     ax=None,
-) -> None:
-    """Count the number of normalized singular values that are greater than
-    the specified tolerance.
+    **kwargs,
+):
+    """Count the number of **normalized** singular values that are greater than
+    a specified threshold.
 
     Parameters
     ----------
     singular_values : (n,) ndarray
-        Singular values of a snapshot set, e.g., scipy.linalg.svdvals(states).
-    tol : float or list(float)
+        Singular values of a snapshot matrix, e.g.,
+        ``scipy.linalg.svdvals(states)``.
+    threshold : float or list[floats]
         Cutoff value(s) for the singular values.
-    normalize : bool
-        If True, normalize so that the maximum singular value is 1.
     plot : bool
-        If True, plot the singular values and the cutoff value(s) against the
-        singular value index.
+        If ``True``, plot the singular values and the cutoff value(s) against
+        the singular value index.
+    right : int or None
+        Maximum singular value index to plot (``plt.xlim(right=right)``).
     ax : plt.Axes or None
-        Matplotlib Axes to plot the results on if plot = True.
+        Axes to plot the results on if ``plot=True``.
         If not given, a new single-axes figure is created.
+    kwargs : dict
+        Options to pass to ``plt.semilogy()``
 
     Returns
     -------
     ranks : int or list(int)
-        The number of singular values greater than the cutoff value(s).
+        Number of singular values greater than the cutoff value(s).
     """
-    # Calculate the number of singular values above the cutoff value(s).
-    one_tol = np.isscalar(tol)
-    if one_tol:
-        tol = [tol]
     singular_values = np.sort(singular_values)[::-1]
-    if normalize:
-        singular_values /= singular_values[0]
-    ranks = [np.count_nonzero(singular_values > epsilon) for epsilon in tol]
+    singular_values /= singular_values[0]
+
+    # Calculate the number of singular values above the cutoff value(s).
+    if threshold:
+        if one_threshold := np.isscalar(threshold):
+            threshold = [threshold]
+        ranks = [np.count_nonzero(singular_values > ep) for ep in threshold]
 
     if plot:
-        # Visualize singular values and cutoff value(s).
+        # Plot singular values.
         if ax is None:
             ax = plt.figure().add_subplot(111)
+
+        options = dict(
+            marker="*",
+            color="k",
+            markersize=8,
+            markeredgewidth=0,
+            zorder=3,
+        )
+        options.update(kwargs)
+        marker = options.pop("marker")
+
         j = np.arange(1, singular_values.size + 1)
-        ax.semilogy(j, singular_values, "C0*", ms=10, mew=0, zorder=3)
-        ax.set_xlim((0, j.size))
-        ylim = ax.get_ylim()
-        for epsilon, r in zip(tol, ranks):
-            ax.axhline(epsilon, color="black", linewidth=0.5, alpha=0.75)
-            ax.axvline(r, color="black", linewidth=0.5, alpha=0.75)
-        ax.set_ylim(ylim)
-        ax.set_xlabel(r"Singular value index $j$")
-        ax.set_ylabel(r"Singular value $\sigma_j$")
+        ax.semilogy(j, singular_values, marker, **options)
+        ax.set_xlim((0, j.size + 1))
+        if right:
+            right = min(right, j.size)
+            ax.set_xlim(right=right)
+            _idx = min(int(right), singular_values.size - 1)
+            ax.set_ylim(bottom=singular_values[_idx] / 5)
+
+        # Draw cutoff value(s).
+        if threshold:
+            rborder = ax.get_xlim()[1]
+            ylim = ax.get_ylim()
+            for sigma, r in zip(threshold, ranks):
+                ax.axhline(sigma, color="gray", linewidth=0.5)
+                ax.text(
+                    rborder - 0.5,
+                    1.05 * sigma,
+                    f"{sigma:.2e}",
+                    color="gray",
+                    horizontalalignment="right",
+                    verticalalignment="bottom",
+                )
+                ax.axvline(r, color="gray", linewidth=0.5)
+                ax.text(
+                    r + 0.5,
+                    1.05 * ylim[0],
+                    f"r = {r}",
+                    color="gray",
+                    horizontalalignment="left",
+                    verticalalignment="bottom",
+                )
+            ax.set_ylim(ylim)
+
+        ax.set_xlabel("Singular value index")
+        ax.set_ylabel("Normalized singular values")
+
+    if threshold:
+        return ranks[0] if one_threshold else ranks
 
-    return ranks[0] if one_tol else ranks
 
+def cumulative_energy(
+    singular_values,
+    threshold: float = 0.9999,
+    plot: bool = True,
+    right=None,
+    ax=None,
+    **kwargs,
+):
+    r"""Compute the number of singular values needed to surpass a given
+    cumulative energy threshold.
 
-def cumulative_energy(singular_values, thresh=0.9999, plot=True, ax=None):
-    """Compute the number of singular values needed to surpass a given
-    energy threshold. The energy of j singular values is defined by
+    The cumulative energy of :math:`r` singular values is defined by
 
-        energy_j = sum(singular_values[:j]**2) / sum(singular_values**2).
+    .. math::
+       \kappa_r = \sum_{i=1}^r\sigma_i^2 \bigg/ \sum_{j=1}^k\sigma_j^2.
+
+    This function determines the smalled :math:`r` such that
+    :math:`\kappa_r \ge` ``threshold``.
 
     Parameters
     ----------
     singular_values : (n,) ndarray
-        Singular values of a snapshot set, e.g., scipy.linalg.svdvals(states).
-    thresh : float or list(float)
+        Singular values of a snapshot matrix, e.g.,
+        ``scipy.linalg.svdvals(states)``.
+    threshold : float or list(float)
         Energy capture threshold(s). Default is 99.99%.
     plot : bool
-        If True, plot the singular values and the cumulative energy against
-        the singular value index (linear scale).
+        If ``True``, plot the cumulative energy and the capture threshold(s)
+        against the singular value index (linear scale).
+    right : int or None
+        Maximum singular value index to plot (``plt.xlim(right=right)``).
     ax : plt.Axes or None
-        Matplotlib Axes to plot the results on if plot = True.
+        Axes to plot the results on if ``plot=True``.
         If not given, a new single-axes figure is created.
+    kwargs : dict
+        Options to pass to ``plt.plot()``
 
     Returns
     -------
     ranks : int or list(int)
-        The number of singular values required to capture more than each
-        energy capture threshold.
+        Number of singular values required to capture the specified energy.
     """
     # Calculate the cumulative energy.
     svdvals2 = np.sort(singular_values)[::-1] ** 2
-    cum_energy = np.cumsum(svdvals2) / np.sum(svdvals2)
+    energy = np.cumsum(svdvals2) / np.sum(svdvals2)
+    energy = np.concatenate(([0], energy))
 
     # Determine the points at which the cumulative energy passes the threshold.
-    one_thresh = np.isscalar(thresh)
-    if one_thresh:
-        thresh = [thresh]
-    ranks = [int(np.searchsorted(cum_energy, xi)) + 1 for xi in thresh]
+    if threshold:
+        if one_threshold := np.isscalar(threshold):
+            threshold = [threshold]
+        ranks = [int(np.searchsorted(energy, xi)) for xi in threshold]
 
     if plot:
-        # Visualize cumulative energy and threshold value(s).
+        # Plot cumulative energy and threshold value(s).
         if ax is None:
             ax = plt.figure().add_subplot(111)
-        j = np.arange(1, singular_values.size + 1)
-        ax.plot(j, cum_energy, "C2.-", ms=10, lw=1, zorder=3)
+
+        options = dict(
+            linestyle="-",
+            marker="o",
+            color="C2",
+            markersize=4,
+            markeredgewidth=0,
+            linewidth=0.5,
+            zorder=3,
+        )
+        options.update(kwargs)
+
+        j = np.arange(singular_values.size + 1)
+        ax.plot(j, energy, **options)
         ax.set_xlim(0, j.size)
-        for xi, r in zip(thresh, ranks):
-            ax.axhline(xi, color="black", linewidth=0.5, alpha=0.5)
-            ax.axvline(r, color="black", linewidth=0.5, alpha=0.5)
+        ylim = (ax.get_ylim()[0], 1.05)
+        if right:
+            right = min(right, j.size)
+            ax.set_xlim(right=right)
+
+        if threshold:
+            rborder = ax.get_xlim()[1]
+            for kappa, r in zip(threshold, ranks):
+                ax.axhline(kappa, color="gray", linewidth=0.5)
+                ax.text(
+                    rborder - 0.5,
+                    kappa + 0.01,
+                    f"{kappa:%}",
+                    color="gray",
+                    horizontalalignment="right",
+                    verticalalignment="bottom",
+                )
+                ax.axvline(r, color="gray", linewidth=0.5)
+                ax.text(
+                    r + 0.5,
+                    ylim[0] + 0.01,
+                    f"r = {r}",
+                    color="gray",
+                    horizontalalignment="left",
+                    verticalalignment="bottom",
+                )
+
+        ax.set_ylim(ylim)
         ax.set_xlabel(r"Singular value index")
         ax.set_ylabel(r"Cumulative energy")
 
-    return ranks[0] if one_thresh else ranks
+    if threshold:
+        return ranks[0] if one_threshold else ranks
 
 
-def residual_energy(singular_values, tol=1e-6, plot=True, ax=None):
-    """Compute the number of singular values needed such that the residual
-    energy drops beneath the given tolerance. The residual energy of j
-    singular values is defined by
+def residual_energy(
+    singular_values,
+    threshold: float = 1e-6,
+    plot: bool = True,
+    right=None,
+    ax=None,
+    **kwargs,
+):
+    r"""Compute the number of singular values needed such that the residual
+    energy drops beneath a given threshold.
+
+    The residual energy of :math:`r` singular values is defined by
+
+    .. math::
+        \epsilon_r
+        = \sum_{i=r+1}^k\sigma_i^2 \bigg/ \sum_{j=1}^k\sigma_j^2
+        = 1 - \left(
+        \sum_{i=1}^r\sigma_i^2 \bigg/ \sum_{j=1}^k\sigma_j^2
+        \right)
 
-        residual_j = 1 - sum(singular_values[:j]**2) / sum(singular_values**2).
+    This function determines the smallest :math:`r` such that
+    :math:`\epsilon_r \le` ``threshold``.
 
     Parameters
     ----------
     singular_values : (n,) ndarray
-        Singular values of a snapshot set, e.g., scipy.linalg.svdvals(states).
-    tol : float or list(float)
-        Energy residual tolerance(s). Default is 10^-6.
+        Singular values of a snapshot matrix, e.g.,
+        ``scipy.linalg.svdvals(states)``.
+    threshold : float or list[floats]
+        Energy residual threshold(s). Default is 10^-6.
     plot : bool
-        If True, plot the singular values and the residual energy against
-        the singular value index (log scale).
+        If ``True``, plot the residual energy and the threshold(s)
+        against the singular value index.
+    right : int or None
+        Maximum singular value index to plot (``plt.xlim(right=right)``).
     ax : plt.Axes or None
-        Matplotlib Axes to plot the results on if plot = True.
+        Axes to plot the results on if ``plot=True``.
         If not given, a new single-axes figure is created.
+    kwargs : dict
+        Options to pass to ``plt.semilogy()``
 
     Returns
     -------
-    ranks : int or list(int)
-        Number of singular values required to for the residual energy to drop
-        beneath each tolerance.
+    ranks : int or list[int]
+        Number of singular values required to shrink the residual energy below
+        the specified threshold.
     """
     # Calculate the residual energy.
     svdvals2 = np.sort(singular_values)[::-1] ** 2
     res_energy = 1 - (np.cumsum(svdvals2) / np.sum(svdvals2))
+    res_energy = np.concatenate(([1], res_energy))
 
-    # Determine the points when the residual energy dips under the tolerance.
-    one_tol = np.isscalar(tol)
-    if one_tol:
-        tol = [tol]
-    ranks = [np.count_nonzero(res_energy > epsilon) + 1 for epsilon in tol]
+    # Determine the points when the residual energy dips under the threshold.
+    if threshold:
+        if one_threshold := np.isscalar(threshold):
+            threshold = [threshold]
+        ranks = [np.count_nonzero(res_energy > eps) for eps in threshold]
 
     if plot:
-        # Visualize residual energy and tolerance value(s).
+        # Plot residual energy and threshold value(s).
         if ax is None:
             ax = plt.figure().add_subplot(111)
-        j = np.arange(1, singular_values.size + 1)
-        ax.semilogy(j, res_energy, "C1.-", ms=10, lw=1, zorder=3)
-        ax.set_xlim(0, j.size)
-        for epsilon, r in zip(tol, ranks):
-            ax.axhline(epsilon, color="black", linewidth=0.5, alpha=0.5)
-            ax.axvline(r, color="black", linewidth=0.5, alpha=0.5)
-        ax.set_xlabel(r"Singular value index")
-        ax.set_ylabel(r"Residual energy")
-
-    return ranks[0] if one_tol else ranks
-
-
-def projection_error(states, basis):
-    """Calculate the absolute and relative projection errors induced by
-    projecting states to a low dimensional basis, i.e.,
 
-        absolute_error = ||Q - Vr Vr^T Q||_F,
-        relative_error = ||Q - Vr Vr^T Q||_F / ||Q||_F
+        options = dict(
+            linestyle="-",
+            marker="s",
+            color="C1",
+            markersize=4,
+            markeredgewidth=0,
+            linewidth=0.5,
+            zorder=3,
+        )
+        options.update(kwargs)
 
-    where Q = states and Vr = basis. Note that Vr Vr^T is the orthogonal
-    projector onto subspace of R^n defined by the basis.
+        j = np.arange(singular_values.size + 1)
+        ax.semilogy(j, res_energy, **options)
+        ax.set_xlim(0, j.size)
+        bottom = res_energy[-2]
+        if right:
+            right = min(right, j.size)
+            ax.set_xlim(right=right)
+            bottom = res_energy[min(int(right) + 1, res_energy.size - 3)]
+        bottom = max(bottom, 1e-17)
+        ylim = (bottom, 1.1)
+
+        if threshold:
+            rborder = ax.get_xlim()[1]
+            for epsilon, r in zip(threshold, ranks):
+                ax.axhline(epsilon, color="gray", linewidth=0.5)
+                ax.text(
+                    rborder - 0.5,
+                    1.1 * epsilon,
+                    f"{epsilon:.2e}",
+                    color="gray",
+                    horizontalalignment="right",
+                    verticalalignment="bottom",
+                )
+                ax.axvline(r, color="gray", linewidth=0.5)
+                ax.text(
+                    r + 0.5,
+                    1.1 * ylim[0],
+                    f"r = {r}",
+                    color="gray",
+                    horizontalalignment="left",
+                    verticalalignment="bottom",
+                )
 
-    Parameters
-    ----------
-    states : (n, k) or (k,) ndarray
-        Matrix of k snapshots where each column is a single snapshot, or a
-        single 1D snapshot. If 2D, use the Frobenius norm; if 1D, the l2 norm.
-    Vr : (n, r) ndarray
-        Low-dimensional basis of rank r. Each column is one basis vector.
+        ax.set_ylim(ylim)
+        ax.set_xlabel(r"Singular value index")
+        ax.set_ylabel(r"Residual energy")
 
-    Returns
-    -------
-    absolute_error : float
-        Absolute projection error ||Q - Vr Vr^T Q||_F.
-    relative_error : float
-        Relative projection error ||Q - Vr Vr^T Q||_F / ||Q||_F.
-    """
-    norm_of_states = la.norm(states)
-    absolute_error = la.norm(states - basis @ (basis.T @ states))
-    return absolute_error, absolute_error / norm_of_states
+    if threshold:
+        return ranks[0] if one_threshold else ranks
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `opinf-0.5.1/src/opinf/ddt/_finite_difference.py` & `opinf-0.5.2/src/opinf/ddt/_finite_difference.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.1/src/opinf/errors.py` & `opinf-0.5.2/src/opinf/errors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # errors.py
 """Custom exception classes."""
 
 
-class DimensionalityError(Exception):  # pragma: no cover
+class DimensionalityError(ValueError):  # pragma: no cover
     """Dimension of data not aligned with previous model information."""
 
     pass
 
 
 class LoadfileFormatError(Exception):  # pragma: no cover
     """File format inconsistent with a loading routine."""
 
     pass
 
 
-class VerificationError(Exception):  # pragma: no cover
+class VerificationError(RuntimeError):  # pragma: no cover
     """Implementation of a template fails to meet requriements."""
 
     pass
 
 
-class UsageWarning(Warning):  # pragma: no cover
+class UsageWarning(UserWarning):  # pragma: no cover
     """Generic warning for package usage."""
 
     pass
```

### Comparing `opinf-0.5.1/src/opinf/lift/_base.py` & `opinf-0.5.2/src/opinf/lift/_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # lift/_base.py
-"""Template class for lifting transformation managers."""
+"""Template class for lifting transformations."""
 
 __all__ = [
     "LifterTemplate",
 ]
 
 import abc
 import numpy as np
 import scipy.linalg as la
 
 from .. import errors, ddt
 
 
 class LifterTemplate(abc.ABC):
-    """Template class for lifting transformation managers.
+    """Template class for lifting transformations.
 
     Classes that inherit from this template must implement the methods
-    :meth:`lift` and :meth:`unlift`, and may also choose to implement
-    :meth:`lift_ddts`.
+    :meth:`lift()` and :meth:`unlift()`. The optional :meth:`lift_ddts` method
+    is used by the ROM class when snapshot time derivative data are available
+    in the native state variables.
 
     See :class:`QuadraticLifter` for an example.
     """
 
     @staticmethod
     @abc.abstractmethod
     def lift(states):  # pragma: no cover
@@ -131,12 +132,12 @@
                 f"!= lift(states).shape = {shape2}"
             )
         lddts_est = ddt.ddt(lifted_states, t)
         if (
             diff := la.norm(lifted_ddts - lddts_est) / la.norm(lddts_est)
         ) > tol:
             raise errors.VerificationError(
-                "ddts_lifted() failed finite difference check,\n\t"
+                "lift_ddts() failed finite difference check,\n\t"
                 "|| lift_ddts(states, d/dt[states]) - d/dt[lift(states)] || "
                 f" / || d/dt[lift(states)] || = {diff} > {tol = }"
             )
         print("lift() and lift_ddts() are consistent")
```

### Comparing `opinf-0.5.1/src/opinf/lift/_polynomial.py` & `opinf-0.5.2/src/opinf/lift/_polynomial.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.1/src/opinf/lstsq/__init__.py` & `opinf-0.5.2/src/opinf/lstsq/__init__.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.1/src/opinf/lstsq/_base.py` & `opinf-0.5.2/src/opinf/lstsq/_base.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.1/src/opinf/lstsq/_tikhonov.py` & `opinf-0.5.2/src/opinf/lstsq/_tikhonov.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.1/src/opinf/lstsq/_total.py` & `opinf-0.5.2/src/opinf/lstsq/_total.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.1/src/opinf/models/mono/_base.py` & `opinf-0.5.2/src/opinf/models/mono/_base.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.1/src/opinf/models/mono/_nonparametric.py` & `opinf-0.5.2/src/opinf/models/mono/_nonparametric.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.1/src/opinf/models/mono/_parametric.py` & `opinf-0.5.2/src/opinf/models/mono/_parametric.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.1/src/opinf/operators/_base.py` & `opinf-0.5.2/src/opinf/operators/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,40 +4,21 @@
 __all__ = [
     "is_nonparametric",
     "has_inputs",
     "is_parametric",
 ]
 
 import abc
-import functools
 import numpy as np
 import scipy.sparse as sparse
 
-from .. import errors
-from ..utils import hdf5_savehandle, hdf5_loadhandle
+from .. import errors, utils
 
 
 # Nonparametric operators =====================================================
-def _requires_entries(func):
-    """Wrapper for Operator methods that require the ``entries`` attribute
-    to be initialized first through ``set_entries()``.
-    """
-
-    @functools.wraps(func)
-    def _decorator(self, *args, **kwargs):
-        if self.entries is None:
-            raise AttributeError(
-                "operator entries have not been set, "
-                "call set_entries() first"
-            )
-        return func(self, *args, **kwargs)
-
-    return _decorator
-
-
 class _NonparametricOperator(abc.ABC):
     """Base class for operators that do not depend on external parameters.
 
     Child classes:
 
     * :class:`opinf.operators.ConstantOperator`
     * :class:`opinf.operators.LinearOperator`
@@ -167,15 +148,15 @@
 
         Returns
         -------
         (r,) ndarray
         """
         raise NotImplementedError
 
-    @_requires_entries
+    @utils.requires("entries")
     def jacobian(self, state, input_=None):  # pragma: no cover
         r"""Construct the state Jacobian of the operator.
 
         If :math:`[\![\q]\!]_{i}` denotes the entry :math:`i` of a vector
         :math:`\q`, then the entries of the state Jacobian are given by
 
         .. math::
@@ -205,15 +186,15 @@
     def galerkin(self, Vr, Wr, func):
         r"""Get the (Petrov-)Galerkin projection of this operator.
 
         Subclasses may implement this function as follows:
 
         .. code-block:: python
 
-           @_requires_entries
+           @utils.requires("entries")
            def galerkin(self, Vr, Wr=None):
                '''Docstring'''
                return _NonparametricOperator.galerkin(self, Vr, Wr,
                    lambda A, V, W:  # compute Galerkin projection of A.
                )
 
         Parameters
@@ -316,30 +297,30 @@
         ----------
         savefile : str
             Path of the file to save the basis in.
         overwrite : bool
             If ``True``, overwrite the file if it already exists. If ``False``
             (default), raise a ``FileExistsError`` if the file already exists.
         """
-        with hdf5_savehandle(savefile, overwrite) as hf:
+        with utils.hdf5_savehandle(savefile, overwrite) as hf:
             meta = hf.create_dataset("meta", shape=(0,))
             meta.attrs["class"] = self.__class__.__name__
             if self.entries is not None:
                 hf.create_dataset("entries", data=self.entries)
 
     @classmethod
     def load(cls, loadfile: str):
         """Load an operator from an HDF5 file.
 
         Parameters
         ----------
         loadfile : str
             Path to the file where the operator was stored via :meth:`save()`.
         """
-        with hdf5_loadhandle(loadfile) as hf:
+        with utils.hdf5_loadhandle(loadfile) as hf:
             if (ClassName := hf["meta"].attrs["class"]) != cls.__name__:
                 raise TypeError(
                     f"file '{loadfile}' contains '{ClassName}' "
                     f"object, use '{ClassName}.load()"
                 )
             return cls(hf["entries"][:] if "entries" in hf else None)
```

### Comparing `opinf-0.5.1/src/opinf/operators/_interpolate.py` & `opinf-0.5.2/src/opinf/operators/_interpolate.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import warnings
 import numpy as np
 import scipy.linalg as la
 import scipy.interpolate as spinterp
 
 from .. import errors, utils
-from ._base import _ParametricOperator, _InputMixin, _requires_entries
+from ._base import _ParametricOperator, _InputMixin
 from ._nonparametric import (
     ConstantOperator,
     LinearOperator,
     QuadraticOperator,
     CubicOperator,
     InputOperator,
     StateInputOperator,
@@ -335,15 +335,15 @@
         if self.entries is not None:
             if self.shape != other.shape:
                 return False
             return np.allclose(self.entries, other.entries)
         return True
 
     # Evaluation --------------------------------------------------------------
-    @_requires_entries
+    @utils.requires("entries")
     def evaluate(self, parameter):
         r"""Evaluate the operator at the given parameter value,
         :math:`\Ophat_{\ell}(\cdot,\cdot;\bfmu)`.
 
         Parameters
         ----------
         parameter : (p,) ndarray or float
@@ -354,15 +354,15 @@
         op : :mod:`opinf.operators` operator of type ``OperatorClass``.
             Nonparametric operator corresponding to the parameter value.
         """
         self._check_parametervalue_dimension(parameter)
         return self.OperatorClass(self.interpolator(parameter))
 
     # Dimensionality reduction ------------------------------------------------
-    @_requires_entries
+    @utils.requires("entries")
     def galerkin(self, Vr, Wr=None):
         r"""Project this operator to a low-dimensional linear space.
 
         Consider an interpolatory operator
 
         .. math::
            \f_\ell(\q,\u;\bfmu)
```

### Comparing `opinf-0.5.1/src/opinf/operators/_nonparametric.py` & `opinf-0.5.2/src/opinf/operators/_nonparametric.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 ]
 
 import itertools
 import numpy as np
 import scipy.linalg as la
 import scipy.special as special
 
-from ._base import _requires_entries, _NonparametricOperator, _InputMixin
+from .. import utils
+from ._base import _NonparametricOperator, _InputMixin
 
 
 # No dependence on state or input =============================================
 class ConstantOperator(_NonparametricOperator):
     r"""Constant operator :math:`\Ophat_{\ell}(\qhat,\u) = \chat \in \RR^{r}`.
 
     Parameters
@@ -63,15 +64,15 @@
             else:
                 raise ValueError(
                     "ConstantOperator entries must be one-dimensional"
                 )
 
         _NonparametricOperator.set_entries(self, entries)
 
-    @_requires_entries
+    @utils.requires("entries")
     def apply(self, state=None, input_=None):
         r"""Apply the operator to the given state / input:
         :math:`\Ophat_{\ell}(\qhat,\u) = \chat`.
 
         Parameters
         ----------
         state : (r,) ndarray or None
@@ -90,15 +91,15 @@
             return np.full_like(state, self.entries[0])  # r = 1, k > 1.
         # if state is None or np.ndim(state) == 1:
         #     return self.entries
         if np.ndim(state) == 2:  # r, k > 1.
             return np.outer(self.entries, np.ones(state.shape[-1]))
         return self.entries  # r > 1, k = 1.
 
-    @_requires_entries
+    @utils.requires("entries")
     def galerkin(self, Vr, Wr=None):
         r"""Return the Galerkin projection of the operator,
         :math:`\chat = \Wr\trp\c`.
 
         Parameters
         ----------
         Vr : (n, r) ndarray
@@ -209,15 +210,15 @@
         if entries.ndim != 2:
             raise ValueError("LinearOperator entries must be two-dimensional")
         if entries.shape[0] != entries.shape[1]:
             raise ValueError("LinearOperator entries must be square (r x r)")
 
         _NonparametricOperator.set_entries(self, entries)
 
-    @_requires_entries
+    @utils.requires("entries")
     def apply(self, state, input_=None):
         r"""Apply the operator to the given state / input:
         :math:`\Ophat_{\ell}(\qhat,\u) = \Ahat\qhat`.
 
         Parameters
         ----------
         state : (r,) ndarray
@@ -230,15 +231,15 @@
         out : (r,) ndarray
             Application :math:`\Ahat\qhat`.
         """
         if self.entries.shape[0] == 1:
             return self.entries[0, 0] * state  # r = 1.
         return self.entries @ state  # r > 1.
 
-    @_requires_entries
+    @utils.requires("entries")
     def jacobian(self, state=None, input_=None):
         r"""Construct the state Jacobian of the operator:
         :math:`\ddqhat\Ophat_{\ell}(\qhat,\u)=\Ahat`.
 
         Parameters
         ----------
         state : (r,) ndarray or None
@@ -249,15 +250,15 @@
         Returns
         -------
         jac : (r, r) ndarray
             State Jacobian :math:`\Ahat`.
         """
         return self.entries
 
-    @_requires_entries
+    @utils.requires("entries")
     def galerkin(self, Vr, Wr=None):
         r"""Return the Galerkin projection of the operator,
         :math:`\Ahat =
         \Wr\trp\A\Vr`.
 
         Parameters
         ----------
@@ -399,15 +400,15 @@
 
         # Precompute compressed Kronecker product mask and Jacobian matrix.
         self._mask = self.ckron_indices(r)
         self._prejac = None
 
         _NonparametricOperator.set_entries(self, entries)
 
-    @_requires_entries
+    @utils.requires("entries")
     def apply(self, state, input_=None):
         r"""Apply the operator to the given state / input:
         :math:`\Ophat_{\ell}(\qhat,\u) = \Hhat[\qhat\otimes\qhat]`
 
         Parameters
         ----------
         state : (r,) ndarray
@@ -420,15 +421,15 @@
         out : (r,) ndarray
             Application :math:`\Hhat[\qhat\otimes\qhat]`.
         """
         if self.entries.shape[0] == 1:
             return self.entries[0, 0] * state**2  # r = 1
         return self.entries @ np.prod(state[self._mask], axis=1)
 
-    @_requires_entries
+    @utils.requires("entries")
     def jacobian(self, state, input_=None):
         r"""Construct the state Jacobian of the operator:
         :math:`\ddqhat\Ophat_{\ell}(\qhat,\u)
         = \Hhat[(\I_r\otimes\qhat) + (\qhat\otimes\I_r)]`.
 
         Parameters
         ----------
@@ -443,15 +444,15 @@
             State Jacobian
             :math:`\Hhat[(\I_r\otimes\qhat) + (\qhat\otimes\I_r)]`.
         """
         if self._prejac is None:
             self._precompute_jacobian_jit()
         return self._prejac @ np.atleast_1d(state)
 
-    @_requires_entries
+    @utils.requires("entries")
     def galerkin(self, Vr, Wr=None):
         r"""Return the (Petrov-)Galerkin projection of the operator,
         :math:`\Hhat = \Wr\trp\H(\Vr\otimes\Vr)`.
 
         Parameters
         ----------
         Vr : (n, r) ndarray
@@ -853,15 +854,15 @@
 
         # Precompute compressed Kronecker product mask and Jacobian tensor.
         self._mask = self.ckron_indices(r)
         self._prejac = None
 
         _NonparametricOperator.set_entries(self, entries)
 
-    @_requires_entries
+    @utils.requires("entries")
     def apply(self, state, input_=None):
         r"""Apply the operator to the given state / input:
         :math:`\Ophat_{\ell}(\qhat,\u) = \Ghat[\qhat\otimes\qhat\otimes\qhat]`.
 
         Parameters
         ----------
         state : (r,) ndarray
@@ -874,15 +875,15 @@
         out : (r,) ndarray
             The evaluation :math:`\Ghat[\qhat\otimes\qhat\otimes\qhat]`.
         """
         if self.entries.shape[0] == 1:
             return self.entries[0, 0] * state**3  # r = 1.
         return self.entries @ np.prod(state[self._mask], axis=1)
 
-    @_requires_entries
+    @utils.requires("entries")
     def jacobian(self, state, input_=None):
         r"""Construct the state Jacobian of the operator:
         :math:`\ddqhat\Ophat_{\ell}(\qhat,\u)
         = \Ghat[(\I_r\otimes\qhat\otimes\qhat)
         + (\qhat\otimes\I_r\otimes\qhat)
         + (\qhat\otimes\qhat\otimes\I_r)]`.
 
@@ -902,15 +903,15 @@
             + (\qhat\otimes\qhat\otimes\I_r)]`.
         """
         if self._prejac is None:
             self._precompute_jacobian_jit()
         q_ = np.atleast_1d(state)
         return (self._prejac @ q_) @ q_
 
-    @_requires_entries
+    @utils.requires("entries")
     def galerkin(self, Vr, Wr=None):
         r"""Return the Galerkin projection of the operator,
         :math:`\widehat{\mathbf{G}} =
         \Wr\trp\mathbf{G}
         (\Vr\otimes\Vr\otimes\Vr)`.
 
         Parameters
@@ -1273,15 +1274,15 @@
             # Assumes r = entries.size, m = 1.
             entries = entries.reshape((-1, 1))
         if entries.ndim != 2:
             raise ValueError("InputOperator entries must be two-dimensional")
 
         _NonparametricOperator.set_entries(self, entries)
 
-    @_requires_entries
+    @utils.requires("entries")
     def apply(self, state, input_):
         r"""Apply the operator to the given state / input:
         :math:`\Ophat_{\ell}(\qhat,\u) = \Bhat\u`.
 
         Parameters
         ----------
         state : (r,) ndarray
@@ -1298,15 +1299,15 @@
             if self.entries.shape[0] == 1:
                 return self.entries[0, 0] * input_  # r = m = 1.
             if dim == 1 and input_.size > 1:  # r, k > 1, m = 1.
                 return np.outer(self.entries[:, 0], input_)
             return self.entries[:, 0] * input_  # r > 1, m = k = 1.
         return self.entries @ input_  # m > 1.
 
-    @_requires_entries
+    @utils.requires("entries")
     def galerkin(self, Vr, Wr=None):
         r"""Return the Galerkin projection of the operator,
         :math:`\Bhat =
         \Wr\trp\B`.
 
         Parameters
         ----------
@@ -1431,15 +1432,15 @@
         r, rm = entries.shape
         m = rm // r
         if rm != r * m:
             raise ValueError("invalid StateInputOperator entries dimensions")
 
         _NonparametricOperator.set_entries(self, entries)
 
-    @_requires_entries
+    @utils.requires("entries")
     def apply(self, state, input_):
         r"""Apply the operator to the given state / input:
         :math:`\Ophat_{\ell}(\qhat,\u) = \Nhat[\u\otimes\qhat]`.
 
         Parameters
         ----------
         state : (r,) ndarray
@@ -1463,15 +1464,15 @@
             return self.entries[0, 0] * input_ * state  # r = m = 1.
         if single:
             return self.entries @ np.kron(input_, state)  # k = 1, rm > 1.
         Q_ = np.atleast_2d(state)
         U = np.atleast_2d(input_)
         return self.entries @ la.khatri_rao(U, Q_)  # k > 1, rm > 1.
 
-    @_requires_entries
+    @utils.requires("entries")
     def jacobian(self, state, input_):
         r"""Construct the state Jacobian of the operator:
         :math:`\ddqhat\Ophat_{\ell}(\qhat,\u) = \sum_{i=1}^{m}u_{i}\Nhat_{i}`
         where :math:`\Nhat=[~\Nhat_{1}~~\cdots~~\Nhat_{m}~]`
         and each :math:`\Nhat_i\in\RR^{r\times r},~i=1,\ldots,m`.
 
         Parameters
@@ -1492,15 +1493,15 @@
         if u.shape[0] != m:
             raise ValueError("invalid input_ shape")
         return np.sum(
             [um * Nm for um, Nm in zip(u, np.split(self.entries, m, axis=1))],
             axis=0,
         )
 
-    @_requires_entries
+    @utils.requires("entries")
     def galerkin(self, Vr, Wr=None):
         r"""Return the Galerkin projection of the operator,
         :math:`\widehat{\mathbf{N}} =
         \Wr\trp\mathbf{N}
         (\I_{m}\otimes\Vr)`.
 
         Parameters
```

### Comparing `opinf-0.5.1/src/opinf/post/_errors.py` & `opinf-0.5.2/src/opinf/post/_errors.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # post/_errors.py
 """Tools for accuracy and error evaluation."""
 
 __all__ = [
-            "projection_error",
-            "frobenius_error",
-            "lp_error",
-            "Lp_error",
-          ]
+    "projection_error",
+    "frobenius_error",
+    "lp_error",
+    "Lp_error",
+]
 
 import numpy as np
 from scipy import linalg as la
 
-from ..basis import projection_error
-
 
 def _absolute_and_relative_error(Qtrue, Qapprox, norm):
     """Compute the absolute and relative errors between Qtrue and Qapprox,
     where Qapprox approximates Qtrue:
 
         absolute_error = ||Qtrue - Qapprox||,
         relative_error = ||Qtrue - Qapprox|| / ||Qtrue||
@@ -25,14 +23,43 @@
     with ||Q|| defined by norm(Q).
     """
     norm_of_data = norm(Qtrue)
     absolute_error = norm(Qtrue - Qapprox)
     return absolute_error, absolute_error / norm_of_data
 
 
+def projection_error(states, basis):
+    """Calculate the absolute and relative projection errors induced by
+    projecting states to a low dimensional basis, i.e.,
+
+        absolute_error = ||Q - Vr Vr^T Q||_F,
+        relative_error = ||Q - Vr Vr^T Q||_F / ||Q||_F
+
+    where Q = states and Vr = basis. Note that Vr Vr^T is the orthogonal
+    projector onto subspace of R^n defined by the basis.
+
+    Parameters
+    ----------
+    states : (n, k) or (k,) ndarray
+        Matrix of k snapshots where each column is a single snapshot, or a
+        single 1D snapshot. If 2D, use the Frobenius norm; if 1D, the l2 norm.
+    Vr : (n, r) ndarray
+        Low-dimensional basis of rank r. Each column is one basis vector.
+
+    Returns
+    -------
+    absolute_error : float
+        Absolute projection error ||Q - Vr Vr^T Q||_F.
+    relative_error : float
+        Relative projection error ||Q - Vr Vr^T Q||_F / ||Q||_F.
+    """
+    Qapprox = basis @ (basis.T @ states)
+    return _absolute_and_relative_error(states, Qapprox, la.norm)
+
+
 def frobenius_error(Qtrue, Qapprox):
     """Compute the absolute and relative Frobenius-norm errors between the
     snapshot sets Qtrue and Qapprox, where Qapprox approximates Qtrue:
 
         absolute_error = ||Qtrue - Qapprox||_F,
         relative_error = ||Qtrue - Qapprox||_F / ||Qtrue||_F.
 
@@ -55,16 +82,17 @@
     # Check dimensions.
     if Qtrue.shape != Qapprox.shape:
         raise ValueError("Qtrue and Qapprox not aligned")
     if Qtrue.ndim != 2:
         raise ValueError("Qtrue and Qapprox must be two-dimensional")
 
     # Compute the errors.
-    return _absolute_and_relative_error(Qtrue, Qapprox,
-                                        lambda Z: la.norm(Z, ord="fro"))
+    return _absolute_and_relative_error(
+        Qtrue, Qapprox, lambda Z: la.norm(Z, ord="fro")
+    )
 
 
 def lp_error(Qtrue, Qapprox, p=2, normalize=False):
     """Compute the absolute and relative lp-norm errors between the snapshot
     sets Qtrue and Qapprox, where Qapprox approximates to Qtrue:
 
         absolute_error_j = ||Qtrue_j - Qapprox_j||_p,
@@ -181,15 +209,15 @@
             raise ValueError("time t required for p < infinty")
         if t.ndim != 1:
             raise ValueError("time t must be one-dimensional")
         if Qtrue.shape[-1] != t.shape[0]:
             raise ValueError("Qtrue not aligned with time t")
 
         def pnorm(Z):
-            return (np.trapz(np.sum(np.abs(Z)**p, axis=0), t))**(1/p)
+            return (np.trapz(np.sum(np.abs(Z) ** p, axis=0), t)) ** (1 / p)
 
     else:  # p == np.inf
 
         def pnorm(Z):
             return np.max(np.abs(Z), axis=0).max()
 
     # Compute the error.
```

### Comparing `opinf-0.5.1/src/opinf/roms/_nonparametric.py` & `opinf-0.5.2/src/opinf/roms/_nonparametric.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.1/src/opinf/utils/_hdf5.py` & `opinf-0.5.2/src/opinf/utils/_hdf5.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,21 +78,21 @@
     Parameters
     ----------
     savefile : str of h5py File/Group handle
         * str : Name of the file to save to.
         * h5py File/Group handle : handle to part of an already open HDF5 file
           to save data to.
     overwrite : bool
-        If ``True``, overwrite the file if it already exists. If ``False``,
-        raise a ``FileExistsError`` if the file already exists.
+        If ``True``, overwrite the file if it already exists.
+        If ``False``, raise a ``FileExistsError`` if the file already exists.
 
     Examples
     --------
-    >>> with hdf5_savehandle("file_to_save_to.h5") as hf:
-    ...     hf.create_dataset(...)
+    >>> with hdf5_savehandle("file_to_save_to.h5", False) as hf:
+    ...     hf.create_dataset("dataset_label", data=dataset_to_save)
     """
 
     def __init__(self, savefile, overwrite):
         return _hdf5_filehandle.__init__(self, savefile, "save", overwrite)
 
 
 class hdf5_loadhandle(_hdf5_filehandle):
@@ -104,15 +104,15 @@
         * str : Name of the file to read from.
         * h5py File/Group handle : handle to part of an already open HDF5 file
           to read data from.
 
     Examples
     --------
     >>> with hdf5_loadhandle("file_to_read_from.h5") as hf:
-    ...    data = hf[...]
+    ...    dataset = hf["dataset_label"][:]
     """
 
     def __init__(self, loadfile):
         return _hdf5_filehandle.__init__(self, loadfile, "load")
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         """Close the file if needed. Raise a LoadfileFormatError if needed."""
```

### Comparing `opinf-0.5.1/src/opinf/utils/_reprojection.py` & `opinf-0.5.2/src/opinf/utils/_reprojection.py`

 * *Files identical despite different names*

### Comparing `opinf-0.5.1/src/opinf.egg-info/PKG-INFO` & `opinf-0.5.2/src/opinf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opinf
-Version: 0.5.1
+Version: 0.5.2
 Summary: Operator Inference for data-driven model reduction of dynamical systems.
 Author-email: Willcox Research Group <kwillcox@oden.utexas.edu>
 Maintainer-email: "Shane A. McQuarrie" <shanemcq@utexas.edu>
 License: MIT License
         
         Copyright (c) 2023 Willcox Research Group
         
@@ -48,15 +48,17 @@
 Provides-Extra: tests
 Requires-Dist: pytest>=6.0.2; extra == "tests"
 Requires-Dist: pytest-cov>=2.12.1; extra == "tests"
 Requires-Dist: black>=23.10.0; extra == "tests"
 Requires-Dist: flake8>=3.9.0; extra == "tests"
 Requires-Dist: pre-commit>=3.5.0; extra == "tests"
 Provides-Extra: docs
+Requires-Dist: bibtexparser>=2.0.0b7; extra == "docs"
 Requires-Dist: chardet>=5.0; extra == "docs"
+Requires-Dist: docutils==0.17.1; extra == "docs"
 Requires-Dist: jupyter-book<0.15.0,>=0.14.0; extra == "docs"
 Requires-Dist: jupyterlab>=4.0.9; extra == "docs"
 Requires-Dist: numpydoc>=1.2; extra == "docs"
 Requires-Dist: pandas>=2.0.3; extra == "docs"
 Requires-Dist: sphinx-design>=0.1.0; extra == "docs"
 Requires-Dist: sphinxcontrib-mermaid>=0.7.1; extra == "docs"
```

### Comparing `opinf-0.5.1/src/opinf.egg-info/SOURCES.txt` & `opinf-0.5.2/src/opinf.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/opinf.egg-info/SOURCES.txt
 src/opinf.egg-info/dependency_links.txt
 src/opinf.egg-info/requires.txt
 src/opinf.egg-info/top_level.txt
 src/opinf/basis/__init__.py
 src/opinf/basis/_base.py
 src/opinf/basis/_linear.py
+src/opinf/basis/_multi.py
 src/opinf/basis/_pod.py
 src/opinf/ddt/__init__.py
 src/opinf/ddt/_finite_difference.py
 src/opinf/lift/__init__.py
 src/opinf/lift/_base.py
 src/opinf/lift/_polynomial.py
 src/opinf/lstsq/__init__.py
@@ -35,14 +36,19 @@
 src/opinf/operators/_base.py
 src/opinf/operators/_interpolate.py
 src/opinf/operators/_nonparametric.py
 src/opinf/post/__init__.py
 src/opinf/post/_errors.py
 src/opinf/pre/__init__.py
 src/opinf/pre/_base.py
+src/opinf/pre/_multi.py
 src/opinf/pre/_shiftscale.py
 src/opinf/roms/__init__.py
 src/opinf/roms/_nonparametric.py
 src/opinf/roms/_parametric.py
 src/opinf/utils/__init__.py
 src/opinf/utils/_hdf5.py
-src/opinf/utils/_reprojection.py
+src/opinf/utils/_mpl_config.py
+src/opinf/utils/_repr.py
+src/opinf/utils/_reprojection.py
+src/opinf/utils/_requires.py
+src/opinf/utils/_timer.py
```

