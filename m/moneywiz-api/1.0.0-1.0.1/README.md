# Comparing `tmp/moneywiz_api-1.0.0.tar.gz` & `tmp/moneywiz_api-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moneywiz_api-1.0.0.tar", last modified: Fri Apr 26 16:46:41 2024, max compression
+gzip compressed data, was "moneywiz_api-1.0.1.tar", last modified: Mon Apr 29 21:20:00 2024, max compression
```

## Comparing `moneywiz_api-1.0.0.tar` & `moneywiz_api-1.0.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.599223 moneywiz_api-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-26 16:46:41.599223 moneywiz_api-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 16:46:41.599223 moneywiz_api-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.595223 moneywiz_api-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.595223 moneywiz_api-1.0.0/src/moneywiz_api/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.595223 moneywiz_api-1.0.0/src/moneywiz_api/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/cli/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/database_accessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.595223 moneywiz_api-1.0.0/src/moneywiz_api/managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/account_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/category_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/investment_holding_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/payee_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/record_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/tag_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/managers/transaction_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.599223 moneywiz_api-1.0.0/src/moneywiz_api/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/account.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/investment_holding.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/payee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/raw_data_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/record.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/model/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/moneywiz_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/src/moneywiz_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.599223 moneywiz_api-1.0.0/src/moneywiz_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-26 16:46:41.000000 moneywiz_api-1.0.0/src/moneywiz_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-26 16:46:41.000000 moneywiz_api-1.0.0/src/moneywiz_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 16:46:41.000000 moneywiz_api-1.0.0/src/moneywiz_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-26 16:46:41.000000 moneywiz_api-1.0.0/src/moneywiz_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 16:46:41.000000 moneywiz_api-1.0.0/src/moneywiz_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 16:46:41.000000 moneywiz_api-1.0.0/src/moneywiz_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 16:46:41.599223 moneywiz_api-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-26 16:46:37.000000 moneywiz_api-1.0.0/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.426801 moneywiz_api-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-29 21:20:00.426801 moneywiz_api-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 21:20:00.426801 moneywiz_api-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.422801 moneywiz_api-1.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.422801 moneywiz_api-1.0.1/src/moneywiz_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.422801 moneywiz_api-1.0.1/src/moneywiz_api/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/cli/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/database_accessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.426801 moneywiz_api-1.0.1/src/moneywiz_api/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/account_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/category_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/investment_holding_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/payee_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/record_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/tag_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/managers/transaction_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.426801 moneywiz_api-1.0.1/src/moneywiz_api/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/investment_holding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/payee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/raw_data_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/model/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/moneywiz_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/src/moneywiz_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.426801 moneywiz_api-1.0.1/src/moneywiz_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-29 21:20:00.000000 moneywiz_api-1.0.1/src/moneywiz_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-29 21:20:00.000000 moneywiz_api-1.0.1/src/moneywiz_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 21:20:00.000000 moneywiz_api-1.0.1/src/moneywiz_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-29 21:20:00.000000 moneywiz_api-1.0.1/src/moneywiz_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 21:20:00.000000 moneywiz_api-1.0.1/src/moneywiz_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 21:20:00.000000 moneywiz_api-1.0.1/src/moneywiz_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:20:00.426801 moneywiz_api-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-29 21:19:56.000000 moneywiz_api-1.0.1/tests/test_config.py
```

### Comparing `moneywiz_api-1.0.0/LICENSE` & `moneywiz_api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/PKG-INFO` & `moneywiz_api-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: moneywiz-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python api to access moneywiz sqlite database
 Author-email: iLeoDo <iLeoDo@gmail.com>
 Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
+Requires-Dist: pytest
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: moneywiz-api Version: 1.0.0 Summary: A Python api
+Metadata-Version: 2.1 Name: moneywiz-api Version: 1.0.1 Summary: A Python api
 to access moneywiz sqlite database Author-email: iLeoDo
 gmail.com> Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: pandas Provides-Extra: dev Requires-Dist: pytest; extra
-== "dev" Requires-Dist: pylint; extra == "dev" Requires-Dist: mypy; extra ==
-"dev" Requires-Dist: black; extra == "dev" Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev" # MoneyWiz-API ![Static Badge](https://
-img.shields.io/badge/Python-3-blue?style=flat&logo=Python) ![PyPI](https://
-img.shields.io/pypi/v/moneywiz-api) _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]A Python API to access
-MoneyWiz Sqlite database. ## Get Started ```bash pip install moneywiz-api ```
-```python from moneywiz_api import MoneywizApi moneywizApi = MoneywizApi("")
-( accessor, account_manager, payee_manager, category_manager,
-transaction_manager, investment_holding_manager, ) = ( moneywizApi.accessor,
+LICENSE Requires-Dist: pandas Requires-Dist: pytest Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev" Requires-Dist: pylint; extra == "dev"
+Requires-Dist: mypy; extra == "dev" Requires-Dist: black; extra == "dev"
+Requires-Dist: build; extra == "dev" Requires-Dist: twine; extra == "dev" #
+MoneyWiz-API ![Static Badge](https://img.shields.io/badge/Python-3-
+blue?style=flat&logo=Python) ![PyPI](https://img.shields.io/pypi/v/moneywiz-
+api) _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]A Python API to access MoneyWiz Sqlite database. ## Get
+Started ```bash pip install moneywiz-api ``` ```python from moneywiz_api import
+MoneywizApi moneywizApi = MoneywizApi("") ( accessor, account_manager,
+payee_manager, category_manager, transaction_manager,
+investment_holding_manager, ) = ( moneywizApi.accessor,
 moneywizApi.account_manager, moneywizApi.payee_manager,
 moneywizApi.category_manager, moneywizApi.transaction_manager,
 moneywizApi.investment_holding_manager, ) record = accessor.get_record
 (record_id) print(record) ``` It also offers a interactive shell `moneywiz-
 cli`. ## Contribution This project is in very early stage, all contributions
 are welcomed!
```

### Comparing `moneywiz_api-1.0.0/README.md` & `moneywiz_api-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/pyproject.toml` & `moneywiz_api-1.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "moneywiz-api"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name="iLeoDo", email="iLeoDo@gmail.com" },
 ]
 description = "A Python api to access moneywiz sqlite database"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/cli/cli.py` & `moneywiz_api-1.0.1/src/moneywiz_api/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,33 +61,36 @@
     (
         accessor,
         account_manager,
         payee_manager,
         category_manager,
         transaction_manager,
         investment_holding_manager,
+        tag_manager,
     ) = (
         moneywiz_api.accessor,
         moneywiz_api.account_manager,
         moneywiz_api.payee_manager,
         moneywiz_api.category_manager,
         moneywiz_api.transaction_manager,
         moneywiz_api.investment_holding_manager,
+        moneywiz_api.tag_manager,
     )
 
     helper = ShellHelper(moneywiz_api)
 
     names: Dict[str, str] = {
         f"{moneywiz_api=}".split("=")[0]: "MoneyWiz API",
         f"{accessor=}".split("=")[0]: "MoneyWiz Database Accessor",
         f"{account_manager=}".split("=")[0]: "Account Manager",
         f"{payee_manager=}".split("=")[0]: "Payee Manager",
         f"{category_manager=}".split("=")[0]: "Category Manageer",
         f"{transaction_manager=}".split("=")[0]: "Transaction Manager",
         f"{investment_holding_manager=}".split("=")[0]: "Investment Holding Manager",
+        f"{tag_manager=}".split("=")[0]: "Tag Manager",
         f"{helper=}".split("=")[0]: "Shell Helper",
     }
 
     banner: List[str] = (
         f"Read-only MoneyWiz Shell on {db_file_path}",
         "",
         "Avaliable components:",
```

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/cli/helpers.py` & `moneywiz_api-1.0.1/src/moneywiz_api/cli/helpers.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/database_accessor.py` & `moneywiz_api-1.0.1/src/moneywiz_api/database_accessor.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/managers/account_manager.py` & `moneywiz_api-1.0.1/src/moneywiz_api/managers/account_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/managers/category_manager.py` & `moneywiz_api-1.0.1/src/moneywiz_api/managers/category_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/managers/investment_holding_manager.py` & `moneywiz_api-1.0.1/src/moneywiz_api/managers/investment_holding_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/managers/record_manager.py` & `moneywiz_api-1.0.1/src/moneywiz_api/managers/record_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/managers/transaction_manager.py` & `moneywiz_api-1.0.1/src/moneywiz_api/managers/transaction_manager.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/model/__init__.py` & `moneywiz_api-1.0.1/src/moneywiz_api/model/__init__.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/model/account.py` & `moneywiz_api-1.0.1/src/moneywiz_api/model/account.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/model/category.py` & `moneywiz_api-1.0.1/src/moneywiz_api/model/category.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/model/investment_holding.py` & `moneywiz_api-1.0.1/src/moneywiz_api/model/investment_holding.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/model/raw_data_handler.py` & `moneywiz_api-1.0.1/src/moneywiz_api/model/raw_data_handler.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/model/record.py` & `moneywiz_api-1.0.1/src/moneywiz_api/model/record.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/model/transaction.py` & `moneywiz_api-1.0.1/src/moneywiz_api/model/transaction.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api/moneywiz_api.py` & `moneywiz_api-1.0.1/src/moneywiz_api/moneywiz_api.py`

 * *Files identical despite different names*

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api.egg-info/PKG-INFO` & `moneywiz_api-1.0.1/src/moneywiz_api.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: moneywiz-api
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python api to access moneywiz sqlite database
 Author-email: iLeoDo <iLeoDo@gmail.com>
 Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
+Requires-Dist: pytest
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: black; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: moneywiz-api Version: 1.0.0 Summary: A Python api
+Metadata-Version: 2.1 Name: moneywiz-api Version: 1.0.1 Summary: A Python api
 to access moneywiz sqlite database Author-email: iLeoDo
 gmail.com> Project-URL: Homepage, https://github.com/ileodo/moneywiz-api
 Project-URL: Bug Tracker, https://github.com/ileodo/moneywiz-api/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: pandas Provides-Extra: dev Requires-Dist: pytest; extra
-== "dev" Requires-Dist: pylint; extra == "dev" Requires-Dist: mypy; extra ==
-"dev" Requires-Dist: black; extra == "dev" Requires-Dist: build; extra == "dev"
-Requires-Dist: twine; extra == "dev" # MoneyWiz-API ![Static Badge](https://
-img.shields.io/badge/Python-3-blue?style=flat&logo=Python) ![PyPI](https://
-img.shields.io/pypi/v/moneywiz-api) _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]A Python API to access
-MoneyWiz Sqlite database. ## Get Started ```bash pip install moneywiz-api ```
-```python from moneywiz_api import MoneywizApi moneywizApi = MoneywizApi("")
-( accessor, account_manager, payee_manager, category_manager,
-transaction_manager, investment_holding_manager, ) = ( moneywizApi.accessor,
+LICENSE Requires-Dist: pandas Requires-Dist: pytest Provides-Extra: dev
+Requires-Dist: pytest; extra == "dev" Requires-Dist: pylint; extra == "dev"
+Requires-Dist: mypy; extra == "dev" Requires-Dist: black; extra == "dev"
+Requires-Dist: build; extra == "dev" Requires-Dist: twine; extra == "dev" #
+MoneyWiz-API ![Static Badge](https://img.shields.io/badge/Python-3-
+blue?style=flat&logo=Python) ![PyPI](https://img.shields.io/pypi/v/moneywiz-
+api) _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]A Python API to access MoneyWiz Sqlite database. ## Get
+Started ```bash pip install moneywiz-api ``` ```python from moneywiz_api import
+MoneywizApi moneywizApi = MoneywizApi("") ( accessor, account_manager,
+payee_manager, category_manager, transaction_manager,
+investment_holding_manager, ) = ( moneywizApi.accessor,
 moneywizApi.account_manager, moneywizApi.payee_manager,
 moneywizApi.category_manager, moneywizApi.transaction_manager,
 moneywizApi.investment_holding_manager, ) record = accessor.get_record
 (record_id) print(record) ``` It also offers a interactive shell `moneywiz-
 cli`. ## Contribution This project is in very early stage, all contributions
 are welcomed!
```

### Comparing `moneywiz_api-1.0.0/src/moneywiz_api.egg-info/SOURCES.txt` & `moneywiz_api-1.0.1/src/moneywiz_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

