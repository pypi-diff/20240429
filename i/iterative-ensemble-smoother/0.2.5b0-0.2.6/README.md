# Comparing `tmp/iterative_ensemble_smoother-0.2.5b0.tar.gz` & `tmp/iterative_ensemble_smoother-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterative_ensemble_smoother-0.2.5b0.tar", last modified: Fri Apr 12 11:55:15 2024, max compression
+gzip compressed data, was "iterative_ensemble_smoother-0.2.6.tar", last modified: Mon Apr 29 12:28:17 2024, max compression
```

## Comparing `iterative_ensemble_smoother-0.2.5b0.tar` & `iterative_ensemble_smoother-0.2.6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.122689 iterative_ensemble_smoother-0.2.5b0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.110689 iterative_ensemble_smoother-0.2.5b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.114689 iterative_ensemble_smoother-0.2.5b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.github/workflows/precommit.yml
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.github/workflows/testing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.github/workflows/upload_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/LITERATURE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-12 11:55:15.122689 iterative_ensemble_smoother-0.2.5b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.110689 iterative_ensemble_smoother-0.2.5b0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.114689 iterative_ensemble_smoother-0.2.5b0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/Adaptive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/LinearRegression.py
--rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/Oscillator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/Polynomial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.110689 iterative_ensemble_smoother-0.2.5b0/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.118689 iterative_ensemble_smoother-0.2.5b0/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/bibliography.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/docs/source/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-12 11:55:15.122689 iterative_ensemble_smoother-0.2.5b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.110689 iterative_ensemble_smoother-0.2.5b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.118689 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-12 11:55:15.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/esmda.py
--rw-r--r--   0 runner    (1001) docker     (127)    20460 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/esmda_inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    16435 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    15246 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/sies.py
--rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/sies_inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.122689 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5282 2024-04-12 11:55:15.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-12 11:55:15.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:55:15.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-12 11:55:15.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 11:55:15.000000 iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.118689 iterative_ensemble_smoother-0.2.5b0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.110689 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.110689 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.118689 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step/test_ensemble_smoother_update_step.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.118689 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step_with_rowscaling/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step_with_rowscaling/test_ensemble_smoother_update_step.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:55:15.122689 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_iterative_ensemble_smoother_update_step/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_iterative_ensemble_smoother_update_step/test_iterative_ensemble_smoother_update_step.csv
--rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/test_esmda.py
--rw-r--r--   0 runner    (1001) docker     (127)    13968 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/test_esmda_inversion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19917 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/test_experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)    35674 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tests/test_sies.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-12 11:55:10.000000 iterative_ensemble_smoother-0.2.5b0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.929968 iterative_ensemble_smoother-0.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.917968 iterative_ensemble_smoother-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.921968 iterative_ensemble_smoother-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/.github/workflows/precommit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/.github/workflows/testing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/.github/workflows/upload_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/.mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5207 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/LITERATURE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-29 12:28:17.929968 iterative_ensemble_smoother-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.917968 iterative_ensemble_smoother-0.2.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.921968 iterative_ensemble_smoother-0.2.6/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)    11509 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/docs/source/Adaptive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/docs/source/LinearRegression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8674 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/docs/source/Oscillator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/docs/source/Polynomial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.917968 iterative_ensemble_smoother-0.2.6/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.925968 iterative_ensemble_smoother-0.2.6/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/docs/source/bibliography.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/docs/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/docs/source/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/docs/source/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-29 12:28:17.929968 iterative_ensemble_smoother-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.917968 iterative_ensemble_smoother-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.925968 iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 12:28:17.000000 iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14161 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/esmda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20460 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/esmda_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17077 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15246 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/sies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/sies_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3587 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.929968 iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-04-29 12:28:17.000000 iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-29 12:28:17.000000 iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 12:28:17.000000 iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-29 12:28:17.000000 iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 12:28:17.000000 iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.925968 iterative_ensemble_smoother-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.917968 iterative_ensemble_smoother-0.2.6/tests/snapshots/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.917968 iterative_ensemble_smoother-0.2.6/tests/snapshots/test_snapshots/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.925968 iterative_ensemble_smoother-0.2.6/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step/test_ensemble_smoother_update_step.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.925968 iterative_ensemble_smoother-0.2.6/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step_with_rowscaling/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step_with_rowscaling/test_ensemble_smoother_update_step.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 12:28:17.925968 iterative_ensemble_smoother-0.2.6/tests/snapshots/test_snapshots/test_iterative_ensemble_smoother_update_step/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/tests/snapshots/test_snapshots/test_iterative_ensemble_smoother_update_step/test_iterative_ensemble_smoother_update_step.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    17823 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/tests/test_esmda.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13968 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/tests/test_esmda_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20860 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/tests/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35674 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/tests/test_sies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-29 12:28:12.000000 iterative_ensemble_smoother-0.2.6/tox.ini
```

### Comparing `iterative_ensemble_smoother-0.2.5b0/.github/workflows/testing.yml` & `iterative_ensemble_smoother-0.2.6/.github/workflows/testing.yml`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/.github/workflows/upload_to_pypi.yml` & `iterative_ensemble_smoother-0.2.6/.github/workflows/upload_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/.gitignore` & `iterative_ensemble_smoother-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/.pre-commit-config.yaml` & `iterative_ensemble_smoother-0.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/CODE_OF_CONDUCT.md` & `iterative_ensemble_smoother-0.2.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/COPYING` & `iterative_ensemble_smoother-0.2.6/COPYING`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/LITERATURE.md` & `iterative_ensemble_smoother-0.2.6/LITERATURE.md`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/PKG-INFO` & `iterative_ensemble_smoother-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterative_ensemble_smoother
-Version: 0.2.5b0
+Version: 0.2.6
 Summary: A library for the iterative ensemble smoother algorithm.
 Author-email: Equinor <fg_sib-scout@equinor.com>
 Maintainer-email: Eivind Jahren <ejah@equinor.com>, Feda Curic <fcur@equinor.com>
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/equinor/iterative_ensemble_smoother
 Project-URL: Repository, https://github.com/equinor/iterative_ensemble_smoother
 Project-URL: Bug Tracker, https://github.com/equinor/iterative_ensemble_smoother/issues
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: numpy
 Requires-Dist: scipy
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: docutils<0.21; extra == "doc"
 Requires-Dist: pydata_sphinx_theme; extra == "doc"
 Requires-Dist: jupyter_sphinx; extra == "doc"
 Requires-Dist: sphinxcontrib.bibtex; extra == "doc"
 Requires-Dist: matplotlib; extra == "doc"
 Requires-Dist: pygments; extra == "doc"
 Requires-Dist: jupytext; extra == "doc"
 Requires-Dist: pandas; extra == "doc"
```

### Comparing `iterative_ensemble_smoother-0.2.5b0/README.md` & `iterative_ensemble_smoother-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/SECURITY.md` & `iterative_ensemble_smoother-0.2.6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/docs/source/Adaptive.py` & `iterative_ensemble_smoother-0.2.6/docs/source/Adaptive.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/docs/source/LinearRegression.py` & `iterative_ensemble_smoother-0.2.6/docs/source/LinearRegression.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/docs/source/Oscillator.py` & `iterative_ensemble_smoother-0.2.6/docs/source/Oscillator.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/docs/source/Polynomial.py` & `iterative_ensemble_smoother-0.2.6/docs/source/Polynomial.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/docs/source/_templates/autosummary/module.rst` & `iterative_ensemble_smoother-0.2.6/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/docs/source/conf.py` & `iterative_ensemble_smoother-0.2.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/docs/source/glossary.rst` & `iterative_ensemble_smoother-0.2.6/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/docs/source/refs.bib` & `iterative_ensemble_smoother-0.2.6/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/pyproject.toml` & `iterative_ensemble_smoother-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 "Repository" = "https://github.com/equinor/iterative_ensemble_smoother"
 "Bug Tracker" = "https://github.com/equinor/iterative_ensemble_smoother/issues"
 "Documentation" = "https://iterative_ensemble_smoother.readthedocs.io/en/stable/"
 
 [project.optional-dependencies]
 doc = [
     "sphinx",
+    "docutils<0.21",
     "pydata_sphinx_theme",
     "jupyter_sphinx",
     "sphinxcontrib.bibtex",
     "matplotlib",
     "pygments",
     "jupytext",
     "pandas",
```

### Comparing `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/__init__.py` & `iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/__init__.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/esmda.py` & `iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/esmda.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/esmda_inversion.py` & `iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/esmda_inversion.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/experimental.py` & `iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/experimental.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,15 @@
         Y: npt.NDArray[np.double],
         D: npt.NDArray[np.double],
         overwrite: bool = False,
         alpha: float,
         correlation_threshold: Union[Callable[[int], float], float, None] = None,
         cov_YY: Optional[npt.NDArray[np.double]] = None,
         progress_callback: Optional[Callable[[Sequence[T]], Sequence[T]]] = None,
+        correlation_callback: Optional[Callable[[npt.NDArray[np.double]], None]] = None,
     ) -> npt.NDArray[np.double]:
         """Assimilate data and return an updated ensemble X_posterior.
 
             X_posterior = smoother.assimilate(X, Y, D, alpha)
 
         This method first computes the cross-covariance and cross-correlation
         matrices between X and Y. Then it sets correlations that are below the
@@ -195,14 +196,19 @@
             A callback function that can be used to wrap the iteration over
             parameters for progress reporting.
             It should accept an iterable as input and return an iterable.
             This allows for integration with progress reporting tools like tqdm,
             which can provide visual feedback on the progress of the
             assimilation process.
             If None, no progress reporting is performed.
+        correlation_callback : Optional[Callable]
+            A callback function that is called with the correlation matrix (2D array)
+            as its argument after the correlation matrix computation is complete.
+            The callback should handle or process the correlation matrix, such as
+            saving or logging it. The callback should not return any value.
         Returns
         -------
         X_posterior : np.ndarray
             2D array of shape (num_parameters, ensemble_size).
         """
         assert X.shape[1] == Y.shape[1]
 
@@ -301,14 +307,17 @@
                 C_D=C_D_subset,
                 D=D_subset,
                 Y=Y_subset,
                 cov_YY=cov_YY_subset,  # Passing cov(Y, Y) avoids re-computation
             )
             X[[param_num], :] += cov_XY_subset @ T
 
+        if correlation_callback is not None:
+            corr_XY = self._cov_to_corr_inplace(cov_XY, stds_X, stds_Y)
+            correlation_callback(corr_XY[significant_rows])
         return X
 
 
 class RowScaling:
     # Illustration of how row scaling works, `multiply` is the important part
     # For the actual implementation, which is more involved, see:
     # https://github.com/equinor/ert/blob/84aad3c56e0e52be27b9966322d93dbb85024c1c/src/clib/lib/enkf/row_scaling.cpp
```

### Comparing `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/sies.py` & `iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/sies.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/sies_inversion.py` & `iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/sies_inversion.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother/utils.py` & `iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother/utils.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/PKG-INFO` & `iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iterative_ensemble_smoother
-Version: 0.2.5b0
+Version: 0.2.6
 Summary: A library for the iterative ensemble smoother algorithm.
 Author-email: Equinor <fg_sib-scout@equinor.com>
 Maintainer-email: Eivind Jahren <ejah@equinor.com>, Feda Curic <fcur@equinor.com>
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/equinor/iterative_ensemble_smoother
 Project-URL: Repository, https://github.com/equinor/iterative_ensemble_smoother
 Project-URL: Bug Tracker, https://github.com/equinor/iterative_ensemble_smoother/issues
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: COPYING
 Requires-Dist: numpy
 Requires-Dist: scipy
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
+Requires-Dist: docutils<0.21; extra == "doc"
 Requires-Dist: pydata_sphinx_theme; extra == "doc"
 Requires-Dist: jupyter_sphinx; extra == "doc"
 Requires-Dist: sphinxcontrib.bibtex; extra == "doc"
 Requires-Dist: matplotlib; extra == "doc"
 Requires-Dist: pygments; extra == "doc"
 Requires-Dist: jupytext; extra == "doc"
 Requires-Dist: pandas; extra == "doc"
```

### Comparing `iterative_ensemble_smoother-0.2.5b0/src/iterative_ensemble_smoother.egg-info/SOURCES.txt` & `iterative_ensemble_smoother-0.2.6/src/iterative_ensemble_smoother.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step/test_ensemble_smoother_update_step.csv` & `iterative_ensemble_smoother-0.2.6/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step/test_ensemble_smoother_update_step.csv`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step_with_rowscaling/test_ensemble_smoother_update_step.csv` & `iterative_ensemble_smoother-0.2.6/tests/snapshots/test_snapshots/test_ensemble_smoother_update_step_with_rowscaling/test_ensemble_smoother_update_step.csv`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/tests/snapshots/test_snapshots/test_iterative_ensemble_smoother_update_step/test_iterative_ensemble_smoother_update_step.csv` & `iterative_ensemble_smoother-0.2.6/tests/snapshots/test_snapshots/test_iterative_ensemble_smoother_update_step/test_iterative_ensemble_smoother_update_step.csv`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/tests/test_esmda.py` & `iterative_ensemble_smoother-0.2.6/tests/test_esmda.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/tests/test_esmda_inversion.py` & `iterative_ensemble_smoother-0.2.6/tests/test_esmda_inversion.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/tests/test_experimental.py` & `iterative_ensemble_smoother-0.2.6/tests/test_experimental.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import functools
 import time
 from copy import deepcopy
 
 import numpy as np
 import pytest
 
 from iterative_ensemble_smoother import ESMDA
@@ -56,14 +57,23 @@
         X, g, observations, covariance, _ = linear_problem
 
         # Create adaptive smoother
         smoother = AdaptiveESMDA(
             covariance=covariance, observations=observations, seed=1
         )
 
+        def correlation_callback(corr_matrix):
+            # A correlation threshold of 1 means that no
+            # correlations are deemed significant.
+            # Therefore, the cross-correlation matrix must
+            # not include any parameter-response pairs.
+            print(corr_matrix)
+            assert corr_matrix.shape[0] == 0
+            assert corr_matrix.shape[1] == len(observations)
+
         X_i = np.copy(X)
         alpha = normalize_alpha(np.ones(5))
         for alpha_i in alpha:
             # Run forward model
             Y_i = g(X_i)
 
             # Create noise D - common to this ESMDA update
@@ -74,39 +84,48 @@
             # Update the relevant parameters and write to X
             X_i = smoother.assimilate(
                 X=X_i,
                 Y=Y_i,
                 D=D_i,
                 alpha=alpha_i,
                 correlation_threshold=1,
+                correlation_callback=correlation_callback,
             )
 
         assert np.allclose(X, X_i)
 
     @pytest.mark.parametrize(
         "linear_problem",
         range(25),
         indirect=True,
         ids=[f"seed-{i+1}" for i in range(25)],
     )
     def test_that_adaptive_localization_with_cutoff_0_equals_standard_ESMDA_update(
         self, linear_problem
     ):
         # Create a problem with g(x) = A @ x
-        X, g, observations, covariance, rng = linear_problem
+        X, g, observations, covariance, _ = linear_problem
 
         # =============================================================================
         # SETUP ESMDA FOR LOCALIZATION AND SOLVE PROBLEM
         # =============================================================================
         alpha = normalize_alpha(np.ones(5))
 
         smoother = AdaptiveESMDA(
             covariance=covariance, observations=observations, seed=1
         )
 
+        def correlation_callback(corr_matrix):
+            # A correlation threshold of 0 means that all
+            # correlations are deemed significant.
+            # Therefore, the cross-correlation matrix must
+            # include all parameter-resposne pairs.
+            assert corr_matrix.shape[0] == X.shape[0]
+            assert corr_matrix.shape[1] == len(observations)
+
         X_i = np.copy(X)
         for _, alpha_i in enumerate(alpha, 1):
             # Run forward model
             Y_i = g(X_i)
 
             # Create noise D - common to this ESMDA update
             D_i = smoother.perturb_observations(
@@ -117,14 +136,15 @@
             smoother.assimilate(
                 X=X_i,
                 Y=Y_i,
                 D=D_i,
                 overwrite=True,
                 alpha=alpha_i,
                 correlation_threshold=0,
+                correlation_callback=functools.partial(correlation_callback),
             )
 
         # =============================================================================
         # VERIFY RESULT AGAINST NORMAL ESMDA ITERATIONS
         # =============================================================================
         smoother = ESMDA(
             covariance=covariance,
```

### Comparing `iterative_ensemble_smoother-0.2.5b0/tests/test_sies.py` & `iterative_ensemble_smoother-0.2.6/tests/test_sies.py`

 * *Files identical despite different names*

### Comparing `iterative_ensemble_smoother-0.2.5b0/tox.ini` & `iterative_ensemble_smoother-0.2.6/tox.ini`

 * *Files identical despite different names*

