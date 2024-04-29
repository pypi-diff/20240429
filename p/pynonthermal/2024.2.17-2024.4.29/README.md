# Comparing `tmp/pynonthermal-2024.2.17.tar.gz` & `tmp/pynonthermal-2024.4.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynonthermal-2024.2.17.tar", last modified: Sat Feb 17 13:18:21 2024, max compression
+gzip compressed data, was "pynonthermal-2024.4.29.tar", last modified: Mon Apr 29 16:16:54 2024, max compression
```

## Comparing `pynonthermal-2024.2.17.tar` & `pynonthermal-2024.4.29.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:18:21.146957 pynonthermal-2024.2.17/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:18:21.130957 pynonthermal-2024.2.17/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:18:21.134957 pynonthermal-2024.2.17/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/.github/workflows/deploypypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/.github/workflows/deploytestpypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/.github/workflows/linter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-02-17 13:18:21.146957 pynonthermal-2024.2.17/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:18:21.134957 pynonthermal-2024.2.17/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    36587 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/docs/oxygen_channels.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:18:21.134957 pynonthermal-2024.2.17/pynonthermal/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/axelrod.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2737 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/collion.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:18:21.138957 pynonthermal-2024.2.17/pynonthermal/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:18:21.138957 pynonthermal-2024.2.17/pynonthermal/data/artis_files/
--rw-r--r--   0 runner    (1001) docker     (127)   618097 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/artis_files/adata.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:18:21.146957 pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/fe1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/fe2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20298 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/fe3.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16147 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/fe4.txt
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/fe5.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/he1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/he2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/o1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/o2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/o3.txt
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/o4.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/artis_files/compositiondata.txt
--rw-r--r--   0 runner    (1001) docker     (127)  4228340 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/artis_files/transitiondata.txt.xz
--rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/collion-AR1985.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/collion-reference.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/data/collion.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/excitation.py
--rw-r--r--   0 runner    (1001) docker     (127)    36900 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/spencerfano.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:18:21.146957 pynonthermal-2024.2.17/pynonthermal/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:18:21.146957 pynonthermal-2024.2.17/pynonthermal/tests/output/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/tests/output/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pynonthermal/tests/test_sfsolve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-17 13:18:21.146957 pynonthermal-2024.2.17/pynonthermal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-02-17 13:18:21.000000 pynonthermal-2024.2.17/pynonthermal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-02-17 13:18:21.000000 pynonthermal-2024.2.17/pynonthermal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-17 13:18:21.000000 pynonthermal-2024.2.17/pynonthermal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-17 13:18:21.000000 pynonthermal-2024.2.17/pynonthermal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-17 13:18:21.000000 pynonthermal-2024.2.17/pynonthermal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)   106293 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-17 13:17:05.000000 pynonthermal-2024.2.17/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-17 13:18:21.146957 pynonthermal-2024.2.17/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:16:54.395501 pynonthermal-2024.4.29/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:16:54.379501 pynonthermal-2024.4.29/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:16:54.383501 pynonthermal-2024.4.29/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/.github/workflows/deploypypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/.github/workflows/deploytestpypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/.github/workflows/linter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-04-29 16:16:54.395501 pynonthermal-2024.4.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:16:54.383501 pynonthermal-2024.4.29/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    36587 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/docs/oxygen_channels.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:16:54.383501 pynonthermal-2024.4.29/pynonthermal/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9079 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/axelrod.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2737 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/collion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:16:54.387501 pynonthermal-2024.4.29/pynonthermal/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:16:54.387501 pynonthermal-2024.4.29/pynonthermal/data/artis_files/
+-rw-r--r--   0 runner    (1001) docker     (127)   618097 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/artis_files/adata.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:16:54.395501 pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/fe1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/fe2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20298 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/fe3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    16147 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/fe4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/fe5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/he1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/he2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/o1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/o2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/o3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/o4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/artis_files/compositiondata.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  4228340 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/artis_files/transitiondata.txt.xz
+-rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/collion-AR1985.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/collion-reference.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/data/collion.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/excitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36900 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/spencerfano.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:16:54.395501 pynonthermal-2024.4.29/pynonthermal/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:16:54.395501 pynonthermal-2024.4.29/pynonthermal/tests/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/tests/output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pynonthermal/tests/test_sfsolve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:16:54.395501 pynonthermal-2024.4.29/pynonthermal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-04-29 16:16:54.000000 pynonthermal-2024.4.29/pynonthermal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-29 16:16:54.000000 pynonthermal-2024.4.29/pynonthermal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:16:54.000000 pynonthermal-2024.4.29/pynonthermal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-29 16:16:54.000000 pynonthermal-2024.4.29/pynonthermal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 16:16:54.000000 pynonthermal-2024.4.29/pynonthermal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)   106252 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-29 16:15:54.000000 pynonthermal-2024.4.29/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:16:54.395501 pynonthermal-2024.4.29/setup.cfg
```

### Comparing `pynonthermal-2024.2.17/.github/workflows/deploypypi.yml` & `pynonthermal-2024.4.29/.github/workflows/deploypypi.yml`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/.github/workflows/deploytestpypi.yml` & `pynonthermal-2024.4.29/.github/workflows/deploytestpypi.yml`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/.github/workflows/linter.yml` & `pynonthermal-2024.4.29/.github/workflows/linter.yml`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/.github/workflows/pytest.yml` & `pynonthermal-2024.4.29/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/.gitignore` & `pynonthermal-2024.4.29/.gitignore`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/.pre-commit-config.yaml` & `pynonthermal-2024.4.29/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/LICENSE` & `pynonthermal-2024.4.29/LICENSE`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/PKG-INFO` & `pynonthermal-2024.4.29/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynonthermal
-Version: 2024.2.17
+Version: 2024.4.29
 Summary: A non-thermal electron deposition (Spencer-Fano equation) solver.
 Author-email: "Luke J. Shingles" <luke.shingles@gmail.com>
 License: MIT License
         
         Copyright (c) 2021-2024 Luke Shingles
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,33 +30,30 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argcomplete>=1.12.1
 Requires-Dist: artistools>=2021.4.23
-Requires-Dist: coveralls>=1.3.0
-Requires-Dist: flake8>=3.8.4
 Requires-Dist: matplotlib>=3.3.4
 Requires-Dist: numpy>=1.19.4
 Requires-Dist: pandas>=1.1
 Requires-Dist: pytest>=6.2.2
 Requires-Dist: pytest-cov>=2.10.1
 Requires-Dist: pytest-runner>=5.2
 Requires-Dist: PyYAML>=5.3.1
 Requires-Dist: scipy>=1.5.4
 Requires-Dist: typeguard>=4.1.5
 Requires-Dist: wheel>=0.36
 
 # pynonthermal
-[![Build and test](https://github.com/lukeshingles/pynonthermal/actions/workflows/pythonapp.yml/badge.svg)](https://github.com/lukeshingles/pynonthermal/actions/workflows/pythonapp.yml)
+[![Build and test](https://github.com/lukeshingles/pynonthermal/actions/workflows/pytest.yml/badge.svg)](https://github.com/lukeshingles/pynonthermal/actions/workflows/pytest.yml)
 [![codecov](https://codecov.io/gh/lukeshingles/pynonthermal/branch/main/graph/badge.svg?token=574XDCYFIi)](https://codecov.io/gh/lukeshingles/pynonthermal)
 
 pynonthermal is a non-thermal energy deposition (Spencer-Fano equation) solver.
 
 When high-energy leptons (electron and positrons) are injected into a plasma, they slow down by ionising and exciting atoms and ions, and Coulomb scattering with free (thermal) electrons. Keeping track of the rates of the processes is important for example, when modelling Type Ia supernovae at late times (>100 days). At late times, ionisation by high-energy non-thermal leptons (seeded by radioactive decay products) generally overtakes photoionisation, and the non-thermal contribution to ionisation is needed to obtain reasonable agreement with observed emission lines of singly- and doubly-ionised species.
 
 The numerical details of the solver are similar to the Spencer-Fano solver in the [ARTIS](https://github.com/artis-mcrt/artis) radiative transfer code ([Shingles et al. 2020](https://ui.adsabs.harvard.edu/abs/2020MNRAS.492.2029S/abstract)), which itself is an independent implementation of the [Kozma & Fransson (1992)](https://ui.adsabs.harvard.edu/abs/1992ApJ...390..602K/abstract) solution to the [Spencer & Fano (1945)](https://ui.adsabs.harvard.edu/abs/1954PhRv...93.1172S/abstract) equation. A similar solver is also applied in the [CMFGEN code](https://kookaburra.phyast.pitt.edu/hillier/web/CMFGEN.htm).
```

### Comparing `pynonthermal-2024.2.17/README.md` & `pynonthermal-2024.4.29/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # pynonthermal
-[![Build and test](https://github.com/lukeshingles/pynonthermal/actions/workflows/pythonapp.yml/badge.svg)](https://github.com/lukeshingles/pynonthermal/actions/workflows/pythonapp.yml)
+[![Build and test](https://github.com/lukeshingles/pynonthermal/actions/workflows/pytest.yml/badge.svg)](https://github.com/lukeshingles/pynonthermal/actions/workflows/pytest.yml)
 [![codecov](https://codecov.io/gh/lukeshingles/pynonthermal/branch/main/graph/badge.svg?token=574XDCYFIi)](https://codecov.io/gh/lukeshingles/pynonthermal)
 
 pynonthermal is a non-thermal energy deposition (Spencer-Fano equation) solver.
 
 When high-energy leptons (electron and positrons) are injected into a plasma, they slow down by ionising and exciting atoms and ions, and Coulomb scattering with free (thermal) electrons. Keeping track of the rates of the processes is important for example, when modelling Type Ia supernovae at late times (>100 days). At late times, ionisation by high-energy non-thermal leptons (seeded by radioactive decay products) generally overtakes photoionisation, and the non-thermal contribution to ionisation is needed to obtain reasonable agreement with observed emission lines of singly- and doubly-ionised species.
 
 The numerical details of the solver are similar to the Spencer-Fano solver in the [ARTIS](https://github.com/artis-mcrt/artis) radiative transfer code ([Shingles et al. 2020](https://ui.adsabs.harvard.edu/abs/2020MNRAS.492.2029S/abstract)), which itself is an independent implementation of the [Kozma & Fransson (1992)](https://ui.adsabs.harvard.edu/abs/1992ApJ...390..602K/abstract) solution to the [Spencer & Fano (1945)](https://ui.adsabs.harvard.edu/abs/1954PhRv...93.1172S/abstract) equation. A similar solver is also applied in the [CMFGEN code](https://kookaburra.phyast.pitt.edu/hillier/web/CMFGEN.htm).
```

### Comparing `pynonthermal-2024.2.17/docs/oxygen_channels.svg` & `pynonthermal-2024.4.29/docs/oxygen_channels.svg`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/axelrod.py` & `pynonthermal-2024.4.29/pynonthermal/axelrod.py`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/base.py` & `pynonthermal-2024.4.29/pynonthermal/base.py`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/collion.py` & `pynonthermal-2024.4.29/pynonthermal/collion.py`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/artis_files/adata.txt` & `pynonthermal-2024.4.29/pynonthermal/data/artis_files/adata.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/fe1.txt` & `pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/fe1.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/fe2.txt` & `pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/fe2.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/fe3.txt` & `pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/fe3.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/fe4.txt` & `pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/fe4.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/fe5.txt` & `pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/fe5.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/he1.txt` & `pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/he1.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/he2.txt` & `pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/he2.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/o1.txt` & `pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/o1.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/o2.txt` & `pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/o2.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/o3.txt` & `pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/o3.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/artis_files/atomic_data_logs/o4.txt` & `pynonthermal-2024.4.29/pynonthermal/data/artis_files/atomic_data_logs/o4.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/artis_files/transitiondata.txt.xz` & `pynonthermal-2024.4.29/pynonthermal/data/artis_files/transitiondata.txt.xz`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/collion-AR1985.txt` & `pynonthermal-2024.4.29/pynonthermal/data/collion-AR1985.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/collion-reference.txt` & `pynonthermal-2024.4.29/pynonthermal/data/collion-reference.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/data/collion.txt` & `pynonthermal-2024.4.29/pynonthermal/data/collion.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/excitation.py` & `pynonthermal-2024.4.29/pynonthermal/excitation.py`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/spencerfano.py` & `pynonthermal-2024.4.29/pynonthermal/spencerfano.py`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal/tests/test_sfsolve.py` & `pynonthermal-2024.4.29/pynonthermal/tests/test_sfsolve.py`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pynonthermal.egg-info/PKG-INFO` & `pynonthermal-2024.4.29/pynonthermal.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynonthermal
-Version: 2024.2.17
+Version: 2024.4.29
 Summary: A non-thermal electron deposition (Spencer-Fano equation) solver.
 Author-email: "Luke J. Shingles" <luke.shingles@gmail.com>
 License: MIT License
         
         Copyright (c) 2021-2024 Luke Shingles
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,33 +30,30 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argcomplete>=1.12.1
 Requires-Dist: artistools>=2021.4.23
-Requires-Dist: coveralls>=1.3.0
-Requires-Dist: flake8>=3.8.4
 Requires-Dist: matplotlib>=3.3.4
 Requires-Dist: numpy>=1.19.4
 Requires-Dist: pandas>=1.1
 Requires-Dist: pytest>=6.2.2
 Requires-Dist: pytest-cov>=2.10.1
 Requires-Dist: pytest-runner>=5.2
 Requires-Dist: PyYAML>=5.3.1
 Requires-Dist: scipy>=1.5.4
 Requires-Dist: typeguard>=4.1.5
 Requires-Dist: wheel>=0.36
 
 # pynonthermal
-[![Build and test](https://github.com/lukeshingles/pynonthermal/actions/workflows/pythonapp.yml/badge.svg)](https://github.com/lukeshingles/pynonthermal/actions/workflows/pythonapp.yml)
+[![Build and test](https://github.com/lukeshingles/pynonthermal/actions/workflows/pytest.yml/badge.svg)](https://github.com/lukeshingles/pynonthermal/actions/workflows/pytest.yml)
 [![codecov](https://codecov.io/gh/lukeshingles/pynonthermal/branch/main/graph/badge.svg?token=574XDCYFIi)](https://codecov.io/gh/lukeshingles/pynonthermal)
 
 pynonthermal is a non-thermal energy deposition (Spencer-Fano equation) solver.
 
 When high-energy leptons (electron and positrons) are injected into a plasma, they slow down by ionising and exciting atoms and ions, and Coulomb scattering with free (thermal) electrons. Keeping track of the rates of the processes is important for example, when modelling Type Ia supernovae at late times (>100 days). At late times, ionisation by high-energy non-thermal leptons (seeded by radioactive decay products) generally overtakes photoionisation, and the non-thermal contribution to ionisation is needed to obtain reasonable agreement with observed emission lines of singly- and doubly-ionised species.
 
 The numerical details of the solver are similar to the Spencer-Fano solver in the [ARTIS](https://github.com/artis-mcrt/artis) radiative transfer code ([Shingles et al. 2020](https://ui.adsabs.harvard.edu/abs/2020MNRAS.492.2029S/abstract)), which itself is an independent implementation of the [Kozma & Fransson (1992)](https://ui.adsabs.harvard.edu/abs/1992ApJ...390..602K/abstract) solution to the [Spencer & Fano (1945)](https://ui.adsabs.harvard.edu/abs/1954PhRv...93.1172S/abstract) equation. A similar solver is also applied in the [CMFGEN code](https://kookaburra.phyast.pitt.edu/hillier/web/CMFGEN.htm).
```

### Comparing `pynonthermal-2024.2.17/pynonthermal.egg-info/SOURCES.txt` & `pynonthermal-2024.4.29/pynonthermal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynonthermal-2024.2.17/pyproject.toml` & `pynonthermal-2024.4.29/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -13,17 +13,18 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Intended Audience :: Science/Research",
 ]
-dynamic = ["version", "dependencies", "entry-points", "readme", "scripts"]
+dynamic = ["version", "dependencies"]
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
+readme = {file = "README.md", content-type='text/markdown'}
 
 [project.urls]
 Repository = "https://www.github.com/lukeshingles/pynonthermal/"
 
 [tool.mypy]
 check_untyped_defs = false
 disallow_any_explicit = false
@@ -137,19 +138,14 @@
 [tool.ruff.lint.flake8-import-conventions.extend-aliases]
 "artistools" = "at"
 "matplotlib" = "mpl"
 "matplotlib.pyplot" = "plt"
 "matplotlib.typing" = "mplt"
 "numpy.typing" = "npt"
 "typing" = "t"
-"polars" = "pl"
-"polars.selectors" = "cs"
-
-[tool.ruff.lint.flake8-tidy-imports]
-ban-relative-imports = "all"
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.lint.isort]
 force-single-line = true
 order-by-type = false
@@ -159,19 +155,17 @@
 include-package-data = true
 license-files = ["LICENSE"]
 
 #[tool.setuptools.packages.find]
 #where = ["."]
 
 [tool.setuptools.dynamic]
-readme = {file = ["README.md"]}
 dependencies = {file = ["requirements.txt"]}
 
 [tool.setuptools_scm]
-write_to = "_version.py"
+version_file = "_version.py"
 local_scheme = "no-local-version"
 
 [tool.vulture]
 exclude = [".*", "build/", ".eggs/"]
-#ignore_names = ["visit_*", "do_*"]
 paths = ["pynonthermal"]
 sort_by_size = true
```

### Comparing `pynonthermal-2024.2.17/quickstart.ipynb` & `pynonthermal-2024.4.29/quickstart.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9870039682539682%*

 * *Differences: {"'cells'": "{0: {'execution_count': None, 'source': {insert: [(1, 'import "*

 * *            "matplotlib_inline.backend_inline\\n'), (2, "*

 * *            '"matplotlib_inline.backend_inline.set_matplotlib_formats(\'svg\')")], delete: [2, '*

 * *            "1]}}, 1: {'metadata': {replace: OrderedDict()}}, 2: {'metadata': {replace: "*

 * *            "OrderedDict()}}, 3: {'metadata': {replace: OrderedDict()}}}",*

 * * "'metadata'": "{'kernelspec': {'display_name': 'Python 3 (ipykernel)'}, 'language_info': "*

 * *               "{'versi […]*

```diff
@@ -1,30 +1,28 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": 23,
+            "execution_count": null,
             "id": "fad5cc44",
             "metadata": {
                 "scrolled": true
             },
             "outputs": [],
             "source": [
                 "import pynonthermal\n",
-                "from IPython.display import set_matplotlib_formats\n",
-                "set_matplotlib_formats('svg')"
+                "import matplotlib_inline.backend_inline\n",
+                "matplotlib_inline.backend_inline.set_matplotlib_formats('svg')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 22,
             "id": "8362d323",
-            "metadata": {
-                "scrolled": false
-            },
+            "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "\n",
                         "Setting up Spencer-Fano equation with 2000 energy points from 1.0 to 3000.0 eV...\n",
@@ -86,17 +84,15 @@
                 "sf.analyse_ntspectrum()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 16,
             "id": "f1a1c569",
-            "metadata": {
-                "scrolled": false
-            },
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/svg+xml": [
                             "<?xml version=\"1.0\" encoding=\"utf-8\" standalone=\"no\"?>\n",
                             "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
                             "  \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
@@ -1259,17 +1255,15 @@
                 "sf.plot_yspectrum()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 14,
             "id": "30d58600",
-            "metadata": {
-                "scrolled": false
-            },
+            "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "image/svg+xml": [
                             "<?xml version=\"1.0\" encoding=\"utf-8\" standalone=\"no\"?>\n",
                             "<!DOCTYPE svg PUBLIC \"-//W3C//DTD SVG 1.1//EN\"\n",
                             "  \"http://www.w3.org/Graphics/SVG/1.1/DTD/svg11.dtd\">\n",
@@ -2857,27 +2851,27 @@
             },
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
-            "display_name": "Python 3",
+            "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
         },
         "language_info": {
             "codemirror_mode": {
                 "name": "ipython",
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.4"
+            "version": "3.12.2"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

