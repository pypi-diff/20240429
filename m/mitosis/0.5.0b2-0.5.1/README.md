# Comparing `tmp/mitosis-0.5.0b2.tar.gz` & `tmp/mitosis-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitosis-0.5.0b2.tar", last modified: Tue Apr 23 04:52:30 2024, max compression
+gzip compressed data, was "mitosis-0.5.1.tar", last modified: Mon Apr 29 19:09:25 2024, max compression
```

## Comparing `mitosis-0.5.0b2.tar` & `mitosis-0.5.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.138217 mitosis-0.5.0b2/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.126217 mitosis-0.5.0b2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.130217 mitosis-0.5.0b2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-04-23 04:52:30.138217 mitosis-0.5.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14010 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.126217 mitosis-0.5.0b2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.130217 mitosis-0.5.0b2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.130217 mitosis-0.5.0b2/mitosis/
--rw-r--r--   0 runner    (1001) docker     (127)    21114 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6292 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/_typing.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-23 04:52:30.000000 mitosis-0.5.0b2/mitosis/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.134217 mitosis-0.5.0b2/mitosis/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/bad_return_experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/mock_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/mock_paper.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/mock_part1.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/mock_part2.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/pyproject_malformed.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/pyproject_missing.toml
--rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/mitosis/tests/test_pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 04:52:30.134217 mitosis-0.5.0b2/mitosis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-04-23 04:52:30.000000 mitosis-0.5.0b2/mitosis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-23 04:52:30.000000 mitosis-0.5.0b2/mitosis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 04:52:30.000000 mitosis-0.5.0b2/mitosis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-23 04:52:30.000000 mitosis-0.5.0b2/mitosis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-23 04:52:30.000000 mitosis-0.5.0b2/mitosis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 04:52:30.000000 mitosis-0.5.0b2/mitosis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-23 04:52:23.000000 mitosis-0.5.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-23 04:52:30.138217 mitosis-0.5.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.110498 mitosis-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-29 19:09:14.000000 mitosis-0.5.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.102498 mitosis-0.5.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.102498 mitosis-0.5.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-29 19:09:14.000000 mitosis-0.5.1/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-29 19:09:14.000000 mitosis-0.5.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-29 19:09:14.000000 mitosis-0.5.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-29 19:09:14.000000 mitosis-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-29 19:09:14.000000 mitosis-0.5.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-29 19:09:14.000000 mitosis-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16259 2024-04-29 19:09:25.110498 mitosis-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14149 2024-04-29 19:09:14.000000 mitosis-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.102498 mitosis-0.5.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.102498 mitosis-0.5.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-29 19:09:14.000000 mitosis-0.5.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-29 19:09:14.000000 mitosis-0.5.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.106498 mitosis-0.5.1/mitosis/
+-rw-r--r--   0 runner    (1001) docker     (127)    21349 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 19:09:25.000000 mitosis-0.5.1/mitosis/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.106498 mitosis-0.5.1/mitosis/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/bad_return_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/mock_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/mock_paper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/mock_part1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/mock_part2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/pyproject_malformed.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/pyproject_missing.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     7373 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-29 19:09:14.000000 mitosis-0.5.1/mitosis/tests/test_pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:09:25.106498 mitosis-0.5.1/mitosis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16259 2024-04-29 19:09:25.000000 mitosis-0.5.1/mitosis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-29 19:09:25.000000 mitosis-0.5.1/mitosis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:09:25.000000 mitosis-0.5.1/mitosis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 19:09:25.000000 mitosis-0.5.1/mitosis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-29 19:09:25.000000 mitosis-0.5.1/mitosis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 19:09:25.000000 mitosis-0.5.1/mitosis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-29 19:09:14.000000 mitosis-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-29 19:09:25.110498 mitosis-0.5.1/setup.cfg
```

### Comparing `mitosis-0.5.0b2/.github/workflows/main.yaml` & `mitosis-0.5.1/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b2/.github/workflows/release.yaml` & `mitosis-0.5.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b2/.gitignore` & `mitosis-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b2/.pre-commit-config.yaml` & `mitosis-0.5.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b2/LICENSE` & `mitosis-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b2/PKG-INFO` & `mitosis-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitosis
-Version: 0.5.0b2
+Version: 0.5.1
 Summary: Reproduce Machine Learning experiments easily
 Author-email: Jake Stevens-Haas <jacob.stevens.haas@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/Jacob-Stevens-Haas/mitosis
 Keywords: Machine Learning,Science,Mathematics,Experiments
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -31,15 +31,15 @@
 Requires-Dist: GitPython
 Requires-Dist: importlib_metadata
 Requires-Dist: ipykernel
 Requires-Dist: matplotlib
 Requires-Dist: nbconvert
 Requires-Dist: nbclient
 Requires-Dist: nbformat
-Requires-Dist: pandas
+Requires-Dist: pandas<2.2
 Requires-Dist: sqlalchemy
 Requires-Dist: toml
 Requires-Dist: types-toml
 Provides-Extra: dev
 Requires-Dist: pytest<8.0.0,>=6.0.0; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
@@ -273,14 +273,19 @@
 `first_exp.linear_pipeline(geospatial.datasets.load_data(...)["data"], ...)`.  Some caution here is advised - mitosis does not yet check all editably-installed packages for being git-clean.
 
 You could then have code in `my_paper` that loads the data from these trials and builds comparison plots, or you could rely on the plots each experiment creates.  You could also have a shell/batch script that spawns the main experiments of your paper.
 
 I'm often on a server and want to disconnect while the experiment is running, so I wrap my experiments in `nohup ... &> exp1.log &`.
 
 
+## pyproject.toml config
+The `[tool.mitosis]` table can be used to set `trials-folder`.  If relative,
+it is relative to repository root.
+
+
 ## Using persistent data
 
 There are two obviously useful things to do after an experiment:
 * view the html file.  `python -m http.server` is helpful to browse results
 * load the data with `load_trial_data()`
 
 Beyond this, the metadata mitosis keeps to disk is useful for troubleshooting or reproducing experiments, but no facility yet exists to browse or compare experiments.
```

### Comparing `mitosis-0.5.0b2/README.md` & `mitosis-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,19 @@
 `first_exp.linear_pipeline(geospatial.datasets.load_data(...)["data"], ...)`.  Some caution here is advised - mitosis does not yet check all editably-installed packages for being git-clean.
 
 You could then have code in `my_paper` that loads the data from these trials and builds comparison plots, or you could rely on the plots each experiment creates.  You could also have a shell/batch script that spawns the main experiments of your paper.
 
 I'm often on a server and want to disconnect while the experiment is running, so I wrap my experiments in `nohup ... &> exp1.log &`.
 
 
+## pyproject.toml config
+The `[tool.mitosis]` table can be used to set `trials-folder`.  If relative,
+it is relative to repository root.
+
+
 ## Using persistent data
 
 There are two obviously useful things to do after an experiment:
 * view the html file.  `python -m http.server` is helpful to browse results
 * load the data with `load_trial_data()`
 
 Beyond this, the metadata mitosis keeps to disk is useful for troubleshooting or reproducing experiments, but no facility yet exists to browse or compare experiments.
```

### Comparing `mitosis-0.5.0b2/docs/source/conf.py` & `mitosis-0.5.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b2/mitosis/__init__.py` & `mitosis-0.5.1/mitosis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from sqlalchemy import MetaData
 from sqlalchemy import select
 from sqlalchemy import String
 from sqlalchemy import Table
 from sqlalchemy import update
 
 from . import _disk
-from ._disk import _locate_trial_folder
+from ._disk import locate_trial_folder
 from ._typing import ExpStep
 from ._typing import Parameter
 from ._version import version as __version__  # noqa: F401
 
 
 def trials_columns():
     return [
@@ -68,15 +68,15 @@
     return [
         Column("name", String, primary_key=True),
         Column("params", String, unique=False),
     ]
 
 
 def load_trial_data(hexstr: str, *, trials_folder: Optional[Path | str] = None):
-    trial = _locate_trial_folder(hexstr, trials_folder=trials_folder)
+    trial = locate_trial_folder(hexstr, trials_folder=trials_folder)
     all_files = glob("results*.dill", root_dir=trial)
     results = []
     for file in all_files:
         with open(trial / file, "rb") as fh:
             results.append(dill.load(fh))
     return results
 
@@ -350,29 +350,30 @@
     nb = nbformat.v4.new_notebook()
     setup_cell = nbformat.v4.new_code_cell(source=code)
     step_loader_cells: list[NotebookNode] = []
     step_runner_cells: list[NotebookNode] = []
     for order, step in enumerate(steps):
         lookup_params = {a.arg_name: a.var_name for a in step.args if not a.evaluate}
         eval_params = {a.arg_name: a.var_name for a in step.args if a.evaluate}
-
+        logfile = trials_folder / "experiment.log"
         code = (
             (
                 f"step_{order} = mitosis.unpack('{step.action_ref}')\n"
                 f"lookup_{order} = mitosis.unpack('{step.lookup_ref}')\n"
                 f"resolved_args_{order} = {{}}\n"
                 f"logger = logging.getLogger('{step.action.__module__}')\n"
             )
             + (
                 "logger.setLevel(logging.DEBUG)\n"
                 if debug
                 else "logger.setLevel(logging.INFO)\n"
             )
             + (
-                f"logger.addHandler(logging.FileHandler('experiment.log', delay=True))\n"  # noqa E501
+                f"logger.addHandler(logging.FileHandler('{str(logfile)}', delay=True))\n"  # noqa E501
+                f"logger.info('Initialized experiment logger')\n"
                 f'print("Loaded step {order} as {step.action_ref}")\n'
                 f'print("Loaded lookup {order} as {step.lookup_ref}")\n'
                 f"for arg_name, var_name in {lookup_params}.items():\n"
                 f"    val = mitosis._lookup_param(arg_name, var_name, lookup_{order}).vals\n"  # noqa E501
                 f"    resolved_args_{order}.update({{arg_name: val}}) \n"
                 f"    print(arg_name,'=',resolved_args_{order}[arg_name])\n\n"
                 f"for arg_name, var_name in {eval_params}.items():\n"
@@ -393,28 +394,29 @@
             f"with open(r'{trials_folder / (f'results_{order}.dill')}', 'wb') as f:\n"  # noqa E501
             f"    dill.dump(curr_result, f)\n"
             f"print(repr(curr_result))\n"
             f"inputs = curr_result.get('data', None)\n"
         )
         step_runner_cells.append(nbformat.v4.new_code_cell(source=code))
 
-    nb["cells"] = [setup_cell] + step_loader_cells + step_runner_cells
+    result_cell = nbformat.v4.new_code_cell(source=("print(curr_result['main'])"))
+    nb["cells"] = [setup_cell] + step_loader_cells + step_runner_cells + [result_cell]
     with open(trials_folder / "source.py", "w") as fh:
         fh.write("".join(cell["source"] for cell in nb.cells))
     ep = ExecutePreprocessor(timeout=-1)
 
     exception = None
     metrics = None
     if debug:
         allowed = cast(tuple[type[Exception], ...], ())
     else:
         allowed = (CellExecutionError,)
     try:
         ep.preprocess(nb, {"metadata": {"path": trials_folder}})
-        metrics = nb["cells"][-1]["outputs"][0]["text"][:-1]
+        metrics = nb["cells"][-1]["outputs"][0]["text"][:-1]  # last char is newline
     except allowed as exc:
         exception = exc
     return nb, metrics, exception
 
 
 def _save_notebook(nb, filename, trials_folder, extension):
     if extension == "html":
@@ -516,15 +518,15 @@
     iteration: int,
     suffix: Optional[str],
     extension: str,
 ) -> str:
     new_filename = f"trial_{variant}_{iteration}_{suffix}"
     if debug:
         new_filename += "debug"
-    elif extension == "html":
+    if extension == "html":
         new_filename += ".html"
     elif extension == "ipynb":
         new_filename += ".ipynb"
     return new_filename
 
 
 def _log_start_experiment(
```

### Comparing `mitosis-0.5.0b2/mitosis/__main__.py` & `mitosis-0.5.1/mitosis/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import argparse
 from itertools import groupby
-from pathlib import Path
 from typing import Any
 from typing import NamedTuple
 
+from . import __version__
 from . import _disk
 from . import run
 from . import unpack
 from ._typing import ExpRun
 from ._typing import ExpStep
 from ._typing import Parameter
 
@@ -25,44 +25,53 @@
     parser.add_argument(
         "-m",
         "--module",
         nargs="?",
         help="Load complete experiment from a module",
     )
     parser.add_argument(
+        "--version",
+        action="store_true",
+        help="Print version information and exit",
+    )
+    parser.add_argument(
         "--debug",
         "-d",
         action="store_true",
         help=(
             "Run in debug mode, allowing one to use uncommitted code changes and not"
             " recording results"
         ),
     )
     parser.add_argument(
         "--config",
         type=str,
         default="pyproject.toml",
-        help="Name or path of config file",
+        help="Name or path to config file",
     )
     parser.add_argument(
-        "--folder",
+        "--trials-folder",
         "-F",
         type=str,
         default=None,
-        help="Where to save trials, relative to the experiment module folder",
+        help=(
+            "Where to save trials, relative to the current working directory. "
+            "If passed, overrides value in config file.  If not passed and no "
+            "configured value , mitosis uses <repository root> / 'trials'."
+        ),
     )
     parser.add_argument(
         "--eval-param",
         "-e",
         type=str,
         default=[],
         action="append",
         help=(
-            "Parameters directly passed on command line.  Make sure to quote if you"
-            " want argument to evaluate as a string"
+            "Parameters directly passed on command line.  Make sure to escape quotes if"
+            " you want argument to evaluate as a string"
         ),
     )
     parser.add_argument(
         "--param",
         "-p",
         action="append",
         default=[],
@@ -166,36 +175,42 @@
             all_steps[step_name],
             ep_dict.get(step_name, []),
             lp_dict.get(step_name, []),
         )
         for step_name in all_steps.keys()
     ]
 
-    if args.folder is None:
-        folder = Path(_disk.get_repo().working_dir) / "trials"
-    else:
-        folder = Path(args.folder)
+    folder = _disk.locate_trial_folder(trials_folder=args.folder, proj_file=args.config)
     return {
         "steps": exp_steps,
         "debug": args.debug,
         "trials_folder": folder,
     }
 
 
+def normalize_modinput(obj_ref: str) -> dict[str, tuple[str, str]]:
+    modname, _, qualname = obj_ref.partition(":")
+    if qualname:
+        sep = ":" + qualname + "."
+    else:
+        sep = ":"
+    return {obj_ref: (modname + sep + "run", modname + sep + "lookup_dict")}
+
+
 def main() -> None:
     parser = _create_parser()
     args = parser.parse_args()
+    if args.version:
+        try:
+            import setuptools_scm  # type: ignore
+
+            vstring = setuptools_scm.get_version()
+        except Exception:
+            vstring = __version__
+        print("mitosis", vstring)
+        return
     kwargs = _process_cl_args(args)
     run(**kwargs)
 
 
 if __name__ == "__main__":
     main()
-
-
-def normalize_modinput(obj_ref: str) -> dict[str, tuple[str, str]]:
-    modname, _, qualname = obj_ref.partition(":")
-    if qualname:
-        sep = ":" + qualname + "."
-    else:
-        sep = ":"
-    return {obj_ref: (modname + sep + "run", modname + sep + "lookup_dict")}
```

### Comparing `mitosis-0.5.0b2/mitosis/_disk.py` & `mitosis-0.5.1/mitosis/_disk.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from functools import lru_cache
 from pathlib import Path
+from typing import Any
 from typing import Optional
 
 import git
 import toml
 
 
 @lru_cache
@@ -16,50 +17,87 @@
         pyproj_file:
             Local or absolute path to pyproject file.  default is pyproject.toml
             if local path or default, use current git repo's top level directory
     Raises:
         Runtime error if cannot load steps, or if they are badly formed.
     """
     proj_file = _choose_toml(proj_file)
-    with open(proj_file, "r") as f:
-        config = toml.load(f)
+    config = _load_config(proj_file)
     try:
-        result = config["tool"]["mitosis"]["steps"]
+        result = config["steps"]
     except KeyError:
         raise RuntimeError(
-            f"{proj_file.absolute()} does not have a tools.mitosis.steps table"
+            f"{proj_file.absolute()} does not have a tool.mitosis.steps table"
         )
     if any(not isinstance(vals, list) or len(vals) != 2 for vals in result.values()):
         raise RuntimeError("tool.mitosis.steps table is malformed")
     return {k: tuple(v) for k, v in result.items()}
 
 
 @lru_cache
 def get_repo() -> git.Repo:
     repo = git.Repo(Path.cwd(), search_parent_directories=True)
     return repo
 
 
+@lru_cache
 def _choose_toml(filename: Path | str | None) -> Path:
+    """Identify the absolute location of the project file"""
     repo = get_repo()
-    directory = Path(repo.working_dir)
+    directory = Path(repo.working_dir).absolute()
     if filename is None:
         return directory / "pyproject.toml"
     elif not Path(filename).is_absolute():
         return directory / filename
     return Path(filename)
 
 
-def _locate_trial_folder(
-    hexstr: str, *, trials_folder: Optional[Path | str] = None
+def _load_config(toml_pth: Path) -> dict[str, Any]:
+    """Load the mitosis section of the config dictionary
+
+    Raises:
+        KeyError if no tool.mitosis table exists
+    """
+    if not toml_pth.is_absolute():
+        raise ValueError("Resolve path prior to final loading step")
+    with open(toml_pth, "rt", encoding="utf-8") as f:
+        config = toml.load(f)
+    return config["tool"]["mitosis"]
+
+
+def locate_trial_folder(
+    hexstr: Optional[str] = None,
+    *,
+    trials_folder: Optional[Path | str] = None,
+    proj_file: str = "pyproject.toml",
 ) -> Path:
+    """Identify where trials are saved.
+
+    Args:
+        hexstr: the hexstring of a trial.  Default (None) returns the
+            directory of all trials.  If not none, returns the metadata
+            folder for that trial
+        trials_folder: relative or absolute path of trials folder.  Default
+            (None) looks for a location in the project config file, or if
+            missing, uses <repository root> / 'trials'.
+        proj_file: path to the toml config for this project.
+    """
     if trials_folder is None:
-        trials_folder = Path().absolute()
+        try:
+            config = _load_config(_choose_toml(proj_file))
+            trials_folder = Path(config["trials-folder"])
+        except KeyError:
+            trials_folder = Path("trials")
     else:
         trials_folder = Path(trials_folder).resolve()
+    if not trials_folder.is_absolute():
+        trials_folder = Path(get_repo().working_dir).absolute() / trials_folder
+    if not hexstr:
+        return trials_folder
+
     matches = trials_folder.glob(f"*{hexstr}")
     try:
         first = next(matches)
     except StopIteration:
         raise FileNotFoundError(f"Could not find a trial that matched {hexstr}")
     try:
         next(matches)
```

### Comparing `mitosis-0.5.0b2/mitosis/_typing.py` & `mitosis-0.5.1/mitosis/_typing.py`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b2/mitosis/tests/test_all.py` & `mitosis-0.5.1/mitosis/tests/test_all.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,23 +136,25 @@
     exp_key = mitosis.run(
         mock_steps,
         debug=True,
         trials_folder=tmp_path,
     )
     data = mitosis.load_trial_data(exp_key, trials_folder=tmp_path)
     assert len(data[1]["data"]) == 5
+    metadata = mitosis._disk.locate_trial_folder(exp_key, trials_folder=tmp_path)
+    assert (metadata / "experiment").resolve().exists()
 
 
 def test_mod_metadata_debug(mock_steps, tmp_path):
     hexstr = mitosis.run(
         mock_steps,
         debug=True,
         trials_folder=tmp_path,
     )
-    trial_folder = _disk._locate_trial_folder(hexstr, trials_folder=tmp_path)
+    trial_folder = _disk.locate_trial_folder(hexstr, trials_folder=tmp_path)
     with open(trial_folder / "experiment.log", "r") as f:
         log_str = "".join(f.readlines())
     assert "This is run every time" in log_str
     assert "This is run in debug mode only" in log_str
     with open(trial_folder / "config.txt") as f:
         config_lines = f.readlines()
     config_params = [eval(line) for line in config_lines]
@@ -163,15 +165,15 @@
 @pytest.mark.clean
 def test_mod_metadata(mock_steps, tmp_path):
     hexstr = mitosis.run(
         mock_steps,
         debug=False,
         trials_folder=tmp_path,
     )
-    trial_folder = _disk._locate_trial_folder(hexstr, trials_folder=tmp_path)
+    trial_folder = _disk.locate_trial_folder(hexstr, trials_folder=tmp_path)
     with open(trial_folder / "experiment.log", "r") as f:
         log_str = "".join(f.readlines())
     assert "This is run every time" in log_str
     assert "This is run in debug mode only" not in log_str
     with open(trial_folder / "config.txt") as f:
         config_lines = f.readlines()
     config_params = [eval(line) for line in config_lines]
@@ -217,15 +219,15 @@
     }
     assert result == expected
 
 
 def test_load_bad_toml():
     parent = Path(__file__).resolve().parent
     tomlfile = parent / "pyproject_missing.toml"
-    with pytest.raises(RuntimeError, match="does not have a tools"):
+    with pytest.raises(RuntimeError, match="does not have a tool"):
         _disk.load_mitosis_steps(tomlfile)
     tomlfile = parent / "pyproject_malformed.toml"
     with pytest.raises(RuntimeError, match="table is malformed"):
         _disk.load_mitosis_steps(tomlfile)
 
 
 def test_unpack():
```

### Comparing `mitosis-0.5.0b2/mitosis/tests/test_cli.py` & `mitosis-0.5.1/mitosis/tests/test_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,19 @@
+import contextlib
+import sys
 from argparse import Namespace
+from io import StringIO
+from typing import Generator
 
 import pytest
 
 from mitosis.__main__ import _create_parser
 from mitosis.__main__ import _process_cl_args
 from mitosis.__main__ import _split_param_str
+from mitosis.__main__ import main
 from mitosis.__main__ import normalize_modinput
 from mitosis.tests.mock_legacy import lookup_dict
 from mitosis.tests.mock_legacy import run
 from mitosis.tests.mock_paper import meth_config
 from mitosis.tests.mock_part1 import Klass
 
 
@@ -56,15 +61,15 @@
     args = parser.parse_args(
         ["-m", "mod", "-d", "--config", "foo.toml", "-F", "foo/bar"]
     )
     assert args.experiment == []
     assert args.module == "mod"
     assert args.debug is True
     assert args.config == "foo.toml"
-    assert args.folder == "foo/bar"
+    assert args.trials_folder == "foo/bar"
     assert args.eval_param == []
     assert args.param == []
 
 
 def test_argparse_main():
     parser = _create_parser()
     args = parser.parse_args(
@@ -72,15 +77,15 @@
             "step1", "step2", "-e", "a=1", "-e", "b=2", "-p", "c=d", "-p", "e=f", "-p", "g=h"  # fmt: skip; # noqa: E501
         ]
     )
     assert args.experiment == ["step1", "step2"]
     assert args.module is None
     assert args.debug is False
     assert args.config == "pyproject.toml"
-    assert args.folder is None
+    assert args.trials_folder is None
     assert len(args.eval_param) == 2
     assert len(args.param) == 3
 
 
 def test_split_param_str():
     result = _split_param_str("+a=b")
     assert result == ("", False, "a", "b")
@@ -102,7 +107,34 @@
     result = normalize_modinput(modinput)
     assert result == {
         "mitosis.tests.mock_experiment:MockExp.MockExpInner": (
             "mitosis.tests.mock_experiment:MockExp.MockExpInner.run",
             "mitosis.tests.mock_experiment:MockExp.MockExpInner.lookup_dict",
         )
     }
+
+
+def test_version():
+    @contextlib.contextmanager
+    def set_argv(*args: str) -> Generator[None, None, None]:
+        temp = sys.argv
+        try:
+            sys.argv = list(args)
+            yield
+        finally:
+            sys.argv = temp
+
+    @contextlib.contextmanager
+    def capture_stdout() -> Generator[StringIO, None, None]:
+        stdout = sys.stdout
+        new_out = StringIO()
+        try:
+            sys.stdout = new_out
+            yield new_out
+        finally:
+            sys.stdout = stdout
+
+    with set_argv("mitosis", "--version"):
+        with capture_stdout() as out:
+            main()
+            result = out.getvalue()
+    assert result.split()[0] == "mitosis"
```

### Comparing `mitosis-0.5.0b2/mitosis.egg-info/PKG-INFO` & `mitosis-0.5.1/mitosis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitosis
-Version: 0.5.0b2
+Version: 0.5.1
 Summary: Reproduce Machine Learning experiments easily
 Author-email: Jake Stevens-Haas <jacob.stevens.haas@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/Jacob-Stevens-Haas/mitosis
 Keywords: Machine Learning,Science,Mathematics,Experiments
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -31,15 +31,15 @@
 Requires-Dist: GitPython
 Requires-Dist: importlib_metadata
 Requires-Dist: ipykernel
 Requires-Dist: matplotlib
 Requires-Dist: nbconvert
 Requires-Dist: nbclient
 Requires-Dist: nbformat
-Requires-Dist: pandas
+Requires-Dist: pandas<2.2
 Requires-Dist: sqlalchemy
 Requires-Dist: toml
 Requires-Dist: types-toml
 Provides-Extra: dev
 Requires-Dist: pytest<8.0.0,>=6.0.0; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
@@ -273,14 +273,19 @@
 `first_exp.linear_pipeline(geospatial.datasets.load_data(...)["data"], ...)`.  Some caution here is advised - mitosis does not yet check all editably-installed packages for being git-clean.
 
 You could then have code in `my_paper` that loads the data from these trials and builds comparison plots, or you could rely on the plots each experiment creates.  You could also have a shell/batch script that spawns the main experiments of your paper.
 
 I'm often on a server and want to disconnect while the experiment is running, so I wrap my experiments in `nohup ... &> exp1.log &`.
 
 
+## pyproject.toml config
+The `[tool.mitosis]` table can be used to set `trials-folder`.  If relative,
+it is relative to repository root.
+
+
 ## Using persistent data
 
 There are two obviously useful things to do after an experiment:
 * view the html file.  `python -m http.server` is helpful to browse results
 * load the data with `load_trial_data()`
 
 Beyond this, the metadata mitosis keeps to disk is useful for troubleshooting or reproducing experiments, but no facility yet exists to browse or compare experiments.
```

### Comparing `mitosis-0.5.0b2/mitosis.egg-info/SOURCES.txt` & `mitosis-0.5.1/mitosis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitosis-0.5.0b2/pyproject.toml` & `mitosis-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
   "GitPython",
   "importlib_metadata",
   "ipykernel",
   "matplotlib",
   "nbconvert",
   "nbclient",
   "nbformat",
-  "pandas",
+  "pandas<2.2",
   "sqlalchemy",
   "toml",
   "types-toml",
 ]
 
 [project.optional-dependencies]
 dev = [
```

