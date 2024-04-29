# Comparing `tmp/stac_api_validator-0.6.1.tar.gz` & `tmp/stac_api_validator-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_api_validator-0.6.1.tar", max compression
+gzip compressed data, was "stac_api_validator-0.6.2.tar", max compression
```

## Comparing `stac_api_validator-0.6.1.tar` & `stac_api_validator-0.6.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11342 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/LICENSE
--rw-r--r--   0        0        0     9879 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/README.md
--rw-r--r--   0        0        0     2450 2023-04-27 16:00:29.129889 stac_api_validator-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       26 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/src/stac_api_validator/__init__.py
--rw-r--r--   0        0        0     6329 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/src/stac_api_validator/__main__.py
--rw-r--r--   0        0        0     9583 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/src/stac_api_validator/filters.py
--rw-r--r--   0        0        0     1303 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/src/stac_api_validator/geometries.py
--rw-r--r--   0        0        0        0 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/src/stac_api_validator/py.typed
--rw-r--r--   0        0        0   130272 2023-04-27 16:00:04.245300 stac_api_validator-0.6.1/src/stac_api_validator/validations.py
--rw-r--r--   0        0        0    11163 1970-01-01 00:00:00.000000 stac_api_validator-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11342 2024-04-29 16:11:52.043551 stac_api_validator-0.6.2/LICENSE
+-rw-r--r--   0        0        0     9879 2024-04-29 16:11:52.043551 stac_api_validator-0.6.2/README.md
+-rw-r--r--   0        0        0     2349 2024-04-29 16:12:05.423692 stac_api_validator-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0       26 2024-04-29 16:11:52.043551 stac_api_validator-0.6.2/src/stac_api_validator/__init__.py
+-rw-r--r--   0        0        0     6330 2024-04-29 16:11:52.043551 stac_api_validator-0.6.2/src/stac_api_validator/__main__.py
+-rw-r--r--   0        0        0     9583 2024-04-29 16:11:52.043551 stac_api_validator-0.6.2/src/stac_api_validator/filters.py
+-rw-r--r--   0        0        0     1303 2024-04-29 16:11:52.043551 stac_api_validator-0.6.2/src/stac_api_validator/geometries.py
+-rw-r--r--   0        0        0        0 2024-04-29 16:11:52.043551 stac_api_validator-0.6.2/src/stac_api_validator/py.typed
+-rw-r--r--   0        0        0   130279 2024-04-29 16:11:52.043551 stac_api_validator-0.6.2/src/stac_api_validator/validations.py
+-rw-r--r--   0        0        0    11170 1970-01-01 00:00:00.000000 stac_api_validator-0.6.2/PKG-INFO
```

### Comparing `stac_api_validator-0.6.1/LICENSE` & `stac_api_validator-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_api_validator-0.6.1/README.md` & `stac_api_validator-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `stac_api_validator-0.6.1/pyproject.toml` & `stac_api_validator-0.6.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 [tool.poetry]
 name = "stac-api-validator"
-version = "0.6.1"
+version = "0.6.2"
 description = "STAC API Validator"
 authors = ["Phil Varner <phil@philvarner.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/stac-utils/stac-api-validator"
 repository = "https://github.com/stac-utils/stac-api-validator"
 documentation = "https://stac-api-validator.readthedocs.io"
-classifiers = [
-    "Development Status :: 4 - Beta",
-]
+classifiers = ["Development Status :: 4 - Beta"]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/stac-utils/stac-api-validator/releases"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.3"
-certifi = "^2022.12.07"  # CVE-2022-23491: https://github.com/certifi/python-certifi/security/advisories/GHSA-43fp-rhv2-5gv8
-pystac-client = "^0.6.1"
-requests = "^2.28.1"
-pystac = {extras = ["orjson"], version = "^1.7.1"}
+certifi = "^2024.2.2"
+pystac-client = "^0.7.5"
+requests = "^2.31.0"
+pystac = { extras = ["orjson"], version = "^1.8.3" }
 jsonschema = "^4.16.0"
-PyYAML = "6.0"
-Shapely = "1.8.4"
+PyYAML = "^6.0.1"
+Shapely = ">=1.8.4"
 more_itertools = "^8.14.0"
 stac-check = "^1.3.1"
 stac-validator = "^3.2.0"
 deepdiff = "^6.2.3"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=22.8.0"
-coverage = {extras = ["toml"], version = ">=6.2"}
+coverage = { extras = ["toml"], version = ">=6.2" }
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
-#flake8-bandit = ">=2.1.2"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = ">=1.6.0"
 flake8-rst-docstrings = ">=0.2.5"
 furo = ">=2021.11.12"
 isort = ">=5.10.1"
 mypy = ">=0.981"
 pep8-naming = ">=0.12.1"
@@ -49,31 +46,31 @@
 pytest = ">=6.2.5"
 pyupgrade = ">=2.29.1"
 safety = ">=1.10.3"
 sphinx = ">=4.3.2"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-click = ">=3.0.2"
 typeguard = ">=2.13.3"
-xdoctest = {extras = ["colors"], version = ">=0.15.10"}
-myst-parser = {version = ">=0.16.1"}
+xdoctest = { extras = ["colors"], version = ">=0.15.10" }
+myst-parser = { version = ">=0.16.1" }
 
 [tool.poetry.scripts]
 stac-api-validator = "stac_api_validator.__main__:main"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
 
 [tool.coverage.run]
 branch = true
 source = ["stac_api_validator", "tests"]
 
 [tool.coverage.report]
 show_missing = true
-fail_under = 10 # todo: get back to 85
+fail_under = 10     # todo: get back to 85
 
 [tool.isort]
 profile = "black"
 force_single_line = true
 lines_after_imports = 2
 
 [tool.mypy]
@@ -82,13 +79,18 @@
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 #ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
-module = ["shapely.geometry", "stac_check.lint", "stac_validator.stac_validator", "deepdiff"]
+module = [
+    "shapely.geometry",
+    "stac_check.lint",
+    "stac_validator.stac_validator",
+    "deepdiff",
+]
 ignore_missing_imports = true
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `stac_api_validator-0.6.1/src/stac_api_validator/__main__.py` & `stac_api_validator-0.6.2/src/stac_api_validator/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Command-line interface."""
+
 import logging
 import sys
 import traceback
 from typing import List
 from typing import Optional
 
 import click
```

### Comparing `stac_api_validator-0.6.1/src/stac_api_validator/filters.py` & `stac_api_validator-0.6.2/src/stac_api_validator/filters.py`

 * *Files identical despite different names*

### Comparing `stac_api_validator-0.6.1/src/stac_api_validator/geometries.py` & `stac_api_validator-0.6.2/src/stac_api_validator/geometries.py`

 * *Files identical despite different names*

### Comparing `stac_api_validator-0.6.1/src/stac_api_validator/validations.py` & `stac_api_validator-0.6.2/src/stac_api_validator/validations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Validations module."""
+
 import copy
 import itertools
 import json
 import logging
 import re
 import time
 from dataclasses import dataclass
@@ -443,15 +444,15 @@
             "This field is required as of STAC 1.0.0",
         )
     else:
         if any(
             x
             for x in conforms_to
             if re.match(
-                r"https://api\.stacspec\.org/v1\.0\.0.*/(core|item-search|ogcapi-features|collections)",
+                r"^https://api\.stacspec\.org/v1\.0\.0.*/(core|item-search|ogcapi-features|collections)$",
                 x,
             )
             and not x.startswith(LATEST_STAC_API_FOUNDATION_VERSION)
         ):
             warnings += f"STAC API Specification {LATEST_STAC_API_FOUNDATION_VERSION} is the latest version, but API advertises an older version or older versions."
 
     if not supports(conforms_to, cc_core_regex):
@@ -741,21 +742,21 @@
     if links is None:
         errors += "/ : 'links' attribute missing"
 
     if not (root := link_by_rel(links, "root")):
         errors += "/ : Link[rel=root] must exist"
     else:
         if not is_json_type(root.get("type")):
-            errors += f"/ : Link[rel=root] type is not application/geo+json, instead {root.get('type')}"
+            errors += f"/ : Link[rel=root] type is not application/json, instead {root.get('type')}"
 
     if not (_self := link_by_rel(links, "self")):
         warnings += "/ : Link[rel=self] must exist"
     else:
         if not is_json_type(_self.get("type")):
-            errors += f"/ : Link[rel=self] type is not application/geo+json, instead {_self.get('type')}"
+            errors += f"/ : Link[rel=self] type is not application/json, instead {_self.get('type')}"
 
     if not (service_desc := link_by_rel(links, "service-desc")):
         errors += "/ : Link[rel=service-desc] must exist"
     else:
         if not (service_desc_type := service_desc.get("type")):
             errors += "/ : Link[rel=service-desc] must have a type defined"
         else:
@@ -2850,15 +2851,15 @@
 
     if Method.POST in methods:
         _, item_collection, _ = retrieve(
             Method.POST,
             search_url,
             errors,
             Context.ITEM_SEARCH,
-            body={"collections": [collection], "intersects": geometry},
+            body={"collections": [collection], "intersects": json.loads(geometry)},
             r_session=r_session,
         )
         if not item_collection or not item_collection.get("features"):
             errors += f"[{Context.ITEM_SEARCH}] POST Search result for intersects={geometry} returned no results"
         else:
             for item in item_collection.get("features", []):
                 if not intersects_shape.intersects(shape(item.get("geometry"))):
```

### Comparing `stac_api_validator-0.6.1/PKG-INFO` & `stac_api_validator-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: stac-api-validator
-Version: 0.6.1
+Version: 0.6.2
 Summary: STAC API Validator
 Home-page: https://github.com/stac-utils/stac-api-validator
 License: Apache-2.0
 Author: Phil Varner
 Author-email: phil@philvarner.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: PyYAML (==6.0)
-Requires-Dist: Shapely (==1.8.4)
-Requires-Dist: certifi (>=2022.12.07,<2023.0.0)
+Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
+Requires-Dist: Shapely (>=1.8.4)
+Requires-Dist: certifi (>=2024.2.2,<2025.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: deepdiff (>=6.2.3,<7.0.0)
 Requires-Dist: jsonschema (>=4.16.0,<5.0.0)
 Requires-Dist: more_itertools (>=8.14.0,<9.0.0)
-Requires-Dist: pystac-client (>=0.6.1,<0.7.0)
-Requires-Dist: pystac[orjson] (>=1.7.1,<2.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: pystac-client (>=0.7.5,<0.8.0)
+Requires-Dist: pystac[orjson] (>=1.8.3,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: stac-check (>=1.3.1,<2.0.0)
 Requires-Dist: stac-validator (>=3.2.0,<4.0.0)
 Project-URL: Changelog, https://github.com/stac-utils/stac-api-validator/releases
 Project-URL: Documentation, https://stac-api-validator.readthedocs.io
 Project-URL: Repository, https://github.com/stac-utils/stac-api-validator
 Description-Content-Type: text/markdown
```

