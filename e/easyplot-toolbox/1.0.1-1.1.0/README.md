# Comparing `tmp/easyplot_toolbox-1.0.1.tar.gz` & `tmp/easyplot_toolbox-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyplot_toolbox-1.0.1.tar", max compression
+gzip compressed data, was "easyplot_toolbox-1.1.0.tar", max compression
```

## Comparing `easyplot_toolbox-1.0.1.tar` & `easyplot_toolbox-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       23 2024-04-24 19:08:21.749602 easyplot_toolbox-1.0.1/easyplot_toolbox/__init__.py
--rw-r--r--   0        0        0    35569 2024-04-24 19:08:21.749602 easyplot_toolbox-1.0.1/easyplot_toolbox/easyplot.py
--rw-r--r--   0        0        0      446 2024-04-24 19:23:39.502294 easyplot_toolbox-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      871 2024-04-24 19:08:21.761604 easyplot_toolbox-1.0.1/readme.md
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 easyplot_toolbox-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-04-28 20:37:03.067281 easyplot_toolbox-1.1.0/easyplot_toolbox/__init__.py
+-rw-r--r--   0        0        0    43826 2024-04-29 00:02:13.718962 easyplot_toolbox-1.1.0/easyplot_toolbox/easyplot.py
+-rw-r--r--   0        0        0     1115 2024-04-23 00:44:35.527423 easyplot_toolbox-1.1.0/license.md
+-rw-r--r--   0        0        0      531 2024-04-29 00:13:22.106376 easyplot_toolbox-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      997 2024-04-29 00:17:20.509228 easyplot_toolbox-1.1.0/readme2.md
+-rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 easyplot_toolbox-1.1.0/PKG-INFO
```

