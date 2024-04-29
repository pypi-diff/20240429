# Comparing `tmp/acasclient-2023.4.1.tar.gz` & `tmp/acasclient-2024.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acasclient-2023.4.1.tar", last modified: Fri Mar  8 17:24:39 2024, max compression
+gzip compressed data, was "acasclient-2024.1.0.tar", last modified: Wed Mar 13 16:31:15 2024, max compression
```

## Comparing `acasclient-2023.4.1.tar` & `acasclient-2024.1.0.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:24:39.076402 acasclient-2023.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-08 17:24:30.000000 acasclient-2023.4.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-03-08 17:24:30.000000 acasclient-2023.4.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-08 17:24:30.000000 acasclient-2023.4.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-08 17:24:30.000000 acasclient-2023.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-08 17:24:30.000000 acasclient-2023.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-08 17:24:39.076402 acasclient-2023.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-08 17:24:30.000000 acasclient-2023.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:24:39.052402 acasclient-2023.4.1/acasclient/
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-03-08 17:24:30.000000 acasclient-2023.4.1/acasclient/CmpdReg.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-08 17:24:30.000000 acasclient-2023.4.1/acasclient/StereoCategory.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-08 17:24:30.000000 acasclient-2023.4.1/acasclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    93837 2024-03-08 17:24:30.000000 acasclient-2023.4.1/acasclient/acasclient.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-08 17:24:30.000000 acasclient-2023.4.1/acasclient/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-03-08 17:24:30.000000 acasclient-2023.4.1/acasclient/ddict.py
--rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-03-08 17:24:30.000000 acasclient-2023.4.1/acasclient/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-03-08 17:24:30.000000 acasclient-2023.4.1/acasclient/interactions.py
--rw-r--r--   0 runner    (1001) docker     (127)   106612 2024-03-08 17:24:30.000000 acasclient-2023.4.1/acasclient/lsthing.py
--rw-r--r--   0 runner    (1001) docker     (127)    31011 2024-03-08 17:24:30.000000 acasclient-2023.4.1/acasclient/selfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-03-08 17:24:30.000000 acasclient-2023.4.1/acasclient/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:24:39.076402 acasclient-2023.4.1/acasclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-08 17:24:39.000000 acasclient-2023.4.1/acasclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-03-08 17:24:39.000000 acasclient-2023.4.1/acasclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 17:24:39.000000 acasclient-2023.4.1/acasclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-08 17:24:39.000000 acasclient-2023.4.1/acasclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 17:24:38.000000 acasclient-2023.4.1/acasclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-08 17:24:39.000000 acasclient-2023.4.1/acasclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-08 17:24:39.000000 acasclient-2023.4.1/acasclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:24:39.056402 acasclient-2023.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-08 17:24:30.000000 acasclient-2023.4.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-08 17:24:30.000000 acasclient-2023.4.1/docs/acasclient.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-08 17:24:30.000000 acasclient-2023.4.1/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4811 2024-03-08 17:24:30.000000 acasclient-2023.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-08 17:24:30.000000 acasclient-2023.4.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-08 17:24:30.000000 acasclient-2023.4.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-08 17:24:30.000000 acasclient-2023.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-08 17:24:30.000000 acasclient-2023.4.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-08 17:24:30.000000 acasclient-2023.4.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-08 17:24:30.000000 acasclient-2023.4.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-08 17:24:30.000000 acasclient-2023.4.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-08 17:24:30.000000 acasclient-2023.4.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-08 17:24:39.076402 acasclient-2023.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-08 17:24:30.000000 acasclient-2023.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:24:39.056402 acasclient-2023.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/project_thing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 17:24:39.076402 acasclient-2023.4.1/tests/test_acasclient/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/12_1_MultipleImage.csv
--rw-r--r--   0 runner    (1001) docker     (127)   261659 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/12_2_MultipleImage.zip
--rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/1_1_Generic-XLS_50_1995_Fail.xls
--rw-r--r--   0 runner    (1001) docker     (127)    29696 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/1_1_Generic.xls
--rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/1_1_Generic.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)    13082 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/1_1_Generic_empty_column.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/4 parameter D-R-validation-no-flags.csv
--rw-r--r--   0 runner    (1001) docker     (127)    43203 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/4 parameter D-R-validation.csv
--rw-r--r--   0 runner    (1001) docker     (127)    68873 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/4 parameter D-R.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2442910 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/50k-lines.csv
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/blob_test.png
--rw-r--r--   0 runner    (1001) docker     (127)    13264 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/dummy.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/dummy2.PDF
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/escaped_quotes.csv
--rw-r--r--   0 runner    (1001) docker     (127)    29184 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/escaped_quotes.xls
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/ibuprofen_big_lot_number.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/ibuprofen_methyl_ester.sdf
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/infinite-numeric-values.csv
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/malformatted-single-quote.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1000988 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/nci1000.sdf
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/non-uniform-commas-with-quoted-text.csv
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/quoted-with-new-line-character-in-string.csv
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/same-header-different-data-types.csv
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/test_000_creds_from_file_credentials
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/test_005_swap_parent_structures.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/test_012_register_sdf.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/test_045_register_sdf_case_insensitive.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/test_047_register_sdf_with_salts.sdf
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/test_048_warn_existing_compound_new_id.sdf
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/test_048_warn_existing_compound_new_id_two.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/test_051_register_parent_aliases.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/test_051_register_parent_aliases_copy.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/test_051_register_parent_aliases_diff_aliases.sdf
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/test_051_register_parent_aliases_overlap_aliases.sdf
--rw-r--r--   0 runner    (1001) docker     (127)  5477940 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/test_dose_response_experiment_loader_accepted_results.json
--rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/test_new_line_character_in_string_experiment_loader_accepted_results.json
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/text_010_partial_parent_aliases.sdf
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient/uniform-commas-with-quoted-text.csv
--rw-r--r--   0 runner    (1001) docker     (127)   219747 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_acasclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    49206 2024-03-08 17:24:30.000000 acasclient-2023.4.1/tests/test_lsthing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:31:15.560480 acasclient-2024.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-13 16:31:07.000000 acasclient-2024.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-03-13 16:31:07.000000 acasclient-2024.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-13 16:31:07.000000 acasclient-2024.1.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-03-13 16:31:07.000000 acasclient-2024.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-13 16:31:07.000000 acasclient-2024.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-13 16:31:15.560480 acasclient-2024.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-13 16:31:07.000000 acasclient-2024.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:31:15.536480 acasclient-2024.1.0/acasclient/
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-03-13 16:31:07.000000 acasclient-2024.1.0/acasclient/CmpdReg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-13 16:31:07.000000 acasclient-2024.1.0/acasclient/StereoCategory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-13 16:31:07.000000 acasclient-2024.1.0/acasclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95804 2024-03-13 16:31:07.000000 acasclient-2024.1.0/acasclient/acasclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-13 16:31:07.000000 acasclient-2024.1.0/acasclient/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-03-13 16:31:07.000000 acasclient-2024.1.0/acasclient/ddict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-03-13 16:31:07.000000 acasclient-2024.1.0/acasclient/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-03-13 16:31:07.000000 acasclient-2024.1.0/acasclient/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106612 2024-03-13 16:31:07.000000 acasclient-2024.1.0/acasclient/lsthing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31011 2024-03-13 16:31:07.000000 acasclient-2024.1.0/acasclient/selfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-03-13 16:31:07.000000 acasclient-2024.1.0/acasclient/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:31:15.556480 acasclient-2024.1.0/acasclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-03-13 16:31:15.000000 acasclient-2024.1.0/acasclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-03-13 16:31:15.000000 acasclient-2024.1.0/acasclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 16:31:15.000000 acasclient-2024.1.0/acasclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-13 16:31:15.000000 acasclient-2024.1.0/acasclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 16:31:15.000000 acasclient-2024.1.0/acasclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-13 16:31:15.000000 acasclient-2024.1.0/acasclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-13 16:31:15.000000 acasclient-2024.1.0/acasclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:31:15.540480 acasclient-2024.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-13 16:31:07.000000 acasclient-2024.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-13 16:31:07.000000 acasclient-2024.1.0/docs/acasclient.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-13 16:31:07.000000 acasclient-2024.1.0/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4811 2024-03-13 16:31:07.000000 acasclient-2024.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-13 16:31:07.000000 acasclient-2024.1.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-13 16:31:07.000000 acasclient-2024.1.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-13 16:31:07.000000 acasclient-2024.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-13 16:31:07.000000 acasclient-2024.1.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-13 16:31:07.000000 acasclient-2024.1.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-13 16:31:07.000000 acasclient-2024.1.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-13 16:31:07.000000 acasclient-2024.1.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-13 16:31:07.000000 acasclient-2024.1.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-13 16:31:15.560480 acasclient-2024.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-13 16:31:07.000000 acasclient-2024.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:31:15.540480 acasclient-2024.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/project_thing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 16:31:15.556480 acasclient-2024.1.0/tests/test_acasclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/12_1_MultipleImage.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   261659 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/12_2_MultipleImage.zip
+-rw-r--r--   0 runner    (1001) docker     (127)    18432 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/1_1_Generic-XLS_50_1995_Fail.xls
+-rw-r--r--   0 runner    (1001) docker     (127)    29696 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/1_1_Generic.xls
+-rw-r--r--   0 runner    (1001) docker     (127)    12878 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/1_1_Generic.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)    13082 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/1_1_Generic_empty_column.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/4 parameter D-R-validation-no-flags.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    43203 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/4 parameter D-R-validation.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    68873 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/4 parameter D-R.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2442910 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/50k-lines.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/blob_test.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13264 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/dummy.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     7478 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/dummy2.PDF
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/escaped_quotes.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    29184 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/escaped_quotes.xls
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/ibuprofen_big_lot_number.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/ibuprofen_methyl_ester.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/infinite-numeric-values.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/malformatted-single-quote.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1000988 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/nci1000.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/non-uniform-commas-with-quoted-text.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/quoted-with-new-line-character-in-string.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/same-header-different-data-types.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/test_000_creds_from_file_credentials
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/test_005_swap_parent_structures.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/test_012_register_sdf.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/test_045_register_sdf_case_insensitive.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/test_047_register_sdf_with_salts.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/test_048_warn_existing_compound_new_id.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/test_048_warn_existing_compound_new_id_two.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/test_051_register_parent_aliases.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/test_051_register_parent_aliases_copy.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/test_051_register_parent_aliases_diff_aliases.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/test_051_register_parent_aliases_overlap_aliases.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)  5477940 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/test_dose_response_experiment_loader_accepted_results.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/test_new_line_character_in_string_experiment_loader_accepted_results.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/test_simple_mol.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/text_010_partial_parent_aliases.sdf
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient/uniform-commas-with-quoted-text.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   234279 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_acasclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49206 2024-03-13 16:31:07.000000 acasclient-2024.1.0/tests/test_lsthing.py
```

### Comparing `acasclient-2023.4.1/CONTRIBUTING.rst` & `acasclient-2024.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/LICENSE` & `acasclient-2024.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/PKG-INFO` & `acasclient-2024.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acasclient
-Version: 2023.4.1
+Version: 2024.1.0
 Summary: ACAS API Client
 Home-page: https://github.com/mcneilco/acasclient
 Author: Brian Bolt
 Author-email: brian.bolt@boltengineered.com
 License: GNU General Public License v3
 Keywords: acasclient
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `acasclient-2023.4.1/README.rst` & `acasclient-2024.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/acasclient/CmpdReg.py` & `acasclient-2024.1.0/acasclient/CmpdReg.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/acasclient/StereoCategory.py` & `acasclient-2024.1.0/acasclient/StereoCategory.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/acasclient/acasclient.py` & `acasclient-2024.1.0/acasclient/acasclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 logger.setLevel(logging.INFO)
 
 VALID_STRUCTURE_SEARCH_TYPES = {"substructure", "duplicate",
                         "duplicate_tautomer", "duplicate_no_tautomer",
                         "stereo_ignore", "full_tautomer", "substructure",
                         "similarity", "full"}
 
+CORPORATE_BATCH_ID = "Corporate Batch ID"
+
 def isBase64(s):
     """Checks if a string is base64 encoded.
     """
     if not isinstance(s, str):
         return False
     return (len(s) % 4 == 0) and re.match('^[A-Za-z0-9+/]+[=]{0,2}$', s)
 
@@ -2440,7 +2442,52 @@
         # Otherwise continue to updateParent
         resp = self.session.post("{}/cmpdreg/updateParent".format(self.url),
                                  headers={'Content-Type': "application/json"},
                                  data=json.dumps(parent))
         resp.raise_for_status()
         resp_data = resp.json()
         return success, resp_data
+
+
+    def get_entity_reference_codes(self, entity_display_name: str, entity_requests: List[str]) -> List[Dict]:
+        """Get the reference codes for a given entity
+
+        Args:
+            entity_display_name (str): The display name of the entity (e.g. Corporate Batch ID)
+            entity_requests (List[str]): A list of entity request names (e.g. ["CMPD-0000001-001"])
+
+        Returns:
+            A list of dicts representing the reference codes for the entity requests e.g.
+            [
+                {
+                    "requestName": "CMPD-0000001-001",
+                    "referenceName": "CMPD-0000001-001"
+                }
+            ]
+        """
+        # Request body needs to be "displayName", "requests": [{"requestName": "entity_display_name1", "requestName": "entity_display_name2"}]
+        body = {
+            "displayName": entity_display_name,
+            "requests": [{"requestName": name} for name in entity_requests]
+        }
+        resp = self.session.post("{}/api/entitymeta/referenceCodes".format(self.url),
+                                 headers={'Content-Type': "application/json"},
+                                 data=json.dumps(body))
+        resp.raise_for_status()
+        return resp.json()['results']
+        
+    def get_preferred_lot_corp_names(self, lot_corp_names: List[str]) -> List[Dict]:
+        """Get the preferred lot corp names for a list of corp names
+
+        Args:
+            lot_corp_names (List[str]): A list of lot corp names (e.g. ["CMPD-0000001-001"])
+        
+        Returns:
+            A list of dicts representing the preferred lot corp names for the input corp names e.g.
+            [
+                {
+                    "requestName": "CMPD-0000001-001",
+                    "referenceName": "CMPD-0000001-001"
+                }
+            ]
+        """
+        return self.get_entity_reference_codes(CORPORATE_BATCH_ID, lot_corp_names)
```

### Comparing `acasclient-2023.4.1/acasclient/ddict.py` & `acasclient-2024.1.0/acasclient/ddict.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/acasclient/experiment.py` & `acasclient-2024.1.0/acasclient/experiment.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/acasclient/interactions.py` & `acasclient-2024.1.0/acasclient/interactions.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/acasclient/lsthing.py` & `acasclient-2024.1.0/acasclient/lsthing.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/acasclient/selfile.py` & `acasclient-2024.1.0/acasclient/selfile.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/acasclient/validation.py` & `acasclient-2024.1.0/acasclient/validation.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/acasclient.egg-info/PKG-INFO` & `acasclient-2024.1.0/acasclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acasclient
-Version: 2023.4.1
+Version: 2024.1.0
 Summary: ACAS API Client
 Home-page: https://github.com/mcneilco/acasclient
 Author: Brian Bolt
 Author-email: brian.bolt@boltengineered.com
 License: GNU General Public License v3
 Keywords: acasclient
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `acasclient-2023.4.1/acasclient.egg-info/SOURCES.txt` & `acasclient-2024.1.0/acasclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -72,9 +72,10 @@
 tests/test_acasclient/test_048_warn_existing_compound_new_id_two.sdf
 tests/test_acasclient/test_051_register_parent_aliases.sdf
 tests/test_acasclient/test_051_register_parent_aliases_copy.sdf
 tests/test_acasclient/test_051_register_parent_aliases_diff_aliases.sdf
 tests/test_acasclient/test_051_register_parent_aliases_overlap_aliases.sdf
 tests/test_acasclient/test_dose_response_experiment_loader_accepted_results.json
 tests/test_acasclient/test_new_line_character_in_string_experiment_loader_accepted_results.json
+tests/test_acasclient/test_simple_mol.sdf
 tests/test_acasclient/text_010_partial_parent_aliases.sdf
 tests/test_acasclient/uniform-commas-with-quoted-text.csv
```

### Comparing `acasclient-2023.4.1/docs/Makefile` & `acasclient-2024.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/docs/conf.py` & `acasclient-2024.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/docs/installation.rst` & `acasclient-2024.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/docs/make.bat` & `acasclient-2024.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/setup.py` & `acasclient-2024.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,10 +44,10 @@
     keywords='acasclient',
     name='acasclient',
     packages=find_packages(include=['acasclient', 'acasclient.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/mcneilco/acasclient',
-    version='2023.4.1',
+    version='2024.1.0',
     zip_safe=False,
 )
```

### Comparing `acasclient-2023.4.1/tests/project_thing.py` & `acasclient-2024.1.0/tests/project_thing.py`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/12_1_MultipleImage.csv` & `acasclient-2024.1.0/tests/test_acasclient/12_1_MultipleImage.csv`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/12_2_MultipleImage.zip` & `acasclient-2024.1.0/tests/test_acasclient/12_2_MultipleImage.zip`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/1_1_Generic-XLS_50_1995_Fail.xls` & `acasclient-2024.1.0/tests/test_acasclient/1_1_Generic-XLS_50_1995_Fail.xls`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/1_1_Generic.xls` & `acasclient-2024.1.0/tests/test_acasclient/1_1_Generic.xls`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/1_1_Generic.xlsx` & `acasclient-2024.1.0/tests/test_acasclient/1_1_Generic.xlsx`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/1_1_Generic_empty_column.xlsx` & `acasclient-2024.1.0/tests/test_acasclient/1_1_Generic_empty_column.xlsx`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/4 parameter D-R-validation-no-flags.csv` & `acasclient-2024.1.0/tests/test_acasclient/4 parameter D-R-validation-no-flags.csv`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/4 parameter D-R-validation.csv` & `acasclient-2024.1.0/tests/test_acasclient/4 parameter D-R-validation.csv`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/4 parameter D-R.csv` & `acasclient-2024.1.0/tests/test_acasclient/4 parameter D-R.csv`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/50k-lines.csv` & `acasclient-2024.1.0/tests/test_acasclient/50k-lines.csv`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/blob_test.png` & `acasclient-2024.1.0/tests/test_acasclient/blob_test.png`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/dummy.pdf` & `acasclient-2024.1.0/tests/test_acasclient/dummy.pdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/dummy2.PDF` & `acasclient-2024.1.0/tests/test_acasclient/dummy2.PDF`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/escaped_quotes.csv` & `acasclient-2024.1.0/tests/test_acasclient/escaped_quotes.csv`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/escaped_quotes.xls` & `acasclient-2024.1.0/tests/test_acasclient/escaped_quotes.xls`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/ibuprofen_big_lot_number.sdf` & `acasclient-2024.1.0/tests/test_acasclient/ibuprofen_big_lot_number.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/ibuprofen_methyl_ester.sdf` & `acasclient-2024.1.0/tests/test_acasclient/ibuprofen_methyl_ester.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/nci1000.sdf` & `acasclient-2024.1.0/tests/test_acasclient/nci1000.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/test_005_swap_parent_structures.sdf` & `acasclient-2024.1.0/tests/test_acasclient/test_005_swap_parent_structures.sdf`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 C5 H11 Cl
 
 >  <Parent Registration Date>
 2022-07-23
 
 >  <Parent Comment>
 
->  <Parent Aliases>
+>  <Parent Alias>
 alias-2
 
 $$$$
 
   -INDIGO-07232218072D
 
   6  5  0  0  1  0  0  0  0  0999 V2000
@@ -196,15 +196,15 @@
 C5 H11 Cl
 
 >  <Parent Registration Date>
 2022-07-23
 
 >  <Parent Comment>
 
->  <Parent Aliases>
+>  <Parent Alias>
 alias-3
 
 $$$$
 
   -INDIGO-07232218072D
 
  11 11  0  0  1  0  0  0  0  0999 V2000
@@ -310,15 +310,15 @@
 C10 H19 F
 
 >  <Parent Registration Date>
 2022-07-23
 
 >  <Parent Comment>
 
->  <Parent Aliases>
+>  <Parent Alias>
 alias-6; alias-6a;
 
 $$$$
 
   -INDIGO-07232218072D
 
  11 11  0  0  1  0  0  0  0  0999 V2000
@@ -424,16 +424,16 @@
 C10 H19 F
 
 >  <Parent Registration Date>
 2022-07-23
 
 >  <Parent Comment>
 
->  <Parent Aliases>
-alias-4
+>  <Parent Alias>
+alias-4-a
 
 $$$$
 
   -INDIGO-07232218072D
 
   4  4  0  0  0  0  0  0  0  0999 V2000
     4.4000   -5.4250    0.0000 C   0  0  0  0  0  0  0  0  0  0  0  0
@@ -524,15 +524,15 @@
 C4 H8
 
 >  <Parent Registration Date>
 2022-07-23
 
 >  <Parent Comment>
 
->  <Parent Aliases>
+>  <Parent Alias>
 alias-4
 
 $$$$
 
   -INDIGO-07232218072D
 
   6  5  0  0  1  0  0  0  0  0999 V2000
@@ -627,11 +627,11 @@
 C5 H11 Cl
 
 >  <Parent Registration Date>
 2022-07-23
 
 >  <Parent Comment>
 
->  <Parent Aliases>
+>  <Parent Alias>
 alias-1
 
 $$$$
```

### Comparing `acasclient-2023.4.1/tests/test_acasclient/test_012_register_sdf.sdf` & `acasclient-2024.1.0/tests/test_acasclient/test_012_register_sdf.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/test_045_register_sdf_case_insensitive.sdf` & `acasclient-2024.1.0/tests/test_acasclient/test_045_register_sdf_case_insensitive.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/test_047_register_sdf_with_salts.sdf` & `acasclient-2024.1.0/tests/test_acasclient/test_047_register_sdf_with_salts.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/test_048_warn_existing_compound_new_id.sdf` & `acasclient-2024.1.0/tests/test_acasclient/test_048_warn_existing_compound_new_id.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/test_048_warn_existing_compound_new_id_two.sdf` & `acasclient-2024.1.0/tests/test_acasclient/test_048_warn_existing_compound_new_id_two.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/test_051_register_parent_aliases.sdf` & `acasclient-2024.1.0/tests/test_acasclient/test_051_register_parent_aliases.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/test_051_register_parent_aliases_copy.sdf` & `acasclient-2024.1.0/tests/test_acasclient/test_051_register_parent_aliases_copy.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/test_051_register_parent_aliases_diff_aliases.sdf` & `acasclient-2024.1.0/tests/test_acasclient/test_051_register_parent_aliases_diff_aliases.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/test_051_register_parent_aliases_overlap_aliases.sdf` & `acasclient-2024.1.0/tests/test_acasclient/test_051_register_parent_aliases_overlap_aliases.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/test_dose_response_experiment_loader_accepted_results.json` & `acasclient-2024.1.0/tests/test_acasclient/test_dose_response_experiment_loader_accepted_results.json`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/test_new_line_character_in_string_experiment_loader_accepted_results.json` & `acasclient-2024.1.0/tests/test_acasclient/test_new_line_character_in_string_experiment_loader_accepted_results.json`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient/text_010_partial_parent_aliases.sdf` & `acasclient-2024.1.0/tests/test_acasclient/text_010_partial_parent_aliases.sdf`

 * *Files identical despite different names*

### Comparing `acasclient-2023.4.1/tests/test_acasclient.py` & `acasclient-2024.1.0/tests/test_acasclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -278,39 +278,51 @@
 def get_or_create_global_project():
     """ Creates a global project for testing purposes """
     r = requests.get(ACAS_NODEAPI_BASE_URL + "/api/systemTest/getOrCreateGlobalProject")
     r.raise_for_status()
     output = r.json()
     return output["messages"]
 
+def delete_all_lots_and_experiments(self):
+    """ Deletes all lots and experiments """
+    lots = self.client.get_all_lots()
+    if len(lots) > 0:
+        self.delete_all_experiments()
+        self.delete_all_cmpd_reg_bulk_load_files()
+        # Check lots again
+        lots = self.client.get_all_lots()
+        if len(lots) > 0:
+            # Delete any remaining lots not from bulk loads
+            for lot in lots:
+                self.client.delete_lot(lot['lotCorpName'])
+
 def requires_basic_cmpd_reg_load(func):
     """
     Decorator to load the basic cmpdreg data if it is not already loaded
     """
     @wraps(func)
     def wrapper(self):
         if self.client.get_meta_lot('CMPD-0000001-001') is None or self.client.get_meta_lot('CMPD-0000002-001') is None:
+            # Delete everything to be safe
+            delete_all_lots_and_experiments(self)
             response = self.basic_cmpd_reg_load()
             # Verify they were loaded
             self.assertIn('New compounds: 2', response['summary'])
             if self.client.get_meta_lot('CMPD-0000001-001') is None or self.client.get_meta_lot('CMPD-0000002-001') is None:
                 raise AssertionError(f"Expected compound lots were not found after basic_cmpd_reg_load. Something has gone seriously wrong! Bulk load response: {response}")
         return func(self)
     return wrapper
 
 def requires_absent_basic_cmpd_reg_load(func):
     """
     Decorator to load the basic cmpdreg data if it is not already loaded
     """
     @wraps(func)
     def wrapper(self):
-        lots = self.client.get_all_lots()
-        if len(lots) > 0:
-            self.delete_all_experiments()
-            self.delete_all_cmpd_reg_bulk_load_files()
+        delete_all_lots_and_experiments(self)
         return func(self)   
     return wrapper
 
 def requires_basic_experiment_load(func):
     """
     Decorator to load the basic experiment data if it is not already loaded, returns None as a fallback if the experiment is not loaded
     """
@@ -826,15 +838,15 @@
                     "required": False,
                     "sdfProperty": "Lot Salt Equivalents"
                 },
                 {
                     "dbProperty": "Parent Alias",
                     "defaultVal": None,
                     "required": False,
-                    "sdfProperty": "Parent Aliases"
+                    "sdfProperty": "Parent Alias"
                 }
             ]
 
         response = self.client.register_sdf(file, "bob",
                                             mappings)
         return response
 
@@ -857,14 +869,43 @@
     
     def _create_dupe_codetable(self, create_method, code, name):
         with self.assertRaises(requests.HTTPError) as context:
             resp = create_method(code=code, name=name)
         self.assertIn('409 Client Error: Conflict', str(context.exception))
 
 
+    def create_restricted_lot(self, project_code):
+        # Bulk load a compound to the restricted project
+        response = self.basic_cmpd_reg_load(project_code)
+        # Assert that the are no errors in the response results level
+        all_lots = self.client.get_all_lots()
+
+        # Sort lots by id and get the latest corp id
+        # This is because we dont' get the corp id in the response from the bulkload
+        all_lots = sorted(all_lots, key=lambda lot: lot['id'])
+        global_project_parent_corp_name = all_lots[0]['parentCorpName']
+
+        # Find the lot that was bulk loaded with the same corp name as the global project
+        restricted_project_lot = [lot for lot in all_lots if lot['parentCorpName'] == global_project_parent_corp_name][-1]
+        restricted_lot_corp_name = restricted_project_lot["lotCorpName"]
+
+        return restricted_lot_corp_name
+
+    def check_lot_exists_in_experiment(self, lot_corp_name, experiment_code_name):
+        experiment = self.client.get_experiment_by_code(experiment_code_name, full = True)
+        # when experiment is deleted, the analysis groups for the lot are deleted
+        for analysis_group in experiment["analysisGroups"]:
+            if analysis_group["deleted"] == True or analysis_group["ignored"] == True:
+                continue
+            for state in analysis_group["lsStates"]:
+                for value in state["lsValues"]:
+                    if value["lsKind"] == "batch code" and value["codeValue"] == lot_corp_name:
+                        return True
+        return False
+
 class TestAcasclient(BaseAcasClientTest):
     """Tests for `acasclient` package."""
 
     def test_000_creds_from_file(self):
         """Test creds from file."""
         file_credentials = Path(__file__).resolve().\
             parent.joinpath('test_acasclient',
@@ -2065,18 +2106,20 @@
         self.client.update_author_roles(author_roles_to_delete=roles_to_remove)
         # Confirm a role was revoked
         updated_author = self.client.get_author_by_username(new_author['userName'])
         self.assertEqual(len(updated_author['authorRoles']), 1)
         role = updated_author['authorRoles'][0]['roleEntry']
         self.assertEqual(role['roleName'], 'ROLE_ACAS-USERS')
         # Try adding a role by updating the author
-        # Unfortunately we need to hardcode the id of the role, or fetch it from the server
+        # We need to fetch the lsRole id from the server
+        ls_roles = self.client.session.get(self.client.url + '/api/lsRoles/codeTable').json()
+        cmpdreg_role_id = [role for role in ls_roles if role['code'] == 'System_CmpdReg_ROLE_CMPDREG-USERS'][0]['id']
         nested_cmpdreg_role = {
             'roleEntry': {
-                'id': 3,
+                'id': cmpdreg_role_id,
                 'lsType': 'System',
                 'lsKind': 'CmpdReg',
                 'roleName': 'ROLE_CMPDREG-USERS',
             }
         }
         updated_author['authorRoles'].append(nested_cmpdreg_role)
         self.client.update_author(updated_author)
@@ -2518,15 +2561,15 @@
         # There are two warnings expected here: only one is related to the feature we are testing here
         self.assertIn('Number of warnings: 2', response['summary'])
         self.assertIn('New compounds: 1', response['summary'])
         self.assertIn('New parent will be assigned due to different stereo category', response['summary'])
         return response
 
     @requires_absent_basic_cmpd_reg_load
-    def test_049_register_large_sdf_with_error(self):
+    def skip_049_register_large_sdf_with_error(self):
         # Large request to test performance and error handling
         file = Path(__file__).resolve().parent\
             .joinpath('test_acasclient', 'nci1000.sdf')
         try:
             # SDF load of 1000 structures should take less than 60 seconds
             # to complete. On my machine it takes 30 seconds.
             # This is a performance check to make sure the
@@ -2857,15 +2900,15 @@
     def test_056_additional_assay_scientists(self):
         """Testing additional assay scientists."""
 
         # Test getting the current assay scientists
         assay_scientists = self.client.get_assay_scientists()
 
         # Verify bob is in the list
-        self.assertEqual(1, len([x for x in assay_scientists if x['code'] == 'bob']))
+        self.assertGreaterEqual(len([x for x in assay_scientists if x['code'] == 'bob']), 1)
 
         # Create a new assay scientist code and name using uuid
         new_assay_scientist_code = str(uuid.uuid4())
         new_assay_scientist_name = str(uuid.uuid4())
 
         # Test create new scientist
         resp = self.client.create_assay_scientist(new_assay_scientist_code, new_assay_scientist_name)
@@ -2929,31 +2972,22 @@
     with open(data_file_to_upload, 'r') as f:
         with open(file_path, 'w') as f2:
             for line in f:
                 f2.write(line.replace(',', "\t"))
     return file_path
 
 class TestCmpdReg(BaseAcasClientTest):
-
-    def create_restricted_lot(self, project_code):
-        # Bulk load a compound to the restricted project
-        response = self.basic_cmpd_reg_load(project_code)
-        # Assert that the are no errors in the response results level
-        all_lots = self.client.get_all_lots()
-
-        # Sort lots by id and get the latest corp id
-        # This is because we dont' get the corp id in the response from the bulkload
-        all_lots = sorted(all_lots, key=lambda lot: lot['id'])
-        global_project_parent_corp_name = all_lots[0]['parentCorpName']
-
-        # Find the lot that was bulk loaded with the same corp name as the global project
-        restricted_project_lot = [lot for lot in all_lots if lot['parentCorpName'] == global_project_parent_corp_name][-1]
-        restricted_lot_corp_name = restricted_project_lot["lotCorpName"]
-
-        return restricted_lot_corp_name
+        
+    def get_first_parent_alias_type_kind(self):
+        """Get the first alias type kind from a lot."""
+        parent_alias_kinds = self.client.get_parent_alias_kinds()
+        self.assertGreater(len(parent_alias_kinds), 0)
+        alias_type = parent_alias_kinds[0]["kindName"]
+        alias_kind = parent_alias_kinds[0]["lsType"]['typeName']
+        return alias_type, alias_kind
 
     @requires_node_api
     @requires_basic_cmpd_reg_load
     def test_001_get_meta_lot(self):
         """Test get meta lot."""
         # The default user is 'bob' and bob has cmpdreg admin role
         # The basic cmpdreg load has a lot registered that is unrestricted (Global project)
@@ -3285,26 +3319,14 @@
                 response = user_client.delete_lot(lot_corp_name)
             except requests.HTTPError:
                 return False
             self.assertIn("success", response)
             self.assertTrue(response['success'])
             return True
 
-        def check_lot_exists_in_experiment(self, lot_corp_name, experiment_code_name):
-            experiment = self.client.get_experiment_by_code(experiment_code_name, full = True)
-            # when experiment is deleted, the analysis groups for the lot are deleted
-            for analysis_group in experiment["analysisGroups"]:
-                if analysis_group["deleted"] == True or analysis_group["ignored"] == True:
-                    continue
-                for state in analysis_group["lsStates"]:
-                    for value in state["lsValues"]:
-                        if value["lsKind"] == "batch code" and value["codeValue"] == lot_corp_name:
-                            return True
-            return False
-
         # Deny Rule: Not an ACAS user and there is assay data for the lot
         self.assertFalse(can_delete_lot(self, cmpdreg_admin, "CMPD-0000001-001", set_owner_first=True))
 
         # Delete the assay data on the lot
         response = self.client.delete_experiment(experiment["codeName"])
 
         ## Deny Rule: Not a Creg admin and disableDeleteMyLots=true by default
@@ -3325,15 +3347,15 @@
         restricted_lot_corp_name = self.create_restricted_lot(project.code_name)
 
         # Load an experiment to the newly created restricted project using the restricted lot
         restricted_lot_corp_name = self.create_restricted_lot(project.code_name)
         file_to_upload = get_basic_experiment_load_file(self.tempdir, project.names[PROJECT_NAME], restricted_lot_corp_name, file_name='4 parameter D-R.csv')
         response = self.client.\
             experiment_loader(file_to_upload, "bob", False)
-        self.assertTrue(check_lot_exists_in_experiment(self, restricted_lot_corp_name, response['results']['experimentCode']))
+        self.assertTrue(self.check_lot_exists_in_experiment(restricted_lot_corp_name, response['results']['experimentCode']))
                         
         # Deny rule: Creg admin is not an acas user
         self.assertFalse(can_delete_lot(self, cmpdreg_admin, restricted_lot_corp_name, set_owner_first=True))
  
         # Deny rule: ACAS admin is not a creg admin
         self.assertFalse(can_delete_lot(self, acas_admin, restricted_lot_corp_name, set_owner_first=True))
 
@@ -3341,15 +3363,15 @@
         self.assertTrue(can_delete_lot(self, self.client, restricted_lot_corp_name, set_owner_first=True))
 
         # Verify lot is actually deleted
         meta_lot = self.client.get_meta_lot(restricted_lot_corp_name)
         self.assertIsNone(meta_lot)
 
         # Get the experiment and verify the lot is deleted
-        self.assertFalse(check_lot_exists_in_experiment(self, restricted_lot_corp_name, response['results']['experimentCode']))
+        self.assertFalse(self.check_lot_exists_in_experiment(restricted_lot_corp_name, response['results']['experimentCode']))
 
         # TODO: The following tests are dependent on a non default configuration: client.cmpdreg.metaLot.disableDeleteMyLots = false so we can't test this by default. We should turn this back on when we have a testing system which can change the configurations of acas.
         # # Global compound, with experiment in Global project
         # ## Deny Rule: Not an acas user so can't delete because dependent experiment exists
         # self.assertFalse(can_delete_lot(self, cmpdreg_user, "CMPD-0000001-001", set_owner_first=True))
 
         # ## Allow Rule: An acas user with access to delete global experiment and global compound
@@ -3411,15 +3433,15 @@
             'test_acasclient', 'test_005_swap_parent_structures.sdf')
         self.basic_cmpd_reg_load(file=file)
 
         # CMPD-0000001 / alias-1 (structure: A, stereo category: Single stereoisomer)
         # CMPD-0000002 / alias-2 (structure: A'(stereoisomer of 1), stereo category: Single stereoisomer)
         # CMPD-0000003 / alias-3 (structure: A'(stereoisomer of 1), stereo category: Single stereoisomer - arbitrary assign)
         # CMPD-0000004 / alias-4 (structure: B, stereo category: Single stereoisomer)
-        # CMPD-0000005 / alias-4(structure: C, stereo category: Unknown, stereo comment: foo)
+        # CMPD-0000005 / alias-4-a(structure: C, stereo category: Unknown, stereo comment: foo)
         # CMPD-0000006 / alias-6, alias-6a(structure: C'(stereoisomer of 5), stereo category: Unknown, stereo comment: foo)
 
         def _get_mol_weights_and_formula(lot_corp_name):
             meta_lot = self.client.get_meta_lot(lot_corp_name)
             lot = meta_lot["lot"]
             parent = lot["parent"]
             return parent["molWeight"], lot["lotMolWeight"], parent["molFormula"]
@@ -3498,21 +3520,22 @@
             self.assertEqual(response["errorMessage"], exp_error_msg)
 
             # Swap unique aliases.
             response = self.client.swap_parent_structures(
                 corp_name1='alias-1', corp_name2='alias-2')
             self.assertFalse(response["hasError"])
 
+            # REMOVED TEST BECAUSE BY DEFAULT ACAS NO LONGER ALLOWS LOADING DUPLICATE ALIAS BY DEFAULT
             # Swap a non-unique alias.
-            exp_error_msg = ("Alias name 'alias-4' has multiple corporate id matches: CMPD-0000004, CMPD-0000005")
-            response = self.client.swap_parent_structures(
-                corp_name1='CMPD-0000006', corp_name2='alias-4'
-            )
-            self.assertTrue(response["hasError"])
-            self.assertEqual(response["errorMessage"], exp_error_msg)
+            # exp_error_msg = ("Alias name 'alias-4' has multiple corporate id matches: CMPD-0000004, CMPD-0000005")
+            # response = self.client.swap_parent_structures(
+            #     corp_name1='CMPD-0000006', corp_name2='alias-4'
+            # )
+            # self.assertTrue(response["hasError"])
+            # self.assertEqual(response["errorMessage"], exp_error_msg)
 
             # Try making a valid swap as a non-admin and confirm it fails
             # due to permissions
             cmpdreg_user = self.create_and_connect_backdoor_user(acas_user=False, acas_admin=False, creg_user=True, creg_admin=False)
             with self.assertRaises(requests.HTTPError) as context:
                 response = cmpdreg_user.swap_parent_structures(
                     corp_name1='CMPD-0000001', corp_name2='CMPD-0000002')
@@ -3652,18 +3675,15 @@
 
         # Get aliases
         aliases = self.client.get_parent_aliases(corp_name)
         self.assertEqual(len(aliases), 1)
         self.assertEquals(aliases[0], alias_1)
 
         # Get parent alias kinds
-        parent_alias_kinds = self.client.get_parent_alias_kinds()
-        self.assertGreater(len(parent_alias_kinds), 0)
-        alias_type = parent_alias_kinds[0]["kindName"]
-        alias_kind = parent_alias_kinds[0]["lsType"]['typeName']
+        alias_type, alias_kind = self.get_first_parent_alias_type_kind()
 
         # Add an alias
         meta_lot = self.client.add_parent_alias(corp_name, test_alias, alias_type, alias_kind)
         aliases = self.client.get_parent_aliases(corp_name)
         self.assertEqual(len(aliases), 2)
         self.assertIn(alias_1, aliases)
         self.assertIn(test_alias, aliases)
@@ -3780,62 +3800,62 @@
             validation_status, validation_resp = self.client.edit_parent(parent, dry_run=True)
             # Confirm validation response mentions the lot
             self.assertTrue(validation_status)
             self.assertEquals(len(validation_resp), 1)
             self.assertEquals(validation_resp[0]['code'], 'CMPD-0000001-001')
             self.assertEquals(validation_resp[0]['name'], 'CMPD-0000001-001')
             # TODO Get this working reliably and uncomment it
-            # # Commit the edit
-            # edit_status, edit_resp = self.client.edit_parent(parent, dry_run=False)
-            # # Confirm edit response mentions the lot
-            # self.assertTrue(edit_status)
-            # self.assertEquals(len(edit_resp), 1)
-            # self.assertEquals(edit_resp[0]['code'], 'CMPD-0000001-001')
-            # self.assertEquals(edit_resp[0]['name'], 'CMPD-0000001-001')
-            # # Get the parent again and check out changes were made
-            # meta_lot = self.client.get_meta_lot('CMPD-0000001-001')
-            # parent = meta_lot['lot']['parent']
-            # self.assertEquals(parent['stereoComment'], TEST_STEREO_COMMENT)
-            # self.assertEquals(parent['stereoCategory']['code'], TEST_STEREO_CAT_CODE)
-            # # Confirm a non-admin cannot attempt a dry run edit
+            # Commit the edit
+            edit_status, edit_resp = self.client.edit_parent(parent, dry_run=False)
+            # Confirm edit response mentions the lot
+            self.assertTrue(edit_status)
+            self.assertEquals(len(edit_resp), 1)
+            self.assertEquals(edit_resp[0]['code'], 'CMPD-0000001-001')
+            self.assertEquals(edit_resp[0]['name'], 'CMPD-0000001-001')
+            # Get the parent again and check out changes were made
+            meta_lot = self.client.get_meta_lot('CMPD-0000001-001')
+            parent = meta_lot['lot']['parent']
+            self.assertEquals(parent['stereoComment'], TEST_STEREO_COMMENT)
+            self.assertEquals(parent['stereoCategory']['code'], TEST_STEREO_CAT_CODE)
+            # Confirm a non-admin cannot attempt a dry run edit
             # with self.assertRaises(requests.HTTPError) as context:
             #     cmpdreg_user.edit_parent(parent, dry_run=True)
             # self.assertIn('401 Client Error: Unauthorized for url', str(context.exception))
             # # Confirm a non-admin cannot edit
             # with self.assertRaises(requests.HTTPError) as context:
             #     cmpdreg_user.edit_parent(parent, dry_run=False)
             # self.assertIn('401 Client Error: Unauthorized for url', str(context.exception))
-            # # Edit back to how it was before and save
-            # parent['stereoComment'] = ORIG_STEREO_COMMENT
-            # parent['stereoCategory'] = stereo_cat_dict[ORIG_STEREO_CAT_CODE]
-            # edit_status, edit_resp = self.client.edit_parent(parent, dry_run=False)
-            # if not edit_status:
-            #     print(f"ERROR: Something went wrong editing the parent: {edit_resp}")
-            # self.assertTrue(edit_status)
-            # # Confirm attributes are back to as they were before
-            # meta_lot = self.client.get_meta_lot('CMPD-0000001-001')
-            # parent = meta_lot['lot']['parent']
-            # self.assertEquals(parent['stereoComment'], ORIG_STEREO_COMMENT)
-            # self.assertEquals(parent['stereoCategory']['code'], ORIG_STEREO_CAT_CODE)
-            # # Edit structure to match parent 2
-            # # This should result in a duplicate, and thus be blocked
-            # parent['molStructure'] = CMPD_2_STRUCTURE
-            # # Validate (should fail)
-            # validation_status, validation_resp = self.client.edit_parent(parent, dry_run=True)
-            # self.assertFalse(validation_status)
-            # self.assertFalse(validation_resp['parentUnique'])
-            # self.assertEquals(len(validation_resp['dupeParents']), 1)
-            # self.assertEquals(validation_resp['dupeParents'][0]['corpName'], 'CMPD-0000002')
-            # # Attempt non-dryrun (should fail)
-            # edit_status, edit_resp = self.client.edit_parent(parent, dry_run=False)
-            # self.assertFalse(edit_status)
-            # self.assertFalse(edit_status)
-            # self.assertFalse(edit_resp['parentUnique'])
-            # self.assertEquals(len(edit_resp['dupeParents']), 1)
-            # self.assertEquals(edit_resp['dupeParents'][0]['corpName'], 'CMPD-0000002')
+            # Edit back to how it was before and save
+            parent['stereoComment'] = ORIG_STEREO_COMMENT
+            parent['stereoCategory'] = stereo_cat_dict[ORIG_STEREO_CAT_CODE]
+            edit_status, edit_resp = self.client.edit_parent(parent, dry_run=False)
+            if not edit_status:
+                print(f"ERROR: Something went wrong editing the parent: {edit_resp}")
+            self.assertTrue(edit_status)
+            # Confirm attributes are back to as they were before
+            meta_lot = self.client.get_meta_lot('CMPD-0000001-001')
+            parent = meta_lot['lot']['parent']
+            self.assertEquals(parent['stereoComment'], ORIG_STEREO_COMMENT)
+            self.assertEquals(parent['stereoCategory']['code'], ORIG_STEREO_CAT_CODE)
+            # Edit structure to match parent 2
+            # This should result in a duplicate, and thus be blocked
+            parent['molStructure'] = CMPD_2_STRUCTURE
+            # Validate (should fail)
+            validation_status, validation_resp = self.client.edit_parent(parent, dry_run=True)
+            self.assertFalse(validation_status)
+            self.assertFalse(validation_resp['parentUnique'])
+            self.assertEquals(len(validation_resp['dupeParents']), 1)
+            self.assertEquals(validation_resp['dupeParents'][0]['corpName'], 'CMPD-0000002')
+            # Attempt non-dryrun (should fail)
+            edit_status, edit_resp = self.client.edit_parent(parent, dry_run=False)
+            self.assertFalse(edit_status)
+            self.assertFalse(edit_status)
+            self.assertFalse(edit_resp['parentUnique'])
+            self.assertEquals(len(edit_resp['dupeParents']), 1)
+            self.assertEquals(edit_resp['dupeParents'][0]['corpName'], 'CMPD-0000002')
         finally:
             # Prevent interaction with other tests.
             self.delete_all_cmpd_reg_bulk_load_files()
     
     @requires_absent_basic_cmpd_reg_load
     def test_010_validate_sdf_with_empty_aliases(self):
         # Test loading a file that has some blank parent aliases
@@ -4112,15 +4132,209 @@
                 self.verify_file_and_content_equal(file_test_path1, file['content'])
             if file["name"] == file_name2:
                 has_file2 = True
                 self.verify_file_and_content_equal(file_test_path2, file['content'])
                 
         self.assertTrue(has_file1)
         self.assertTrue(has_file2)
+
+    @requires_absent_basic_cmpd_reg_load
+    def test_013_unique_parent_alias_tests(self):
+        """Test bulk loading multiple lots to an existing parent"""
+
+        # Get a file that just has a simple mol structure
+        file = Path(__file__).resolve().parent.joinpath(
+            'test_acasclient', 'test_simple_mol.sdf')
+        
+        # Read the mol
+        with open(file, 'r') as f:
+            simple_mol = f.read()
+
+        # Append the > <Parent Alias> to the file content after "M  END"
+        parent_alias_1 = str(uuid.uuid4())
+        stereo_comment_1 = str(uuid.uuid4())
+        parent_1 = simple_mol.replace("M  END", f"M  END\n> <Parent Alias>\n{parent_alias_1}\n")
+        parent_1 = parent_1.replace("M  END", f"M  END\n> <Parent Stereo Comment>\n{stereo_comment_1}\n")
+
+        # Write the file back out to self.tempdir
+        file = Path(self.tempdir).joinpath('test_multiple_lots.sdf')
+        with open(file, 'w') as f:
+            # Write out the content twice so we can test that we can load multiple lots of the same parent
+            f.write(parent_1)
+
+        project_code = self.global_project_code
+        mappings = [
+                {
+                    "dbProperty": "Parent Corp Name",
+                    "defaultVal": None,
+                    "required": False,
+                    "sdfProperty": "Parent Corp Name"
+                },
+                {
+                    "dbProperty": "Lot Corp Name",
+                    "defaultVal": None,
+                    "required": False,
+                    "sdfProperty": "Lot Corp Name"
+                },
+                {
+                    "dbProperty": "Lot Chemist",
+                    "defaultVal": "bob",
+                    "required": True,
+                    "sdfProperty": None
+                },
+                {
+                    "dbProperty": "Project",
+                    "defaultVal": project_code,
+                    "required": True,
+                    "sdfProperty": "Project Code Name"
+                },
+                {
+                    "dbProperty": "Parent Stereo Category",
+                    "defaultVal": STEREO_CATEGORY,
+                    "required": True,
+                    "sdfProperty": None
+                },
+                {
+                    "dbProperty": "Parent Alias",
+                    "defaultVal": None,
+                    "required": False,
+                    "sdfProperty": "Parent Alias"
+                },
+                {
+                    "dbProperty": "Parent Stereo Comment",
+                    "defaultVal": None,
+                    "required": False,
+                    "sdfProperty": "Parent Stereo Comment"
+                },
+            ]
+        
+        # Load the parent with the alias
+        # Confirm this dryruns successfully and loads successfully
+        response = self.client.register_sdf(file, "bob", mappings, dry_run=False)
+        self.assertIn("Number of entries processed: 1", response['summary'])
+        self.assertIn("Number of entries with error: 0", response['summary'])
+        self.assertIn('New compounds: 1', response['summary'])
+
+        # Test 1: Load lots 2, 3 in the same file with the same parent alias and confirm it succeeds
+        # Append the content into the file again
+        # The file will contain lots 2, 3 of the parent we just loaded
+        with open(file, 'a') as f:
+            f.write(parent_1)
+        # Confirm this dryruns successfully
+        response = self.client.register_sdf(file, "bob", mappings, dry_run=True)
+        # There should not be any errors
+        self.assertIn("Number of entries processed: 2", response['summary'])
+        self.assertIn("Number of entries with error: 0", response['summary'])
+        self.assertIn("New lots of existing compounds: 2", response['summary'])
+        self.assertEqual(0, len(response['results']))
+        # Confirm this loads successfully
+        response = self.client.register_sdf(file, "bob", mappings, dry_run=False)
+        self.assertIn("Number of entries processed: 2", response['summary'])
+        self.assertIn("Number of entries with error: 0", response['summary'])
+        self.assertIn("New lots of existing compounds: 2", response['summary'])
+        self.assertEqual(0, len(response['results']))
+
+        # Test 2: Load a new parent with the same alias as the first parent and confirm it fails
+        stereo_comment_2 = str(uuid.uuid4())
+        parent_2 = simple_mol.replace("M  END", f"M  END\n> <Parent Stereo Comment>\n{stereo_comment_2}\n")
+        parent_2_with_parent_alias_1 = parent_2.replace("M  END", f"M  END\n> <Parent Alias>\n{parent_alias_1}\n")
+        # Write a file with the new parent
+        file = Path(self.tempdir).joinpath('fail_duplicate_blah.sdf')
+        with open(file, 'w') as f:
+            # Write out the content twice so we can test that we can load multiple lots of the same parent
+            f.write(parent_2_with_parent_alias_1)
+        # Should fail dry run
+        response = self.client.register_sdf(file, "bob", mappings, dry_run=True)
+        self.assertIn(f"1 entries had: Duplicate parent alias {parent_alias_1}", response['summary'])
+        # Should fail load
+        response = self.client.register_sdf(file, "bob", mappings, dry_run=False)
+        self.assertIn(f"1 entries had: Duplicate parent alias {parent_alias_1}", response['summary'])
+
+        # Test 3: Load 2 new parents with the same alias and confirm it fails
+        parent_alias_3 = str(uuid.uuid4())
+        stereo_comment_3 = str(uuid.uuid4())
+        stereo_comment_4 = str(uuid.uuid4())
+        parent_3 = simple_mol.replace("M  END", f"M  END\n> <Parent Stereo Comment>\n{stereo_comment_3}\n")
+        parent_3 = parent_3.replace("M  END", f"M  END\n> <Parent Alias>\n{parent_alias_3}\n")
+        parent_4 = simple_mol.replace("M  END", f"M  END\n> <Parent Stereo Comment>\n{stereo_comment_4}\n")
+        parent_4_alias_3 = parent_4.replace("M  END", f"M  END\n> <Parent Alias>\n{parent_alias_3}\n")
+        # Write the file with 2 new parents and same alias
+        file = Path(self.tempdir).joinpath('within_file_same_alias_2_compounds.sdf')
+        with open(file, 'w') as f:
+            f.write(parent_3)
+            f.write(parent_4_alias_3)
+        # Should fail dry run
+        response = self.client.register_sdf(file, "bob", mappings, dry_run=True)
+        self.assertIn("Number of entries processed: 2", response['summary'])
+        self.assertIn("Number of entries with error: 1", response['summary'])
+        self.assertIn(f"1 entries had: Within File, Parent Alias {parent_alias_3} is not unique", response['summary'])
+        # Should fail load the second lot
+        response = self.client.register_sdf(file, "bob", mappings, dry_run=False)
+        self.assertIn("Number of entries processed: 2", response['summary'])
+        self.assertIn("Number of entries with error: 1", response['summary'])
+        self.assertIn(f"1 entries had: Duplicate parent alias {parent_alias_3}", response['summary'])
+
+        # Test 4: Load 2 new parents, one with a parent alias that already exists and one new alias
+        stereo_comment_5 = str(uuid.uuid4())
+        parent_alias_6 = str(uuid.uuid4())
+        stereo_comment_6 = str(uuid.uuid4())
+        parent_5 = simple_mol.replace("M  END", f"M  END\n> <Parent Stereo Comment>\n{stereo_comment_5}\n")
+        parent_5_alias_1 = parent_5.replace("M  END", f"M  END\n> <Parent Alias>\n{parent_alias_1}\n")
+        parent_6 = simple_mol.replace("M  END", f"M  END\n> <Parent Stereo Comment>\n{stereo_comment_6}\n")
+        parent_6 = parent_6.replace("M  END", f"M  END\n> <Parent Alias>\n{parent_alias_6}\n")
+        # Write the file with 2 new parents and same alias
+        file = Path(self.tempdir).joinpath('within_file_same_alias_2_compounds.sdf')
+        with open(file, 'w') as f:
+            # Write out the content twice so we can test that we can load multiple lots of the same parent
+            f.write(parent_5_alias_1)
+            f.write(parent_6)
+        # Should fail dry run
+        response = self.client.register_sdf(file, "bob", mappings, dry_run=True)
+        self.assertIn("Number of entries processed: 2", response['summary'])
+        self.assertIn("Number of entries with error: 1", response['summary'])
+        self.assertIn(f"1 entries had: Duplicate parent alias {parent_alias_1}", response['summary'])
+        # Should fail load one
+        response = self.client.register_sdf(file, "bob", mappings, dry_run=False)
+        self.assertIn("Number of entries processed: 2", response['summary'])
+        self.assertIn("Number of entries with error: 1", response['summary'])
+        self.assertIn(f"1 entries had: Duplicate parent alias {parent_alias_1}", response['summary'])
+
+
+    @requires_basic_cmpd_reg_load
+    def test_014_get_preferred_lot_corp_names(self):
+        """Test get preferred lot corp names"""
+        # Setup constants
+        corp_name = "CMPD-0000001"
+        lot_corp_name = f"{corp_name}-001"
+        parent_alias = str(uuid.uuid4())
+        parent_alias_lot_corp_name = f"{parent_alias}-001"
+
         
+        # Add the parent alias to the parent
+        alias_type, alias_kind = self.get_first_parent_alias_type_kind()
+        self.client.add_parent_alias(corp_name, parent_alias, alias_type, alias_kind)
+
+        # Call get preferred lot corp names and verify that the lot corp name is returned
+        requests = [parent_alias_lot_corp_name, "FAKE"]
+        preferred_lot_corp_names_response = self.client.get_preferred_lot_corp_names(requests)
+
+        # Response length should always match the request length
+        self.assertEqual(len(preferred_lot_corp_names_response), 2)
+
+        # Items should have requestName and referenceCode
+        self.assertIn("requestName", preferred_lot_corp_names_response[0])
+        self.assertIn("referenceCode", preferred_lot_corp_names_response[0])
+
+        # First response should be the parent alias lot corp name
+        self.assertEqual(preferred_lot_corp_names_response[0]["requestName"], parent_alias_lot_corp_name)
+        self.assertEqual(preferred_lot_corp_names_response[0]["referenceCode"], lot_corp_name)
+
+        # Second response should be empty string returned
+        self.assertEqual(preferred_lot_corp_names_response[1]["requestName"], "FAKE")
+        self.assertEqual(preferred_lot_corp_names_response[1]["referenceCode"], "")
 
 class TestExperimentLoader(BaseAcasClientTest):
     """Tests for `Experiment Loading`."""
     
     # Test for malformed single quote format file
     def assert_malformed_single_quote_file(self, response):
         self.assertTrue(response['hasError'])
@@ -4582,8 +4796,55 @@
     @requires_basic_cmpd_reg_load
     def test_018_image_file(self):
         """Test experiment loader with image file."""
         data_file_to_upload = Path(__file__).resolve()\
             .parent.joinpath('test_acasclient', '12_1_MultipleImage.csv')
         image_file_path = Path(__file__).resolve().parent\
             .joinpath('test_acasclient', '12_2_MultipleImage.zip')
-        self.experiment_load_test(data_file_to_upload, False, images_file_to_upload=image_file_path)
+        self.experiment_load_test(data_file_to_upload, False, images_file_to_upload=image_file_path)
+
+    @requires_basic_cmpd_reg_load
+    def test_19_project_restrictions(self):
+        """Check experiment loader project restrictions are working."""
+
+        # Setup for tests
+        # Create a restricted project
+        restricted_project_1 = self.create_basic_project_with_roles()
+        # Create a restricted lot in a different restricted project
+        restricted_project_2 = self.create_basic_project_with_roles()
+        restricted_lot_corp_name_2 = self.create_restricted_lot(restricted_project_2.code_name)
+
+        # (Dissallowed) Restricted experiment proj1 with lot restricted proj2
+        # Create an upload file which uploads to restricted_project_1 but has a lot from restricted_project_2
+        file_to_upload = get_basic_experiment_load_file(self.tempdir, restricted_project_1.names[PROJECT_NAME], corp_name=restricted_lot_corp_name_2, file_name='uniform-commas-with-quoted-text.csv')
+        # Upload the file and expect it to fail
+        response = self.experiment_load_test(file_to_upload, True, expect_failure=True)
+        # Verify that the error message is correct
+        expected_messages = [
+            {
+                "errorLevel": "error",
+                "message": f"Compounds '{restricted_lot_corp_name_2}' are in a restricted project that does not match the one entered for this Experiment."
+            }
+        ]
+        self.check_expected_messages(expected_messages, response['errorMessages'])
+
+        # (Allowed) Restricted experiment proj1 with lot restricted proj1
+        # Create another restricted lot in restricted_project_1
+        restricted_lot_corp_name_1 = self.create_restricted_lot(restricted_project_1.code_name)
+        # Create an upload file which uploads to restricted_project_1 and has a lot from restricted_project_1
+        file_to_upload = get_basic_experiment_load_file(self.tempdir, restricted_project_1.names[PROJECT_NAME], corp_name=restricted_lot_corp_name_1, file_name='uniform-commas-with-quoted-text.csv')
+        # Upload the file and expect it to succeed
+        response = self.experiment_load_test(file_to_upload, True, expect_failure=False)
+
+        # (Allowed) Restricted experiment proj1 with lot unrestricted
+        # Basic cmpdreg load creates a lot in the Global unrestricted project
+        # So we expect that it can be uploaded to a restricted project
+        # Get a file to upload to restricted_project_1 but has a lot from the Global unrestricted project
+        file_to_upload = get_basic_experiment_load_file(self.tempdir, restricted_project_1.names[PROJECT_NAME], corp_name=None, file_name='uniform-commas-with-quoted-text.csv')
+        # Upload the file and expect it to succeed
+        response = self.experiment_load_test(file_to_upload, True, expect_failure=False)
+
+        # (Allowed) Unrestricted experiment Global with lot restricted proj2
+        # Create an upload file which uploads to Global(unrestricted) but has a lot from restricted_project_2
+        file_to_upload = get_basic_experiment_load_file(self.tempdir, project_code=None, corp_name=restricted_lot_corp_name_2, file_name='uniform-commas-with-quoted-text.csv')
+        # Upload the file and expect it to succeed
+        response = self.experiment_load_test(file_to_upload, False, expect_failure=False)
```

### Comparing `acasclient-2023.4.1/tests/test_lsthing.py` & `acasclient-2024.1.0/tests/test_lsthing.py`

 * *Files identical despite different names*

