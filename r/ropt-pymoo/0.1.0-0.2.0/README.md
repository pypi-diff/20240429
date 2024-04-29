# Comparing `tmp/ropt_pymoo-0.1.0.tar.gz` & `tmp/ropt_pymoo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ropt_pymoo-0.1.0.tar", last modified: Mon Apr 22 07:26:56 2024, max compression
+gzip compressed data, was "ropt_pymoo-0.2.0.tar", last modified: Mon Apr 29 12:25:57 2024, max compression
```

## Comparing `ropt_pymoo-0.1.0.tar` & `ropt_pymoo-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 07:26:56.193792 ropt_pymoo-0.1.0/
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 07:26:56.189792 ropt_pymoo-0.1.0/.github/
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 07:26:56.189792 ropt_pymoo-0.1.0/.github/workflows/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      959 2024-04-22 06:34:37.000000 ropt_pymoo-0.1.0/.github/workflows/static-checks.yml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      774 2024-04-22 06:32:14.000000 ropt_pymoo-0.1.0/.github/workflows/tests.yml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       62 2024-04-22 06:30:31.000000 ropt_pymoo-0.1.0/.gitignore
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    35149 2024-04-22 06:31:18.000000 ropt_pymoo-0.1.0/LICENSE
--rw-r--r--   0 verveerpj  (1000) verveerpj  (1000)     6333 2024-04-22 07:26:56.193792 ropt_pymoo-0.1.0/PKG-INFO
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     5383 2024-04-22 07:16:18.000000 ropt_pymoo-0.1.0/README.md
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 07:26:56.189792 ropt_pymoo-0.1.0/examples/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2685 2024-04-22 06:34:15.000000 ropt_pymoo-0.1.0/examples/discrete_ga.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      691 2023-12-04 15:08:51.000000 ropt_pymoo-0.1.0/examples/discrete_ga.yml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2245 2024-04-22 06:34:18.000000 ropt_pymoo-0.1.0/examples/rosenbrock_cmaes.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2172 2024-04-22 07:22:51.000000 ropt_pymoo-0.1.0/pyproject.toml
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       38 2024-04-22 07:26:56.193792 ropt_pymoo-0.1.0/setup.cfg
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 07:26:56.189792 ropt_pymoo-0.1.0/src/
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 07:26:56.189792 ropt_pymoo-0.1.0/src/ropt_pymoo/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       78 2024-04-22 06:34:22.000000 ropt_pymoo-0.1.0/src/ropt_pymoo/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     8658 2024-01-17 11:38:25.000000 ropt_pymoo-0.1.0/src/ropt_pymoo/_config.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        0 2023-12-04 15:08:51.000000 ropt_pymoo-0.1.0/src/ropt_pymoo/py.typed
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    10621 2024-04-22 06:34:24.000000 ropt_pymoo-0.1.0/src/ropt_pymoo/pymoo.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      411 2024-04-22 07:26:56.000000 ropt_pymoo-0.1.0/src/ropt_pymoo/version.py
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 07:26:56.193792 ropt_pymoo-0.1.0/src/ropt_pymoo.egg-info/
--rw-r--r--   0 verveerpj  (1000) verveerpj  (1000)     6333 2024-04-22 07:26:56.000000 ropt_pymoo-0.1.0/src/ropt_pymoo.egg-info/PKG-INFO
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      629 2024-04-22 07:26:56.000000 ropt_pymoo-0.1.0/src/ropt_pymoo.egg-info/SOURCES.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        1 2024-04-22 07:26:56.000000 ropt_pymoo-0.1.0/src/ropt_pymoo.egg-info/dependency_links.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       65 2024-04-22 07:26:56.000000 ropt_pymoo-0.1.0/src/ropt_pymoo.egg-info/entry_points.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       58 2024-04-22 07:26:56.000000 ropt_pymoo-0.1.0/src/ropt_pymoo.egg-info/requires.txt
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)       11 2024-04-22 07:26:56.000000 ropt_pymoo-0.1.0/src/ropt_pymoo.egg-info/top_level.txt
-drwxrwxr-x   0 verveerpj  (1000) verveerpj  (1000)        0 2024-04-22 07:26:56.193792 ropt_pymoo-0.1.0/tests/
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)        0 2023-12-04 15:08:51.000000 ropt_pymoo-0.1.0/tests/__init__.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)     2496 2024-04-22 06:34:25.000000 ropt_pymoo-0.1.0/tests/conftest.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)      958 2024-02-27 07:12:09.000000 ropt_pymoo-0.1.0/tests/test_examples.py
--rw-rw-r--   0 verveerpj  (1000) verveerpj  (1000)    10165 2024-04-22 06:34:26.000000 ropt_pymoo-0.1.0/tests/test_pymoo_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.961099 ropt_pymoo-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.957099 ropt_pymoo-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.957099 ropt_pymoo-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/.github/workflows/static-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-29 12:25:57.961099 ropt_pymoo-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.957099 ropt_pymoo-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/examples/discrete_ga.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/examples/discrete_ga.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/examples/rosenbrock_cmaes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 12:25:57.961099 ropt_pymoo-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.957099 ropt_pymoo-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.961099 ropt_pymoo-0.2.0/src/ropt_pymoo/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/src/ropt_pymoo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8641 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/src/ropt_pymoo/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/src/ropt_pymoo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/src/ropt_pymoo/pymoo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 12:25:57.000000 ropt_pymoo-0.2.0/src/ropt_pymoo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.961099 ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-29 12:25:57.000000 ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-29 12:25:57.000000 ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:25:57.000000 ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-29 12:25:57.000000 ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-29 12:25:57.000000 ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 12:25:57.000000 ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:57.961099 ropt_pymoo-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-04-29 12:25:53.000000 ropt_pymoo-0.2.0/tests/test_pymoo_backend.py
```

### Comparing `ropt_pymoo-0.1.0/.github/workflows/static-checks.yml` & `ropt_pymoo-0.2.0/.github/workflows/static-checks.yml`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install ropt
         python -m pip install .[test]
     - name: Run ruff format
       if: always()
       run: |
         python -m ruff format --check src/ropt_pymoo tests
     - name: Run ruff
       if: always()
```

### Comparing `ropt_pymoo-0.1.0/.github/workflows/tests.yml` & `ropt_pymoo-0.2.0/.github/workflows/tests.yml`

 * *Files 11% similar despite different names*

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
         python -m pip install pytest ruamel.yaml
         python -m pip install .
     - name: Run pytest
       run: |
         python -m pytest tests
```

### Comparing `ropt_pymoo-0.1.0/LICENSE` & `ropt_pymoo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ropt_pymoo-0.1.0/PKG-INFO` & `ropt_pymoo-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt-pymoo
-Version: 0.1.0
+Version: 0.2.0
 Summary: A pymoo backend for the ropt robust optimization library
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,14 +14,15 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pymoo
 Requires-Dist: pydantic
+Requires-Dist: ropt>=0.2.1
 Provides-Extra: test
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: ruamel.yaml; extra == "test"
 
 # A pymoo optimizer plugin for ropt
@@ -45,18 +46,16 @@
 ```bash
 pip install ropt-pymoo
 ```
 
 
 ## Usage
 An optimization by ropt using the plugin works mostly as any other optimization
-run (see also the `ropt` documentation on
-[GitHubPages](https://tno-ropt.github.io/ropt/) or on [Read the
-Docs](https://ropt.readthedocs.io/)). However, there are a few things to
-consider:
+run (see also the [ropt documentation](https://tno-ropt.github.io/ropt/)).
+However, there are a few things to consider:
 
 1. Gradients are not used, as `pymoo` does not seem to support passing
    user-defined gradients. Hence, any specifications relating to gradient
    calulcations in ropt are ignored.
 2. Some standard optimization parameters that can be specified in the
    optimization section are ignored, specifically:
     - `max_iterations`
```

### Comparing `ropt_pymoo-0.1.0/README.md` & `ropt_pymoo-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,16 @@
 ```bash
 pip install ropt-pymoo
 ```
 
 
 ## Usage
 An optimization by ropt using the plugin works mostly as any other optimization
-run (see also the `ropt` documentation on
-[GitHubPages](https://tno-ropt.github.io/ropt/) or on [Read the
-Docs](https://ropt.readthedocs.io/)). However, there are a few things to
-consider:
+run (see also the [ropt documentation](https://tno-ropt.github.io/ropt/)).
+However, there are a few things to consider:
 
 1. Gradients are not used, as `pymoo` does not seem to support passing
    user-defined gradients. Hence, any specifications relating to gradient
    calulcations in ropt are ignored.
 2. Some standard optimization parameters that can be specified in the
    optimization section are ignored, specifically:
     - `max_iterations`
```

### Comparing `ropt_pymoo-0.1.0/examples/discrete_ga.py` & `ropt_pymoo-0.2.0/examples/discrete_ga.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from pathlib import Path  # noqa: INP001
 from typing import Any, Dict
 
 import numpy as np
 from numpy.typing import NDArray
-from ruamel import yaml
 from ropt.config.enopt import EnOptConfig
 from ropt.enums import ConstraintType, EventType
 from ropt.evaluator import EvaluatorContext, EvaluatorResult
 from ropt.events import OptimizationEvent
 from ropt.optimization import EnsembleOptimizer
 from ropt.results import FunctionResults
+from ruamel import yaml
 
 # For convenience we use a YAML file to store the optimizer options:
 options = yaml.YAML(typ="safe", pure=True).load(Path("discrete_ga.yml"))
 
 CONFIG: Dict[str, Any] = {
     "variables": {
         # Ignored, but needed to establish the number of variables:
```

### Comparing `ropt_pymoo-0.1.0/examples/discrete_ga.yml` & `ropt_pymoo-0.2.0/examples/discrete_ga.yml`

 * *Files identical despite different names*

### Comparing `ropt_pymoo-0.1.0/examples/rosenbrock_cmaes.py` & `ropt_pymoo-0.2.0/examples/rosenbrock_cmaes.py`

 * *Files identical despite different names*

### Comparing `ropt_pymoo-0.1.0/pyproject.toml` & `ropt_pymoo-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
 ]
 requires-python = ">=3.8"
 dynamic = ["version"]
-dependencies = ["numpy", "pymoo", "pydantic"]
+dependencies = ["numpy", "pymoo", "pydantic", "ropt>=0.2.1"]
 
 [project.optional-dependencies]
 test = ["ruff", "mypy", "pytest", "ruamel.yaml"]
 
 [project.entry-points."ropt.plugins.optimizer"]
 pymoo = "ropt_pymoo.pymoo:PyMooOptimizer"
```

### Comparing `ropt_pymoo-0.1.0/src/ropt_pymoo/_config.py` & `ropt_pymoo-0.2.0/src/ropt_pymoo/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
         """
         if isinstance(self.termination, tuple):
             return self.termination
         module_name, _, name = self.termination.name.rpartition(".")
         if not module_name:
             try:
                 return get_termination(name, **self.termination.parameters)
-            except Exception as exc:  # noqa: BLE001
+            except Exception as exc:
                 msg = f"Failed to run get_termination for: {name}"
                 raise ValueError(msg) from exc
         termination_class = _get_class(
             self.termination.name,
             prefix="pymoo.termination",
             keyword="name",
         )
@@ -179,15 +179,15 @@
     def get_constraints(self) -> Any:  # noqa: ANN401
         """Parse the constraints config.
 
         Raises:
             ValueError: When the constraints object is not found.
 
         Returns:
-            An `pymoo` constraints class.
+            A `pymoo` constraints class.
         """
         if self.constraints is None:
             return None
         constraints_class = _get_class(
             self.constraints.name,
             prefix="pymoo.constraints",
             keyword="name",
```

### Comparing `ropt_pymoo-0.1.0/src/ropt_pymoo/pymoo.py` & `ropt_pymoo-0.2.0/src/ropt_pymoo/pymoo.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 if TYPE_CHECKING:
     from numpy.typing import NDArray
     from ropt.config.enopt import EnOptConfig
     from ropt.plugins.optimizer.protocol import OptimizerCallback
 
 _OUTPUT_FILE = "optimizer_output"
 
+# These algorithms do not allow NaN fucntion values:
+_NO_FAILURE_HANDLING = {"NelderMead"}
+
 
 @dataclass
 class _Constraints:
     linear_eq: NDArray[np.uintc] = field(
         default_factory=lambda: np.array([], dtype=np.uintc)
     )
     linear_ineq: NDArray[np.uintc] = field(
@@ -133,14 +136,19 @@
         self._parameters = ParametersConfig.model_validate(options)
         self._bounds = self._get_bounds()
         self._constraints = self._get_constraints()
         self._cached_variables: Optional[NDArray[np.float64]] = None
         self._cached_function: Optional[NDArray[np.float64]] = None
         self._stdout: TextIO
 
+        self._allow_nan = True
+        for algorithm in _NO_FAILURE_HANDLING:
+            if algorithm in self._parameters.algorithm:
+                self._allow_nan = False
+
     def start(self, initial_values: NDArray[np.float64]) -> None:
         """Start the optimization.
 
         See the [ropt.plugins.optimizer.protocol.OptimizerBackend][] protocol.
 
         # noqa
         """
@@ -167,25 +175,36 @@
         output_file: Union[str, Path]
         if output_dir is None:
             output_file = os.devnull
         else:
             output_file = create_output_path(_OUTPUT_FILE, output_dir, suffix=".txt")
 
         self._stdout = sys.stdout
+
         with Path(output_file).open("a", encoding="utf-8") as output, redirect_stdout(
             output
         ):
             minimize(
                 problem,
                 self._parameters.get_algorithm(),
                 termination=self._parameters.get_termination(),
                 seed=self._parameters.seed,
                 verbose=output_dir is not None,
             )
 
+    @property
+    def allow_nan(self) -> bool:
+        """Whether NaN is allowed.
+
+        See the [ropt.plugins.optimizer.protocol.Optimizer][] protocol.
+
+        # noqa
+        """
+        return self._allow_nan
+
     def _get_bounds(self) -> Tuple[NDArray[np.float64], NDArray[np.float64]]:
         lower_bounds = self._config.variables.lower_bounds
         upper_bounds = self._config.variables.upper_bounds
         variable_indices = self._config.variables.indices
         if variable_indices is not None:
             lower_bounds = lower_bounds[variable_indices]
             upper_bounds = upper_bounds[variable_indices]
@@ -277,11 +296,15 @@
         ):
             self._cached_variables = None
             self._cached_function = None
         if self._cached_function is None:
             self._cached_variables = variables.copy()
             with redirect_stdout(self._stdout):
                 function, _ = self._optimizer_callback(
-                    variables, return_functions=True, return_gradients=False
+                    variables,
+                    return_functions=True,
+                    return_gradients=False,
                 )
+                if self._allow_nan:
+                    function = np.where(np.isnan(function), np.inf, function)
             self._cached_function = function.copy()
         return self._cached_function
```

### Comparing `ropt_pymoo-0.1.0/src/ropt_pymoo.egg-info/PKG-INFO` & `ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ropt-pymoo
-Version: 0.1.0
+Version: 0.2.0
 Summary: A pymoo backend for the ropt robust optimization library
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,14 +14,15 @@
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pymoo
 Requires-Dist: pydantic
+Requires-Dist: ropt>=0.2.1
 Provides-Extra: test
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: ruamel.yaml; extra == "test"
 
 # A pymoo optimizer plugin for ropt
@@ -45,18 +46,16 @@
 ```bash
 pip install ropt-pymoo
 ```
 
 
 ## Usage
 An optimization by ropt using the plugin works mostly as any other optimization
-run (see also the `ropt` documentation on
-[GitHubPages](https://tno-ropt.github.io/ropt/) or on [Read the
-Docs](https://ropt.readthedocs.io/)). However, there are a few things to
-consider:
+run (see also the [ropt documentation](https://tno-ropt.github.io/ropt/)).
+However, there are a few things to consider:
 
 1. Gradients are not used, as `pymoo` does not seem to support passing
    user-defined gradients. Hence, any specifications relating to gradient
    calulcations in ropt are ignored.
 2. Some standard optimization parameters that can be specified in the
    optimization section are ignored, specifically:
     - `max_iterations`
```

### Comparing `ropt_pymoo-0.1.0/src/ropt_pymoo.egg-info/SOURCES.txt` & `ropt_pymoo-0.2.0/src/ropt_pymoo.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitignore
 LICENSE
 README.md
 pyproject.toml
+.github/workflows/release.yml
 .github/workflows/static-checks.yml
 .github/workflows/tests.yml
 examples/discrete_ga.py
 examples/discrete_ga.yml
 examples/rosenbrock_cmaes.py
 src/ropt_pymoo/__init__.py
 src/ropt_pymoo/_config.py
```

### Comparing `ropt_pymoo-0.1.0/tests/conftest.py` & `ropt_pymoo-0.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ropt_pymoo-0.1.0/tests/test_examples.py` & `ropt_pymoo-0.2.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `ropt_pymoo-0.1.0/tests/test_pymoo_backend.py` & `ropt_pymoo-0.2.0/tests/test_pymoo_backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # pylint: disable=protected-access
 
 from typing import Any, Dict, cast
 
 import numpy as np
 import pytest
 from numpy.typing import NDArray
-from ropt.enums import ConstraintType
+from ropt.enums import ConstraintType, EventType, OptimizerExitCode
+from ropt.events import OptimizationEvent
 from ropt.optimization import EnsembleOptimizer
 
 
 @pytest.fixture(name="enopt_config")
 def enopt_config_fixture() -> Dict[str, Any]:
     return {
         "variables": {
@@ -303,7 +304,102 @@
                     "constraint_tolerance": 1e-4,
                 }
             },
         ],
     )
     assert result is not None
     assert np.allclose(result.evaluations.variables, [-0.05, 0.0, 0.45], atol=0.02)
+
+
+def test_pymoo_bound_constraints_with_failure(
+    enopt_config: Dict[str, Any], evaluator: Any, test_functions: Any
+) -> None:
+    enopt_config["variables"]["lower_bounds"] = [0.15, -1.0, -1.0]
+    enopt_config["variables"]["upper_bounds"] = [1.0, 1.0, 0.2]
+    enopt_config["optimizer"]["algorithm"] = "soo.nonconvex.de.DE"
+    enopt_config["optimizer"]["parallel"] = True
+    enopt_config["optimizer"]["max_functions"] = 800
+    enopt_config["realizations"] = {"realization_min_success": 0}
+    optimizer = EnsembleOptimizer(evaluator())
+    result1 = optimizer.start_optimization(
+        plan=[
+            {"config": enopt_config},
+            {"optimizer": {"id": "opt"}},
+            {"tracker": {"id": "optimum", "source": "opt"}},
+        ],
+    )
+    assert result1 is not None
+    assert np.allclose(result1.evaluations.variables, [0.15, 0.0, 0.2], atol=0.02)
+
+    counter = 0
+
+    def _add_nan(x: Any) -> Any:
+        nonlocal counter
+        counter += 1
+        if counter == 2:
+            counter = 0
+            return np.nan
+        return test_functions[0](x)
+
+    optimizer = EnsembleOptimizer(evaluator((_add_nan, test_functions[1])))
+    result2 = optimizer.start_optimization(
+        plan=[
+            {"config": enopt_config},
+            {"optimizer": {"id": "opt"}},
+            {"tracker": {"id": "optimum", "source": "opt"}},
+        ],
+    )
+    assert result2 is not None
+    assert np.allclose(result2.evaluations.variables, [0.15, 0.0, 0.2], atol=0.02)
+    assert not np.all(
+        np.equal(result1.evaluations.variables, result2.evaluations.variables)
+    )
+
+
+def test_pymoo_bound_constraints_no_failure_handling(
+    enopt_config: Dict[str, Any], evaluator: Any, test_functions: Any
+) -> None:
+    enopt_config["variables"]["lower_bounds"] = [0.15, -1.0, -1.0]
+    enopt_config["variables"]["upper_bounds"] = [1.0, 1.0, 0.2]
+    enopt_config["optimizer"]["algorithm"] = "soo.nonconvex.nelder.NelderMead"
+    enopt_config["optimizer"]["parallel"] = True
+    enopt_config["optimizer"]["max_functions"] = 800
+
+    optimizer = EnsembleOptimizer(evaluator())
+    result1 = optimizer.start_optimization(
+        plan=[
+            {"config": enopt_config},
+            {"optimizer": {"id": "opt"}},
+            {"tracker": {"id": "optimum", "source": "opt"}},
+        ],
+    )
+    assert result1 is not None
+    assert np.allclose(result1.evaluations.variables, [0.15, 0.0, 0.2], atol=0.02)
+
+    enopt_config["realizations"] = {"realization_min_success": 0}
+
+    counter = 0
+
+    def _add_nan(x: Any) -> Any:
+        nonlocal counter
+        counter += 1
+        if counter == 2:
+            counter = 0
+            return np.nan
+        return test_functions[0](x)
+
+    def handle_finished(event: OptimizationEvent) -> None:
+        assert event.exit_code == OptimizerExitCode.TOO_FEW_REALIZATIONS
+
+    optimizer = EnsembleOptimizer(evaluator((_add_nan, test_functions[1])))
+    optimizer.add_observer(EventType.FINISHED_OPTIMIZER_STEP, handle_finished)
+    result2 = optimizer.start_optimization(
+        plan=[
+            {"config": enopt_config},
+            {"optimizer": {"id": "opt"}},
+            {"tracker": {"id": "optimum", "source": "opt"}},
+        ],
+    )
+    assert result2 is not None
+    assert not np.all(
+        np.equal(result1.evaluations.variables, result2.evaluations.variables)
+    )
```

