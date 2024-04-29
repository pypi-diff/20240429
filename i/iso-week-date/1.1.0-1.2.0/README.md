# Comparing `tmp/iso_week_date-1.1.0.tar.gz` & `tmp/iso_week_date-1.2.0.tar.gz`

## Comparing `iso_week_date-1.1.0.tar` & `iso_week_date-1.2.0.tar`

### file list

```diff
@@ -1,49 +1,16 @@
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/Makefile
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/mkdocs.yaml
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/.github/dependabot.yaml
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/.github/workflows/check-typos.yaml
--rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/.github/workflows/deploy-docs.yaml
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/.github/workflows/pre-commit-update.yaml
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/.github/workflows/pull-request.yaml
--rw-r--r--   0        0        0     3186 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/contribute.md
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/index.md
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/installation.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/api/baseisoweek.md
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/api/isoweek.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/api/isoweekdate.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/api/mixins.md
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/api/pandas.md
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/api/polars.md
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/img/coverage.svg
--rw-r--r--   0        0        0    11873 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/img/interrogate-shield.svg
--rw-r--r--   0        0        0    35238 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/img/iso-week-date-logo.png
--rw-r--r--   0        0        0     5398 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/img/iso-week-date-logo.svg
--rw-r--r--   0        0        0     4409 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/user-guide/dataframe-modules.md
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/user-guide/features.md
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/user-guide/internals.md
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/user-guide/pydantic.md
--rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/docs/user-guide/quickstart.md
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/iso_week_date/__init__.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/iso_week_date/_patterns.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/iso_week_date/_utils.py
--rw-r--r--   0        0        0     9472 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/iso_week_date/base.py
--rw-r--r--   0        0        0    14494 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/iso_week_date/isoweek.py
--rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/iso_week_date/isoweekdate.py
--rw-r--r--   0        0        0    13908 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/iso_week_date/mixin.py
--rw-r--r--   0        0        0    17251 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/iso_week_date/pandas_utils.py
--rw-r--r--   0        0        0    17326 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/iso_week_date/polars_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/iso_week_date/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/tests/base_test.py
--rw-r--r--   0        0        0     7673 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/tests/isoweek_test.py
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/tests/isoweekdate_test.py
--rw-r--r--   0        0        0     5991 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/tests/mixin_test.py
--rw-r--r--   0        0        0     7727 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/tests/pandas_utils_test.py
--rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/tests/polars_utils_test.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/LICENSE
--rw-r--r--   0        0        0     5794 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/README.md
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     8955 2020-02-02 00:00:00.000000 iso_week_date-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/__init__.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/_patterns.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/_utils.py
+-rw-r--r--   0        0        0     9472 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/base.py
+-rw-r--r--   0        0        0    14494 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/isoweek.py
+-rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/isoweekdate.py
+-rw-r--r--   0        0        0    13908 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/mixin.py
+-rw-r--r--   0        0        0    17271 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/pandas_utils.py
+-rw-r--r--   0        0        0    17344 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/polars_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/py.typed
+-rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/iso_week_date/pydantic.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5886 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/README.md
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     9828 2020-02-02 00:00:00.000000 iso_week_date-1.2.0/PKG-INFO
```

### Comparing `iso_week_date-1.1.0/iso_week_date/_patterns.py` & `iso_week_date-1.2.0/iso_week_date/_patterns.py`

 * *Files identical despite different names*

### Comparing `iso_week_date-1.1.0/iso_week_date/_utils.py` & `iso_week_date-1.2.0/iso_week_date/_utils.py`

 * *Files identical despite different names*

### Comparing `iso_week_date-1.1.0/iso_week_date/base.py` & `iso_week_date-1.2.0/iso_week_date/base.py`

 * *Files identical despite different names*

### Comparing `iso_week_date-1.1.0/iso_week_date/isoweek.py` & `iso_week_date-1.2.0/iso_week_date/isoweek.py`

 * *Files identical despite different names*

### Comparing `iso_week_date-1.1.0/iso_week_date/isoweekdate.py` & `iso_week_date-1.2.0/iso_week_date/isoweekdate.py`

 * *Files identical despite different names*

### Comparing `iso_week_date-1.1.0/iso_week_date/mixin.py` & `iso_week_date-1.2.0/iso_week_date/mixin.py`

 * *Files identical despite different names*

### Comparing `iso_week_date-1.1.0/iso_week_date/pandas_utils.py` & `iso_week_date-1.2.0/iso_week_date/pandas_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     from typing_extensions import Self  # pragma: no cover
 
 try:
     import pandas as pd
     from pandas.api.types import is_datetime64_any_dtype as is_datetime
 except ImportError:  # pragma: no cover
     raise ImportError(
-        "pandas is required for this module, install it with `pip install pandas`"
-        " or `pip install iso-week-date[pandas]`"
+        "pandas is required for this module, install it with `python -m pip install pandas`"
+        " or `python -m pip install iso-week-date[pandas]`"
     )
 
 
 def _datetime_to_format(
     series: pd.Series,
     offset: Union[pd.Timedelta, int],
     _format: str,
```

### Comparing `iso_week_date-1.1.0/iso_week_date/polars_utils.py` & `iso_week_date-1.2.0/iso_week_date/polars_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 else:
     from typing_extensions import Self  # pragma: no cover
 
 try:
     import polars as pl
 except ImportError:  # pragma: no cover
     raise ImportError(
-        "polars>=0.18.0 is required for this module, install it with "
-        "`pip install polars --upgrade` or `pip install iso-week-date[polars]`"
+        "polars>=0.18.0 is required for this module, install it with `python -m pip install polars>=0.18.0` "
+        "or `python -m pip install iso-week-date[polars]`"
     )
 
 T = TypeVar("T", pl.Series, pl.Expr)
 
 
 def _datetime_to_format(
     series: T,
```

### Comparing `iso_week_date-1.1.0/.gitignore` & `iso_week_date-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `iso_week_date-1.1.0/LICENSE` & `iso_week_date-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iso_week_date-1.1.0/README.md` & `iso_week_date-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-<img src="docs/img/iso-week-date-logo.svg" width=185 height=185 align="right">
+# ISO Week Date
 
-![](https://img.shields.io/github/license/FBruzzesi/iso-week-date)
-<img src ="docs/img/interrogate-shield.svg">
+![license-shield](https://img.shields.io/github/license/FBruzzesi/iso-week-date)
+![interrogate-shield](docs/img/interrogate-shield.svg)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-<img src="docs/img/coverage.svg">
-<img src="https://img.shields.io/pypi/pyversions/iso-week-date">
+![coverage](docs/img/coverage.svg)
+![pypi-versions](https://img.shields.io/pypi/pyversions/iso-week-date)
 
-# ISO Week Date
+<img src="docs/img/iso-week-date-logo.svg" width=160 height=160 align="right">
 
 **iso-week-date** is a toolkit to work with strings representing [ISO Week date](https://en.wikipedia.org/wiki/ISO_week_date) in two formats, namely:
 
-- Week format **YYYY-WNN** (corresponding to the date format **%Y-W%V**)
-- Week date format **YYYY-WNN-D** (corresponding to the date format **%Y-W%V-%u**)
+- Week format **YYYY-WNN** (date format **%Y-W%V**)
+- Week date format **YYYY-WNN-D** (date format **%Y-W%V-%u**)
 
-(where YYYY represents the year, W is a literal, NN represents the week number, and D represents the day of the week)
+where _YYYY_ represents the year, _W_ is a literal, _NN_ represents the week number, and _D_ represents the day of the week.
 
 In a nutshell it provides:
 
-- [`IsoWeek`](https://fbruzzesi.github.io/iso-week-date/api/isoweek/) and [`IsoWeekDate`](https://fbruzzesi.github.io/iso-week-date/api/isoweekdate/) classes implementing a series of methods to work with ISO Week (Date) formats and avoiding the pitfalls of going back and forth between string, date and datetime python objects
-- [pandas](https://fbruzzesi.github.io/iso-week-date/api/pandas/) and [polars](https://fbruzzesi.github.io/iso-week-date/api/polars/) functionalities to work with series of ISO Week dates
+- [`IsoWeek`](https://fbruzzesi.github.io/iso-week-date/api/isoweek/) and [`IsoWeekDate`](https://fbruzzesi.github.io/iso-week-date/api/isoweekdate/) classes that implement a series of methods to work with ISO Week (Date) formats directly, avoiding the pitfalls of going back and forth between string, date and datetime python objects.
+- [pandas](https://fbruzzesi.github.io/iso-week-date/api/pandas/) and [polars](https://fbruzzesi.github.io/iso-week-date/api/polars/) functionalities (and namespaces) to work with series of ISO Week dates.
 
 ---
 
-[Documentation](https://fbruzzesi.github.io/iso-week-date/) | [Source Code](https://github.com/fbruzzesi/iso-week-date/)
+[Documentation](https://fbruzzesi.github.io/iso-week-date/) | [Source Code](https://github.com/fbruzzesi/iso-week-date/) | [Issue Tracker](https://github.com/fbruzzesi/iso-week-date/issues)
 
 ---
 
 ## Installation
 
 **iso-week-date** is published as a Python package on [pypi](https://pypi.org/project/iso-week-date/), and it can be installed with pip, or directly from source using git, or with a local clone:
```

### Comparing `iso_week_date-1.1.0/pyproject.toml` & `iso_week_date-1.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "iso-week-date"
-version = "1.1.0"
+version = "1.2.0"
 description = "Toolkit to work with str representing ISO Week date format"
 
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{name = "Francesco Bruzzesi"}]
 
@@ -38,21 +38,25 @@
     "pandas",
 ]
 
 polars = [
     "polars>=0.18.0",
 ]
 
+pydantic = [
+    "pydantic>=2.4.0",
+]
+
 dev = [
     "pre-commit==2.21.0",
     "hatch"
 ]
 
 lint = [
-    "ruff>=0.1.0"
+    "ruff>=0.4.0"
 ]
 
 docs = [
     "mkdocs>=1.4.2",
     "mkdocs-material>=9.2.0",
     "mkdocstrings[python]>=0.20.0",
     "mkdocs-autorefs",
@@ -61,34 +65,27 @@
 test = [
     "interrogate>=1.5.0",
     "pytest==7.2.0",
     "pytest-xdist==3.2.1",
     "coverage==7.2.1",
 ]
 
-all = ["iso-week-date[pandas,polars]"]
-all-dev = ["iso-week-date[pandas,polars,dev,lint,test,docs]"]
+all = ["iso-week-date[pandas,polars,pydantic]"]
+all-dev = ["iso-week-date[pandas,polars,pydantic,dev,lint,test,docs]"]
 
-[tool.setuptools.packages.find]
-include = ["iso_week_date*"]
-exclude = [
-    "data",
-    "docs",
-    "docker",
-    "kubernetes",
-    "notebooks",
-    "results",
-    "tests",
-]
+[tool.hatch.build.targets.sdist]
+only-include = ["iso_week_date"]
 
-[tool.setuptools.package-data]
-iso_week_date = ["py.typed"]
+[tool.hatch.build.targets.wheel]
+packages = ["iso_week_date"]
 
 [tool.ruff]
 line-length = 120
+
+[tool.ruff.lint]
 extend-select = ["I"]
 ignore = [
     "E731",  # do not assign a `lambda` expression, use a `def`
     ]
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
```

### Comparing `iso_week_date-1.1.0/PKG-INFO` & `iso_week_date-1.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: iso-week-date
-Version: 1.1.0
+Version: 1.2.0
 Summary: Toolkit to work with str representing ISO Week date format
 Project-URL: repository, https://github.com/fbruzzesi/iso-week-date
 Project-URL: issue-tracker, https://github.com/fbruzzesi/iso-week-date/issues
 Project-URL: documentation, https://fbruzzesi.github.io/iso-week-date/
 Author: Francesco Bruzzesi
 License: MIT License
         
@@ -36,63 +36,80 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: typing-extensions>=4.4.0; python_version < '3.12'
 Provides-Extra: all
-Requires-Dist: iso-week-date[pandas,polars]; extra == 'all'
+Requires-Dist: pandas; extra == 'all'
+Requires-Dist: polars>=0.18.0; extra == 'all'
+Requires-Dist: pydantic>=2.4.0; extra == 'all'
 Provides-Extra: all-dev
-Requires-Dist: iso-week-date[dev,docs,lint,pandas,polars,test]; extra == 'all-dev'
+Requires-Dist: coverage==7.2.1; extra == 'all-dev'
+Requires-Dist: hatch; extra == 'all-dev'
+Requires-Dist: interrogate>=1.5.0; extra == 'all-dev'
+Requires-Dist: mkdocs-autorefs; extra == 'all-dev'
+Requires-Dist: mkdocs-material>=9.2.0; extra == 'all-dev'
+Requires-Dist: mkdocs>=1.4.2; extra == 'all-dev'
+Requires-Dist: mkdocstrings[python]>=0.20.0; extra == 'all-dev'
+Requires-Dist: pandas; extra == 'all-dev'
+Requires-Dist: polars>=0.18.0; extra == 'all-dev'
+Requires-Dist: pre-commit==2.21.0; extra == 'all-dev'
+Requires-Dist: pydantic>=2.4.0; extra == 'all-dev'
+Requires-Dist: pytest-xdist==3.2.1; extra == 'all-dev'
+Requires-Dist: pytest==7.2.0; extra == 'all-dev'
+Requires-Dist: ruff>=0.4.0; extra == 'all-dev'
 Provides-Extra: dev
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: pre-commit==2.21.0; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs-autorefs; extra == 'docs'
 Requires-Dist: mkdocs-material>=9.2.0; extra == 'docs'
 Requires-Dist: mkdocs>=1.4.2; extra == 'docs'
 Requires-Dist: mkdocstrings[python]>=0.20.0; extra == 'docs'
 Provides-Extra: lint
-Requires-Dist: ruff>=0.1.0; extra == 'lint'
+Requires-Dist: ruff>=0.4.0; extra == 'lint'
 Provides-Extra: pandas
 Requires-Dist: pandas; extra == 'pandas'
 Provides-Extra: polars
 Requires-Dist: polars>=0.18.0; extra == 'polars'
+Provides-Extra: pydantic
+Requires-Dist: pydantic>=2.4.0; extra == 'pydantic'
 Provides-Extra: test
 Requires-Dist: coverage==7.2.1; extra == 'test'
 Requires-Dist: interrogate>=1.5.0; extra == 'test'
 Requires-Dist: pytest-xdist==3.2.1; extra == 'test'
 Requires-Dist: pytest==7.2.0; extra == 'test'
 Description-Content-Type: text/markdown
 
-<img src="docs/img/iso-week-date-logo.svg" width=185 height=185 align="right">
+# ISO Week Date
 
-![](https://img.shields.io/github/license/FBruzzesi/iso-week-date)
-<img src ="docs/img/interrogate-shield.svg">
+![license-shield](https://img.shields.io/github/license/FBruzzesi/iso-week-date)
+![interrogate-shield](docs/img/interrogate-shield.svg)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
-<img src="docs/img/coverage.svg">
-<img src="https://img.shields.io/pypi/pyversions/iso-week-date">
+![coverage](docs/img/coverage.svg)
+![pypi-versions](https://img.shields.io/pypi/pyversions/iso-week-date)
 
-# ISO Week Date
+<img src="docs/img/iso-week-date-logo.svg" width=160 height=160 align="right">
 
 **iso-week-date** is a toolkit to work with strings representing [ISO Week date](https://en.wikipedia.org/wiki/ISO_week_date) in two formats, namely:
 
-- Week format **YYYY-WNN** (corresponding to the date format **%Y-W%V**)
-- Week date format **YYYY-WNN-D** (corresponding to the date format **%Y-W%V-%u**)
+- Week format **YYYY-WNN** (date format **%Y-W%V**)
+- Week date format **YYYY-WNN-D** (date format **%Y-W%V-%u**)
 
-(where YYYY represents the year, W is a literal, NN represents the week number, and D represents the day of the week)
+where _YYYY_ represents the year, _W_ is a literal, _NN_ represents the week number, and _D_ represents the day of the week.
 
 In a nutshell it provides:
 
-- [`IsoWeek`](https://fbruzzesi.github.io/iso-week-date/api/isoweek/) and [`IsoWeekDate`](https://fbruzzesi.github.io/iso-week-date/api/isoweekdate/) classes implementing a series of methods to work with ISO Week (Date) formats and avoiding the pitfalls of going back and forth between string, date and datetime python objects
-- [pandas](https://fbruzzesi.github.io/iso-week-date/api/pandas/) and [polars](https://fbruzzesi.github.io/iso-week-date/api/polars/) functionalities to work with series of ISO Week dates
+- [`IsoWeek`](https://fbruzzesi.github.io/iso-week-date/api/isoweek/) and [`IsoWeekDate`](https://fbruzzesi.github.io/iso-week-date/api/isoweekdate/) classes that implement a series of methods to work with ISO Week (Date) formats directly, avoiding the pitfalls of going back and forth between string, date and datetime python objects.
+- [pandas](https://fbruzzesi.github.io/iso-week-date/api/pandas/) and [polars](https://fbruzzesi.github.io/iso-week-date/api/polars/) functionalities (and namespaces) to work with series of ISO Week dates.
 
 ---
 
-[Documentation](https://fbruzzesi.github.io/iso-week-date/) | [Source Code](https://github.com/fbruzzesi/iso-week-date/)
+[Documentation](https://fbruzzesi.github.io/iso-week-date/) | [Source Code](https://github.com/fbruzzesi/iso-week-date/) | [Issue Tracker](https://github.com/fbruzzesi/iso-week-date/issues)
 
 ---
 
 ## Installation
 
 **iso-week-date** is published as a Python package on [pypi](https://pypi.org/project/iso-week-date/), and it can be installed with pip, or directly from source using git, or with a local clone:
```

