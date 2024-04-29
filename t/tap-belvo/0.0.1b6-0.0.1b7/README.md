# Comparing `tmp/tap_belvo-0.0.1b6.tar.gz` & `tmp/tap_belvo-0.0.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu Dec  7 06:12:03 2023, max compression
+gzip compressed data, last modified: Mon Apr 29 20:21:53 2024, max compression
```

## Comparing `tap_belvo-0.0.1b6.tar` & `tap_belvo-0.0.1b7.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0      681 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/.copier-answers.yml
--rw-r--r--   0        0        0      162 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/.flake8
--rw-r--r--   0        0        0      797 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1374 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/meltano.yml
--rw-r--r--   0        0        0      972 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/.github/dependabot.yml
--rw-r--r--   0        0        0       25 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/.github/workflows/constraints.txt
--rw-r--r--   0        0        0      860 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/.github/workflows/dynamic-publish.yaml
--rw-r--r--   0        0        0     2011 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/.github/workflows/test.yml
--rw-r--r--   0        0        0      409 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/.secrets/.gitignore
--rw-r--r--   0        0        0       14 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/output/.gitignore
--rw-r--r--   0        0        0     4473 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/plugins/loaders/target-duckdb--jwills.lock
--rw-r--r--   0        0        0     1708 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/plugins/loaders/target-jsonl--andyh1203.lock
--rw-r--r--   0        0        0       80 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/tap_belvo/__init__.py
--rw-r--r--   0        0        0      110 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/tap_belvo/__main__.py
--rw-r--r--   0        0        0     5422 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/tap_belvo/client.py
--rw-r--r--   0        0        0     2006 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/tap_belvo/tap.py
--rw-r--r--   0        0        0  1287233 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/tap_belvo/openapi/BelvoOpenFinanceApiSpec.json
--rw-r--r--   0        0        0      754 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/tap_belvo/openapi/__init__.py
--rw-r--r--   0        0        0      936 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/tap_belvo/streams/__init__.py
--rw-r--r--   0        0        0     2651 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/tap_belvo/streams/banking.py
--rw-r--r--   0        0        0      845 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/tap_belvo/streams/enrichment.py
--rw-r--r--   0        0        0     1771 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/tap_belvo/streams/fiscal.py
--rw-r--r--   0        0        0     1021 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/tap_belvo/streams/links.py
--rw-r--r--   0        0        0       74 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/tests/__init__.py
--rw-r--r--   0        0        0      148 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/tests/conftest.py
--rw-r--r--   0        0        0     1791 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/tests/test_core.py
--rw-r--r--   0        0        0     3903 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/.gitignore
--rw-r--r--   0        0        0     1068 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/LICENSE
--rw-r--r--   0        0        0     2580 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/README.md
--rw-r--r--   0        0        0     3020 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/pyproject.toml
--rw-r--r--   0        0        0     4031 2023-12-07 06:12:03.000000 tap_belvo-0.0.1b6/PKG-INFO
+-rw-r--r--   0        0        0      681 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/.copier-answers.yml
+-rw-r--r--   0        0        0      798 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1374 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/meltano.yml
+-rw-r--r--   0        0        0     1184 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/.github/dependabot.yml
+-rw-r--r--   0        0        0       23 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/.github/workflows/constraints.txt
+-rw-r--r--   0        0        0      860 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/.github/workflows/dynamic-publish.yaml
+-rw-r--r--   0        0        0     1987 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/.github/workflows/test.yml
+-rw-r--r--   0        0        0      409 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/.secrets/.gitignore
+-rw-r--r--   0        0        0       14 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/output/.gitignore
+-rw-r--r--   0        0        0     5776 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/plugins/loaders/target-duckdb--jwills.lock
+-rw-r--r--   0        0        0     1708 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/plugins/loaders/target-jsonl--andyh1203.lock
+-rw-r--r--   0        0        0       80 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/tap_belvo/__init__.py
+-rw-r--r--   0        0        0      110 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/tap_belvo/__main__.py
+-rw-r--r--   0        0        0     5422 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/tap_belvo/client.py
+-rw-r--r--   0        0        0     1970 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/tap_belvo/tap.py
+-rw-r--r--   0        0        0  1287233 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/tap_belvo/openapi/BelvoOpenFinanceApiSpec.json
+-rw-r--r--   0        0        0      754 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/tap_belvo/openapi/__init__.py
+-rw-r--r--   0        0        0      936 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/tap_belvo/streams/__init__.py
+-rw-r--r--   0        0        0     2467 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/tap_belvo/streams/banking.py
+-rw-r--r--   0        0        0      761 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/tap_belvo/streams/enrichment.py
+-rw-r--r--   0        0        0     1603 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/tap_belvo/streams/fiscal.py
+-rw-r--r--   0        0        0      965 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/tap_belvo/streams/links.py
+-rw-r--r--   0        0        0       74 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/tests/__init__.py
+-rw-r--r--   0        0        0       92 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/tests/conftest.py
+-rw-r--r--   0        0        0     1791 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/tests/test_core.py
+-rw-r--r--   0        0        0     3903 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/.gitignore
+-rw-r--r--   0        0        0     1068 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/LICENSE
+-rw-r--r--   0        0        0     2579 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/README.md
+-rw-r--r--   0        0        0     2941 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/pyproject.toml
+-rw-r--r--   0        0        0     3971 2024-04-29 20:21:53.000000 tap_belvo-0.0.1b7/PKG-INFO
```

### Comparing `tap_belvo-0.0.1b6/.copier-answers.yml` & `tap_belvo-0.0.1b7/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b6/.pre-commit-config.yaml` & `tap_belvo-0.0.1b7/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,22 @@
   - id: check-toml
   - id: check-yaml
   - id: end-of-file-fixer
     exclude: "plugins/.*/.*\\.lock"
   - id: trailing-whitespace
 
 - repo: https://github.com/tox-dev/pyproject-fmt
-  rev: "1.5.3"
+  rev: "1.6.0"
   hooks:
   - id: pyproject-fmt
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: "v0.1.7"
+  rev: "v0.1.13"
   hooks:
   - id: ruff
     args: [--fix, --exit-non-zero-on-fix, --show-fixes]
   - id: ruff-format
 
 - repo: https://github.com/pre-commit/pre-commit
-  rev: v3.5.0
+  rev: v3.6.0
   hooks:
   - id: validate_manifest
```

### Comparing `tap_belvo-0.0.1b6/meltano.yml` & `tap_belvo-0.0.1b7/meltano.yml`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b6/.github/dependabot.yml` & `tap_belvo-0.0.1b7/.github/dependabot.yml`

 * *Files 19% similar despite different names*

```diff
@@ -11,14 +11,18 @@
       interval: "daily"
     reviewers:
       - "edgarrmondragon"
     versioning-strategy: increase-if-necessary
     commit-message:
       prefix: "chore(deps): "
       prefix-development: "chore(deps-dev): "
+    groups:
+      singer-sdk:
+        patterns:
+          - "singer-sdk*"
   - package-ecosystem: pip
     directory: "/.github/workflows"
     schedule:
       interval: "daily"
     reviewers:
       - "edgarrmondragon"
     commit-message:
@@ -27,7 +31,12 @@
     directory: "/"
     schedule:
       interval: "weekly"
     reviewers:
       - "edgarrmondragon"
     commit-message:
       prefix: "ci: "
+    groups:
+      artifacts:
+        patterns:
+          - "actions/*-load-artifact"
+          - "hynek/build-and-inspect-python-package"
```

### Comparing `tap_belvo-0.0.1b6/.github/workflows/dynamic-publish.yaml` & `tap_belvo-0.0.1b7/.github/workflows/dynamic-publish.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -11,30 +11,30 @@
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
         ref: ${{ github.ref }}
     - uses: actions/setup-python@v5
       with:
         python-version: "3.11"
-    - uses: hynek/build-and-inspect-python-package@v1
+    - uses: hynek/build-and-inspect-python-package@v2
 
   publish:
     name: Publish to PyPI
     if: startsWith(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
     needs: build
     permissions:
       contents: write
       id-token: write
 
     steps:
-    - uses: actions/download-artifact@v3
+    - uses: actions/download-artifact@v4
       with:
         name: Packages
         path: dist
     - uses: svenstaro/upload-release-action@v2
       with:
         file: dist/*.whl
         tag: ${{ github.ref }}
         overwrite: true
         file_glob: true
-    - uses: pypa/gh-action-pypi-publish@v1.8.11
+    - uses: pypa/gh-action-pypi-publish@v1.8.14
```

### Comparing `tap_belvo-0.0.1b6/.github/workflows/test.yml` & `tap_belvo-0.0.1b7/.github/workflows/test.yml`

 * *Files 9% similar despite different names*

```diff
@@ -21,42 +21,40 @@
   - cron: "0 10 * * *"
 
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
         - { script: "test:dependencies", python-version: "3.11" }
         - { script: "typing:check",      python-version: "3.11" }
 
     steps:
-    - name: Checkout code
-      uses: actions/checkout@v4
-
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v5
+    - uses: actions/checkout@v4
+    - uses: actions/setup-python@v5
+      id: setup-python
       with:
         python-version: ${{ matrix.python-version }}
         cache: pip
 
     - name: Upgrade pip
       run: |
         pip install pip
         pip --version
 
     - name: Install Hatch
       run: |
-        pipx install hatch --python "python${{ matrix.python-version }}"
+        pipx install --python '${{ steps.setup-python.outputs.python-path }}' hatch
         hatch --version
 
     - name: Run
       env:
         TAP_BELVO_SECRET_ID: ${{ secrets.TAP_BELVO_SECRET_ID }}
         TAP_BELVO_PASSWORD: ${{ secrets.TAP_BELVO_PASSWORD }}
         TAP_BELVO_BASE_URL: https://sandbox.belvo.com
@@ -74,11 +72,11 @@
     - name: Set up Python
       uses: actions/setup-python@v5
       with:
         python-version: "3.11"
         cache: pip
         cache-dependency-path: .pre-commit-config.yaml
 
-    - uses: pre-commit/action@v3.0.0
+    - uses: pre-commit/action@v3.0.1
 
-    - uses: pre-commit-ci/lite-action@v1.0.1
+    - uses: pre-commit-ci/lite-action@v1.0.2
       if: always()
```

### Comparing `tap_belvo-0.0.1b6/plugins/loaders/target-duckdb--jwills.lock` & `tap_belvo-0.0.1b7/plugins/loaders/target-duckdb--jwills.lock`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9423202614379086%*

 * *Differences: {"'pip_url'": "'target-duckdb~=0.6'",*

 * * "'settings'": "{1: {'description': 'Alias of `path`.', 'placeholder': "*

 * *               "'/path/to/local/file.duckdb', 'value': "*

 * *               "'${MELTANO_PROJECT_ROOT}/output/warehouse.duckdb'}, 9: {'value': "*

 * *               "'$MELTANO_EXTRACT__LOAD_SCHEMA'}, insert: [(0, OrderedDict([('name', 'path'), "*

 * *               "('kind', 'string'), ('label', 'Connection Path'), ('description', 'The path to use "*

 * *               'for the `duckdb.connect` call; either a local fi […]*

```diff
@@ -1,24 +1,64 @@
 {
     "description": "DuckDB loader",
     "docs": "https://hub.meltano.com/loaders/target-duckdb--jwills",
     "label": "DuckDB",
     "logo_url": "https://hub.meltano.com/assets/logos/loaders/duckdb.png",
     "name": "target-duckdb",
     "namespace": "target_duckdb",
-    "pip_url": "target-duckdb~=0.4",
+    "pip_url": "target-duckdb~=0.6",
     "plugin_type": "loaders",
     "repo": "https://github.com/jwills/target-duckdb",
     "settings": [
         {
-            "description": "Path to the local DuckDB file.",
+            "description": "The path to use for the `duckdb.connect` call; either a local file or a MotherDuck connection uri.",
+            "kind": "string",
+            "label": "Connection Path",
+            "name": "path",
+            "placeholder": "/path/to/local/file.duckdb"
+        },
+        {
+            "description": "Alias of `path`.",
             "kind": "string",
             "label": "File Path",
             "name": "filepath",
-            "placeholder": "/path/to/local/duckdb.file"
+            "placeholder": "/path/to/local/file.duckdb",
+            "value": "${MELTANO_PROJECT_ROOT}/output/warehouse.duckdb"
+        },
+        {
+            "description": "The database name to write to; this will be inferred from the path property if it is not specified.",
+            "kind": "string",
+            "label": "Database",
+            "name": "dbname"
+        },
+        {
+            "description": "Alias of `dbname`.",
+            "kind": "string",
+            "label": "Database name",
+            "name": "database"
+        },
+        {
+            "description": "For MotherDuck connections, the auth token to use.",
+            "kind": "password",
+            "label": "Token",
+            "name": "token"
+        },
+        {
+            "description": "The delimiter to use for the CSV files that are used for record imports.",
+            "kind": "string",
+            "label": "Delimiter",
+            "name": "delimiter",
+            "value": ","
+        },
+        {
+            "description": "The quote character to use for the CSV files that are used for record imports.",
+            "kind": "string",
+            "label": "Quote Character",
+            "name": "quotechar",
+            "value": "\""
         },
         {
             "description": "Maximum number of rows in each batch. At the end of each batch, the rows in the batch are loaded into DuckDB.",
             "kind": "integer",
             "label": "Batch Size Rows",
             "name": "batch_size_rows",
             "value": 100000
@@ -30,15 +70,16 @@
             "name": "flush_all_streams",
             "value": false
         },
         {
             "description": "Name of the schema where the tables will be created. If schema_mapping is not defined then every stream sent by the tap is loaded into this schema.",
             "kind": "string",
             "label": "Default Target Schema",
-            "name": "default_target_schema"
+            "name": "default_target_schema",
+            "value": "$MELTANO_EXTRACT__LOAD_SCHEMA"
         },
         {
             "description": "Useful if you want to load multiple streams from one tap to multiple DuckDB schemas.\n\nIf the tap sends the stream_id in <schema_name>-<table_name> format then this option overwrites the default_target_schema value.\n",
             "kind": "object",
             "label": "schema_mapping",
             "name": "schema_mapping"
         },
```

### Comparing `tap_belvo-0.0.1b6/plugins/loaders/target-jsonl--andyh1203.lock` & `tap_belvo-0.0.1b7/plugins/loaders/target-jsonl--andyh1203.lock`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b6/tap_belvo/client.py` & `tap_belvo-0.0.1b7/tap_belvo/client.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b6/tap_belvo/tap.py` & `tap_belvo-0.0.1b7/tap_belvo/tap.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,14 @@
         # TODO(edgarrmondragon): Add tax declarations and tax returns
         # https://github.com/edgarrmondragon/tap-belvo/issues/76
         return [
             links.Links(self),
             links.Institutions(self),
             banking.Accounts(self),
             banking.Transactions(self),
-            banking.Balances(self),
             banking.Owners(self),
             # banking.InvestmentPortfolios(self),  # noqa: ERA001
             # banking.ReceivableTransactions(self),  # noqa: ERA001
             enrichment.Incomes(self),
             enrichment.RecurringExpenses(self),
             enrichment.RiskInsights(self),
             fiscal.Invoices(self),
```

### Comparing `tap_belvo-0.0.1b6/tap_belvo/openapi/BelvoOpenFinanceApiSpec.json` & `tap_belvo-0.0.1b7/tap_belvo/openapi/BelvoOpenFinanceApiSpec.json`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b6/tap_belvo/openapi/__init__.py` & `tap_belvo-0.0.1b7/tap_belvo/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b6/tap_belvo/streams/__init__.py` & `tap_belvo-0.0.1b7/tap_belvo/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b6/tap_belvo/streams/banking.py` & `tap_belvo-0.0.1b7/tap_belvo/streams/banking.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 
 class Accounts(BelvoStream):
     """Accounts stream."""
 
     name = "banking_accounts"
     path = "/api/accounts"
-    primary_keys = ("id",)  # type: ignore[assignment]
+    primary_keys = ("id",)
     replication_key = "created_at"
     openapi_ref = "Account"
 
 
 class Transactions(BelvoStream):
     """Transactions stream."""
 
     name = "banking_transactions"
     path = "/api/transactions"
-    primary_keys = ("id",)  # type: ignore[assignment]
+    primary_keys = ("id",)
     replication_key = "created_at"
     openapi_ref = "Account"
     parent_stream_type = Links
 
     def get_url_params(
         self,
         context: dict[Any, Any] | None,
@@ -50,54 +50,54 @@
         if context is not None:
             params["link"] = context["link_id"]
 
         return params
 
 
 class Balances(BelvoStream):
-    """Balances stream."""
+    """DEPRECATED. Balances stream."""
 
     name = "banking_balances"
     path = "/api/balances"
-    primary_keys = ("id",)  # type: ignore[assignment]
+    primary_keys = ("id",)
     replication_key = "value_date"
     openapi_ref = "Balance"
 
 
 class Owners(BelvoStream):
     """Owners stream."""
 
     name = "banking_owners"
     path = "/api/owners"
-    primary_keys = ("id",)  # type: ignore[assignment]
+    primary_keys = ("id",)
     replication_key = "created_at"
     openapi_ref = "Owner"
 
 
 class InvestmentPortfolios(BelvoStream):
     """Portfolios stream."""
 
     name = "investment_portfolios"
     path = "/investments/portfolios"
-    primary_keys = ("id",)  # type: ignore[assignment]
+    primary_keys = ("id",)
     replication_key = None
     openapi_ref = "InvestmentsPortfolio"
 
 
 class InvestmentTransactions(BelvoStream):
     """Investment transactions stream."""
 
     name = "investment_transactions"
     path = "/investments/transactions"
-    primary_keys = ("id",)  # type: ignore[assignment]
+    primary_keys = ("id",)
     replication_key = "created_at"
     openapi_ref = "InvestmentsInstrumentTransaction"
 
 
 class ReceivableTransactions(BelvoStream):
     """Receivable transactions stream."""
 
     name = "receivable_transactions"
     path = "/receivables/transactions"
-    primary_keys = ("id",)  # type: ignore[assignment]
+    primary_keys = ("id",)
     replication_key = "created_at"
     openapi_ref = "ReceivablesTransaction"
```

### Comparing `tap_belvo-0.0.1b6/tap_belvo/streams/fiscal.py` & `tap_belvo-0.0.1b7/tap_belvo/streams/fiscal.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,61 +6,61 @@
 
 
 class Invoices(BelvoStream):
     """Invoices stream."""
 
     name = "fiscal_invoices"
     path = "/api/invoices"
-    primary_keys = ("id",)  # type: ignore[assignment]
+    primary_keys = ("id",)
     replication_key = "created_at"
     openapi_ref = "InvoiceWithIdSat"
 
 
 class TaxComplianceStatuses(BelvoStream):
     """Tax Compliance Statuses stream."""
 
     name = "fiscal_tax_compliance_statuses"
     path = "/api/tax-compliance-status"
-    primary_keys = ("id",)  # type: ignore[assignment]
+    primary_keys = ("id",)
     replication_key = "created_at"
     openapi_ref = "TaxComplianceStatus"
 
 
 # NOTE: This is stream is in beta and its schema is not yet documented.
 class TaxDeclarations(BelvoStream):
     """Tax Declarations stream."""
 
     name = "fiscal_tax_declarations"
     path = "/api/tax-declarations"
-    primary_keys = ("id",)  # type: ignore[assignment]
+    primary_keys = ("id",)
     replication_key = "created_at"
     openapi_ref = "TaxDeclaration"
 
 
 class TaxRetentions(BelvoStream):
     """Tax Retentions stream."""
 
     name = "fiscal_tax_retentions"
     path = "/api/tax-retentions"
-    primary_keys = ("id",)  # type: ignore[assignment]
+    primary_keys = ("id",)
     replication_key = "created_at"
     openapi_ref = "TaxRetentions"
 
 
 class TaxReturns(BelvoStream):
     """Tax Returns stream."""
 
     name = "fiscal_tax_returns"
     path = "/api/tax-returns"
-    primary_keys = ("id",)  # type: ignore[assignment]
+    primary_keys = ("id",)
     replication_key = "created_at"
     openapi_ref = "TaxReturn"
 
 
 class TaxStatuses(BelvoStream):
     """Tax Statuses stream."""
 
     name = "fiscal_tax_statuses"
     path = "/api/tax-status"
-    primary_keys = ("id",)  # type: ignore[assignment]
+    primary_keys = ("id",)
     replication_key = "created_at"
     openapi_ref = "TaxStatusSat"
```

### Comparing `tap_belvo-0.0.1b6/tap_belvo/streams/links.py` & `tap_belvo-0.0.1b7/tap_belvo/streams/links.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class Links(BelvoStream):
     """Links stream."""
 
     name = "links_links"
     path = "/api/links"
-    primary_keys = ("id",)  # type: ignore[assignment]
+    primary_keys = ("id",)
     replication_key = "created_at"
     openapi_ref = "Link"
 
     def get_child_context(
         self,
         record: dict[str, t.Any],
         context: dict[t.Any, t.Any] | None,  # noqa: ARG002
@@ -34,10 +34,10 @@
 
 
 class Institutions(BelvoStream):
     """Institutions stream."""
 
     name = "links_institutions"
     path = "/api/institutions"
-    primary_keys = ("id",)  # type: ignore[assignment]
+    primary_keys = ("id",)
     replication_key = None
     openapi_ref = "Institution"
```

### Comparing `tap_belvo-0.0.1b6/tests/test_core.py` & `tap_belvo-0.0.1b7/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b6/.gitignore` & `tap_belvo-0.0.1b7/.gitignore`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b6/LICENSE` & `tap_belvo-0.0.1b7/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_belvo-0.0.1b6/README.md` & `tap_belvo-0.0.1b7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 ```
 
 ### Create and Run Tests
 
 Run integration tests:
 
 ```bash
-hatch run tests:integration
+hatch run test:integration
 ```
 
 You can also test the `tap-belvo` CLI interface directly:
 
 ```bash
 hatch run sync:console -- --about --format=json
 ```
```

### Comparing `tap_belvo-0.0.1b6/pyproject.toml` & `tap_belvo-0.0.1b7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -26,43 +26,39 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  'importlib_resources; python_version < "3.9"',
-  'pendulum~=3.0.0b1; python_version >= "3.12"',
+  'importlib-resources; python_version < "3.9"',
   "requests",
   "requests-cache==1.*",
-  "singer-sdk~=0.34.0",
+  "singer-sdk~=0.37.0",
 ]
-[project.optional-dependencies]
-testing = [
+optional-dependencies.testing = [
   "deptry>=0.12",
   "pytest>=7.4",
-  "singer-sdk[testing]~=0.34.0",
+  "singer-sdk[testing]~=0.37.0",
 ]
-typing = [
+optional-dependencies.typing = [
   "mypy",
   "types-requests",
 ]
-[project.urls]
-Documentation = "https://github.com/edgarrmondragon/tap-belvo#readme"
-Homepage = "https://github.com/edgarrmondragon/tap-belvo"
-Source = "https://github.com/edgarrmondragon/tap-belvo"
-[project.scripts]
-"tap-belvo" = "tap_belvo.tap:TapBelvo.cli"
+urls.Documentation = "https://github.com/edgarrmondragon/tap-belvo#readme"
+urls.Homepage = "https://github.com/edgarrmondragon/tap-belvo"
+urls.Source = "https://github.com/edgarrmondragon/tap-belvo"
+scripts."tap-belvo" = "tap_belvo.tap:TapBelvo.cli"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.envs.sync.scripts]
-console = "tap-belvo {args:tests}"
-jsonl = "tap-belvo {args:tests} > tap-belvo.jsonl"
+console = "tap-belvo {args}"
+jsonl = "tap-belvo {args} > tap-belvo.jsonl"
 
 [tool.hatch.envs.test]
 features = ["testing"]
 [tool.hatch.envs.test.scripts]
 integration = "pytest {args:tests}"
 dependencies = "deptry ."
 
@@ -70,15 +66,14 @@
 features = ["testing", "typing"]
 [tool.hatch.envs.typing.scripts]
 check = "mypy --strict {args:tap_belvo tests}"
 
 [tool.ruff]
 line-length = 88
 src = ["tap_belvo", "tests"]
-target-version = "py38"
 
 [tool.ruff.lint]
 ignore = [
   "ANN101",  # missing-type-self
   "DJ",      # flake8-django
   "FIX002",  # line-contains-todo
   "COM812",  # missing-trailing-comma
@@ -101,24 +96,23 @@
 known-first-party = ["tap_belvo"]
 required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.deptry.package_module_name_map]
+importlib-resources = "importlib_resources"
 mypy = "mypy"
-types-requests = "types_requests"
+types-requests = "requests"
 
 [tool.deptry.per_rule_ignores]
 DEP002 = [
   "deptry",
   "mypy",
-  "pendulum",
   "pytest",
-  "types-requests",
 ]
 
 [tool.pytest.ini_options]
 addopts = "-vvv"
 
 [tool.mypy]
 python_version = "3.11"
```

### Comparing `tap_belvo-0.0.1b6/PKG-INFO` & `tap_belvo-0.0.1b7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tap-belvo
-Version: 0.0.1b6
+Version: 0.0.1b7
 Summary: `tap-belvo` is a Singer tap for Belvo, built with the Meltano SDK for Singer Taps.
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-belvo#readme
 Project-URL: Homepage, https://github.com/edgarrmondragon/tap-belvo
 Project-URL: Source, https://github.com/edgarrmondragon/tap-belvo
 Author-email: Edgar Ramírez-Mondragón <edgarrm358@gmail.com>
 Maintainer-email: Edgar Ramírez-Mondragón <edgarrm358@gmail.com>
 License-Expression: Apache-2.0
@@ -14,22 +14,21 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: importlib-resources; python_version < '3.9'
-Requires-Dist: pendulum~=3.0.0b1; python_version >= '3.12'
 Requires-Dist: requests
 Requires-Dist: requests-cache==1.*
-Requires-Dist: singer-sdk~=0.34.0
+Requires-Dist: singer-sdk~=0.37.0
 Provides-Extra: testing
 Requires-Dist: deptry>=0.12; extra == 'testing'
 Requires-Dist: pytest>=7.4; extra == 'testing'
-Requires-Dist: singer-sdk[testing]~=0.34.0; extra == 'testing'
+Requires-Dist: singer-sdk[testing]~=0.37.0; extra == 'testing'
 Provides-Extra: typing
 Requires-Dist: mypy; extra == 'typing'
 Requires-Dist: types-requests; extra == 'typing'
 Description-Content-Type: text/markdown
 
 # `tap-belvo`
 
@@ -86,15 +85,15 @@
 ```
 
 ### Create and Run Tests
 
 Run integration tests:
 
 ```bash
-hatch run tests:integration
+hatch run test:integration
 ```
 
 You can also test the `tap-belvo` CLI interface directly:
 
 ```bash
 hatch run sync:console -- --about --format=json
 ```
```

