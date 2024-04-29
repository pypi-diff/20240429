# Comparing `tmp/fairly-0.4.1.tar.gz` & `tmp/fairly-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairly-0.4.1.tar", last modified: Tue Aug 29 20:53:29 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `fairly-0.4.1.tar` & `fairly-1.0.0.tar`

### file list

```diff
@@ -1,52 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:53:29.135585 fairly-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (999)     1073 2023-08-29 20:53:18.000000 fairly-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)       35 2023-08-29 20:53:18.000000 fairly-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     7503 2023-08-29 20:53:29.135585 fairly-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     5386 2023-08-29 20:53:18.000000 fairly-0.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (999)     1191 2023-08-29 20:53:18.000000 fairly-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)      138 2023-08-29 20:53:29.135585 fairly-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:53:29.131585 fairly-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:53:29.131585 fairly-0.4.1/src/cli/
--rw-r--r--   0 runner    (1001) docker     (999)     1779 2023-08-29 20:53:18.000000 fairly-0.4.1/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1901 2023-08-29 20:53:18.000000 fairly-0.4.1/src/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (999)     4279 2023-08-29 20:53:18.000000 fairly-0.4.1/src/cli/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:53:29.131585 fairly-0.4.1/src/fairly/
--rw-r--r--   0 runner    (1001) docker     (999)    12891 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:53:29.135585 fairly-0.4.1/src/fairly/client/
--rw-r--r--   0 runner    (1001) docker     (999)    20868 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     6499 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/client/dataverse.py
--rw-r--r--   0 runner    (1001) docker     (999)     2016 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/client/djehuty.py
--rw-r--r--   0 runner    (1001) docker     (999)    31371 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/client/figshare.py
--rw-r--r--   0 runner    (1001) docker     (999)    33394 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/client/zenodo.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:53:29.135585 fairly-0.4.1/src/fairly/data/
--rw-r--r--   0 runner    (1001) docker     (999)      526 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/data/config.json
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:53:29.135585 fairly-0.4.1/src/fairly/data/languages/
--rw-r--r--   0 runner    (1001) docker     (999)    15501 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/data/languages/ISO-639-2_8859-1.tab
--rw-r--r--   0 runner    (1001) docker     (999)    15636 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/data/languages/ISO-639-2_UTF-8.tab
--rw-r--r--   0 runner    (1001) docker     (999)   201810 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/data/languages/ISO-639-3_8859-1.tab
--rw-r--r--   0 runner    (1001) docker     (999)   202920 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/data/languages/ISO-639-3_UTF-8.tab
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:53:29.135585 fairly-0.4.1/src/fairly/data/templates/
--rw-r--r--   0 runner    (1001) docker     (999)     1964 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/data/templates/default.yaml
--rw-r--r--   0 runner    (1001) docker     (999)     3009 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/data/templates/figshare.yaml
--rw-r--r--   0 runner    (1001) docker     (999)    12492 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/data/templates/zenodo.yaml
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:53:29.135585 fairly-0.4.1/src/fairly/dataset/
--rw-r--r--   0 runner    (1001) docker     (999)     6449 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    20870 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/dataset/local.py
--rw-r--r--   0 runner    (1001) docker     (999)     6832 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/dataset/remote.py
--rw-r--r--   0 runner    (1001) docker     (999)     1835 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/diff.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:53:29.135585 fairly-0.4.1/src/fairly/file/
--rw-r--r--   0 runner    (1001) docker     (999)     1485 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     7154 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/file/local.py
--rw-r--r--   0 runner    (1001) docker     (999)     1756 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/file/remote.py
--rw-r--r--   0 runner    (1001) docker     (999)     6292 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/metadata.py
--rw-r--r--   0 runner    (1001) docker     (999)    10524 2023-08-29 20:53:18.000000 fairly-0.4.1/src/fairly/person.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:53:29.131585 fairly-0.4.1/src/fairly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     7503 2023-08-29 20:53:29.000000 fairly-0.4.1/src/fairly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1089 2023-08-29 20:53:29.000000 fairly-0.4.1/src/fairly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-29 20:53:29.000000 fairly-0.4.1/src/fairly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       35 2023-08-29 20:53:29.000000 fairly-0.4.1/src/fairly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)      128 2023-08-29 20:53:29.000000 fairly-0.4.1/src/fairly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       11 2023-08-29 20:53:29.000000 fairly-0.4.1/src/fairly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 20:53:29.135585 fairly-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (999)     1930 2023-08-29 20:53:18.000000 fairly-0.4.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (999)     3740 2023-08-29 20:53:18.000000 fairly-0.4.1/tests/test_fairly.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 fairly-1.0.0/CITATION.cff
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 fairly-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 fairly-1.0.0/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 fairly-1.0.0/.github/workflows/test_workflow.yaml
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/.readthedocs.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/Makefile
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/conf.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/index.rst
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/installation.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/make.bat
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/modules.rst
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/osf2023.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/requirements.txt
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/_static/css/custom.css
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/api/fairly.client.rst
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/api/fairly.dataset.rst
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/api/fairly.file.rst
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/api/fairly.rst
+-rw-r--r--   0        0        0    79435 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/add-filles.png
+-rw-r--r--   0        0        0    68050 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/clone1.png
+-rw-r--r--   0        0        0    87734 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/clone2.png
+-rw-r--r--   0        0        0    65408 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/contex-menu.png
+-rw-r--r--   0        0        0    88937 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/create-dataset1.png
+-rw-r--r--   0        0        0    83099 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/create-dataset2.png
+-rw-r--r--   0        0        0    52616 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/create-directory.png
+-rw-r--r--   0        0        0    23376 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/labs-home.png
+-rw-r--r--   0        0        0    29374 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/labs-start.png
+-rw-r--r--   0        0        0    71432 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/my-dataset.png
+-rw-r--r--   0        0        0   102838 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/open-metadata.png
+-rw-r--r--   0        0        0    82431 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/osf-banner2023.png
+-rw-r--r--   0        0        0    95783 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/push-confirm.png
+-rw-r--r--   0        0        0    97453 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/push-menu.png
+-rw-r--r--   0        0        0   100270 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/start-jupyterlab.png
+-rw-r--r--   0        0        0    49967 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/zenodo-cli-upload.png
+-rw-r--r--   0        0        0    72320 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/zenodo-token.png
+-rw-r--r--   0        0        0    84240 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/img/zenodo-upload.png
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/package/account-datasets.ipynb
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/package/account-token.rst
+-rw-r--r--   0        0        0     6747 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/package/archiving-datasets.ipynb
+-rw-r--r--   0        0        0    10121 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/package/demo-4tu.ipynb
+-rw-r--r--   0        0        0     7828 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/package/demo-zenodo.ipynb
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/package/installation.rst
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/tutorials/cli.rst
+-rw-r--r--   0        0        0    13199 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/tutorials/jupyterlab.rst
+-rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/tutorials/python-api.ipynb
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 fairly-1.0.0/docs/tutorials/workshop.rst
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 fairly-1.0.0/src/cli/__init__.py
+-rw-r--r--   0        0        0     1859 2020-02-02 00:00:00.000000 fairly-1.0.0/src/cli/config.py
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 fairly-1.0.0/src/cli/dataset.py
+-rw-r--r--   0        0        0    16087 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/__init__.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/diff.py
+-rw-r--r--   0        0        0     7539 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/metadata.py
+-rw-r--r--   0        0        0    10600 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/person.py
+-rw-r--r--   0        0        0    21051 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/client/__init__.py
+-rw-r--r--   0        0        0    11876 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/client/dataverse.py
+-rw-r--r--   0        0        0    30709 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/client/djehuty.py
+-rw-r--r--   0        0        0    32367 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/client/figshare.py
+-rw-r--r--   0        0        0    21956 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/client/invenio.py
+-rw-r--r--   0        0        0    33823 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/client/zenodo.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/data/config.json
+-rw-r--r--   0        0        0    15501 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/data/languages/ISO-639-2_8859-1.tab
+-rw-r--r--   0        0        0    15636 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/data/languages/ISO-639-2_UTF-8.tab
+-rw-r--r--   0        0        0   201810 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/data/languages/ISO-639-3_8859-1.tab
+-rw-r--r--   0        0        0   202920 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/data/languages/ISO-639-3_UTF-8.tab
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/data/templates/default.yaml
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/data/templates/figshare.yaml
+-rw-r--r--   0        0        0    12492 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/data/templates/zenodo.yaml
+-rw-r--r--   0        0        0     7573 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/dataset/__init__.py
+-rw-r--r--   0        0        0    21986 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/dataset/local.py
+-rw-r--r--   0        0        0     8010 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/dataset/remote.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/file/__init__.py
+-rw-r--r--   0        0        0     8062 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/file/local.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 fairly-1.0.0/src/fairly/file/remote.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fairly-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 fairly-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 fairly-1.0.0/tests/test_cli.py
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 fairly-1.0.0/tests/test_fairly.py
+-rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 fairly-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fairly-1.0.0/LICENSE
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 fairly-1.0.0/README.rst
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 fairly-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 fairly-1.0.0/PKG-INFO
```

### Comparing `fairly-0.4.1/LICENSE` & `fairly-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fairly-0.4.1/PKG-INFO` & `fairly-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fairly
-Version: 0.4.1
+Version: 1.0.0
 Summary: A package to create, publish, and download research datasets
+Project-URL: Homepage, https://github.com/ITC-CRIB/fairly
+Project-URL: Bug Tracker, https://github.com/ITC-CRIB/fairly/issues
+Project-URL: Documentation, https://fairly.readthedocs.io
+Project-URL: Funding, https://nwo.nl/en/researchprogrammes/open-science/open-science-fund
 Author-email: Serkan Girgin <s.girgin@utwente.nl>, Manuel Garcia Alvarez <m.g.garciaalvarez@tudelft.nl>, Jose Urra Llanusa <j.c.urrallanusa@tudelft.nl>
 License: MIT License
         
         Copyright (c) 2022 JupyterFAIR Team
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -20,27 +24,33 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/ITC-CRIB/fairly
-Project-URL: Bug Tracker, https://github.com/ITC-CRIB/fairly/issues
-Project-URL: Documentation, https://fairly.readthedocs.io/en/latest/
-Project-URL: Funding, https://nwo.nl/en/researchprogrammes/open-science/open-science-fund
-Keywords: fairly,open science,research data,data management
-Classifier: Programming Language :: Python :: 3
+License-File: LICENSE
+Keywords: data management,fairly,open science,research data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
+Requires-Dist: python-dateutil
+Requires-Dist: requests
+Requires-Dist: requests-toolbelt>=1.0.0
+Requires-Dist: rich
+Requires-Dist: ruamel-yaml>=0.17.26
+Requires-Dist: typer>=0.9.0
 Provides-Extra: dev
-License-File: LICENSE
+Requires-Dist: build; extra == 'dev'
+Requires-Dist: hatch; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: pytest-cov; extra == 'dev'
+Requires-Dist: python-dotenv; extra == 'dev'
+Description-Content-Type: text/x-rst
 
 .. list-table::
    :widths: 25 25
    :header-rows: 1
 
    * - `fair-software.nl <https://fair-software.nl>`_ recommendations
      - Badges
@@ -195,15 +205,15 @@
 
    # Store dataset to a local directory (i.e. clone dataset)
    local_dataset = dataset.store('/path/dataset')
 
 Currently, the package supports the following research data management
 platforms:
 
--  `Zenodo <https://zenodo.org/>`__
+-  `Invenio <https://inveniosoftware.org/>`__
 -  `Figshare <https://figshare.com/>`__
 -  `Djehuty <https://github.com/4TUResearchData/djehuty/>`__
    (experimental)
 
 All research data repositories based on the listed platforms are
 supported.
```

### Comparing `fairly-0.4.1/README.rst` & `fairly-1.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
 
    # Store dataset to a local directory (i.e. clone dataset)
    local_dataset = dataset.store('/path/dataset')
 
 Currently, the package supports the following research data management
 platforms:
 
--  `Zenodo <https://zenodo.org/>`__
+-  `Invenio <https://inveniosoftware.org/>`__
 -  `Figshare <https://figshare.com/>`__
 -  `Djehuty <https://github.com/4TUResearchData/djehuty/>`__
    (experimental)
 
 All research data repositories based on the listed platforms are
 supported.
```

### Comparing `fairly-0.4.1/pyproject.toml` & `fairly-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
 [project]
 name = "fairly"
-version = "0.4.1"
+version = "1.0.0"
 authors = [
   { name="Serkan Girgin", email="s.girgin@utwente.nl" },
   { name="Manuel Garcia Alvarez", email="m.g.garciaalvarez@tudelft.nl" },
   { name="Jose Urra Llanusa", email="j.c.urrallanusa@tudelft.nl" }, ]
 description = "A package to create, publish, and download research datasets"
 readme = "README.rst"
 license = { file="LICENSE" }
@@ -23,18 +27,20 @@
     ]
 keywords = ["fairly", "open science", "research data", "data management"]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-cov",
-    "python-dotenv"
+    "python-dotenv",
+    "build",
+    "hatch"
     ]
 
 [project.urls]
 "Homepage" = "https://github.com/ITC-CRIB/fairly"
 "Bug Tracker" = "https://github.com/ITC-CRIB/fairly/issues"
-"Documentation" = "https://fairly.readthedocs.io/en/latest/"
+"Documentation" = "https://fairly.readthedocs.io"
 "Funding" = "https://nwo.nl/en/researchprogrammes/open-science/open-science-fund"
 
 [project.scripts]
 fairly = "cli:app"
```

### Comparing `fairly-0.4.1/src/cli/__init__.py` & `fairly-1.0.0/src/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 @app.command()
 def list_repos():
     '''List all repositories supported by fairly'''
     repositories = fairly.get_repositories()
 
     print("List of repositories to use with fairly:")
-    
+
     for key in repositories:
         print("- " + key)
 
 @app.command()
 @app.command()
 def list_user_datasets(
     repository: str = typer.Argument("", help="Repository name"),
@@ -49,14 +49,14 @@
                     if i == 'title': item[i] = metadata[i]
                     if i == 'doi': item[i] = metadata[i]
 
                 # pretty print the list of datasets with yaml format
                 yaml.dump(item, sys.stdout)
                 print("------------------")
 
-    except Exception as e: 
+    except Exception as e:
         print(e)
         print("Please specify a repository name that is valid")
     return None
 
 if __name__ == "__main__":
     app()
```

### Comparing `fairly-0.4.1/src/cli/config.py` & `fairly-1.0.0/src/cli/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,25 +16,25 @@
 
 
 # @app.command()
 def add(
     id: str = typer.Argument("", help="Repository ID"),
 ):
     '''Add a repository to the config file,
-    
+
     fairly repository add --id <id> --name <name> --api-url <url> --token <token>
 
     Notice that this should only be allowed once there is a corresponing module
     for the repository.
     '''
     raise NotImplementedError
 
 @app.command()
 def show(
-    
+
 ):
     '''Show config details'''
     yaml = YAML()
     # expand user path
     print(f"You can edit the config file located at: {CONFIG_FILE}")
 
     print("FAIRLY CONFIG")
@@ -50,25 +50,25 @@
     token: str = typer.Argument("", help="Repository token")
 ):
     ''' Update a repository token os.path.expanduser('~/.fairly/config.json)'''
     config = {}
     try:
         with open(CONFIG_FILE, 'r', encoding='utf-8') as f:
             config = json.loads(f.read())
-            
+
             # check if token is already set with the same value
             if config[id]["token"] == token:
                 print(f"Token for repository {id} is already set to {token}")
                 return
-            
+
             else: config[id]["token"] = token
-        
+
         with open(CONFIG_FILE, 'w', encoding='utf-8') as f:
             f.write(json.dumps(config, indent=4))
-  
+
     except FileNotFoundError:
         print(f"Config file not found at {CONFIG_FILE}")
         return
 
 
 # @app.command()
 def remove():
```

### Comparing `fairly-0.4.1/src/cli/dataset.py` & `fairly-1.0.0/src/cli/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,22 +34,25 @@
     extract: bool = typer.Option(False, help="Extract archive files"),
 ) -> None:
     '''
     Clones a dataset by using its URL address, DOI or unique ID.
 
     Examples: \n
         >>> fairly dataset clone <url|doi|uid> \n \n
-        >>> fairly dataset clone https://zenodo.org/record/7759648 \n
+        >>> fairly dataset clone https://zenodo.org/records/7759648 \n
         >>> fairly dataset clone 10.5281/zenodo.7759648 \n
         >>> fairly dataset clone <repository> <id> \n
         >>> fairly dataset clone --repo zenodo 7759648 \n
     '''
 
     if repo:
-        client = fairly.client(repo, token=token)
+        if token:
+            client = fairly.client(repo, token=token)
+        else:
+            client = fairly.client(repo)
         dataset = client.get_dataset(id)
 
     else:
         dataset = fairly.dataset(id)
 
     if not path:
         path = dataset.doi if dataset.doi else "dataset"
@@ -93,40 +96,43 @@
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
         transient = True,
     ) as progress:
         progress.add_task(description=f"Uploading dataset {path}", total=None)
         remote_dataset = dataset.upload(client, notify=notify)
 
-    print(f"Dataset {path} is successfully uploaded at {remote_dataset.url}")
+    print(f"Dataset {path} is successfully uploaded at {remote_dataset.url or remote_dataset.plain_id}")
 
 
 @app.command()
 def delete(
     id: str = typer.Argument(help="Dataset identifier (URL address, DOI, or unique ID)"),
     repo: str = typer.Option("", help="Repository option argument"),
     token: str = typer.Option("", help="Access token option argument"),
 ):
     '''
     Deletes a dataset by using its URL address, DOI or unique ID.
     '''
     if repo:
-        client = fairly.client(repo, token=token)
+        if token:
+            client = fairly.client(repo, token=token)
+        else:
+            client = fairly.client(repo)
         dataset = client.get_dataset(id)
 
     else:
         dataset = fairly.dataset(id)
         client = dataset.client
 
     with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
         transient = True,
     ) as progress:
-        progress.add_task(description="Deleting dataset {id}", total=None)
+        progress.add_task(description=f"Deleting dataset {id}", total=None)
         client.delete_dataset(dataset.id)
 
     print(f"Dataset {id} is successfully deleted.")
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `fairly-0.4.1/src/fairly/__init__.py` & `fairly-1.0.0/src/fairly/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 """
 fairly
 """
 from __future__ import annotations
-from typing import Dict, List
+from typing import Dict, List, Callable
 
 import sys
 import os
 import json
 import pkgutil
 import importlib
+import requests
+import re
 from functools import lru_cache
+import logging
+from urllib.parse import urlparse
 
 from .client import Client
 from .dataset import Dataset
 from .dataset.local import LocalDataset
 from .file import File
 
 
+MAX_WORKERS = 4
+
+_max_workers = None
+
+
 def is_testing() -> bool:
     """Returns unit testing state.
 
     Returns:
         True if performing unit tests, False otherwise
     """
     return getattr(sys.modules[__name__], "TESTING", False)
@@ -92,33 +101,34 @@
 
 # REMARK: @cache decorator can be used for Python 3.9+
 @lru_cache(maxsize=None)
 def get_clients() -> Dict:
     """Returns available clients.
 
     Returns:
-        Dictionary of the available clients. Keys are client identifiers (str), values are client classes (Client).
+        Dictionary of the available clients.
+        Keys are client identifiers (str), values are client classes (Client).
 
     Raises:
-        AttributeError: If a client module is not valid.
+        AttributeError("Invalid client module", id): If a client module is invalid.
 
     Examples:
         >>> fairly.get_clients()
         >>> {'figshare': <class 'fairly.client.figshare.FigshareClient'>, ...}
     """
     clients = {}
 
     # For each client module
     for _, id, _ in pkgutil.iter_modules([os.path.join(__path__[0], "client")]):
         # Load module
         client = importlib.import_module(f"fairly.client.{id}")
         # Get client class name
         classname = client.CLASS_NAME
         if not classname:
-            raise AttributeError(f"Invalid client module: {id}")
+            raise AttributeError("Invalid client module", id)
         # Set client class
         clients[id] = getattr(client, classname)
 
     # Return
     return clients
 
 
@@ -216,14 +226,18 @@
         if ext == ".yaml":
             # TODO: Check if a valid metadata template
             templates.append(name)
 
     return templates
 
 
+def _match_domain(url: str, domain_url: str) -> bool:
+    hostname = urlparse(url).hostname
+    return False if not hostname else hostname.endswith(urlparse(domain_url).hostname)
+
 def get_repository(uid: str) -> Dict:
     """Returns repository dictionary of the specified repository.
 
     Args:
         uid (str): Repository id or URL address.
 
     Returns:
@@ -237,17 +251,18 @@
         >>>
     """
     repositories = get_repositories()
 
     if uid in repositories:
         return repositories[uid].copy()
 
-    for _, repository in repositories.items():
-        if uid == repository["url"]:
-            return repository.copy()
+    if re.fullmatch(Client.REGEXP_URL, uid):
+        for _, repository in repositories.items():
+            if _match_domain(uid, repository["url"]):
+                return repository.copy()
 
     return None
 
 
 def client(id: str, **kwargs) -> Client:
     """Creates client object from a client or repository identifier.
 
@@ -259,15 +274,15 @@
         id (str): Client or repository identifier.
         **kwargs: Other client arguments.
 
     Returns:
         Client object.
 
     Raises:
-        ValueError: If invalid client id.
+        ValueError("Invalid client id"): If invalid client id.
 
     Examples:
         >>> # Create a 4TU.ResearchData client (id = "4tu")
         >>> client = fairly.client("4tu")
 
         >>> # Create a Figshare client with a custom URL address
         >>> client = fairly.client("figshare", url="https://data.4tu.nl/")
@@ -276,64 +291,76 @@
 
     repository = get_repository(id)
     if repository:
         kwargs["repository_id"] = repository["id"]
         id = repository["client_id"]
 
     if id not in clients:
-        raise ValueError(f"Invalid client id: {id}")
+        raise ValueError("Invalid client id")
 
     return clients[id](**kwargs)
 
 
 def dataset(id: str) -> Dataset:
     """Creates dataset object from a dataset identifier.
 
     The following types of dataset identifiers are supported:
-        - DOI : Digital object identifier of the remote dataset.
-        - URL : URL address of the remote dataset.
-        - Path : Path of the local dataset.
+        - DOI : Digital object identifier of a remote dataset.
+        - URL : URL address of a remote dataset.
+        - Path : Path of a local dataset.
 
     Repository of the dataset is automatically detected by checking the URL
     addresses and the DOI prefixes of the recognized repositories.
 
     Args:
         id (str): Dataset identifier.
 
     Returns:
         Dataset object.
 
     Raises:
-        ValueError: If unknown dataset identifier.
+        ValueError("Unknown dataset identifier"): If unknown dataset identifier.
 
     Examples:
         >>> dataset = fairly.dataset("10.5281/zenodo.6026285")
-        >>> dataset = fairly.dataset("https://zenodo.org/record/6026285")
+        >>> dataset = fairly.dataset("https://zenodo.org/records/6026285")
     """
     if isinstance(id, str):
         key, val = Client.parse_id(id)
     else:
         key = None
 
     if key == "url":
+        logging.info("Checking recognized repositories for %s.", val)
         for repository_id, repository in get_repositories().items():
             url = repository.get("url")
-            if url and val.startswith(url):
+            if url and _match_domain(val, url):
+                logging.info("%s matched %s.", repository_id, val)
                 return client(repository_id).get_dataset(url=val)
 
+        logging.info("Checking clients for auto-detection.")
+        for cls in get_clients().values():
+            if not hasattr(cls, "get_client"):
+                continue
+            try:
+                result = cls.get_client(val)
+            except Exception as err:
+                logging.debug("Exception %s", err)
+                continue
+            logging.info("%s client is found at %s.", result.client_id, result.config.get("url"))
+            return result.get_dataset(url=val)
+
     elif key == "doi":
-        for repository_id, repository in get_repositories().items():
-            for prefix in repository.get("doi_prefixes", []):
-                if prefix and val.startswith(prefix):
-                    return client(repository_id).get_dataset(doi=val)
+        url = resolveDOI(val)
+        return dataset(url)
 
     else:
         return LocalDataset(id)
 
-    raise ValueError(f"Unknown dataset identifier: {id}")
+    raise ValueError("Unknown dataset identifier")
 
 
 def init_dataset(path: str, template: str = "default", create: bool = True) -> LocalDataset:
     """Initializes a local dataset.
 
     Args:
         path (str): Local path of the dataset.
@@ -420,10 +447,97 @@
 
     Returns:
         Local dataset object
     """
     return dataset(id).store(path, notify=notify, extract=extract)
 
 
+def resolveDOI(doi: str) -> str:
+    """Returns URL address to a DOI.
+
+    Args:
+        doi (str): Digital object identifier
+
+    Returns:
+        URL address of the DOI.
+
+    Raises:
+        ValueError("Invalid DOI"): If DOI is invalid.
+    """
+
+    match = re.fullmatch(r"(doi:|https?://doi\.org/)?(10\..+)", doi, flags=re.IGNORECASE)
+    if not match:
+        raise ValueError("Invalid DOI")
+
+    url = "https://doi.org/" + match[2]
+    try:
+        logging.info("Sending DOI resolve request to %s.", url)
+        response = requests.head(url, allow_redirects=True)
+        response.raise_for_status()
+    except:
+        raise ValueError("Invalid DOI")
+
+    url = response.headers.get("Location", response.url)
+    if not url:
+        raise ValueError("Invalid DOI")
+    logging.info("Resolved URL address is %s.", url)
+
+    return url
+
+
+def set_max_workers(num: int=None, force: bool=False) -> int:
+    """Sets number of maximum workers for file operations.
+
+    Maximum number of workers is limited to `MAX_WORKERS`, unless `force` 
+    flag is set.
+
+    Args:
+        num (int): Maximum number of workers for file operations.
+        force (bool): Set True to increase the number beyond `MAX_WORKERS` (default False).
+
+    Returns:
+        Maximum number of workers for file operations.
+
+    Raises:
+        ValueError("Invalid maximum number of workers"): If the number is more than the number of available cores.
+    """
+    global _max_workers
+
+    if not num and num is not None:
+        num = 1
+
+    if hasattr(os, "sched_getaffinity"):
+        max = len(os.sched_getaffinity(0))
+    else:
+        max = os.cpu_count()
+    logging.info("Number of available cores is %d.", max)
+
+    if num is None:
+        num = max
+
+    elif num > max:
+        raise ValueError("Invalid maximum number of workers")
+
+    if not force and num > MAX_WORKERS:
+        logging.info("Limiting %d maximum workers to %d.", num, MAX_WORKERS)
+        num = MAX_WORKERS
+
+    _max_workers = num
+
+    return _max_workers
+
+
+def max_workers() -> int:
+    """Returns maximum number of workers for file operations."""
+    global _max_workers
+
+    return _max_workers if _max_workers else set_max_workers()
+
+
+def debug(state: bool=True) -> None:
+    level = logging.DEBUG if state else logging.INFO
+    logging.basicConfig(level=level)
+
+
 if __name__ == "__main__":
     # TODO: CLI implementation
     raise NotImplementedError
```

### Comparing `fairly-0.4.1/src/fairly/client/__init__.py` & `fairly-1.0.0/src/fairly/client/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from __future__ import annotations
-from typing import Any, Dict, List, Tuple, Union
+from typing import Any, Dict, List, Tuple, Callable
 from abc import ABC, abstractmethod
 
 import fairly
 from ..dataset.remote import RemoteDataset
 from ..file.local import LocalFile
 from ..file.remote import RemoteFile
 from ..metadata import Metadata
@@ -11,36 +11,38 @@
 import os
 import os.path
 import re
 import json
 import requests
 import hashlib
 import http.client
+import uuid
+import logging
+import time
+
 
 class Client(ABC):
     """
-
     Attributes:
-        config (dict): Configuration options
+        config (Dict): Configuration options
         _session (Session): HTTP session object
-        _datasets (dict): Public dataset cache
+        _datasets (Dict): Public dataset cache
         _account_datasets (List): Account dataset cache
-        _licenses (List): Licenses cache
 
     Class Attributes:
         REGEXP_URL: Regular expression to validate URL address.
         REQUEST_FORMAT: Request data format
-        CHUCK_SIZE: Data transfer chuck size
+        CHUNK_SIZE: Chunk size in bytes to transfer data (default = 65536)
     """
 
-    REGEXP_URL = re.compile(r"^[(http(s)?):\/\/(www\.)?a-zA-Z0-9@:%._\+~#=]{2,256}\.[a-z]{2,6}\b([-a-zA-Z0-9@:%_\+.~#?&//=]*)$", re.IGNORECASE)
+    REGEXP_URL = re.compile(r"(http(s)?):\/\/(www\.)?[a-z\d@:%._\+~#=-]{2,256}\.[a-z]{2,6}\b([-a-z\d@:%_\+.~#?&//=]*)", re.IGNORECASE)
 
     REQUEST_FORMAT = "json"
 
-    CHUNK_SIZE = 2**16
+    CHUNK_SIZE = 2**18
 
 
     def __init__(self, repository_id: str=None, **kwargs):
         # Get client id
         self._client_id = self.__module__.split(".")[-1]
 
         config = {}
@@ -51,30 +53,29 @@
             repository = fairly.get_repository(repository_id)
 
             if repository:
                 if repository["client_id"] != self._client_id:
                     raise ValueError("Repository client id mismatch")
                 config = repository
 
-            elif re.match(Client.REGEXP_URL, repository_id):
+            elif re.fullmatch(Client.REGEXP_URL, repository_id):
                 kwargs["api_url"] = repository_id
 
         self._repository_id = repository_id
 
         # Append named arguments
         config.update(kwargs)
 
         # Set configuration
         self.config = type(self).get_config(**config)
 
         # Initialize attributes
         self._session = None
         self._datasets = {}
         self._account_datasets = None
-        self._licenses = None
 
 
     @property
     def client_id(self) -> str:
         """Client identifier"""
         return self._client_id
 
@@ -83,62 +84,51 @@
     def repository_id(self) -> str:
         """Repository identifier of the client"""
         return self._repository_id
 
 
     @classmethod
     def get_config_parameters(cls) -> Dict:
-        """Returns configuration parameters
-
-        Args:
-            None
+        """Returns configuration parameters.
 
         Returns:
             Dictionary of configuration parameters.
             Keys are the parameter names, values are the descriptions.
         """
         return {
             "name": "Repository name.",
             "url": "URL address of the repository.",
             "api_url": "API end-point URL address of the repository.",
-            "doi_prefixes": "DOI prefixes of the repository.",
         }
 
 
     @classmethod
     def get_config(cls, **kwargs) -> Dict:
         config = {}
         for key, val in kwargs.items():
             if key == "name":
                 config["name"] = val
             elif key == "url":
-                if not re.match(Client.REGEXP_URL, val):
+                if not re.fullmatch(Client.REGEXP_URL, val):
                     raise ValueError("Invalid URL address")
                 config["url"] = val
             elif key == "api_url":
-                if not re.match(Client.REGEXP_URL, val):
+                if not re.fullmatch(Client.REGEXP_URL, val):
                     raise ValueError("Invalid API URL address")
                 config["api_url"] = val
-            elif key == "doi_prefixes":
-                if not isinstance(val, list):
-                    raise ValueError("Invalid DOI prefixes")
-                config["doi_prefixes"] = val
             else:
                 pass
         return config
 
 
     def save_config(self, save_environment=False) -> None:
         """Saves client configuration.
 
         Args:
-            save_environment: Set True to save environment variables
-
-        Returns:
-            None
+            save_environment: Set True to save environment variables (default False)
         """
         id = self.repository_id if self.repository_id else self.client_id
 
         common = {}
         try:
             with open(os.path.join(__path__[0], "..", "data", "config.json"), "r") as file:
                 common = json.load(file).get(id, {})
@@ -174,26 +164,33 @@
 
         with open(path, "w") as file:
             json.dump(data, file, indent=2)
 
 
     @classmethod
     def parse_id(cls, id: str) -> Tuple(str, str):
-        """Parses the specified identifier
+        """Parses the specified identifier.
+
+        Args:
+            id : Identifier.
 
         Returns:
-          Tuple of identifier type and value
+          Tuple of identifier type and value.
         """
-        match = re.match(r"^(doi:|https?:\/\/doi.org\/)(.+)$", id)
+        match = re.fullmatch(r"(doi:|https?:\/\/doi.org\/)(.+)", id)
+
         if match:
             return "doi", match.group(2)
-        elif re.match(Metadata.REGEXP_DOI, id):
+
+        elif re.fullmatch(Metadata.REGEXP_DOI, id):
             return "doi", id
-        elif re.match(r"^https?:\/\/", id):
+
+        elif re.match(r"https?:\/\/", id):
             return "url", id
+
         else:
             return "id", id
 
 
     @abstractmethod
     def _get_dataset_id(self, **kwargs) -> Dict:
         raise NotImplementedError
@@ -208,47 +205,68 @@
 
         Returns:
             Standard dataset identifier
         """
         if id:
             if isinstance(id, dict):
                 return id
+
             elif isinstance(id, str):
                 key, val = self.parse_id(id)
                 kwargs[key] = val
+
             else:
                 kwargs["id"] = id
+
         return self._get_dataset_id(**kwargs)
 
 
+    def get_dataset_plain_id(self, id: Dict) -> str:
+        """Returns plain standard dataset identifier.
+
+        Args:
+            id (Dict): Standard dataset identifier.
+
+        Returns:
+            Plain standard dataset identifier.
+        """
+        parts = []
+
+        for key, val in id.items():
+            if bool(val) or isinstance(val, (bool, int, float)):
+                parts.append(val)
+
+        return "/".join(parts)
+
+
     @abstractmethod
     def _get_dataset_hash(self, id: Dict) -> str:
-        """Returns hash of the standard dataset identifier
+        """Returns hash of the standard dataset identifier.
 
         Args:
-            id (Dict): Standard dataset identifier
+            id (Dict): Standard dataset identifier.
 
         Returns:
-            Hash of the dataset identifier
+            Hash of the dataset identifier.
         """
         raise NotImplementedError
 
 
     @classmethod
-    def normalize(cls, name: str, val) -> Any:
+    def normalize_value(cls, name: str, val) -> Any:
         """Normalized metadata attribute value
 
         Args:
             name (str): Attribute name
             val: Attribute value
 
         Returns:
             Normalized attribute value
         """
-        return Metadata.normalize(name, val)
+        return Metadata.normalize_value(name, val)
 
 
     @abstractmethod
     def _create_dataset(self, metadata: Metadata) -> Dict:
         """Creates a dataset with the specified standard metadata
 
         Args:
@@ -293,23 +311,25 @@
 
         # Get dataset
         dataset = self.get_dataset(id)
 
         # Cache dataset
         hash = self._get_dataset_hash(id)
         self._datasets[hash] = dataset
+
+        # Append dataset to the account datasets
         if not self._account_datasets:
             self._account_datasets = []
         self._account_datasets.append(dataset)
 
         # Return dataset
         return dataset
 
 
-    def _create_session(self) -> Session:
+    def _create_session(self) -> requests.Session:
         return requests.Session()
 
 
     def _request(self, endpoint: str, method: str="GET", headers: dict=None, data=None, format: str=None, serialize: bool=True) -> Tuple(Any, requests.Response):
         """ Sends a HTTP request and returns the result
 
         Returns:
@@ -345,54 +365,33 @@
 
         _headers = headers.copy() if headers else {}
         if format == "json":
             _headers["Accept"] = "application/json"
             if "Content-Type" not in _headers:
                 _headers["Content-Type"] = "application/json"
 
+        logging.info("Sending %s request to %s.", method, url)
+        if _headers:
+            logging.debug("Headers %s", _headers)
         response = self._session.request(method, url, headers=_headers, data=data)
         response.raise_for_status()
 
         if response.content:
             if format == "json":
                 content = response.json()
             else:
                 content = response.content
+            logging.debug("Content %s", content)
         else:
             content = None
 
         return content, response
 
 
     @abstractmethod
-    def _get_licenses(self) -> Dict:
-        raise NotImplementedError
-
-
-    def get_licenses(self, refresh: bool=False) -> List[Dict]:
-        """Returns list of available licenses
-
-        Args:
-            refresh (bool): Set True to refresh licenses (default = False)
-
-        Returns:
-            List of client-specific license dictionaries
-        """
-        if self._licenses is None or refresh:
-            self._licenses = self._get_licenses()
-
-        return self._licenses
-
-
-    @property
-    def licenses(self) -> Dict:
-        return self.get_licenses()
-
-
-    @abstractmethod
     def _get_account_datasets(self) -> List[RemoteDataset]:
         raise NotImplementedError
 
 
     def get_account_datasets(self, refresh: bool=False) -> List[RemoteDataset]:
         if self._account_datasets is None or refresh:
             datasets = self._get_account_datasets()
@@ -413,19 +412,15 @@
 
         # Get standard id
         id = self.get_dataset_id(id, **kwargs)
         # Get dataset hash
         hash = self._get_dataset_hash(id)
         # Fetch dataset if required
         if hash not in self._datasets or refresh:
-            details = {}
-            for key in ["url", "doi"]:
-                if kwargs.get(key):
-                    details[key] = kwargs[key]
-            self._datasets[hash] = RemoteDataset(self, id, details)
+            self._datasets[hash] = RemoteDataset(self, id)
 
         # Return dataset
         return self._datasets[hash]
 
 
     @abstractmethod
     def _get_versions(self, id: Dict) -> OrderedDict:
@@ -492,27 +487,24 @@
         Returns:
             Standard metadata
         """
         # Get standard metadata attributes
         attrs = self._get_metadata(id)
 
         # Return metadata
-        return Metadata(normalize=self.normalize, **attrs)
+        return Metadata(normalize=self.normalize_value, **attrs)
 
 
     @abstractmethod
     def save_metadata(self, id: Dict, metadata: Metadata) -> None:
-        """Saves metadata of the specified dataset
+        """Saves metadata of the specified dataset.
 
         Args:
-            id (Dict): Standard dataset id
-            metadata (Metadata): Metadata to be saved
-
-        Returns:
-            None
+            id (Dict): Standard dataset id.
+            metadata (Metadata): Metadata to be saved.
         """
         raise NotImplementedError
 
 
     @abstractmethod
     def validate_metadata(self, metadata: Metadata) -> Dict:
         """Validates metadata
@@ -545,51 +537,74 @@
         Returns:
             Local file object.
 
         Raises:
             ValueError("No URL address"): If remote file has no URL address.
             IOError("Invalid MD5 checksum"): If MD5 checksum is invalid.
         """
+        logging.info("Downloading file %s.", file.path)
         if not file.url:
             raise ValueError("No URL address")
 
         if not path:
             path = os.getcwd()
 
-        if not name:
-            name = file.path
-            dirs = os.path.dirname(name)
-            if dirs:
-                os.makedirs(os.path.join(path, dirs), exist_ok=True)
+        fullpath = os.path.join(path, name or file.path)
+
+        while True:
+            temppath = os.path.join(path, "." + uuid.uuid4().hex)
+            if not os.path.isfile(temppath):
+                break
 
-        fullpath = os.path.join(path, name)
         current_size = 0
         md5 = hashlib.md5()
         if self._session is None:
             self._session = self._create_session()
+
         try:
             with self._session.get(file.url, stream=True) as response:
                 response.raise_for_status()
-                os.makedirs(os.path.dirname(fullpath), exist_ok=True)
-                with open(fullpath, "wb") as local_file:
+
+                # Create directories if required
+                # TODO: Store the list of directories for a potential clean-up
+                os.makedirs(os.path.dirname(temppath), exist_ok=True)
+
+                # Download file
+                start = time.time()
+                logging.info("Started at %s", time.strftime("%Y-%m-%d %H:%M:%S"))
+                with open(temppath, "wb") as local_file:
                     for chunk in response.iter_content(self.CHUNK_SIZE):
                         local_file.write(chunk)
                         md5.update(chunk)
                         current_size += len(chunk)
                         if notify:
                             notify(file, current_size)
+                logging.info("Done in %d s.", time.time() - start)
+
+                # Rename file
+                os.makedirs(os.path.dirname(fullpath), exist_ok=True)
+                os.rename(temppath, fullpath)
+
+            # Validate checksum
             md5 = md5.hexdigest()
             if file.md5 and file.md5 != md5:
+                logging.debug("Invalid checksum %s vs %s.", file.md5, md5)
                 raise IOError("Invalid MD5 checksum")
+
         except:
             # Clean up if incomplete download
             # TODO: Remove created directories
+            if os.path.isfile(temppath):
+                os.remove(temppath)
+
             if os.path.isfile(fullpath):
                 os.remove(fullpath)
+
             raise
+
         return LocalFile(fullpath, basepath=path, md5=md5)
 
 
     @abstractmethod
     def _upload_file(self, id: Dict, file: LocalFile, notify: Callable=None) -> RemoteFile:
         raise NotImplementedError
 
@@ -627,38 +642,28 @@
 
         # TODO: Do not refresh the complete file list
         dataset.get_files(refresh=True)
 
 
     @abstractmethod
     def _delete_dataset(self, id: Dict) -> None:
-        """Deletes dataset specified by the standard identifier from the repository
+        """Deletes dataset from the repository.
 
         Args:
-            id (Dict): Standard dataset identifier
-
-        Returns:
-            None
-
-        Raises:
-            ValueError("Operation not permitted")
-            ValueError("Invalid dataset id")
+            id (Dict): Standard dataset identifier.
         """
         raise NotImplementedError
 
 
     def delete_dataset(self, id, **kwargs) -> None:
-        """Deletes specified dataset from the repository
+        """Deletes dataset from the repository.
 
         Args:
-            id: Dataset identifier
-            **kwargs: Other identifier arguments
-
-        Returns:
-            None
+            id: Dataset identifier.
+            **kwargs: Other identifier arguments.
         """
         # Get standard id
         id = self.get_dataset_id(id, **kwargs)
 
         # Delete dataset
         self._delete_dataset(id)
```

### Comparing `fairly-0.4.1/src/fairly/client/figshare.py` & `fairly-1.0.0/src/fairly/client/figshare.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-from typing import Any, List, Dict, Callable
+from typing import List, Dict, Callable
 
 from . import Client
 from ..metadata import Metadata
 from ..person import Person, PersonList
 from ..dataset.remote import RemoteDataset
 from ..file.local import LocalFile
 from ..file.remote import RemoteFile
 
 import re
 from urllib.parse import urlparse
 import requests
-from requests import Session
 from requests.exceptions import HTTPError
 from collections import OrderedDict
 import time
 import warnings
 import dateutil.parser
+import logging
+from functools import cached_property
 
 CLASS_NAME = "FigshareClient"
 
+
 class FigshareClient(Client):
 
     PAGE_SIZE = 25
 
     LOCKED_SLEEP = 5
     LOCKED_TRIES = 5
 
@@ -54,18 +56,15 @@
 
         # Initialize properties
         self._categories = None
 
 
     @classmethod
     def get_config_parameters(cls) -> Dict:
-        """Returns configuration parameters
-
-        Args:
-            None
+        """Returns configuration parameters.
 
         Returns:
             Dictionary of configuration parameters.
             Keys are the parameter names, values are the descriptions.
         """
         return {**super().get_config_parameters(), **{
             "token": "Access token.",
@@ -81,15 +80,58 @@
                 config["token"] = val
             else:
                 pass
 
         return config
 
 
-    def _create_session(self) -> Session:
+    @classmethod
+    def get_client(cls, url: str) -> Client:
+        """Creates a repository client from the specified URL address.
+
+        Args:
+            url (str): URL address of the repository or dataset.
+
+        Returns:
+            Client object (InvenioClient).
+
+        Raises:
+            ValueError("Invalid repository"): If repository is not valid.
+        """
+        logging.info("Checking Figshare client for %s.", url)
+        parts = urlparse(url).path.strip("/").split("/")
+        if parts[-1].isnumeric():
+            if parts[-2].isnumeric():
+                id = parts[-2]
+                version = parts[-1]
+            else:
+                id = parts[-1]
+                version = None
+        else:
+            raise ValueError("Invalid URL address")
+
+        parts = urlparse(url)
+        client = FigshareClient(
+            name=parts.hostname,
+            url=parts.scheme + "://" + parts.netloc,
+            api_url="https://api.figshare.com/v2/"
+        )
+
+        try:
+            dataset = client.get_dataset(id=id, version=version)
+        except:
+            raise ValueError("Invalid repository")
+
+        if dataset.url != url:
+            raise ValueError("Invalid repository")
+
+        return client
+
+
+    def _create_session(self) -> requests.Session:
         session = super()._create_session()
 
         # Set authentication token
         if self.config.get("token"):
             session.headers["Authorization"] = f"token {self.config['token']}"
 
         return session
@@ -107,54 +149,60 @@
         Raises:
             ValueError("Invalid id")
             ValueError("Invalid URL address")
             ValueError("No identifier")
             ValueError("Invalid version")
         """
         version = None
+
         if kwargs.get("id"):
             id = str(kwargs["id"])
             if not id.isnumeric():
                 raise ValueError("Invalid id")
+
         elif kwargs.get("url"):
             parts = urlparse(kwargs["url"]).path.strip("/").split("/")
             if parts[-1].isnumeric():
                 if parts[-2].isnumeric():
                     id = parts[-2]
                     version = parts[-1]
                 else:
                     id = parts[-1]
             else:
                 raise ValueError("Invalid URL address")
+
         elif kwargs.get("doi"):
             match = re.search(r"(\.figshare\.|\/)(\d+)(\.v(\d+))?$", kwargs["doi"])
             if match:
                 id = match.group(2)
                 version = match.group(4)
             else:
                 # TODO: Find id from DOI
                 # https://docs.figshare.com/#private_articles_search
                 raise NotImplementedError
+
         else:
             raise ValueError("No identifier")
+
         if version is None and kwargs.get("version"):
             version = str(kwargs["version"])
             if not version.isnumeric():
                 raise ValueError("Invalid version")
+
         return {"id": id, "version": version}
 
 
     def _get_dataset_hash(self, id: Dict) -> str:
         """Returns hash of the standard dataset identifier.
 
         Args:
-            id (Dict): Standard dataset identifier
+            id (Dict): Standard dataset identifier.
 
         Returns:
-            Hash string of the dataset identifier
+            Hash of the dataset identifier.
         """
         if id["version"]:
             return f"{id['id']}_{id['version']}"
         else:
             return id["id"]
 
 
@@ -199,34 +247,37 @@
         """Retrieves list of account datasets
 
         Returns:
             List of datasets related to the account
         """
         if "token" not in self.config:
             return []
+
         datasets = []
         page = 1
+
         while True:
             # TODO: Add error handling
             items, _ = self._request(f"account/articles?page={page}&page_size={self.PAGE_SIZE}")
+
             if not items:
                 break
+
             for item in items:
                 id = self.get_dataset_id(**item)
-                dataset = RemoteDataset(self, id, {
-                    "title": item.get("title"),
-                    "url": item.get("url_public_html", item.get("url_private_html")),
-                    "doi": item.get("doi"),
-                })
+                dataset = RemoteDataset(self, id)
                 datasets.append(dataset)
+
             page += 1
+
         return datasets
 
 
-    def _get_licenses(self) -> Dict:
+    @cached_property
+    def licenses(self) -> Dict:
         """Retrieves list of available licenses
 
         License dictionary:
             - id (int): License identifier
             - name (str): Name of the license
             - url (str): URL address of the license
 
@@ -335,15 +386,15 @@
     def _get_metadata(self, id: Dict) -> Dict:
         # Get record details
         details = self._get_dataset_details(id)
 
         # Set metadata attributes
         attrs = {}
 
-        def _set(key: str, val=None, source_key: str=None):
+        def _set(key: str, val=None, source_key: str=None) -> None:
             attrs[key] = details.get(source_key if source_key else key, val)
 
         # Common attributes
 
         # Authors (editable)
         val = PersonList()
         for item in details.get("authors", []):
@@ -364,15 +415,15 @@
         # Embargo deadline
         _set("embargo_date")
 
         # License
         val = details.get("license")
         if val:
             try:
-                licenses = self.get_licenses()
+                licenses = self.licenses
             except:
                 licenses = {}
 
             if isinstance(val, dict):
                 if val["value"] in licenses:
                     val = val["name"]
                 else:
@@ -498,25 +549,22 @@
         # - timeline.revision: Revision date from curation (not editable)
 
         # Return metadata attributes
         return attrs
 
 
     def save_metadata(self, id: Dict, metadata: Metadata) -> None:
-        """Saves metadata of the specified dataset
+        """Saves metadata of the specified dataset.
 
         Args:
-            id (Dict): Standard dataset id
-            metadata (Metadata): Metadata to be saved
-
-        Returns:
-            None
+            id (Dict): Standard dataset id.
+            metadata (Metadata): Metadata to be saved.
 
         Raises:
-            ValueError("No access token")
+            ValueError("No access token"): If not access token.
         """
         # Raise exception if no access token
         if not self.config.get("token"):
             raise ValueError("No access token")
 
         # Serialize metadata
         data = self._serialize_metadata(metadata)
@@ -599,26 +647,31 @@
 
         return result
 
 
     def get_files(self, id: Dict) -> List[RemoteFile]:
         # REMARK: Uses article details endpoint instead of files endpoint to support versions
         details = self._get_dataset_details(id)
+
         if "files" not in details:
             return []
+
         files = []
+
         for item in details["files"]:
+
             file = RemoteFile(
                 url=item["download_url"],
                 id=item["id"],
                 path=item["name"],
                 size=item["size"],
                 md5=item["computed_md5"],
             )
             files.append(file)
+
         return files
 
 
     def _get_license_id(self, license) -> int:
         """Returns license id from license information, e.g. name, url, id
 
         Args:
@@ -633,15 +686,15 @@
         if not license:
             return None
         elif isinstance(license, int):
             return license
         elif isinstance(license, str):
             if license.isnumeric():
                 return int(license)
-            for id, item in self.get_licenses().items():
+            for id, item in self.licenses.items():
                 if license == item["name"] or license == item["url"]:
                     return id
         elif isinstance(license, dict):
             return license["id"]
         raise ValueError("Invalid license")
 
 
@@ -652,15 +705,15 @@
             metadata (Metadata): Dataset metadata
 
         Returns:
             Client-specific dictionary of the metadata
         """
         out = {}
 
-        def _serialize(key: str, target_key=None):
+        def _serialize(key: str, target_key=None) -> None:
             if key in metadata:
                 out[key] = metadata[target_key if target_key else key]
 
         def _serialize_person(person: Person) -> Dict:
             try:
                 if person["figshare_id"]:
                     return {"id": person["figshare_id"]}
@@ -888,22 +941,19 @@
         if not file.id:
             raise ValueError("No file id")
 
         result, response = self._request(f"account/articles/{id['id']}/files/{file.id}", "DELETE")
 
 
     def _delete_dataset(self, id: Dict) -> None:
-        """Deletes dataset specified by the standard identifier from the repository
+        """Deletes dataset from the repository.
 
         Args:
             id (Dict): Standard dataset identifier
 
-        Returns:
-            None
-
         Raises:
             ValueError("Operation not permitted")
             ValueError("Invalid dataset id")
         """
         # REMARK: Only private articles can be deleted
         # https://help.figshare.com/article/ive-accidentally-set-my-data-to-public-what-should-i-do
```

### Comparing `fairly-0.4.1/src/fairly/client/zenodo.py` & `fairly-1.0.0/src/fairly/client/zenodo.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from ..person import Person, PersonList
 from ..dataset.remote import RemoteDataset
 from ..file.local import LocalFile
 from ..file.remote import RemoteFile
 
 import re
 from urllib.parse import urlparse
-from requests import Session
+import requests
 from requests.exceptions import HTTPError
 from collections import OrderedDict
 from requests_toolbelt.multipart.encoder import MultipartEncoderMonitor
 from datetime import datetime
+from functools import cached_property
 
 CLASS_NAME = "ZenodoClient"
 
 class ZenodoClient(Client):
 
     """
     Attributes:
@@ -137,18 +138,15 @@
         super().__init__(repository_id, **kwargs)
 
         self._details = {}
 
 
     @classmethod
     def get_config_parameters(cls) -> Dict:
-        """Returns configuration parameters
-
-        Args:
-            None
+        """Returns configuration parameters.
 
         Returns:
             Dictionary of configuration parameters.
             Keys are the parameter names, values are the descriptions.
         """
         return {**super().get_config_parameters(), **{
             "token": "Access token.",
@@ -164,15 +162,15 @@
                 config["token"] = val
             else:
                 pass
 
         return config
 
 
-    def _create_session(self) -> Session:
+    def _create_session(self) -> requests.Session:
         session = super()._create_session()
 
         # Set authentication token
         if self.config.get("token"):
             session.headers["Authorization"] = f"Bearer {self.config['token']}"
 
         return session
@@ -193,53 +191,54 @@
           ValueError("No identifier")
 
         """
         if "id" in kwargs:
             id = str(kwargs["id"])
             if not id.isnumeric():
                 raise ValueError("Invalid id")
+
         elif "url" in kwargs:
             parts = urlparse(kwargs["url"]).path.strip("/").split("/")
-            if parts[-1].isnumeric():
+            if parts and len(parts) >= 2 and parts[-2] == "records":
                 id = parts[-1]
             else:
                 raise ValueError("Invalid URL address")
+
         elif "doi" in kwargs:
             # REMARK: zenodo in the regular expression may not be always valid
             match = re.search(r"\/zenodo\.(\d+)$", kwargs["doi"])
             if match:
                 id = match.group(1)
             else:
                 raise ValueError("Invalid DOI")
+
         else:
             raise ValueError("No identifier")
+
         return {"id": id}
 
 
     def _get_dataset_hash(self, id: Dict) -> str:
-        """Returns hash of the standard dataset identifier
+        """Returns hash of the standard dataset identifier.
 
         Args:
-            id (Dict): Standard dataset identifier
+            id (Dict): Standard dataset identifier.
 
         Returns:
-            Hash string of the dataset identifier
+            Hash of the dataset identifier.
         """
         return id["id"]
 
 
     def _set_details(self, id: Dict, details: Dict) -> None:
         """Stores dataset details in the cache.
 
         Args:
             id (Dict): Standard dataset id.
             details (Dict): Dataset details. Set None to clear the cached details.
-
-        Returns:
-            None
         """
         hash = self._get_dataset_hash(id)
 
         if details:
             self._details[hash] = [details, datetime.now()]
 
         else:
@@ -379,33 +378,30 @@
 
     def _get_account_datasets(self) -> List[RemoteDataset]:
         if "token" not in self.config:
             return []
 
         datasets = []
         page = 1
+
         while True:
             # TODO: Add error handling
             items, _ = self._request(f"deposit/depositions?page={page}&size={self.PAGE_SIZE}")
 
             if not items:
                 break
 
             for item in items:
                 id = self.get_dataset_id(**item)
-                dataset = RemoteDataset(self, id)
-                datasets.append(dataset)
 
                 # Store details
                 self._set_details(id, item)
 
-                # Prevent unnecessary requests by triggering the use of available details
-                dataset.title
-                dataset.metadata
-                dataset.files
+                dataset = RemoteDataset(self, id)
+                datasets.append(dataset)
 
             if len(items) < self.PAGE_SIZE:
                 break
 
             page += 1
 
         return datasets
@@ -445,30 +441,28 @@
             raise ValueError("Invalid dataset id")
 
         self._set_details(id, details)
 
         return details
 
 
-    def _get_licenses(self) -> Dict:
+    @cached_property
+    def licenses(self) -> Dict:
         """Retrieves the list of available licenses
 
         License dictionary:
             - id (str): Unique id
             - name (str): Name of the license
             - url (str): URL address of the license (optional)
 
         For the complete list of data fields check the JSON schema available at:
         http://zenodo.org/schemas/licenses/license-v1.0.0.json
 
         Returns:
-            Dictionary of available licenses
-
-        Raises:
-            None
+            Dictionary of available licenses.
         """
         # REMARK: It looks like license names are not unique
         return self._get_entities("licenses", page_size = 2000, key = "id", process=lambda item: {
             "id": item["metadata"]["id"],
             "name": item["metadata"]["title"],
             "url": item["metadata"]["url"],
         })
@@ -487,18 +481,15 @@
             - created (str): Creation date of the community
             - last_record_accepted (str): Date of the last record accepted
             - description (str): Short description of the community
             - about (str): Long description of the community
             - curation_policy (str): Curation policy of the community
 
         Returns:
-            List of community dictionaries
-
-        Raises:
-            None
+            List of community dictionaries.
         """
         return self._get_entities("communities", page_size=2000, process=lambda item: {
             "id": item["id"],
             "name": item["title"],
             "url": item["links"]["html"],
             "logo_url": item["logo_url"],
             "created": item["created"],
@@ -522,18 +513,15 @@
             - country (str): Country code of the funder
             - acronyms (list): Acronyms of the funder
 
         For the complete list of data fields check the JSON schema available at:
         http://zenodo.org/schemas/funders/funder-v1.0.0.json
 
         Returns:
-            List of funder dictionaries
-
-        Raises:
-            None
+            List of funder dictionaries.
         """
         return self._get_entities("funders", page_size=2000, process=lambda item: {
             # REMARK: Zenodo uses DOI to identify funders
             "id": item["metadata"]["doi"],
             "name": item["metadata"]["name"],
             "type": item["metadata"]["type"],
             "subtype": item["metadata"]["subtype"],
@@ -588,36 +576,39 @@
 
         # Set metadata attributes
 
         # REMARK: Attributes follow the order of the Zenodo API documentation
         # https://developers.zenodo.org/#deposit-metadata
         attrs = {}
 
-        def _set(key: str, val=None, source_key: str=None):
+        def _set(key: str, val=None, source_key: str=None) -> None:
             attrs[key] = metadata.get(source_key if source_key else key, val)
 
         def _get_person(item: Dict) -> Person:
             return Person(
                 fullname = item.get("name"),
                 institution = item.get("affiliation"),
                 orcid_id = item.get("orcid"),
                 gnd_id = item.get("gnd"),
                 role = item.get("type")
             )
 
         # Common attributes
 
         # Record type
-        type = metadata["upload_type"]
-        if type == "publication":
+        type = metadata["upload_type"] if "upload_type" in metadata else metadata["resource_type"]["type"]
+
+        if type == "publication" and ("publication_type" in metadata):
             if metadata["publication_type"] != "other":
                 type = metadata["publication_type"]
+
         elif type == "image":
             if metadata["image_type"] != "other":
                 type = metadata["image_type"]
+
         attrs["type"] = type
 
         # Date of publication in ISO8601 format (YYYY-MM-DD)
         _set("publication_date")
 
         # Title
         _set("title")
@@ -660,15 +651,15 @@
         # List of contributors
         attrs["contributors"] = PersonList([_get_person(item) for item in metadata.get("contributors", [])])
 
         # List of references
         _set("references", [])
 
         # List of communities the record appear
-        attrs["communities"] = [item["identifier"] for item in metadata.get("communities", [])]
+        attrs["communities"] = [item.get("identifier", item.get("id")) for item in metadata.get("communities", [])]
 
         # List of OpenAIRE-supported grants that funded the research
         attrs["grants"] = [item["id"] for item in metadata.get("grants", [])]
 
         # Journal article attributes
         if type == "article":
             _set("journal_title")
@@ -759,15 +750,15 @@
             metadata (Metadata): Dataset metadata
 
         Returns:
             Client-specific dictionary of the metadata
         """
         out = {}
 
-        def _serialize(key: str, default=None):
+        def _serialize(key: str, default=None) -> None:
             if key in metadata:
                 out[key] = metadata[key]
             elif default is not None:
                 out[key] = default
 
         _serialize("title", "")
 
@@ -861,17 +852,14 @@
     def save_metadata(self, id: Dict, metadata: Metadata) -> None:
         """Saves metadata of the specified dataset
 
         Args:
             id (Dict): Standard dataset id
             metadata (Metadata): Metadata to be saved
 
-        Returns:
-            None
-
         Raises:
             ValueError("No access token")
         """
         # Raise exception if no access token
         if not self.config.get("token"):
             raise ValueError("No access token")
 
@@ -917,44 +905,57 @@
             pass
 
         return result
 
 
     def get_files(self, id: Dict) -> List[RemoteFile]:
         details = self._get_dataset_details(id)
+
         if "files" not in details:
             return []
+
         files = []
+
         for item in details["files"]:
-            # REMARK: Depending on the endpoint file information differs
-            if "id" in item:
-                file = RemoteFile(
-                    id=item["id"],
-                    url=item["links"]["download"],
-                    path=item["filename"],
-                    size=item["filesize"],
-                    md5=item["checksum"],
-                )
-            else:
-                file = RemoteFile(
-                    url=item["links"]["self"],
-                    path=item["key"],
-                    size=item["size"],
-                    md5=item["checksum"][4:],
+
+            args = {
+                "id": item.get("id"),
+                "path": item.get("filename", item.get("key")),
+                "size": item.get("filesize", item.get("size")),
+                "md5": item.get("checksum"),
+                "url": item["links"]["self"]
+            }
+
+            # Fix invalid download link if required
+            if "download" in item["links"]:
+                # args["url"] = item["links"]["download"]
+                args["url"] = (
+                    args["url"][:args["url"].find("/files/")]
+                    +
+                    item["links"]["download"][item["links"]["download"].find("/files/"):]
                 )
+
+            # Remove 'md5:' prefix from the checksum if required
+            # REMARK: string.removeprefix() method can be used for Python 3.9+
+            if args["md5"] and args["md5"].startswith("md5:"):
+                args["md5"] = args["md5"][4:]
+
+            file = RemoteFile(**args)
+
             files.append(file)
+
         return files
 
 
     def _upload_file(self, id: Dict, file: LocalFile, notify: Callable=None) -> RemoteFile:
         # REMARK: requests_toolbelt MultipartEncoder is used to stream data
         # ref: https://stackoverflow.com/questions/22915295/python-requests-post-and-big-content
         # ref: https://stackoverflow.com/questions/12385179/how-to-send-a-multipart-form-data-with-requests-in-python
 
-        def _notify(monitor):
+        def _notify(monitor) -> None:
             if notify:
                 notify(file, monitor.bytes_read)
 
         encoder = MultipartEncoderMonitor.from_fields(
             fields={
                 'file': (file.path, open(file.fullpath, 'rb'), file.type),
             },
@@ -1001,17 +1002,14 @@
 
     def _delete_dataset(self, id: Dict) -> None:
         """Deletes dataset specified by the standard identifier from the repository
 
         Args:
             id (Dict): Standard dataset identifier
 
-        Returns:
-            None
-
         Raises:
             ValueError("Operation not permitted")
             ValueError("Invalid dataset id")
         """
         # REMARK: Only unpublished depositions can be deleted
         try:
             result, response = self._request(f"deposit/depositions/{id['id']}", "DELETE")
@@ -1061,21 +1059,33 @@
             "unsubmitted": "draft",
             "error": "error",
             "open": "public",
             "embargoed": "embargoed",
             "restricted": "restricted",
             "closed": "closed",
         }
-        state = details["state"] if details["state"] != "done" else details["metadata"]["access_right"]
+
+        if "state" in details and details["state"] != "done":
+            state = details["state"]
+
+        elif "access_right" in details["metadata"]:
+            state = details["metadata"]["access_right"]
+
+        elif "access" in details:
+            state = details["access"].get("status")
+
+        else:
+            state = None
+
         status = statuses.get(state, "unknown")
 
         # Calculate data size
         size = 0
         for file in details.get("files", []):
-            size += file["filesize"]
+            size += file.get("filesize", file.get("size"))
 
         return {
             "title": details["title"],
             "url": details["links"].get("html"),
             "doi": details.get("doi"),
             "status": status,
             "size": size,
```

### Comparing `fairly-0.4.1/src/fairly/data/languages/ISO-639-2_8859-1.tab` & `fairly-1.0.0/src/fairly/data/languages/ISO-639-2_8859-1.tab`

 * *Files identical despite different names*

### Comparing `fairly-0.4.1/src/fairly/data/languages/ISO-639-2_UTF-8.tab` & `fairly-1.0.0/src/fairly/data/languages/ISO-639-2_UTF-8.tab`

 * *Files identical despite different names*

### Comparing `fairly-0.4.1/src/fairly/data/languages/ISO-639-3_8859-1.tab` & `fairly-1.0.0/src/fairly/data/languages/ISO-639-3_8859-1.tab`

 * *Files identical despite different names*

### Comparing `fairly-0.4.1/src/fairly/data/languages/ISO-639-3_UTF-8.tab` & `fairly-1.0.0/src/fairly/data/languages/ISO-639-3_UTF-8.tab`

 * *Files identical despite different names*

### Comparing `fairly-0.4.1/src/fairly/data/templates/default.yaml` & `fairly-1.0.0/src/fairly/data/templates/default.yaml`

 * *Files identical despite different names*

### Comparing `fairly-0.4.1/src/fairly/data/templates/figshare.yaml` & `fairly-1.0.0/src/fairly/data/templates/figshare.yaml`

 * *Files identical despite different names*

### Comparing `fairly-0.4.1/src/fairly/data/templates/zenodo.yaml` & `fairly-1.0.0/src/fairly/data/templates/zenodo.yaml`

 * *Files identical despite different names*

### Comparing `fairly-0.4.1/src/fairly/dataset/__init__.py` & `fairly-1.0.0/src/fairly/dataset/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,99 +1,113 @@
+"""Dataset class module.
+
+Dataset class is used to represent datasets in a standardized manner.
+It is an abstract class.
+
+Implementations:
+    LocalDataset
+    RemoteDataset
+"""
 from __future__ import annotations
-from typing import List, Dict, Union
+from typing import List, Dict
 from abc import ABC, abstractmethod
 
 import datetime
 
 from ..metadata import Metadata
 from ..file import File
 from ..diff import Diff
 
 
 class Dataset(ABC):
-    """
+    """Dataset class.
 
     Attributes:
-      _metadata (Metadata): Metadata
-      _files (list): Files list
-      _modified (datetime.datetime): Last known modification date
-      _auto_refresh (bool): Auto-refresh flag
-
+      _metadata (Metadata): Metadata.
+      _files (list): Files list.
+      _modified (datetime.datetime): Last known modification date.
+      _auto_refresh (bool): Auto-refresh flag.
     """
 
     def __init__(self, auto_refresh: bool=False):
         """Initializes Dataset object.
 
         Args:
-            auto_refresh (bool): Set True to auto-refresh dataset information
+            auto_refresh (bool): Set True to auto-refresh dataset information (default False).
         """
         self._metadata = None
         self._files = None
         self._modified = None
         self._auto_refresh = auto_refresh
 
 
     @abstractmethod
     def _get_metadata(self) -> Metadata:
-        """Retrieves metadata of the dataset
+        """Retrieves metadata of the dataset.
 
         Returns:
-            Metadata of the dataset
+            Metadata of the dataset.
         """
         raise NotImplementedError
 
 
     def get_metadata(self, refresh: bool=False) -> Metadata:
-        """Returns metadata of the dataset
+        """Returns metadata of the dataset.
 
         Args:
-            refresh (bool): Set True to enforce metadata retrieval
+            refresh (bool): Set True to enforce metadata retrieval (default False).
 
         Returns:
-            Metadata of the dataset
+            Metadata of the dataset.
         """
         if self._metadata is None or refresh:
             self._metadata = self._get_metadata()
             self._modified = self.modified
 
         return self._metadata
 
 
     @property
     def metadata(self) -> Metadata:
-        """Metadata of the dataset"""
+        """Metadata of the dataset.
+
+        Refreshes metadata automatically if metadata object is not modified by
+        the user, auto-fresh flag is set, and metadata is modified externally.
+        """
         if self._metadata and self._metadata.is_modified:
             refresh = False
         else:
             refresh = self._auto_refresh and self.is_modified
 
         return self.get_metadata(refresh=refresh)
 
 
     def set_metadata(self, **kwargs) -> None:
+        """Sets metadata attributes.
+
+        Args:
+            **kwargs: Metadata attributes.
+        """
         self.metadata.update(kwargs)
 
 
     @abstractmethod
     def _save_metadata(self) -> None:
-        """Stores dataset metadata"""
+        """Stores dataset metadata."""
         raise NotImplementedError
 
 
     def save_metadata(self, force: bool=False) -> None:
-        """Stores dataset metadata if exists
+        """Stores dataset metadata if exists.
 
         Args:
-            force (bool): Set True to enforce save even if existing dataset is modified
-
-        Returns:
-            None
+            force (bool): Set True to enforce save even if existing dataset is modified (default False).
 
         Raises:
-            Warning("Existing dataset is modified")
+            Warning("Existing dataset is modified"): If dataset is modified.
         """
         if self._metadata is None:
             return
 
         # REMARK: It can be better to check if metadata is actually changed
         if self.is_modified and not force:
             raise Warning("Existing dataset is modified")
@@ -101,67 +115,82 @@
         self._save_metadata()
 
         self.get_metadata(refresh=True)
 
 
     @abstractmethod
     def _get_files(self) -> List[File]:
+        """Returns list of files of the dataset."""
         raise NotImplementedError
 
 
     def get_files(self, refresh: bool=False) -> Dict[str, File]:
-        """Returns dictionary of files of the dataset
+        """Returns dictionary of files of the dataset.
 
         Args:
-            refresh (bool): Set True to enforce file list retrieval
+            refresh (bool): Set True to enforce file list retrieval.
 
         Returns:
-            Dictionary of files of the dataset (key = path, value = File object)
+            Dictionary of files of the dataset.
+            Keys are paths, values are File objects.
         """
         if self._files is None or refresh or self.auto_refresh:
             files = {}
             for file in self._get_files():
                 files[file.path] = file
             self._files = files
             self._modified = self.modified
 
         return self._files
 
 
     @property
     def files(self) -> List[File]:
-        """List of files of the dataset"""
+        """List of files of the dataset."""
         return self.get_files(refresh=self.is_modified)
 
 
     def get_file(self, val: str, refresh: bool=False) -> File:
+        """Returns specified file of the dataset.
+
+        Args:
+            val (str): File identifier.
+            refresh (bool): Set True to enforce file information retrieval.
+
+        Returns:
+            File object if file is found, None otherwise.
+        """
         # TODO: Implement without using get_files()
         files = self.get_files(refresh)
 
         if isinstance(val, int):
             return list(files.values())[val]
 
         for key, file in files.items():
             if file.match(val):
                 return file
 
         return None
 
 
     def file(self, val: str) -> File:
+        """Returns specified file of the dataset.
+
+        Automatically refreshes file information if dataset is modified.
+        """
         return self.get_file(val, refresh=self.is_modified)
 
 
     @abstractmethod
     def reproduce(self) -> Dataset:
         """Reproduces an actual copy of the dataset."""
         raise NotImplementedError
 
 
-    def diff_metadata(self, dataset: Dataset=None):
+    def diff_metadata(self, dataset: Dataset=None) -> Diff:
         diff = Diff()
 
         if dataset is None:
             dataset = self.reproduce()
 
         metadata = self.metadata
         other_metadata = dataset.metadata
@@ -209,17 +238,18 @@
             if path not in files:
                 diff.remove(path, other_file)
 
         return diff
 
 
     @property
+    @abstractmethod
     def title(self) -> str:
         """Title of the dataset."""
-        return self.metadata["title"]
+        raise NotImplementedError
 
 
     @property
     @abstractmethod
     def size(self) -> int:
         """Total size of the dataset in bytes."""
         raise NotImplementedError
@@ -247,13 +277,15 @@
             True if the existing dataset is modified, False otherwise.
         """
         return None if self._modified is None else self._modified != self.modified
 
 
     @property
     def auto_refresh(self) -> bool:
+        """Auto-refresh flag of the dataset."""
         return self._auto_refresh
 
 
     @auto_refresh.setter
-    def auto_refresh(self, val):
+    def auto_refresh(self, val) -> None:
+        """Sets auto-refresh flag of the dataset."""
         self._auto_refresh = bool(val)
```

### Comparing `fairly-0.4.1/src/fairly/dataset/local.py` & `fairly-1.0.0/src/fairly/dataset/local.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List, Dict, Set
 
 from . import Dataset
 from ..metadata import Metadata
 from ..file.local import LocalFile
 from .remote import RemoteDataset
 from ..client import Client
+from typing import Callable
 
 import fairly
 
 import os
 import os.path
 from ruamel.yaml import YAML
 import re
@@ -24,19 +25,19 @@
     """
 
     Attributes:
         _path (str): Path of the dataset
         _manifest_path (str): Path of the dataset manifest
         _includes (set): File inclusion rules
         _excludes (set): File exclusion rules
-        _md5s (dict): MD5 hash cache of the files
+        _md5s (Dict): MD5 checksum cache of the files
         _yaml: YAML object
 
     Class Attributes:
-        _regexps (dict): Regular expression cache of the file rules
+        _regexps (Dict): Regular expression cache of the file rules
     """
 
     _regexps: Dict = {}
 
     def __init__(self, path: str, auto_refresh: bool=True):
         """Initializes LocalDataset object.
 
@@ -60,15 +61,15 @@
         # Set manifest path
         self._manifest_path = os.path.join(path, "manifest.yaml")
 
         # Set file rules
         self._includes = None
         self._excludes = None
 
-        # Load cached MD5 hashes
+        # Load cached MD5 checksums
         self._load_md5s()
 
         self._yaml = YAML()
         self._yaml.allow_unicode = True
         self._yaml.encoding = "utf-8"
 
 
@@ -161,17 +162,14 @@
 
 
     def _set_manifest(self, manifest: Dict) -> None:
         """Stores the dataset manifest.
 
         Args:
             manifest (Dict): Dataset manifest
-
-        Returns:
-            None
         """
         if "metadata" not in manifest:
             manifest["metadata"] = {}
 
         if "files" not in manifest:
             manifest["files"] = {
                 "includes": [],
@@ -211,36 +209,32 @@
                        directory, e.g. data/table.csv, data/results.csv
         data/*/*.cvs : Files with the .csv extension under the sub-directories
                        of the data directory, e.g. data/set1/results.csv,
                        data/set2/results.csv
 
         Returns:
             True if file name matches the rule, False otherwise
-
-        Raises:
-            None
-
         """
         if not rule in self._regexps:
             regexps = []
             for part in os.path.normpath(rule).split(os.sep):
                 if part:
                     pattern = re.escape(part).replace("\*", ".*").replace("\?", ".")
-                    regexp = re.compile(f"^{pattern}$", re.IGNORECASE)
+                    regexp = re.compile(pattern, re.IGNORECASE)
                 else:
                     regexp = None
                 regexps.append(regexp)
             self._regexps[rule] = regexps
         for i, part in enumerate(os.path.normpath(name).split(os.sep)):
             try:
                 regexp = self._regexps[rule][i]
             except:
                 regexp = None
             if part:
-                if not regexp or not regexp.match(part):
+                if not regexp or not regexp.fullmatch(part):
                     return False
             elif regexp:
                 return False
         return True
 
 
     def _get_files(self) -> List[LocalFile]:
@@ -302,15 +296,15 @@
                         md5 = md5
                     )
                     files.append(file)
         return files
 
 
     def _load_md5s(self) -> None:
-        """Loads MD5 hashes stored in the dataset directory"""
+        """Loads MD5 checksums stored in the dataset directory"""
         self._md5s = {}
         path = os.path.join(self.path, ".fairly_md5")
         try:
             with open(path, "r") as file:
                 reader = csv.reader(file)
                 for name, date, size, md5 in reader:
                     self._md5s[name] = (date, size, md5)
@@ -320,33 +314,28 @@
 
     def save_files(self, force: bool=False) -> None:
         """Stores dataset file list if exists.
 
         Args:
             force (bool): Set True to enforce save even if existing dataset is modified
 
-        Returns:
-            None
-
         Raises:
             Warning("Existing dataset is modified")
         """
         # REMARK: It can be better to check if file list is actually changed
         if self.is_modified and not force:
             raise Warning("Existing dataset is modified")
 
         manifest = self._get_manifest()
         manifest["files"] = {
             "includes": self.includes,
             "excludes": self.excludes,
         }
         self._set_manifest(manifest)
 
-        self.get_files(refresh=True)
-
 
     def save(self) -> None:
         """Saves metadata and file inclusion/exclusion rules."""
         self.save_metadata()
         self.save_files()
 
 
@@ -492,14 +481,20 @@
         if client.repository_id:
             self.set_remote_dataset(dataset)
 
         return dataset
 
 
     @property
+    def title(self) -> str:
+        """Title of the dataset."""
+        return self.metadata["title"]
+
+
+    @property
     def size(self) -> int:
         """Total size of the dataset in bytes."""
         size = 0
         for file in self.files.values():
             size += file.size
 
         return size
@@ -535,32 +530,26 @@
 
     def synchronize(self, source, notify: Callable=None) -> None:
         if not isinstance(source, Dataset):
             source = fairly.dataset(source)
 
         diff = source.diff_metadata(self)
         # TODO: Synchronize metadata
-        print(diff)
 
         diff = source.diff_files(self)
 
         for file in diff.added.values():
             pass
 
 
     def reproduce(self) -> LocalDataset:
         """Reproduces an actual copy of the dataset."""
         return LocalDataset(self.path)
 
 
-    def reproduce(self) -> LocalDataset:
-        """Reproduces an actual copy of the dataset."""
-        return LocalDataset(self.path)
-
-
     def set_remote_dataset(self, dataset) -> None:
         if not isinstance(dataset, RemoteDataset):
             dataset = fairly.dataset(dataset)
             if not isinstance(dataset, RemoteDataset):
                 raise ValueError("Invalid remote dataset")
 
         id = dataset.client.repository_id
@@ -589,14 +578,31 @@
             elif remote_datasets:
                 return list(remote_datasets.values())[0]
 
         return None
 
 
     def push(self, target=None, notify: Callable=None) -> RemoteDataset:
+        """
+        Pushes local changes to metadata and files the data repository to
+        update a remote dataset. Dataset must exits in data repository.
+
+        Args:
+            target: Target repository identifier or client. If not specified,
+            identifier in manifest is used.
+            notify (Callable): Notification callback function.
+
+        Returns:
+            Remote dataset
+
+        Raises:
+            ValueError("No target dataset"): If target dataset is not specified.
+
+        """
+
         remote = self.get_remote_dataset(target)
         if not remote:
             raise ValueError("No target dataset")
 
         diff = self.diff_metadata(remote)
         if diff:
             remote.set_metadata(**self.metadata)
@@ -616,32 +622,54 @@
                 client.upload_file(remote, file)
 
             remote.get_files(refresh=True)
 
         return remote
 
 
-    def pull(self, source=None, notify: Callable=None) -> None:
+    def pull(self, source=None, notify: Callable=None) -> RemoteDataset:
+        """
+        Pulls changes made to metadata and files from the data repository
+        to update the local dataset. Dataset must exits in data repository.
+
+        Args:
+            source: Source repository identifier or client. If not specified,
+            identifier in manifest is used.
+            notify (Callable): Notification callback function.
+
+        Returns:
+            Remote dataset
+
+        Raises:
+            ValueError("No source dataset"): If source dataset is not specified.
+
+        """
+
         remote = self.get_remote_dataset(source)
         if not remote:
             raise ValueError("No source dataset")
 
         diff = remote.diff_metadata(self)
         if diff:
             self.set_metadata(**remote.metadata)
             self.save_metadata()
 
         diff = remote.diff_files(self)
         if diff:
             client = remote.client
             for file in diff.added.values():
                 client.download_file(file, path=self.path, notify=notify)
+                self.includes.append(file.path)
 
             for file in diff.removed.values():
                 os.remove(file.fullpath)
+                if file.path in self.includes:
+                    self.includes.remove(file.path)
+                else:
+                    self.excludes.append(file.path)
 
             for file, remote_file in diff.modified.values():
                 os.remove(file.fullpath)
                 client.download_file(remote_file, path=self.path, notify=notify)
 
             self.get_files(refresh=True)
```

### Comparing `fairly-0.4.1/src/fairly/dataset/remote.py` & `fairly-1.0.0/src/fairly/dataset/remote.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,76 @@
 from __future__ import annotations
-from typing import List, Dict, Callable
+from typing import Any, List, Dict, Callable
 
 import fairly
 
 from . import Dataset
 from ..metadata import Metadata
 from ..file.local import LocalFile
 from ..file.remote import RemoteFile
 # FIXME: Importing Client or LocalDataset results in circular dependency
 # from ..client import Client
 
 import os
+import os.path
 import datetime
+import concurrent.futures
 from functools import cached_property
+import logging
+
 
 class RemoteDataset(Dataset):
     """
 
     Attributes:
         _client (Client): Client object
         _id (str): Dataset identifier
         _details (Dict): Dataset details
 
     """
 
-    def __init__(self, client, id=None, auto_refresh: bool=True, details: Dict=None, **kwargs):
+    def __init__(self, client, id=None, auto_refresh: bool=True, **kwargs):
         """Initializes RemoteDataset object.
 
         Args:
             client (Client): Client of the dataset
             id: Dataset identifier
             auto_refresh (bool): Set True to auto-refresh dataset information
         """
         # Call parent method
         super().__init__(auto_refresh=auto_refresh)
+
         # Set client
         self._client = client
+
         # Set dataset id
         self._id = client.get_dataset_id(id, **kwargs)
 
-        if id and isinstance(id, str):
-            key, val = Client.parse_id(id)
-            kwargs[key] = val
-
-        # REMARK: User-specific details should be validated once actual details becomes available
-        self._details = None if not details else details.copy()
+        # Set details
+        self._details = client.get_details(self.id)
 
 
     @property
     def client(self) -> Client:
-        """Client of the dataset"""
+        """Client of the dataset."""
         return self._client
 
 
     @property
     def id(self) -> Dict:
-        """Identifier of the dataset"""
+        """Identifier of the dataset."""
         return self._id
 
 
+    @property
+    def plain_id(self) -> str:
+        """Plain identifier of the dataset."""
+        return self._client.get_dataset_plain_id(self._id)
+
+
     def _get_metadata(self) -> Metadata:
         return self.client.get_metadata(self.id)
 
 
     def _save_metadata(self) -> None:
         return self.client.save_metadata(self.id, self.metadata)
 
@@ -76,85 +84,126 @@
 
         Returns:
             List of remote datasets of all available versions.
         """
         return self.client.get_versions(self.id)
 
 
-    def _download_file(self, file: RemoteFile, path: str=None, name: str=None, notify: Callable=None) -> LocalFile:
-        return self.client.download_file(file, path, name, notify)
+    def _store_file(self, file, path, extract, notify):
+        # Download file
+        local_file = self.client.download_file(file, path, notify=notify)
+
+        # Check if file should be extracted
+        if extract and local_file.is_archive and local_file.is_simple:
+
+            # Start extraction loop
+            while True:
+                files = local_file.extract(path, notify=notify)
+                os.remove(local_file.fullpath)
+
+                if len(files) == 1:
+                    inner_file = LocalFile(os.path.join(path, files[0]))
+                    if inner_file.is_archive:
+                        local_file = inner_file
+                        continue
+
+                break
+
+            return {file.path: files}
+
+        else:
+            return file.path
 
 
-    def store(self, path: str=None, notify: Callable=None, extract: bool=False) -> LocalDataset:
+    def store(self, path: str=None, notify: Callable=None, extract: bool=False, max_workers: int=None) -> LocalDataset:
         """Stores the dataset to a local directory.
 
         If no path is provided, DOI is used by replacing slashes and backslashes with underscores.
         Local directory is created if it does not exist.
 
         Args:
             path (str): Path to the local directory (optional).
             notify (Callable): Notification callback method (optional).
-            extract (bool): Set True to extract archive files (default = False).
+            extract (bool): Set True to extract archive files (default False).
+            max_workers (int): Number of workers (optional).
 
         Returns:
             LocalDataset object of the stored local dataset.
 
         Raises:
             ValueError("Empty path")
             ValueError("Directory is not empty")
         """
+        # Set number of workers if required
+        if not max_workers:
+            max_workers = fairly.max_workers()
+
+        # Set path based on DOI if required
         if not path:
             path = self.doi
             if not path:
                 raise ValueError("Empty path")
             for sep in ["/", "\\"]:
                 path = path.replace(sep, "_")
 
+        # Create path
         os.makedirs(path, exist_ok=True)
 
         # check if directory is empty,
         # while ignoring hidden files or directories
         entries = os.listdir(path)
         visible_entries = [entry for entry in entries if not entry.startswith(".")]
         if len(visible_entries) > 0:
             raise ValueError("Directory is not empty.")
 
+        # Set dataset template
         templates = fairly.metadata_templates()
+
         if self.client.repository_id in templates:
             template = self.client.repository_id
+
         elif self.client.client_id in templates:
             template = self.client.client_id
+
         else:
             template = None
 
+        # Initialize dataset
         dataset = fairly.init_dataset(path, template=template)
 
+        # Save metadata
         # TODO: Set metadata directly without serialization
         dataset.set_metadata(**self.metadata)
         dataset.save_metadata()
 
-        includes = dataset.includes
-        for name, file in self.files.items():
-            local_file = self._download_file(file, path, notify=notify)
-            if extract and local_file.is_archive and local_file.is_simple:
-                files = local_file.extract(path, notify=notify)
-                includes.append({file.path: files})
-                os.remove(local_file.fullpath)
-            else:
-                includes.append(file.path)
+        with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
+
+            futures = []
+
+            for _, file in self.files.items():
+                futures.append(
+                    executor.submit(self._store_file, file, path, extract, notify)
+                )
+
+            for future in concurrent.futures.as_completed(futures):
+                dataset.includes.append(future.result())
+
+        # Save file information
         dataset.save_files()
 
+        # Set remote dataset id if possible
+        # REMARK: It might be possible to store configuration for custom clients.
         if self.client.repository_id:
             dataset.set_remote_dataset(self)
 
         return dataset
 
 
     def _get_detail(self, key: str, refresh: bool=False) -> Any:
-        if not self._details or key not in self._details or refresh:
+        if refresh:
             self._details = self.client.get_details(self.id)
 
         return self._details.get(key)
 
 
     @property
     def title(self) -> str:
@@ -192,15 +241,22 @@
         """
         return self._get_detail("status")
 
 
     @property
     def size(self) -> int:
         """Total size of the dataset in bytes."""
-        return self._get_detail("size")
+        size = self._get_detail("size")
+
+        if size is None:
+            size = 0
+            for file in self.get_files():
+                size += file.size
+
+        return size
 
 
     @cached_property
     def created(self) -> datetime.datetime:
         """Creation date and time of the dataset"""
         return self._get_detail("created")
```

### Comparing `fairly-0.4.1/src/fairly/diff.py` & `fairly-1.0.0/src/fairly/diff.py`

 * *Files identical despite different names*

### Comparing `fairly-0.4.1/src/fairly/file/local.py` & `fairly-1.0.0/src/fairly/file/local.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" LocalFile class module.
+"""LocalFile class module.
 
 LocalFile class is used to perform operations on local files.
 
 Usage example:
 
     >>> file = LocalFile("/path/to/local/file/filename.txt")
     >>> file.type
@@ -17,100 +17,121 @@
 
 import os
 import os.path
 import mimetypes
 import hashlib
 import zipfile
 import tarfile
+import logging
 
 
 class LocalFile(File):
     """LocalFile class.
 
     Class Attributes:
-        CHUNK_SIZE: Chunk size in bytes to calculate MD5 checksum (default = 65536)
+        CHUNK_SIZE: Chunk size in bytes to calculate MD5 checksum (default = 65536).
+        NO_EXTRACT: List of file extensions which should not be extracted.
+
+    Attributes:
+        _fullpath (str): Full path of the local file.
     """
-    CHUNK_SIZE = 2**16
 
+    CHUNK_SIZE = 2**18
+
+    NO_EXTRACT = [
+        ".docx",
+        ".xlsx",
+        ".pptx",
+    ]
 
     def __init__(self, fullpath: str, basepath: str = None, md5: str = None):
         """Initializes LocalFile object.
 
+        Args:
+            fullpath (str): Full path of the local file.
+            basepath (str): Base path of the local file (optional).
+            md5 (str): MD5 checksum of the local file (optional).
+
         Raises:
-            ValueError("Invalid file path"): If fullpath is not a valid file path
+            ValueError("Invalid file path"): If fullpath is not a valid file path.
         """
         if not os.path.isfile(fullpath):
             raise ValueError("Invalid file path")
         self._fullpath = fullpath
-        self._path = os.path.relpath(
-            fullpath, basepath) if basepath else fullpath
+        self._path = os.path.relpath(fullpath, basepath) if basepath else fullpath
         self._name = os.path.basename(fullpath)
         self._size = os.path.getsize(fullpath)
         self._type = None
         self._md5 = md5
 
 
     @property
     def fullpath(self) -> str:
-        """Full path of the file.
-
-        Returns:
-            Full path of the file (str).
-        """
+        """Full path of the local file."""
         return self._fullpath
 
 
     @property
     def type(self) -> str:
-        """MIME type of the file.
-
-        Returns:
-            MIME type of the file (str).
-        """
+        """Content type of the local file."""
         if self._type is None:
+            logging.info("Guessing content type of %s.", self.fullpath)
             self._type, _ = mimetypes.guess_type(self.fullpath)
+            logging.info("Guessed content type is %s.", self._type)
+
         return self._type
 
 
     @property
     def md5(self) -> str:
-        """MD5 checksum of the file.
+        """MD5 checksum of the local file.
 
-        Returns:
-            MD5 checksum of the file (str).
+        MD5 checksum is only calculated once and cached for subsequent calls.
         """
         if self._md5 is None:
+            logging.info("Calculating MD5 checksum of %s.", self.fullpath)
             with open(self.fullpath, "rb") as file:
                 md5 = hashlib.md5()
                 while chunk := file.read(self.CHUNK_SIZE):
                     md5.update(chunk)
             self._md5 = md5.hexdigest()
+            logging.info("Calculated MD5 checksum is %s.", self._md5)
+
         return self._md5
 
 
     @property
     def is_archive(self) -> bool:
         """Checks if file is an archive file.
 
         Returns:
             True if file is an archive file, False otherwise.
         """
+        if self.NO_EXTRACT and (self.extension in self.NO_EXTRACT):
+            return False
+
         if zipfile.is_zipfile(self.fullpath):
             return True
 
         elif tarfile.is_tarfile(self.fullpath):
             return True
 
         else:
             return False
 
 
     def match(self, val: str) -> bool:
         """Checks if file matches the specified file identifier.
 
+        File fullpath is compared with the specified identifier in addition to
+        the properties checked by File.match().
+
+        Args:
+            val (str): File identifier.
+
         Returns:
             True if file matches the specified file identifier, False otherwise.
         """
         return True if self.fullpath == val else super().match(val)
 
 
     def extract(self, path: str = None, notify: Callable = None) -> List:
@@ -119,26 +140,26 @@
         Args:
             path: Path of the directory to extract to. Default is the
                 current working directory.
 
             notify: Notification callback function. Three arguments are
                 provided to the callback function:
 
-                - file (LocalFile): File object of the extracted local file
+                - file (LocalFile): File object of the extracted local file.
                 - current_size (int): Current total uncompressed size of
                     extracted files.
-                - total_size (int): Total uncompressed size of the archive
+                - total_size (int): Total uncompressed size of the archive.
 
         Raises:
-          ValueError("Invalid path"): If path is not a directory path.
-          ValueError("Invalid archive item {name}"): If archive item path is not valid.
-          ValueError("Invalid archive file"): If file is not an archive file.
+            ValueError("Invalid path"): If path is not a directory path.
+            ValueError("Invalid archive item {name}"): If archive item path is not valid.
+            ValueError("Invalid archive file"): If file is not an archive file.
 
         Returns:
-          List of names of extracted files (str).
+            List of names of extracted files (str).
         """
         # Raise exception if invalid path
         if path:
             if not os.path.isdir(path):
                 raise ValueError("Invalid path")
         else:
             path = ""
```

### Comparing `fairly-0.4.1/src/fairly/metadata.py` & `fairly-1.0.0/src/fairly/metadata.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,51 +5,56 @@
 Usage example:
 
     >>> metadata = Metadata({"title": "Title", "DOI": "doi:xxx"})
     >>> metadata["authors"] = ["Doe, John"]
 
 """
 from __future__ import annotations
-from typing import Any, Dict
+from typing import Any, Dict, List, Callable
 from collections.abc import MutableMapping
 
 from .person import Person, PersonList
 
 import re
 import copy
 import sys
 import ruamel.yaml
 
+
 class Metadata(MutableMapping):
     """Metadata class.
 
     Attributes:
-        _normalize (Callable): Attribute normalization method.
         _attrs (Dict): Metadata attributes.
         _basis (Dict): Basis of metadata attributes.
+        _normalize (Callable): Attribute normalization method.
+        _serialize (Callable): Attribute serialization method.
 
     Class Attributes:
         REGEXP_DOI: Regular expression to validate DOI.
     """
 
-    REGEXP_DOI = re.compile(r"^10.\d{4,9}/[-._;()/:a-z0-9]+$", re.IGNORECASE)
+    REGEXP_DOI = re.compile(r"10\.\d{4,9}/[-._;()/:a-z\d]+", re.IGNORECASE)
 
 
-    def __init__(self, normalize: Callable=None, **kwargs):
+    def __init__(self, normalize: Callable=None, serialize: Callable=None, **kwargs):
         """Initializes Metadata object.
 
-        The default normalization method `Metadata.normalize()` is not called
-        if user-defined normalization method is provided.
+        The corresponding default methods are not called if user-defined
+        attribute value normalization and serialization methods are provided.
 
         Args:
-            normalize: User-defined normalization method.
+            normalize: Attribute value normalization method (optional).
+            serialize: Attribute value serialization method (optional).
             **kwargs: Metadata attributes.
         """
-        self._normalize = normalize if normalize else Metadata.normalize
+        self._normalize = normalize if normalize else Metadata.normalize_value
+        self._serialize = serialize if serialize else Metadata.serialize_value
         self._attrs = {}
+
         for key, val in kwargs.items():
             if bool(val) or isinstance(val, (bool, int, float)):
                 self._attrs[key] = self._normalize(key, val)
 
         self.rebase()
 
 
@@ -80,104 +85,128 @@
         return str(self._attrs)
 
 
     def __repr__(self):
         return "Metadata({})".format(self._attrs)
 
 
-    def rebase(self):
+    def rebase(self) -> None:
+        """Updates the basis of the metadata attributes."""
         self._basis = copy.deepcopy(self._attrs)
 
 
     @property
     def is_modified(self) -> bool:
         """Checks if metadata is modified.
 
         Returns:
             True is metadata is modified, False otherwise.
         """
         return self._attrs != self._basis
 
 
     @classmethod
-    def normalize(cls, name: str, val) -> Any:
+    def normalize_value(cls, key: str, val) -> Any:
         """Normalizes metadata attribute value.
 
+        Supported attributes:
+            - doi
+            - keywords
+            - authors
+
         Args:
-            name: Attribute name.
+            key (str): Attribute key.
             val: Attribute value.
 
         Returns:
             Normalized attribute value.
 
         Raises:
             ValueError: If invalid attribute value.
         """
         # Digital Object Identifier
-        if name == "doi":
+        if key == "doi":
             if isinstance(val, str):
                 val = val.lower()
                 if val.startswith("doi:"):
                     val = val[4:]
                 elif val.startswith("http://doi.org/"):
                     val = val[15:]
                 elif val.startswith("https://doi.org/"):
                     val = val[16:]
-                if not re.match(Metadata.REGEXP_DOI, val):
+                if not re.fullmatch(Metadata.REGEXP_DOI, val):
                     raise ValueError
             else:
                 raise ValueError
 
         # Keywords
-        elif name == "keywords":
+        elif key == "keywords":
             if isinstance(val, str):
                 val = re.split(r"[,;\n]", val)
             try:
                 val = [keyword.strip() for keyword in iter(val)]
             except TypeError:
                 raise ValueError
 
         # Authors
-        elif name == "authors":
+        elif key == "authors":
             val = Person.get_persons(val)
 
         # Return normalized value
         return val
 
 
-    def serialize(self) -> Dict:
-        """Serializes metadata as a dictionary.
+    @classmethod
+    def serialize_value(cls, key: str, val) -> Any:
+        """Serializes metadata attribute value.
+
+        Supported attributes:
+            - Any attribute with a data type of `Person`.
+            - Any attribute with a data type of `PersonList`.
+
+        Args:
+            key (str): Attribute key.
+            val: Attribute value.
 
         Returns:
-            Metadata dictionary.
+            Serialized attribute value.
         """
-        out = self._attrs.copy()
+        if isinstance(val, Person):
+            return val.serialize()
 
-        for key, val in out.items():
+        if isinstance(val, PersonList):
+            return [person.serialize() for person in val]
 
-            if isinstance(val, Person):
-                val = val.serialize()
+        return copy.deepcopy(val)
 
-            elif isinstance(val, PersonList):
-                val = [person.serialize() for person in val]
 
-            else:
-                continue
+    def serialize(self) -> Dict:
+        """Serializes metadata as a dictionary.
+
+        Returns:
+            Metadata dictionary.
+        """
+        out = {}
 
-            out[key] = val
+        for key, val in self._attrs.items():
+            out[key] = self._serialize(key, val)
 
         return out
 
 
     def autocomplete(self, overwrite: bool=False, attrs: List=None, **kwargs) -> Dict:
         """Completes missing metadata attributes by using the available information.
 
+        Supported attributes:
+            - Any attribute with a data type of `Person`.
+            - Any attribute with a data type of `PersonList`.
+
         Args:
-            overwrite: Set True to overwrite existing attributes.
-            attrs: List of attributes to be completed.
+            overwrite (bool): Set True to overwrite existing attributes (default False).
+            attrs (List): List of attributes to be completed (optional).
             **kwargs: Arguments for the specific autocomplete methods.
 
         Returns:
             A dictionary of attributes set by method.
         """
         updated = {}
 
@@ -201,38 +230,45 @@
 
             if result:
                 updated[key] = result
 
         return updated
 
 
-    def _remove_comments(self, d):
-        """Removes comments from a YAML dictionary recursively."""
+    def _remove_comments(self, var) -> None:
+        """Removes comments from a YAML dictionary recursively.
 
-        # REMARK: https://stackoverflow.com/questions/60080325/how-to-delete-all-comments-in-ruamel-yaml
-        if isinstance(d, dict):
-            for k, v in d.items():
-                self._remove_comments(k)
-                self._remove_comments(v)
-
-        elif isinstance(d, list):
-            for elem in d:
-                self._remove_comments(elem)
+        Args:
+            var: YAML dictionary or a dictionary item, if called recursively.
+        """
+        # REMARK: Based on https://stackoverflow.com/questions/60080325/how-to-delete-all-comments-in-ruamel-yaml
+        if isinstance(var, dict):
+            for key, val in var.items():
+                self._remove_comments(key)
+                self._remove_comments(val)
+
+        elif isinstance(var, list):
+            for item in var:
+                self._remove_comments(item)
 
         try:
-             # literal scalarstring might have comment associated with them
-             attr = 'comment' if isinstance(d, ruamel.yaml.scalarstring.ScalarString) \
-                      else ruamel.yaml.comments.Comment.attrib
-             delattr(d, attr)
+             if isinstance(var, ruamel.yaml.scalarstring.ScalarString):
+                attr = "comment"
+             else:
+                attr = ruamel.yaml.comments.Comment.attrib
+             delattr(var, attr)
+
         except AttributeError:
             pass
 
 
-    def print(self):
-        """Pretty prints metadata."""
+    def print(self) -> None:
+        """Pretty prints metadata.
 
+        Serializes metadata and prints as YAML without comments.
+        """
         yaml = ruamel.yaml.YAML()
 
         out = self.serialize()
         self._remove_comments(out)
 
-        yaml.dump(out, sys.stdout)
+        yaml.dump(out, sys.stdout)
```

### Comparing `fairly-0.4.1/src/fairly/person.py` & `fairly-1.0.0/src/fairly/person.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     Class Attributes:
         REGEXP_ORCID_ID: Regular expression to validate ORCID identifier.
         REGEXP_EMAIL: Regular expression to validate e-mail address.
     """
 
     # TODO: Check the checksum digit
     # https://support.orcid.org/hc/en-us/articles/360006897674-Structure-of-the-ORCID-Identifier
-    REGEXP_ORCID_ID = re.compile(r"^(\d{4}-){3}\d{3}(\d|X)$")
-    REGEXP_EMAIL = re.compile(r"^[\w\.+-]+@([\w-]+\.)+[\w-]{2,}$")
+    REGEXP_ORCID_ID = re.compile(r"(\d{4}-){3}\d{3}(\d|X)")
+    REGEXP_EMAIL = re.compile(r"[\w\.+-]+@([\w-]+\.)+[\w-]{2,}")
 
 
     def __init__(self, person: str=None, **kwargs):
         """Initializes Person object.
 
         Full name is obtained from name and surname, if required.
 
@@ -114,18 +114,18 @@
             person: Person identifier (e.g. fullname)
 
         Returns:
             Dictionary of person attributes.
         """
         person = person.strip()
 
-        if re.match(Person.REGEXP_ORCID_ID, person):
+        if re.fullmatch(Person.REGEXP_ORCID_ID, person):
             return {"orcid_id": person}
 
-        if re.match(Person.REGEXP_EMAIL, person):
+        if re.fullmatch(Person.REGEXP_EMAIL, person):
             return {"email": person}
 
         attrs = {"fullname": person}
         parts = [part.strip() for part in person.split(",")]
         if len(parts) == 2:
             attrs["surname"], attrs["name"] = parts
 
@@ -170,14 +170,15 @@
             "https://orcid.org/oauth/token",
             data=f"client_id={client_id}&client_secret={client_secret}&grant_type=client_credentials&scope=/read-public",
             headers={
                 "Accept": "application/json",
                 "Content-Type": "application/x-www-form-urlencoded",
             }
         )
+        response.raise_for_status()
 
         json = response.json()
 
         if "access_token" not in json:
             raise ValueError("Invalid response")
 
         return json["access_token"]
@@ -191,15 +192,15 @@
         also not available, it is retrieved by using `get_orcid_token()` method.
 
         Args:
             orcid_id: ORCID identifier.
             token: ORCID access token.
 
         Returns:
-            Person object if valid ORCID identifier, otherwise None.
+            Person object if valid ORCID identifier, None otherwise.
 
         Raises:
             ValueError("No access token"): If access token is not available.
             ValueError("Invalid ORCID identifier"): If ORCID identified is not valid.
         """
         # Get default access token if required
         if not token:
@@ -216,14 +217,15 @@
         response = requests.get(
             f"https://pub.orcid.org/v3.0/expanded-search/?q=orcid:{orcid_id}&fl={fields}",
             headers={
                 "Content-type": "application/vnd.orcid+json",
                 "Authorization type and Access token": f"Bearer {token}"
             }
         )
+        response.raise_for_status()
         results = response.json().get("expanded-result")
 
         # Raise exception if no results
         if not results:
             raise ValueError("Invalid ORCID Id")
 
         # Return the first person matching the ORCID identifier
```

### Comparing `fairly-0.4.1/tests/test_cli.py` & `fairly-1.0.0/tests/test_cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,14 +51,14 @@
         pytest.skip("No access token")
 
     create_dummy_dataset(tmpdir)
 
     result = runner.invoke(app, ["dataset", "upload", str(tmpdir), repository_id])
     assert result.exit_code == 0, result.stdout
 
-    match = re.search(r"(https?://[^\s]+)", result.stdout)
+    match = re.search(r"uploaded at (.+)", result.stdout)
     assert match
 
-    url = match[0]
+    id = match[1]
 
-    result = runner.invoke(app, ["dataset", "delete", url])
+    result = runner.invoke(app, ["dataset", "delete", "--repo", repository_id, id])
     assert result.exit_code == 0, result.stdout
```

### Comparing `fairly-0.4.1/tests/test_fairly.py` & `fairly-1.0.0/tests/test_fairly.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 
 import fairly
 
 from fairly.dataset.local import LocalDataset
 from fairly.dataset.remote import RemoteDataset
 
 from fairly.client.figshare import FigshareClient
-from fairly.client.zenodo import ZenodoClient
+from fairly.client.invenio import InvenioClient
 
 # Set testing flag
 fairly.TESTING = True
 
 
 def params_create_client():
     return [
         ("figshare", FigshareClient),
-        ("zenodo", ZenodoClient)
+        ("invenio", InvenioClient)
     ]
 
 
 def test_load_config():
     config = fairly.get_config("zenodo")
     assert config is not None
     assert config["url"] == "https://zenodo.org/"
 
 
 def test_get_clients():
     clients = fairly.get_clients()
     assert clients
     assert "fairly" not in clients
     assert "figshare" in clients
-    assert "zenodo" in clients
+    assert "invenio" in clients
     assert "djehuty" in clients
 
 
 @pytest.mark.parametrize("client_id, client_class", params_create_client())
 def test_create_client(client_id, client_class):
     """Test client creation."""
     client = fairly.client(client_id)
@@ -44,36 +44,14 @@
 
 
 @pytest.mark.parametrize("repository_id", fairly.get_repositories())
 def test_dataset_upload_delete(repository_id, tmpdir):
     '''Test dataset upload to the recognized repositories.'''
 
     repository = fairly.get_repository(repository_id)
-    if not repository.get("token"):
-        pytest.skip("No access token")
-
-    create_dummy_dataset(tmpdir)
-
-    result = runner.invoke(app, ["dataset", "upload", str(tmpdir), repository_id])
-    assert result.exit_code == 0, result.stdout
-
-    match = re.search(r"(https?://[^\s]+)", result.stdout)
-    assert match
-
-    url = match[0]
-
-    result = runner.invoke(app, ["dataset", "delete", url])
-    assert result.exit_code == 0, result.stdout
-
-
-@pytest.mark.parametrize("repository_id", fairly.get_repositories())
-def test_dataset_upload_delete(repository_id, tmpdir):
-    '''Test dataset upload to the recognized repositories.'''
-
-    repository = fairly.get_repository(repository_id)
     if not repository.get("token"):
         pytest.skip("No access token")
 
     create_dummy_dataset(tmpdir)
 
     local_dataset = fairly.dataset(str(tmpdir))
     assert isinstance(local_dataset, LocalDataset)
```

