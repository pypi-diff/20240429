# Comparing `tmp/drf_spectacular_websocket-1.2.5.tar.gz` & `tmp/drf_spectacular_websocket-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_spectacular_websocket-1.2.5.tar", last modified: Sat Apr 27 10:49:23 2024, max compression
+gzip compressed data, was "drf_spectacular_websocket-1.2.6.tar", last modified: Mon Apr 29 10:34:45 2024, max compression
```

## Comparing `drf_spectacular_websocket-1.2.5.tar` & `drf_spectacular_websocket-1.2.6.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:49:23.962387 drf_spectacular_websocket-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:49:23.958387 drf_spectacular_websocket-1.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:49:23.958387 drf_spectacular_websocket-1.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-27 10:49:23.962387 drf_spectacular_websocket-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:49:23.958387 drf_spectacular_websocket-1.2.5/images/
--rw-r--r--   0 runner    (1001) docker     (127)    66494 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/images/example_receive.png
--rw-r--r--   0 runner    (1001) docker     (127)    89056 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/images/example_send.png
--rw-r--r--   0 runner    (1001) docker     (127)    11660 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 10:49:23.962387 drf_spectacular_websocket-1.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:49:23.958387 drf_spectacular_websocket-1.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:49:23.958387 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:49:23.962387 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5928 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/schemas/consumer_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/schemas/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:49:23.958387 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:49:23.962387 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/templates/drf_spectacular/
--rw-r--r--   0 runner    (1001) docker     (127)    20795 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/templates/drf_spectacular/swagger_ui.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:49:23.962387 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6836 2024-04-27 10:49:23.000000 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-27 10:49:23.000000 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 10:49:23.000000 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-27 10:49:23.000000 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-27 10:49:23.000000 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-27 10:49:23.000000 drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 10:49:23.962387 drf_spectacular_websocket-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/tests/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/tests/consumers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/tests/expected_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/tests/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-27 10:49:20.000000 drf_spectacular_websocket-1.2.5/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.093299 drf_spectacular_websocket-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.081298 drf_spectacular_websocket-1.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.085298 drf_spectacular_websocket-1.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-04-29 10:34:45.093299 drf_spectacular_websocket-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9980 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.085298 drf_spectacular_websocket-1.2.6/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    66494 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/images/example_receive.png
+-rw-r--r--   0 runner    (1001) docker     (127)    89056 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/images/example_send.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12793 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:34:45.093299 drf_spectacular_websocket-1.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.081298 drf_spectacular_websocket-1.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.085298 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.089298 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/schemas/consumer_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/schemas/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.085298 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.089298 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/templates/drf_spectacular/
+-rw-r--r--   0 runner    (1001) docker     (127)    20795 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/templates/drf_spectacular/swagger_ui.js
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.089298 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-04-29 10:34:45.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-29 10:34:45.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:34:45.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-29 10:34:45.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-29 10:34:45.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 10:34:45.000000 drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.089298 drf_spectacular_websocket-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/consumers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:45.089298 drf_spectacular_websocket-1.2.6/tests/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/schemas/expected_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/schemas/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 10:34:41.000000 drf_spectacular_websocket-1.2.6/tests/urls.py
```

### Comparing `drf_spectacular_websocket-1.2.5/.editorconfig` & `drf_spectacular_websocket-1.2.6/.editorconfig`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.5/.github/workflows/publish-to-pypi.yml` & `drf_spectacular_websocket-1.2.6/.github/workflows/publish-to-pypi.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # For more information see: https://packaging.python.org/en/latest/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/
 
-name: Publish Python 🐍 distribution 📦 to PyPI and TestPyPI
+name: Publish Python 🐍 distribution 📦 to PyPI
 
 # Build on every branch push, tag push, and pull request change
 on:
   push:
     branches:
       - main
     tags:
@@ -49,17 +49,26 @@
       run: |
         python -m ruff check --fix
 
     - name: Run format
       run: |
         python -m ruff format
 
-    - name: Run pytest
+    - name: Run mypy
       run: |
-        python -m pytest
+        python -m mypy
+
+    - name: Run pytest with coverage
+      run: |
+        python -m pytest --cov
+
+    - name: Upload coverage reports to Codecov
+      uses: codecov/codecov-action@v4.0.1
+      with:
+        token: ${{ secrets.CODECOV_TOKEN }}
 
   build:
     name: Build distribution 📦
     needs:
       - test
     runs-on: ubuntu-latest
 
@@ -111,34 +120,34 @@
       with:
         name: python-package-distributions
         path: dist/
 
     - name: Publish distribution 📦 to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
 
-  publish-to-testpypi:
-    name: Publish Python 🐍 distribution 📦 to TestPyPI
-
-    if: github.repository_owner == 'Friskes' && github.event_name == 'push'
-
-    needs:
-    - build
-    runs-on: ubuntu-latest
-
-    environment:
-      name: testpypi
-      url: https://test.pypi.org/p/drf-spectacular-websocket
-
-    permissions:
-      id-token: write
+  # publish-to-testpypi:
+  #   name: Publish Python 🐍 distribution 📦 to TestPyPI
 
-    steps:
-    - name: Download all the dists
-      uses: actions/download-artifact@v4
-      with:
-        name: python-package-distributions
-        path: dist/
+  #   if: github.repository_owner == 'Friskes' && github.event_name == 'push'
 
-    - name: Publish distribution 📦 to TestPyPI
-      uses: pypa/gh-action-pypi-publish@release/v1
-      with:
-        repository-url: https://test.pypi.org/legacy/
+  #   needs:
+  #   - build
+  #   runs-on: ubuntu-latest
+
+  #   environment:
+  #     name: testpypi
+  #     url: https://test.pypi.org/p/drf-spectacular-websocket
+
+  #   permissions:
+  #     id-token: write
+
+  #   steps:
+  #   - name: Download all the dists
+  #     uses: actions/download-artifact@v4
+  #     with:
+  #       name: python-package-distributions
+  #       path: dist/
+
+  #   - name: Publish distribution 📦 to TestPyPI
+  #     uses: pypa/gh-action-pypi-publish@release/v1
+  #     with:
+  #       repository-url: https://test.pypi.org/legacy/
```

### Comparing `drf_spectacular_websocket-1.2.5/.pre-commit-config.yaml` & `drf_spectacular_websocket-1.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.5/LICENSE` & `drf_spectacular_websocket-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.5/images/example_receive.png` & `drf_spectacular_websocket-1.2.6/images/example_receive.png`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.5/images/example_send.png` & `drf_spectacular_websocket-1.2.6/images/example_send.png`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.5/pyproject.toml` & `drf_spectacular_websocket-1.2.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -42,25 +42,29 @@
 # pip install .[dev]
 # pip install .[ci]
 [project.optional-dependencies]
 dev = [
     "pre-commit>=3.5.0",
     "ruff==0.4.1",
     "pytest>=7.0.1",
+    "mypy>=1.10.0",
+    "pytest-cov>=5.0.0",
 ]
 ci = [
     "ruff==0.4.1",
     "pytest>=7.0.1",
+    "mypy>=1.10.0",
+    "pytest-cov>=5.0.0",
 ]
 
 
 [project.urls]
-"Homepage" = "https://github.com/Friskes/drf-spectacular-websocket"
+"Repository" = "https://github.com/Friskes/drf-spectacular-websocket"
+"Changelog" = "https://github.com/Friskes/drf-spectacular-websocket/releases/"
 "Bug Reports" = "https://github.com/Friskes/drf-spectacular-websocket/issues"
-"Source" = "https://github.com/Friskes/drf-spectacular-websocket/"
 
 
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=8"]
 build-backend = "setuptools.build_meta"
 
 
@@ -90,14 +94,40 @@
 xfail_strict = true
 filterwarnings = [
     "error",
     "ignore::DeprecationWarning:typer",
 ]
 
 
+[tool.mypy]
+# for ignore rules:  # type: ignore[error_code]
+packages = ["src.drf_spectacular_websocket", "tests"]
+python_version = "3.9"
+strict = true  # строгая проверка типов
+ignore_missing_imports = true  # [import-untyped]
+# Проверять тело функции без типизации аргументов
+check_untyped_defs = true  # [annotation-unchecked]
+# Не ругаться на нетипизированный родительский класс
+disallow_subclassing_any = false  # [misc]
+# Не ругаться на вызов нетипизированной функции
+disallow_untyped_calls = false  # [no-untyped-call]
+# Не ругаться на return -> Any
+warn_return_any = false  # [no-any-return]
+
+
+[tool.coverage.run]
+concurrency = ["multiprocessing", "thread"]
+omit = ["*/tests/*"]
+parallel = true
+source = ["src.drf_spectacular_websocket"]
+
+[tool.coverage.report]
+fail_under = 80  # Тест упадёт если покрытие составит менее 80%
+
+
 # https://docs.astral.sh/ruff/settings/
 # https://docs.astral.sh/ruff/configuration/#full-command-line-interface
 # cmd: ruff format  # Отформатирует все файлы в `.` текущем каталоге.
 [tool.ruff]
 required-version = "==0.4.1"
 target-version = "py312"  # Версия python которую будет обслуживать ruff
 line-length = 105  # Макс длина строки кода после которой будет выполнен автоперенос
```

### Comparing `drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/schemas/consumer_schema.py` & `drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/schemas/consumer_schema.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,82 @@
 from __future__ import annotations
 
+from typing import TYPE_CHECKING, Any
+
 from drf_spectacular.openapi import AutoSchema
 from drf_spectacular.plumbing import (
     build_media_type_object,
     force_instance,
     is_list_serializer,
     is_serializer,
 )
 from inflection import camelize
-from rest_framework import serializers, status
+from rest_framework import status
 from rest_framework.parsers import JSONParser
 from rest_framework.renderers import JSONRenderer
+from rest_framework.serializers import CharField, Serializer
+
+if TYPE_CHECKING:
+    from drf_spectacular.utils import Direction, _SchemaType
 
+    from drf_spectacular_websocket.types import _Type
 
-class EmptySerializer(serializers.Serializer):
+
+class EmptySerializer(Serializer):
     pass
 
 
 class NotReadyError(Exception):
     pass
 
 
 class EventHandler:
     request = None
-    kwargs = {}
+    kwargs: dict[str, Any] = {}
     versioning_class = None
 
-    def __init__(self, name):
+    def __init__(self, name: str) -> None:
         self.name = name
 
-    def get_parsers(self):
+    def get_parsers(self) -> list[JSONParser]:
         return [JSONParser]
 
-    def get_renderers(self):
+    def get_renderers(self) -> list[JSONRenderer]:
         return [JSONRenderer]
 
-    def determine_version(self, *args, **kwargs):
+    def determine_version(self, *args: Any, **kwargs: Any) -> tuple[None, None]:
         return None, None
 
 
 class ConsumerAutoSchema(AutoSchema):
     """"""
 
-    def __init__(self):
+    method: _Type
+    method_name: str
+    event: str
+    include_event: bool
+
+    def __init__(self) -> None:
         super().__init__()
-        self.method_name: str | None = None
-        self.event: str | None = None
-        self.prepared = {'request': {}, 'response': {}}
+        self.prepared: dict[str, dict[str, Serializer]] = {'request': {}, 'response': {}}
 
     @property
-    def view(self):
+    def view(self) -> EventHandler:
         return EventHandler(name=self.event)
 
-    def get_operation_id(self):
+    def get_operation_id(self) -> str:
         return '%s_%s' % (self.method, self.method_name)
 
-    def get_request_body(self, serializer, method):
+    def get_request_body(self, serializer: Serializer) -> dict[str, dict[str, _SchemaType]] | None:
+        """"""
         _, serializer = self._force_ws_serializer(
             serializer=serializer, serializer_type='request'
         ).popitem()
 
-        schema, request_body_required = self._get_request_for_media_type(serializer, method)
+        schema, _ = self._get_request_for_media_type(serializer)
         if schema is None:
             return None
 
         content = [
             (media_type, schema, self._get_examples(serializer, 'request', media_type))
             for media_type in self.map_parsers()
         ]
@@ -72,57 +84,65 @@
         return {
             'content': {
                 media_type: build_media_type_object(schema, examples)
                 for media_type, schema, examples in content
             }
         }
 
-    def _get_request_for_media_type(self, serializer, method):
-        component = self.resolve_serializer(serializer, method)
+    def _get_request_for_media_type(
+        self, serializer: Serializer, direction: Direction = 'request'
+    ) -> tuple[_SchemaType | None, bool]:
+        """"""
+        component = self.resolve_serializer(serializer, direction)
 
         if not component:
             # serializer is empty so skip content enumeration
             return None, False
 
         schema = component.ref
         return schema, True
 
-    def get_response_bodies(self, response_serializers, method):
-        if response_serializers:
-            if isinstance(response_serializers, dict):
-                return {
-                    f'{self.event}   {code}': self._get_response_for_code(
-                        force_instance(serializer), code
-                    )
-                    for code, serializer in response_serializers.items()
-                }
-
-            serializers_ = self._force_ws_serializer(
-                serializer=response_serializers, direction='receive', serializer_type='response'
-            )
+    def get_response_bodies(
+        self, response_serializers: Serializer | dict[int, Serializer]
+    ) -> dict[str, Any] | None:
+        """"""
+        if not response_serializers:
+            return None
 
+        if isinstance(response_serializers, dict):
             return {
-                f'{event}   {status.HTTP_200_OK}': self._get_response_for_code(
-                    serializer, status.HTTP_200_OK
-                )
-                for event, serializer in serializers_.items()
+                f'{self.event}   {code}': self._get_response_for_code(force_instance(serializer), code)
+                for code, serializer in response_serializers.items()
             }
 
-    def _get_serializer_name(self, serializer, direction: str, bypass_extensions: bool = False):
-        return serializer.__class__.__name__
+        serializers_ = self._force_ws_serializer(
+            serializer=response_serializers, serializer_type='response', direction='receive'
+        )
+
+        return {
+            f'{event}   {status.HTTP_200_OK}': self._get_response_for_code(
+                serializer, status.HTTP_200_OK
+            )
+            for event, serializer in serializers_.items()
+        }
+
+    def _get_serializer_name(
+        self, serializer: Serializer, direction: str, bypass_extensions: bool = False
+    ) -> str:
+        return type(serializer).__name__
 
-    def get_tags(self):
+    def get_tags(self) -> list[str]:
         return ['web_socket']
 
-    def get_summary(self):
+    def get_summary(self) -> str:
         return ''
 
     def _force_ws_serializer(
-        self, serializer, direction: str | None = None, serializer_type: str | None = None
-    ) -> dict[str, serializers.Serializer]:
+        self, serializer: Serializer, serializer_type: Direction, direction: _Type | None = None
+    ) -> dict[str, Serializer]:
         if serializer is None:
             return {self.event: force_instance(EmptySerializer)}
 
         serializer = force_instance(serializer)
 
         if isinstance(serializer, EmptySerializer):
             return {self.event: serializer}
@@ -145,33 +165,33 @@
 
         name: str = self._get_forced_serializer_name(
             direction=direction, serializer_name=serializer_name
         )
 
         if is_list_serializer(serializer):
             inner_name: str = 'Ws%sDataSerializer' % self.event.capitalize()
-            serializer = type(inner_name, (serializers.Serializer,), {self.event: serializer})()
+            serializer = type(inner_name, (Serializer,), {self.event: serializer})()
 
             attrs = {
-                'event': serializers.CharField(default=self.event),
+                'event': CharField(default=self.event),
                 'data': serializer,
             }
         else:
             attrs = {
-                'event': serializers.CharField(default=self.event),
+                'event': CharField(default=self.event),
                 'data': serializer,
             }
 
-        prepared = type(name, (serializers.Serializer,), attrs)() if self.include_event else serializer
+        prepared = type(name, (Serializer,), attrs)() if self.include_event else serializer
 
         self.prepared[serializer_type][self.event] = prepared
         return {self.event: prepared}
 
-    def _force_serializers_list(self, events, serializer_type) -> dict[str, serializers.Serializer]:
-        result: dict[str, serializers.Serializer] = {}
+    def _force_serializers_list(self, events: list[str], serializer_type: str) -> dict[str, Serializer]:
+        result: dict[str, Serializer] = {}
 
         for event in events:
             forced = self.prepared[serializer_type].get(event)
             if forced is None:
                 raise NotReadyError
             result[event] = forced
```

### Comparing `drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/schemas/schema.py` & `drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/schemas/schema.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
-from channels.routing import URLRouter
+from channels.routing import ProtocolTypeRouter, URLRouter
 from django.conf import settings
 from django.contrib.admindocs.views import simplify_regex
 from django.utils.module_loading import import_string
 from drf_spectacular.generators import SchemaGenerator
+from typing_extensions import Never  # noqa: UP035
 
-from .consumer_schema import NotReadyError
+from .consumer_schema import ConsumerAutoSchema, NotReadyError
 
 if TYPE_CHECKING:
     from collections.abc import Callable
 
+    from channels.consumer import AsyncConsumer
+    from rest_framework.serializers import Serializer
+
 
 class WsSchemaGenerator(SchemaGenerator):
     """"""
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
-        self.prepared = {'request': {}, 'response': {}}
+        self.prepared: dict[str, dict[str, Serializer]] = {'request': {}, 'response': {}}
 
-    def parse(self, input_request, public):
+    def parse(self, input_request: None, public: bool) -> dict[str, Any]:
         result = super().parse(input_request, public)
-        ws_result = self.get_ws_endpoints()
+        ws_result = self.get_ws_endpoints
         result.update(ws_result)
         return result
 
     @staticmethod
-    def get_asgi_application():
+    def get_asgi_application() -> ProtocolTypeRouter:
         return import_string(settings.ASGI_APPLICATION)
 
-    def get_ws_endpoints(self):
+    @property
+    def get_ws_endpoints(self) -> list[Never] | dict[str, Any]:
         application = self.get_asgi_application()
 
         socket_routes = application.application_mapping.get('websocket')
 
         if socket_routes is None:
             return []
 
@@ -48,69 +53,65 @@
 
         for route in router.routes:
             consumer = route.callback.consumer_class()
             result.update(self._find_methods(consumer=consumer, path=simplify_regex(str(route.pattern))))
 
         return result
 
-    def _get_router(self, middleware):
+    def _get_router(self, middleware: Any) -> Any:
         try:
             return middleware.inner
         except AttributeError:
             try:
                 return middleware.application
             except AttributeError:
                 return middleware._auths[0]
 
-    def _find_methods(self, consumer, path: str):
+    def _find_methods(self, consumer: AsyncConsumer, path: str) -> dict[str, Any]:
         consumer_endpoints = {}
 
         methods_list = self._get_extended_methods_list(consumer)
         while methods_list:
             method = methods_list.pop(0)
-            event: str = method.event
+            event: str = method.event  # type: ignore[attr-defined]
             name: str = '%s::%s' % (path, event)
 
             action_schema = self.get_action_schema(method=method)
             try:
                 consumer_endpoints[name] = {
                     action_schema.method == 'receive' and 'get' or 'post': {
                         'operationId': f'{event}_{action_schema.get_operation_id()}',
                         'requestBody': action_schema.get_request_body(
                             serializer=action_schema.get_request_serializer(),
-                            method=action_schema.method,
                         ),
                         'summary': action_schema.get_summary(),
                         'description': action_schema.get_description(),
                         'tags': action_schema.get_tags(),
                         'responses': action_schema.get_response_bodies(
                             action_schema.get_response_serializers(),
-                            method=action_schema.method,
                         ),
                     }
                 }
             except NotReadyError:
                 methods_list.append(method)
 
         return consumer_endpoints
 
     @staticmethod
-    def _get_extended_methods_list(consumer):
-        methods_list: list[Callable] = []
+    def _get_extended_methods_list(consumer: AsyncConsumer) -> list[Callable[..., Any]]:
+        methods_list = []
         for attr in dir(consumer):
             method = getattr(consumer, attr)
             if callable(method) and hasattr(method, 'kwargs'):
                 methods_list.append(method)
-
         return methods_list
 
-    def get_action_schema(self, method: Callable):
+    def get_action_schema(self, method: Callable[..., Any]) -> ConsumerAutoSchema:
         schema_class = getattr(method, 'kwargs', {}).get('schema', None)
-        schema = schema_class()
+        schema: ConsumerAutoSchema = schema_class()
         schema.method_name = method.__name__
-        schema.method = method.type
-        schema.event = method.event
-        schema.include_event = method.include_event
+        schema.method = method.type  # type: ignore[attr-defined]
+        schema.event = method.event  # type: ignore[attr-defined]
+        schema.include_event = method.include_event  # type: ignore[attr-defined]
         schema.registry = self.registry
         schema.prepared = self.prepared
-
         return schema
```

### Comparing `drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/settings.py` & `drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+from __future__ import annotations
+
+from typing import Any
+
 from django.conf import settings
 
-SPECTACULAR_SETTINGS: dict = getattr(settings, 'SPECTACULAR_SETTINGS', {})
+SPECTACULAR_SETTINGS: dict[str, Any] = getattr(settings, 'SPECTACULAR_SETTINGS', {})
 
 SPECTACULAR_SETTINGS['DEFAULT_GENERATOR_CLASS'] = 'drf_spectacular_websocket.schemas.WsSchemaGenerator'
 SPECTACULAR_SETTINGS['SWAGGER_UI_DIST'] = 'SIDECAR'
 SPECTACULAR_SETTINGS['SWAGGER_UI_FAVICON_HREF'] = 'SIDECAR'
 SPECTACULAR_SETTINGS['REDOC_DIST'] = 'SIDECAR'
-SWAGGER_UI_SETTINGS: dict = SPECTACULAR_SETTINGS.get('SWAGGER_UI_SETTINGS', {})
+SWAGGER_UI_SETTINGS: dict[str, Any] = SPECTACULAR_SETTINGS.get('SWAGGER_UI_SETTINGS', {})
 SWAGGER_UI_SETTINGS.setdefault('connectSocket', True)
 SWAGGER_UI_SETTINGS.setdefault('socketMaxMessages', 8)
 SWAGGER_UI_SETTINGS.setdefault('socketMessagesInitialOpened', False)
```

### Comparing `drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket/templates/drf_spectacular/swagger_ui.js` & `drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket/templates/drf_spectacular/swagger_ui.js`

 * *Files identical despite different names*

### Comparing `drf_spectacular_websocket-1.2.5/src/drf_spectacular_websocket.egg-info/SOURCES.txt` & `drf_spectacular_websocket-1.2.6/src/drf_spectacular_websocket.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 .editorconfig
 .gitignore
 .pre-commit-config.yaml
+CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
 .github/workflows/publish-to-pypi.yml
 images/example_receive.png
 images/example_send.png
 src/drf_spectacular_websocket/__init__.py
 src/drf_spectacular_websocket/apps.py
 src/drf_spectacular_websocket/decorators.py
 src/drf_spectacular_websocket/settings.py
+src/drf_spectacular_websocket/types.py
 src/drf_spectacular_websocket.egg-info/PKG-INFO
 src/drf_spectacular_websocket.egg-info/SOURCES.txt
 src/drf_spectacular_websocket.egg-info/dependency_links.txt
 src/drf_spectacular_websocket.egg-info/entry_points.txt
 src/drf_spectacular_websocket.egg-info/requires.txt
 src/drf_spectacular_websocket.egg-info/top_level.txt
 src/drf_spectacular_websocket/schemas/__init__.py
 src/drf_spectacular_websocket/schemas/consumer_schema.py
 src/drf_spectacular_websocket/schemas/schema.py
 src/drf_spectacular_websocket/templates/drf_spectacular/swagger_ui.js
 tests/__init__.py
 tests/asgi.py
 tests/conftest.py
 tests/consumers.py
-tests/expected_schemas.py
 tests/serializers.py
-tests/test_schema.py
-tests/urls.py
+tests/urls.py
+tests/schemas/__init__.py
+tests/schemas/expected_schema.py
+tests/schemas/test_schema.py
```

### Comparing `drf_spectacular_websocket-1.2.5/tests/consumers.py` & `drf_spectacular_websocket-1.2.6/tests/consumers.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,45 +9,45 @@
     @extend_ws_schema(
         type='send',
         summary='method_1 summary',
         description='method_1 description',
         request=InputSerializer,
         responses=OutputSerializer,
     )
-    def method_1(self):
+    def method_1(self) -> None:
         pass
 
     @extend_ws_schema(
         type='send',
         summary='method_2 summary',
         description='method_2 description',
         request=InputSerializer,
         responses={
             status.HTTP_201_CREATED: OutputSerializer,
             status.HTTP_400_BAD_REQUEST: BadOutputSerializer,
         },
     )
-    def method_2(self):
+    def method_2(self) -> None:
         pass
 
     @extend_ws_schema(
         type='receive',
         summary='method_3 summary',
         description='method_3 description',
         request=None,
         responses=OutputSerializer,
     )
-    def method_3(self):
+    def method_3(self) -> None:
         pass
 
     @extend_ws_schema(
         type='receive',
         summary='method_4 summary',
         description='method_4 description',
         request=None,
         responses={
             status.HTTP_201_CREATED: OutputSerializer,
             status.HTTP_400_BAD_REQUEST: BadOutputSerializer,
         },
     )
-    def method_4(self):
+    def method_4(self) -> None:
         pass
```

### Comparing `drf_spectacular_websocket-1.2.5/tests/expected_schemas.py` & `drf_spectacular_websocket-1.2.6/tests/schemas/expected_schema.py`

 * *Files identical despite different names*

