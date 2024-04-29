# Comparing `tmp/ba_tsconcat-0.1.0.tar.gz` & `tmp/ba_tsconcat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ba_tsconcat-0.1.0.tar", max compression
+gzip compressed data, was "ba_tsconcat-0.1.1.tar", max compression
```

## Comparing `ba_tsconcat-0.1.0.tar` & `ba_tsconcat-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    26190 2024-01-09 15:33:57.670371 ba_tsconcat-0.1.0/LICENSE
--rw-r--r--   0        0        0     2701 2024-01-09 15:33:57.670371 ba_tsconcat-0.1.0/README.md
--rw-r--r--   0        0        0     1812 2024-01-09 15:33:57.670371 ba_tsconcat-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      262 2024-01-09 15:33:57.670371 ba_tsconcat-0.1.0/src/tsconcat/__init__.py
--rw-r--r--   0        0        0     5297 2024-01-09 15:33:57.670371 ba_tsconcat-0.1.0/src/tsconcat/cli.py
--rw-r--r--   0        0        0     1139 2024-01-09 15:33:57.670371 ba_tsconcat-0.1.0/src/tsconcat/concat.py
--rw-r--r--   0        0        0     2623 2024-01-09 15:33:57.670371 ba_tsconcat-0.1.0/src/tsconcat/pretreeprint.py
--rw-r--r--   0        0        0     2793 2024-01-09 15:33:57.670371 ba_tsconcat-0.1.0/src/tsconcat/utils.py
--rw-r--r--   0        0        0     3443 1970-01-01 00:00:00.000000 ba_tsconcat-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    26190 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2779 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/README.md
+-rw-r--r--   0        0        0     1695 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      262 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/src/tsconcat/__init__.py
+-rw-r--r--   0        0        0     5911 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/src/tsconcat/cli.py
+-rw-r--r--   0        0        0     1139 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/src/tsconcat/concat.py
+-rw-r--r--   0        0        0     2623 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/src/tsconcat/pretreeprint.py
+-rw-r--r--   0        0        0     2793 2024-04-29 20:52:29.284104 ba_tsconcat-0.1.1/src/tsconcat/utils.py
+-rw-r--r--   0        0        0     3494 1970-01-01 00:00:00.000000 ba_tsconcat-0.1.1/PKG-INFO
```

### Comparing `ba_tsconcat-0.1.0/LICENSE` & `ba_tsconcat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.0/README.md` & `ba_tsconcat-0.1.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 # `tsconcat`
 
-[![Build](https://github.com/cmi-dair/tsconcat/actions/workflows/test.yaml/badge.svg?branch=main)](https://github.com/cmi-dair/tsconcat/actions/workflows/test.yaml?query=branch%3Amain)
-[![codecov](https://codecov.io/gh/cmi-dair/tsconcat/branch/main/graph/badge.svg?token=22HWWFWPW5)](https://codecov.io/gh/cmi-dair/tsconcat)
+[![Build](https://github.com/childmindresearch/tsconcat/actions/workflows/test.yaml/badge.svg?branch=main)](https://github.com/childmindresearch/tsconcat/actions/workflows/test.yaml?query=branch%3Amain)
+[![codecov](https://codecov.io/gh/childmindresearch/tsconcat/branch/main/graph/badge.svg?token=22HWWFWPW5)](https://codecov.io/gh/childmindresearch/tsconcat)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 ![stability-wip](https://img.shields.io/badge/stability-work_in_progress-lightgrey.svg)
 [![L-GPL License](https://img.shields.io/badge/license-L--GPL-blue.svg)](LICENSE)
-[![pages](https://img.shields.io/badge/api-docs-blue)](https://cmi-dair.github.io/tsconcat)
-
+[![pages](https://img.shields.io/badge/api-docs-blue)](https://childmindresearch.github.io/tsconcat)
 
 BIDS App and Python library for concatenating MRI time series.
 
 Inspired by [Cho et al. 2021](https://doi.org/10.1016/j.neuroimage.2020.117549).
 
 ## Features
 
 - Concatenate BOLD time series from multiple datasets, sessions, subjects or runs into a single file.
 - Dry run mode to check what the output directory will look like.
-- Fake mode to produce a [bids2table](https://github.com/cmi-dair/bids2table) compatible parquet output directory.
+- Fake mode to produce a [bids2table](https://github.com/childmindresearch/bids2table) compatible parquet output directory.
 
 ## Installation
 
 <!--
 Install this package via:
 
 ```sh
 pip install tsconcat
 ```
 
 Or -->Get the newest development version via:
 
 ```sh
-pip install git+https://github.com/cmi-dair/tsconcat
+pip install git+https://github.com/childmindresearch/tsconcat
 ```
 
 ## Quick start
 
 ```sh
 ba-tsconcat /path/to/input/bids /path/to/output group --concat ses --dry_run
 ```
 
-![image](https://github.com/cmi-dair/tsconcat/assets/33600480/501037b0-77c6-40fe-bc7d-a3575944b0c6)
+![image](https://github.com/childmindresearch/tsconcat/assets/33600480/501037b0-77c6-40fe-bc7d-a3575944b0c6)
 
 ## Usage
 
 ```sh
 ba-tsconcat --help
 usage: ba-tsconcat [-h] [-c CONCAT] [-d] [-f] bids_dir output_dir {group}
 
@@ -58,13 +57,11 @@
   -h, --help            show this help message and exit
   -c CONCAT, --concat CONCAT
                         Concat across. Can be any combination of dataset, sub, ses, run separated by spaces. Output data will be grouped by the set difference.
   -d, --dry_run         Dry run. Print output directory structure instead of actually doing something. If this is enabled 'bids_dir' may be a path to a bids2table parquet directory.
   -f, --fake            Fake output. Output a bids2table parquet directory instead of actually doing something.
 ```
 
-
-
 ## Links or References
 
 - [Impact of concatenating fMRI data on reliability for functional connectomics (Cho et al. 2021)](https://doi.org/10.1016/j.neuroimage.2020.117549)
-- [bids2table](https://github.com/cmi-dair/bids2table)
+- [bids2table](https://github.com/childmindresearch/bids2table)
```

### Comparing `ba_tsconcat-0.1.0/pyproject.toml` & `ba_tsconcat-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 [tool.poetry]
 name = "ba-tsconcat"
-version = "0.1.0"
+version = "0.1.1"
 description = "BIDS App and Python library for concatenating MRI time series."
 authors = ["CMI DAIR Center <florian.rupprecht@childmind.org>"]
 license = "LGPL-2.1"
 readme = "README.md"
 packages = [{include = "tsconcat", from = "src"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
-bids2table = "^0.1.0a0"
-pdoc = {version = "^14.3.0", optional = true}
+python = "^3.10"
+bids2table = "^0.1.0b0"
 nibabel = "^5.2.0"
 numpy = "^1.26.3"
-pandas = "<2.1"  # 2.1.x breaks bids2table/elbow
+pandas = ">1.0"
 rich = "^13.4.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 mypy = "^1.8.0"
 pre-commit = "^3.6.0"
 pytest-cov = "^4.1.0"
 ruff = "^0.1.8"
 
 [tool.poetry.group.docs.dependencies]
-pdoc = "^14.3.0"
-
-[tool.poetry.extras]
-docs = ["pdoc"]
+pdoc = "^14.4.0"
 
 [tool.poetry.scripts]
 ba-tsconcat = "tsconcat.cli:main"
 
 [tool.pytest.ini_options]
 pythonpath = [
   "src"
```

### Comparing `ba_tsconcat-0.1.0/src/tsconcat/cli.py` & `ba_tsconcat-0.1.1/src/tsconcat/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,29 +17,37 @@
     file_path_from_b2table_row,
     file_paths_from_b2table,
     sidecar_path_from_b2table_row,
 )
 
 elbow.utils.setup_logging("ERROR")
 
-REDUCE_COLUMNS = ["dataset", "sub", "ses", "run"]
+REDUCE_COLUMNS = ["ds__dataset", "ent__sub", "ent__ses", "ent__run"]
 REDUCE_COLUMNS_SET = set(REDUCE_COLUMNS)
+REDUCE_COLUMNS_ALIAS = {
+    "dataset": "ds__dataset",
+    "sub": "ent__sub",
+    "subject": "ent__sub",
+    "ses": "ent__ses",
+    "session": "ent__ses",
+    "run": "ent__run",
+}
 
 
 def _reduce_op(
     df: pd.DataFrame,
     group_by: List[str],
     inplace: bool = False,
     group_callback: Optional[Callable[[pd.DataFrame], None]] = None,
 ) -> pd.DataFrame:
     """Reduce dataframe to one row per group."""
     if not inplace:
         df = df.copy()
 
-    group_by_set = set(group_by)
+    group_by_set = set(REDUCE_COLUMNS_ALIAS.get(g, g) for g in group_by)
 
     unknown_cols = list(group_by_set - REDUCE_COLUMNS_SET)
     if len(unknown_cols) > 0:
         raise Exception(f"Unknown columns: {unknown_cols}")
     del unknown_cols
 
     df.sort_values(by=REDUCE_COLUMNS, inplace=True)
@@ -77,15 +85,15 @@
     """Concatenate MRI timeseries."""
     parser = build_bidsapp_group_parser(prog="ba-tsconcat", description="Concatenate MRI timeseries.")
 
     parser.add_argument(
         "-c",
         "--concat",
         type=str,
-        help=f"Concat across. Can be any combination of {', '.join(REDUCE_COLUMNS)} separated by spaces. "
+        help=f"Concat across. Can be any combination of {', '.join(REDUCE_COLUMNS_ALIAS.keys())} separated by spaces. "
         f"Output data will be grouped by the set difference.",
         default="ses",
     )
 
     parser.add_argument(
         "-d",
         "--dry_run",
@@ -99,68 +107,84 @@
         "-f",
         "--fake",
         action="store_true",
         help="Fake output. Output a bids2table parquet directory instead of actually doing something.",
         default=False,
     )
 
+    # workers
+    parser.add_argument(
+        "-w",
+        "--workers",
+        type=int,
+        help="Number of workers for bids2table. Default is 1.",
+        default=1,
+    )
+
     args = parser.parse_args()
 
     input_dir: pl.Path = args.bids_dir
     output_dir: pl.Path = args.output_dir
     concat_labels: List[str] = args.concat.split(" ")
     dry_run: bool = args.dry_run
     fake: bool = args.fake
     dry_run = dry_run or fake
+    workers: int = args.workers
 
     if not input_dir.exists():
         raise Exception("Input directory does not exist.")
 
     if dry_run and (df := _read_if_parquet(input_dir)) is not None:
         df = bids2table.table.flat_to_multi_columns(df)
     else:
-        df = bids2table.bids2table(input_dir)
+        df = bids2table.bids2table(input_dir, workers=workers)
 
         if df.shape[0] == 0:
             raise Exception("Empty BIDS dataset")
 
     if not dry_run:
         output_dir.mkdir(parents=True, exist_ok=True)
 
-    # We dont care about these
-    df = df.droplevel(0, axis="columns")
+    # print dataframe columns
+    print(df.columns)
 
     df_bold = df.query(
-        "datatype == 'func' and "
-        "ext == '.nii.gz' and "
-        "suffix == 'bold' and "
-        "desc == 'preproc' and "
-        "space == 'MNI152NLin6ASym'"
+        "ent__datatype == 'func' and "
+        "ent__ext == '.nii.gz' and "
+        "ent__suffix == 'bold'"# and "
+        #"ent__desc == 'preproc' and "
+        #"ent__space == 'MNI152NLin6ASym'"
     )
 
+    print(df)
+    print(df_bold)
+
+    if df_bold.shape[0] == 0:
+        raise Exception("No BOLD files found")
+
     def _process_group(df_group: pd.DataFrame) -> None:
         group_identifiers = df_group.iloc[0][list(REDUCE_COLUMNS_SET - set(concat_labels))].to_dict()
         print(f"Process group: {group_identifiers}")
 
         first_row: pd.Series = df_group.iloc[0]
 
         for group_label in concat_labels:
             first_row[group_label] = None  # todo does vectorized work here?
 
         # Generate file
 
         file_path = output_dir / file_path_from_b2table_row(first_row)
 
         file_path.parent.mkdir(parents=True, exist_ok=True)
-        concat_nifti1_4d(paths=df_group.file_path.values, out_path=file_path)
+        concat_nifti1_4d(paths=df_group.finfo__file_path.values, out_path=file_path)
 
         # Generate sidecar
 
         sidecar_path = output_dir / sidecar_path_from_b2table_row(first_row)
-        sidecar_contents = first_row["sidecar"]  # TODO: Maybe add list of files that were concatenated?
+        sidecar_contents = first_row["meta__json"]  # TODO: Maybe add list of files that were concatenated?
         with open(sidecar_path, "w", encoding="utf-8") as fp:
             json.dump(sidecar_contents, fp)
 
     df_reduced_bold = _reduce_op(
         df_bold,
         group_by=concat_labels,
         group_callback=None if dry_run else _process_group,
```

### Comparing `ba_tsconcat-0.1.0/src/tsconcat/concat.py` & `ba_tsconcat-0.1.1/src/tsconcat/concat.py`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.0/src/tsconcat/pretreeprint.py` & `ba_tsconcat-0.1.1/src/tsconcat/pretreeprint.py`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.0/src/tsconcat/utils.py` & `ba_tsconcat-0.1.1/src/tsconcat/utils.py`

 * *Files identical despite different names*

### Comparing `ba_tsconcat-0.1.0/PKG-INFO` & `ba_tsconcat-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,68 @@
 Metadata-Version: 2.1
 Name: ba-tsconcat
-Version: 0.1.0
+Version: 0.1.1
 Summary: BIDS App and Python library for concatenating MRI time series.
 License: LGPL-2.1
 Author: CMI DAIR Center
 Author-email: florian.rupprecht@childmind.org
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: docs
-Requires-Dist: bids2table (>=0.1.0a0,<0.2.0)
+Requires-Dist: bids2table (>=0.1.0b0,<0.2.0)
 Requires-Dist: nibabel (>=5.2.0,<6.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
-Requires-Dist: pandas (<2.1)
-Requires-Dist: pdoc (>=14.3.0,<15.0.0) ; extra == "docs"
+Requires-Dist: pandas (>1.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Description-Content-Type: text/markdown
 
 # `tsconcat`
 
-[![Build](https://github.com/cmi-dair/tsconcat/actions/workflows/test.yaml/badge.svg?branch=main)](https://github.com/cmi-dair/tsconcat/actions/workflows/test.yaml?query=branch%3Amain)
-[![codecov](https://codecov.io/gh/cmi-dair/tsconcat/branch/main/graph/badge.svg?token=22HWWFWPW5)](https://codecov.io/gh/cmi-dair/tsconcat)
+[![Build](https://github.com/childmindresearch/tsconcat/actions/workflows/test.yaml/badge.svg?branch=main)](https://github.com/childmindresearch/tsconcat/actions/workflows/test.yaml?query=branch%3Amain)
+[![codecov](https://codecov.io/gh/childmindresearch/tsconcat/branch/main/graph/badge.svg?token=22HWWFWPW5)](https://codecov.io/gh/childmindresearch/tsconcat)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 ![stability-wip](https://img.shields.io/badge/stability-work_in_progress-lightgrey.svg)
 [![L-GPL License](https://img.shields.io/badge/license-L--GPL-blue.svg)](LICENSE)
-[![pages](https://img.shields.io/badge/api-docs-blue)](https://cmi-dair.github.io/tsconcat)
-
+[![pages](https://img.shields.io/badge/api-docs-blue)](https://childmindresearch.github.io/tsconcat)
 
 BIDS App and Python library for concatenating MRI time series.
 
 Inspired by [Cho et al. 2021](https://doi.org/10.1016/j.neuroimage.2020.117549).
 
 ## Features
 
 - Concatenate BOLD time series from multiple datasets, sessions, subjects or runs into a single file.
 - Dry run mode to check what the output directory will look like.
-- Fake mode to produce a [bids2table](https://github.com/cmi-dair/bids2table) compatible parquet output directory.
+- Fake mode to produce a [bids2table](https://github.com/childmindresearch/bids2table) compatible parquet output directory.
 
 ## Installation
 
 <!--
 Install this package via:
 
 ```sh
 pip install tsconcat
 ```
 
 Or -->Get the newest development version via:
 
 ```sh
-pip install git+https://github.com/cmi-dair/tsconcat
+pip install git+https://github.com/childmindresearch/tsconcat
 ```
 
 ## Quick start
 
 ```sh
 ba-tsconcat /path/to/input/bids /path/to/output group --concat ses --dry_run
 ```
 
-![image](https://github.com/cmi-dair/tsconcat/assets/33600480/501037b0-77c6-40fe-bc7d-a3575944b0c6)
+![image](https://github.com/childmindresearch/tsconcat/assets/33600480/501037b0-77c6-40fe-bc7d-a3575944b0c6)
 
 ## Usage
 
 ```sh
 ba-tsconcat --help
 usage: ba-tsconcat [-h] [-c CONCAT] [-d] [-f] bids_dir output_dir {group}
 
@@ -79,14 +77,12 @@
   -h, --help            show this help message and exit
   -c CONCAT, --concat CONCAT
                         Concat across. Can be any combination of dataset, sub, ses, run separated by spaces. Output data will be grouped by the set difference.
   -d, --dry_run         Dry run. Print output directory structure instead of actually doing something. If this is enabled 'bids_dir' may be a path to a bids2table parquet directory.
   -f, --fake            Fake output. Output a bids2table parquet directory instead of actually doing something.
 ```
 
-
-
 ## Links or References
 
 - [Impact of concatenating fMRI data on reliability for functional connectomics (Cho et al. 2021)](https://doi.org/10.1016/j.neuroimage.2020.117549)
-- [bids2table](https://github.com/cmi-dair/bids2table)
+- [bids2table](https://github.com/childmindresearch/bids2table)
```

