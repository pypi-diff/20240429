# Comparing `tmp/adafruit-circuitpython-itertools-2.1.0.tar.gz` & `tmp/adafruit_circuitpython_itertools-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-itertools-2.1.0.tar", last modified: Fri Feb 23 20:37:19 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_itertools-2.1.1.tar", last modified: Mon Apr 29 15:51:29 2024, max compression
```

## Comparing `adafruit-circuitpython-itertools-2.1.0.tar` & `adafruit_circuitpython_itertools-2.1.1.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:37:19.709683 adafruit-circuitpython-itertools-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:37:19.697683 adafruit-circuitpython-itertools-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:37:19.701683 adafruit-circuitpython-itertools-2.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:37:19.701683 adafruit-circuitpython-itertools-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:37:19.701683 adafruit-circuitpython-itertools-2.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/LICENSES/PSF-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-02-23 20:37:19.705683 adafruit-circuitpython-itertools-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:37:19.705683 adafruit-circuitpython-itertools-2.1.0/adafruit_circuitpython_itertools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-02-23 20:37:19.000000 adafruit-circuitpython-itertools-2.1.0/adafruit_circuitpython_itertools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-23 20:37:19.000000 adafruit-circuitpython-itertools-2.1.0/adafruit_circuitpython_itertools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 20:37:19.000000 adafruit-circuitpython-itertools-2.1.0/adafruit_circuitpython_itertools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-23 20:37:19.000000 adafruit-circuitpython-itertools-2.1.0/adafruit_circuitpython_itertools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-23 20:37:19.000000 adafruit-circuitpython-itertools-2.1.0/adafruit_circuitpython_itertools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:37:19.705683 adafruit-circuitpython-itertools-2.1.0/adafruit_itertools/
--rw-r--r--   0 runner    (1001) docker     (127)    18457 2024-02-23 20:37:13.000000 adafruit-circuitpython-itertools-2.1.0/adafruit_itertools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-02-23 20:37:13.000000 adafruit-circuitpython-itertools-2.1.0/adafruit_itertools/adafruit_itertools_extras.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:37:19.705683 adafruit-circuitpython-itertools-2.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:37:19.705683 adafruit-circuitpython-itertools-2.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:37:19.705683 adafruit-circuitpython-itertools-2.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-23 20:37:13.000000 adafruit-circuitpython-itertools-2.1.0/examples/itertools_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-02-23 20:37:13.000000 adafruit-circuitpython-itertools-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 20:37:19.709683 adafruit-circuitpython-itertools-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:37:19.705683 adafruit-circuitpython-itertools-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-02-23 20:37:07.000000 adafruit-circuitpython-itertools-2.1.0/tests/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-02-23 20:37:13.000000 adafruit-circuitpython-itertools-2.1.0/tests/test_itertools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:51:29.485899 adafruit_circuitpython_itertools-2.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:51:29.477899 adafruit_circuitpython_itertools-2.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:51:29.477899 adafruit_circuitpython_itertools-2.1.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:51:29.477899 adafruit_circuitpython_itertools-2.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:51:29.481899 adafruit_circuitpython_itertools-2.1.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/LICENSES/PSF-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-29 15:51:29.481899 adafruit_circuitpython_itertools-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:51:29.481899 adafruit_circuitpython_itertools-2.1.1/adafruit_circuitpython_itertools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-29 15:51:29.000000 adafruit_circuitpython_itertools-2.1.1/adafruit_circuitpython_itertools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-29 15:51:29.000000 adafruit_circuitpython_itertools-2.1.1/adafruit_circuitpython_itertools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:51:29.000000 adafruit_circuitpython_itertools-2.1.1/adafruit_circuitpython_itertools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 15:51:29.000000 adafruit_circuitpython_itertools-2.1.1/adafruit_circuitpython_itertools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 15:51:29.000000 adafruit_circuitpython_itertools-2.1.1/adafruit_circuitpython_itertools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:51:29.481899 adafruit_circuitpython_itertools-2.1.1/adafruit_itertools/
+-rw-r--r--   0 runner    (1001) docker     (127)    19061 2024-04-29 15:51:26.000000 adafruit_circuitpython_itertools-2.1.1/adafruit_itertools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-04-29 15:51:26.000000 adafruit_circuitpython_itertools-2.1.1/adafruit_itertools/adafruit_itertools_extras.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:51:29.481899 adafruit_circuitpython_itertools-2.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:51:29.481899 adafruit_circuitpython_itertools-2.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:51:29.481899 adafruit_circuitpython_itertools-2.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-29 15:51:26.000000 adafruit_circuitpython_itertools-2.1.1/examples/itertools_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-29 15:51:26.000000 adafruit_circuitpython_itertools-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:51:29.485899 adafruit_circuitpython_itertools-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:51:29.481899 adafruit_circuitpython_itertools-2.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-29 15:51:21.000000 adafruit_circuitpython_itertools-2.1.1/tests/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12603 2024-04-29 15:51:26.000000 adafruit_circuitpython_itertools-2.1.1/tests/test_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-04-29 15:51:26.000000 adafruit_circuitpython_itertools-2.1.1/tests/test_itertools_extras.py
```

### Comparing `adafruit-circuitpython-itertools-2.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_itertools-2.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.1.0/.gitignore` & `adafruit_circuitpython_itertools-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.1.0/.pre-commit-config.yaml` & `adafruit_circuitpython_itertools-2.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.1.0/.pylintrc` & `adafruit_circuitpython_itertools-2.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.1.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_itertools-2.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.1.0/LICENSE` & `adafruit_circuitpython_itertools-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.1.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_itertools-2.1.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.1.0/LICENSES/MIT.txt` & `adafruit_circuitpython_itertools-2.1.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.1.0/LICENSES/PSF-2.0.txt` & `adafruit_circuitpython_itertools-2.1.1/LICENSES/PSF-2.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.1.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_itertools-2.1.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.1.0/PKG-INFO` & `adafruit_circuitpython_itertools-2.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-itertools
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python's itertools for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IterTools
 Keywords: adafruit,itertools,cpython,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -12,14 +12,15 @@
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Adafruit-Blinka
 Provides-Extra: optional
+Requires-Dist: more-itertools; extra == "optional"
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-itertools/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/itertools/en/latest/
     :alt: Documentation Status
```

### Comparing `adafruit-circuitpython-itertools-2.1.0/README.rst` & `adafruit_circuitpython_itertools-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.1.0/adafruit_circuitpython_itertools.egg-info/PKG-INFO` & `adafruit_circuitpython_itertools-2.1.1/adafruit_circuitpython_itertools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-itertools
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python's itertools for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IterTools
 Keywords: adafruit,itertools,cpython,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -12,14 +12,15 @@
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Adafruit-Blinka
 Provides-Extra: optional
+Requires-Dist: more-itertools; extra == "optional"
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-itertools/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/itertools/en/latest/
     :alt: Documentation Status
```

### Comparing `adafruit-circuitpython-itertools-2.1.0/adafruit_circuitpython_itertools.egg-info/SOURCES.txt` & `adafruit_circuitpython_itertools-2.1.1/adafruit_circuitpython_itertools.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -33,8 +33,9 @@
 docs/index.rst
 docs/index.rst.license
 docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/itertools_simpletest.py
 tests/README.rst
-tests/test_itertools.py
+tests/test_itertools.py
+tests/test_itertools_extras.py
```

### Comparing `adafruit-circuitpython-itertools-2.1.0/adafruit_itertools/__init__.py` & `adafruit_circuitpython_itertools-2.1.1/adafruit_itertools/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 """
 # pylint:disable=invalid-name,redefined-builtin,attribute-defined-outside-init
 # pylint:disable=stop-iteration-return,anomalous-backslash-in-string
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Itertools.git"
 
 try:
     from typing import (
         Any,
         Callable,
         Iterable,
@@ -49,15 +49,18 @@
     _N: TypeAlias = Union[int, float, complex]
     _Predicate: TypeAlias = Callable[[_T], object]
 
 except ImportError:
     pass
 
 
-def accumulate(iterable, func=lambda x, y: x + y):
+def accumulate(
+    iterable: Iterable[_T],
+    func: Callable[[_T, _T], _T] = lambda x, y: x + y,  # type: ignore[operator]
+) -> Iterator[_T]:
     """Make an iterator that returns accumulated sums, or accumulated
     results of other binary functions (specified via the optional func
     argument). If func is supplied, it should be a function of two
     arguments that returns a value. Elements of the input iterable may
     be any type that can be accepted as arguments to func.  (For
     example, with the default operation of addition, elements may be any
     addable type including Decimal or Fraction.) If the input iterable
@@ -196,24 +199,24 @@
 
     """
     while True:
         yield start
         start += step
 
 
-def cycle(p):
+def cycle(p: Iterable[_T]) -> Iterator[_T]:
     """Make an iterator returning elements from the iterable and saving a copy
     of each. When the iterable is exhausted, return elements from the saved
     copy. Repeats indefinitely.
 
     :param p: the iterable from which to yield elements
 
     """
     try:
-        len(p)
+        len(p)  # type: ignore[arg-type]
     except TypeError:
         # len() is not defined for this type. Assume it is
         # a finite iterable so we must cache the elements.
         cache = []
         for i in p:
             yield i
             cache.append(i)
@@ -238,15 +241,17 @@
         if not predicate(x):
             yield x
             break
     for x in iterable:
         yield x
 
 
-def filterfalse(predicate: _Predicate[_T], iterable: Iterable[_T]) -> Iterator[_T]:
+def filterfalse(
+    predicate: Optional[_Predicate[_T]], iterable: Iterable[_T]
+) -> Iterator[_T]:
     """Make an iterator that filters elements from iterable returning only those
     for which the predicate is False. If predicate is None, return the items
     that are false.
 
     :param predicate: used to test each value
     :param iterable: source of values
 
@@ -284,41 +289,52 @@
     :param key: the key computation function (default is None)
 
     """
 
     # [k for k, g in groupby('AAAABBBCCDAABBB')] --> A B C D A B
     # [list(g) for k, g in groupby('AAAABBBCCD')] --> AAAA BBB CC D
 
-    def __init__(self, iterable, key=None):
+    def __init__(
+        self,
+        iterable: Iterable[_T],
+        key: Optional[Callable[[_T], Any]] = None,
+    ):
         self.keyfunc = key if key is not None else lambda x: x
         self.it = iter(iterable)
-        self.tgtkey = self.currkey = self.currvalue = object()
+        # Sentinel values, not actually returned during iteration.
+        self.currvalue: _T = object()  # type: ignore[assignment]
+        self.tgtkey = self.currkey = self.currvalue
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Tuple[Any, Iterator[_T]]]:
         return self
 
-    def __next__(self):
+    def __next__(self) -> Tuple[Any, Iterator[_T]]:
         self.id = object()
         while self.currkey == self.tgtkey:
             self.currvalue = next(self.it)  # Exit on StopIteration
             self.currkey = self.keyfunc(self.currvalue)
         self.tgtkey = self.currkey
         return (self.currkey, self._grouper(self.tgtkey, self.id))
 
-    def _grouper(self, tgtkey, id):
+    def _grouper(self, tgtkey: Any, id: object) -> Iterator[_T]:
         while self.id is id and self.currkey == tgtkey:
             yield self.currvalue
             try:
                 self.currvalue = next(self.it)
             except StopIteration:
                 return
             self.currkey = self.keyfunc(self.currvalue)
 
 
-def islice(p, start, stop=(), step=1):
+def islice(
+    p: Iterable[_T],
+    start: int,
+    stop: Optional[int] = (),  # type: ignore[assignment]
+    step: int = 1,
+) -> Iterator[_T]:
     """Make an iterator that returns selected elements from the
     iterable. If start is non-zero and stop is unspecified, then the
     value for start is used as end, and start is taken to be 0. Thus the
     supplied value specifies how many elements are to be generated,
     starting the the first one.If stop is specified, then elements from
     iterable are skipped until start is reached. Afterward, elements are
     returned consecutively unless step is set higher than one which
@@ -416,15 +432,16 @@
                 indices[i], indices[-j] = indices[-j], indices[i]
                 yield tuple(pool[i] for i in indices[:r])
                 break
         else:
             return
 
 
-def product(*args: Iterable[_T], r: int = 1) -> Iterator[Tuple[_T, ...]]:
+# def product(*args: Iterable[_T], r: int = 1) -> Iterator[Tuple[_T, ...]]:
+def product(*args: Iterable[Any], r: int = 1) -> Iterator[Tuple[Any, ...]]:
     """Cartesian product of input iterables.
 
     Roughly equivalent to nested for-loops in a generator expression. For
     example, product(A, B) returns the same as ((x,y) for x in A for y in
     B).
 
     The nested loops cycle like an odometer with the rightmost element
@@ -440,15 +457,15 @@
     :param r: number of times to duplicate the (single) arg for taking a
               product with itself (default is 1)
 
     """
     # product('ABCD', 'xy') --> Ax Ay Bx By Cx Cy Dx Dy
     # product(range(2), repeat=3) --> 000 001 010 011 100 101 110 111
     pools = [tuple(pool) for pool in args] * r
-    result: List[List[_T]] = [[]]
+    result: List[List[Any]] = [[]]
     for pool in pools:
         result = [x + [y] for x in result for y in pool]
     for prod in result:
         yield tuple(prod)
 
 
 def repeat(el: _T, n: Optional[int] = None) -> Iterator[_T]:
@@ -509,26 +526,26 @@
     :param n: the number of iterators to make (default is 2)
 
     """
     return [iter(iterable) for _ in range(n)]
 
 
 def zip_longest(
-    *args: Iterable[_T], fillvalue: _OptionalFill = None
-) -> Iterator[Tuple[Union[_T, _OptionalFill], ...]]:
+    *args: Iterable[Any], fillvalue: _OptionalFill = None
+) -> Iterator[Tuple[Any, ...]]:
     """Make an iterator that aggregates elements from each of the
     iterables. If the iterables are of uneven length, missing values are
     filled-in with fillvalue. Iteration continues until the longest
     iterable is exhausted.
 
     :param args: the iterables to combine
     :param fillvalue: value to fill in those missing from shorter iterables
     """
     # zip_longest('ABCD', 'xy', fillvalue='-') --> Ax By C- D-
-    iterators: List[Iterator[Union[_T, _OptionalFill]]] = [iter(it) for it in args]
+    iterators: List[Iterator[Any]] = [iter(it) for it in args]
     num_active = len(iterators)
     if not num_active:
         return
     while True:
         values = []
         for i, it in enumerate(iterators):
             try:
```

### Comparing `adafruit-circuitpython-itertools-2.1.0/adafruit_itertools/adafruit_itertools_extras.py` & `adafruit_circuitpython_itertools-2.1.1/adafruit_itertools/adafruit_itertools_extras.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,45 +37,77 @@
   https://github.com/adafruit/circuitpython/releases
 """
 
 # pylint:disable=invalid-name,keyword-arg-before-vararg,relative-beyond-top-level
 
 import adafruit_itertools as it
 
-__version__ = "2.1.0"
+try:
+    from typing import (
+        Any,
+        Callable,
+        Iterable,
+        Iterator,
+        List,
+        Optional,
+        Tuple,
+        Type,
+        TypeVar,
+        Union,
+    )
+    from typing_extensions import TypeAlias
+
+    _T = TypeVar("_T")
+    _N: TypeAlias = Union[int, float, complex]
+    _Predicate: TypeAlias = Callable[[_T], bool]
+except ImportError:
+    pass
+
+
+__version__ = "2.1.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Itertools.git"
 
 
-def all_equal(iterable):
+def all_equal(iterable: Iterable[Any]) -> bool:
     """Returns True if all the elements are equal to each other.
 
     :param iterable: source of values
 
     """
     g = it.groupby(iterable)
-    next(g)  # should succeed, value isn't relevant
     try:
-        next(g)  # should fail: only 1 group
+        next(g)  # value isn't relevant
+    except StopIteration:
+        # Empty iterable, return True to match cpython behavior.
+        return True
+    try:
+        next(g)
+        # more than one group, so we have different elements.
         return False
     except StopIteration:
+        # Only one group - all elements must be equal.
         return True
 
 
-def dotproduct(vec1, vec2):
+def dotproduct(vec1: Iterable[_N], vec2: Iterable[_N]) -> _N:
     """Compute the dot product of two vectors.
 
     :param vec1: the first vector
     :param vec2: the second vector
 
     """
     # dotproduct([1, 2, 3], [1, 2, 3]) -> 14
     return sum(map(lambda x, y: x * y, vec1, vec2))
 
 
-def first_true(iterable, default=False, pred=None):
+def first_true(
+    iterable: Iterable[_T],
+    default: Union[bool, _T] = False,
+    pred: Optional[_Predicate[_T]] = None,
+) -> Union[bool, _T]:
     """Returns the first true value in the iterable.
 
     If no true value is found, returns *default*
 
     If *pred* is not None, returns the first item for which pred(item)
     is true.
 
@@ -90,39 +122,41 @@
     # first_true([a,b], x, f) --> a if f(a) else b if f(b) else x
     try:
         return next(filter(pred, iterable))
     except StopIteration:
         return default
 
 
-def flatten(iterable_of_iterables):
+def flatten(iterable_of_iterables: Iterable[Iterable[_T]]) -> Iterator[_T]:
     """Flatten one level of nesting.
 
     :param iterable_of_iterables: a sequence of iterables to flatten
 
     """
     # flatten(['ABC', 'DEF']) --> A B C D E F
     return it.chain_from_iterable(iterable_of_iterables)
 
 
-def grouper(iterable, n, fillvalue=None):
+def grouper(
+    iterable: Iterable[_T], n: int, fillvalue: Optional[_T] = None
+) -> Iterator[Tuple[_T, ...]]:
     """Collect data into fixed-length chunks or blocks.
 
     :param iterable: source of values
     :param n: chunk size
     :param fillvalue: value to use for filling out the final chunk.
                       Defaults to None.
 
     """
     # grouper('ABCDEFG', 3, 'x') --> ABC DEF Gxx
     args = [iter(iterable)] * n
     return it.zip_longest(*args, fillvalue=fillvalue)
 
 
-def iter_except(func, exception):
+def iter_except(func: Callable[[], _T], exception: Type[BaseException]) -> Iterator[_T]:
     """Call a function repeatedly, yielding the results, until exception is raised.
 
     Converts a call-until-exception interface to an iterator interface.
     Like builtins.iter(func, sentinel) but uses an exception instead
     of a sentinel to end the loop.
 
     Examples:
@@ -139,114 +173,122 @@
     try:
         while True:
             yield func()
     except exception:
         pass
 
 
-def ncycles(iterable, n):
+def ncycles(iterable: Iterable[_T], n: int) -> Iterator[_T]:
     """Returns the sequence elements a number of times.
 
     :param iterable: the source of values
     :param n: how many time to repeal the values
 
     """
     return it.chain_from_iterable(it.repeat(tuple(iterable), n))
 
 
-def nth(iterable, n, default=None):
+def nth(iterable: Iterable[_T], n: int, default: Optional[_T] = None) -> Optional[_T]:
     """Returns the nth item or a default value.
 
     :param iterable: the source of values
     :param n: the index of the item to fetch, starts at 0
 
     """
     try:
         return next(it.islice(iterable, n, n + 1))
     except StopIteration:
         return default
 
 
-def padnone(iterable):
+def padnone(iterable: Iterable[_T]) -> Iterator[Optional[_T]]:
     """Returns the sequence elements and then returns None indefinitely.
 
     Useful for emulating the behavior of the built-in map() function.
 
     :param iterable: the source of initial values
     """
     # take(5, padnone([1, 2, 3])) -> 1 2 3 None None
     return it.chain(iterable, it.repeat(None))
 
 
-def pairwise(iterable):
-    """Pair up valuesin the iterable.
+def pairwise(iterable: Iterable[_T]) -> Iterator[Tuple[_T, _T]]:
+    """Return successive overlapping pairs from the iterable.
+
+    The number of tuples from the output will be one fewer than the
+    number of values in the input. It will be empty if the input has
+    fewer than two values.
 
     :param iterable: source of values
 
     """
-    # pairwise(range(11)) -> (1, 2), (3, 4), (5, 6), (7, 8), (9, 10)
+    # pairwise(range(5)) -> (0, 1), (1, 2), (2, 3), (3, 4)
     a, b = it.tee(iterable)
     try:
         next(b)
     except StopIteration:
         pass
     return zip(a, b)
 
 
-def partition(pred, iterable):
+def partition(
+    pred: _Predicate[_T], iterable: Iterable[_T]
+) -> Tuple[Iterator[_T], Iterator[_T]]:
     """Use a predicate to partition entries into false entries and true entries.
 
     :param pred: the predicate that divides the values
     :param iterable: source of values
 
     """
     # partition(lambda x: x % 2, range(10)) --> 0 2 4 6 8   and  1 3 5 7 9
     t1, t2 = it.tee(iterable)
     return it.filterfalse(pred, t1), filter(pred, t2)
 
 
-def prepend(value, iterator):
+def prepend(value: _T, iterator: Iterable[_T]) -> Iterator[_T]:
     """Prepend a single value in front of an iterator
 
     :param value: the value to prepend
     :param iterator: the iterator to which to prepend
 
     """
     # prepend(1, [2, 3, 4]) -> 1 2 3 4
     return it.chain([value], iterator)
 
 
-def quantify(iterable, pred=bool):
+def quantify(iterable: Iterable[_T], pred: _Predicate[_T] = bool) -> int:
     """Count how many times the predicate is true.
 
     :param iterable: source of values
     :param pred: the predicate whose result is to be quantified when applied to
                  all values in iterable. Defaults to bool()
 
     """
     # quantify([2, 56, 3, 10, 85], lambda x: x >= 10) -> 3
     return sum(map(pred, iterable))
 
 
-def repeatfunc(func, times=None, *args):
+def repeatfunc(
+    func: Callable[..., _T], times: Optional[int] = None, *args: Any
+) -> Iterator[_T]:
     """Repeat calls to func with specified arguments.
 
     Example:  repeatfunc(random.random)
 
     :param func: the function to be called
     :param times: the number of times to call it: size of the resulting iterable
                   None means infinitely. Default is None.
 
     """
     if times is None:
         return it.starmap(func, it.repeat(args))
     return it.starmap(func, it.repeat(args, times))
 
 
-def roundrobin(*iterables):
+def roundrobin(*iterables: Iterable[_T]) -> Iterator[_T]:
     """Return an iterable created by repeatedly picking value from each
     argument in order.
 
     :param args: the iterables to pick from
 
     """
     # roundrobin('ABC', 'D', 'EF') --> A D E B F C
@@ -259,26 +301,27 @@
                 yield n()
         except StopIteration:
             # Remove the iterator we just exhausted from the cycle.
             num_active -= 1
             nexts = it.cycle(it.islice(nexts, num_active))
 
 
-def tabulate(function, start=0):
-    """Apply a function to a sequence of consecutive integers.
+def tabulate(function: Callable[[int], int], start: int = 0) -> Iterator[int]:
+    """Apply a function to a sequence of consecutive numbers.
 
-    :param function: the function of one integer argument
+    :param function: the function of one numeric argument.
     :param start: optional value to start at (default is 0)
 
     """
     # take(5, tabulate(lambda x: x * x))) -> 0 1 4 9 16
-    return map(function, it.count(start))
+    counter: Iterator[int] = it.count(start)  # type: ignore[assignment]
+    return map(function, counter)
 
 
-def tail(n, iterable):
+def tail(n: int, iterable: Iterable[_T]) -> Iterator[_T]:
     """Return an iterator over the last n items
 
     :param n: how many values to return
     :param iterable: the source of values
 
     """
     # tail(3, 'ABCDEFG') --> E F G
@@ -290,15 +333,15 @@
             if len(buf) > n:
                 buf.pop(0)
         except StopIteration:
             break
     return iter(buf)
 
 
-def take(n, iterable):
+def take(n: int, iterable: Iterable[_T]) -> List[_T]:
     """Return first n items of the iterable as a list
 
     :param n: how many values to take
     :param iterable: the source of values
 
     """
     # take(3, 'ABCDEF')) -> A B C
```

### Comparing `adafruit-circuitpython-itertools-2.1.0/docs/_static/favicon.ico` & `adafruit_circuitpython_itertools-2.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.1.0/docs/conf.py` & `adafruit_circuitpython_itertools-2.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.1.0/docs/index.rst` & `adafruit_circuitpython_itertools-2.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.1.0/examples/itertools_simpletest.py` & `adafruit_circuitpython_itertools-2.1.1/examples/itertools_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.1.0/pyproject.toml` & `adafruit_circuitpython_itertools-2.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-itertools"
 description = "Python's itertools for CircuitPython"
-version = "2.1.0"
+version = "2.1.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_IterTools"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-itertools-2.1.0/tests/README.rst` & `adafruit_circuitpython_itertools-2.1.1/tests/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,34 @@
 ..
 
 Itertools Tests
 ===============
 
 These tests run under CPython, and are intended to verify that the
 Adafruit library functions return the same outputs compared to ones in
-the standard `itertools` module.
+the standard `itertools` module, and also to exercise some type
+annotations.
 
 These tests run automatically from the standard `circuitpython github
 workflow <wf_>`_. To run them manually, first install these packages
 if necessary::
 
   $ pip3 install pytest
 
 Then ensure you're in the *root* directory of the repository and run
 the following command::
 
   $ python -m pytest
 
+Type annotation tests don't run automatically at this point. But to
+verify type-related issues manually, first install these packages if
+necessary::
+
+  $ pip3 install mypy
+
+Then ensure you're in the *root* directory of the repository and run
+the following command::
+
+  $ mypy --warn-unused-ignores --disallow-untyped-defs tests
+
+
 .. _wf: https://github.com/adafruit/workflows-circuitpython-libs/blob/6e1562eaabced4db1bd91173b698b1cc1dfd35ab/build/action.yml#L78-L84
```

