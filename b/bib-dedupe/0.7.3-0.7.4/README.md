# Comparing `tmp/bib_dedupe-0.7.3.tar.gz` & `tmp/bib_dedupe-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bib_dedupe-0.7.3.tar", max compression
+gzip compressed data, was "bib_dedupe-0.7.4.tar", max compression
```

## Comparing `bib_dedupe-0.7.3.tar` & `bib_dedupe-0.7.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1070 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/LICENSE
--rw-r--r--   0        0        0     3083 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/README.md
--rw-r--r--   0        0        0      411 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/__init__.py
--rw-r--r--   0        0        0     6496 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/bib_dedupe.py
--rw-r--r--   0        0        0     8465 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/block.py
--rw-r--r--   0        0        0      269 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/cli.py
--rw-r--r--   0        0        0     2795 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/cluster.py
--rw-r--r--   0        0        0      253 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/constants/__init__.py
--rw-r--r--   0        0        0      191 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/constants/colors.py
--rw-r--r--   0        0        0      490 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/constants/entrytypes.py
--rw-r--r--   0        0        0     1033 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/constants/fields.py
--rw-r--r--   0        0        0     2212 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/debug.py
--rw-r--r--   0        0        0    19499 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/dedupe_benchmark.py
--rw-r--r--   0        0        0   109747 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/journal_variants.csv
--rw-r--r--   0        0        0     5770 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/match.py
--rw-r--r--   0        0        0     5683 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/match_conditions.py
--rw-r--r--   0        0        0     5763 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/maybe_cases.py
--rw-r--r--   0        0        0     7871 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/merge.py
--rw-r--r--   0        0        0     7191 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/prep.py
--rw-r--r--   0        0        0     2071 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/prep_abstract.py
--rw-r--r--   0        0        0     9428 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/prep_author.py
--rw-r--r--   0        0        0     5719 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/prep_container_title.py
--rw-r--r--   0        0        0     1220 2024-04-16 19:30:23.006076 bib_dedupe-0.7.3/bib_dedupe/prep_doi.py
--rw-r--r--   0        0        0      817 2024-04-16 19:30:23.010076 bib_dedupe-0.7.3/bib_dedupe/prep_number.py
--rw-r--r--   0        0        0     2516 2024-04-16 19:30:23.010076 bib_dedupe-0.7.3/bib_dedupe/prep_pages.py
--rw-r--r--   0        0        0     5010 2024-04-16 19:30:23.010076 bib_dedupe-0.7.3/bib_dedupe/prep_title.py
--rw-r--r--   0        0        0     1374 2024-04-16 19:30:23.010076 bib_dedupe-0.7.3/bib_dedupe/prep_volume.py
--rw-r--r--   0        0        0      573 2024-04-16 19:30:23.010076 bib_dedupe-0.7.3/bib_dedupe/prep_year.py
--rw-r--r--   0        0        0    15071 2024-04-16 19:30:23.010076 bib_dedupe-0.7.3/bib_dedupe/sim.py
--rw-r--r--   0        0        0      836 2024-04-16 19:30:23.010076 bib_dedupe-0.7.3/bib_dedupe/util.py
--rw-r--r--   0        0        0     1637 2024-04-16 19:30:24.154071 bib_dedupe-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     4353 1970-01-01 00:00:00.000000 bib_dedupe-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/LICENSE
+-rw-r--r--   0        0        0     3867 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/README.md
+-rw-r--r--   0        0        0      411 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/__init__.py
+-rw-r--r--   0        0        0     6496 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/bib_dedupe.py
+-rw-r--r--   0        0        0     8465 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/block.py
+-rw-r--r--   0        0        0      269 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/cli.py
+-rw-r--r--   0        0        0     2795 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/cluster.py
+-rw-r--r--   0        0        0      253 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/constants/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/constants/colors.py
+-rw-r--r--   0        0        0      490 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/constants/entrytypes.py
+-rw-r--r--   0        0        0     1033 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/constants/fields.py
+-rw-r--r--   0        0        0     2212 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/debug.py
+-rw-r--r--   0        0        0    19504 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/dedupe_benchmark.py
+-rw-r--r--   0        0        0   109747 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/journal_variants.csv
+-rw-r--r--   0        0        0     5770 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/match.py
+-rw-r--r--   0        0        0     5683 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/match_conditions.py
+-rw-r--r--   0        0        0     5789 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/maybe_cases.py
+-rw-r--r--   0        0        0     7871 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/merge.py
+-rw-r--r--   0        0        0     7191 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep.py
+-rw-r--r--   0        0        0     2071 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_abstract.py
+-rw-r--r--   0        0        0     9428 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_author.py
+-rw-r--r--   0        0        0     5719 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_container_title.py
+-rw-r--r--   0        0        0     1220 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_doi.py
+-rw-r--r--   0        0        0      817 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_number.py
+-rw-r--r--   0        0        0     2516 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_pages.py
+-rw-r--r--   0        0        0     5010 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_title.py
+-rw-r--r--   0        0        0     1374 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_volume.py
+-rw-r--r--   0        0        0      573 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/prep_year.py
+-rw-r--r--   0        0        0    15071 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/sim.py
+-rw-r--r--   0        0        0      836 2024-04-29 05:22:57.930206 bib_dedupe-0.7.4/bib_dedupe/util.py
+-rw-r--r--   0        0        0     1541 2024-04-29 05:22:59.086204 bib_dedupe-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     5137 1970-01-01 00:00:00.000000 bib_dedupe-0.7.4/PKG-INFO
```

### Comparing `bib_dedupe-0.7.3/LICENSE` & `bib_dedupe-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/README.md` & `bib_dedupe-0.7.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,21 @@
+<div align="center">
+
 # BibDedupe
 
+
 <!-- [![License](https://img.shields.io/github/license/CoLRev-Ecosystem/bib-dedupe.svg)](https://github.com/CoLRev-Environment/bib-dedupe/releases/) -->
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bib-dedupe)
 [![status](https://joss.theoj.org/papers/b954027d06d602c106430e275fe72130/status.svg)](https://joss.theoj.org/papers/b954027d06d602c106430e275fe72130)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bib-dedupe)<br>
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/CoLRev-Environment/bib-dedupe/.github%2Fworkflows%2Ftests.yml?label=tests)](https://github.com/CoLRev-Environment/bib-dedupe/actions/workflows/tests.yml)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/CoLRev-Environment/bib-dedupe/.github%2Fworkflows%2Fdocs.yml?label=docs)](https://github.com/CoLRev-Environment/bib-dedupe/actions/workflows/docs.yml)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/CoLRev-Environment/bib-dedupe/.github%2Fworkflows%2Fevaluate.yml?label=continuous%20evaluation)](https://github.com/CoLRev-Environment/bib-dedupe/actions/workflows/evaluate.yml)
 
+</div>
 
 ## Overview
 
 BibDedupe is an open-source **Python library for deduplication of bibliographic records**, tailored for literature reviews.
 Unlike traditional deduplication methods, BibDedupe focuses on entity resolution, linking duplicate records instead of simply deleting them.
 
 ## Features
```

### Comparing `bib_dedupe-0.7.3/bib_dedupe/bib_dedupe.py` & `bib_dedupe-0.7.4/bib_dedupe/bib_dedupe.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/block.py` & `bib_dedupe-0.7.4/bib_dedupe/block.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/cluster.py` & `bib_dedupe-0.7.4/bib_dedupe/cluster.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/constants/fields.py` & `bib_dedupe-0.7.4/bib_dedupe/constants/fields.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/debug.py` & `bib_dedupe-0.7.4/bib_dedupe/debug.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/dedupe_benchmark.py` & `bib_dedupe-0.7.4/bib_dedupe/dedupe_benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -402,30 +402,29 @@
                 results[FP] += 1
                 results[TP] += len(true_merged_id_set) - 1
             elif nr_in_merged_df >= 1:
                 results[TN] += 1
                 results[FN] += nr_in_merged_df - 1
                 results[TP] += len(true_merged_id_set) - nr_in_merged_df
 
-        specificity = results[TN] / (results[TN] + results[FP])
-        sensitivity = results[TP] / (results[TP] + results[FN])
-
         results[FP_RATE] = results[FP] / (results[FP] + results[TN])
 
-        results[SPECIFICITY] = specificity
-        results[SENSITIVITY] = sensitivity
+        results[SPECIFICITY] = results[TN] / (results[TN] + results[FP])
+        results[SENSITIVITY] = results[TP] / (results[TP] + results[FN])
         if (results[TP] + results[FP]) > 0:
             results[PRECISION] = results[TP] / (results[TP] + results[FP])
+        else:
+            results[PRECISION] = 0.0
+        if (results[PRECISION] + results[SENSITIVITY]) > 0:
             results[F1] = (
                 2
                 * (results[PRECISION] * results[SENSITIVITY])
                 / (results[PRECISION] + results[SENSITIVITY])
             )
         else:
-            results[PRECISION] = 0.0
             results[F1] = 0.0
 
         results["dataset"] = Path(self.benchmark_path).name
 
         return results
 
     def export_cases(
```

### Comparing `bib_dedupe-0.7.3/bib_dedupe/journal_variants.csv` & `bib_dedupe-0.7.4/bib_dedupe/journal_variants.csv`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/match.py` & `bib_dedupe-0.7.4/bib_dedupe/match.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/match_conditions.py` & `bib_dedupe-0.7.4/bib_dedupe/match_conditions.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/maybe_cases.py` & `bib_dedupe-0.7.4/bib_dedupe/maybe_cases.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,21 +69,22 @@
     # consider only one link between clusters (the first ID of duplicate_id_clusters)
     duplicate_id_dict = {
         i: duplicate_id_cluster[0]
         for duplicate_id_cluster in duplicate_id_clusters
         for i in duplicate_id_cluster
         if i != duplicate_id_cluster[0]
     }
-    maybe_df = matched_df[matched_df[DUPLICATE_LABEL] == MAYBE]
-    maybe_df[f"{ID}_1"] = (
+    maybe_df = matched_df.loc[matched_df[DUPLICATE_LABEL] == MAYBE].copy()
+    maybe_df.loc[:, f"{ID}_1"] = (
         maybe_df[f"{ID}_1"].map(duplicate_id_dict).fillna(maybe_df[f"{ID}_1"])
     )
-    maybe_df[f"{ID}_2"] = (
+    maybe_df.loc[:, f"{ID}_2"] = (
         maybe_df[f"{ID}_2"].map(duplicate_id_dict).fillna(maybe_df[f"{ID}_2"])
     )
+
     maybe_df = maybe_df.drop_duplicates(subset=[f"{ID}_1", f"{ID}_2"])
 
     maybe_id_pairs = maybe_df[[f"{ID}_1", f"{ID}_2"]].values.tolist()
     maybe_id_pairs = [pair for pair in maybe_id_pairs if pair[0] != pair[1]]
 
     maybe_cases_df = pd.DataFrame()
     maybe_cases_df.loc[:, ID] = [id for sublist in maybe_id_pairs for id in sublist]
```

### Comparing `bib_dedupe-0.7.3/bib_dedupe/merge.py` & `bib_dedupe-0.7.4/bib_dedupe/merge.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/prep.py` & `bib_dedupe-0.7.4/bib_dedupe/prep.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/prep_abstract.py` & `bib_dedupe-0.7.4/bib_dedupe/prep_abstract.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/prep_author.py` & `bib_dedupe-0.7.4/bib_dedupe/prep_author.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/prep_container_title.py` & `bib_dedupe-0.7.4/bib_dedupe/prep_container_title.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/prep_doi.py` & `bib_dedupe-0.7.4/bib_dedupe/prep_doi.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/prep_number.py` & `bib_dedupe-0.7.4/bib_dedupe/prep_number.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/prep_pages.py` & `bib_dedupe-0.7.4/bib_dedupe/prep_pages.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/prep_title.py` & `bib_dedupe-0.7.4/bib_dedupe/prep_title.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/prep_volume.py` & `bib_dedupe-0.7.4/bib_dedupe/prep_volume.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/prep_year.py` & `bib_dedupe-0.7.4/bib_dedupe/prep_year.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/sim.py` & `bib_dedupe-0.7.4/bib_dedupe/sim.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/bib_dedupe/util.py` & `bib_dedupe-0.7.4/bib_dedupe/util.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.3/pyproject.toml` & `bib_dedupe-0.7.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bib-dedupe"
-version = "0.7.3"
+version = "0.7.4"
 description = "Identify and merge duplicates in bibliographic records"
 authors = ["Gerit Wagner <gerit.wagner@uni-bamberg.de>"]
 license = "MIT"
 readme = "README.md"
 
 [[tool.poetry.packages]]
 include = "bib_dedupe"
@@ -34,16 +34,14 @@
 [tool.mypy]
 python_version = 3.8
 warn_unused_configs = true
 ignore_missing_imports = true
 
 [[tool.mypy.overrides]]
 module = [
-    "requests.*",
-    "yaml.*",
     "pkg_resources.*",
 ]
 ignore_missing_imports = true
 
 [tool.pylint.'MESSAGES CONTROL']
 disable = ["R0801"]
 
@@ -53,22 +51,20 @@
     "/tmp/*",
     "tests/*",
 ]
 
 [tool.coverage.run]
 omit = [
     "/usr/*", # omit everything in /usr
-    "*crossrefapi/crossref/*",
     "/tmp/*",
     "tests/*",
 ]
 
 [tool.ruff]
 line-length = 160
 
 [tool.ruff.per-file-ignores]
 "**/{tests,docs}/*" = ["E501"]
 
 [build-system]
-# requires = ["poetry>=1.2.0b1"]
 requires = ["poetry-core>=1.0.0", "cython<3.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bib_dedupe-0.7.3/PKG-INFO` & `bib_dedupe-0.7.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bib-dedupe
-Version: 0.7.3
+Version: 0.7.4
 Summary: Identify and merge duplicates in bibliographic records
 License: MIT
 Author: Gerit Wagner
 Author-email: gerit.wagner@uni-bamberg.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,21 +25,28 @@
 Requires-Dist: pytest (>=7.2.1,<8.0.0) ; extra == "dev"
 Requires-Dist: rapidfuzz (>=3.5.2,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: setuptools (>=69.1.1,<70.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Description-Content-Type: text/markdown
 
+<div align="center">
+
 # BibDedupe
 
+
 <!-- [![License](https://img.shields.io/github/license/CoLRev-Ecosystem/bib-dedupe.svg)](https://github.com/CoLRev-Environment/bib-dedupe/releases/) -->
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bib-dedupe)
 [![status](https://joss.theoj.org/papers/b954027d06d602c106430e275fe72130/status.svg)](https://joss.theoj.org/papers/b954027d06d602c106430e275fe72130)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bib-dedupe)<br>
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/CoLRev-Environment/bib-dedupe/.github%2Fworkflows%2Ftests.yml?label=tests)](https://github.com/CoLRev-Environment/bib-dedupe/actions/workflows/tests.yml)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/CoLRev-Environment/bib-dedupe/.github%2Fworkflows%2Fdocs.yml?label=docs)](https://github.com/CoLRev-Environment/bib-dedupe/actions/workflows/docs.yml)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/CoLRev-Environment/bib-dedupe/.github%2Fworkflows%2Fevaluate.yml?label=continuous%20evaluation)](https://github.com/CoLRev-Environment/bib-dedupe/actions/workflows/evaluate.yml)
 
+</div>
 
 ## Overview
 
 BibDedupe is an open-source **Python library for deduplication of bibliographic records**, tailored for literature reviews.
 Unlike traditional deduplication methods, BibDedupe focuses on entity resolution, linking duplicate records instead of simply deleting them.
 
 ## Features
```

