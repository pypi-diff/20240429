# Comparing `tmp/tap_bitso-0.2.1.tar.gz` & `tmp/tap_bitso-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Mar  4 20:07:40 2024, max compression
+gzip compressed data, last modified: Mon Apr 29 19:42:59 2024, max compression
```

## Comparing `tap_bitso-0.2.1.tar` & `tap_bitso-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      252 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/.env.example
--rw-r--r--   0        0        0       99 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/.flake8
--rw-r--r--   0        0        0      796 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1265 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/meltano.yml
--rw-r--r--   0        0        0      642 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/tap_bitso_logging.yaml
--rw-r--r--   0        0        0     1143 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/.github/dependabot.yml
--rw-r--r--   0        0        0       23 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/.github/workflows/constraints.txt
--rw-r--r--   0        0        0      782 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1504 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      409 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/output/.gitignore
--rw-r--r--   0        0        0     1708 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/plugins/loaders/target-jsonl--andyh1203.lock
--rw-r--r--   0        0        0     7599 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/plugins/loaders/target-postgres--transferwise.lock
--rw-r--r--   0        0        0     1174 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/plugins/loaders/target-sqlite--meltano.lock
--rw-r--r--   0        0        0       74 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/tap_bitso/__init__.py
--rw-r--r--   0        0        0     2568 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/tap_bitso/auth.py
--rw-r--r--   0        0        0     4994 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/tap_bitso/client.py
--rw-r--r--   0        0        0     1698 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/tap_bitso/streams.py
--rw-r--r--   0        0        0     2713 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/tap_bitso/tap.py
--rw-r--r--   0        0        0       58 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/tap_bitso/schemas/__init__.py
--rw-r--r--   0        0        0     8787 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/tap_bitso/schemas/book.json
--rw-r--r--   0        0        0     3098 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/tap_bitso/schemas/ledger.json
--rw-r--r--   0        0        0     3398 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/tap_bitso/schemas/ticker.json
--rw-r--r--   0        0        0     2232 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/tap_bitso/schemas/trade.json
--rw-r--r--   0        0        0       68 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0       92 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0      671 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/tests/test_core.py
--rw-r--r--   0        0        0     2272 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/.gitignore
--rw-r--r--   0        0        0    11357 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/LICENSE
--rw-r--r--   0        0        0     2707 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/README.md
--rw-r--r--   0        0        0     2799 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/pyproject.toml
--rw-r--r--   0        0        0    17192 2024-03-04 20:07:40.000000 tap_bitso-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      252 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/.env.example
+-rw-r--r--   0        0        0       99 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/.flake8
+-rw-r--r--   0        0        0      796 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1265 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/meltano.yml
+-rw-r--r--   0        0        0      642 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/tap_bitso_logging.yaml
+-rw-r--r--   0        0        0     1143 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/.github/dependabot.yml
+-rw-r--r--   0        0        0       23 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0      782 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1528 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      409 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/output/.gitignore
+-rw-r--r--   0        0        0     1708 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/plugins/loaders/target-jsonl--andyh1203.lock
+-rw-r--r--   0        0        0     7599 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/plugins/loaders/target-postgres--transferwise.lock
+-rw-r--r--   0        0        0     1174 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/plugins/loaders/target-sqlite--meltano.lock
+-rw-r--r--   0        0        0       74 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/tap_bitso/__init__.py
+-rw-r--r--   0        0        0     2568 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/tap_bitso/auth.py
+-rw-r--r--   0        0        0     4994 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/tap_bitso/client.py
+-rw-r--r--   0        0        0     1698 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/tap_bitso/streams.py
+-rw-r--r--   0        0        0     2713 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/tap_bitso/tap.py
+-rw-r--r--   0        0        0       58 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/tap_bitso/schemas/__init__.py
+-rw-r--r--   0        0        0     8787 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/tap_bitso/schemas/book.json
+-rw-r--r--   0        0        0     3098 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/tap_bitso/schemas/ledger.json
+-rw-r--r--   0        0        0     3728 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/tap_bitso/schemas/ticker.json
+-rw-r--r--   0        0        0     2232 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/tap_bitso/schemas/trade.json
+-rw-r--r--   0        0        0       68 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0      671 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/tests/test_core.py
+-rw-r--r--   0        0        0     2272 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/.gitignore
+-rw-r--r--   0        0        0    11357 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2707 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/README.md
+-rw-r--r--   0        0        0     2799 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0    17192 2024-04-29 19:42:59.000000 tap_bitso-0.2.2/PKG-INFO
```

### Comparing `tap_bitso-0.2.1/.pre-commit-config.yaml` & `tap_bitso-0.2.2/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 
 - repo: https://github.com/tox-dev/pyproject-fmt
   rev: "1.7.0"
   hooks:
   - id: pyproject-fmt
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.2.0
+  rev: v0.3.5
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

### Comparing `tap_bitso-0.2.1/meltano.yml` & `tap_bitso-0.2.2/meltano.yml`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/tap_bitso_logging.yaml` & `tap_bitso-0.2.2/tap_bitso_logging.yaml`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/.github/dependabot.yml` & `tap_bitso-0.2.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/.github/workflows/release.yaml` & `tap_bitso-0.2.2/.github/workflows/release.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,8 @@
         with:
           file: dist/*.whl
           tag: ${{ github.ref }}
           overwrite: true
           file_glob: true
 
       - name: Publish
-        uses: pypa/gh-action-pypi-publish@v1.8.12
+        uses: pypa/gh-action-pypi-publish@v1.8.14
```

### Comparing `tap_bitso-0.2.1/.github/workflows/test.yml` & `tap_bitso-0.2.2/.github/workflows/test.yml`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
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
```

### Comparing `tap_bitso-0.2.1/plugins/loaders/target-jsonl--andyh1203.lock` & `tap_bitso-0.2.2/plugins/loaders/target-jsonl--andyh1203.lock`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/plugins/loaders/target-postgres--transferwise.lock` & `tap_bitso-0.2.2/plugins/loaders/target-postgres--transferwise.lock`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/plugins/loaders/target-sqlite--meltano.lock` & `tap_bitso-0.2.2/plugins/loaders/target-sqlite--meltano.lock`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/tap_bitso/auth.py` & `tap_bitso-0.2.2/tap_bitso/auth.py`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/tap_bitso/client.py` & `tap_bitso-0.2.2/tap_bitso/client.py`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/tap_bitso/streams.py` & `tap_bitso-0.2.2/tap_bitso/streams.py`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/tap_bitso/tap.py` & `tap_bitso-0.2.2/tap_bitso/tap.py`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/tap_bitso/schemas/book.json` & `tap_bitso-0.2.2/tap_bitso/schemas/book.json`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/tap_bitso/schemas/ledger.json` & `tap_bitso-0.2.2/tap_bitso/schemas/ledger.json`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/tap_bitso/schemas/ticker.json` & `tap_bitso-0.2.2/tap_bitso/schemas/ticker.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954545454545455%*

 * *Differences: {"'properties'": "{'rolling_average_change': OrderedDict([('$id', "*

 * *                 "'#/properties/rolling_average_change'), ('type', 'object'), ('examples', "*

 * *                 "[OrderedDict([('6', '-0.5228')])]), ('properties', OrderedDict([('6', "*

 * *                 "OrderedDict([('type', 'string'), ('examples', ['-0.5228'])]))]))])}"}*

```diff
@@ -96,14 +96,31 @@
             "description": "An explanation about the purpose of this instance.",
             "examples": [
                 "5450.00"
             ],
             "title": "The low schema",
             "type": "string"
         },
+        "rolling_average_change": {
+            "$id": "#/properties/rolling_average_change",
+            "examples": [
+                {
+                    "6": "-0.5228"
+                }
+            ],
+            "properties": {
+                "6": {
+                    "examples": [
+                        "-0.5228"
+                    ],
+                    "type": "string"
+                }
+            },
+            "type": "object"
+        },
         "volume": {
             "$id": "#/properties/volume",
             "default": "",
             "description": "An explanation about the purpose of this instance.",
             "examples": [
                 "22.31349615"
             ],
```

### Comparing `tap_bitso-0.2.1/tap_bitso/schemas/trade.json` & `tap_bitso-0.2.2/tap_bitso/schemas/trade.json`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/tests/test_core.py` & `tap_bitso-0.2.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/.gitignore` & `tap_bitso-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/LICENSE` & `tap_bitso-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/README.md` & `tap_bitso-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tap_bitso-0.2.1/pyproject.toml` & `tap_bitso-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,34 +28,34 @@
   "Programming Language :: Python :: 3.12",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
   'importlib-resources<7,>=6; python_version < "3.9"',
-  "singer-sdk~=0.36.0",
+  "singer-sdk~=0.37.0",
   "stamina~=24.2.0",
   "structlog<25,>=23",
 ]
 optional-dependencies.dev = [
   "colorama>=0.4.4",
-  "singer-sdk[testing,typing]~=0.36.0",
+  "singer-sdk[testing,typing]~=0.37.0",
 ]
 optional-dependencies.testing = [
   "deptry>=0.12",
   "pytest>=7.4",
-  "singer-sdk[testing]~=0.36.0",
+  "singer-sdk[testing]~=0.37.0",
 ]
 optional-dependencies.typing = [
   "mypy",
   "types-requests",
 ]
-urls.documentation = "https://github.com/edgarrmondragon/tap-bitso#readme"
-urls.homepage = "https://github.com/edgarrmondragon/tap-bitso"
-urls.repository = "https://github.com/edgarrmondragon/tap-bitso"
+urls.Documentation = "https://github.com/edgarrmondragon/tap-bitso#readme"
+urls.Homepage = "https://github.com/edgarrmondragon/tap-bitso"
+urls.Repository = "https://github.com/edgarrmondragon/tap-bitso"
 scripts."tap-bitso" = 'tap_bitso.tap:TapBitso.cli'
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.envs.sync.scripts]
 console = "tap-bitso {args}"
```

### Comparing `tap_bitso-0.2.1/PKG-INFO` & `tap_bitso-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tap-bitso
-Version: 0.2.1
+Version: 0.2.2
 Summary: `tap-bitso` is a Singer tap for Bitso, built with the Meltano SDK for Singer Taps.
-Project-URL: documentation, https://github.com/edgarrmondragon/tap-bitso#readme
-Project-URL: homepage, https://github.com/edgarrmondragon/tap-bitso
-Project-URL: repository, https://github.com/edgarrmondragon/tap-bitso
+Project-URL: Documentation, https://github.com/edgarrmondragon/tap-bitso#readme
+Project-URL: Homepage, https://github.com/edgarrmondragon/tap-bitso
+Project-URL: Repository, https://github.com/edgarrmondragon/tap-bitso
 Author-email: Edgar Ramírez-Mondragón <edgarrm358@gmail.com>
 Maintainer-email: Edgar Ramírez-Mondragón <edgarrm358@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -214,24 +214,24 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: importlib-resources<7,>=6; python_version < '3.9'
-Requires-Dist: singer-sdk~=0.36.0
+Requires-Dist: singer-sdk~=0.37.0
 Requires-Dist: stamina~=24.2.0
 Requires-Dist: structlog<25,>=23
 Provides-Extra: dev
 Requires-Dist: colorama>=0.4.4; extra == 'dev'
-Requires-Dist: singer-sdk[testing,typing]~=0.36.0; extra == 'dev'
+Requires-Dist: singer-sdk[testing,typing]~=0.37.0; extra == 'dev'
 Provides-Extra: testing
 Requires-Dist: deptry>=0.12; extra == 'testing'
 Requires-Dist: pytest>=7.4; extra == 'testing'
-Requires-Dist: singer-sdk[testing]~=0.36.0; extra == 'testing'
+Requires-Dist: singer-sdk[testing]~=0.37.0; extra == 'testing'
 Provides-Extra: typing
 Requires-Dist: mypy; extra == 'typing'
 Requires-Dist: types-requests; extra == 'typing'
 Description-Content-Type: text/markdown
 
 # tap-bitso
```

