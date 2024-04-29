# Comparing `tmp/circuitpython_fake_bme280-1.0.2.tar.gz` & `tmp/circuitpython_fake_bme280-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython_fake_bme280-1.0.2.tar", last modified: Mon Apr 22 16:51:13 2024, max compression
+gzip compressed data, was "circuitpython_fake_bme280-1.0.3.tar", last modified: Mon Apr 29 18:53:20 2024, max compression
```

## Comparing `circuitpython_fake_bme280-1.0.2.tar` & `circuitpython_fake_bme280-1.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:51:13.830237 circuitpython_fake_bme280-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:51:13.822237 circuitpython_fake_bme280-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:51:13.826237 circuitpython_fake_bme280-1.0.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:51:13.826237 circuitpython_fake_bme280-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:51:13.826237 circuitpython_fake_bme280-1.0.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-22 16:51:13.830237 circuitpython_fake_bme280-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:51:13.830237 circuitpython_fake_bme280-1.0.2/circuitpython_fake_bme280.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-22 16:51:13.000000 circuitpython_fake_bme280-1.0.2/circuitpython_fake_bme280.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-22 16:51:13.000000 circuitpython_fake_bme280-1.0.2/circuitpython_fake_bme280.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 16:51:13.000000 circuitpython_fake_bme280-1.0.2/circuitpython_fake_bme280.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-22 16:51:13.000000 circuitpython_fake_bme280-1.0.2/circuitpython_fake_bme280.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-22 16:51:13.000000 circuitpython_fake_bme280-1.0.2/circuitpython_fake_bme280.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:51:13.830237 circuitpython_fake_bme280-1.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:51:13.830237 circuitpython_fake_bme280-1.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:51:13.830237 circuitpython_fake_bme280-1.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-22 16:51:11.000000 circuitpython_fake_bme280-1.0.2/examples/fake_bme280_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 16:51:13.830237 circuitpython_fake_bme280-1.0.2/fake_bme280/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 16:51:11.000000 circuitpython_fake_bme280-1.0.2/fake_bme280/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-04-22 16:51:11.000000 circuitpython_fake_bme280-1.0.2/fake_bme280/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-22 16:51:11.000000 circuitpython_fake_bme280-1.0.2/fake_bme280/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-22 16:51:11.000000 circuitpython_fake_bme280-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-22 16:51:05.000000 circuitpython_fake_bme280-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 16:51:13.830237 circuitpython_fake_bme280-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:53:20.862377 circuitpython_fake_bme280-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:53:20.854377 circuitpython_fake_bme280-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:53:20.858377 circuitpython_fake_bme280-1.0.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:53:20.858377 circuitpython_fake_bme280-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:53:20.858377 circuitpython_fake_bme280-1.0.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-29 18:53:20.862377 circuitpython_fake_bme280-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:53:20.862377 circuitpython_fake_bme280-1.0.3/circuitpython_fake_bme280.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-29 18:53:20.000000 circuitpython_fake_bme280-1.0.3/circuitpython_fake_bme280.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-29 18:53:20.000000 circuitpython_fake_bme280-1.0.3/circuitpython_fake_bme280.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:53:20.000000 circuitpython_fake_bme280-1.0.3/circuitpython_fake_bme280.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-29 18:53:20.000000 circuitpython_fake_bme280-1.0.3/circuitpython_fake_bme280.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 18:53:20.000000 circuitpython_fake_bme280-1.0.3/circuitpython_fake_bme280.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:53:20.862377 circuitpython_fake_bme280-1.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:53:20.862377 circuitpython_fake_bme280-1.0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:53:20.862377 circuitpython_fake_bme280-1.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-29 18:53:18.000000 circuitpython_fake_bme280-1.0.3/examples/fake_bme280_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:53:20.862377 circuitpython_fake_bme280-1.0.3/fake_bme280/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:53:18.000000 circuitpython_fake_bme280-1.0.3/fake_bme280/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9578 2024-04-29 18:53:18.000000 circuitpython_fake_bme280-1.0.3/fake_bme280/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-29 18:53:18.000000 circuitpython_fake_bme280-1.0.3/fake_bme280/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-29 18:53:18.000000 circuitpython_fake_bme280-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-29 18:53:11.000000 circuitpython_fake_bme280-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 18:53:20.862377 circuitpython_fake_bme280-1.0.3/setup.cfg
```

### Comparing `circuitpython_fake_bme280-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `circuitpython_fake_bme280-1.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/.github/workflows/release_gh.yml` & `circuitpython_fake_bme280-1.0.3/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/.gitignore` & `circuitpython_fake_bme280-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/.pre-commit-config.yaml` & `circuitpython_fake_bme280-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/.pylintrc` & `circuitpython_fake_bme280-1.0.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/LICENSE` & `circuitpython_fake_bme280-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/LICENSES/CC-BY-4.0.txt` & `circuitpython_fake_bme280-1.0.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/LICENSES/MIT.txt` & `circuitpython_fake_bme280-1.0.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/LICENSES/Unlicense.txt` & `circuitpython_fake_bme280-1.0.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/PKG-INFO` & `circuitpython_fake_bme280-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-fake-bme280
-Version: 1.0.2
+Version: 1.0.3
 Summary: BME280 Driver for CircuitPython used for testing functionality with no hardware attached
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/brentru/CircuitPython_Fake_BME280
 Keywords: adafruit,blinka,circuitpython,micropython,fake_bme280,bme280,,test,,fake,,mock,,stub
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Adafruit-Blinka
 Requires-Dist: adafruit-circuitpython-busdevice
 Requires-Dist: adafruit-circuitpython-register
+Requires-Dist: toml
 Provides-Extra: optional
 
 Introduction
 ============
```

### Comparing `circuitpython_fake_bme280-1.0.2/README.rst` & `circuitpython_fake_bme280-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/circuitpython_fake_bme280.egg-info/PKG-INFO` & `circuitpython_fake_bme280-1.0.3/circuitpython_fake_bme280.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-fake-bme280
-Version: 1.0.2
+Version: 1.0.3
 Summary: BME280 Driver for CircuitPython used for testing functionality with no hardware attached
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/brentru/CircuitPython_Fake_BME280
 Keywords: adafruit,blinka,circuitpython,micropython,fake_bme280,bme280,,test,,fake,,mock,,stub
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: Adafruit-Blinka
 Requires-Dist: adafruit-circuitpython-busdevice
 Requires-Dist: adafruit-circuitpython-register
+Requires-Dist: toml
 Provides-Extra: optional
 
 Introduction
 ============
```

### Comparing `circuitpython_fake_bme280-1.0.2/circuitpython_fake_bme280.egg-info/SOURCES.txt` & `circuitpython_fake_bme280-1.0.3/circuitpython_fake_bme280.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/docs/_static/favicon.ico` & `circuitpython_fake_bme280-1.0.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/docs/conf.py` & `circuitpython_fake_bme280-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/docs/index.rst` & `circuitpython_fake_bme280-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/examples/fake_bme280_simpletest.py` & `circuitpython_fake_bme280-1.0.3/examples/fake_bme280_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/fake_bme280/basic.py` & `circuitpython_fake_bme280-1.0.3/fake_bme280/basic.py`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/fake_bme280/protocol.py` & `circuitpython_fake_bme280-1.0.3/fake_bme280/protocol.py`

 * *Files identical despite different names*

### Comparing `circuitpython_fake_bme280-1.0.2/pyproject.toml` & `circuitpython_fake_bme280-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-fake-bme280"
 description = "BME280 Driver for CircuitPython used for testing functionality with no hardware attached"
-version = "1.0.2"
+version = "1.0.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/brentru/CircuitPython_Fake_BME280"}
 keywords = [
     "adafruit",
```

