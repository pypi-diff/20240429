# Comparing `tmp/ropt_nomad-0.2.0.tar.gz` & `tmp/ropt_nomad-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ropt_nomad-0.2.0.tar", last modified: Thu Apr 25 09:41:05 2024, max compression
+gzip compressed data, was "ropt_nomad-0.2.1.tar", last modified: Mon Apr 29 12:25:44 2024, max compression
```

## Comparing `ropt_nomad-0.2.0.tar` & `ropt_nomad-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.132851 ropt_nomad-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.124851 ropt_nomad-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.128851 ropt_nomad-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/.github/workflows/static-checks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-25 09:41:05.132851 ropt_nomad-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.128851 ropt_nomad-0.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/examples/discrete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/examples/rosenbrock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 09:41:05.132851 ropt_nomad-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.124851 ropt_nomad-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.128851 ropt_nomad-0.2.0/src/ropt_nomad/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/src/ropt_nomad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12571 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/src/ropt_nomad/nomad.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/src/ropt_nomad/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-25 09:41:05.000000 ropt_nomad-0.2.0/src/ropt_nomad/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.128851 ropt_nomad-0.2.0/src/ropt_nomad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-25 09:41:05.000000 ropt_nomad-0.2.0/src/ropt_nomad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-25 09:41:05.000000 ropt_nomad-0.2.0/src/ropt_nomad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 09:41:05.000000 ropt_nomad-0.2.0/src/ropt_nomad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-25 09:41:05.000000 ropt_nomad-0.2.0/src/ropt_nomad.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-25 09:41:05.000000 ropt_nomad-0.2.0/src/ropt_nomad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-25 09:41:05.000000 ropt_nomad-0.2.0/src/ropt_nomad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:05.128851 ropt_nomad-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-04-25 09:41:01.000000 ropt_nomad-0.2.0/tests/test_nomad_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.680877 ropt_nomad-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.676877 ropt_nomad-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.676877 ropt_nomad-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/.github/workflows/static-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-29 12:25:44.680877 ropt_nomad-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.676877 ropt_nomad-0.2.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/examples/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/examples/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:25:44.680877 ropt_nomad-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.676877 ropt_nomad-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.680877 ropt_nomad-0.2.1/src/ropt_nomad/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/src/ropt_nomad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12739 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/src/ropt_nomad/nomad.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/src/ropt_nomad/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 12:25:44.000000 ropt_nomad-0.2.1/src/ropt_nomad/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.680877 ropt_nomad-0.2.1/src/ropt_nomad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-29 12:25:44.000000 ropt_nomad-0.2.1/src/ropt_nomad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-29 12:25:44.000000 ropt_nomad-0.2.1/src/ropt_nomad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:25:44.000000 ropt_nomad-0.2.1/src/ropt_nomad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-29 12:25:44.000000 ropt_nomad-0.2.1/src/ropt_nomad.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 12:25:44.000000 ropt_nomad-0.2.1/src/ropt_nomad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 12:25:44.000000 ropt_nomad-0.2.1/src/ropt_nomad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:44.680877 ropt_nomad-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-04-29 12:25:40.000000 ropt_nomad-0.2.1/tests/test_nomad_backend.py
```

### Comparing `ropt_nomad-0.2.0/.github/workflows/release.yml` & `ropt_nomad-0.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.0/.github/workflows/static-checks.yml` & `ropt_nomad-0.2.1/.github/workflows/static-checks.yml`

 * *Files 8% similar despite different names*

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
         python -m ruff format --check src/ropt_nomad tests
     - name: Run ruff
       if: always()
```

### Comparing `ropt_nomad-0.2.0/.github/workflows/tests.yml` & `ropt_nomad-0.2.1/.github/workflows/tests.yml`

 * *Files 22% similar despite different names*

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

### Comparing `ropt_nomad-0.2.0/LICENSE` & `ropt_nomad-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.0/PKG-INFO` & `ropt_nomad-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt-nomad
-Version: 0.2.0
+Version: 0.2.1
 Summary: A NOMAD backend for the ropt robust optimization package
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyNomadBBO
+Requires-Dist: ropt>=0.2.1
 Provides-Extra: test
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 
 # A NOMAD optimizer plugin for ropt
 This package installs a plugin for the [ropt](https://github.com/tno-ropt/ropt)
```

### Comparing `ropt_nomad-0.2.0/README.md` & `ropt_nomad-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.0/examples/discrete.py` & `ropt_nomad-0.2.1/examples/discrete.py`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.0/examples/rosenbrock.py` & `ropt_nomad-0.2.1/examples/rosenbrock.py`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.0/pyproject.toml` & `ropt_nomad-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
 ]
 requires-python = ">=3.8"
 dynamic = ["version"]
-dependencies = ["PyNomadBBO"]
+dependencies = ["PyNomadBBO", "ropt>=0.2.1"]
 
 [project.optional-dependencies]
 test = ["ruff", "mypy", "pytest"]
 
 [project.entry-points."ropt.plugins.optimizer"]
 nomad = "ropt_nomad.nomad:NomadOptimizer"
```

### Comparing `ropt_nomad-0.2.0/src/ropt_nomad/nomad.py` & `ropt_nomad-0.2.1/src/ropt_nomad/nomad.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,14 +121,24 @@
                 self._evaluate,
                 initial_values.tolist(),
                 self._bounds[0],
                 self._bounds[1],
                 self._parameters,
             )
 
+    @property
+    def allow_nan(self) -> bool:
+        """Whether NaN is allowed.
+
+        See the [ropt.plugins.optimizer.protocol.Optimizer][] protocol.
+
+        # noqa
+        """
+        return True
+
     def _get_bounds(self) -> Tuple[List[float], List[float]]:
         lower_bounds = self._config.variables.lower_bounds
         upper_bounds = self._config.variables.upper_bounds
         variable_indices = self._config.variables.indices
         if variable_indices is not None:
             lower_bounds = lower_bounds[variable_indices]
             upper_bounds = upper_bounds[variable_indices]
@@ -321,11 +331,10 @@
         if self._cached_function is None:
             self._cached_variables = variables.copy()
             with self._redirector.stop():
                 function, _ = self._optimizer_callback(
                     variables,
                     return_functions=True,
                     return_gradients=False,
-                    allow_nan=True,
                 )
             self._cached_function = function.copy()
         return self._cached_function
```

### Comparing `ropt_nomad-0.2.0/src/ropt_nomad.egg-info/PKG-INFO` & `ropt_nomad-0.2.1/src/ropt_nomad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt-nomad
-Version: 0.2.0
+Version: 0.2.1
 Summary: A NOMAD backend for the ropt robust optimization package
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: PyNomadBBO
+Requires-Dist: ropt>=0.2.1
 Provides-Extra: test
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 
 # A NOMAD optimizer plugin for ropt
 This package installs a plugin for the [ropt](https://github.com/tno-ropt/ropt)
```

### Comparing `ropt_nomad-0.2.0/src/ropt_nomad.egg-info/SOURCES.txt` & `ropt_nomad-0.2.1/src/ropt_nomad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.0/tests/conftest.py` & `ropt_nomad-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.0/tests/test_examples.py` & `ropt_nomad-0.2.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ropt_nomad-0.2.0/tests/test_nomad_backend.py` & `ropt_nomad-0.2.1/tests/test_nomad_backend.py`

 * *Files identical despite different names*

