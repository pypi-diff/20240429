# Comparing `tmp/tap_shortcut-0.4.0a1.tar.gz` & `tmp/tap_shortcut-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Feb  5 19:52:02 2024, max compression
+gzip compressed data, last modified: Mon Apr 29 20:22:18 2024, max compression
```

## Comparing `tap_shortcut-0.4.0a1.tar` & `tap_shortcut-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0      670 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/.copier-answers.yml
--rw-r--r--   0        0        0      797 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1051 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/meltano.yml
--rw-r--r--   0        0        0      712 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/.github/FUNDING.yml
--rw-r--r--   0        0        0     1298 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/.github/dependabot.yml
--rw-r--r--   0        0        0       23 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/.github/workflows/constraints.txt
--rw-r--r--   0        0        0      793 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/.github/workflows/dynamic-publish.yaml
--rw-r--r--   0        0        0     1489 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/.github/workflows/test.yml
--rw-r--r--   0        0        0       14 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/output/.gitignore
--rw-r--r--   0        0        0     1709 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/plugins/loaders/target-jsonl--andyh1203.lock
--rw-r--r--   0        0        0     1260 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/plugins/loaders/target-sqlite--meltanolabs.lock
--rw-r--r--   0        0        0       47 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/tap_shortcut/__init__.py
--rw-r--r--   0        0        0      119 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/tap_shortcut/__main__.py
--rw-r--r--   0        0        0     1953 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/tap_shortcut/client.py
--rw-r--r--   0        0        0     2895 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/tap_shortcut/streams.py
--rw-r--r--   0        0        0     3738 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/tap_shortcut/tap.py
--rw-r--r--   0        0        0       63 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/tests/conftest.py
--rw-r--r--   0        0        0      545 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/tests/test_core.py
--rw-r--r--   0        0        0     5006 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/tests/test_openapi.py
--rw-r--r--   0        0        0     1914 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/.gitignore
--rw-r--r--   0        0        0    11357 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/LICENSE
--rw-r--r--   0        0        0     2439 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/README.md
--rw-r--r--   0        0        0     3090 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/pyproject.toml
--rw-r--r--   0        0        0    16722 2024-02-05 19:52:02.000000 tap_shortcut-0.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0      670 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/.copier-answers.yml
+-rw-r--r--   0        0        0      797 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1051 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/meltano.yml
+-rw-r--r--   0        0        0     1298 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/.github/dependabot.yml
+-rw-r--r--   0        0        0       23 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0      793 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/.github/workflows/dynamic-publish.yaml
+-rw-r--r--   0        0        0     1513 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0       14 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/output/.gitignore
+-rw-r--r--   0        0        0     1709 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/plugins/loaders/target-jsonl--andyh1203.lock
+-rw-r--r--   0        0        0     1260 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/plugins/loaders/target-sqlite--meltanolabs.lock
+-rw-r--r--   0        0        0       47 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/tap_shortcut/__init__.py
+-rw-r--r--   0        0        0      119 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/tap_shortcut/__main__.py
+-rw-r--r--   0        0        0     1954 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/tap_shortcut/client.py
+-rw-r--r--   0        0        0     2895 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/tap_shortcut/streams.py
+-rw-r--r--   0        0        0     3739 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/tap_shortcut/tap.py
+-rw-r--r--   0        0        0       64 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0      545 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/tests/test_core.py
+-rw-r--r--   0        0        0     5007 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/tests/test_openapi.py
+-rw-r--r--   0        0        0     1914 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/.gitignore
+-rw-r--r--   0        0        0    11357 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2438 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/README.md
+-rw-r--r--   0        0        0     3066 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    16719 2024-04-29 20:22:18.000000 tap_shortcut-0.4.1/PKG-INFO
```

### Comparing `tap_shortcut-0.4.0a1/.copier-answers.yml` & `tap_shortcut-0.4.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.4.0a1/.pre-commit-config.yaml` & `tap_shortcut-0.4.1/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,33 @@
   autofix_prs: false
   autofix_commit_msg: '[pre-commit.ci] auto fixes'
   autoupdate_schedule: weekly
   autoupdate_commit_msg: 'chore(deps): pre-commit autoupdate'
 
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
   - id: check-json
     exclude: "\\.vscode/.*.json"
   - id: check-toml
   - id: check-yaml
   - id: end-of-file-fixer
     exclude: "plugins/.*/.*\\.lock"
   - id: trailing-whitespace
 
 - repo: https://github.com/tox-dev/pyproject-fmt
-  rev: "1.7.0"
+  rev: "1.8.0"
   hooks:
   - id: pyproject-fmt
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: "v0.2.0"
+  rev: "v0.4.2"
   hooks:
   - id: ruff
     args: [--fix, --exit-non-zero-on-fix, --show-fixes]
   - id: ruff-format
 
 - repo: https://github.com/pre-commit/pre-commit
-  rev: v3.6.0
+  rev: v3.7.0
   hooks:
   - id: validate_manifest
```

### Comparing `tap_shortcut-0.4.0a1/meltano.yml` & `tap_shortcut-0.4.1/meltano.yml`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.4.0a1/.github/dependabot.yml` & `tap_shortcut-0.4.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.4.0a1/.github/workflows/dynamic-publish.yaml` & `tap_shortcut-0.4.1/.github/workflows/dynamic-publish.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,8 @@
         with:
           file: dist/*.whl
           tag: ${{ github.ref }}
           overwrite: true
           file_glob: true
 
       - name: Publish
-        uses: pypa/gh-action-pypi-publish@v1.8.11
+        uses: pypa/gh-action-pypi-publish@v1.8.14
```

### Comparing `tap_shortcut-0.4.0a1/.github/workflows/test.yml` & `tap_shortcut-0.4.1/.github/workflows/test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -22,30 +22,30 @@
   workflow_dispatch:
 
 jobs:
   tests:
     runs-on: ubuntu-latest
     env:
       FORCE_COLOR: "1"
-      PIP_CONSTRAINT: .github/workflows/constraints.txt
+      PIP_CONSTRAINT: ${{ github.workspace }}/.github/workflows/constraints.txt
     strategy:
       fail-fast: false
       matrix:
         script: ["test:integration"]
         python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
         include:
         - { script: "test:dependencies", python-version: "3.12" }
         - { script: "typing:check",      python-version: "3.12" }
 
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
 
-    - uses: actions/setup-python@v5.0.0
+    - uses: actions/setup-python@v5.1.0
       id: setup-python
       with:
         python-version: ${{ matrix.python-version }}
         cache: pip
 
     - name: Upgrade pip
       run: |
```

### Comparing `tap_shortcut-0.4.0a1/plugins/loaders/target-jsonl--andyh1203.lock` & `tap_shortcut-0.4.1/plugins/loaders/target-jsonl--andyh1203.lock`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.4.0a1/plugins/loaders/target-sqlite--meltanolabs.lock` & `tap_shortcut-0.4.1/plugins/loaders/target-sqlite--meltanolabs.lock`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.4.0a1/tap_shortcut/client.py` & `tap_shortcut-0.4.1/tap_shortcut/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """REST client handling, including ShortcutStream base class."""
+
 from __future__ import annotations
 
 import typing as t
 
 from singer_sdk import RESTStream
 from singer_sdk.authenticators import APIKeyAuthenticator
```

### Comparing `tap_shortcut-0.4.0a1/tap_shortcut/streams.py` & `tap_shortcut-0.4.1/tap_shortcut/streams.py`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.4.0a1/tap_shortcut/tap.py` & `tap_shortcut-0.4.1/tap_shortcut/tap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Shortcut tap class."""
+
 from __future__ import annotations
 
 from copy import deepcopy
 from typing import TYPE_CHECKING, Any
 
 import requests
 from singer_sdk import RESTStream, Stream, Tap
```

### Comparing `tap_shortcut-0.4.0a1/tests/test_core.py` & `tap_shortcut-0.4.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.4.0a1/tests/test_openapi.py` & `tap_shortcut-0.4.1/tests/test_openapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test OpenAPI handling."""
+
 from __future__ import annotations
 
 import typing as t
 
 import pytest
 
 from tap_shortcut.tap import handle_x_nullable
```

### Comparing `tap_shortcut-0.4.0a1/.gitignore` & `tap_shortcut-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.4.0a1/LICENSE` & `tap_shortcut-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_shortcut-0.4.0a1/README.md` & `tap_shortcut-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 ```
 
 ### Create and Run Tests
 
 Run integration tests:
 
 ```bash
-hatch run tests:integration
+hatch run test:integration
 ```
 
 You can also test the `tap-shortcut` CLI interface directly:
 
 ```bash
 hatch run sync:console -- --about --format=json
 ```
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 -about` ### Source Authentication and Authorization See https://
 developer.shortcut.com/api/rest/v3#Authentication. ## Usage You can easily run
 `tap-shortcut` by itself or in a pipeline using [Meltano](https://meltano.com/
 ). ### Executing the Tap Directly ```bash tap-shortcut --version tap-shortcut -
 -help tap-shortcut --config CONFIG --discover > ./catalog.json ``` ## Developer
 Resources ### Initialize your Development Environment ```bash pipx install
 hatch ``` ### Create and Run Tests Run integration tests: ```bash hatch run
-tests:integration ``` You can also test the `tap-shortcut` CLI interface
+test:integration ``` You can also test the `tap-shortcut` CLI interface
 directly: ```bash hatch run sync:console -- --about --format=json ``` ###
 Testing with [Meltano](https://www.meltano.com) _**Note:** This tap will work
 in any Singer environment and does not require Meltano. Examples here are for
 convenience and to streamline end-to-end orchestration scenarios._ Your project
 comes with a custom `meltano.yml` project file already created. Go ahead and
 [install Meltano](https://docs.meltano.com/getting-started/installation/) if
 you haven't already. 1. Install all plugins ```bash meltano install ``` 1.
```

### Comparing `tap_shortcut-0.4.0a1/pyproject.toml` & `tap_shortcut-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -27,21 +27,21 @@
   "Programming Language :: Python :: 3.12",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   "requests",
-  "singer-sdk~=0.35.0",
+  "singer-sdk~=0.37.0",
   "toolz==0.12.1",
 ]
 optional-dependencies.testing = [
   "deptry>=0.12",
   "pytest>=7.4",
-  "singer-sdk[testing]~=0.35.0",
+  "singer-sdk[testing]~=0.37.0",
 ]
 optional-dependencies.typing = [
   "mypy",
   "types-requests",
 ]
 urls.documentation = "https://github.com/edgarrmondragon/tap-shortcut#readme"
 urls.homepage = "https://github.com/edgarrmondragon/tap-shortcut"
@@ -70,15 +70,14 @@
 features = ["testing", "typing"]
 [tool.hatch.envs.typing.scripts]
 check = "mypy --strict {args:tap_shortcut tests}"
 
 [tool.ruff]
 line-length = 88
 src = ["tap_shortcut", "tests"]
-target-version = "py38"
 
 [tool.ruff.lint]
 ignore = [
   "ANN101", # missing-type-self
   "DJ",     # flake8-django
   "COM812",  # missing-trailing-comma
   "ISC001",  # single-line-implicit-string-concatenation
```

### Comparing `tap_shortcut-0.4.0a1/PKG-INFO` & `tap_shortcut-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tap-shortcut
-Version: 0.4.0a1
+Version: 0.4.1
 Summary: `tap-shortcut` is a Singer tap for Shortcut, built with the Meltano SDK for Singer Taps.
 Project-URL: documentation, https://github.com/edgarrmondragon/tap-shortcut#readme
 Project-URL: homepage, https://github.com/edgarrmondragon/tap-shortcut
 Project-URL: source, https://github.com/edgarrmondragon/tap-shortcut
 Author-email: Edgar Ramírez-Mondragón <edgarrm358@gmail.com>
 Maintainer-email: Edgar Ramírez-Mondragón <edgarrm358@gmail.com>
 License:                                  Apache License
@@ -214,20 +214,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: requests
-Requires-Dist: singer-sdk~=0.35.0
+Requires-Dist: singer-sdk~=0.37.0
 Requires-Dist: toolz==0.12.1
 Provides-Extra: testing
 Requires-Dist: deptry>=0.12; extra == 'testing'
 Requires-Dist: pytest>=7.4; extra == 'testing'
-Requires-Dist: singer-sdk[testing]~=0.35.0; extra == 'testing'
+Requires-Dist: singer-sdk[testing]~=0.37.0; extra == 'testing'
 Provides-Extra: typing
 Requires-Dist: mypy; extra == 'typing'
 Requires-Dist: types-requests; extra == 'typing'
 Description-Content-Type: text/markdown
 
 <div align="center">
 
@@ -287,15 +287,15 @@
 ```
 
 ### Create and Run Tests
 
 Run integration tests:
 
 ```bash
-hatch run tests:integration
+hatch run test:integration
 ```
 
 You can also test the `tap-shortcut` CLI interface directly:
 
 ```bash
 hatch run sync:console -- --about --format=json
 ```
```

