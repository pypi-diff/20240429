# Comparing `tmp/ropt_dakota-0.1.1.tar.gz` & `tmp/ropt_dakota-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ropt_dakota-0.1.1.tar", last modified: Mon Apr 22 06:57:04 2024, max compression
+gzip compressed data, was "ropt_dakota-0.2.0.tar", last modified: Mon Apr 29 12:21:27 2024, max compression
```

## Comparing `ropt_dakota-0.1.1.tar` & `ropt_dakota-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:57:04.848228 ropt_dakota-0.1.1/
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:57:04.840228 ropt_dakota-0.1.1/.github/
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:57:04.844228 ropt_dakota-0.1.1/.github/workflows/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      974 2024-04-19 12:39:55.000000 ropt_dakota-0.1.1/.github/workflows/static-checks.yml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      766 2024-04-19 13:16:05.000000 ropt_dakota-0.1.1/.github/workflows/tests.yml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       63 2024-04-19 12:37:21.000000 ropt_dakota-0.1.1/.gitignore
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    35149 2024-04-19 14:26:30.000000 ropt_dakota-0.1.1/LICENSE
--rw-r--r--   0 verveerpj  (1000) verveerpj  (1000)     1927 2024-04-22 06:57:04.844228 ropt_dakota-0.1.1/PKG-INFO
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1063 2024-04-22 06:56:12.000000 ropt_dakota-0.1.1/README.md
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     1978 2024-04-22 06:52:17.000000 ropt_dakota-0.1.1/pyproject.toml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       38 2024-04-22 06:57:04.848228 ropt_dakota-0.1.1/setup.cfg
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:57:04.840228 ropt_dakota-0.1.1/src/
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:57:04.844228 ropt_dakota-0.1.1/src/ropt_dakota/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       42 2024-04-19 12:40:07.000000 ropt_dakota-0.1.1/src/ropt_dakota/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    18308 2024-04-19 12:40:20.000000 ropt_dakota-0.1.1/src/ropt_dakota/dakota.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 12:33:56.000000 ropt_dakota-0.1.1/src/ropt_dakota/py.typed
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      411 2024-04-22 06:57:04.000000 ropt_dakota-0.1.1/src/ropt_dakota/version.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:57:04.844228 ropt_dakota-0.1.1/src/ropt_dakota.egg-info/
--rw-r--r--   0 verveerpj  (1000) verveerpj  (1000)     1927 2024-04-22 06:57:04.000000 ropt_dakota-0.1.1/src/ropt_dakota.egg-info/PKG-INFO
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      514 2024-04-22 06:57:04.000000 ropt_dakota-0.1.1/src/ropt_dakota.egg-info/SOURCES.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        1 2024-04-22 06:57:04.000000 ropt_dakota-0.1.1/src/ropt_dakota.egg-info/dependency_links.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       69 2024-04-22 06:57:04.000000 ropt_dakota-0.1.1/src/ropt_dakota.egg-info/entry_points.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       40 2024-04-22 06:57:04.000000 ropt_dakota-0.1.1/src/ropt_dakota.egg-info/requires.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       12 2024-04-22 06:57:04.000000 ropt_dakota-0.1.1/src/ropt_dakota.egg-info/top_level.txt
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 06:57:04.844228 ropt_dakota-0.1.1/tests/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-19 12:33:56.000000 ropt_dakota-0.1.1/tests/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2496 2024-04-19 12:40:23.000000 ropt_dakota-0.1.1/tests/conftest.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    12950 2024-04-19 12:41:17.000000 ropt_dakota-0.1.1/tests/test_dakota_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:27.119937 ropt_dakota-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:27.115937 ropt_dakota-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:27.119937 ropt_dakota-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/.github/workflows/static-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-29 12:21:27.119937 ropt_dakota-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:21:27.119937 ropt_dakota-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:27.115937 ropt_dakota-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:27.119937 ropt_dakota-0.2.0/src/ropt_dakota/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/src/ropt_dakota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18513 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/src/ropt_dakota/dakota.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/src/ropt_dakota/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 12:21:27.000000 ropt_dakota-0.2.0/src/ropt_dakota/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:27.119937 ropt_dakota-0.2.0/src/ropt_dakota.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-29 12:21:27.000000 ropt_dakota-0.2.0/src/ropt_dakota.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-29 12:21:27.000000 ropt_dakota-0.2.0/src/ropt_dakota.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:21:27.000000 ropt_dakota-0.2.0/src/ropt_dakota.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 12:21:27.000000 ropt_dakota-0.2.0/src/ropt_dakota.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-29 12:21:27.000000 ropt_dakota-0.2.0/src/ropt_dakota.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 12:21:27.000000 ropt_dakota-0.2.0/src/ropt_dakota.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:27.119937 ropt_dakota-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12950 2024-04-29 12:21:16.000000 ropt_dakota-0.2.0/tests/test_dakota_backend.py
```

### Comparing `ropt_dakota-0.1.1/.github/workflows/static-checks.yml` & `ropt_dakota-0.2.0/.github/workflows/static-checks.yml`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install ropt
         python -m pip install .[test]
     - name: Run ruff format
       if: always()
       run: |
         python -m ruff format --check src/ropt_dakota tests
     - name: Run ruff
       if: always()
```

### Comparing `ropt_dakota-0.1.1/.github/workflows/tests.yml` & `ropt_dakota-0.2.0/.github/workflows/tests.yml`

 * *Files 12% similar despite different names*

```diff
@@ -21,13 +21,12 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install ropt
         python -m pip install pytest
         python -m pip install .
     - name: Run pytest
       run: |
         python -m pytest tests
```

### Comparing `ropt_dakota-0.1.1/LICENSE` & `ropt_dakota-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ropt_dakota-0.1.1/PKG-INFO` & `ropt_dakota-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt-dakota
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Dakota optimizer plugin for ropt
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: carolina
+Requires-Dist: ropt>=0.2.1
 Provides-Extra: test
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 
 # A Dakota optimizer plugin for `ropt`
 This package installs a plugin for the `ropt` robust optimization package,
@@ -35,28 +36,30 @@
 This code has been tested with Python versions 3.8-3.12.
 
 The plugin is based on the [Dakota](https://dakota.sandia.gov/) optimizer and
 depends on the [Carolina](https://github.com/equinor/Carolina) Python wrapper.
 
 
 ## Installation
+From PyPI:
 ```bash
 pip install ropt-dakota
 ```
 
 
 ## Development
 The `ropt-dakota` source distribution can be found on
 [GitHub](https://github.com/tno-ropt/ropt-dakota). To install from source, enter
-the `ropt` distribution directory and execute:
+the distribution directory and execute:
 
 ```bash
 pip install .
 ```
 
+
 ## Running the tests
 To run the test suite, install the necessary dependencies and execute `pytest`:
 
 ```bash
 pip install .[test]
 pytest
 ```
```

### Comparing `ropt_dakota-0.1.1/README.md` & `ropt_dakota-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,28 +11,30 @@
 This code has been tested with Python versions 3.8-3.12.
 
 The plugin is based on the [Dakota](https://dakota.sandia.gov/) optimizer and
 depends on the [Carolina](https://github.com/equinor/Carolina) Python wrapper.
 
 
 ## Installation
+From PyPI:
 ```bash
 pip install ropt-dakota
 ```
 
 
 ## Development
 The `ropt-dakota` source distribution can be found on
 [GitHub](https://github.com/tno-ropt/ropt-dakota). To install from source, enter
-the `ropt` distribution directory and execute:
+the distribution directory and execute:
 
 ```bash
 pip install .
 ```
 
+
 ## Running the tests
 To run the test suite, install the necessary dependencies and execute `pytest`:
 
 ```bash
 pip install .[test]
 pytest
 ```
```

### Comparing `ropt_dakota-0.1.1/pyproject.toml` & `ropt_dakota-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
 ]
 requires-python = ">=3.8"
 dynamic = ["version"]
-dependencies = ["numpy", "carolina"]
+dependencies = ["numpy", "carolina", "ropt>=0.2.1"]
 
 [project.optional-dependencies]
 test = ["ruff", "mypy", "pytest"]
 
 [project.entry-points."ropt.plugins.optimizer"]
 dakota = "ropt_dakota.dakota:DakotaOptimizer"
 
@@ -40,15 +40,15 @@
 
 [tool.setuptools_scm]
 write_to = "src/ropt_dakota/version.py"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "error",
-    'ignore:.*Pydantic will allow any object with no validation.*:UserWarning',          # 3.8
+    'ignore:.*Pydantic will allow any object with no validation.*:UserWarning', # 3.8
 ]
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
     "ANN101",
     "ANN102",
```

### Comparing `ropt_dakota-0.1.1/src/ropt_dakota/dakota.py` & `ropt_dakota-0.2.0/src/ropt_dakota/dakota.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,24 @@
             with TemporaryDirectory() as output_dir:
                 self._output_dir = Path(output_dir)
                 self._start(initial_values)
         else:
             self._output_dir = self._config.optimizer.output_dir
             self._start(initial_values)
 
+    @property
+    def allow_nan(self) -> bool:
+        """Whether NaN is allowed.
+
+        See the [ropt.plugins.optimizer.protocol.Optimizer][] protocol.
+
+        # noqa
+        """
+        return False
+
     def _get_constraint_indices(self) -> Optional[_ConstraintIndices]:
         if self._config.nonlinear_constraints is None:
             return None
         types = self._config.nonlinear_constraints.types
         return (
             np.fromiter(
                 (idx for idx, type_ in enumerate(types) if type_ == ConstraintType.LE),
```

### Comparing `ropt_dakota-0.1.1/src/ropt_dakota.egg-info/PKG-INFO` & `ropt_dakota-0.2.0/src/ropt_dakota.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt-dakota
-Version: 0.1.1
+Version: 0.2.0
 Summary: A Dakota optimizer plugin for ropt
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: carolina
+Requires-Dist: ropt>=0.2.1
 Provides-Extra: test
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 
 # A Dakota optimizer plugin for `ropt`
 This package installs a plugin for the `ropt` robust optimization package,
@@ -35,28 +36,30 @@
 This code has been tested with Python versions 3.8-3.12.
 
 The plugin is based on the [Dakota](https://dakota.sandia.gov/) optimizer and
 depends on the [Carolina](https://github.com/equinor/Carolina) Python wrapper.
 
 
 ## Installation
+From PyPI:
 ```bash
 pip install ropt-dakota
 ```
 
 
 ## Development
 The `ropt-dakota` source distribution can be found on
 [GitHub](https://github.com/tno-ropt/ropt-dakota). To install from source, enter
-the `ropt` distribution directory and execute:
+the distribution directory and execute:
 
 ```bash
 pip install .
 ```
 
+
 ## Running the tests
 To run the test suite, install the necessary dependencies and execute `pytest`:
 
 ```bash
 pip install .[test]
 pytest
 ```
```

### Comparing `ropt_dakota-0.1.1/src/ropt_dakota.egg-info/SOURCES.txt` & `ropt_dakota-0.2.0/src/ropt_dakota.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
+.github/workflows/release.yml
 .github/workflows/static-checks.yml
 .github/workflows/tests.yml
 src/ropt_dakota/__init__.py
 src/ropt_dakota/dakota.py
 src/ropt_dakota/py.typed
 src/ropt_dakota/version.py
 src/ropt_dakota.egg-info/PKG-INFO
```

### Comparing `ropt_dakota-0.1.1/tests/conftest.py` & `ropt_dakota-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ropt_dakota-0.1.1/tests/test_dakota_backend.py` & `ropt_dakota-0.2.0/tests/test_dakota_backend.py`

 * *Files identical despite different names*

