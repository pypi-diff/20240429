# Comparing `tmp/aeolus-0.4.9.tar.gz` & `tmp/aeolus-24.4.29.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeolus-0.4.9.tar", last modified: Mon Apr 12 13:13:39 2021, max compression
+gzip compressed data, was "aeolus-24.4.29.1.tar", last modified: Mon Apr 29 16:59:54 2024, max compression
```

## Comparing `aeolus-0.4.9.tar` & `aeolus-24.4.29.1.tar`

### file list

```diff
@@ -1,89 +1,126 @@
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.147147 aeolus-0.4.9/
--rw-r--r--   0 ds591     (1000) ds591     (1000)     7652 2019-02-28 17:46:52.000000 aeolus-0.4.9/LICENSE
--rw-r--r--   0 ds591     (1000) ds591     (1000)      209 2020-10-13 09:19:31.000000 aeolus-0.4.9/MANIFEST.in
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     2506 2021-04-12 13:13:39.147147 aeolus-0.4.9/PKG-INFO
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     1164 2020-11-26 21:30:51.000000 aeolus-0.4.9/README.md
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.135147 aeolus-0.4.9/docs/
--rw-r--r--   0 ds591     (1000) ds591     (1000)      605 2020-12-17 13:52:16.000000 aeolus-0.4.9/docs/Makefile
--rw-r--r--   0 ds591     (1000) ds591     (1000)      235 2021-04-12 11:12:49.000000 aeolus-0.4.9/docs/environment.yml
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.135147 aeolus-0.4.9/docs/source/
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.135147 aeolus-0.4.9/docs/source/_static/
--rw-r--r--   0 ds591     (1000) ds591     (1000)     4286 2020-01-03 17:53:42.000000 aeolus-0.4.9/docs/source/_static/favicon.ico
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.139147 aeolus-0.4.9/docs/source/api/
--rw-r--r--   0 ds591     (1000) ds591     (1000)     2222 2021-03-25 11:26:46.000000 aeolus-0.4.9/docs/source/api/calc.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      176 2020-01-02 13:49:09.000000 aeolus-0.4.9/docs/source/api/const.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1371 2020-12-03 19:56:03.000000 aeolus-0.4.9/docs/source/api/coord.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      147 2020-12-03 22:55:06.000000 aeolus-0.4.9/docs/source/api/core.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      558 2020-06-08 17:01:40.000000 aeolus-0.4.9/docs/source/api/index.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      123 2020-09-28 16:49:30.000000 aeolus-0.4.9/docs/source/api/io.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      191 2020-06-08 17:03:16.000000 aeolus-0.4.9/docs/source/api/model.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      415 2020-03-31 22:43:42.000000 aeolus-0.4.9/docs/source/api/plot.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)       53 2019-03-28 16:39:59.000000 aeolus-0.4.9/docs/source/api/region.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      301 2020-11-27 11:29:06.000000 aeolus-0.4.9/docs/source/api/subset.rst
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     5179 2021-04-12 11:13:41.000000 aeolus-0.4.9/docs/source/changelog.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)     7287 2021-01-26 09:58:23.000000 aeolus-0.4.9/docs/source/conf.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)      154 2019-02-28 18:01:29.000000 aeolus-0.4.9/docs/source/contributing.rst
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.139147 aeolus-0.4.9/docs/source/examples/
--rw-r--r--   0 ds591     (1000) ds591     (1000)      305 2019-02-28 18:16:56.000000 aeolus-0.4.9/docs/source/examples/_index_header_rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      726 2020-05-03 14:58:16.000000 aeolus-0.4.9/docs/source/index.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)     2604 2020-11-25 15:56:20.000000 aeolus-0.4.9/docs/source/install.rst
--rw-r--r--   0 ds591     (1000) ds591     (1000)      714 2020-11-26 17:54:26.000000 aeolus-0.4.9/pyproject.toml
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     1936 2021-04-12 13:13:39.147147 aeolus-0.4.9/setup.cfg
--rw-r--r--   0 ds591     (1000) ds591     (1000)      221 2020-10-13 09:13:58.000000 aeolus-0.4.9/setup.py
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.135147 aeolus-0.4.9/src/
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.147147 aeolus-0.4.9/src/aeolus/
--rw-r--r--   0 ds591     (1000) ds591     (1000)      115 2019-02-28 18:19:47.000000 aeolus-0.4.9/src/aeolus/__init__.py
--rw-rw-r--   0 ds591     (1000) ds591     (1000)      497 2021-04-12 13:13:39.147147 aeolus-0.4.9/src/aeolus/_version.py
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.143147 aeolus-0.4.9/src/aeolus/calc/
--rw-r--r--   0 ds591     (1000) ds591     (1000)     2188 2021-03-25 11:24:42.000000 aeolus-0.4.9/src/aeolus/calc/__init__.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     5359 2020-12-03 22:34:03.000000 aeolus-0.4.9/src/aeolus/calc/calculus.py
--rw-rw-r--   0 ds591     (1000) ds591     (1000)    27230 2021-03-29 11:18:53.000000 aeolus-0.4.9/src/aeolus/calc/diag.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     3509 2021-04-01 15:23:03.000000 aeolus-0.4.9/src/aeolus/calc/flux_h.py
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     3618 2021-02-25 16:36:06.000000 aeolus-0.4.9/src/aeolus/calc/meta.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     3115 2019-12-03 15:30:30.000000 aeolus-0.4.9/src/aeolus/calc/metpy.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     9722 2021-04-01 15:36:37.000000 aeolus-0.4.9/src/aeolus/calc/stats.py
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     3952 2020-12-03 20:29:28.000000 aeolus-0.4.9/src/aeolus/calc/tl.py
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.143147 aeolus-0.4.9/src/aeolus/const/
--rw-r--r--   0 ds591     (1000) ds591     (1000)      215 2021-02-23 09:32:46.000000 aeolus-0.4.9/src/aeolus/const/__init__.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     6676 2021-04-01 15:37:01.000000 aeolus-0.4.9/src/aeolus/const/const.py
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.143147 aeolus-0.4.9/src/aeolus/const/store/
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1283 2020-05-19 20:47:52.000000 aeolus-0.4.9/src/aeolus/const/store/earth.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)      738 2020-09-09 19:58:06.000000 aeolus-0.4.9/src/aeolus/const/store/general.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1157 2020-05-01 06:22:57.000000 aeolus-0.4.9/src/aeolus/const/store/proxb.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1297 2020-05-18 10:58:39.000000 aeolus-0.4.9/src/aeolus/const/store/titan.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)      935 2020-01-06 13:38:56.000000 aeolus-0.4.9/src/aeolus/const/store/trap1d.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1158 2020-05-01 06:22:59.000000 aeolus-0.4.9/src/aeolus/const/store/trap1e.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)      934 2020-01-06 13:38:56.000000 aeolus-0.4.9/src/aeolus/const/store/trap1f.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)    32903 2021-04-01 15:37:45.000000 aeolus-0.4.9/src/aeolus/coord.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)    13489 2021-04-12 10:51:39.000000 aeolus-0.4.9/src/aeolus/core.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1410 2021-04-01 15:20:07.000000 aeolus-0.4.9/src/aeolus/exceptions.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     2535 2021-02-23 09:37:14.000000 aeolus-0.4.9/src/aeolus/io.py
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.143147 aeolus-0.4.9/src/aeolus/model/
--rw-r--r--   0 ds591     (1000) ds591     (1000)      128 2020-06-08 16:28:18.000000 aeolus-0.4.9/src/aeolus/model/__init__.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     2545 2021-02-23 19:28:35.000000 aeolus-0.4.9/src/aeolus/model/base.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     5885 2021-02-23 19:28:14.000000 aeolus-0.4.9/src/aeolus/model/um.py
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.143147 aeolus-0.4.9/src/aeolus/plot/
--rw-r--r--   0 ds591     (1000) ds591     (1000)      503 2020-04-28 10:22:32.000000 aeolus-0.4.9/src/aeolus/plot/__init__.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     3505 2020-04-28 10:22:50.000000 aeolus-0.4.9/src/aeolus/plot/cart.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     5517 2021-01-25 21:37:58.000000 aeolus-0.4.9/src/aeolus/plot/cloud.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)    10102 2019-10-29 12:07:06.000000 aeolus-0.4.9/src/aeolus/plot/cm_custom.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1788 2021-04-01 15:16:34.000000 aeolus-0.4.9/src/aeolus/plot/mpl.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     4654 2021-04-01 15:20:58.000000 aeolus-0.4.9/src/aeolus/plot/pv.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1455 2019-10-29 12:08:29.000000 aeolus-0.4.9/src/aeolus/plot/text.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     6644 2020-07-02 14:12:26.000000 aeolus-0.4.9/src/aeolus/region.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     4144 2021-03-31 14:01:54.000000 aeolus-0.4.9/src/aeolus/subset.py
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.139147 aeolus-0.4.9/src/aeolus.egg-info/
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     2506 2021-04-12 13:13:39.000000 aeolus-0.4.9/src/aeolus.egg-info/PKG-INFO
--rw-rw-r--   0 ds591     (1000) ds591     (1000)     1783 2021-04-12 13:13:39.000000 aeolus-0.4.9/src/aeolus.egg-info/SOURCES.txt
--rw-rw-r--   0 ds591     (1000) ds591     (1000)        1 2021-04-12 13:13:39.000000 aeolus-0.4.9/src/aeolus.egg-info/dependency_links.txt
--rw-rw-r--   0 ds591     (1000) ds591     (1000)        1 2021-01-25 21:49:48.000000 aeolus-0.4.9/src/aeolus.egg-info/not-zip-safe
--rw-rw-r--   0 ds591     (1000) ds591     (1000)      108 2021-04-12 13:13:39.000000 aeolus-0.4.9/src/aeolus.egg-info/requires.txt
--rw-rw-r--   0 ds591     (1000) ds591     (1000)        7 2021-04-12 13:13:39.000000 aeolus-0.4.9/src/aeolus.egg-info/top_level.txt
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.147147 aeolus-0.4.9/tests/
-drwxrwxr-x   0 ds591     (1000) ds591     (1000)        0 2021-04-12 13:13:39.147147 aeolus-0.4.9/tests/data/
--rw-r--r--   0 ds591     (1000) ds591     (1000)       94 2019-11-04 10:21:23.000000 aeolus-0.4.9/tests/data/dummy.json
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1278 2020-08-28 21:13:15.000000 aeolus-0.4.9/tests/test_calc.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1893 2021-02-25 16:18:02.000000 aeolus-0.4.9/tests/test_const.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)     1980 2021-02-25 16:15:37.000000 aeolus-0.4.9/tests/test_coord.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)      551 2019-11-21 10:24:28.000000 aeolus-0.4.9/tests/test_core.py
--rw-r--r--   0 ds591     (1000) ds591     (1000)    68611 2019-02-28 18:05:47.000000 aeolus-0.4.9/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.981552 aeolus-24.4.29.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.961552 aeolus-24.4.29.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.965552 aeolus-24.4.29.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/.github/workflows/pypipublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-04-29 16:59:54.981552 aeolus-24.4.29.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.965552 aeolus-24.4.29.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.965552 aeolus-24.4.29.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.965552 aeolus-24.4.29.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.969552 aeolus-24.4.29.1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/api/calc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/api/const.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/api/coord.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/api/core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/api/io.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/api/lfric.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/api/log.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/api/model.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/api/plot.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/api/proc_um_output.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/api/region.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/api/subset.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/api/synthobs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.969552 aeolus-24.4.29.1/docs/source/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/examples/_index_header_rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2625 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/docs/source/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.969552 aeolus-24.4.29.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    14225 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/examples/00_Constants.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9965 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/examples/01_Loading_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/examples/02_Model_Field_Names.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   280121 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/examples/03_Transmission_Spectrum.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   306941 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/examples/04_Rotational_And_Divergent_Winds.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.969552 aeolus-24.4.29.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/requirements/environment-py3.10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/requirements/environment-py3.11.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/requirements/environment-py3.12.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/requirements/pypi-core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:59:54.981552 aeolus-24.4.29.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.961552 aeolus-24.4.29.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.973552 aeolus-24.4.29.1/src/aeolus/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-29 16:59:54.000000 aeolus-24.4.29.1/src/aeolus/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.977552 aeolus-24.4.29.1/src/aeolus/calc/
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/calc/calculus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33269 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/calc/diag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/calc/flux_h.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/calc/metpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/calc/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/calc/tl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.977552 aeolus-24.4.29.1/src/aeolus/const/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/const/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/const/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.977552 aeolus-24.4.29.1/src/aeolus/const/store/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/const/store/earth.json
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/const/store/general.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/const/store/proxb.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/const/store/titan.json
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/const/store/trap1d.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/const/store/trap1e.json
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/const/store/trap1f.json
+-rw-r--r--   0 runner    (1001) docker     (127)    33880 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/coord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/decor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/lfric.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.977552 aeolus-24.4.29.1/src/aeolus/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/model/lfric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/model/um.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.977552 aeolus-24.4.29.1/src/aeolus/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/plot/cart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5875 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/plot/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10103 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/plot/cm_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/plot/mpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5669 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/plot/pv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/plot/text.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5323 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/proc_um_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12713 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/src/aeolus/synthobs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.981552 aeolus-24.4.29.1/src/aeolus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12431 2024-04-29 16:59:54.000000 aeolus-24.4.29.1/src/aeolus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-29 16:59:54.000000 aeolus-24.4.29.1/src/aeolus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:59:54.000000 aeolus-24.4.29.1/src/aeolus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 16:59:54.000000 aeolus-24.4.29.1/src/aeolus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:59:54.000000 aeolus-24.4.29.1/src/aeolus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-29 16:59:54.000000 aeolus-24.4.29.1/src/aeolus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 16:59:54.000000 aeolus-24.4.29.1/src/aeolus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:59:54.981552 aeolus-24.4.29.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5590 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/tests/test_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/tests/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/tests/test_coord.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/tests/test_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-04-29 16:59:43.000000 aeolus-24.4.29.1/tests/test_synthobs.py
```

### Comparing `aeolus-0.4.9/LICENSE` & `aeolus-24.4.29.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.9/docs/Makefile` & `aeolus-24.4.29.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.9/docs/source/_static/favicon.ico` & `aeolus-24.4.29.1/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.9/docs/source/api/index.rst` & `aeolus-24.4.29.1/docs/source/api/index.rst`

 * *Files 8% similar despite different names*

```diff
@@ -17,11 +17,15 @@
    :maxdepth: 1
 
    calc
    core
    const
    coord
    io
+   lfric
+   log
    model
    plot
+   proc_um_output
    region
    subset
+   synthobs
```

### Comparing `aeolus-0.4.9/docs/source/conf.py` & `aeolus-24.4.29.1/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,25 +13,26 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
+import datetime
 import os
 from glob import glob
 
 import aeolus
 
 
 # -- Project information -----------------------------------------------------
 
 project = "aeolus"
-copyright = "2021, the aeolus developers"  # noqa
-author = "The aeolus developers"
+author = f"{project} contributors"
+copyright = f"2020 - {datetime.datetime.now().year}, {author}"
 
 # The short X.Y version
 version = aeolus.__version__
 # The full version, including alpha/beta/rc tags
 release = version
 
 
@@ -47,14 +48,15 @@
 extensions = [
     "sphinx.ext.extlinks",
     "sphinx.ext.intersphinx",
     "sphinx.ext.mathjax",
     "sphinx.ext.viewcode",
     "sphinx.ext.napoleon",
     "nbsphinx",
+    "IPython.sphinxext.ipython_console_highlighting",
 ]
 napoleon_numpy_docstring = True
 napoleon_include_init_with_doc = False
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
@@ -90,15 +92,14 @@
 # a list of builtin themes.
 
 html_theme_path = ["_themes"]
 
 # import sphinx_rtd_theme  # noqa
 html_theme = "sphinx_rtd_theme"
 # html_theme = 'sphinxdoc'
-# html_theme = "sphinx13_aeolus"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
@@ -120,15 +121,15 @@
 # Site icon
 html_favicon = "_static/favicon.ico"
 
 
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = "aeolusdoc"
+htmlhelp_basename = f"{project}doc"
 
 
 # -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
@@ -143,36 +144,44 @@
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
-latex_documents = [(master_doc, "aeolus.tex", "aeolus Documentation", "Denis Sergeev", "manual")]
+latex_documents = [
+    (
+        master_doc,
+        f"{project}.tex",
+        f"{project} Documentation",
+        author,
+        "manual",
+    )
+]
 
 
 # -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [(master_doc, "aeolus", "aeolus Documentation", [author], 1)]
+man_pages = [(master_doc, project, f"{project} Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output ----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
         master_doc,
-        "aeolus",
-        "aeolus Documentation",
-        author,
-        "aeolus",
+        project,
+        f"{project} Documentation",
+        project,
+        project,
         "One line description of project.",
         "Miscellaneous",
     )
 ]
 
 
 # -- Options for Epub output -------------------------------------------------
@@ -195,15 +204,15 @@
 
 # -- Extension configuration -------------------------------------------------
 
 # -- Options for intersphinx extension ---------------------------------------
 # Options for intersphinx.
 intersphinx_mapping = {
     "cartopy": ("https://scitools.org.uk/cartopy/docs/latest/", None),
-    "iris": ("https://scitools.org.uk/iris/docs/latest/", None),
+    "iris": ("https://scitools-iris.readthedocs.io/en/latest/", None),
     "matplotlib": ("https://matplotlib.org", None),
     "mpl_toolkits": ("https://matplotlib.org", None),
     "numpy": ("https://numpy.org/doc/stable", None),
     "python": ("https://docs.python.org/3/", None),
     "pyvista": ("https://docs.pyvista.org/", None),
 }
 nitpick_ignore = [("py:class", "optional"), ("py:class", "array-like")]
```

### Comparing `aeolus-0.4.9/docs/source/install.rst` & `aeolus-24.4.29.1/docs/source/install.rst`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,18 @@
    We highly recommend installing and using the free `Anaconda
    <https://www.anaconda.com/download/>`_ distribution of Python (or
    `Miniconda <https://conda.io/miniconda.html>`_, if you don't want
    all of the extra packages that come built-in with Anaconda), which
    works on Mac, Linux, and Windows, both on normal computers and
    institutional clusters and doesn't require root permissions.
 
-The main dependency of aeolus is `iris <https://scitools.org.uk/iris/docs/latest/>`, but various
+The main dependency of aeolus is `iris <https://scitools.org.uk/iris/docs/latest/>`_, but various
 minor parts also depend on the following Python packages
 
+- cached-property
 - cartopy
 - matplotlib
 - numpy
 - latlon23
 - metpy
 - python-stratify
 - pyvista
@@ -39,51 +40,51 @@
 
 The recommended installation method is via `conda <https://conda.io/docs/>`_
 
 To install aeolus and its primary dependencies ::
 
   conda install -c conda-forge aeolus
 
-To get the latest "nightly" build ::
-
-  conda install -c conda-forge/label/nightly aeolus
-
 Alternative method: PyPI
 ========================
 Install aeolus from the Python Package Index ::
 
   pip install aeolus
 
 
-Alternative method: clone from Github
-=====================================
+Alternative method: install from source
+=======================================
 
-You can also directly clone the `Github repo <https://github.com/exoclim/aeolus>`_ ::
+To get the latest (potentially unstable) version of the library you can directly clone the `GitHub repository <https://github.com/exoclim/aeolus>`_ ::
 
   git clone https://www.github.com/exoclim/aeolus.git
   cd aeolus
 
 and install aeolus in the standard mode ::
 
   python setup.py install
 
 and install aeolus in the developer mode ::
 
   python setup.py develop
 
+or::
+
+  pip install -e .
+
 
 Verifying proper installation
 =============================
 
 Once installed via any of these methods, you can run aeolus's suite of
-tests using `py.test <http://doc.pytest.org/>`_.  From the top-level
+tests using `pytest <http://doc.pytest.org/>`_.  From the top-level
 directory of the aeolus installation ::
 
   conda install pytest  # if you don't have it already; or 'pip install pytest'
-  py.test aeolus
+  pytest aeolus
 
 If you don't know the directory where aeolus was installed, you can find it via ::
 
   python -c "import aeolus; print(aeolus.__path__[0])"
 
 If the pytest command results in any error messages or test failures,
 something has gone wrong, and please refer to the Troubleshooting
```

### Comparing `aeolus-0.4.9/src/aeolus/calc/__init__.py` & `aeolus-24.4.29.1/src/aeolus/calc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 """Calculations."""
+
 from .calculus import d_dx, d_dy, d_dz, deriv, div_h, integrate
 from .diag import (
     air_density,
     air_potential_temperature,
+    air_pressure,
     air_temperature,
     bond_albedo,
+    calc_derived_cubes,
     dry_lapse_rate,
     flux,
     geopotential_height,
     ghe_norm,
+    greenhouse_effect,
     heat_redist_eff,
     horiz_wind_cmpnts,
     meridional_mass_streamfunction,
     precip_sum,
     sfc_net_energy,
     sfc_water_balance,
     sigma_p,
     superrotation_index,
     toa_cloud_radiative_effect,
     toa_eff_temp,
     toa_net_energy,
     water_path,
+    wind_rot_div,
     wind_speed,
     zonal_mass_streamfunction,
 )
-from .flux_h import horizontal_fluxes_through_region_boundaries, net_horizontal_flux_to_region
+from .flux_h import (
+    horizontal_fluxes_through_region_boundaries,
+    net_horizontal_flux_to_region,
+)
 from .stats import (
     abs_coord_mean,
+    after_n_day_mean,
+    between_day_mean,
     cumsum,
     last_n_day_mean,
     meridional_mean,
     minmaxdiff,
     normalize_cube,
     region_mean_diff,
     spatial,
@@ -44,28 +54,33 @@
     regrid_to_rotated_pole_coordinates,
     regrid_to_tidally_locked_coordinates,
     rotate_winds_to_tidally_locked_coordinates,
 )
 
 __all__ = (
     "abs_coord_mean",
+    "after_n_day_mean",
     "air_density",
     "air_potential_temperature",
+    "air_pressure",
     "air_temperature",
+    "between_day_mean",
     "bond_albedo",
+    "calc_derived_cubes",
     "cumsum",
     "d_dx",
     "d_dy",
     "d_dz",
     "deriv",
     "div_h",
     "dry_lapse_rate",
     "flux",
     "geopotential_height",
     "ghe_norm",
+    "greenhouse_effect",
     "heat_redist_eff",
     "horiz_wind_cmpnts",
     "horizontal_fluxes_through_region_boundaries",
     "integrate",
     "last_n_day_mean",
     "meridional_mass_streamfunction",
     "meridional_mean",
@@ -87,11 +102,12 @@
     "superrotation_index",
     "time_mean",
     "toa_cloud_radiative_effect",
     "toa_eff_temp",
     "toa_net_energy",
     "vertical_mean",
     "water_path",
+    "wind_rot_div",
     "wind_speed",
     "zonal_mass_streamfunction",
     "zonal_mean",
 )
```

### Comparing `aeolus-0.4.9/src/aeolus/calc/calculus.py` & `aeolus-24.4.29.1/src/aeolus/calc/calculus.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 """Generic calculus functions."""
-from cf_units import Unit
-
-import iris
-from iris.analysis.calculus import _coord_cos, _curl_differentiate, _curl_regrid, differentiate
 
+from cf_units import Unit
+from iris.analysis import Linear
+from iris.analysis.calculus import (
+    _coord_cos,
+    _curl_differentiate,
+    _curl_regrid,
+    differentiate,
+)
+from iris.analysis.maths import add, divide, multiply
+from iris.coord_systems import GeogCS, RotatedGeogCS
 import numpy as np
 
-from .meta import update_metadata
 from ..const import get_planet_radius
 from ..exceptions import NotYetImplementedError
+from ..meta import update_metadata
 from ..model import um
 
-
 __all__ = (
     "d_dx",
     "d_dy",
     "d_dz",
     "deriv",
     "div_h",
     "integrate",
@@ -52,21 +57,21 @@
         Coordinate for differentiation.
 
     Returns
     -------
     iris.cube.Cube
         d(cube)/d(coord).
 
-    See also
+    See Also
     --------
-    aeolus.calc.calculus.d_dx, aeolus.calc.calculus.d_dy, aeolus.calc.calculus.d_dz
+    aeolus.calc.calculus.d_dx, aeolus.calc.calculus.d_dy
     """
     pnts = cube.coord(coord).points
     diff = differentiate(cube, coord)
-    res = diff.interpolate([(coord, pnts)], iris.analysis.Linear())
+    res = diff.interpolate([(coord, pnts)], Linear())
     return res
 
 
 @update_metadata(name="horizontal_divergence")
 def div_h(i_cube, j_cube, r_planet=None, model=um):
     r"""
     Calculate horizontal divergence.
@@ -93,67 +98,67 @@
     Notes
     -----
     Divergence in spherical coordinates is defined as
 
     .. math::
 
         \nabla\cdot \vec A = \frac{1}{r cos \theta} (
-        \frac{\partial \vec A_\lambda}{\partial \lambda}
+        \frac{\partial A_\lambda}{\partial \lambda}
         + \frac{\partial}{\partial \theta}
-        (\vec A_\theta cos \theta))
+        (A_\theta cos \theta))
 
     where \lambda is longitude, \theta is latitude.
     """
     x_coord = i_cube.coord(model.x)
     y_coord = i_cube.coord(model.y)
 
     y_dim = i_cube.coord_dims(y_coord)[0]
 
     horiz_cs = i_cube.coord_system("CoordSystem")
 
     # Check for spherical coords
-    spherical_coords = isinstance(
-        horiz_cs, (iris.coord_systems.GeogCS, iris.coord_systems.RotatedGeogCS)
-    )
+    spherical_coords = isinstance(horiz_cs, (GeogCS, RotatedGeogCS))
     if spherical_coords:
         # Get the radius of the planet
         if r_planet is None:
             r = get_planet_radius(i_cube)
         else:
             r = r_planet
         r_unit = Unit("m")
 
         lon_coord = x_coord.copy()
         lat_coord = y_coord.copy()
         lon_coord.convert_units("radians")
         lat_coord.convert_units("radians")
         lat_cos_coord = _coord_cos(lat_coord)
 
-        # j-component: \frac{\partial}{\partial \theta} (\vec A_\theta cos \theta))
-        temp = iris.analysis.maths.multiply(j_cube, lat_cos_coord, y_dim)
+        # j-comp: \frac{\partial}{\partial \theta} (\vec A_\theta cos \theta))
+        temp = multiply(j_cube, lat_cos_coord, y_dim)
         djcos_dtheta = _curl_differentiate(temp, lat_coord)
         prototype_diff = djcos_dtheta
 
-        # i-component: \frac{\partial \vec A_\lambda}{\partial \lambda}
+        # i-comp: \frac{\partial \vec A_\lambda}{\partial \lambda}
         d_i_cube_dlambda = _curl_differentiate(i_cube, lon_coord)
         d_i_cube_dlambda = _curl_regrid(d_i_cube_dlambda, prototype_diff)
         new_lat_coord = d_i_cube_dlambda.coord(model.y)
         new_lat_cos_coord = _coord_cos(new_lat_coord)
         lat_dim = d_i_cube_dlambda.coord_dims(new_lat_coord)[0]
 
         # Sum and divide
-        div = iris.analysis.maths.divide(
-            iris.analysis.maths.add(d_i_cube_dlambda, djcos_dtheta),
+        div = divide(
+            add(d_i_cube_dlambda, djcos_dtheta),
             r * new_lat_cos_coord,
             dim=lat_dim,
         )
         div.units /= r_unit
-        div = div.regrid(i_cube, iris.analysis.Linear())
+        div = div.regrid(i_cube, Linear())
     else:
-        raise NotYetImplementedError("Non-spherical coordinates are not implemented yet.")
+        raise NotYetImplementedError(
+            "Non-spherical coordinates are not implemented yet."
+        )
     return div
 
 
 def integrate(cube, coord):
     """
     Integrate the cube along a 1D coordinate using the trapezoidal rule.
 
@@ -169,18 +174,22 @@
     Returns
     -------
     iris.cube.Cube
         Integrated cube.
     """
     # TODO: allow non-dim coordinates
     c = cube.coord(coord)
-    others = [dc.name() for dc in cube.dim_coords if cube.coord_dims(dc) != cube.coord_dims(c)]
+    others = [
+        dc.name()
+        for dc in cube.dim_coords
+        if cube.coord_dims(dc) != cube.coord_dims(c)
+    ]
     dim = cube.coord_dims(c)[0]
     data = np.trapz(cube.data, c.points, axis=dim)
     res = next(cube.slices(others)).copy(data=data)
     res.units = cube.units * c.units
     res.remove_coord(c)
     res.rename(f"integral_of_{cube.name()}_wrt_{c.name()}")
     # ensure_bounds(cube, [c])
-    # delta = iris.coords.AuxCoord(c.bounds[:, 1] - c.bounds[:, 0], units=c.units)
-    # res = iris.analysis.maths.multiply(cube, delta, dim=dim).collapsed(c, iris.analysis.SUM)
+    # delta = AuxCoord(c.bounds[:, 1] - c.bounds[:, 0], units=c.units)
+    # res = multiply(cube, delta, dim=dim).collapsed(c, iris.analysis.SUM)
     return res
```

### Comparing `aeolus-0.4.9/src/aeolus/calc/diag.py` & `aeolus-24.4.29.1/src/aeolus/calc/diag.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 """Some commonly used diagnostics in atmospheric science."""
-from cf_units import Unit
 
+from cf_units import Unit
 from iris.analysis.calculus import _coord_cos
 from iris.analysis.maths import add, apply_ufunc, multiply
 from iris.exceptions import ConstraintMismatchError as ConMisErr
 from iris.util import reverse
-
 import numpy as np
 
-from .calculus import d_dz, integrate
-from .meta import const_from_attrs, update_metadata
-from .stats import cumsum, spatial_mean, time_mean, zonal_mean
 from ..const import init_const
 from ..coord import coord_to_cube, ensure_bounds, regrid_3d
 from ..exceptions import ArgumentError, MissingCubeError
+from ..meta import const_from_attrs, preserve_shape, update_metadata
 from ..model import um
 from ..subset import _dim_constr
-
+from .calculus import d_dz, integrate
+from .stats import cumsum, spatial_mean, time_mean, zonal_mean
 
 __all__ = (
     "air_density",
     "air_potential_temperature",
+    "air_pressure",
     "air_temperature",
     "bond_albedo",
+    "calc_derived_cubes",
     "dry_lapse_rate",
     "flux",
     "geopotential_height",
     "ghe_norm",
+    "greenhouse_effect",
     "heat_redist_eff",
     "horiz_wind_cmpnts",
     "meridional_mass_streamfunction",
     "precip_sum",
     "sfc_net_energy",
     "sfc_water_balance",
     "sigma_p",
     "toa_cloud_radiative_effect",
     "toa_eff_temp",
     "toa_net_energy",
     "water_path",
+    "wind_rot_div",
     "wind_speed",
     "zonal_mass_streamfunction",
 )
 
 
 def _precip_name_mapping(model=um):
     """Generate lists of variable names for `precip_sum()`."""
@@ -71,15 +73,15 @@
     Exner pressure or air pressure, and potential temperature.
 
     Parameters
     ----------
     cubelist: iris.cube.CubeList
         Input list of cubes containing temperature.
     const: aeolus.const.const.ConstContainer, optional
-        Must have `reference_surface_pressure` and `dry_air_gas_constant` as attributes.
+        Must have `reference_surface_pressure` and `dry_air_gas_constant`.
         If not given, an attempt is made to retrieve it from cube attributes.
     model: aeolus.model.Model, optional
         Model class with relevant variable names.
 
     Returns
     -------
     iris.cube.Cube
@@ -87,27 +89,31 @@
     """
     try:
         return cubelist.extract_cube(model.temp)
     except ConMisErr:
         try:
             thta = cubelist.extract_cube(model.thta)
         except ConMisErr:
-            raise MissingCubeError(f"Unable to get air temperature from {cubelist}")
+            raise MissingCubeError(
+                f"Unable to get air temperature from {cubelist}"
+            )
 
         if len(cubelist.extract(model.exner)) == 1:
             exner = cubelist.extract_cube(model.exner)
         elif len(cubelist.extract(model.pres)) == 1:
             if const is None:
                 const = thta.attributes["planet_conf"]
             pres = cubelist.extract_cube(model.pres)
             exner = (pres / const.reference_surface_pressure) ** (
                 const.dry_air_gas_constant / const.dry_air_spec_heat_press
             ).data
         else:
-            raise MissingCubeError(f"Unable to get air temperature from {cubelist}")
+            raise MissingCubeError(
+                f"Unable to get air temperature from {cubelist}"
+            )
         temp = thta * exner
         temp.rename(model.temp)
         return temp
 
 
 @update_metadata(units="K")
 def air_potential_temperature(cubelist, const=None, model=um):
@@ -118,15 +124,15 @@
     Exner pressure or air pressure, and real temperature.
 
     Parameters
     ----------
     cubelist: iris.cube.CubeList
         Input list of cubes containing temperature.
     const: aeolus.const.const.ConstContainer, optional
-        Must have `reference_surface_pressure` and `dry_air_gas_constant` as attributes.
+        Must have `reference_surface_pressure` and `dry_air_gas_constant`.
         If not given, an attempt is made to retrieve it from cube attributes.
     model: aeolus.model.Model, optional
         Model class with relevant variable names.
 
     Returns
     -------
     iris.cube.Cube
@@ -134,39 +140,100 @@
     """
     try:
         return cubelist.extract_cube(model.thta)
     except ConMisErr:
         try:
             temp = cubelist.extract_cube(model.temp)
         except ConMisErr:
-            raise MissingCubeError(f"Unable to get air potential temperature from {cubelist}")
+            raise MissingCubeError(
+                f"Unable to get air potential temperature from {cubelist}"
+            )
 
         if len(cubelist.extract(model.exner)) == 1:
             exner = cubelist.extract_cube(model.exner)
         elif len(cubelist.extract(model.pres)) == 1:
             if const is None:
                 const = temp.attributes["planet_conf"]
             pres = cubelist.extract_cube(model.pres)
             exner = (pres / const.reference_surface_pressure) ** (
                 const.dry_air_gas_constant / const.dry_air_spec_heat_press
             ).data
         else:
-            raise MissingCubeError(f"Unable to get air potential temperature from {cubelist}")
+            raise MissingCubeError(
+                f"Unable to get air potential temperature from {cubelist}"
+            )
         thta = temp / exner
         thta.rename(model.thta)
         thta.convert_units("K")
         return thta
 
 
+@const_from_attrs()
+@update_metadata(units="Pa")
+def air_pressure(cubelist, const=None, model=um):
+    """
+    Get pressure from the given cube list.
+
+    If not present, it is attempted to calculate it from other variables,
+    such as Exner pressure or air potential temperature and real temperature.
+
+    Parameters
+    ----------
+    cubelist: iris.cube.CubeList
+        Input list of cubes containing related variables.
+    const: aeolus.const.const.ConstContainer, optional
+        Must have `reference_surface_pressure` and `dry_air_gas_constant`.
+        If not given, an attempt is made to retrieve it from cube attributes.
+    model: aeolus.model.Model, optional
+        Model class with relevant variable names.
+
+    Returns
+    -------
+    iris.cube.Cube
+        Cube of air pressure.
+    """
+    try:
+        return cubelist.extract_cube(model.pres)
+    except ConMisErr:
+        try:
+            exner = cubelist.extract_cube(model.exner)
+            pres = (
+                const.reference_surface_pressure
+                * exner
+                ** (
+                    const.dry_air_spec_heat_press / const.dry_air_gas_constant
+                ).data
+            )
+        except ConMisErr:
+            try:
+                temp = cubelist.extract_cube(model.temp)
+                thta = cubelist.extract_cube(model.temp)
+                exner = temp / thta
+                pres = (
+                    const.reference_surface_pressure
+                    * exner
+                    ** (
+                        const.dry_air_spec_heat_press
+                        / const.dry_air_gas_constant
+                    ).data
+                )
+            except ConMisErr:
+                raise MissingCubeError(
+                    f"Unable to calculate air pressure from {cubelist}"
+                )
+        pres.rename(model.pres)
+        return pres
+
+
 @update_metadata(units="kg m-3")
 def air_density(cubelist, const=None, model=um):
     """
     Get air density from the given cube list.
 
-    If not present, it is attempted to calculate it from pressure and temperature.
+    If not present, try to calculate it from pressure and temperature.
 
     Parameters
     ----------
     cubelist: iris.cube.CubeList
         Input list of cubes containing temperature.
     const: aeolus.const.const.ConstContainer, optional
         Must have `dry_air_gas_constant` as an attribute.
@@ -187,18 +254,50 @@
             pres = cubelist.extract_cube(model.pres)
             if const is None:
                 const = pres.attributes["planet_conf"]
             rho = pres / (const.dry_air_gas_constant * temp)
             rho.rename(model.dens)
             return rho
         except ConMisErr:
-            _msg = f"Unable to get variables from\n{cubelist}\nto calculate air density"
+            _msg = (
+                f"Unable to get variables from\n{cubelist}"
+                "\nto calculate air density"
+            )
             raise MissingCubeError(_msg)
 
 
+@const_from_attrs()
+def calc_derived_cubes(cubelist, const=None, model=um):
+    """Calculate additional variables."""
+    try:
+        cubelist.extract_cube(model.temp)
+    except ConMisErr:
+        cubelist.append(air_temperature(cubelist, const=const, model=model))
+    try:
+        cubelist.extract_cube(model.thta)
+    except ConMisErr:
+        cubelist.append(
+            air_potential_temperature(cubelist, const=const, model=model)
+        )
+    try:
+        cubelist.extract_cube(model.pres)
+    except ConMisErr:
+        cubelist.append(air_pressure(cubelist, const=const, model=model))
+    try:
+        cubelist.extract_cube(model.dens)
+    except ConMisErr:
+        cubelist.append(air_density(cubelist, const=const, model=model))
+    try:
+        cubelist.extract_cube(model.ghgt)
+    except ConMisErr:
+        cubelist.append(
+            geopotential_height(cubelist, const=const, model=model)
+        )
+
+
 @update_metadata(units="m2 s-2")
 def geopotential_height(cubelist, const=None, model=um):
     """
     Get geopotential height from the given cube list.
 
     If not present, the altitude coordinate is transformed into a cube.
 
@@ -217,19 +316,25 @@
     iris.cube.Cube
         Cube of geopotential height.
     """
     try:
         return cubelist.extract_cube(model.ghgt)
     except ConMisErr:
         try:
-            cube_w_height = cubelist.extract(_dim_constr(model.z, strict=False))[0]
+            cube_w_height = cubelist.extract(
+                _dim_constr(model.z, strict=False)
+            )[0]
             if const is None:
                 const = cube_w_height.attributes["planet_conf"]
             g_hgt = coord_to_cube(cube_w_height, model.z) * const.gravity
-            g_hgt.attributes = {k: v for k, v in cube_w_height.attributes.items() if k != "STASH"}
+            g_hgt.attributes = {
+                k: v
+                for k, v in cube_w_height.attributes.items()
+                if k != "STASH"
+            }
             ensure_bounds(g_hgt, [model.z])
             g_hgt.rename(model.ghgt)
             return g_hgt
         except ConMisErr:
             _msg = f"No cubes in \n{cubelist}\nwith {model.z} as a coordinate."
             raise MissingCubeError(_msg)
 
@@ -248,15 +353,15 @@
     cubelist: iris.cube.CubeList
         Input list of cubes.
     quantity: str or iris.Constraint
         Quantity (present in the cube list).
     axis: str
         Axis of the flux component (x|y|z)
     weight_by_density: bool, optional
-        Multiply by a cube of air density (must be present in the input cube list).
+        Multiply by air density (must be present in the input cube list).
     model: aeolus.model.Model, optional
         Model class with relevant variable names.
 
     Returns
     -------
     iris.cube.Cube
         Cube of a flux component with the same dimensions as input cubes.
@@ -299,16 +404,16 @@
     if kind == "sw":
         all_sky = model.toa_osr
         clr_sky = model.toa_osr_cs
     elif kind == "lw":
         all_sky = model.toa_olr
         clr_sky = model.toa_olr_cs
     elif kind == "total":
-        sw = toa_cloud_radiative_effect(cubelist, "sw")
-        lw = toa_cloud_radiative_effect(cubelist, "lw")
+        sw = toa_cloud_radiative_effect(cubelist, "sw", model=model)
+        lw = toa_cloud_radiative_effect(cubelist, "lw", model=model)
         cre = sw + lw
         cre.rename(name)
         return cre
 
     cube_clr = cubelist.extract_cube(clr_sky)
     cube_all = cubelist.extract_cube(all_sky)
     cre = cube_clr - cube_all
@@ -337,15 +442,16 @@
         model.toa_isr,
         model.toa_osr,
         model.toa_olr,
     ]
     terms = cubelist.extract(varnames)
     if len(terms) != 3:
         raise MissingCubeError(
-            f"{varnames} required for TOA energy balance are missing from cubelist:\n{cubelist}"
+            f"{varnames} required for TOA energy balance"
+            " are missing from cubelist:\n{cubelist}"
         )
     terms_ave = []
     for cube in terms:
         terms_ave.append(cube)
     toa_net = terms_ave[0] - terms_ave[1] - terms_ave[2]
     return toa_net
 
@@ -354,15 +460,15 @@
 def sfc_net_energy(cubelist, model=um):
     """
     Calculate domain-average surface energy flux.
 
     Parameters
     ----------
     cubelist: iris.cube.CubeList
-        Input list of cubes with net LW and SW radiation, sensible and latent surface fluxes.
+        Input cubes with net LW and SW, sensible and latent surface fluxes.
     model: aeolus.model.Model, optional
         Model class with relevant variable names.
 
     Returns
     -------
     iris.cube.Cube
         Cube of total surface downward energy flux.
@@ -371,15 +477,15 @@
     net_down_sw = cubelist.extract_cube(model.sfc_net_down_sw)
     shf = cubelist.extract_cube(model.sfc_shf)
     lhf = cubelist.extract_cube(model.sfc_lhf)
     sfc_net = net_down_lw + net_down_sw - shf - lhf
     return sfc_net
 
 
-@const_from_attrs
+@const_from_attrs()
 @update_metadata(name="surface_net_downward_water_flux", units="mm h-1")
 def sfc_water_balance(cubelist, const=None, model=um):
     """
     Calculate domain-average precipitation minus evaporation.
 
     Parameters
     ----------
@@ -400,27 +506,29 @@
         evap = cubelist.extract_cube(model.sfc_evap)
     except ConMisErr:
         try:
             lhf = cubelist.extract_cube(model.sfc_lhf)
             evap = lhf / const.condensible_heat_vaporization
             evap /= const.condensible_density
         except (KeyError, ConMisErr):
-            raise MissingCubeError(f"Cannot retrieve evaporation from\n{cubelist}")
+            raise MissingCubeError(
+                f"Cannot retrieve evaporation from\n{cubelist}"
+            )
     try:
         precip = cubelist.extract_cube(model.ppn)
         precip /= const.condensible_density
     except ConMisErr:
         precip = precip_sum(cubelist, ptype="total", const=const, model=model)
     precip.convert_units("mm h-1")
     evap.convert_units("mm h-1")
     net = precip - evap
     return net
 
 
-@const_from_attrs
+@const_from_attrs()
 def precip_sum(cubelist, ptype="total", const=None, model=um):
     """
     Calculate a sum of different types of precipitation [:math:`mm~day^{-1}`].
 
     Parameters
     ----------
     cubelist: iris.cube.CubeList
@@ -440,25 +548,28 @@
     """
     try:
         varnames = _precip_name_mapping(model=model)[ptype]
     except KeyError:
         raise ArgumentError(f"Unknown ptype={ptype}")
     if len(cubelist.extract(varnames)) == 0:
         raise MissingCubeError(
-            f"{varnames} required for ptype={ptype} are missing from cubelist:\n{cubelist}"
+            f"{varnames} required for ptype={ptype} "
+            "are missing from cubelist:\n{cubelist}"
         )
     precip = 0.0
     for varname in varnames:
         try:
             cube = cubelist.extract_cube(varname)
+            if varname in [model.cv_rain, model.cv_snow]:
+                cube = cube.copy(data=cube.data.filled(fill_value=0))
             precip += cube
         except ConMisErr:
             pass
     precip /= const.condensible_density
-    precip.convert_units("mm day^-1")
+    precip.convert_units("mm day-1")
     precip.rename(f"{ptype}_precip_rate")
     return precip
 
 
 @update_metadata(name="heat_redistribution_efficiency", units="1")
 def heat_redist_eff(cubelist, region_a, region_b, model=um):
     r"""
@@ -536,15 +647,47 @@
     t_sfc = cubelist.extract_cube(model.t_sfc)
     t_eff = toa_eff_temp(cubelist, model=model)
     out = (t_eff / t_sfc) ** 4
     out = out.copy(data=1 - out.data)
     return out
 
 
-@const_from_attrs
+@const_from_attrs()
+@update_metadata(name="greenhouse_effect_parameter", units="K")
+def greenhouse_effect(cubelist, kind="all_sky", const=None, model=um):
+    r"""
+    Calculate the greenhouse effect [K].
+
+    .. math::
+        GHE = T_{sfc} - \left(\frac{T_{eff}}{T_{sfc}}\right)^4
+
+    Parameters
+    ----------
+    cubelist: iris.cube.CubeList
+        Input list of cubes.
+    kind: str, optional
+        Type of GHE:  "all_sky" or "clear_sky"
+    model: aeolus.model.Model, optional
+        Model class with relevant variable names.
+
+    Returns
+    -------
+    iris.cube.Cube
+        Cube of greenhouse effect parameter.
+    """
+    t_sfc = cubelist.extract_cube(model.t_sfc)
+    if kind == "all_sky":
+        toa_olr = cubelist.extract_cube(model.toa_olr)
+    elif kind == "clear_sky":
+        toa_olr = cubelist.extract_cube(model.toa_olr_cs)
+    ghe = t_sfc - (toa_olr / const.stefan_boltzmann) ** 0.25
+    return ghe
+
+
+@const_from_attrs()
 @update_metadata(name="bond_albedo", units="1")
 def bond_albedo(cubelist, const=None, model=um):
     r"""
     Bold albedo.
 
     .. math::
         4 \frac{OSR_{TOA}}{S_{0}}
@@ -577,19 +720,20 @@
 
     .. math::
         WP = \int_{z_{sfc}}^{z_{top}} \rho q dz
 
     Parameters
     ----------
     cubelist: iris.cube.CubeList
-        Input list of cubes containing appropriate mixing ratio and air density.
+        Input list of cubes containing mixing ratio and air density.
     kind: str, optional
         Short name of the water phase to be integrated.
-        Options are water_vapour (default) | liquid_water | ice_water | cloud_water
-        `cloud_water` is the sum of liquid and ice phases.
+        Options:
+        water_vapour (default) | liquid_water | ice_water | cloud_water
+        where `cloud_water` is the sum of liquid and ice phases.
     model: aeolus.model.Model, optional
         Model class with relevant coordinate names.
         `model.z` is used as a vertical coordinate for integration.
 
     Returns
     -------
     iris.cube.Cube
@@ -631,15 +775,15 @@
     """
     temp = cubelist.extract_cube(model.temp)
     return d_dz(temp, model=model)
 
 
 def horiz_wind_cmpnts(cubelist, model=um):
     """
-    Extract u and v wind components from a cube list and interpolate v on u's grid if necessary.
+    Extract u and v winds and interpolate v on u's grid if necessary.
 
     Parameters
     ----------
     cubelist: iris.cube.CubeList
         List of cubes with horizontal wind components
     model: aeolus.model.Model, optional
         Model class with relevant variable names.
@@ -653,15 +797,15 @@
     u = cubelist.extract(model.u)[0]
     v = cubelist.extract(model.v)[0]
     # interpolate v on u's grid if coordinates are different
     v = regrid_3d(v, u, model=model)
     return u, v
 
 
-@const_from_attrs
+@const_from_attrs()
 @update_metadata(name="local_superrotation_index", units="1")
 def superrotation_index(cubelist, const=None, model=um):
     r"""
     Local superrotation index.
 
     .. math::
         s = \frac{m}{\Omega a^2} - 1,
@@ -707,69 +851,70 @@
     r_coslat.units = Unit("m")
     inner_sum = add(u, omega_r_coslat, dim=lat_dim)
 
     # Calculate axial component of specific absolute angular momentum
     ang_mom = multiply(inner_sum, r_coslat, dim=lat_dim)
 
     # Final index
-    s_idx = ang_mom / omega / (r ** 2)
+    s_idx = ang_mom / omega / (r**2)
     s_idx.convert_units("1")
     s_idx = s_idx.copy(data=s_idx.data - 1)
     return s_idx
 
 
 @update_metadata(name="wind_speed", units="m s-1")
 def wind_speed(*components):
     r"""
     Calculate the wind speed (magnitude of the wind vector).
 
+    .. math::
+        \sqrt{u^2 + v^2 + w^2}
+
     Parameters
     ----------
     args: iris.cube.Cube
         Cubes of u, v, w wind components.
 
-    .. math::
-        \sqrt{u^2 + v^2 + w^2}
+    Returns
+    -------
+    iris.cube.Cube
     """
-    out = sum(cube ** 2 for cube in components) ** 0.5
+    out = sum(cube**2 for cube in components) ** 0.5
     return out
 
 
-@const_from_attrs
 @update_metadata(name="atmosphere_hybrid_sigma_pressure_coordinate", units="1")
-def sigma_p(cubelist, const=None, model=um):
+def sigma_p(cubelist, model=um):
     r"""
     Calculate sigma (normalised pressure coordinate) from a cube of pressure.
 
     .. math::
         \sigma = p / p_{sfc}
 
     Parameters
     ----------
     cubelist: iris.cube.CubeList
         Input list of cubes.
-    const: aeolus.const.const.ConstContainer, optional
-        Must have a cube of reference (surface) pressure as an attribute.
-        If not given, attempt to retrieve it from cube attributes.
     model: aeolus.model.Model, optional
         Model class with relevant variable names.
     """
-    pres_cube = time_mean(spatial_mean(cubelist.extract_cube(model.pres)))
-    pres_cube.convert_units("Pa")
-    return pres_cube / const.reference_surface_pressure
+    pres_atm = cubelist.extract_cube(model.pres)
+    pres_sfc = cubelist.extract_cube(model.p_sfc)
+    out = pres_atm / pres_sfc
+    return out
 
 
-@const_from_attrs
+@const_from_attrs()
 @update_metadata(name="zonal_mass_streamfunction", units="kg s^-1")
 def zonal_mass_streamfunction(cubelist, const=None, model=um):
     r"""
     Calculate mean zonal mass streamfunction.
 
     .. math::
-        \Psi_Z = 2\pi a \int_{z_{sfc}}^{z_{top}}\overline{\rho}^* \overline{u}^* dz
+        \Psi_Z=2\pi a\int_{z_{sfc}}^{z_{top}}\overline{\rho}^*\overline{u}^* dz
 
     References
     ----------
     Haqq-Misra & Kopparapu (2015), eq. 5;
     Hartmann (1994), Global Physical Climatology, eq. 6.21
 
     Examples
@@ -802,29 +947,29 @@
         res = cumsum(integrand, "z", axis_weights=True, model=model)
         res /= const.gravity
 
     res *= streamf_const
     return res
 
 
-@const_from_attrs
+@const_from_attrs()
 @update_metadata(name="meridional_mass_streamfunction", units="kg s^-1")
 def meridional_mass_streamfunction(cubelist, const=None, model=um):
     r"""
     Calculate the mean meridional mass streamfunction.
 
     * In height coordinates
 
     .. math::
         \Psi_M = - 2\pi cos\phi a \int_{z_{sfc}}^{z_{top}}\overline{\rho v} dz
 
     * In pressure coordinates
 
     .. math::
-        \Psi_M = 2\pi cos\phi a \int_{0}^{p_{sfc}}\overline{\rho v} dp / g
+        \Psi_M = 2\pi cos\phi a \int_{0}^{p_{sfc}}\overline{v} dp / g
 
     Parameters
     ----------
     cubelist: iris.cube.CubeList
         Input cubelist.
     const: aeolus.const.const.ConstContainer, optional
         If not given, constants are attempted to be retrieved from
@@ -845,28 +990,90 @@
     Examples
     --------
     >>> from aeolus.calc import meridional_mass_streamfunction, time_mean
     >>> from aeolus.const import init_const
     >>> from aeolus.model import um
     >>> earth_constants = init_const("earth")
     >>> cubes = iris.cube.CubeList([time_mean(cube) for cube in input_cubes])
-    >>> mmsf = meridional_mass_streamfunction(cubes, const=earth_constants, model=um)
+    >>> mmsf = meridional_mass_streamfunction(cubes, const=earth_constants)
     """
     v = cubelist.extract_cube(model.v)
     v = zonal_mean(v, model=model)
     if v.coord(model.z).units.is_convertible("m"):
         rho = zonal_mean(cubelist.extract_cube(model.dens), model=model)
         rho.coord(model.z).bounds = None
         v.coord(model.z).bounds = None
-        # Reverse the coordinate to start from the model top (where p=0 or z=z_top)
+        # Reverse the coordinate to start from the top (where p=0 or z=z_top)
         # TODO: check if the coordinate is ascending or descending
         integrand = reverse(v * rho, model.z)
         res = -1 * cumsum(integrand, "z", axis_weights=True, model=model)
         # Reverse the result back
         res = reverse(res, model.z)
     elif v.coord(model.z).units.is_convertible("Pa"):
         res = cumsum(v, "z", axis_weights=True, model=model)
         res /= const.gravity
     # Calculate the constant: 2 pi cos\phi a
     streamf_const = 2 * np.pi * const.radius * lat_cos(res, model=model)
     res *= streamf_const
     return res
+
+
+@const_from_attrs()
+def wind_rot_div(u, v, truncation=None, const=None, model=um):
+    """
+    Split the horizontal wind field into divergent and rotational parts.
+
+    The Helmholtz decomposition method uses the `windspharm` library:
+    https://ajdawson.github.io/windspharm/latest/
+
+    Parameters
+    ----------
+    u: iris.cube.Cube
+        Eastward wind.
+    v: iris.cube.Cube
+        Northward wind.
+    truncation: int
+        Truncation for the spherical harmonic computation
+        (See windspharm docs for details).
+    const: aeolus.const.const.ConstContainer, optional
+        If not given, constants are attempted to be retrieved from
+        attributes of a cube in the cube list.
+    model: aeolus.model.Model, optional
+        Model class with relevant variable names.
+
+    Returns
+    -------
+    out: dict
+        Dictionary of cubes of:
+          - input wind components (for convenience),
+          - divergent components,
+          - rotational components,
+          - zonal mean rotational components,
+          - zonal eddy rotational components.
+
+    References
+    ----------
+    Hammond and Lewis (2021), https://doi.org/10.1073/pnas.2022705118.
+    """
+    from windspharm.iris import VectorWind
+
+    vec = VectorWind(u, v, rsphere=const.radius.data)
+    div_cmpnt_u, div_cmpnt_v, rot_cmpnt_u, rot_cmpnt_v = vec.helmholtz(
+        truncation=truncation
+    )
+    out = {}
+    out["u_total"] = u
+    out["v_total"] = v
+    out["u_div"] = reverse(div_cmpnt_u, model.y)
+    out["v_div"] = reverse(div_cmpnt_v, model.y)
+    out["u_rot"] = reverse(rot_cmpnt_u, model.y)
+    out["v_rot"] = reverse(rot_cmpnt_v, model.y)
+
+    for cmpnt in ["u", "v"]:
+        rot_cmpnt = out[f"{cmpnt}_rot"]
+        out[f"{cmpnt}_rot_zm"] = preserve_shape(zonal_mean)(rot_cmpnt)
+        out[f"{cmpnt}_rot_zm"].rename(f"zonal_mean_of_{rot_cmpnt.name()}")
+        out[f"{cmpnt}_rot_eddy"] = rot_cmpnt - out[f"{cmpnt}_rot_zm"]
+        out[f"{cmpnt}_rot_eddy"].rename(
+            f"zonal_deviation_of_{rot_cmpnt.name()}"
+        )
+    return out
```

### Comparing `aeolus-0.4.9/src/aeolus/calc/flux_h.py` & `aeolus-24.4.29.1/src/aeolus/calc/flux_h.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,91 +1,126 @@
-# -*- coding: utf-8 -*-
 """Integrated fluxes."""
-import iris
 
+from iris import Constraint
+from iris.analysis import SUM
+from iris.cube import CubeList
+from iris.util import guess_coord_axis
 import numpy as np
 
 from ..const import get_planet_radius
 from ..coord import nearest_coord_value, vertical_cross_section_area
 from ..exceptions import _warn
 from ..model import um
 
-
-__all__ = ("horizontal_fluxes_through_region_boundaries", "net_horizontal_flux_to_region")
+__all__ = (
+    "horizontal_fluxes_through_region_boundaries",
+    "net_horizontal_flux_to_region",
+)
 
 
 def horizontal_fluxes_through_region_boundaries(
-    scalar_cube, region, u, v, r_planet=None, vertical_constraint=None, warn_thresh=10, model=um
+    scalar_cube,
+    region,
+    u,
+    v,
+    r_planet=None,
+    vertical_constraint=None,
+    warn_thresh=10,
+    model=um,
 ):
-    """Calculate horizontal fluxes of `scalar_cube` through planes of a rectangular region."""
+    """Calculate horizontal fluxes through planes of a rectangular region."""
     perpendicular_wind_cmpnts = {um.x: u, um.y: v}
 
     if r_planet is None:
         r = get_planet_radius(scalar_cube)
     else:
         r = r_planet
 
-    total_h_fluxes = iris.cube.CubeList()
+    total_h_fluxes = CubeList()
     for bound in region:
         this_coord = bound["coord"]
-        other_coord, (other_min, other_max) = region._perpendicular_side_limits(bound["name"])
+        (
+            other_coord,
+            other_min,
+            other_max,
+        ) = region._perpendicular_side_limits(bound["name"])
         nearest = nearest_coord_value(scalar_cube, this_coord, bound["value"])
         if abs(nearest - bound["value"]) >= warn_thresh:
             _warn(
-                f"Nearest value is {np.round(nearest - bound['value'], 2)} deg away"
-                f" from the given value of {this_coord}",
+                f"Nearest value is {np.round(nearest - bound['value'], 2)}"
+                f" deg away from the given value of {this_coord}",
             )
-        vcross_cnstr = iris.Constraint(**{this_coord: nearest})
+        vcross_cnstr = Constraint(**{this_coord: nearest})
         vcross_cnstr &= vertical_constraint
 
         if other_max >= other_min:
-            vcross_cnstr &= iris.Constraint(**{other_coord: lambda x: other_min <= x <= other_max})
+            vcross_cnstr &= Constraint(
+                **{other_coord: lambda x: other_min <= x <= other_max}
+            )
             cube = scalar_cube.extract(vcross_cnstr)
         else:
-            vcross_cnstr &= iris.Constraint(
+            vcross_cnstr &= Constraint(
                 **{other_coord: lambda x: (other_max >= x) or (other_min <= x)}
             )
             cube = scalar_cube.extract(vcross_cnstr)
-        cube_slice = next(cube.slices([cube.coord(axis="z").name(), other_coord]))
+        cube_slice = next(
+            cube.slices([cube.coord(axis="z").name(), other_coord])
+        )
         vcross_area = vertical_cross_section_area(cube_slice, r_planet=r)
 
         # Calculate side flux (2d)
-        cube = perpendicular_wind_cmpnts[this_coord].extract(vcross_cnstr) * cube * vcross_area
-        cube.rename(f"{scalar_cube.name()}_flux_through_{bound['name']}_boundary")
+        cube = (
+            perpendicular_wind_cmpnts[this_coord].extract(vcross_cnstr)
+            * cube
+            * vcross_area
+        )
+        cube.rename(
+            f"{scalar_cube.name()}_flux_through_{bound['name']}_boundary"
+        )
         # Total flux
         collapsible_dims = [
-            i for i in cube.dim_coords if iris.util.guess_coord_axis(i) in ["Z", "Y", "X"]
+            i
+            for i in cube.dim_coords
+            if guess_coord_axis(i) in ["Z", "Y", "X"]
         ]
-        cube_total = cube.collapsed(collapsible_dims, iris.analysis.SUM)
+        cube_total = cube.collapsed(collapsible_dims, SUM)
         total_h_fluxes.append(cube_total)
     return total_h_fluxes
 
 
 def net_horizontal_flux_to_region(
-    scalar_cube, region, u, v, r_planet=None, vertical_constraint=None, model=um
+    scalar_cube,
+    region,
+    u,
+    v,
+    r_planet=None,
+    vertical_constraint=None,
+    model=um,
 ):
-    """Calculate horizontal fluxes of `scalar_cube` quantity and add them to get the net result."""
+    """Calculate horizontal fluxes and add them to get the net result."""
     total_h_fluxes = horizontal_fluxes_through_region_boundaries(
         scalar_cube,
         region,
         u,
         v,
         r_planet=r_planet,
         vertical_constraint=vertical_constraint,
         model=model,
     )
     net_flux = (
-        total_h_fluxes.extract_cube(iris.Constraint(cube_func=lambda x: "through_west" in x.name()))
+        total_h_fluxes.extract_cube(
+            Constraint(cube_func=lambda x: "through_west" in x.name())
+        )
         - total_h_fluxes.extract_cube(
-            iris.Constraint(cube_func=lambda x: "through_east" in x.name())
+            Constraint(cube_func=lambda x: "through_east" in x.name())
         )
         + total_h_fluxes.extract_cube(
-            iris.Constraint(cube_func=lambda x: "through_south" in x.name())
+            Constraint(cube_func=lambda x: "through_south" in x.name())
         )
         - total_h_fluxes.extract_cube(
-            iris.Constraint(cube_func=lambda x: "through_north" in x.name())
+            Constraint(cube_func=lambda x: "through_north" in x.name())
         )
     )
     net_flux.rename(f"net_{scalar_cube.name()}_horizontal_flux_to_region")
     net_flux.attributes["region_str"] = str(region)
 
     return net_flux
```

### Comparing `aeolus-0.4.9/src/aeolus/calc/meta.py` & `aeolus-24.4.29.1/src/aeolus/meta.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,55 @@
 """Metadata-related functionality."""
-import functools
+
 from collections.abc import Iterable
 from dataclasses import is_dataclass
+import functools
 
 import cf_units
-
-import iris
 from iris.analysis import _dimensional_metadata_comparison
+from iris.cube import Cube, CubeList
 from iris.util import broadcast_to_shape
 
-from ..exceptions import ArgumentError
+from .exceptions import ArgumentError  # , _warn
 
 
-def const_from_attrs(func):
-    """Get constants container from the input cube attributes if not passed explicitly."""
+def const_from_attrs(strict=True):
+    """Get constants from the cube attributes if not passed explicitly."""
 
-    @functools.wraps(func)
-    def wrapper(*args, **kwargs):
-        const = kwargs.pop("const", None)
-        if const is None:
-            for arg in args:
-                if isinstance(arg, iris.cube.Cube):
-                    const = arg.attributes.get("planet_conf")
-                elif isinstance(arg, iris.cube.CubeList):
-                    try:
-                        const = arg[0].attributes.get("planet_conf")
-                    except IndexError:
-                        const = None
-        if is_dataclass(const):
-            kwargs.update(const=const)
-        else:
-            raise ArgumentError(
-                "Constants dataclass has to be an argument or in the cube attributes"
-            )
-        # Call the decorated function
-        out = func(*args, **kwargs)
-        return out
+    def decorator(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            const = kwargs.pop("const", None)
+            if const is None:
+                for arg in args:
+                    if isinstance(arg, Cube):
+                        const = arg.attributes.get("planet_conf")
+                    elif isinstance(arg, CubeList):
+                        try:
+                            const = arg[0].attributes.get("planet_conf")
+                        except IndexError:
+                            const = None
+            if is_dataclass(const):
+                kwargs.update(const=const)
+            else:
+                msg = (
+                    "`const` has to be the function argument "
+                    "or in the cube attributes."
+                )
+                if strict:
+                    raise ArgumentError(msg)
+                # else:
+                #     _warn(msg)
+            # Call the decorated function
+            out = func(*args, **kwargs)
+            return out
 
-    return wrapper
+        return wrapper
+
+    return decorator
 
 
 def copy_doc(original):
     """Copy docstring from another function."""
 
     def wrapper(func):
         func.__doc__ = original.__doc__
@@ -52,31 +60,35 @@
 
 def preserve_shape(func):
     """Preserve shape of the output array."""
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         cube_in = args[0]
-        if isinstance(cube_in, iris.cube.Cube):
+        if isinstance(cube_in, Cube):
             orig_shape = cube_in.shape
         else:
             raise ArgumentError(
                 "`preserve_shape` decorator requires the first argument"
                 "of the function and its output to be a cube."
             )
         # Call the decorated function
         cube_out = func(*args, **kwargs)
         out_name = cube_out.name()
         cell_methods = cube_out.cell_methods
         dim_map = []
         for ndim, _ in enumerate(orig_shape):
-            for pair in _dimensional_metadata_comparison(cube_out, cube_in)["not_equal"]:
+            for pair in _dimensional_metadata_comparison(cube_out, cube_in)[
+                "not_equal"
+            ]:
                 if ndim not in cube_in.coord_dims(pair[0]):
                     dim_map.append(ndim)
-        bc_data = broadcast_to_shape(cube_out.data, orig_shape, sorted(set(dim_map)))
+        bc_data = broadcast_to_shape(
+            cube_out.data, orig_shape, sorted(set(dim_map))
+        )
         cube_out = cube_in.copy(data=bc_data)
         cube_out.rename(out_name)
         cube_out.cell_methods = cell_methods
         return cube_out
 
     return wrapper
 
@@ -102,15 +114,15 @@
             cube.attributes.update(attrs)
 
     def decorator(func):
         @functools.wraps(func)
         def wrapper(*args, **kwargs):
             # Call the decorated function
             out = func(*args, **kwargs)
-            if isinstance(out, iris.cube.Cube):
+            if isinstance(out, Cube):
                 _update(out)
             elif isinstance(out, Iterable):
                 [_update(cube) for cube in out]
             return out
 
         return wrapper
```

### Comparing `aeolus-0.4.9/src/aeolus/calc/metpy.py` & `aeolus-24.4.29.1/src/aeolus/calc/metpy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 """Interface to metpy calc functions."""
+
 import functools
 
 import cf_units
-
-import iris
-
+from iris.cube import Cube
 import metpy.units as metunits
-
 import numpy as np
-
 import pint
-
 import xarray as xr
 
 from ..exceptions import UnitFormatError
 
-
 __all__ = ("preprocess_iris",)
 
 
 def preprocess_iris(f):
     """
     Wrap a function from `metpy.calc` for it to accept iris cubes as arguments.
 
-    In addition, this decorator converts `metpy.calc` output by using the first input argument
-    as a 'donor' cube.
-    Note this works only for functions that preserve dimensions and may not work with some units.
-    Now that metpy has xarray preprocessor, this decorator depends on it.
+    In addition, this decorator converts `metpy.calc` output by using the first
+    input argument as a 'donor' cube.
+    Note this works only for functions that preserve dimensions and may not
+    work with some units. Now that metpy has xarray preprocessor,
+    this decorator depends on it.
     """
+
     # Define local functions
     def to_xarray(cube):
-        """Convert `iris.cube.Cube` to `xarray.DataArray` and format units correctly."""
+        """Convert `iris cube` to `DataArray` and format units correctly."""
         _unit = None
         for ut_format in set(cf_units.UT_FORMATS):
             try:
                 _unit = metunits.units(cube.units.format(ut_format))
             except pint.errors.DimensionalityError:
                 pass
         if _unit is None:
-            raise UnitFormatError(f"Unable to convert cube units of\n{repr(cube)}\nto metpy units")
+            raise UnitFormatError(
+                f"Unable to convert \n{repr(cube)} units \nto metpy units"
+            )
         arr = xr.DataArray.from_iris(cube)
         arr.attrs["units"] = str(_unit)
         return arr
 
     def to_iris(donor_cube, arr, name):
         """Convert metpy calc result to `iris.cube.Cube`."""
         try:
@@ -64,27 +63,28 @@
     @functools.wraps(f)
     def wrapper(*args, **kwargs):
         nargs = []
         _cube = None  # a donor cube with metadata
 
         # Loop over cubes and re-format units
         for arg in args:
-            if isinstance(arg, iris.cube.Cube):
+            if isinstance(arg, Cube):
                 if arg.ndim > 0:
                     # TODO: make this flexible
                     _cube = arg
                 elif _cube is None:
                     _cube = arg
 
                 nargs.append(to_xarray(arg))
             else:
                 nargs.append(arg)
 
         kwargs = {
-            k: (to_xarray(v) if isinstance(v, iris.cube.Cube) else v) for k, v in kwargs.items()
+            k: (to_xarray(v) if isinstance(v, Cube) else v)
+            for k, v in kwargs.items()
         }
 
         # Call the decorated function
         out = f(*nargs, **kwargs)
         if _cube is None:
             # Inputs are not iris cubes
             return out
```

### Comparing `aeolus-0.4.9/src/aeolus/calc/stats.py` & `aeolus-24.4.29.1/src/aeolus/calc/stats.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 """Statistical functions."""
-import iris
+
+from collections.abc import Iterable, Mapping
+
+import iris.analysis
+from iris.analysis.maths import apply_ufunc
+from iris.coords import AuxCoord
+from iris.cube import Cube
 from iris.exceptions import CoordinateCollapseError as CoColErr
 from iris.exceptions import CoordinateNotFoundError as CoNotFound
-from iris.util import broadcast_to_shape
-
+import iris.util
+from iris.util import broadcast_to_shape, promote_aux_coord_to_dim_coord
 import numpy as np
 
-from .calculus import integrate
 from ..coord import area_weights_cube, coord_to_cube, ensure_bounds
 from ..exceptions import ArgumentError, _warn
 from ..model import um
-from ..subset import extract_last_n_days
-
+from ..subset import (
+    extract_after_n_days,
+    extract_between_days,
+    extract_last_n_days,
+)
+from .calculus import integrate
 
 __all__ = (
     "abs_coord_mean",
+    "after_n_day_mean",
+    "between_day_mean",
     "cumsum",
     "last_n_day_mean",
     "meridional_mean",
     "minmaxdiff",
     "normalize_cube",
     "region_mean_diff",
     "spatial",
@@ -45,28 +56,30 @@
         Coordinate to apply abs().
 
     Returns
     -------
     iris.cube.Cube
         Cube with a reduced dimension.
     """
-    sign_lat = iris.analysis.maths.apply_ufunc(np.sign, coord_to_cube(cube, coord, broadcast=False))
+    sign_lat = apply_ufunc(
+        np.sign, coord_to_cube(cube, coord, broadcast=False)
+    )
     sign_cube = sign_lat * cube
     _coord = sign_cube.coord(coord)
     _coord_dim = sign_cube.coord_dims(_coord)
-    abs_coord = iris.coords.AuxCoord.from_coord(_coord)
+    abs_coord = AuxCoord.from_coord(_coord)
     abs_coord.rename(f"abs_{abs_coord.name()}")
     abs_coord.points = np.abs(_coord.points)
     abs_coord.bounds = np.abs(_coord.bounds)
     sign_cube.add_aux_coord(abs_coord, data_dims=_coord_dim)
     out = sign_cube.aggregated_by(abs_coord, iris.analysis.MEAN)
     out.remove_coord(_coord)
     out.rename(cube.name())
     out.units = cube.units
-    iris.util.promote_aux_coord_to_dim_coord(out, abs_coord.name())
+    promote_aux_coord_to_dim_coord(out, abs_coord.name())
     out.coord(abs_coord).rename(_coord.name())
     return out
 
 
 def cumsum(cube, axis, axis_weights=False, model=um):
     """
     Cumulative sum of a cube.
@@ -91,30 +104,53 @@
         c = cube.coord(getattr(model, axis)).copy()
     except (AttributeError, CoNotFound):
         c = cube.coord(axis=axis).copy()
     dim = cube.coord_dims(c)
     if axis_weights:
         if not c.has_bounds():
             c.guess_bounds()
-        weights = broadcast_to_shape(c.bounds[:, 1] - c.bounds[:, 0], cube.shape, dim)
+        weights = broadcast_to_shape(
+            c.bounds[:, 1] - c.bounds[:, 0], cube.shape, dim
+        )
         data = cube.data * weights
         units = cube.units * c.units
     else:
         data = cube.data
         units = cube.units
     data = np.nancumsum(data, axis=dim[0])
     res = cube.copy(data=data)
     res.rename(f"cumulative_sum_of_{cube.name()}_along_{axis}")
     res.units = units
     return res
 
 
 def last_n_day_mean(cube, days=365, model=um):
     """Average the cube over the last `n` days of its time dimension."""
-    cube_sub = time_mean(extract_last_n_days(cube, days=days, model=model), model=model)
+    cube_sub = time_mean(
+        extract_last_n_days(cube, days=days, model=model), model=model
+    )
+    return cube_sub
+
+
+def after_n_day_mean(cube, days=365, model=um):
+    """Average the cube over the last `n` days of its time dimension."""
+    cube_sub = time_mean(
+        extract_after_n_days(cube, days=days, model=model), model=model
+    )
+    return cube_sub
+
+
+def between_day_mean(cube, day_start, day_end, model=um):
+    """Average the cube over a subset of days."""
+    cube_sub = time_mean(
+        extract_between_days(
+            cube, day_start=day_start, day_end=day_end, model=model
+        ),
+        model=model,
+    )
     return cube_sub
 
 
 def meridional_mean(cube, model=um):
     """
     Calculate cube's meridional average.
 
@@ -128,16 +164,20 @@
     Returns
     -------
     iris.cube.Cube
         Collapsed cube.
     """
     lat_name = model.y
     coslat = np.cos(np.deg2rad(cube.coord(lat_name).points))
-    coslat2d = iris.util.broadcast_to_shape(coslat, cube.shape, cube.coord_dims(lat_name))
-    cube_mean = (cube * coslat2d).collapsed(lat_name, iris.analysis.SUM) / np.sum(coslat)
+    coslat2d = broadcast_to_shape(
+        coslat, cube.shape, cube.coord_dims(lat_name)
+    )
+    cube_mean = (cube * coslat2d).collapsed(
+        lat_name, iris.analysis.SUM
+    ) / np.sum(coslat)
     return cube_mean
 
 
 def minmaxdiff(cubelist, name):
     """
     Spatial maximum minus spatial minimum for a given cube.
 
@@ -193,18 +233,22 @@
         First region.
     region_b: aeolus.region.Region
         Second region.
 
     Returns
     -------
     iris.cube.Cube
-        Difference between the region averages with collapsed spatial dimensions.
+        Difference between the region averages with collapsed spatial dims.
     """
-    mean_a = spatial_mean(cubelist.extract_cube(name).extract(region_a.constraint))
-    mean_b = spatial_mean(cubelist.extract_cube(name).extract(region_b.constraint))
+    mean_a = spatial_mean(
+        cubelist.extract_cube(name).extract(region_a.constraint)
+    )
+    mean_b = spatial_mean(
+        cubelist.extract_cube(name).extract(region_b.constraint)
+    )
     diff = mean_a - mean_b
     diff.rename(f"{name}_mean_diff_{region_a}_{region_b}")
     return diff
 
 
 def spatial(cube, aggr, model=um):
     """
@@ -250,27 +294,45 @@
     """Shortcut for spatial(cube, "mean")."""
     return spatial(cube, "mean", model=model)
 
 
 def spatial_quartiles(cube, model=um):
     """Calculate quartiles over horizontal coordinates."""
     _warn("No weights are applied!")
-    q25 = cube.collapsed((model.y, model.x), iris.analysis.PERCENTILE, percent=25)
-    q75 = cube.collapsed((model.y, model.x), iris.analysis.PERCENTILE, percent=75)
+    q25 = cube.collapsed(
+        (model.y, model.x), iris.analysis.PERCENTILE, percent=25
+    )
+    q75 = cube.collapsed(
+        (model.y, model.x), iris.analysis.PERCENTILE, percent=75
+    )
     return q25, q75
 
 
-def time_mean(cube, model=um):
-    """Time average of a cube."""
-    try:
-        out = cube.collapsed(model.t, iris.analysis.MEAN)
-    except CoColErr as e:
-        _warn(f"Caught exception in time_mean():\n{e}")
-        # out = iris.util.squeeze(cube)
-        out = cube
+def time_mean(obj, squeeze=False, model=um):
+    """Time average of a cube or a container with cubes."""
+    if isinstance(obj, Cube):
+        try:
+            out = obj.collapsed(model.t, iris.analysis.MEAN)
+        except CoColErr as e:
+            _warn(f"Caught exception in time_mean():\n{e}")
+            out = obj
+        if squeeze:
+            out = iris.util.squeeze(out)
+    elif isinstance(obj, Mapping):
+        out = {}
+        for key, cube in obj.items():
+            out[key] = time_mean(cube, model=model)
+        out = obj.__class__(out)
+    elif isinstance(obj, Iterable):
+        out = []
+        for cube in obj:
+            out.append(time_mean(cube, model=model))
+        out = obj.__class__(out)
+    else:
+        raise ArgumentError(f"Unrecognised type of obj: {type(obj)}")
     return out
 
 
 def vertical_mean(cube, weight_by=None, model=um):
     """
     Vertical mean of a cube with optional weighting.
 
@@ -286,33 +348,39 @@
     Returns
     -------
     iris.cube.Cube
         Collapsed cube.
     """
     coord = model.z
     if len(cube.coord_dims(coord)) == 0:
-        _warn(f"The {repr(coord)} does not describe any dimension in {repr(cube)}.")
+        _warn(
+            f"{repr(coord)} does not describe any dimension in {repr(cube)}."
+        )
         return cube
     if weight_by is None:
         vmean = cube.collapsed(coord, iris.analysis.MEAN)
     else:
         if isinstance(weight_by, (str, iris.coords.Coord)):
             weights = broadcast_to_shape(
-                cube.coord(weight_by).points.squeeze(), cube.shape, cube.coord_dims(weight_by)
+                cube.coord(weight_by).points.squeeze(),
+                cube.shape,
+                cube.coord_dims(weight_by),
             )
             vmean = cube.collapsed(coord, iris.analysis.MEAN, weights=weights)
         elif isinstance(weight_by, iris.cube.Cube):
             a_copy = cube.copy()
             b_copy = weight_by.copy()
             a_copy.coord(coord).bounds = None
             b_copy.coord(coord).bounds = None
             prod = b_copy * a_copy
             vmean = integrate(prod, coord) / integrate(weight_by, coord)
         else:
-            raise ArgumentError(f"Unrecognised type of weight_by: {type(weight_by)}")
+            raise ArgumentError(
+                f"Unrecognised type of weight_by: {type(weight_by)}"
+            )
     vmean.rename(f"vertical_mean_of_{cube.name()}")
     return vmean
 
 
 def zonal_mean(cube, model=um):
     """
     Calculate cube's zonal average.
```

### Comparing `aeolus-0.4.9/src/aeolus/calc/tl.py` & `aeolus-24.4.29.1/src/aeolus/calc/tl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """Operations in tidally-locked coordinates."""
-import iris
+
+import iris.analysis
 from iris.analysis.cartography import _meshgrid, rotate_pole, rotate_winds
 from iris.coord_systems import RotatedGeogCS
-
+from iris.coords import AuxCoord
+from iris.cube import Cube
+from iris.util import promote_aux_coord_to_dim_coord
 import numpy as np
 
 from ..coord import get_xy_coords
 from ..exceptions import BadCoordinateError
 from ..model import um
 
 __all__ = (
@@ -34,55 +37,65 @@
         Model class with relevant coordinate and variable names.
     """
     _cs = cube.coord_system()
     xcoord, ycoord = get_xy_coords(cube, model=model)
     lon2d, lat2d = _meshgrid(xcoord.points, ycoord.points)
     r_lons, r_lats = rotate_pole(lon2d, lat2d, pole_lon, pole_lat)
 
-    r_lon_coord = iris.coords.AuxCoord(
+    r_lon_coord = AuxCoord(
         r_lons.flatten(),
         units=xcoord.units,
         standard_name=xcoord.standard_name,
         var_name=xcoord.var_name,
         coord_system=_cs,
     )
-    r_lat_coord = iris.coords.AuxCoord(
+    r_lat_coord = AuxCoord(
         r_lats.flatten(),
         units=ycoord.units,
         standard_name=ycoord.standard_name,
         var_name=ycoord.var_name,
         coord_system=_cs,
     )
-    non_xy_coords = [(i, cube.coord_dims(i)) for i in cube.dim_coords if i not in [xcoord, ycoord]]
+    non_xy_coords = [
+        (i, cube.coord_dims(i))
+        for i in cube.dim_coords
+        if i not in [xcoord, ycoord]
+    ]
     # assume latitude and longitude are the rightmost dimensions
     lat_dim = len(non_xy_coords)
     if lat_dim != cube.coord_dims(ycoord)[0]:
-        raise BadCoordinateError("Ensure latitude and longitude are the rightmost dimensions.")
-    cube_flat = iris.cube.Cube(
-        cube.core_data().reshape((*cube.shape[:lat_dim], np.product(cube.shape[lat_dim:]))),
+        raise BadCoordinateError(
+            "Ensure latitude and longitude are the rightmost dimensions."
+        )
+    cube_flat = Cube(
+        cube.core_data().reshape(
+            (*cube.shape[:lat_dim], np.product(cube.shape[lat_dim:]))
+        ),
         aux_coords_and_dims=[
             *non_xy_coords,
             (r_lat_coord, lat_dim),
             (r_lon_coord, lat_dim),
         ],
         units=cube.units,
     )
     for coord, _ in non_xy_coords:
-        iris.util.promote_aux_coord_to_dim_coord(cube_flat, coord)
+        promote_aux_coord_to_dim_coord(cube_flat, coord)
 
     out = cube_flat.regrid(cube, iris.analysis.UnstructuredNearest())
     return out
 
 
-def regrid_to_tidally_locked_coordinates(cube, pole_lon=0, pole_lat=0, model=um):
+def regrid_to_tidally_locked_coordinates(
+    cube, pole_lon=0, pole_lat=0, model=um
+):
     """
     Regrid a cube to tidally locked coordinates.
 
-    The substellar and antistellar point become the north and south pole, respectively.
-    By default, the substellar point is assumed to be at (0, 0).
+    The substellar and antistellar point become the north and south pole,
+    respectively. By default, the substellar point is assumed to be at (0, 0).
 
     Parameters
     ----------
     cube: iris.cube.Cube
         Input cube.
     pole_lon: float, optional
         New North Pole longitude.
@@ -96,23 +109,23 @@
     )
 
 
 def rotate_winds_to_tidally_locked_coordinates(u, v, pole_lon=0, pole_lat=0):
     """
     Rotate the horizontal wind components to tidally locked coordinates.
 
-    The substellar and antistellar point become the north and south pole, respectively.
-    By default, the substellar point is assumed to be at (0, 0).
+    The substellar and antistellar point become the north and south pole,
+    respectively. By default, the substellar point is assumed to be at (0, 0).
 
     Parameters
     ----------
     u: iris.cube.Cube
-        An instance of :class:`iris.cube.Cube` that contains the x-component of the vector.
+        :class:`iris.cube.Cube` that contains the x-component of the vector.
     v: iris.cube.Cube
-        An instance of :class:`iris.cube.Cube` that contains the y-component of the vector.
+        :class:`iris.cube.Cube` that contains the y-component of the vector.
     pole_lon: float, optional
         New North Pole longitude.
     pole_lat: float, optional
         New North Pole latitude.
     """
     tl_cs = RotatedGeogCS(pole_lon, pole_lat, ellipsoid=u.coord_system())
     tl_u, tl_v = rotate_winds(u, v, tl_cs)
```

### Comparing `aeolus-0.4.9/src/aeolus/const/const.py` & `aeolus-24.4.29.1/src/aeolus/const/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,97 +1,74 @@
-# -*- coding: utf-8 -*-
 """Main interface to the physical constants store."""
-import json
+
 from dataclasses import make_dataclass
+import json
 from pathlib import Path
 
-import iris
-
+from iris.coord_systems import GeogCS
+from iris.cube import Cube
+import iris.fileformats
 import numpy as np
 
 from ..exceptions import ArgumentError, LoadError, _warn
 
-
 __all__ = ("add_planet_conf_to_cubes", "get_planet_radius", "init_const")
 
 CONST_DIR = Path(__file__).parent / "store"
 
 DERIVED_CONST = {
     "dry_air_gas_constant": (
         lambda slf: slf.molar_gas_constant / slf.dry_air_molecular_weight,
         "J kg-1 K-1",
     ),
     "molecular_weight_ratio": (
-        lambda slf: slf.condensible_molecular_weight / slf.dry_air_molecular_weight,
+        lambda slf: slf.condensible_molecular_weight
+        / slf.dry_air_molecular_weight,
         "1",
     ),
-    "poisson_exponent": (
+    "kappa": (
         lambda slf: slf.dry_air_gas_constant / slf.dry_air_spec_heat_press,
         "1",
+    ),  # poisson_exponent
+    "planet_rotation_rate": (
+        lambda slf: (slf.day / (2 * np.pi)) ** (-1),
+        "s-1",
     ),
-    "planet_rotation_rate": (lambda slf: (slf.day / (2 * np.pi)) ** (-1), "s-1"),
 }
 
 
-class ScalarCube(iris.cube.Cube):
-    """Cube without coordinates."""
-
-    def __init__(self, *args, **kw):
-        """Initialise aeolus.const.const.ScalarCube."""
-        _warn(
-            "ScalarCube is deprecated and will be removed in the next release. "
-            "Use iris.cube.Cube instead.",
-        )
-        super(ScalarCube, self).__init__(*args, **kw)
-
-    def __repr__(self):
-        """Repr of this class."""
-        return f"<ScalarCube of {self.long_name} [{self.units}]>"
-
-    def __deepcopy__(self, memo):
-        """Deep copy of a scalar cube."""
-        return self.from_cube(self._deepcopy(memo))
-
-    @property
-    def asc(self):
-        """Convert cube to AuxCoord for math ops."""
-        return iris.coords.AuxCoord(
-            np.asarray(self.data), units=self.units, long_name=self.long_name
-        )
-
-    @classmethod
-    def from_cube(cls, cube):
-        """Convert iris cube to ScalarCube."""
-        return cls(**{k: getattr(cube, k) for k in ["data", "units", "long_name"]})
-
-
 class ConstContainer:
     """Base class for creating dataclasses and storing planetary constants."""
 
     def __repr__(self):
         """Create custom repr."""
         cubes_str = ", ".join(
             [
-                f"{getattr(self, _field).long_name} [{getattr(self, _field).units}]"
+                (
+                    f"{getattr(self, _field).long_name}"
+                    f" [{getattr(self, _field).units}]"
+                )
                 for _field in self.__dataclass_fields__
             ]
         )
         return f"{self.__class__.__name__}({cubes_str})"
 
     def __post_init__(self):
         """Do things automatically after __init__()."""
         self._convert_to_iris_cubes()
         self._derive_const()
 
     def _convert_to_iris_cubes(self):
         """Loop through fields and convert each of them to `iris.cube.Cube`."""
         for name in self.__dataclass_fields__:
             _field = getattr(self, name)
-            cube = iris.cube.Cube(
-                data=_field.get("value"), units=_field.get("units", 1), long_name=name
+            cube = Cube(
+                data=_field.get("value"),
+                units=_field.get("units", 1),
+                long_name=name,
             )
             object.__setattr__(self, name, cube)
 
     def _derive_const(self):
         """Not fully implemented yet."""
         for name, recipe in DERIVED_CONST.items():
             func, units = recipe
@@ -110,44 +87,47 @@
         raise ArgumentError("directory must be a pathlib.Path object")
     try:
         with (directory / name).with_suffix(".json").open("r") as fp:
             list_of_dicts = json.load(fp)
         # transform the list of dictionaries into a dictionary
         const_dict = {}
         for vardict in list_of_dicts:
-            const_dict[vardict["name"]] = {k: v for k, v in vardict.items() if k != "name"}
+            const_dict[vardict["name"]] = {
+                k: v for k, v in vardict.items() if k != "name"
+            }
         return const_dict
     except FileNotFoundError:
         raise LoadError(
-            f"JSON file for {name} configuration not found, check the directory: {directory}"
+            f"JSON file for {name} configuration not found,"
+            f"check the directory: {directory}"
         )
 
 
 def init_const(name="general", directory=None):
     """
     Create a dataclass with a given set of constants.
 
     Parameters
     ----------
     name: str, optional
         Name of the constants set.
-        Should be identical to the JSON file name (without the .json extension).
+        Should be identical to the JSON file name (w/o the .json extension).
         If not given, only general physical constants are returned.
     directory: pathlib.Path, optional
-        Path to a folder with JSON files containing constants for a specific planet.
+        Path to a folder with JSON files with constants for a specific planet.
 
     Returns
     -------
     Dataclass with constants as iris cubes.
 
     Examples
     --------
     >>> c = init_const('earth')
     >>> c
-    EarthConstants(gravity [m s-2], radius [m], day [s], solar_constant [W m-2], ...)
+    EarthConstants(gravity [m s-2], radius [m], day [s], ...)
     >>> c.gravity
     <iris 'Cube' of gravity / (m s-2) (scalar cube)>
     """
     cls_name = f"{name.capitalize()}Constants"
     if directory is None:
         # use default directory
         kw = {}
@@ -164,15 +144,15 @@
         frozen=True,
         repr=False,
     )
     return kls(**const_dict)
 
 
 def get_planet_radius(cube, default=iris.fileformats.pp.EARTH_RADIUS):
-    """Get planet radius in metres from cube attributes or coordinate system."""
+    """Get the planet radius in metres from cube attributes."""
     cs = cube.coord_system("CoordSystem")
     if cs is not None:
         r = cs.semi_major_axis
     else:
         try:
             r = cube.attributes["planet_conf"].radius.copy()
             r.convert_units("m")
@@ -181,25 +161,25 @@
             _warn("Using default radius")
             r = default
     return r
 
 
 def add_planet_conf_to_cubes(cubelist, const):
     """
-    Add constants container to the cube attributes and replace its coordinate system.
+    Add constants container to the cube attributes and adjust its coord system.
 
     Parameters
     ----------
     cubelist: iris.cube.CubeList
         List of cubes containing a cube of zonal velocity (u).
     const: aeolus.const.const.ConstContainer, optional
         Constainer with the relevant planetary constants.
     """
     const.radius.convert_units("m")
-    _coord_system = iris.coord_systems.GeogCS(semi_major_axis=const.radius.data)
+    _coord_system = GeogCS(semi_major_axis=const.radius.data)
     for cube in cubelist:
         # add constants to cube attributes
         cube.attributes["planet_conf"] = const
         for coord in cube.coords():
             if coord.coord_system:
-                # Replace coordinate system with the planet radius given in `self.const`
+                # Replace coordinate system with the radius from `self.const`
                 coord.coord_system = _coord_system
```

### Comparing `aeolus-0.4.9/src/aeolus/const/store/earth.json` & `aeolus-24.4.29.1/src/aeolus/const/store/earth.json`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.9/src/aeolus/const/store/general.json` & `aeolus-24.4.29.1/src/aeolus/const/store/general.json`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.9/src/aeolus/const/store/proxb.json` & `aeolus-24.4.29.1/src/aeolus/const/store/proxb.json`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.9/src/aeolus/const/store/titan.json` & `aeolus-24.4.29.1/src/aeolus/const/store/titan.json`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.9/src/aeolus/const/store/trap1d.json` & `aeolus-24.4.29.1/src/aeolus/const/store/trap1d.json`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.9/src/aeolus/const/store/trap1e.json` & `aeolus-24.4.29.1/src/aeolus/const/store/trap1e.json`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.9/src/aeolus/const/store/trap1f.json` & `aeolus-24.4.29.1/src/aeolus/const/store/trap1f.json`

 * *Files identical despite different names*

### Comparing `aeolus-0.4.9/src/aeolus/coord.py` & `aeolus-24.4.29.1/src/aeolus/coord.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,36 @@
-# -*- coding: utf-8 -*-
 """Functionality related to coordinates of cubes."""
+
 from datetime import timedelta
 
 from cartopy.util import add_cyclic_point
-
-import iris
+import dask.array as da
+from iris import Constraint
+import iris.analysis
+import iris.analysis.cartography
 from iris.analysis.cartography import wrap_lons
 from iris.coord_categorisation import _months_in_season, add_categorised_coord
+from iris.coords import AuxCoord, DimCoord
+from iris.cube import Cube, CubeList
 from iris.exceptions import CoordinateNotFoundError as CoNotFound
-from iris.experimental import stratify
-from iris.util import broadcast_to_shape, guess_coord_axis, is_regular
-
+import iris.fileformats
+from iris.util import (
+    broadcast_to_shape,
+    guess_coord_axis,
+    is_regular,
+    promote_aux_coord_to_dim_coord,
+    squeeze,
+)
 import numpy as np
 
 from .const import get_planet_radius
 from .exceptions import ArgumentError, BadCoordinateError, NotFoundError, _warn
+from .meta import const_from_attrs
 from .model import um
 
-
 __all__ = (
     "CoordContainer",
     "add_binned_coord",
     "add_cyclic_point_to_cube",
     "add_planet_calendar",
     "area_weights_cube",
     "check_coords",
@@ -30,18 +39,17 @@
     "coord_to_cube",
     "ensure_bounds",
     "get_cube_datetimes",
     "get_cube_rel_days",
     "get_dim_coord",
     "get_xy_coords",
     "isel",
-    "interp_all_to_pres_lev",
+    "interp_cube_from_height_to_pressure_levels",
+    "interp_cubelist_from_height_to_pressure_levels",
     "interp_to_cube_time",
-    "interp_to_pres_lev",
-    "interp_to_single_pres_lev",
     "nearest_coord_value",
     "not_equal_coord_axes",
     "regrid_3d",
     "replace_z_coord",
     "roll_cube_0_360",
     "roll_cube_pm180",
     "vertical_cross_section_area",
@@ -53,23 +61,23 @@
     """
     Calculate coordinate cell boundaries.
 
     Taken from SciTools iris package.
 
     Parameters
     ----------
-    points: numpy.array
+    points: numpy.ndarray
         One-dimensional array of uniformy spaced values of shape (M,)
     bound_position: bool, optional
         The desired position of the bounds relative to the position
         of the points.
 
     Returns
     -------
-    bounds: numpy.array
+    bounds: numpy.ndarray
         Array of shape (M+1,)
 
     Examples
     --------
     >>> a = np.arange(-1, 2.5, 0.5)
     >>> a
     array([-1. , -0.5,  0. ,  0.5,  1. ,  1.5,  2. ])
@@ -79,37 +87,37 @@
     See Also
     --------
     aeolus.coord._cell_centres
     """
     assert points.ndim == 1, "Only 1D points are allowed"
     diffs = np.diff(points)
     if not np.allclose(diffs, diffs[0]):
-        _warn("_cell_bounds() is supposed to work only for uniformly spaced points")
+        _warn("_cell_bounds() assumes uniformly spaced points")
     delta = diffs[0] * bound_position
     bounds = np.concatenate([[points[0] - delta], points + delta])
     return bounds
 
 
 def _cell_centres(bounds, bound_position=0.5):
     """
     Calculate coordinate cell centres.
 
     Taken from SciTools iris package.
 
     Parameters
     ----------
-    bounds: numpy.array
+    bounds: numpy.ndarray
         One-dimensional array of cell boundaries of shape (M,)
     bound_position: bool, optional
         The desired position of the bounds relative to the position
         of the points.
 
     Returns
     -------
-    centres: numpy.array
+    centres: numpy.ndarray
         Array of shape (M-1,)
 
     Examples
     --------
     >>> a = np.arange(-1, 3., 1.)
     >>> a
     array([-1,  0,  1,  2])
@@ -126,40 +134,45 @@
     return centres
 
 
 def _is_longitude_global(lon_points):
     """Return True if array of longitudes covers the whole sphere."""
     dx = np.diff(lon_points)[0]  # assume regular grid
     case_0_360 = ((lon_points[0] - dx) <= 0) and ((lon_points[-1] + dx) >= 360)
-    case_pm180 = ((lon_points[0] - dx) <= -180) and ((lon_points[-1] + dx) >= 180)
+    case_pm180 = ((lon_points[0] - dx) <= -180) and (
+        (lon_points[-1] + dx) >= 180
+    )
     return case_0_360 or case_pm180
 
 
 class CoordContainer:
     """
     Coordinate container.
 
     Attributes
     ----------
     {x,y,z,t}: iris.coord.Coord
         Coordinates in the respective dimensions
     """
 
-    def __init__(self, cubes, model=um):
+    def __init__(self, cubes, coord_check=False, model=um):
         """
         Instantiate an `AtmosFlow` object.
 
         Parameters
         ----------
         cubes: iris.cube.CubeList
             Atmospheric fields with necessary coordinates.
+        coord_check: bool, optional
+            Check if all cubes have the same set of coordinates.
         model: aeolus.model.Model, optional
             Model class with relevant coordinate and variable names.
         """
-        check_coords(cubes)
+        if coord_check:
+            check_coords(cubes)
         # self.x = cubes[0].coord(model.x)
         self.model = model
         for axis in ["x", "y", "z", "t"]:
             try:
                 setattr(self, axis, cubes[0].coord(axis=axis, dim_coords=True))
             except CoNotFound:
                 pass
@@ -181,47 +194,51 @@
     Returns
     -------
     iris.cube.Cube
     """
     cube_out = cube.copy()
     binned_points = np.digitize(cube_out.coord(coord_name).points, bins)
     binned_points = np.clip(binned_points, 0, len(bins) - 1)
-    new_coord = iris.coords.AuxCoord(binned_points, long_name=f"{coord_name}_binned")
+    new_coord = AuxCoord(binned_points, long_name=f"{coord_name}_binned")
     cube_out.add_aux_coord(new_coord, cube_out.coord_dims(coord_name))
     return cube_out
 
 
 def add_cyclic_point_to_cube(cube, coord=um.x):
     """
     Add a cyclic point to a cube and a corresponding coordinate.
 
-    A wrapper for `cartopy.util.add_cyclic_point()`, generalising it for iris cubes.
+    A wrapper for `cartopy.util.add_cyclic_point()` for iris cubes.
 
     Parameters
     ----------
     cube: iris.cube.Cube
         An n-dimensional cube of data to add a cyclic point to.
     coord: iris.coords.Coord or str
         A 1-dimensional coordinate which specifies the coordinate values for
         the dimension the cyclic point is to be added to. The coordinate
         values must be regularly spaced. Defaults to the "x"-coordinate.
 
     Returns
     -------
-    cyclic_cube
+    iris.cube.Cube
         The cube with a cyclic point added.
     """
     the_coord = cube.coord(coord)
     dim = cube.coord_dims(the_coord)
 
     # TODO: use core_data()?
-    cy_data, cy_coord_pnts = add_cyclic_point(cube.data, coord=the_coord.points, axis=dim[0])
+    cy_data, cy_coord_pnts = add_cyclic_point(
+        cube.data, coord=the_coord.points, axis=dim[0]
+    )
 
     dim_coords_and_dims = [
-        (coord, cube.coord_dims(coord)) for coord in cube.dim_coords if coord != the_coord
+        (coord, cube.coord_dims(coord))
+        for coord in cube.dim_coords
+        if coord != the_coord
     ]
     dim_coords_and_dims.append((the_coord.copy(cy_coord_pnts), dim))
 
     aux_coords_and_dims = [
         (coord, cube.coord_dims(coord))
         for coord in cube.aux_coords
         if cube.coord_dims(coord) != dim
@@ -235,15 +252,15 @@
             "var_name",
             "units",
             "cell_methods",
             "aux_factories",
             "cell_measures_and_dims",
         ]
     }
-    cyclic_cube = iris.cube.Cube(
+    cyclic_cube = Cube(
         cy_data,
         dim_coords_and_dims=dim_coords_and_dims,
         aux_coords_and_dims=aux_coords_and_dims,
         **other_kwargs,
     )
     return cyclic_cube
 
@@ -268,15 +285,15 @@
     time_coord: iris.coords.Coord or str
         Original time coordinate of the cube.
     days_in_year: int or float
         Number of Earth days in one year on the given planet.
     days_in_month: int or float
         Number of Earth days in one month on the given planet.
     days_in_day: int or float
-        Number of Earth days in one day on the given planet (e.g. ~16 for Titan).
+        Number of Earth days in one day on the given planet.
     run_start_day: int or float, optional
         Earth day of the start of the simulation.
     seasons: tuple, optional
         Sequences of letters corresponding to month names.
     planet: str, optional
         Name of the planet to be used to name the new coordinate.
     """
@@ -338,16 +355,15 @@
         aw.rename("normalized_grid_cell_area")
         aw.units = "1"
     else:
         if r_planet is None:
             r = get_planet_radius(cube)
         else:
             r = r_planet
-        aw *= (r / iris.fileformats.pp.EARTH_RADIUS) ** 2
-        aw = cube.copy(data=aw)
+        aw = cube.copy(data=aw * (r / iris.fileformats.pp.EARTH_RADIUS) ** 2)
         aw.rename("grid_cell_area")
         aw.units = "m**2"
     return aw
 
 
 def check_coords(cubes):
     """Check the cubes coordinates for consistency."""
@@ -364,15 +380,17 @@
             )
         )
 
     bad_coords = coord_comparison["resamplable"]
     if bad_coords:
         raise BadCoordinateError(
             "Some coordinates are different ({}), "
-            "consider resampling.".format(", ".join(group.name() for group in bad_coords))
+            "consider resampling.".format(
+                ", ".join(group.name() for group in bad_coords)
+            )
         )
 
 
 def coarsen_cube(cube, lon_bins, lat_bins, model=um):
     """
     Block-average cube in longitude and latitude.
 
@@ -394,41 +412,52 @@
     iris.cube.Cube
     """
     cube_out = cube.copy()
     coord_names = [model.y, model.x]
     cube_out = add_binned_coord(cube_out, model.x, lon_bins)
     cube_out = add_binned_coord(cube_out, model.y, lat_bins)
 
-    # To avoid oversampling on the edges, extract subset within the boundaries of target coords
+    # To avoid oversampling on the edges,
+    # extract subset within the boundaries of target coords
     for coord, target_points in zip(coord_names, (lat_bins, lon_bins)):
         cube_out = cube_out.extract(
-            iris.Constraint(**{coord: lambda p: target_points.min() <= p <= target_points.max()})
+            Constraint(
+                **{
+                    coord: lambda p: target_points.min()
+                    <= p
+                    <= target_points.max()
+                }
+            )
         )
 
     for coord in coord_names:
-        cube_out = cube_out.aggregated_by([f"{coord}_binned"], iris.analysis.MEAN)
+        cube_out = cube_out.aggregated_by(
+            [f"{coord}_binned"], iris.analysis.MEAN
+        )
 
     for coord, target_points in zip(coord_names, (lat_bins, lon_bins)):
         dim = cube_out.coord_dims(coord)
         units = cube_out.coord(coord).units
         cube_out.remove_coord(coord)
         aux = cube_out.coord(f"{coord}_binned")
         new_points = target_points[aux.points]
-        new_coord = iris.coords.DimCoord.from_coord(aux.copy(points=new_points, bounds=None))
+        new_coord = DimCoord.from_coord(
+            aux.copy(points=new_points, bounds=None)
+        )
         cube_out.remove_coord(f"{coord}_binned")
         new_coord.rename(coord)
         new_coord.units = units
         cube_out.add_dim_coord(new_coord, dim)
 
     return cube_out
 
 
 def coord_delta_to_cube(cube, coord, normalize=False):
     """
-    Convert 1D coordinate spacings to a cube of the same dimension as the given cube.
+    Convert 1D coord spacings to a cube of the same dim as the given cube.
 
     Parameters
     ----------
     cube: iris.cube.Cube
         Cube containing the coordinate to be broadcast.
     coord: str or iris.coords.Coord
         Coordinate to be broadcast.
@@ -459,22 +488,22 @@
     else:
         units = _coord.units
         prefix = ""
     if len(dim_map) > 0:
         _data = broadcast_to_shape(_data, cube.shape, dim_map)
         dc = [(c.copy(), cube.coord_dims(c)) for c in cube.dim_coords]
         ac = [(c.copy(), cube.coord_dims(c)) for c in cube.aux_coords]
-        new_cube = iris.cube.Cube(
+        new_cube = Cube(
             data=_data,
             units=units,
             dim_coords_and_dims=dc,
             aux_coords_and_dims=ac,
         )
     else:
-        new_cube = iris.cube.Cube(data=_data, units=units)
+        new_cube = Cube(data=_data, units=units)
     new_cube.rename(f"{prefix}delta_{_coord.name()}")
     return new_cube
 
 
 def coord_to_cube(cube, coord, broadcast=True):
     """
     Convert coordinate points to a cube with the same dimensions.
@@ -505,17 +534,21 @@
     }
     dim_map = cube.coord_dims(_coord.name())
     _data = _coord.points
     if len(dim_map) > 0 and broadcast:
         _data = broadcast_to_shape(_data, cube.shape, dim_map)
         dc = [(c.copy(), cube.coord_dims(c)) for c in cube.dim_coords]
         ac = [(c.copy(), cube.coord_dims(c)) for c in cube.aux_coords]
-        new_cube = iris.cube.Cube(data=_data, dim_coords_and_dims=dc, aux_coords_and_dims=ac, **kw)
+        new_cube = Cube(
+            data=_data, dim_coords_and_dims=dc, aux_coords_and_dims=ac, **kw
+        )
     else:
-        new_cube = iris.cube.Cube(data=_data, dim_coords_and_dims=[(_coord.copy(), 0)], **kw)
+        new_cube = Cube(
+            data=_data, dim_coords_and_dims=[(_coord.copy(), 0)], **kw
+        )
     return new_cube
 
 
 def ensure_bounds(cube, coords=("x", "y"), model=um):
     """Auto-generate bounds for cube coordinates."""
     for coord in coords:
         try:
@@ -537,15 +570,15 @@
     cube: iris.cube.Cube
         Cube containing a time coordinate.
     model: aeolus.model.Model, optional
         Model class with relevant coordinate names.
 
     Returns
     -------
-    numpy.array
+    numpy.ndarray
         Array of datetime-like objects.
     """
     return cube.coord(model.t).units.num2date(cube.coord(model.t).points)
 
 
 def get_cube_rel_days(cube, model=um):
     """
@@ -556,117 +589,201 @@
     cube: iris.cube.Cube
         Cube containing a time coordinate.
     model: aeolus.model.Model, optional
         Model class with relevant coordinate names.
 
     Returns
     -------
-    numpy.array
+    numpy.ndarray
         Array of relative days.
     """
     dts = get_cube_datetimes(cube, model=model)
     days = ((dts - dts[0]) / timedelta(days=1)).astype(np.float64)
     return days
 
 
 def get_dim_coord(cube, axis):
     """
     Return a coordinate from a cube based on the axis it represents.
 
-    Uses :py:func:`iris.util.guess_coord_axis` to heuristically match a dimensional coordinate
-    with the requested axis.
+    Uses :py:func:`iris.util.guess_coord_axis` to heuristically match a
+    dimensional coordinate with the requested axis.
 
     Adapted from https://github.com/LSaffin/iris-extensions
 
     Parameters
     ----------
     cube: iris.cube.Cube
         Cube with the desired coordinate.
     axis: str
         The co-ordinate axis to take from the cube. Must be one of X, Y, Z, T.
 
     Returns
     -------
     iris.coords.DimCoord
-        The dimensional coordinate matching the requested axis on the given cube.
+        The dim coordinate matching the requested axis on the given cube.
 
     Raises
     ------
     ArgumentError: If axis is not one of {X, Y, Z, T}.
-    NotFoundError: If the cube does not contain a coord with the requested axis.
+    NotFoundError: If the cube does not contain a coord with the given axis.
     """
     _allowed = ["X", "Y", "Z", "T"]
     axis = axis.upper()
     # If the axis supplied is not correct raise an error
     if axis not in _allowed:
-        raise ArgumentError(f"Axis must be one of {_allowed}, {axis} is given.")
+        raise ArgumentError(
+            f"Axis must be one of {_allowed}, {axis} is given."
+        )
 
     # Loop over dimensional coords in the cube
     for coord in cube.dim_coords:
         # Return the coordinate if it matches the axis
         if axis == guess_coord_axis(coord):
             return coord
 
     # If no coordinate matches raise an error
     raise NotFoundError(f"Cube has no coordinate for axis {axis}")
 
 
 def get_xy_coords(cube, model=um):
     """
-    Return X and Y coordinate tuple for a given `cube` using names from a given `model` container.
+    Return X and Y coords tuple using names from a given `model` container.
 
     Parameters
     ----------
     cube: iris.cube.Cube
         Input cube.
     model: aeolus.model.Model, optional
         Model class with relevant coordinate and variable names.
     """
     y_coord = cube.coord(model.y)
     x_coord = cube.coord(model.x)
     return (x_coord, y_coord)
 
 
-def interp_all_to_pres_lev(cubelist, levels, interpolator=None, model=um):
+@const_from_attrs(strict=False)
+def interp_cube_from_height_to_pressure_levels(
+    variable,
+    pressure,
+    levels,
+    p_ref_frac=False,
+    const=None,
+    interpolator=None,
+    model=um,
+):
     """
-    Interpolate all cubes within a cubelist to the given set of pressure levels.
+    Interpolate a cube from height to pressure level(s).
+
+    Parameters
+    ----------
+    variable: iris.cube.Cube
+        A cube to interpolate.
+        Must have the same dimensions as the pressure cube.
+    pressure: iris.cube.Cube
+        A cube of pressure.
+    levels: array-like
+        Sequence of pressure levels
+        (same units as the units of pressure cube in `cubelist`).
+    p_ref_frac: bool, optional
+        If True, `levels` are used as fractions of the surface pressure.
+    const: aeolus.const.const.ConstContainer, optional
+        Required if p_ref_frac=True.
+        If not given, constants are attempted to be retrieved from
+        attributes of a cube in the cube list.
+    interpolator: callable or None
+        The interpolator to use when computing the interpolation.
+        See `relevel()` docs for more.
+    model: aeolus.model.Model, optional
+        Model class with relevant variable names.
+
+    Returns
+    -------
+    iris.cube.Cube
+        The variable interpolated to pressure level(s).
+    """
+    from iris.experimental import stratify
+
+    if p_ref_frac:
+        p_ref = const.reference_surface_pressure.copy()
+        p_ref.convert_units(pressure.units)
+        p_tgt = np.atleast_1d(levels) * float(p_ref.data)
+    else:
+        p_tgt = np.atleast_1d(levels)
+    cube_plev = stratify.relevel(
+        variable, pressure, p_tgt, axis=model.z, interpolator=interpolator
+    )
+    cube_plev.coord(model.pres).attributes = {}
+    return squeeze(cube_plev)
+
+
+@const_from_attrs(strict=False)
+def interp_cubelist_from_height_to_pressure_levels(
+    cubelist,
+    levels,
+    p_ref_frac=False,
+    const=None,
+    interpolator=None,
+    model=um,
+    include_pressure=False,
+):
+    """
+    Interpolate all cubes to the given set of pressure levels.
+
+    Pressure variable is found using the `model.pres` name and then optionally
+    excluded from the output list of interpolated cubes.
 
     Parameters
     ----------
     cubelist: iris.cube.CubeList
         List of cubes, including a cube of pressure.
     levels: array-like
-        Sequence of pressure levels (same units as the units of pressure cube in `cubelist`).
+        Sequence of pressure levels
+        (same units as the units of pressure cube in `cubelist`).
+    p_ref_frac: bool, optional
+        If True, `levels` are used as fractions of the surface pressure.
+    const: aeolus.const.const.ConstContainer, optional
+        Required if p_ref_frac=True.
+        If not given, constants are attempted to be retrieved from
+        attributes of a cube in the cube list.
     interpolator: callable or None
-        The interpolator to use when computing the interpolation. See relevel() docs for more.
+        The interpolator to use when computing the interpolation.
+        See `relevel()` docs for more.
     model: aeolus.model.Model, optional
         Model class with relevant variable names.
+    include_pressure: bool, optional
+        If True, include the pressure cube in the output.
 
     Returns
     -------
     iris.cube.CubeList
         List of cubes interpolated to pressure level(s).
     """
     pres = cubelist.extract_cube(model.pres)
-    cl_out = iris.cube.CubeList()
+    cl_out = CubeList()
     for cube in cubelist:
-        if cube != pres:
-            cube_plev = interp_to_pres_lev(
-                cubelist, cube.name(), levels, interpolator=interpolator, model=model
+        if include_pressure or cube != pres:
+            cube_plev = interp_cube_from_height_to_pressure_levels(
+                cube,
+                pres,
+                levels,
+                p_ref_frac=p_ref_frac,
+                const=const,
+                interpolator=interpolator,
+                model=model,
             )
-            cube_plev.coord(model.pres).attributes = {}
             cl_out.append(cube_plev)
     return cl_out
 
 
 def interp_to_cube_time(cube_src, cube_tgt, model=um):
     """
-    Linearly interpolate `cube_src` to `cube_tgt` along the time dimension (`model.t`).
+    Interpolate `cube_src` to `cube_tgt` along the time dimension (`model.t`).
 
-    Forecast period is copied from `cube_tgt`.
+    Linear interpolation is used. Forecast period is copied from `cube_tgt`.
 
     Parameters
     ----------
     cube_src: iris.cube.Cube
         Cube to interpolate.
     cube_tgt: iris.cube.Cube
         Cube with time dimension to interpolate to.
@@ -685,85 +802,14 @@
         try:
             out.replace_coord(cube_tgt.coord(getattr(model, coord)))
         except (AttributeError, CoNotFound):
             pass
     return out
 
 
-def interp_to_pres_lev(cubelist, constraint, levels, interpolator=None, model=um):
-    """
-    Interpolate a cube to pressure level(s) using stratify relevel() function.
-
-    Parameters
-    ----------
-    cubelist: iris.cube.CubeList
-        List of cubes containing a cube extractable by `constraint` and a cube of pressure.
-    constraint: str or iris.Constraint
-        Variable name or constraint to extract a cube from `cubelist`.
-    levels: array-like
-        Sequence of pressure levels (same units as the units of pressure cube in `cubelist`).
-    interpolator: callable or None
-        The interpolator to use when computing the interpolation. See relevel() docs for more.
-    model: aeolus.model.Model, optional
-        Model class with relevant variable names.
-
-    Returns
-    -------
-    iris.cube.Cube
-        Cube of `varname` interpolated to pressure level(s).
-    """
-    cube = cubelist.extract_cube(constraint)
-    pres = cubelist.extract_cube(model.pres)
-    cube_plev = stratify.relevel(cube, pres, levels, axis=model.z, interpolator=interpolator)
-    cube_plev.coord(model.pres).attributes = {}
-    return iris.util.squeeze(cube_plev)
-
-
-def interp_to_single_pres_lev(
-    cubelist, constraint, p_ref_frac=0.5, const=None, interpolator=None, model=um
-):
-    """
-    Interpolate the field defined by `constraint` to a single pressure level.
-
-    The level is found from the given fraction of the reference surface pressure.
-
-    Parameters
-    ----------
-    cubelist: iris.cube.CubeList
-        Input cubelist.
-    constraint: str or iris.Constraint
-        Variable name or constraint to extract a cube from `cubelist`.
-    p_ref_frac: float, optional
-        Fraction of reference surface pressure at which the estimate is made.
-        The default value is 0.1, which for an Earth-like atmosphere means 100 hPa.
-    const: aeolus.const.const.ConstContainer, optional
-        If not given, constants are attempted to be retrieved from
-        attributes of a cube in the cube list.
-    interpolator: callable or None
-        The interpolator to use when computing the interpolation. See relevel() docs for more.
-    model: aeolus.model.Model, optional
-        Model class with relevant variable names.
-
-    Returns
-    -------
-    iris.cube.Cube
-        Cube on a single pressure level.
-    """
-    if const is None:
-        const = cubelist[0].attributes["planet_conf"]
-    p_ref = const.reference_surface_pressure
-    p_tgt = p_ref_frac * p_ref
-    pres = cubelist.extract_cube(model.pres)
-    p_tgt.convert_units(pres.units)
-    out = interp_to_pres_lev(
-        cubelist, constraint, [p_tgt.data], interpolator=interpolator, model=model
-    )
-    return out
-
-
 def isel(obj, coord, idx, skip_not_found=None):
     """
     Slice cubes by an index of a coordinate (index-selector).
 
     Parameters
     ----------
     obj: iris.cube.Cube or iris.cube.CubeList
@@ -777,34 +823,43 @@
         a cube list and inactive if dealing with a single cube.
 
     Returns
     -------
     iris.cube.Cube or iris.cube.CubeList
         Slice along the coordinate.
     """
-    if isinstance(obj, iris.cube.Cube):
+    if isinstance(obj, Cube):
         try:
-            _coord = obj.coord(coord)
-            val = _coord.points[idx]
-            try:
-                val = _coord.units.num2date(val)
-            except ValueError:
-                pass
-            constr = iris.Constraint(**{_coord.name(): lambda x: x.point == val})
-            out = obj.extract(constr)
+            # _coord = obj.coord(coord)
+            # val = _coord.points[idx]
+            # try:
+            #     val = _coord.units.num2date(val)
+            # except ValueError:
+            #     pass
+            # constr = Constraint(**{_coord.name(): lambda x: x.point == val})
+            # out = obj.extract(constr)
+            val = obj.coord(coord)[idx]
+            out = squeeze(obj.subset(val))
         except CoNotFound as e:
             if skip_not_found:
                 out = obj
             else:
                 raise e
     elif isinstance(obj, (list, set, tuple)):
         out = []
         for cube in obj:
             out.append(
-                isel(cube, coord, idx, skip_not_found=((skip_not_found is None) or skip_not_found))
+                isel(
+                    cube,
+                    coord,
+                    idx,
+                    skip_not_found=(
+                        (skip_not_found is None) or skip_not_found
+                    ),
+                )
             )
         out = obj.__class__(out)
     return out
 
 
 def nearest_coord_value(cube, coord_name, val):
     """
@@ -828,25 +883,27 @@
     i = coord.nearest_neighbour_index(val)
     return coord.points[i]
 
 
 def not_equal_coord_axes(cube1, cube2):
     """Given 2 cubes, return axes of unequal dimensional coordinates."""
     coord_comp = iris.analysis._dimensional_metadata_comparison(cube1, cube2)
-    neq_dim_coords = set(coord_comp["not_equal"]).intersection(set(coord_comp["dimensioned"]))
+    neq_dim_coords = set(coord_comp["not_equal"]).intersection(
+        set(coord_comp["dimensioned"])
+    )
     dims = []
     for coord_pair in neq_dim_coords:
         for coord in coord_pair:
-            dims.append(iris.util.guess_coord_axis(coord))
+            dims.append(guess_coord_axis(coord))
     return set(filter(None, dims))
 
 
 def regrid_3d(cube, target, model=um):
     """
-    Regrid a cube in the horizontal and in the vertical on to coordinates of the target cube.
+    Regrid a cube in the horizontal and in the vertical.
 
     Adapted from https://github.com/LSaffin/iris-extensions
 
     Parameters
     ----------
     cube: iris.cube.Cube
         The cube to be regridded.
@@ -903,115 +960,134 @@
     Returns
     -------
     iris.cube.Cube
         Copy of the input cube with a new vertical coordinate.
     """
     new_cube = cube.copy()
     new_cube.coord(model.z).bounds = None
-    iris.util.promote_aux_coord_to_dim_coord(new_cube, model.z)
+    promote_aux_coord_to_dim_coord(new_cube, model.z)
     ensure_bounds(new_cube, coords=[model.z])
     for coord in [model.s, model.lev]:
         # By default, model levels and sigma coordinates are removed.
         try:
             new_cube.remove_coord(coord)
         except CoNotFound:
             pass
     return new_cube
 
 
-def roll_cube_0_360(cube_in, model=um):
+def roll_cube_0_360(cube_in, add_shift=0, model=um):
     """
-    Take a cube spanning -180...180 degrees in longitude and roll it to 0...360 degrees.
+    Take a cube spanning -180...180 degrees and roll it to 0...360 degrees.
 
     Works with global model output, and in some cases for regional.
 
     Parameters
     ----------
     cube: iris.cube.Cube
         Cube with longitude and latitude coordinates.
+    add_shift: int
+        Additional shift of data (is not applied to the longitude coordinate).
     model: aeolus.model.Model, optional
         Model class with a relevant longitude coordinate name.
 
     Returns
     -------
     iris.cube.Cube
 
-    See also
+    See Also
     --------
     aeolus.coord.roll_cube_pm180
     """
     cube = cube_in.copy()
     coord_name = model.x  # get the name of the longitude coordinate
     lon = cube.coord(coord_name)
     if (lon.points < 0.0).any():
         add = 180
-        cube.data = np.roll(cube.data, len(lon.points) // 2, axis=-1)
+        cube.data = da.roll(
+            cube.core_data(), len(lon.points) // 2 + add_shift, axis=-1
+        )
         if lon.has_bounds():
             bounds = lon.bounds + add
         else:
             bounds = None
-        cube.replace_coord(lon.copy(points=lon.points + add, bounds=bounds))
+        new_points = lon.points + add
+        cube.replace_coord(lon.copy(points=new_points, bounds=bounds))
     return cube
 
 
-def roll_cube_pm180(cube_in, model=um):
+def roll_cube_pm180(cube_in, add_shift=0, model=um):
     """
-    Take a cube spanning 0...360 degrees in longitude and roll it to -180...180 degrees.
+    Take a cube spanning 0...360 degrees and roll it to -180...180 degrees.
 
     Works with global model output, and in some cases for regional.
 
     Parameters
     ----------
     cube: iris.cube.Cube
         Cube with longitude and latitude coordinates.
+    add_shift: int
+        Additional shift of data (is not applied to the longitude coordinate).
     model: aeolus.model.Model, optional
         Model class with a relevant longitude coordinate name.
 
     Returns
     -------
     iris.cube.Cube
 
-    See also
+    See Also
     --------
     aeolus.coord.roll_cube_0_360
     """
     cube = cube_in.copy()
     coord_name = model.x  # get the name of the longitude coordinate
     xcoord = cube.coord(coord_name)
     if (xcoord.points >= 0.0).all():
-        assert is_regular(xcoord), "Operation is only valid for a regularly spaced coordinate."
+        assert is_regular(
+            xcoord
+        ), "Operation is only valid for a regularly spaced coordinate."
         if _is_longitude_global(xcoord.points):
             # Shift data symmetrically only when dealing with global cubes
-            cube.data = np.roll(cube.data, len(xcoord.points) // 2, axis=-1)
+            cube.data = da.roll(
+                cube.core_data(), len(xcoord.points) // 2 + add_shift, axis=-1
+            )
 
         if xcoord.has_bounds():
             bounds = wrap_lons(xcoord.bounds, -180, 360)  # + subtract
             bounds = bounds[bounds[:, 0].argsort(axis=0)]
         else:
             bounds = None
         cube.replace_coord(
-            xcoord.copy(points=np.sort(wrap_lons(xcoord.points, -180, 360)), bounds=bounds)
+            xcoord.copy(
+                points=np.sort(wrap_lons(xcoord.points, -180, 360)),
+                bounds=bounds,
+            )
         )
     else:
         # Nothing to do, the cube is already centered on 0 longitude
         # unless there is something wrong with longitude
-        msg = f"Incorrect {coord_name} values: from {xcoord.points.min()} to {xcoord.points.max()}"
-        assert ((xcoord.points >= -180.0) & (xcoord.points <= 180.0)).all(), msg
+        msg = (
+            f"Incorrect {coord_name} values: "
+            f"from {xcoord.points.min()} to {xcoord.points.max()}"
+        )
+        assert (
+            (xcoord.points >= -180.0) & (xcoord.points <= 180.0)
+        ).all(), msg
     return cube
 
 
 def vertical_cross_section_area(cube2d, r_planet=None):
     """Create a cube of vertical cross-section areas in metres."""
     cube2d = cube2d.copy()
     if r_planet is None:
         r = get_planet_radius(cube2d)
     else:
         r = r_planet
     m_per_deg = (np.pi / 180) * r
-    if iris.util.guess_coord_axis(cube2d.dim_coords[1]) == "X":
+    if guess_coord_axis(cube2d.dim_coords[1]) == "X":
         m_per_deg *= np.cos(np.deg2rad(cube2d.coord(axis="Y").points[0]))
 
     for dim_coord in cube2d.dim_coords:
         if not dim_coord.has_bounds():
             dim_coord.guess_bounds()
     x_bounds = cube2d.coord(cube2d.dim_coords[1]).bounds
     z_bounds = cube2d.coord(cube2d.dim_coords[0]).bounds
@@ -1044,15 +1120,17 @@
         Model class with relevant coordinate names.
 
     Returns
     -------
     iris.cube.Cube
         Cube of area weights with the same metadata as the input cube
     """
-    area_cube = area_weights_cube(cube, r_planet=r_planet, normalize=normalize, model=model)
+    area_cube = area_weights_cube(
+        cube, r_planet=r_planet, normalize=normalize, model=model
+    )
     height_deltas = coord_delta_to_cube(cube, model.z, normalize=normalize)
     volume = area_cube * height_deltas
     if normalize:
         volume.rename("normalized_volume_weights")
         volume.convert_units("1")
     else:
         volume.rename("volume_weights")
```

### Comparing `aeolus-0.4.9/src/aeolus/exceptions.py` & `aeolus-24.4.29.1/src/aeolus/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# -*- coding: utf-8 -*-
 """Exceptions specific to aeolus package."""
+
 from warnings import warn
 
 
 def _warn(msg):
     """Raise an aeolus-related warning."""
-    warn(msg, AeolusWarning)
+    warn(msg, AeolusWarning, stacklevel=2)
 
 
 class AeolusWarning(UserWarning):
     """Base class for warnings in aeolus package."""
 
     pass
```

### Comparing `aeolus-0.4.9/src/aeolus/model/base.py` & `aeolus-24.4.29.1/src/aeolus/model/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """Model-specific dictionaries of variable names and coordinates."""
-from dataclasses import dataclass
 
+from dataclasses import dataclass
+import textwrap
 
 __all__ = "Model"
 
 
 @dataclass
 class Model:
     """Base class for model-specific names."""
 
+    def __hash__(self):  # noqa
+        return hash(id(self))
+
     # Coordinates
     t: str = None  # time
     fcst_ref: str = None  # forecast reference
     fcst_prd: str = None  # forecast period
     z: str = None  # height
     lev: str = None  # level number
     s: str = None  # sigma
@@ -37,37 +41,48 @@
     toa_olr_cs: str = None
     toa_osr: str = None
     toa_osr_cs: str = None
     sfc_dn_lw: str = None
     sfc_dn_lw_cs: str = None
     sfc_dn_sw: str = None
     sfc_dn_sw_cs: str = None
+    sfc_up_lw: str = None
+    sfc_up_lw_cs: str = None
+    sfc_up_sw: str = None
+    sfc_up_sw_cs: str = None
     sfc_net_down_lw: str = None
     sfc_net_down_sw: str = None
     lw_up: str = None
+    lw_up_forcing: str = None
+    lw_dn_forcing: str = None
     sw_up: str = None
     lw_dn: str = None
     sw_dn: str = None
     lw_up_cs: str = None
     sw_up_cs: str = None
     lw_dn_cs: str = None
     sw_dn_cs: str = None
     # BL
     sfc_shf: str = None
     sfc_lhf: str = None
     sfc_evap: str = None
+    sfc_x_wind_stress: str = None
+    sfc_y_wind_stress: str = None
     # Extra physics
     temp: str = None
     dens: str = None
     ghgt: str = None
     rh: str = None
     # Precip & Cloud
     cld_ice_mf: str = None
     cld_liq_mf: str = None
     rain_mf: str = None
+    cca_anvil: str = None
+    ccw_rad: str = None
+    cld_top_hgt: str = None
     cld_ice_v: str = None
     cld_liq_v: str = None
     cld_v: str = None
     caf: str = None
     caf_h: str = None
     caf_m: str = None
     caf_l: str = None
@@ -91,14 +106,47 @@
     dq_sw: str = None
     dq_lw: str = None
     dq_lsppn: str = None
     dq_bl: str = None
     dq_cv: str = None
     dq_lscld: str = None
     dq_adv: str = None
+    # Increments of eastward wind
+    du_bl: str = None
+    du_cv: str = None
+    du_solve: str = None
+    du_adv: str = None
+    du_total: str = None
     # Soil
     soil_moist: str = None
+    # Eliassen-Palm flux
+    ep_flux_y: str = None
+    ep_flux_z: str = None
+    ep_flux_div: str = None
+    # Lightning
+    light_flash_rate: str = None
+    light_number: str = None
 
     def __repr__(self):
         """Override the repr method of the dataclass."""
-        size = len([_ for _, v in self.__dataclass_fields__.items() if v.name is not None])
-        return f"{self.__class__}({size} fields)"
+        size = len(
+            [
+                _
+                for _, v in self.__dataclass_fields__.items()
+                if v.name is not None
+            ]
+        )
+        return f"{self.__class__.__name__} [{size} fields]"
+
+    def __str__(self):
+        """Override the str method of the dataclass."""
+        fields = [
+            v.name
+            for _, v in self.__dataclass_fields__.items()
+            if v.name is not None
+        ]
+        size = len(fields)
+        s = (
+            f"{self.__class__.__name__} with {size} fields:"
+            f"\n{', '.join(fields)}"
+        )
+        return "\n".join(textwrap.wrap(s, 100))
```

### Comparing `aeolus-0.4.9/src/aeolus/plot/cart.py` & `aeolus-24.4.29.1/src/aeolus/plot/cart.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 """Plotting functions used with cartopy."""
+
 import cartopy.crs as ccrs
 from cartopy.mpl.geoaxes import GeoAxes
-
 from matplotlib.transforms import offset_copy
-
 from mpl_toolkits.axes_grid1 import AxesGrid
 
 from .text import fmt_lonlat
 
-
 __all__ = ("GeoAxesGrid", "label_global_map_gridlines")
 
 
 class GeoAxesGrid(AxesGrid):
     """
     Grid of cartopy axes.
 
@@ -34,19 +32,26 @@
         in :class:`~matplotlib.figure.Figure` *fig* with
         *rect=[left, bottom, width, height]* (in
         :class:`~matplotlib.figure.Figure` coordinates) or
         the subplot position code (e.g., "121").
         """
         axesgrid_kw["axes_class"] = (GeoAxes, {"map_projection": projection})
         axesgrid_kw["label_mode"] = ""  # note the empty label_mode
-        super(GeoAxesGrid, self).__init__(fig, rect, nrows_ncols, **axesgrid_kw)
+        super().__init__(fig, rect, nrows_ncols, **axesgrid_kw)
 
 
 def label_global_map_gridlines(
-    fig, ax, xticks=[], yticks=[], xoff=-10, yoff=-10, degree=False, **text_kw
+    fig,
+    ax,
+    xticks=None,
+    yticks=None,
+    xoff=-10,
+    yoff=-10,
+    degree=False,
+    **text_kw,
 ):
     """
     Label gridlines of a global cartopy map.
 
     Parameters
     ----------
     fig: matplotlib.figure.Figure
@@ -67,31 +72,43 @@
         otherwise at the north boundary.
     degree: bool, optional
         Add a degree symbol to tick labels.
     **text_kw: dict, optional
         Label text properties.
     """
     # Define what boundary to use
+    if yticks is None:
+        yticks = []
+    if xticks is None:
+        xticks = []
     extent = ax.get_extent(crs=ccrs.PlateCarree())
     if xoff <= 0:
         xpos = extent[0]  # labels at the east boundary
     else:
         xpos = extent[1]  # labels at the west boundary
     if yoff <= 0:
         ypos = extent[2]  # labels at the south boundary
     else:
         ypos = extent[3]  # labels at the north boundary
     geodetic_trans = ccrs.Geodetic()
     xlab_kw = ylab_kw = {**{"va": "center", "ha": "center"}, **text_kw}
     for xtick in xticks:
         s = fmt_lonlat(xtick, "lon", degree=degree)
         text_transform = offset_copy(
-            geodetic_trans._as_mpl_transform(ax), fig=fig, units="points", x=0, y=yoff
+            geodetic_trans._as_mpl_transform(ax),
+            fig=fig,
+            units="points",
+            x=0,
+            y=yoff,
         )
         ax.text(xtick, ypos, s, transform=text_transform, **xlab_kw)
 
     for ytick in yticks:
         s = fmt_lonlat(ytick, "lat", degree=degree)
         text_transform = offset_copy(
-            geodetic_trans._as_mpl_transform(ax), fig=fig, units="points", x=xoff, y=0
+            geodetic_trans._as_mpl_transform(ax),
+            fig=fig,
+            units="points",
+            x=xoff,
+            y=0,
         )
         ax.text(xpos, ytick, s, transform=text_transform, **ylab_kw)
```

### Comparing `aeolus-0.4.9/src/aeolus/plot/cloud.py` & `aeolus-24.4.29.1/src/aeolus/plot/cloud.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """Utilities to plot cloud-related output of UM."""
-import warnings
 
 import iris
-
 import matplotlib as mpl
-
 import numpy as np
 
+from ..exceptions import _warn
 from .cm_custom import cloudtypes_cmap
 
-
 __all__ = ("CloudPlotter", "cloudtypes_cmap")
 
 
 class CloudPlotter:
-    """Factory to create a composite plot of low, medium, high cloud area fractions."""
+    """Factory to create a plot of low, medium, high cloud area fractions."""
 
     _stash_items = {"lo": "m01s09i203", "me": "m01s09i204", "hi": "m01s09i205"}
     _scales = {"lo": 100, "me": 200, "hi": 400}
     cloud_labels = [
         "No\nCloud",
         "L",
         "M",
@@ -26,43 +23,52 @@
         "H",
         "H + L",
         "H + M",
         "All",
     ]
 
     def __init__(self, cubelist):
-        """Initialise CloudPlotter from `iris.cube.CubeList` containing cloud fractions."""
+        """Initialise CloudPlotter."""
         self.factor = 10.0  # scaling factor
         self.cubes = {}
         for key, stash in self._stash_items.items():
             try:
-                self.cubes[key] = cubelist.extract_cube(iris.AttributeConstraint(STASH=stash))
+                self.cubes[key] = cubelist.extract_cube(
+                    iris.AttributeConstraint(STASH=stash)
+                )
             except iris.exceptions.ConstraintMismatchError:
-                warnings.warn(f"Warning!\n{key} ({stash}) is not found in\n\n{cubelist}")
+                _warn(
+                    f"Warning!\n{key} ({stash}) is not found in\n\n{cubelist}"
+                )
 
     def scale_data(self, threshold=0.1):
         """
-        Scale cloud levels and add them together to make a composite cloud field.
+        Scale cloud levels & add them together to make a composite cloud field.
 
         Values below `threshold` are set to zero.
         """
         for i, (key, cube) in enumerate(self.cubes.items()):
             cp_cube = cube.copy(
                 data=np.where(
-                    cube.data >= threshold, cube.data * self.factor + self._scales[key], 0.0
+                    cube.data >= threshold,
+                    cube.data * self.factor + self._scales[key],
+                    0.0,
                 )
             )
             if i == 0:
                 self.aggr_cld = cp_cube
             else:
                 self.aggr_cld += cp_cube
         self.aggr_cld.rename("aggregated_cloud_fraction")
         self.aggr_cld.attributes["source"] = " + ".join(
             [
-                (f"({self._stash_items[k]}*{self.factor}" f"+{self._scales[k]})")
+                (
+                    f"({self._stash_items[k]}*{self.factor}"
+                    f"+{self._scales[k]})"
+                )
                 for k in self.cubes.keys()
             ]
         )
 
     def _make_norm(self, cmap, nsteps):
         """
         Create `BoundaryNorm` for cloud levels.
@@ -71,46 +77,59 @@
         Also returns `midpoints` used for colorbar labelling.
         """
         base = np.linspace(0, self.factor, nsteps) + 1
         assert nsteps > 0, "number of intervals should be positive"
         lvls = [base]  # no clouds
         lvls.append(base + self._scales["lo"])  # low clouds (101-110)
         lvls.append(base + self._scales["me"])  # medium clouds (201-210)
-        lvls.append(base * 2 + self._scales["lo"] + self._scales["me"])  # low + medium (302-320)
+        lvls.append(
+            base * 2 + self._scales["lo"] + self._scales["me"]
+        )  # low + medium (302-320)
         lvls.append(base + self._scales["hi"])  # high clouds (401-410)
-        lvls.append(base * 2 + self._scales["lo"] + self._scales["hi"])  # high + low (502-520)
-        lvls.append(base * 2 + self._scales["hi"] + self._scales["me"])  # high + medium (602-620)
         lvls.append(
-            base * 3 + self._scales["lo"] + self._scales["me"] + self._scales["hi"]
+            base * 2 + self._scales["lo"] + self._scales["hi"]
+        )  # high + low (502-520)
+        lvls.append(
+            base * 2 + self._scales["hi"] + self._scales["me"]
+        )  # high + medium (602-620)
+        lvls.append(
+            base * 3
+            + self._scales["lo"]
+            + self._scales["me"]
+            + self._scales["hi"]
         )  # high + medium + low (703-730)
         lvls.append([1000])
         midpoints = []
         if nsteps == 1:
             for lvl1, lvl2 in zip(lvls[:-1], lvls[1:]):
                 midpoints.append(0.5 * (lvl1[-1] + lvl2[0]))
         else:
             for lvl in lvls[:-1]:
                 if len(lvl) % 2 == 0:
                     midpoints.append(lvl[len(lvl) // 2])
                 else:
-                    midpoints.append(0.5 * (lvl[len(lvl) // 2] + lvl[(len(lvl) // 2) + 1]))
+                    midpoints.append(
+                        0.5 * (lvl[len(lvl) // 2] + lvl[(len(lvl) // 2) + 1])
+                    )
         midpoints = np.asarray(midpoints)
         norm = mpl.colors.BoundaryNorm(np.concatenate(lvls), cmap.N)
         return norm, midpoints
 
     def get_all(self, nsteps=10, cmap=None):
         """Get cloud types cube and kwargs for external plotting."""
         if cmap is None:
             cmap = cloudtypes_cmap  # colormap from a separate file
         norm, cb_ticks = self._make_norm(cmap=cmap, nsteps=nsteps)
         plt_kw = {"norm": norm, "cmap": cmap}
         cb_labels = self.cloud_labels
         return self.aggr_cld, plt_kw, cb_ticks, cb_labels
 
-    def pcolormesh(self, ax, xy=(), nsteps=10, cmap=None, cb_kwargs={}, **pc_kwargs):
+    def pcolormesh(
+        self, ax, xy=(), nsteps=10, cmap=None, cb_kwargs=None, **pc_kwargs
+    ):
         """
         Display composite cloud plot using `matplotlib.pyplot.pcolormesh`.
 
         Parameters
         ----------
         ax: matplotlib axes object
             Axes where to create the plot in
@@ -120,26 +139,31 @@
             Number of colour steps for each of cloud category
         cmap: matplotlib.colors.ListedColormap, optional
             Colormap instance. If not given, custom cloud colormap is used.
         cb_kwags: dict, optional
             Dictionary of kwargs passed to colorbar
         **pc_kwargs: optional
             additional pcolormesh arguments
+
         Returns
         -------
         h: `matplotlib.collections.QuadMesh`
             pcolormesh instance
         cb: `matplotlib.colorbar.Colorbar`
             colorbar
         """
+        if cb_kwargs is None:
+            cb_kwargs = {}
         fig = ax.figure
         if cmap is None:
             cmap = cloudtypes_cmap  # colormap from a separate file
         norm, midpoints = self._make_norm(cmap=cmap, nsteps=nsteps)
-        h = ax.pcolormesh(*xy, self.aggr_cld.data, cmap=cmap, norm=norm, **pc_kwargs)
+        h = ax.pcolormesh(
+            *xy, self.aggr_cld.data, cmap=cmap, norm=norm, **pc_kwargs
+        )
         if "cax" in cb_kwargs:
             ax_kw = {}
         else:
             ax_kw = {"ax": ax}
         cb = fig.colorbar(h, **ax_kw, **cb_kwargs)
         cb.set_ticks(midpoints)
         cb.set_ticklabels(self.cloud_labels)
```

### Comparing `aeolus-0.4.9/src/aeolus/plot/cm_custom.py` & `aeolus-24.4.29.1/src/aeolus/plot/cm_custom.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Custom colormaps."""
+
 from matplotlib.colors import ListedColormap
 
 __all__ = ("cloudtypes_cmap",)
 
 _cloudtypes_data = [
     [1.000_000, 0.984_314, 0.992_157],
     [1.000_000, 0.984_314, 0.992_157],
```

### Comparing `aeolus-0.4.9/src/aeolus/plot/pv.py` & `aeolus-24.4.29.1/src/aeolus/plot/pv.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,96 @@
 """Prepare data in spherical coordinates for pyvista plotting."""
-import numpy as np
 
+from typing import Optional
+
+import geovista as gv
+import iris
+import numpy as np
+import pyvista as pv
 from pyvista import grid_from_sph_coords, transform_vectors_sph_to_cart
 
 from ..coord import _cell_bounds
 from ..exceptions import _warn
 from ..model import um
+from ..model.base import Model
 
-
-__all__ = ("grid_for_scalar_cube_sph", "grid_for_vector_cubes_sph")
-
-
-def grid_for_scalar_cube_sph(cube, z_scale=1, z_offset=0, grid=None, label="scalar3d", model=um):
+__all__ = (
+    "grid_for_scalar_cube_sph",
+    "grid_for_vector_cubes_sph",
+    "ugrid_mesh_to_gv_mesh",
+)
+
+
+def grid_for_scalar_cube_sph(
+    cube: iris.cube.Cube,
+    z_scale: Optional[float] = 1,
+    z_offset: Optional[float] = 0,
+    grid: Optional[pv.StructuredGrid] = None,
+    label: Optional[str] = "scalar3d",
+    model: Optional[Model] = um,
+) -> pv.PolyData:
     """
-    Create a `pyvista` grid for an `iris` cube (2D or 3D) in spherical coordinates.
+    Create a `pyvista` grid for an `iris` cube in spherical coordinates.
 
     Parameters
     ----------
     cube: iris.cube.Cube
         2D or 3D cube with (longitude, latitude, [level_height]) coordinates.
     z_scale: float, optional
         Scaling factor for the vertical level dimension.
     z_offset: float, optional
         Scaling offset for the vertical level dimension.
     grid: pyvista.StructuredGrid, optional
-        If given, add data to the existing grid, otherwise create a new one from
-        the input cube's coordinates.
+        If given, add data to the existing grid, otherwise create a new one
+        from the input cube's coordinates.
     label: str, optional
         Label for the data within the grid.
     model: aeolus.model.Model, optional
         Model class with relevant variable names.
 
     Returns
     -------
     pyvista.StructuredGrid
-       PyVista grid with data in cell_arrays.
+       PyVista grid with data in the cell_data attribute.
     """
     if grid is None:
         lons = _cell_bounds(cube.coord(model.x).points)
         lats = 90.0 - _cell_bounds(cube.coord(model.y).points)
         if cube.ndim == 3:
             # TODO check if _cell_bounds should be here
             levels = _cell_bounds(cube.coord(model.z).points)
         else:
             levels = np.array([0])
         levels = z_scale * levels + z_offset
 
         grid = grid_from_sph_coords(lons, lats, levels)
 
     # Add data arras to grid
-    if label in grid.cell_arrays:
+    if label in grid.cell_data:
         _warn(f"Label '{label}' exists in {grid}")
-    grid.cell_arrays[label] = np.array(cube.data).swapaxes(-2, -1).ravel("C")
+    grid.cell_data[label] = np.array(cube.data).swapaxes(-2, -1).ravel("C")
     return grid
 
 
 def grid_for_vector_cubes_sph(
-    u,
-    v,
-    w,
-    vector_scale=1,
-    vertical_wind_scale=1,
-    z_scale=1,
-    z_offset=0,
-    xstride=1,
-    ystride=1,
-    grid=None,
-    label="vector3d",
-    model=um,
-):
+    u: iris.cube.Cube,
+    v: iris.cube.Cube,
+    w: iris.cube.Cube,
+    vector_scale: Optional[float] = 1,
+    vertical_wind_scale: Optional[float] = 1,
+    z_scale: Optional[float] = 1,
+    z_offset: Optional[float] = 0,
+    xstride: Optional[int] = 1,
+    ystride: Optional[int] = 1,
+    grid: Optional[pv.StructuredGrid] = None,
+    label: Optional[str] = "vector3d",
+    model: Optional[Model] = um,
+) -> pv.PolyData:
     """
-    Take wind vectors in spherical coordinates and create a `pyvista` grid for them.
+    Take winds in spherical coordinates and create a `pyvista` grid for them.
 
     Parameters
     ----------
     u: iris.cube.Cube
         2D or 3D cube of x-wind component (zonal wind).
     v: iris.cube.Cube
         2D or 3D cube of y-wind component (meridional wind).
@@ -89,25 +105,25 @@
     z_offset: float, optional
         Scaling offset for the vertical level dimension.
     xstride: float, optional
         Stride along the longitude axis.
     ystride: float, optional
         Stride along the latitude axis.
     grid: pyvista.StructuredGrid, optional
-        If given, add data to the existing grid, otherwise create a new one from
-        the input cube's coordinates.
+        If given, add data to the existing grid, otherwise create a new one
+        from the input cube's coordinates.
     label: str, optional
         Label for the data within the grid.
     model: aeolus.model.Model, optional
         Model class with relevant variable names.
 
     Returns
     -------
     pyvista.StructuredGrid
-       PyVista grid with vector data in point_arrays.
+       PyVista grid with vector data in the point_data attribute.
     """
     assert (u.shape == v.shape) and (
         u.shape == w.shape
     ), "Wind components should have the same array size!"
 
     lons = u.coord(model.x).points
     lats = 90.0 - u.coord(model.y).points
@@ -122,15 +138,15 @@
     u_sdata = u.data[..., ::ystride, ::xstride].transpose(inv_axes)
     v_sdata = v.data[..., ::ystride, ::xstride].transpose(inv_axes)
     w_sdata = w.data[..., ::ystride, ::xstride].transpose(inv_axes)
 
     # Rescale vertical wind for better viz
     w_sdata *= vertical_wind_scale
 
-    # Create a stack of vectors transformed from spherical to cartesian coordinates
+    # Create a stack of vectors transformed from spherical to cartesian coords
     vectors = np.stack(
         [
             i.transpose(inv_axes).swapaxes(u.ndim - 2, u.ndim - 1).ravel("C")
             for i in transform_vectors_sph_to_cart(
                 lons_s, lats_s, levels, u_sdata, -v_sdata, w_sdata
             )
         ],
@@ -139,9 +155,28 @@
     # Scale vectors
     vectors *= vector_scale
 
     if grid is None:
         grid = grid_from_sph_coords(lons_s, lats_s, levels)
 
     # Add vectors to the grid
-    grid.point_arrays[label] = vectors
+    grid.point_data[label] = vectors
     return grid
+
+
+def ugrid_mesh_to_gv_mesh(
+    topology: iris.experimental.ugrid.mesh.Mesh, **kwargs
+) -> pv.PolyData:
+    """Create a geovista mesh from the LFRic mesh."""
+    face_node = topology.face_node_connectivity
+
+    indices = face_node.indices_by_location()
+
+    lons, lats = topology.node_coords
+
+    return gv.Transform.from_unstructured(
+        lons.points,
+        lats.points,
+        indices,
+        start_index=face_node.start_index,
+        **kwargs,
+    )
```

### Comparing `aeolus-0.4.9/tests/test_const.py` & `aeolus-24.4.29.1/tests/test_const.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 """Test calc submodule."""
-from pathlib import Path
-
-from aeolus import const
-from aeolus.exceptions import ArgumentError, LoadError
 
-import iris
+from pathlib import Path
 
+import iris.cube
 import numpy.testing as npt
-
 import pytest
 
+from aeolus import const
+from aeolus.exceptions import ArgumentError, LoadError
 
-TST_DATA = Path(__file__).parent / "data"
+TST_DATA = Path(__file__).parent / "data" / "test_data"
 CONST_FILE = "dummy"
 
 
 def test_init_const_general():
-    """Test init_const function w/o arguments."""
     cnsts = const.init_const()
     assert str(cnsts).startswith("GeneralConstants")
     assert isinstance(cnsts, const.const.ConstContainer)
     for key in cnsts.__dataclass_fields__.keys():
         attr = getattr(cnsts, key)
         assert isinstance(attr, iris.cube.Cube)
         assert attr.ndim == 0  # XXX could be relaxed
@@ -28,30 +25,29 @@
     assert key in cnsts.__dataclass_fields__
     cube = getattr(cnsts, key)
     assert cube.units == "W m-2 K-4"
     npt.assert_allclose(cube.data, 5.670367e-08)
 
 
 def test_loaderror():
-    """Test raising LoadError."""
     with pytest.raises(LoadError):
         const.init_const(CONST_FILE)
     with pytest.raises(LoadError):
-        const.init_const(CONST_FILE, directory=TST_DATA / "nonexistent_directory")
+        const.init_const(
+            CONST_FILE, directory=TST_DATA / "nonexistent_directory"
+        )
 
 
 def test_argumenterror():
-    """Test raising ArgumentError."""
     with pytest.raises(ArgumentError):
-        const.init_const(CONST_FILE, directory=str(TST_DATA))
+        const.init_const(CONST_FILE, directory=str(TST_DATA / "json"))
 
 
 def test_init_const_custom():
-    """Test init_const function with a custom JSON file."""
-    cnsts = const.init_const(CONST_FILE, directory=TST_DATA)
+    cnsts = const.init_const(CONST_FILE, directory=TST_DATA / "json")
     assert str(cnsts).startswith("DummyConstants")
     assert isinstance(cnsts, const.const.ConstContainer)
     for key in cnsts.__dataclass_fields__.keys():
         attr = getattr(cnsts, key)
         assert isinstance(attr, iris.cube.Cube)
         assert attr.ndim == 0  # XXX could be relaxed
     key = "my_constant"
```

