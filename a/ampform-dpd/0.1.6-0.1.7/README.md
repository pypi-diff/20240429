# Comparing `tmp/ampform-dpd-0.1.6.tar.gz` & `tmp/ampform_dpd-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampform-dpd-0.1.6.tar", last modified: Wed Mar 20 11:04:05 2024, max compression
+gzip compressed data, was "ampform_dpd-0.1.7.tar", last modified: Mon Apr 29 08:52:35 2024, max compression
```

## Comparing `ampform-dpd-0.1.6.tar` & `ampform_dpd-0.1.7.tar`

### file list

```diff
@@ -1,73 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:04:05.588714 ampform-dpd-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:04:05.576714 ampform-dpd-0.1.6/.constraints/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.constraints/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.constraints/py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.constraints/py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.constraints/py3.12.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.constraints/py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.constraints/py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.cspell.json
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:04:05.576714 ampform-dpd-0.1.6/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:04:05.576714 ampform-dpd-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.github/workflows/clean-caches.yml
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.github/workflows/pr-linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.github/workflows/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.gitpod.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.taplo.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:04:05.576714 ampform-dpd-0.1.6/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-03-20 11:04:05.588714 ampform-dpd-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:04:05.580714 ampform-dpd-0.1.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:04:05.580714 ampform-dpd-0.1.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:04:05.580714 ampform-dpd-0.1.6/docs/comparison/
--rw-r--r--   0 runner    (1001) docker     (127)    32583 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/docs/comparison/d2kkk.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    32026 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/docs/comparison/jpsi2phipipi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    31843 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/docs/comparison/jpsi2pipipi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/docs/comparison.md
--rw-r--r--   0 runner    (1001) docker     (127)     6697 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    28704 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/docs/jpsi2ksp.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/docs/lc2pkpi.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/docs/references.bib
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/docs/references.md
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 11:04:05.588714 ampform-dpd-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:04:05.572714 ampform-dpd-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:04:05.580714 ampform-dpd-0.1.6/src/ampform_dpd/
--rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/src/ampform_dpd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/src/ampform_dpd/_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/src/ampform_dpd/_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/src/ampform_dpd/angles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5214 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/src/ampform_dpd/decay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/src/ampform_dpd/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9931 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/src/ampform_dpd/io.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/src/ampform_dpd/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/src/ampform_dpd/spin.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-20 11:04:05.000000 ampform-dpd-0.1.6/src/ampform_dpd/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:04:05.584714 ampform-dpd-0.1.6/src/ampform_dpd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-03-20 11:04:05.000000 ampform-dpd-0.1.6/src/ampform_dpd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-03-20 11:04:05.000000 ampform-dpd-0.1.6/src/ampform_dpd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 11:04:05.000000 ampform-dpd-0.1.6/src/ampform_dpd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-20 11:04:05.000000 ampform-dpd-0.1.6/src/ampform_dpd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-20 11:04:05.000000 ampform-dpd-0.1.6/src/ampform_dpd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 11:04:05.584714 ampform-dpd-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/tests/test_angles.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/tests/test_decay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-03-20 11:03:58.000000 ampform-dpd-0.1.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:35.440656 ampform_dpd-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:35.428655 ampform_dpd-0.1.7/.constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.constraints/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.constraints/py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.constraints/py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.constraints/py3.12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.constraints/py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.constraints/py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.cspell.json
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:35.428655 ampform_dpd-0.1.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:35.428655 ampform_dpd-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.github/workflows/clean-caches.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.github/workflows/pr-linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.github/workflows/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.gitpod.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.taplo.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:35.428655 ampform_dpd-0.1.7/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-29 08:52:35.440656 ampform_dpd-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:35.432655 ampform_dpd-0.1.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:35.432655 ampform_dpd-0.1.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:35.432655 ampform_dpd-0.1.7/docs/comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)    28057 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/docs/comparison/d2kkk.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    27534 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/docs/comparison/jpsi2phipipi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    27353 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/docs/comparison/jpsi2pipipi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/docs/comparison.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    22797 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/docs/jpsi2ksp.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     8990 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/docs/lc2pkpi.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/docs/references.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/docs/references.md
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 08:52:35.440656 ampform_dpd-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:35.424656 ampform_dpd-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:35.432655 ampform_dpd-0.1.7/src/ampform_dpd/
+-rw-r--r--   0 runner    (1001) docker     (127)    16595 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/src/ampform_dpd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/src/ampform_dpd/_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/src/ampform_dpd/_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:35.432655 ampform_dpd-0.1.7/src/ampform_dpd/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/src/ampform_dpd/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/src/ampform_dpd/adapter/qrules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7496 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/src/ampform_dpd/angles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/src/ampform_dpd/decay.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:35.432655 ampform_dpd-0.1.7/src/ampform_dpd/dynamics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/src/ampform_dpd/dynamics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/src/ampform_dpd/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/src/ampform_dpd/particle-definitions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/src/ampform_dpd/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/src/ampform_dpd/spin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 08:52:35.000000 ampform_dpd-0.1.7/src/ampform_dpd/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:35.436655 ampform_dpd-0.1.7/src/ampform_dpd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-29 08:52:35.000000 ampform_dpd-0.1.7/src/ampform_dpd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-29 08:52:35.000000 ampform_dpd-0.1.7/src/ampform_dpd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 08:52:35.000000 ampform_dpd-0.1.7/src/ampform_dpd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-29 08:52:35.000000 ampform_dpd-0.1.7/src/ampform_dpd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-29 08:52:35.000000 ampform_dpd-0.1.7/src/ampform_dpd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:35.436655 ampform_dpd-0.1.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:35.436655 ampform_dpd-0.1.7/tests/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/tests/adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/tests/adapter/test_qrules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/tests/test_angles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/tests/test_decay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-29 08:52:27.000000 ampform_dpd-0.1.7/tox.ini
```

### Comparing `ampform-dpd-0.1.6/.constraints/py3.10.txt` & `ampform_dpd-0.1.7/.constraints/py3.10.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,224 +10,228 @@
 arrow==1.3.0
 asttokens==2.4.1
 astunparse==1.6.3
 async-lru==2.0.4
 attrs==23.2.0
 babel==2.14.0
 beautifulsoup4==4.12.3
-black==24.3.0
+black==24.4.0
 bleach==6.1.0
 cachetools==5.3.3
 cattrs==23.2.3
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 chardet==5.2.0
 charset-normalizer==3.3.2
 click==8.1.7
 cloudpickle==3.0.0
 colorama==0.4.6
 comm==0.2.2
-contourpy==1.2.0
-coverage==7.4.4
+contourpy==1.2.1
+coverage==7.5.0
 cycler==0.12.1
 debugpy==1.8.1
 decorator==5.1.1
 defusedxml==0.7.1
 distlib==0.3.8
 dm-tree==0.1.8
 docstring-to-markdown==0.15
-docutils==0.20.1
-exceptiongroup==1.2.0
-execnet==2.0.2
+docutils==0.21.2
+exceptiongroup==1.2.1
+execnet==2.1.1
 executing==2.0.1
 fastjsonschema==2.19.1
-filelock==3.13.1
-flatbuffers==24.3.7
-fonttools==4.50.0
+filelock==3.13.4
+flatbuffers==24.3.25
+fonttools==4.51.0
 fqdn==1.5.1
 gast==0.5.4
 gitdb==4.0.11
-gitpython==3.1.42
+gitpython==3.1.43
 google-pasta==0.2.0
-graphviz==0.20.1
+graphviz==0.20.3
 greenlet==3.0.3
-grpcio==1.62.1
+grpcio==1.62.2
 h11==0.14.0
-h5py==3.10.0
+h5py==3.11.0
 hepunits==2.3.3
-httpcore==1.0.4
+httpcore==1.0.5
 httpx==0.27.0
-identify==2.5.35
-idna==3.6
+identify==2.5.36
+idna==3.7
 imagesize==1.4.1
 iminuit==2.25.2
-importlib-metadata==7.0.2
+importlib-metadata==7.1.0
 iniconfig==2.0.0
-ipykernel==6.29.3
-ipympl==0.9.3
-ipython==8.22.2
+ipykernel==6.29.4
+ipympl==0.9.4
+ipython==8.23.0
 ipython-genutils==0.2.0
 ipywidgets==8.1.2
 isoduration==20.11.0
 isort==5.13.2
-jax==0.4.25
-jaxlib==0.4.25
+jax==0.4.26
+jaxlib==0.4.26
 jedi==0.19.1
 jinja2==3.1.3
-json5==0.9.24
+json5==0.9.25
 jsonpointer==2.4
 jsonschema==4.21.1
 jsonschema-specifications==2023.12.1
 jupyter-cache==1.0.0
 jupyter-client==8.6.1
 jupyter-core==5.7.2
-jupyter-events==0.9.1
-jupyter-lsp==2.2.4
-jupyter-server==2.13.0
+jupyter-events==0.10.0
+jupyter-lsp==2.2.5
+jupyter-server==2.14.0
 jupyter-server-mathjax==0.2.6
 jupyter-server-terminals==0.5.3
-jupyterlab==4.1.5
+jupyterlab==4.1.6
 jupyterlab-code-formatter==2.2.1
 jupyterlab-git==0.50.0
 jupyterlab-lsp==5.1.0
-jupyterlab-myst==2.3.1
+jupyterlab-myst==2.3.2
 jupyterlab-pygments==0.3.0
-jupyterlab-server==2.25.4
+jupyterlab-server==2.27.1
 jupyterlab-widgets==3.0.10
-keras==3.0.5
+keras==3.3.2
 kiwisolver==1.4.5
 latexcodec==3.0.0
-libclang==16.0.6
-livereload==2.6.3
+libclang==18.1.1
 llvmlite==0.42.0
 lsprotocol==2023.0.1
 markdown==3.6
 markdown-it-py==3.0.0
 markupsafe==2.1.5
-matplotlib==3.8.3
-matplotlib-inline==0.1.6
+matplotlib==3.8.4
+matplotlib-inline==0.1.7
 mdit-py-plugins==0.4.0
 mdurl==0.1.2
 mistune==3.0.2
 ml-dtypes==0.3.2
 mpmath==1.3.0
 mypy-extensions==1.0.0
-myst-nb==1.0.0
-myst-parser==2.0.0
-namex==0.0.7
+myst-nb==1.1.0
+myst-parser==3.0.0
+namex==0.0.8
 nbclient==0.6.8
-nbconvert==7.16.2
+nbconvert==7.16.3
 nbdime==4.0.1
-nbformat==5.10.3
+nbformat==5.10.4
 nbmake==1.5.3
 nest-asyncio==1.6.0
 nodeenv==1.8.0
 notebook-shim==0.2.4
-numba==0.59.0
+numba==0.59.1
 numpy==1.26.4
 opt-einsum==3.3.0
+optree==0.11.0
 overrides==7.7.0
 packaging==24.0
 pandocfilters==1.5.1
-parso==0.8.3
-particle==0.23.1
+parso==0.8.4
+particle==0.24.0
 pathspec==0.12.1
 pexpect==4.9.0
-phasespace==1.9.0
-pillow==10.2.0
-platformdirs==4.2.0
-pluggy==1.4.0
-pre-commit==3.6.2
+phasespace==1.10.3
+pillow==10.3.0
+platformdirs==4.2.1
+pluggy==1.5.0
+pre-commit==3.7.0
 prometheus-client==0.20.0
 prompt-toolkit==3.0.43
 protobuf==4.25.3
 psutil==5.9.8
 ptyprocess==0.7.0
 pure-eval==0.2.2
 pybtex==0.24.0
 pybtex-docutils==1.0.3
-pycparser==2.21
+pycparser==2.22
 pydata-sphinx-theme==0.15.2
 pygments==2.17.2
 pyparsing==3.1.2
 pyproject-api==1.6.1
 pytest==8.1.1
-pytest-cov==4.1.0
+pytest-cov==5.0.0
 pytest-xdist==3.5.0
-python-constraint==1.3.1
+python-constraint==1.4.0
 python-dateutil==2.9.0.post0
 python-json-logger==2.0.7
 python-lsp-jsonrpc==1.1.2
 python-lsp-ruff==2.2.0
-python-lsp-server==1.10.1
+python-lsp-server==1.11.0
 pytoolconfig==1.3.1
 pyyaml==6.0.1
-pyzmq==25.1.2
+pyzmq==26.0.2
 qrules==0.10.1
-referencing==0.34.0
+referencing==0.35.0
 requests==2.31.0
 rfc3339-validator==0.1.4
 rfc3986-validator==0.1.1
 rich==13.7.1
-rope==1.12.0
+rope==1.13.0
 rpds-py==0.18.0
-ruff==0.3.3
-scipy==1.12.0
-send2trash==1.8.2
+ruff==0.4.1
+scipy==1.13.0
+send2trash==1.8.3
 six==1.16.0
 smmap==5.0.1
 sniffio==1.3.1
 snowballstemmer==2.2.0
 soupsieve==2.5
-sphinx==7.2.6
-sphinx-api-relink==0.0.8
-sphinx-autobuild==2024.2.4
+sphinx==7.3.7
+sphinx-api-relink==0.0.9
+sphinx-autobuild==2024.4.16
 sphinx-book-theme==1.1.2
-sphinx-codeautolink==0.15.0
+sphinx-codeautolink==0.15.1
 sphinx-copybutton==0.5.2
 sphinx-design==0.5.0
 sphinx-pybtex-etal-style==0.0.2
 sphinx-togglebutton==0.3.2
 sphinxcontrib-applehelp==1.0.8
 sphinxcontrib-bibtex==2.6.2
 sphinxcontrib-devhelp==1.0.6
 sphinxcontrib-htmlhelp==2.0.5
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.7
 sphinxcontrib-serializinghtml==1.1.10
-sqlalchemy==2.0.28
+sqlalchemy==2.0.29
 stack-data==0.6.3
+starlette==0.37.2
 sympy==1.12
 tabulate==0.9.0
 tensorboard==2.16.2
 tensorboard-data-server==0.7.2
 tensorflow==2.16.1
 tensorflow-io-gcs-filesystem==0.36.0
 tensorflow-probability==0.24.0
 tensorwaves==0.4.12
 termcolor==2.4.0
 terminado==0.18.1
-tinycss2==1.2.1
+tinycss2==1.3.0
 tomli==2.0.1
 tornado==6.4
-tox==4.14.1
+tox==4.14.2
 tqdm==4.66.2
-traitlets==5.14.2
+traitlets==5.14.3
 types-python-dateutil==2.9.0.20240316
-typing-extensions==4.10.0
+typing-extensions==4.11.0
 ujson==5.9.0
 uri-template==1.3.0
 urllib3==2.2.1
-virtualenv==20.25.1
+uvicorn==0.29.0
+virtualenv==20.26.0
+watchfiles==0.21.0
 wcwidth==0.2.13
 webcolors==1.13
 webencodings==0.5.1
-websocket-client==1.7.0
-werkzeug==3.0.1
+websocket-client==1.8.0
+websockets==12.0
+werkzeug==3.0.2
 wheel==0.43.0
 widgetsnbextension==4.0.10
 wrapt==1.16.0
 zipp==3.18.1
 
 # The following packages were excluded from the output:
 # setuptools
```

### Comparing `ampform-dpd-0.1.6/.constraints/py3.11.txt` & `ampform_dpd-0.1.7/.constraints/py3.9.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,231 +1,238 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile pyproject.toml -o .constraints/py3.11.txt --all-extras --no-annotate --python-version=3.11 --no-emit-package setuptools
+#    uv pip compile pyproject.toml -o .constraints/py3.9.txt --all-extras --no-annotate --python-version=3.9 --no-emit-package setuptools
 absl-py==2.1.0
 accessible-pygments==0.0.4
 alabaster==0.7.16
 ampform==0.15.0
 anyio==4.3.0
 argon2-cffi==23.1.0
 argon2-cffi-bindings==21.2.0
 arrow==1.3.0
 asttokens==2.4.1
 astunparse==1.6.3
 async-lru==2.0.4
 attrs==23.2.0
 babel==2.14.0
 beautifulsoup4==4.12.3
-black==24.3.0
+black==24.4.0
 bleach==6.1.0
 cachetools==5.3.3
 cattrs==23.2.3
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 chardet==5.2.0
 charset-normalizer==3.3.2
 click==8.1.7
 cloudpickle==3.0.0
 colorama==0.4.6
 comm==0.2.2
-contourpy==1.2.0
-coverage==7.4.4
+contourpy==1.2.1
+coverage==7.5.0
 cycler==0.12.1
 debugpy==1.8.1
 decorator==5.1.1
 defusedxml==0.7.1
 distlib==0.3.8
 dm-tree==0.1.8
 docstring-to-markdown==0.15
-docutils==0.20.1
-execnet==2.0.2
+docutils==0.21.2
+exceptiongroup==1.2.1
+execnet==2.1.1
 executing==2.0.1
 fastjsonschema==2.19.1
-filelock==3.13.1
-flatbuffers==24.3.7
-fonttools==4.50.0
+filelock==3.13.4
+flatbuffers==24.3.25
+fonttools==4.51.0
 fqdn==1.5.1
 gast==0.5.4
 gitdb==4.0.11
-gitpython==3.1.42
+gitpython==3.1.43
 google-pasta==0.2.0
-graphviz==0.20.1
+graphviz==0.20.3
 greenlet==3.0.3
-grpcio==1.62.1
+grpcio==1.62.2
 h11==0.14.0
-h5py==3.10.0
+h5py==3.11.0
 hepunits==2.3.3
-httpcore==1.0.4
+httpcore==1.0.5
 httpx==0.27.0
-identify==2.5.35
-idna==3.6
+identify==2.5.36
+idna==3.7
 imagesize==1.4.1
 iminuit==2.25.2
-importlib-metadata==7.0.2
+importlib-metadata==7.1.0
+importlib-resources==6.4.0
 iniconfig==2.0.0
-ipykernel==6.29.3
-ipympl==0.9.3
-ipython==8.22.2
+ipykernel==6.29.4
+ipympl==0.9.4
+ipython==8.18.1
 ipython-genutils==0.2.0
 ipywidgets==8.1.2
 isoduration==20.11.0
 isort==5.13.2
-jax==0.4.25
-jaxlib==0.4.25
+jax==0.4.26
+jaxlib==0.4.26
 jedi==0.19.1
 jinja2==3.1.3
-json5==0.9.24
+json5==0.9.25
 jsonpointer==2.4
 jsonschema==4.21.1
 jsonschema-specifications==2023.12.1
 jupyter-cache==1.0.0
 jupyter-client==8.6.1
 jupyter-core==5.7.2
-jupyter-events==0.9.1
-jupyter-lsp==2.2.4
-jupyter-server==2.13.0
+jupyter-events==0.10.0
+jupyter-lsp==2.2.5
+jupyter-server==2.14.0
 jupyter-server-mathjax==0.2.6
 jupyter-server-terminals==0.5.3
-jupyterlab==4.1.5
+jupyterlab==4.1.6
 jupyterlab-code-formatter==2.2.1
 jupyterlab-git==0.50.0
 jupyterlab-lsp==5.1.0
-jupyterlab-myst==2.3.1
+jupyterlab-myst==2.3.2
 jupyterlab-pygments==0.3.0
-jupyterlab-server==2.25.4
+jupyterlab-server==2.27.1
 jupyterlab-widgets==3.0.10
-keras==3.0.5
+keras==3.3.2
 kiwisolver==1.4.5
 latexcodec==3.0.0
-libclang==16.0.6
-livereload==2.6.3
+libclang==18.1.1
 llvmlite==0.42.0
 lsprotocol==2023.0.1
 markdown==3.6
 markdown-it-py==3.0.0
 markupsafe==2.1.5
-matplotlib==3.8.3
-matplotlib-inline==0.1.6
+matplotlib==3.8.4
+matplotlib-inline==0.1.7
 mdit-py-plugins==0.4.0
 mdurl==0.1.2
 mistune==3.0.2
 ml-dtypes==0.3.2
 mpmath==1.3.0
 mypy-extensions==1.0.0
-myst-nb==1.0.0
-myst-parser==2.0.0
-namex==0.0.7
+myst-nb==1.1.0
+myst-parser==3.0.0
+namex==0.0.8
 nbclient==0.6.8
-nbconvert==7.16.2
+nbconvert==7.16.3
 nbdime==4.0.1
-nbformat==5.10.3
+nbformat==5.10.4
 nbmake==1.5.3
 nest-asyncio==1.6.0
 nodeenv==1.8.0
 notebook-shim==0.2.4
-numba==0.59.0
+numba==0.59.1
 numpy==1.26.4
 opt-einsum==3.3.0
+optree==0.11.0
 overrides==7.7.0
 packaging==24.0
 pandocfilters==1.5.1
-parso==0.8.3
-particle==0.23.1
+parso==0.8.4
+particle==0.24.0
 pathspec==0.12.1
 pexpect==4.9.0
-phasespace==1.9.0
-pillow==10.2.0
-platformdirs==4.2.0
-pluggy==1.4.0
-pre-commit==3.6.2
+phasespace==1.10.3
+pillow==10.3.0
+platformdirs==4.2.1
+pluggy==1.5.0
+pre-commit==3.7.0
 prometheus-client==0.20.0
 prompt-toolkit==3.0.43
 protobuf==4.25.3
 psutil==5.9.8
 ptyprocess==0.7.0
 pure-eval==0.2.2
 pybtex==0.24.0
 pybtex-docutils==1.0.3
-pycparser==2.21
+pycparser==2.22
 pydata-sphinx-theme==0.15.2
 pygments==2.17.2
 pyparsing==3.1.2
 pyproject-api==1.6.1
 pytest==8.1.1
-pytest-cov==4.1.0
+pytest-cov==5.0.0
 pytest-xdist==3.5.0
-python-constraint==1.3.1
+python-constraint==1.4.0
 python-dateutil==2.9.0.post0
 python-json-logger==2.0.7
 python-lsp-jsonrpc==1.1.2
 python-lsp-ruff==2.2.0
-python-lsp-server==1.10.1
+python-lsp-server==1.11.0
 pytoolconfig==1.3.1
 pyyaml==6.0.1
-pyzmq==25.1.2
+pyzmq==26.0.2
 qrules==0.10.1
-referencing==0.34.0
+referencing==0.35.0
 requests==2.31.0
 rfc3339-validator==0.1.4
 rfc3986-validator==0.1.1
 rich==13.7.1
-rope==1.12.0
+rope==1.13.0
 rpds-py==0.18.0
-ruff==0.3.3
-scipy==1.12.0
-send2trash==1.8.2
+ruff==0.4.1
+scipy==1.13.0
+send2trash==1.8.3
 six==1.16.0
 smmap==5.0.1
 sniffio==1.3.1
 snowballstemmer==2.2.0
 soupsieve==2.5
-sphinx==7.2.6
-sphinx-api-relink==0.0.8
-sphinx-autobuild==2024.2.4
+sphinx==7.3.7
+sphinx-api-relink==0.0.9
+sphinx-autobuild==2024.4.16
 sphinx-book-theme==1.1.2
-sphinx-codeautolink==0.15.0
+sphinx-codeautolink==0.15.1
 sphinx-copybutton==0.5.2
 sphinx-design==0.5.0
 sphinx-pybtex-etal-style==0.0.2
 sphinx-togglebutton==0.3.2
 sphinxcontrib-applehelp==1.0.8
 sphinxcontrib-bibtex==2.6.2
 sphinxcontrib-devhelp==1.0.6
 sphinxcontrib-htmlhelp==2.0.5
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.7
 sphinxcontrib-serializinghtml==1.1.10
-sqlalchemy==2.0.28
+sqlalchemy==2.0.29
 stack-data==0.6.3
+starlette==0.37.2
 sympy==1.12
 tabulate==0.9.0
 tensorboard==2.16.2
 tensorboard-data-server==0.7.2
 tensorflow==2.16.1
 tensorflow-io-gcs-filesystem==0.36.0
 tensorflow-probability==0.24.0
 tensorwaves==0.4.12
 termcolor==2.4.0
 terminado==0.18.1
-tinycss2==1.2.1
+tinycss2==1.3.0
+tomli==2.0.1
 tornado==6.4
-tox==4.14.1
+tox==4.14.2
 tqdm==4.66.2
-traitlets==5.14.2
+traitlets==5.14.3
 types-python-dateutil==2.9.0.20240316
-typing-extensions==4.10.0
+typing-extensions==4.11.0
 ujson==5.9.0
 uri-template==1.3.0
 urllib3==2.2.1
-virtualenv==20.25.1
+uvicorn==0.29.0
+virtualenv==20.26.0
+watchfiles==0.21.0
 wcwidth==0.2.13
 webcolors==1.13
 webencodings==0.5.1
-websocket-client==1.7.0
-werkzeug==3.0.1
+websocket-client==1.8.0
+websockets==12.0
+werkzeug==3.0.2
 wheel==0.43.0
 widgetsnbextension==4.0.10
 wrapt==1.16.0
 zipp==3.18.1
 
 # The following packages were excluded from the output:
 # setuptools
```

### Comparing `ampform-dpd-0.1.6/.constraints/py3.12.txt` & `ampform_dpd-0.1.7/.constraints/py3.11.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,230 +1,235 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile pyproject.toml -o .constraints/py3.12.txt --all-extras --no-annotate --python-version=3.12 --no-emit-package setuptools
+#    uv pip compile pyproject.toml -o .constraints/py3.11.txt --all-extras --no-annotate --python-version=3.11 --no-emit-package setuptools
 absl-py==2.1.0
 accessible-pygments==0.0.4
 alabaster==0.7.16
 ampform==0.15.0
 anyio==4.3.0
 argon2-cffi==23.1.0
 argon2-cffi-bindings==21.2.0
 arrow==1.3.0
 asttokens==2.4.1
 astunparse==1.6.3
 async-lru==2.0.4
 attrs==23.2.0
 babel==2.14.0
 beautifulsoup4==4.12.3
-black==24.3.0
+black==24.4.0
 bleach==6.1.0
 cachetools==5.3.3
 cattrs==23.2.3
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 chardet==5.2.0
 charset-normalizer==3.3.2
 click==8.1.7
 cloudpickle==3.0.0
 colorama==0.4.6
 comm==0.2.2
-contourpy==1.2.0
-coverage==7.4.4
+contourpy==1.2.1
+coverage==7.5.0
 cycler==0.12.1
 debugpy==1.8.1
 decorator==5.1.1
 defusedxml==0.7.1
 distlib==0.3.8
 dm-tree==0.1.8
 docstring-to-markdown==0.15
-docutils==0.20.1
-execnet==2.0.2
+docutils==0.21.2
+execnet==2.1.1
 executing==2.0.1
 fastjsonschema==2.19.1
-filelock==3.13.1
-flatbuffers==24.3.7
-fonttools==4.50.0
+filelock==3.13.4
+flatbuffers==24.3.25
+fonttools==4.51.0
 fqdn==1.5.1
 gast==0.5.4
 gitdb==4.0.11
-gitpython==3.1.42
+gitpython==3.1.43
 google-pasta==0.2.0
-graphviz==0.20.1
+graphviz==0.20.3
 greenlet==3.0.3
-grpcio==1.62.1
+grpcio==1.62.2
 h11==0.14.0
-h5py==3.10.0
+h5py==3.11.0
 hepunits==2.3.3
-httpcore==1.0.4
+httpcore==1.0.5
 httpx==0.27.0
-identify==2.5.35
-idna==3.6
+identify==2.5.36
+idna==3.7
 imagesize==1.4.1
 iminuit==2.25.2
-importlib-metadata==7.0.2
+importlib-metadata==7.1.0
 iniconfig==2.0.0
-ipykernel==6.29.3
-ipympl==0.9.3
-ipython==8.22.2
+ipykernel==6.29.4
+ipympl==0.9.4
+ipython==8.23.0
 ipython-genutils==0.2.0
 ipywidgets==8.1.2
 isoduration==20.11.0
 isort==5.13.2
-jax==0.4.25
-jaxlib==0.4.25
+jax==0.4.26
+jaxlib==0.4.26
 jedi==0.19.1
 jinja2==3.1.3
-json5==0.9.24
+json5==0.9.25
 jsonpointer==2.4
 jsonschema==4.21.1
 jsonschema-specifications==2023.12.1
 jupyter-cache==1.0.0
 jupyter-client==8.6.1
 jupyter-core==5.7.2
-jupyter-events==0.9.1
-jupyter-lsp==2.2.4
-jupyter-server==2.13.0
+jupyter-events==0.10.0
+jupyter-lsp==2.2.5
+jupyter-server==2.14.0
 jupyter-server-mathjax==0.2.6
 jupyter-server-terminals==0.5.3
-jupyterlab==4.1.5
+jupyterlab==4.1.6
 jupyterlab-code-formatter==2.2.1
 jupyterlab-git==0.50.0
 jupyterlab-lsp==5.1.0
-jupyterlab-myst==2.3.1
+jupyterlab-myst==2.3.2
 jupyterlab-pygments==0.3.0
-jupyterlab-server==2.25.4
+jupyterlab-server==2.27.1
 jupyterlab-widgets==3.0.10
-keras==3.0.5
+keras==3.3.2
 kiwisolver==1.4.5
 latexcodec==3.0.0
-libclang==16.0.6
-livereload==2.6.3
+libclang==18.1.1
 llvmlite==0.42.0
 lsprotocol==2023.0.1
 markdown==3.6
 markdown-it-py==3.0.0
 markupsafe==2.1.5
-matplotlib==3.8.3
-matplotlib-inline==0.1.6
+matplotlib==3.8.4
+matplotlib-inline==0.1.7
 mdit-py-plugins==0.4.0
 mdurl==0.1.2
 mistune==3.0.2
 ml-dtypes==0.3.2
 mpmath==1.3.0
 mypy-extensions==1.0.0
-myst-nb==1.0.0
-myst-parser==2.0.0
-namex==0.0.7
+myst-nb==1.1.0
+myst-parser==3.0.0
+namex==0.0.8
 nbclient==0.6.8
-nbconvert==7.16.2
+nbconvert==7.16.3
 nbdime==4.0.1
-nbformat==5.10.3
+nbformat==5.10.4
 nbmake==1.5.3
 nest-asyncio==1.6.0
 nodeenv==1.8.0
 notebook-shim==0.2.4
-numba==0.59.0
+numba==0.59.1
 numpy==1.26.4
 opt-einsum==3.3.0
+optree==0.11.0
 overrides==7.7.0
 packaging==24.0
 pandocfilters==1.5.1
-parso==0.8.3
-particle==0.23.1
+parso==0.8.4
+particle==0.24.0
 pathspec==0.12.1
 pexpect==4.9.0
-phasespace==1.9.0
-pillow==10.2.0
-platformdirs==4.2.0
-pluggy==1.4.0
-pre-commit==3.6.2
+phasespace==1.10.3
+pillow==10.3.0
+platformdirs==4.2.1
+pluggy==1.5.0
+pre-commit==3.7.0
 prometheus-client==0.20.0
 prompt-toolkit==3.0.43
 protobuf==4.25.3
 psutil==5.9.8
 ptyprocess==0.7.0
 pure-eval==0.2.2
 pybtex==0.24.0
 pybtex-docutils==1.0.3
-pycparser==2.21
+pycparser==2.22
 pydata-sphinx-theme==0.15.2
 pygments==2.17.2
 pyparsing==3.1.2
 pyproject-api==1.6.1
 pytest==8.1.1
-pytest-cov==4.1.0
+pytest-cov==5.0.0
 pytest-xdist==3.5.0
-python-constraint==1.3.1
+python-constraint==1.4.0
 python-dateutil==2.9.0.post0
 python-json-logger==2.0.7
 python-lsp-jsonrpc==1.1.2
 python-lsp-ruff==2.2.0
-python-lsp-server==1.10.1
+python-lsp-server==1.11.0
 pytoolconfig==1.3.1
 pyyaml==6.0.1
-pyzmq==25.1.2
+pyzmq==26.0.2
 qrules==0.10.1
-referencing==0.34.0
+referencing==0.35.0
 requests==2.31.0
 rfc3339-validator==0.1.4
 rfc3986-validator==0.1.1
 rich==13.7.1
-rope==1.12.0
+rope==1.13.0
 rpds-py==0.18.0
-ruff==0.3.3
-scipy==1.12.0
-send2trash==1.8.2
+ruff==0.4.1
+scipy==1.13.0
+send2trash==1.8.3
 six==1.16.0
 smmap==5.0.1
 sniffio==1.3.1
 snowballstemmer==2.2.0
 soupsieve==2.5
-sphinx==7.2.6
-sphinx-api-relink==0.0.8
-sphinx-autobuild==2024.2.4
+sphinx==7.3.7
+sphinx-api-relink==0.0.9
+sphinx-autobuild==2024.4.16
 sphinx-book-theme==1.1.2
-sphinx-codeautolink==0.15.0
+sphinx-codeautolink==0.15.1
 sphinx-copybutton==0.5.2
 sphinx-design==0.5.0
 sphinx-pybtex-etal-style==0.0.2
 sphinx-togglebutton==0.3.2
 sphinxcontrib-applehelp==1.0.8
 sphinxcontrib-bibtex==2.6.2
 sphinxcontrib-devhelp==1.0.6
 sphinxcontrib-htmlhelp==2.0.5
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.7
 sphinxcontrib-serializinghtml==1.1.10
-sqlalchemy==2.0.28
+sqlalchemy==2.0.29
 stack-data==0.6.3
+starlette==0.37.2
 sympy==1.12
 tabulate==0.9.0
 tensorboard==2.16.2
 tensorboard-data-server==0.7.2
 tensorflow==2.16.1
+tensorflow-io-gcs-filesystem==0.36.0
 tensorflow-probability==0.24.0
 tensorwaves==0.4.12
 termcolor==2.4.0
 terminado==0.18.1
-tinycss2==1.2.1
+tinycss2==1.3.0
 tornado==6.4
-tox==4.14.1
+tox==4.14.2
 tqdm==4.66.2
-traitlets==5.14.2
+traitlets==5.14.3
 types-python-dateutil==2.9.0.20240316
-typing-extensions==4.10.0
+typing-extensions==4.11.0
 ujson==5.9.0
 uri-template==1.3.0
 urllib3==2.2.1
-virtualenv==20.25.1
+uvicorn==0.29.0
+virtualenv==20.26.0
+watchfiles==0.21.0
 wcwidth==0.2.13
 webcolors==1.13
 webencodings==0.5.1
-websocket-client==1.7.0
-werkzeug==3.0.1
+websocket-client==1.8.0
+websockets==12.0
+werkzeug==3.0.2
 wheel==0.43.0
 widgetsnbextension==4.0.10
 wrapt==1.16.0
 zipp==3.18.1
 
 # The following packages were excluded from the output:
 # setuptools
```

### Comparing `ampform-dpd-0.1.6/.constraints/py3.8.txt` & `ampform_dpd-0.1.7/.constraints/py3.8.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,235 +11,235 @@
 asttokens==2.4.1
 astunparse==1.6.3
 async-lru==2.0.4
 attrs==23.2.0
 babel==2.14.0
 backcall==0.2.0
 beautifulsoup4==4.12.3
-black==24.3.0
+black==24.4.0
 bleach==6.1.0
 cachetools==5.3.3
 cattrs==23.2.3
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 chardet==5.2.0
 charset-normalizer==3.3.2
 click==8.1.7
 cloudpickle==3.0.0
 colorama==0.4.6
 comm==0.2.2
 contourpy==1.1.1
-coverage==7.4.4
+coverage==7.5.0
 cycler==0.12.1
 debugpy==1.8.1
 decorator==5.1.1
 defusedxml==0.7.1
 distlib==0.3.8
 dm-tree==0.1.8
 docstring-to-markdown==0.15
 docutils==0.17.1
-exceptiongroup==1.2.0
-execnet==2.0.2
+exceptiongroup==1.2.1
+execnet==2.1.1
 executing==2.0.1
 fastjsonschema==2.19.1
-filelock==3.13.1
-flatbuffers==24.3.7
-fonttools==4.50.0
+filelock==3.13.4
+flatbuffers==24.3.25
+fonttools==4.51.0
 fqdn==1.5.1
 gast==0.4.0
 gitdb==4.0.11
-gitpython==3.1.42
-google-auth==2.28.2
+gitpython==3.1.43
+google-auth==2.29.0
 google-auth-oauthlib==0.4.6
 google-pasta==0.2.0
-graphviz==0.20.1
+graphviz==0.20.3
 greenlet==3.0.3
-grpcio==1.62.1
+grpcio==1.62.2
 h11==0.14.0
-h5py==3.10.0
+h5py==3.11.0
 hepunits==2.3.3
-httpcore==1.0.4
+httpcore==1.0.5
 httpx==0.27.0
-identify==2.5.35
-idna==3.6
+identify==2.5.36
+idna==3.7
 imagesize==1.4.1
 iminuit==2.25.2
-importlib-metadata==7.0.2
-importlib-resources==6.3.1
+importlib-metadata==7.1.0
+importlib-resources==6.4.0
 iniconfig==2.0.0
-ipykernel==6.29.3
+ipykernel==6.29.4
 ipympl==0.9.3
 ipython==8.12.3
 ipython-genutils==0.2.0
 ipywidgets==8.1.2
 isoduration==20.11.0
 isort==5.13.2
 jax==0.4.13
 jaxlib==0.4.13
 jedi==0.19.1
 jinja2==3.1.3
-json5==0.9.24
+json5==0.9.25
 jsonpointer==2.4
 jsonschema==4.21.1
 jsonschema-specifications==2023.12.1
 jupyter-cache==0.6.1
 jupyter-client==8.6.1
 jupyter-core==5.7.2
-jupyter-events==0.9.1
-jupyter-lsp==2.2.4
-jupyter-server==2.13.0
+jupyter-events==0.10.0
+jupyter-lsp==2.2.5
+jupyter-server==2.14.0
 jupyter-server-mathjax==0.2.6
 jupyter-server-terminals==0.5.3
-jupyterlab==4.1.5
+jupyterlab==4.1.6
 jupyterlab-code-formatter==2.2.1
 jupyterlab-git==0.50.0
 jupyterlab-lsp==5.1.0
-jupyterlab-myst==2.3.1
+jupyterlab-myst==2.3.2
 jupyterlab-pygments==0.3.0
-jupyterlab-server==2.25.4
+jupyterlab-server==2.27.1
 jupyterlab-widgets==3.0.10
 keras==2.11.0
 kiwisolver==1.4.5
 latexcodec==3.0.0
-libclang==16.0.6
+libclang==18.1.1
 livereload==2.6.3
 llvmlite==0.41.1
 lsprotocol==2023.0.1
 markdown==3.6
 markdown-it-py==2.2.0
 markupsafe==2.1.5
 matplotlib==3.7.5
-matplotlib-inline==0.1.6
+matplotlib-inline==0.1.7
 mdit-py-plugins==0.3.5
 mdurl==0.1.2
 mistune==3.0.2
 ml-dtypes==0.2.0
 mpmath==1.3.0
 mypy-extensions==1.0.0
 myst-nb==0.17.2
 myst-parser==0.18.1
 nbclient==0.6.8
-nbconvert==7.16.2
+nbconvert==7.16.3
 nbdime==4.0.1
-nbformat==5.10.3
+nbformat==5.10.4
 nbmake==1.5.3
 nest-asyncio==1.6.0
 nodeenv==1.8.0
 notebook-shim==0.2.4
 numba==0.58.1
 numpy==1.24.4
 oauthlib==3.2.2
 opt-einsum==3.3.0
 overrides==7.7.0
 packaging==24.0
 pandocfilters==1.5.1
-parso==0.8.3
-particle==0.23.1
+parso==0.8.4
+particle==0.24.0
 pathspec==0.12.1
 pexpect==4.9.0
 phasespace==1.9.0
 pickleshare==0.7.5
-pillow==10.2.0
+pillow==10.3.0
 pkgutil-resolve-name==1.3.10
-platformdirs==4.2.0
-pluggy==1.4.0
+platformdirs==4.2.1
+pluggy==1.5.0
 pre-commit==3.5.0
 prometheus-client==0.20.0
 prompt-toolkit==3.0.43
 protobuf==3.19.6
 psutil==5.9.8
 ptyprocess==0.7.0
 pure-eval==0.2.2
-pyasn1==0.5.1
-pyasn1-modules==0.3.0
+pyasn1==0.6.0
+pyasn1-modules==0.4.0
 pybtex==0.24.0
 pybtex-docutils==1.0.3
-pycparser==2.21
+pycparser==2.22
 pydata-sphinx-theme==0.14.4
 pygments==2.17.2
 pyparsing==3.1.2
 pyproject-api==1.6.1
 pytest==8.1.1
-pytest-cov==4.1.0
+pytest-cov==5.0.0
 pytest-xdist==3.5.0
-python-constraint==1.3.1
+python-constraint==1.4.0
 python-dateutil==2.9.0.post0
 python-json-logger==2.0.7
 python-lsp-jsonrpc==1.1.2
 python-lsp-ruff==2.2.0
-python-lsp-server==1.10.1
+python-lsp-server==1.11.0
 pytoolconfig==1.3.1
 pytz==2024.1
 pyyaml==6.0.1
-pyzmq==25.1.2
+pyzmq==26.0.2
 qrules==0.10.1
-referencing==0.34.0
+referencing==0.35.0
 requests==2.31.0
-requests-oauthlib==1.4.0
+requests-oauthlib==2.0.0
 rfc3339-validator==0.1.4
 rfc3986-validator==0.1.1
-rope==1.12.0
+rope==1.13.0
 rpds-py==0.18.0
 rsa==4.9
-ruff==0.3.3
+ruff==0.4.1
 scipy==1.10.1
-send2trash==1.8.2
+send2trash==1.8.3
 six==1.16.0
 smmap==5.0.1
 sniffio==1.3.1
 snowballstemmer==2.2.0
 soupsieve==2.5
 sphinx==5.3.0
-sphinx-api-relink==0.0.8
+sphinx-api-relink==0.0.9
 sphinx-autobuild==2021.3.14
 sphinx-book-theme==1.0.1
-sphinx-codeautolink==0.15.0
+sphinx-codeautolink==0.15.1
 sphinx-copybutton==0.5.2
 sphinx-design==0.5.0
 sphinx-pybtex-etal-style==0.0.2
 sphinx-togglebutton==0.3.2
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-bibtex==2.6.2
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-sqlalchemy==2.0.28
+sqlalchemy==2.0.29
 stack-data==0.6.3
 sympy==1.12
 tabulate==0.9.0
 tensorboard==2.11.2
 tensorboard-data-server==0.6.1
 tensorboard-plugin-wit==1.8.1
 tensorflow==2.11.1
 tensorflow-estimator==2.11.0
 tensorflow-io-gcs-filesystem==0.34.0
 tensorflow-probability==0.20.1
 tensorwaves==0.4.12
 termcolor==2.4.0
 terminado==0.18.1
-tinycss2==1.2.1
+tinycss2==1.3.0
 tomli==2.0.1
 tornado==6.4
-tox==4.14.1
+tox==4.14.2
 tqdm==4.66.2
-traitlets==5.14.2
+traitlets==5.14.3
 types-python-dateutil==2.9.0.20240316
-typing-extensions==4.10.0
+typing-extensions==4.11.0
 ujson==5.9.0
 uri-template==1.3.0
 urllib3==2.2.1
-virtualenv==20.25.1
+virtualenv==20.26.0
 wcwidth==0.2.13
 webcolors==1.13
 webencodings==0.5.1
-websocket-client==1.7.0
-werkzeug==3.0.1
+websocket-client==1.8.0
+werkzeug==3.0.2
 wheel==0.43.0
 widgetsnbextension==4.0.10
 wrapt==1.16.0
 zipp==3.18.1
 
 # The following packages were excluded from the output:
 # setuptools
```

### Comparing `ampform-dpd-0.1.6/.constraints/py3.9.txt` & `ampform_dpd-0.1.7/.constraints/py3.12.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,234 +1,234 @@
 # This file was autogenerated by uv via the following command:
-#    uv pip compile pyproject.toml -o .constraints/py3.9.txt --all-extras --no-annotate --python-version=3.9 --no-emit-package setuptools
+#    uv pip compile pyproject.toml -o .constraints/py3.12.txt --all-extras --no-annotate --python-version=3.12 --no-emit-package setuptools
 absl-py==2.1.0
 accessible-pygments==0.0.4
 alabaster==0.7.16
 ampform==0.15.0
 anyio==4.3.0
 argon2-cffi==23.1.0
 argon2-cffi-bindings==21.2.0
 arrow==1.3.0
 asttokens==2.4.1
 astunparse==1.6.3
 async-lru==2.0.4
 attrs==23.2.0
 babel==2.14.0
 beautifulsoup4==4.12.3
-black==24.3.0
+black==24.4.0
 bleach==6.1.0
 cachetools==5.3.3
 cattrs==23.2.3
 certifi==2024.2.2
 cffi==1.16.0
 cfgv==3.4.0
 chardet==5.2.0
 charset-normalizer==3.3.2
 click==8.1.7
 cloudpickle==3.0.0
 colorama==0.4.6
 comm==0.2.2
-contourpy==1.2.0
-coverage==7.4.4
+contourpy==1.2.1
+coverage==7.5.0
 cycler==0.12.1
 debugpy==1.8.1
 decorator==5.1.1
 defusedxml==0.7.1
 distlib==0.3.8
 dm-tree==0.1.8
 docstring-to-markdown==0.15
-docutils==0.20.1
-exceptiongroup==1.2.0
-execnet==2.0.2
+docutils==0.21.2
+execnet==2.1.1
 executing==2.0.1
 fastjsonschema==2.19.1
-filelock==3.13.1
-flatbuffers==24.3.7
-fonttools==4.50.0
+filelock==3.13.4
+flatbuffers==24.3.25
+fonttools==4.51.0
 fqdn==1.5.1
 gast==0.5.4
 gitdb==4.0.11
-gitpython==3.1.42
+gitpython==3.1.43
 google-pasta==0.2.0
-graphviz==0.20.1
+graphviz==0.20.3
 greenlet==3.0.3
-grpcio==1.62.1
+grpcio==1.62.2
 h11==0.14.0
-h5py==3.10.0
+h5py==3.11.0
 hepunits==2.3.3
-httpcore==1.0.4
+httpcore==1.0.5
 httpx==0.27.0
-identify==2.5.35
-idna==3.6
+identify==2.5.36
+idna==3.7
 imagesize==1.4.1
 iminuit==2.25.2
-importlib-metadata==7.0.2
-importlib-resources==6.3.1
+importlib-metadata==7.1.0
 iniconfig==2.0.0
-ipykernel==6.29.3
-ipympl==0.9.3
-ipython==8.18.1
+ipykernel==6.29.4
+ipympl==0.9.4
+ipython==8.23.0
 ipython-genutils==0.2.0
 ipywidgets==8.1.2
 isoduration==20.11.0
 isort==5.13.2
-jax==0.4.25
-jaxlib==0.4.25
+jax==0.4.26
+jaxlib==0.4.26
 jedi==0.19.1
 jinja2==3.1.3
-json5==0.9.24
+json5==0.9.25
 jsonpointer==2.4
 jsonschema==4.21.1
 jsonschema-specifications==2023.12.1
 jupyter-cache==1.0.0
 jupyter-client==8.6.1
 jupyter-core==5.7.2
-jupyter-events==0.9.1
-jupyter-lsp==2.2.4
-jupyter-server==2.13.0
+jupyter-events==0.10.0
+jupyter-lsp==2.2.5
+jupyter-server==2.14.0
 jupyter-server-mathjax==0.2.6
 jupyter-server-terminals==0.5.3
-jupyterlab==4.1.5
+jupyterlab==4.1.6
 jupyterlab-code-formatter==2.2.1
 jupyterlab-git==0.50.0
 jupyterlab-lsp==5.1.0
-jupyterlab-myst==2.3.1
+jupyterlab-myst==2.3.2
 jupyterlab-pygments==0.3.0
-jupyterlab-server==2.25.4
+jupyterlab-server==2.27.1
 jupyterlab-widgets==3.0.10
-keras==3.0.5
+keras==3.3.2
 kiwisolver==1.4.5
 latexcodec==3.0.0
-libclang==16.0.6
-livereload==2.6.3
+libclang==18.1.1
 llvmlite==0.42.0
 lsprotocol==2023.0.1
 markdown==3.6
 markdown-it-py==3.0.0
 markupsafe==2.1.5
-matplotlib==3.8.3
-matplotlib-inline==0.1.6
+matplotlib==3.8.4
+matplotlib-inline==0.1.7
 mdit-py-plugins==0.4.0
 mdurl==0.1.2
 mistune==3.0.2
 ml-dtypes==0.3.2
 mpmath==1.3.0
 mypy-extensions==1.0.0
-myst-nb==1.0.0
-myst-parser==2.0.0
-namex==0.0.7
+myst-nb==1.1.0
+myst-parser==3.0.0
+namex==0.0.8
 nbclient==0.6.8
-nbconvert==7.16.2
+nbconvert==7.16.3
 nbdime==4.0.1
-nbformat==5.10.3
+nbformat==5.10.4
 nbmake==1.5.3
 nest-asyncio==1.6.0
 nodeenv==1.8.0
 notebook-shim==0.2.4
-numba==0.59.0
+numba==0.59.1
 numpy==1.26.4
 opt-einsum==3.3.0
+optree==0.11.0
 overrides==7.7.0
 packaging==24.0
 pandocfilters==1.5.1
-parso==0.8.3
-particle==0.23.1
+parso==0.8.4
+particle==0.24.0
 pathspec==0.12.1
 pexpect==4.9.0
-phasespace==1.9.0
-pillow==10.2.0
-platformdirs==4.2.0
-pluggy==1.4.0
-pre-commit==3.6.2
+phasespace==1.10.3
+pillow==10.3.0
+platformdirs==4.2.1
+pluggy==1.5.0
+pre-commit==3.7.0
 prometheus-client==0.20.0
 prompt-toolkit==3.0.43
 protobuf==4.25.3
 psutil==5.9.8
 ptyprocess==0.7.0
 pure-eval==0.2.2
 pybtex==0.24.0
 pybtex-docutils==1.0.3
-pycparser==2.21
+pycparser==2.22
 pydata-sphinx-theme==0.15.2
 pygments==2.17.2
 pyparsing==3.1.2
 pyproject-api==1.6.1
 pytest==8.1.1
-pytest-cov==4.1.0
+pytest-cov==5.0.0
 pytest-xdist==3.5.0
-python-constraint==1.3.1
+python-constraint==1.4.0
 python-dateutil==2.9.0.post0
 python-json-logger==2.0.7
 python-lsp-jsonrpc==1.1.2
 python-lsp-ruff==2.2.0
-python-lsp-server==1.10.1
+python-lsp-server==1.11.0
 pytoolconfig==1.3.1
 pyyaml==6.0.1
-pyzmq==25.1.2
+pyzmq==26.0.2
 qrules==0.10.1
-referencing==0.34.0
+referencing==0.35.0
 requests==2.31.0
 rfc3339-validator==0.1.4
 rfc3986-validator==0.1.1
 rich==13.7.1
-rope==1.12.0
+rope==1.13.0
 rpds-py==0.18.0
-ruff==0.3.3
-scipy==1.12.0
-send2trash==1.8.2
+ruff==0.4.1
+scipy==1.13.0
+send2trash==1.8.3
 six==1.16.0
 smmap==5.0.1
 sniffio==1.3.1
 snowballstemmer==2.2.0
 soupsieve==2.5
-sphinx==7.2.6
-sphinx-api-relink==0.0.8
-sphinx-autobuild==2024.2.4
+sphinx==7.3.7
+sphinx-api-relink==0.0.9
+sphinx-autobuild==2024.4.16
 sphinx-book-theme==1.1.2
-sphinx-codeautolink==0.15.0
+sphinx-codeautolink==0.15.1
 sphinx-copybutton==0.5.2
 sphinx-design==0.5.0
 sphinx-pybtex-etal-style==0.0.2
 sphinx-togglebutton==0.3.2
 sphinxcontrib-applehelp==1.0.8
 sphinxcontrib-bibtex==2.6.2
 sphinxcontrib-devhelp==1.0.6
 sphinxcontrib-htmlhelp==2.0.5
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.7
 sphinxcontrib-serializinghtml==1.1.10
-sqlalchemy==2.0.28
+sqlalchemy==2.0.29
 stack-data==0.6.3
+starlette==0.37.2
 sympy==1.12
 tabulate==0.9.0
 tensorboard==2.16.2
 tensorboard-data-server==0.7.2
 tensorflow==2.16.1
-tensorflow-io-gcs-filesystem==0.36.0
 tensorflow-probability==0.24.0
 tensorwaves==0.4.12
 termcolor==2.4.0
 terminado==0.18.1
-tinycss2==1.2.1
-tomli==2.0.1
+tinycss2==1.3.0
 tornado==6.4
-tox==4.14.1
+tox==4.14.2
 tqdm==4.66.2
-traitlets==5.14.2
+traitlets==5.14.3
 types-python-dateutil==2.9.0.20240316
-typing-extensions==4.10.0
+typing-extensions==4.11.0
 ujson==5.9.0
 uri-template==1.3.0
 urllib3==2.2.1
-virtualenv==20.25.1
+uvicorn==0.29.0
+virtualenv==20.26.0
+watchfiles==0.21.0
 wcwidth==0.2.13
 webcolors==1.13
 webencodings==0.5.1
-websocket-client==1.7.0
-werkzeug==3.0.1
+websocket-client==1.8.0
+websockets==12.0
+werkzeug==3.0.2
 wheel==0.43.0
 widgetsnbextension==4.0.10
 wrapt==1.16.0
 zipp==3.18.1
 
 # The following packages were excluded from the output:
 # setuptools
```

### Comparing `ampform-dpd-0.1.6/.cspell.json` & `ampform_dpd-0.1.7/.cspell.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9904130591630592%*

 * *Differences: {"'ignorePaths'": "{insert: [(3, '*particle*.*ml')]}",*

 * * "'ignoreWords'": "{insert: [(73, 'simplefilter')]}",*

 * * "'words'": "{insert: [(14, 'isospin'), (29, 'sympify')]}"}*

```diff
@@ -18,14 +18,15 @@
         "transision",
         "transisions"
     ],
     "ignorePaths": [
         "**/*.bib",
         "**/.cspell.json",
         "*.ico",
+        "*particle*.*ml",
         ".constraints/*.txt",
         ".editorconfig",
         ".gitignore",
         ".gitpod.*",
         ".pre-commit-config.yaml",
         ".prettierignore",
         ".vscode/*",
@@ -105,14 +106,15 @@
         "redeboer",
         "repr",
         "savefig",
         "sdist",
         "seealso",
         "setuptools",
         "sharey",
+        "simplefilter",
         "startswith",
         "suptitle",
         "textwrap",
         "toctree",
         "tqdm",
         "trigsimp",
         "unsrt",
@@ -139,26 +141,28 @@
         "Conda",
         "Dalitz",
         "doctests",
         "Flatt\u00e9",
         "Gordan",
         "helicities",
         "helicity",
+        "isospin",
         "JPAC",
         "lambdify",
         "lambdifying",
         "LHCb",
         "lineshape",
         "lineshapes",
         "matplotlib",
         "NumPy",
         "PyPA",
         "pyplot",
         "pyright",
         "pytest",
         "PYTHONHASHSEED",
         "QRules",
+        "sympify",
         "SymPy",
         "TensorWaves",
         "Weisskopf"
     ]
 }
```

### Comparing `ampform-dpd-0.1.6/.github/release-drafter.yml` & `ampform_dpd-0.1.7/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ampform-dpd-0.1.6/.github/workflows/cd.yml` & `ampform_dpd-0.1.7/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `ampform-dpd-0.1.6/.github/workflows/ci.yml` & `ampform_dpd-0.1.7/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ampform-dpd-0.1.6/.github/workflows/requirements.yml` & `ampform_dpd-0.1.7/.github/workflows/requirements.yml`

 * *Files identical despite different names*

### Comparing `ampform-dpd-0.1.6/.gitpod.yml` & `ampform_dpd-0.1.7/.gitpod.yml`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     - eamodio.gitlens
     - editorconfig.editorconfig
     - esbenp.prettier-vscode
     - executablebookproject.myst-highlight
     - github.vscode-github-actions
     - github.vscode-pull-request-github
     - ms-python.python
+    - ms-python.mypy-type-checker
     - ms-python.vscode-pylance
     - ms-toolsai.vscode-jupyter-cell-tags
     - ms-vscode.live-server
     - ms-vsliveshare.vsliveshare
     - oijaz.unicode-latex
     - redhat.vscode-yaml
     - soulcode.vscode-unwanted-extensions
```

### Comparing `ampform-dpd-0.1.6/.pre-commit-config.yaml` & `ampform_dpd-0.1.7/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ci:
   autoupdate_commit_msg: "MAINT: update pip constraints and pre-commit"
   autoupdate_schedule: quarterly # already done by requirements-cron.yml
   skip:
+    - mypy
     - prettier
     - pyright
     - taplo
 
 repos:
   - repo: meta
     hooks:
@@ -17,16 +18,18 @@
     hooks:
       - id: nbstripout
         args:
           - --extra-keys
           - |
             cell.attachments
             cell.metadata.code_folding
+            cell.metadata.editable
             cell.metadata.id
             cell.metadata.pycharm
+            cell.metadata.slideshow
             cell.metadata.user_expressions
             metadata.celltoolbar
             metadata.colab.name
             metadata.colab.provenance
             metadata.interpreter
             metadata.notify_time
             metadata.toc
@@ -34,36 +37,36 @@
             metadata.toc-showcode
             metadata.toc-showmarkdowntxt
             metadata.toc-showtags
             metadata.varInspector
             metadata.vscode
 
   - repo: https://github.com/ComPWA/policy
-    rev: 0.3.3
+    rev: 0.3.6
     hooks:
       - id: check-dev-files
         args:
           - --doc-apt-packages=graphviz
           - --no-prettierrc
           - --pin-requirements=bimonthly
           - --repo-name=ampform-dpd
           - --repo-title=AmpForm-DPD
       - id: colab-toc-visible
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.3
+    rev: v0.4.1
     hooks:
       - id: ruff
         args: [--fix]
         types_or: [python, pyi, jupyter]
       - id: ruff-format
         types_or: [python, pyi, jupyter]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-ast
       - id: check-case-conflict
       - id: check-json
       - id: check-merge-conflict
       - id: check-toml
       - id: check-vcs-permalinks
@@ -87,26 +90,36 @@
     rev: v0.23.1
     hooks:
       - id: toml-sort
         args:
           - --in-place
 
   - repo: https://github.com/streetsidesoftware/cspell-cli
-    rev: v8.6.0
+    rev: v8.7.0
     hooks:
       - id: cspell
 
   - repo: https://github.com/editorconfig-checker/editorconfig-checker.python
     rev: 2.7.3
     hooks:
       - id: editorconfig-checker
         name: editorconfig
         alias: ec
         exclude: >-
           (?x)^(
             .*\.py
           )$
 
+  - repo: local
+    hooks:
+      - id: mypy
+        name: mypy
+        entry: mypy
+        language: system
+        require_serial: true
+        types:
+          - python
+
   - repo: https://github.com/ComPWA/mirrors-pyright
-    rev: v1.1.354
+    rev: v1.1.359
     hooks:
       - id: pyright
```

### Comparing `ampform-dpd-0.1.6/.vscode/extensions.json` & `ampform_dpd-0.1.7/.vscode/extensions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9624999999999999%*

 * *Differences: {"'recommendations'": "{insert: [(8, 'ms-python.mypy-type-checker')]}",*

 * * "'unwantedRecommendations'": '{delete: [6]}'}*

```diff
@@ -4,14 +4,15 @@
         "eamodio.gitlens",
         "editorconfig.editorconfig",
         "esbenp.prettier-vscode",
         "executablebookproject.myst-highlight",
         "github.vscode-github-actions",
         "github.vscode-pull-request-github",
         "ms-python.python",
+        "ms-python.mypy-type-checker",
         "ms-python.vscode-pylance",
         "ms-toolsai.vscode-jupyter-cell-tags",
         "ms-vscode.live-server",
         "ms-vsliveshare.vsliveshare",
         "oijaz.unicode-latex",
         "redhat.vscode-yaml",
         "soulcode.vscode-unwanted-extensions",
@@ -23,13 +24,12 @@
     "unwantedRecommendations": [
         "bungcip.better-toml",
         "davidanson.vscode-markdownlint",
         "garaioag.garaio-vscode-unwanted-recommendations",
         "ms-python.black-formatter",
         "ms-python.flake8",
         "ms-python.isort",
-        "ms-python.mypy-type-checker",
         "ms-python.pylint",
         "travisillig.vscode-json-stable-stringify",
         "tyriar.sort-lines"
     ]
 }
```

### Comparing `ampform-dpd-0.1.6/.vscode/settings.json` & `ampform_dpd-0.1.7/.vscode/settings.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8970588235294118%*

 * *Differences: {"'mypy-type-checker.args'": "['--config-file=${workspaceFolder}/pyproject.toml']",*

 * * "'mypy-type-checker.importStrategy'": "'fromEnvironment'",*

 * * "'search.exclude'": "OrderedDict([('**/tests/**/__init__.py', True), ('.constraints/*.txt', "*

 * *                     "True), ('typings/**', True)])",*

 * * "'yaml.schemas'": '{replace: '*

 * *                   "OrderedDict([('https://raw.githubusercontent.com/ComPWA/qrules/0.10.x/src/qrules/particle-validation.json', "*

 * *                   "['*particle*.y*ml'])])}"}*

```diff
@@ -40,14 +40,18 @@
     "files.eol": "\n",
     "github-actions.workflows.pinned.workflows": [
         ".github/workflows/ci.yml"
     ],
     "gitlens.telemetry.enabled": false,
     "livePreview.defaultPreviewPath": "docs/_build/html",
     "multiDiffEditor.experimental.enabled": true,
+    "mypy-type-checker.args": [
+        "--config-file=${workspaceFolder}/pyproject.toml"
+    ],
+    "mypy-type-checker.importStrategy": "fromEnvironment",
     "notebook.codeActionsOnSave": {
         "notebook.source.organizeImports": "explicit"
     },
     "notebook.formatOnSave.enabled": true,
     "notebook.gotoSymbols.showAllSymbols": true,
     "python.analysis.autoImportCompletions": false,
     "python.analysis.inlayHints.pytestParameters": true,
@@ -58,12 +62,19 @@
     "python.testing.pytestEnabled": true,
     "python.testing.unittestEnabled": false,
     "redhat.telemetry.enabled": false,
     "rewrap.wrappingColumn": 88,
     "ruff.enable": true,
     "ruff.importStrategy": "fromEnvironment",
     "ruff.organizeImports": true,
+    "search.exclude": {
+        "**/tests/**/__init__.py": true,
+        ".constraints/*.txt": true,
+        "typings/**": true
+    },
     "telemetry.telemetryLevel": "off",
     "yaml.schemas": {
-        "https://json.schemastore.org/github-workflow.json": ".github/workflows/requirements.yml"
+        "https://raw.githubusercontent.com/ComPWA/qrules/0.10.x/src/qrules/particle-validation.json": [
+            "*particle*.y*ml"
+        ]
     }
 }
```

### Comparing `ampform-dpd-0.1.6/LICENSE` & `ampform_dpd-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ampform-dpd-0.1.6/PKG-INFO` & `ampform_dpd-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampform-dpd
-Version: 0.1.6
+Version: 0.1.7
 Summary: Symbolic expressions for Dalitz-Plot Decomposition
 Author-email: Common Partial Wave Analysis <compwa-admin@ep1.rub.de>
 License: GPLv3 or later
 Project-URL: Changelog, https://github.com/ComPWA/ampform-dpd/releases
 Project-URL: Documentation, https://compwa.github.io/ampform-dpd
 Project-URL: Source, https://github.com/ComPWA/ampform-dpd
 Project-URL: Tracker, https://github.com/ComPWA/ampform-dpd/issues
@@ -26,14 +26,15 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ampform>=0.14.8
 Requires-Dist: attrs>=20.1.0
 Requires-Dist: cloudpickle
+Requires-Dist: qrules>=0.10.0
 Requires-Dist: sympy>=1.10
 Requires-Dist: tensorwaves[jax]
 Provides-Extra: dev
 Requires-Dist: ampform-dpd[doc]; extra == "dev"
 Requires-Dist: ampform-dpd[jupyter]; extra == "dev"
 Requires-Dist: ampform-dpd[sty]; extra == "dev"
 Requires-Dist: ampform-dpd[test]; extra == "dev"
@@ -69,14 +70,15 @@
 Requires-Dist: jupyterlab-myst; extra == "jupyter"
 Requires-Dist: python-lsp-ruff; extra == "jupyter"
 Requires-Dist: python-lsp-server[rope]; extra == "jupyter"
 Provides-Extra: numba
 Requires-Dist: tensorwaves[numba]; extra == "numba"
 Provides-Extra: sty
 Requires-Dist: ampform-dpd[types]; extra == "sty"
+Requires-Dist: mypy; extra == "sty"
 Requires-Dist: pre-commit>=1.4.0; extra == "sty"
 Requires-Dist: ruff; extra == "sty"
 Provides-Extra: tensorflow
 Requires-Dist: ampform-dpd[tf]; extra == "tensorflow"
 Provides-Extra: test
 Requires-Dist: nbmake; extra == "test"
 Requires-Dist: numpy; extra == "test"
```

### Comparing `ampform-dpd-0.1.6/README.md` & `ampform_dpd-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ampform-dpd-0.1.6/codecov.yml` & `ampform_dpd-0.1.7/codecov.yml`

 * *Files identical despite different names*

### Comparing `ampform-dpd-0.1.6/docs/_static/favicon.ico` & `ampform_dpd-0.1.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `ampform-dpd-0.1.6/docs/comparison/d2kkk.ipynb` & `ampform_dpd-0.1.7/docs/comparison/d2kkk.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9826993847570311%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict([('tags', [])])}}, 1: {'source': {insert: [(4, "*

 * *            "'import warnings\\n'), (6, 'from typing import TYPE_CHECKING\\n'), (17, 'from "*

 * *            "IPython.display import Latex, Markdown, clear_output, display\\n'), (35, 'from "*

 * *            "ampform_dpd.adapter.qrules import normalize_state_ids, to_three_body_decay\\n'), (36, "*

 * *            "'from ampform_dpd.decay import Particle\\n'), (53, "*

 * *            '\'warnings.simplefilter("ignore")\\n\')], de […]*

```diff
@@ -1,12 +1,14 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
                 "# D\u2070 \u2192 K\u2070 K\u207a K\u207b\n",
                 "\n",
                 "```{autolink-concat}\n",
                 "```\n",
                 "\n",
                 "The decay $D^0 \\to K^0K^+K^-$ has a spinless initial and final state, which means that there is no need to align spin with Dalitz-plot decomposition. This notebook shows that the model formulated by {mod}`ampform` is the same as that formulated by {doc}`AmpForm-DPD</index>`. To simplify this comparison, we do not define any dynamics."
@@ -27,30 +29,30 @@
                     "scroll-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "from __future__ import annotations\n",
                 "\n",
-                "import itertools\n",
                 "import logging\n",
                 "import os\n",
+                "import warnings\n",
                 "from textwrap import dedent\n",
-                "from typing import TYPE_CHECKING, Iterable\n",
+                "from typing import TYPE_CHECKING\n",
                 "\n",
                 "import ampform\n",
                 "import graphviz\n",
                 "import ipywidgets\n",
                 "import jax.numpy as jnp\n",
                 "import matplotlib.pyplot as plt\n",
                 "import qrules\n",
                 "import sympy as sp\n",
                 "from ampform.kinematics.lorentz import FourMomentumSymbol, InvariantMass\n",
                 "from ampform.sympy import perform_cached_doit\n",
-                "from IPython.display import SVG, Latex, Markdown, clear_output, display\n",
+                "from IPython.display import Latex, Markdown, clear_output, display\n",
                 "from ipywidgets import (\n",
                 "    Accordion,\n",
                 "    Checkbox,\n",
                 "    GridBox,\n",
                 "    HBox,\n",
                 "    Layout,\n",
                 "    SelectMultiple,\n",
@@ -60,32 +62,33 @@
                 "    interactive_output,\n",
                 ")\n",
                 "from tensorwaves.data.phasespace import TFPhaseSpaceGenerator\n",
                 "from tensorwaves.data.rng import TFUniformRealNumberGenerator\n",
                 "from tensorwaves.data.transform import SympyDataTransformer\n",
                 "\n",
                 "from ampform_dpd import DalitzPlotDecompositionBuilder\n",
-                "from ampform_dpd.decay import IsobarNode, Particle, ThreeBodyDecay, ThreeBodyDecayChain\n",
+                "from ampform_dpd.adapter.qrules import normalize_state_ids, to_three_body_decay\n",
+                "from ampform_dpd.decay import Particle\n",
                 "from ampform_dpd.io import (\n",
                 "    as_markdown_table,\n",
                 "    aslatex,\n",
                 "    get_readable_hash,\n",
                 "    perform_cached_lambdify,\n",
                 "    simplify_latex_rendering,\n",
                 ")\n",
-                "from ampform_dpd.spin import filter_parity_violating_ls, generate_ls_couplings\n",
                 "\n",
                 "if TYPE_CHECKING:\n",
                 "    from ampform.helicity import HelicityModel\n",
                 "    from qrules.transition import ReactionInfo\n",
                 "    from tensorwaves.interface import DataSample, ParameterValue, ParametrizedFunction\n",
                 "\n",
                 "simplify_latex_rendering()\n",
                 "logging.getLogger(\"jax\").setLevel(logging.ERROR)  # mute JAX\n",
                 "os.environ[\"TF_CPP_MIN_LOG_LEVEL\"] = \"3\"  # mute TF\n",
+                "warnings.simplefilter(\"ignore\")\n",
                 "NO_TQDM = \"EXECUTE_NB\" in os.environ\n",
                 "if NO_TQDM:\n",
                 "    logging.getLogger(\"ampform.sympy\").setLevel(logging.ERROR)\n",
                 "    logging.getLogger(\"ampform_dpd.io\").setLevel(logging.ERROR)"
             ]
         },
         {
@@ -98,73 +101,50 @@
                 "## Decay definition"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "jupyter": {
-                    "source_hidden": true
-                },
                 "mystnb": {
-                    "code_prompt_show": "Define initial and final state"
+                    "code_prompt_show": "Generate transitions"
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "PDG = qrules.load_pdg()\n",
-                "PARTICLE_DB = {\n",
-                "    p.name: Particle(\n",
-                "        name=p.name,\n",
-                "        latex=p.latex,\n",
-                "        spin=p.spin,\n",
-                "        parity=int(p.parity),\n",
-                "        mass=p.mass,\n",
-                "        width=p.width,\n",
-                "    )\n",
-                "    for p in PDG\n",
-                "    if p.parity is not None\n",
-                "}\n",
-                "INITIAL_STATE = PARTICLE_DB[\"D0\"]\n",
-                "FS_zero = PARTICLE_DB[\"K0\"]\n",
-                "FS_neg = PARTICLE_DB[\"K-\"]\n",
-                "FS_pos = PARTICLE_DB[\"K+\"]\n",
-                "PARTICLE_TO_ID = {INITIAL_STATE: 0, FS_zero: 1, FS_neg: 2, FS_pos: 3}\n",
-                "_, *FINAL_STATE = PARTICLE_TO_ID\n",
-                "Markdown(as_markdown_table(list(PARTICLE_TO_ID)))"
+                "REACTION = qrules.generate_transitions(\n",
+                "    initial_state=\"D0\",\n",
+                "    final_state=[\"K0\", \"K-\", \"K+\"],\n",
+                "    allowed_intermediate_particles=[\"a(0)\", \"f(0)(980)\", \"pi(1)\"],\n",
+                "    mass_conservation_factor=0.2,\n",
+                "    formalism=\"helicity\",\n",
+                ")\n",
+                "REACTION123 = normalize_state_ids(REACTION)\n",
+                "dot = qrules.io.asdot(REACTION123, collapse_graphs=True)\n",
+                "graphviz.Source(dot)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
                     "source_hidden": true
                 },
-                "mystnb": {
-                    "code_prompt_show": "Generate transitions"
-                },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "reaction = qrules.generate_transitions(\n",
-                "    initial_state=INITIAL_STATE.name,\n",
-                "    final_state=[p.name for p in FINAL_STATE],\n",
-                "    allowed_intermediate_particles=[\"a(0)\", \"f(0)(980)\", \"pi(1)\"],\n",
-                "    mass_conservation_factor=0.2,\n",
-                "    formalism=\"helicity\",\n",
-                ")\n",
-                "dot = qrules.io.asdot(reaction, collapse_graphs=True)\n",
-                "graphviz.Source(dot)"
+                "DECAY = to_three_body_decay(REACTION123.transitions, min_ls=True)\n",
+                "Markdown(as_markdown_table([DECAY.initial_state, *DECAY.final_state.values()]))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -172,109 +152,35 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "qrules_resonances = sorted(\n",
-                "    reaction.get_intermediate_particles(),\n",
-                "    key=lambda p: (p.charge, p.mass, p.name),\n",
+                "resonances = sorted(\n",
+                "    {t.resonance for t in DECAY.chains},\n",
+                "    key=lambda p: (p.name[0], p.mass),\n",
                 ")\n",
-                "resonance_names = [p.name for p in qrules_resonances]\n",
-                "resonances = [PARTICLE_DB[name] for name in resonance_names]\n",
+                "resonance_names = [p.name for p in resonances]\n",
                 "Markdown(as_markdown_table(resonances))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
                     "source_hidden": true
                 },
                 "tags": [
-                    "hide-input",
-                    "scroll-input"
+                    "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "def load_three_body_decay(\n",
-                "    resonance_names: Iterable[str],\n",
-                "    particle_definitions: dict[str, Particle],\n",
-                "    min_ls: bool = True,\n",
-                ") -> ThreeBodyDecay:\n",
-                "    _resonances = [particle_definitions[name] for name in resonance_names]\n",
-                "    chains: list[ThreeBodyDecayChain] = []\n",
-                "    for res in _resonances:\n",
-                "        chains.extend(_create_isobar(res, min_ls))\n",
-                "    return ThreeBodyDecay(\n",
-                "        states={state_id: particle for particle, state_id in PARTICLE_TO_ID.items()},\n",
-                "        chains=tuple(chains),\n",
-                "    )\n",
-                "\n",
-                "\n",
-                "def _create_isobar(resonance: Particle, min_ls: bool) -> list[ThreeBodyDecayChain]:\n",
-                "    if resonance.name.endswith(\"-\"):\n",
-                "        child1, child2, spectator = FS_zero, FS_neg, FS_pos\n",
-                "    elif resonance.name.endswith(\"+\"):\n",
-                "        child1, child2, spectator = FS_pos, FS_zero, FS_neg\n",
-                "    else:\n",
-                "        child1, child2, spectator = FS_neg, FS_pos, FS_zero\n",
-                "    prod_ls_couplings = _generate_ls(\n",
-                "        INITIAL_STATE, resonance, spectator, conserve_parity=False\n",
-                "    )\n",
-                "    dec_ls_couplings = _generate_ls(resonance, child1, child2, conserve_parity=True)\n",
-                "    if min_ls:\n",
-                "        decay = IsobarNode(\n",
-                "            parent=INITIAL_STATE,\n",
-                "            child1=IsobarNode(\n",
-                "                parent=resonance,\n",
-                "                child1=child1,\n",
-                "                child2=child2,\n",
-                "                interaction=min(dec_ls_couplings),\n",
-                "            ),\n",
-                "            child2=spectator,\n",
-                "            interaction=min(prod_ls_couplings),\n",
-                "        )\n",
-                "        return [ThreeBodyDecayChain(decay)]\n",
-                "    chains = []\n",
-                "    for dec_ls, prod_ls in itertools.product(dec_ls_couplings, prod_ls_couplings):\n",
-                "        decay = IsobarNode(\n",
-                "            parent=INITIAL_STATE,\n",
-                "            child1=IsobarNode(\n",
-                "                parent=resonance,\n",
-                "                child1=child1,\n",
-                "                child2=child2,\n",
-                "                interaction=dec_ls,\n",
-                "            ),\n",
-                "            child2=spectator,\n",
-                "            interaction=prod_ls,\n",
-                "        )\n",
-                "        chains.append(ThreeBodyDecayChain(decay))\n",
-                "    return chains\n",
-                "\n",
-                "\n",
-                "def _generate_ls(\n",
-                "    parent: Particle, child1: Particle, child2: Particle, conserve_parity: bool\n",
-                ") -> list[tuple[int, sp.Rational]]:\n",
-                "    ls = generate_ls_couplings(parent.spin, child1.spin, child2.spin)\n",
-                "    if conserve_parity:\n",
-                "        return filter_parity_violating_ls(\n",
-                "            ls, parent.parity, child1.parity, child2.parity\n",
-                "        )\n",
-                "    return ls\n",
-                "\n",
-                "\n",
-                "DECAY = load_three_body_decay(\n",
-                "    resonance_names,\n",
-                "    particle_definitions=PARTICLE_DB,\n",
-                "    min_ls=True,\n",
-                ")\n",
                 "Latex(aslatex(DECAY, with_jp=True))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
@@ -291,38 +197,37 @@
             },
             "source": [
                 "### DPD model"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {
-                "jp-MarkdownHeadingCollapsed": true,
-                "tags": []
-            },
+            "metadata": {},
             "source": [
                 "Note that, as opposed to {ref}`\u039bc\u207a \u2192 p\u03c0\u207aK\u207b<lc2pkpi:Model formulation>` and {ref}`J/\u03c8 \u2192 K\u2070\u03a3\u207ap\u0305<jpsi2ksp:Model formulation>`, there are no Wigner-$d$ functions, because the final state is spinless."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
                     "source_hidden": true
                 },
                 "tags": [
+                    "full-width",
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "model_builder = DalitzPlotDecompositionBuilder(DECAY, min_ls=True)\n",
-                "dpd_model = model_builder.formulate(reference_subsystem=1)\n",
-                "dpd_model.intensity"
+                "DPD_MODEL = model_builder.formulate(reference_subsystem=1)\n",
+                "del model_builder\n",
+                "DPD_MODEL.intensity.cleanup()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -331,38 +236,24 @@
                 "tags": [
                     "hide-input",
                     "full-width"
                 ]
             },
             "outputs": [],
             "source": [
-                "Latex(aslatex(dpd_model.amplitudes))"
+                "Latex(aslatex(DPD_MODEL.amplitudes))"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "There is an isobar Wigner-$d$ function, which takes the following helicity angles as argument:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "metadata": {
-                "jupyter": {
-                    "source_hidden": true
-                },
-                "tags": [
-                    "hide-input"
-                ]
+                "tags": []
             },
-            "outputs": [],
             "source": [
-                "Latex(aslatex(dpd_model.variables))"
+                "There is an isobar Wigner-$d$ function, which takes the following helicity angles as argument:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -370,35 +261,32 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "masses = {\n",
-                "    sp.Symbol(f\"m{i}\", nonnegative=True): round(p.mass, 7)\n",
-                "    for p, i in PARTICLE_TO_ID.items()\n",
-                "}\n",
-                "dpd_model.parameter_defaults.update(masses)\n",
-                "Latex(aslatex(masses))"
+                "Latex(aslatex(DPD_MODEL.variables))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "jp-MarkdownHeadingCollapsed": true,
                 "tags": []
             },
             "source": [
                 "### AmpForm model"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
                 "AmpForm does not formulate alignment Wigner-$D$ functions. For the case of this spinless final state, this means the intensity is the same as that of the [](#dpd-model)."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -408,18 +296,20 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "model_builder = ampform.get_builder(reaction)\n",
+                "model_builder = ampform.get_builder(REACTION)\n",
                 "model_builder.use_helicity_couplings = False\n",
-                "ampform_model = model_builder.formulate()\n",
-                "ampform_model.intensity"
+                "model_builder.config.scalar_initial_state_mass = True\n",
+                "model_builder.config.stable_final_state_ids = [0, 1, 2]\n",
+                "AMPFORM_MODEL = model_builder.formulate()\n",
+                "AMPFORM_MODEL.intensity"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -428,15 +318,15 @@
                 "tags": [
                     "hide-input",
                     "full-width"
                 ]
             },
             "outputs": [],
             "source": [
-                "Latex(aslatex(ampform_model.amplitudes))"
+                "Latex(aslatex(AMPFORM_MODEL.amplitudes))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -444,15 +334,15 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "Latex(aslatex(ampform_model.kinematic_variables))"
+                "Latex(aslatex(AMPFORM_MODEL.kinematic_variables))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "jp-MarkdownHeadingCollapsed": true,
                 "tags": []
@@ -461,44 +351,45 @@
                 "## Phase space sample"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
+                "jupyter": {
+                    "source_hidden": true
+                },
                 "mystnb": {
                     "code_prompt_show": "Formulate kinematic variables in terms of four-momenta"
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "p1, p2, p3 = tuple(FourMomentumSymbol(f\"p{i}\", shape=[]) for i in (0, 1, 2))\n",
-                "s1, s2, s3 = sp.symbols(\"sigma1:4\", nonnegative=True)\n",
+                "s1, s2, s3 = sorted(DPD_MODEL.invariants, key=str)\n",
                 "mass_definitions = {\n",
+                "    **DPD_MODEL.masses,\n",
                 "    s1: InvariantMass(p2 + p3) ** 2,\n",
                 "    s2: InvariantMass(p1 + p3) ** 2,\n",
                 "    s3: InvariantMass(p1 + p2) ** 2,\n",
                 "    sp.Symbol(\"m_01\", nonnegative=True): InvariantMass(p1 + p2),\n",
                 "    sp.Symbol(\"m_02\", nonnegative=True): InvariantMass(p1 + p3),\n",
                 "    sp.Symbol(\"m_12\", nonnegative=True): InvariantMass(p2 + p3),\n",
                 "}\n",
                 "dpd_variables = {\n",
-                "    sp.Symbol(f\"m{i}\", nonnegative=True): sp.Float(p.mass)\n",
-                "    for i, p in enumerate(PARTICLE_TO_ID)\n",
+                "    symbol: expr.doit().xreplace(DPD_MODEL.variables).xreplace(mass_definitions)\n",
+                "    for symbol, expr in DPD_MODEL.variables.items()\n",
                 "}\n",
-                "for symbol, expr in dpd_model.variables.items():\n",
-                "    expr = expr.doit().xreplace(mass_definitions).xreplace(dpd_variables)\n",
-                "    dpd_variables[symbol] = expr\n",
                 "dpd_transformer = SympyDataTransformer.from_sympy(dpd_variables, backend=\"jax\")\n",
                 "\n",
                 "ampform_transformer = SympyDataTransformer.from_sympy(\n",
-                "    ampform_model.kinematic_variables, backend=\"jax\"\n",
+                "    AMPFORM_MODEL.kinematic_variables, backend=\"jax\"\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -511,15 +402,15 @@
                 "    phsp_generator = TFPhaseSpaceGenerator(\n",
                 "        initial_state_mass=reaction.initial_state[-1].mass,\n",
                 "        final_state_masses={i: p.mass for i, p in reaction.final_state.items()},\n",
                 "    )\n",
                 "    return phsp_generator.generate(size, rng)\n",
                 "\n",
                 "\n",
-                "phsp = generate_phase_space(ampform_model.reaction_info, size=100_000)\n",
+                "phsp = generate_phase_space(AMPFORM_MODEL.reaction_info, size=100_000)\n",
                 "ampform_phsp = ampform_transformer(phsp)\n",
                 "dpd_phsp = dpd_transformer(phsp)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -542,33 +433,33 @@
                 "    unfolded_intensity = perform_cached_doit(model.intensity)\n",
                 "    unfolded_amplitudes = {\n",
                 "        symbol: perform_cached_doit(expr) for symbol, expr in model.amplitudes.items()\n",
                 "    }\n",
                 "    return unfolded_intensity.xreplace(unfolded_amplitudes)\n",
                 "\n",
                 "\n",
-                "ampform_intensity_expr = unfold_intensity(ampform_model)\n",
-                "dpd_intensity_expr = unfold_intensity(dpd_model)"
+                "ampform_intensity_expr = unfold_intensity(AMPFORM_MODEL)\n",
+                "dpd_intensity_expr = unfold_intensity(DPD_MODEL)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "ampform_func = perform_cached_lambdify(\n",
                 "    ampform_intensity_expr,\n",
-                "    parameters=ampform_model.parameter_defaults,\n",
+                "    parameters=AMPFORM_MODEL.parameter_defaults,\n",
                 ")\n",
                 "dpd_func = perform_cached_lambdify(\n",
                 "    dpd_intensity_expr,\n",
-                "    parameters=dpd_model.parameter_defaults,\n",
+                "    parameters=DPD_MODEL.parameter_defaults,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -634,16 +525,16 @@
                     "hide-input",
                     "scroll-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "def create_sliders() -> dict[str, ToggleButtons]:\n",
-                "    all_parameters = dict(ampform_model.parameter_defaults.items())\n",
-                "    all_parameters.update(dpd_model.parameter_defaults)\n",
+                "    all_parameters = dict(AMPFORM_MODEL.parameter_defaults.items())\n",
+                "    all_parameters.update(DPD_MODEL.parameter_defaults)\n",
                 "    sliders = {}\n",
                 "    for symbol, value in all_parameters.items():\n",
                 "        value = \"+1\"\n",
                 "        if (\n",
                 "            symbol.name.startswith(R\"\\mathcal{H}^\\mathrm{decay}\") and \"+\" in symbol.name\n",
                 "        ) and any(s in symbol.name for s in [\"{1}\", \"*\", \"rho\"]):\n",
                 "            value = \"-1\"\n",
@@ -720,14 +611,15 @@
                 "jupyter": {
                     "source_hidden": true
                 },
                 "mystnb": {
                     "code_prompt_show": "Generate comparison widget"
                 },
                 "tags": [
+                    "full-width",
                     "hide-input",
                     "scroll-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
@@ -736,25 +628,26 @@
                 "fig.canvas.toolbar_visible = False\n",
                 "fig.canvas.header_visible = False\n",
                 "fig.canvas.footer_visible = False\n",
                 "(\n",
                 "    (ax_s1, ax_s2, ax_s3),\n",
                 "    (ax_t1, ax_t2, ax_t3),\n",
                 ") = axes\n",
-                "final_state = ampform_model.reaction_info.final_state\n",
                 "for ax in axes[:, 0].flatten():\n",
                 "    ax.set_ylabel(\"Intensity (a.u.)\")\n",
                 "for ax in axes[:, 1:].flatten():\n",
                 "    ax.set_yticks([])\n",
-                "ax_s1.set_xlabel(f\"$m({FINAL_STATE[1].latex}, {FINAL_STATE[2].latex})$\")\n",
-                "ax_s2.set_xlabel(f\"$m({FINAL_STATE[0].latex}, {FINAL_STATE[2].latex})$\")\n",
-                "ax_s3.set_xlabel(f\"$m({FINAL_STATE[0].latex}, {FINAL_STATE[1].latex})$\")\n",
-                "ax_t1.set_xlabel(Rf\"$\\theta({FINAL_STATE[1].latex}, {FINAL_STATE[2].latex})$\")\n",
-                "ax_t2.set_xlabel(Rf\"$\\theta({FINAL_STATE[0].latex}, {FINAL_STATE[2].latex})$\")\n",
-                "ax_t3.set_xlabel(Rf\"$\\theta({FINAL_STATE[0].latex}, {FINAL_STATE[1].latex})$\")\n",
+                "\n",
+                "final_state = DECAY.final_state\n",
+                "ax_s1.set_xlabel(f\"$m({final_state[2].latex}, {final_state[3].latex})$\")\n",
+                "ax_s2.set_xlabel(f\"$m({final_state[1].latex}, {final_state[3].latex})$\")\n",
+                "ax_s3.set_xlabel(f\"$m({final_state[1].latex}, {final_state[2].latex})$\")\n",
+                "ax_t1.set_xlabel(Rf\"$\\theta({final_state[2].latex}, {final_state[3].latex})$\")\n",
+                "ax_t2.set_xlabel(Rf\"$\\theta({final_state[1].latex}, {final_state[3].latex})$\")\n",
+                "ax_t3.set_xlabel(Rf\"$\\theta({final_state[1].latex}, {final_state[2].latex})$\")\n",
                 "fig.suptitle(f'Selected resonances: ${\", \".join(resonance_selector.value)}$')\n",
                 "fig.tight_layout()\n",
                 "\n",
                 "lines = None\n",
                 "\n",
                 "__EXPRS: dict[int, sp.Expr] = {}\n",
                 "\n",
@@ -941,21 +834,21 @@
                 "    if hide_expressions.value:\n",
                 "        clear_output()\n",
                 "    else:\n",
                 "        if simplify_expressions.value:\n",
                 "            ampform_expr = _simplify(\n",
                 "                ampform_intensity_expr,\n",
                 "                ampform_pars,\n",
-                "                ampform_model.kinematic_variables,\n",
+                "                AMPFORM_MODEL.kinematic_variables,\n",
                 "                selected_resonances,\n",
                 "            )\n",
                 "            dpd_expr = _simplify(\n",
                 "                dpd_intensity_expr,\n",
                 "                dpd_pars,\n",
-                "                dpd_model.variables,\n",
+                "                DPD_MODEL.variables,\n",
                 "                selected_resonances,\n",
                 "            )\n",
                 "        else:\n",
                 "            ampform_expr = ampform_intensity_expr\n",
                 "            dpd_expr = dpd_intensity_expr\n",
                 "        src = Rf\"\"\"\n",
                 "        \\begin{{eqnarray}}\n",
@@ -974,34 +867,14 @@
                 "        \"resonance_selector\": resonance_selector,\n",
                 "        \"hide_expressions\": hide_expressions,\n",
                 "        \"simplify_expressions\": simplify_expressions,\n",
                 "    },\n",
                 ")\n",
                 "display(output, ui)"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "jupyter": {
-                    "source_hidden": true
-                },
-                "tags": [
-                    "remove-input",
-                    "full-width"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "if NO_TQDM:\n",
-                "    filename = \"d02kkk-comparison.svg\"\n",
-                "    plt.savefig(filename)\n",
-                "    display(SVG(filename))"
-            ]
         }
     ],
     "metadata": {
         "colab": {
             "toc_visible": true
         },
         "kernelspec": {
@@ -1015,13 +888,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.17"
+            "version": "3.9.19"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `ampform-dpd-0.1.6/docs/comparison/jpsi2phipipi.ipynb` & `ampform_dpd-0.1.7/docs/comparison/jpsi2phipipi.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9830458938174984%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict([('tags', [])])}}, 1: {'source': {insert: [(4, "*

 * *            "'import warnings\\n'), (6, 'from typing import TYPE_CHECKING\\n'), (17, 'from "*

 * *            "IPython.display import Latex, Markdown, clear_output, display\\n'), (35, 'from "*

 * *            "ampform_dpd.adapter.qrules import normalize_state_ids, to_three_body_decay\\n'), (36, "*

 * *            "'from ampform_dpd.decay import Particle\\n'), (53, "*

 * *            '\'warnings.simplefilter("ignore")\\n\')], de […]*

```diff
@@ -1,12 +1,14 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
                 "# J/\u03c8 \u2192 \u03c6(1020) \u03c0\u207a \u03c0\u207b\n",
                 "\n",
                 "```{autolink-concat}\n",
                 "```\n",
                 "\n",
                 "The decay $J/\\psi \\to \\phi(1020) \\pi^+ \\pi^-$ has an initial state with spin and has one vector meson, $\\phi(1020)$, in the final state. This is a follow-up to {doc}`jpsi2pipipi`, where there is no spin in the final state."
@@ -27,30 +29,30 @@
                     "scroll-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "from __future__ import annotations\n",
                 "\n",
-                "import itertools\n",
                 "import logging\n",
                 "import os\n",
+                "import warnings\n",
                 "from textwrap import dedent\n",
-                "from typing import TYPE_CHECKING, Iterable\n",
+                "from typing import TYPE_CHECKING\n",
                 "\n",
                 "import ampform\n",
                 "import graphviz\n",
                 "import ipywidgets\n",
                 "import jax.numpy as jnp\n",
                 "import matplotlib.pyplot as plt\n",
                 "import qrules\n",
                 "import sympy as sp\n",
                 "from ampform.kinematics.lorentz import FourMomentumSymbol, InvariantMass\n",
                 "from ampform.sympy import perform_cached_doit\n",
-                "from IPython.display import SVG, Latex, Markdown, clear_output, display\n",
+                "from IPython.display import Latex, Markdown, clear_output, display\n",
                 "from ipywidgets import (\n",
                 "    Accordion,\n",
                 "    Checkbox,\n",
                 "    GridBox,\n",
                 "    HBox,\n",
                 "    Layout,\n",
                 "    SelectMultiple,\n",
@@ -60,32 +62,33 @@
                 "    interactive_output,\n",
                 ")\n",
                 "from tensorwaves.data.phasespace import TFPhaseSpaceGenerator\n",
                 "from tensorwaves.data.rng import TFUniformRealNumberGenerator\n",
                 "from tensorwaves.data.transform import SympyDataTransformer\n",
                 "\n",
                 "from ampform_dpd import DalitzPlotDecompositionBuilder\n",
-                "from ampform_dpd.decay import IsobarNode, Particle, ThreeBodyDecay, ThreeBodyDecayChain\n",
+                "from ampform_dpd.adapter.qrules import normalize_state_ids, to_three_body_decay\n",
+                "from ampform_dpd.decay import Particle\n",
                 "from ampform_dpd.io import (\n",
                 "    as_markdown_table,\n",
                 "    aslatex,\n",
                 "    get_readable_hash,\n",
                 "    perform_cached_lambdify,\n",
                 "    simplify_latex_rendering,\n",
                 ")\n",
-                "from ampform_dpd.spin import filter_parity_violating_ls, generate_ls_couplings\n",
                 "\n",
                 "if TYPE_CHECKING:\n",
                 "    from ampform.helicity import HelicityModel\n",
                 "    from qrules.transition import ReactionInfo\n",
                 "    from tensorwaves.interface import DataSample, ParameterValue, ParametrizedFunction\n",
                 "\n",
                 "simplify_latex_rendering()\n",
                 "logging.getLogger(\"jax\").setLevel(logging.ERROR)  # mute JAX\n",
                 "os.environ[\"TF_CPP_MIN_LOG_LEVEL\"] = \"3\"  # mute TF\n",
+                "warnings.simplefilter(\"ignore\")\n",
                 "NO_TQDM = \"EXECUTE_NB\" in os.environ\n",
                 "if NO_TQDM:\n",
                 "    logging.getLogger(\"ampform.sympy\").setLevel(logging.ERROR)\n",
                 "    logging.getLogger(\"ampform_dpd.io\").setLevel(logging.ERROR)"
             ]
         },
         {
@@ -98,73 +101,50 @@
                 "## Decay definition"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "jupyter": {
-                    "source_hidden": true
-                },
                 "mystnb": {
-                    "code_prompt_show": "Define initial and final state"
+                    "code_prompt_show": "Generate transitions"
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "PDG = qrules.load_pdg()\n",
-                "PARTICLE_DB = {\n",
-                "    p.name: Particle(\n",
-                "        name=p.name,\n",
-                "        latex=p.latex,\n",
-                "        spin=p.spin,\n",
-                "        parity=int(p.parity),\n",
-                "        mass=p.mass,\n",
-                "        width=p.width,\n",
-                "    )\n",
-                "    for p in PDG\n",
-                "    if p.parity is not None\n",
-                "}\n",
-                "INITIAL_STATE = PARTICLE_DB[\"J/psi(1S)\"]\n",
-                "FS_zero = PARTICLE_DB[\"phi(1020)\"]\n",
-                "FS_neg = PARTICLE_DB[\"pi-\"]\n",
-                "FS_pos = PARTICLE_DB[\"pi+\"]\n",
-                "PARTICLE_TO_ID = {INITIAL_STATE: 0, FS_zero: 1, FS_neg: 2, FS_pos: 3}\n",
-                "_, *FINAL_STATE = PARTICLE_TO_ID\n",
-                "Markdown(as_markdown_table(list(PARTICLE_TO_ID)))"
+                "REACTION = qrules.generate_transitions(\n",
+                "    initial_state=\"J/psi(1S)\",\n",
+                "    final_state=[\"phi(1020)\", \"pi-\", \"pi+\"],\n",
+                "    allowed_intermediate_particles=[\"a(0)(1450\", \"rho(1450)\"],\n",
+                "    mass_conservation_factor=0,\n",
+                "    formalism=\"helicity\",\n",
+                ")\n",
+                "REACTION123 = normalize_state_ids(REACTION)\n",
+                "dot = qrules.io.asdot(REACTION123, collapse_graphs=True)\n",
+                "graphviz.Source(dot)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
                     "source_hidden": true
                 },
-                "mystnb": {
-                    "code_prompt_show": "Generate transitions"
-                },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "reaction = qrules.generate_transitions(\n",
-                "    initial_state=INITIAL_STATE.name,\n",
-                "    final_state=[p.name for p in FINAL_STATE],\n",
-                "    allowed_intermediate_particles=[\"a(0)(1450\", \"rho(1450)\"],\n",
-                "    mass_conservation_factor=0,\n",
-                "    formalism=\"helicity\",\n",
-                ")\n",
-                "dot = qrules.io.asdot(reaction, collapse_graphs=True)\n",
-                "graphviz.Source(dot)"
+                "DECAY = to_three_body_decay(REACTION123.transitions, min_ls=True)\n",
+                "Markdown(as_markdown_table([DECAY.initial_state, *DECAY.final_state.values()]))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -172,109 +152,35 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "qrules_resonances = sorted(\n",
-                "    reaction.get_intermediate_particles(),\n",
-                "    key=lambda p: (p.charge, p.mass, p.name),\n",
+                "resonances = sorted(\n",
+                "    {t.resonance for t in DECAY.chains},\n",
+                "    key=lambda p: (p.name[0], p.mass),\n",
                 ")\n",
-                "resonance_names = [p.name for p in qrules_resonances]\n",
-                "resonances = [PARTICLE_DB[name] for name in resonance_names]\n",
+                "resonance_names = [p.name for p in resonances]\n",
                 "Markdown(as_markdown_table(resonances))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
                     "source_hidden": true
                 },
                 "tags": [
-                    "hide-input",
-                    "scroll-input"
+                    "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "def load_three_body_decay(\n",
-                "    resonance_names: Iterable[str],\n",
-                "    particle_definitions: dict[str, Particle],\n",
-                "    min_ls: bool = True,\n",
-                ") -> ThreeBodyDecay:\n",
-                "    _resonances = [particle_definitions[name] for name in resonance_names]\n",
-                "    chains: list[ThreeBodyDecayChain] = []\n",
-                "    for res in _resonances:\n",
-                "        chains.extend(_create_isobar(res, min_ls))\n",
-                "    return ThreeBodyDecay(\n",
-                "        states={state_id: particle for particle, state_id in PARTICLE_TO_ID.items()},\n",
-                "        chains=tuple(chains),\n",
-                "    )\n",
-                "\n",
-                "\n",
-                "def _create_isobar(resonance: Particle, min_ls: bool) -> list[ThreeBodyDecayChain]:\n",
-                "    if resonance.name.endswith(\"-\"):\n",
-                "        child1, child2, spectator = FS_zero, FS_neg, FS_pos\n",
-                "    elif resonance.name.endswith(\"+\"):\n",
-                "        child1, child2, spectator = FS_pos, FS_zero, FS_neg\n",
-                "    else:\n",
-                "        child1, child2, spectator = FS_neg, FS_pos, FS_zero\n",
-                "    prod_ls_couplings = _generate_ls(\n",
-                "        INITIAL_STATE, resonance, spectator, conserve_parity=False\n",
-                "    )\n",
-                "    dec_ls_couplings = _generate_ls(resonance, child1, child2, conserve_parity=False)\n",
-                "    if min_ls:\n",
-                "        decay = IsobarNode(\n",
-                "            parent=INITIAL_STATE,\n",
-                "            child1=IsobarNode(\n",
-                "                parent=resonance,\n",
-                "                child1=child1,\n",
-                "                child2=child2,\n",
-                "                interaction=min(dec_ls_couplings),\n",
-                "            ),\n",
-                "            child2=spectator,\n",
-                "            interaction=min(prod_ls_couplings),\n",
-                "        )\n",
-                "        return [ThreeBodyDecayChain(decay)]\n",
-                "    chains = []\n",
-                "    for dec_ls, prod_ls in itertools.product(dec_ls_couplings, prod_ls_couplings):\n",
-                "        decay = IsobarNode(\n",
-                "            parent=INITIAL_STATE,\n",
-                "            child1=IsobarNode(\n",
-                "                parent=resonance,\n",
-                "                child1=child1,\n",
-                "                child2=child2,\n",
-                "                interaction=dec_ls,\n",
-                "            ),\n",
-                "            child2=spectator,\n",
-                "            interaction=prod_ls,\n",
-                "        )\n",
-                "        chains.append(ThreeBodyDecayChain(decay))\n",
-                "    return chains\n",
-                "\n",
-                "\n",
-                "def _generate_ls(\n",
-                "    parent: Particle, child1: Particle, child2: Particle, conserve_parity: bool\n",
-                ") -> list[tuple[int, sp.Rational]]:\n",
-                "    ls = generate_ls_couplings(parent.spin, child1.spin, child2.spin)\n",
-                "    if conserve_parity:\n",
-                "        return filter_parity_violating_ls(\n",
-                "            ls, parent.parity, child1.parity, child2.parity\n",
-                "        )\n",
-                "    return ls\n",
-                "\n",
-                "\n",
-                "DECAY = load_three_body_decay(\n",
-                "    resonance_names,\n",
-                "    particle_definitions=PARTICLE_DB,\n",
-                "    min_ls=True,\n",
-                ")\n",
                 "Latex(aslatex(DECAY, with_jp=True))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
@@ -297,22 +203,24 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
                     "source_hidden": true
                 },
                 "tags": [
+                    "full-width",
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "model_builder = DalitzPlotDecompositionBuilder(DECAY, min_ls=True)\n",
-                "dpd_model = model_builder.formulate(reference_subsystem=1)\n",
-                "dpd_model.intensity"
+                "DPD_MODEL = model_builder.formulate(reference_subsystem=1)\n",
+                "del model_builder\n",
+                "DPD_MODEL.intensity.cleanup()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -321,38 +229,24 @@
                 "tags": [
                     "hide-input",
                     "full-width"
                 ]
             },
             "outputs": [],
             "source": [
-                "Latex(aslatex(dpd_model.amplitudes))"
+                "Latex(aslatex(DPD_MODEL.amplitudes))"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "There is an isobar Wigner-$d$ function, which takes the following helicity angles as argument:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "metadata": {
-                "jupyter": {
-                    "source_hidden": true
-                },
-                "tags": [
-                    "hide-input"
-                ]
+                "tags": []
             },
-            "outputs": [],
             "source": [
-                "Latex(aslatex(dpd_model.variables))"
+                "There is an isobar Wigner-$d$ function, which takes the following helicity angles as argument:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -360,20 +254,15 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "masses = {\n",
-                "    sp.Symbol(f\"m{i}\", nonnegative=True): round(p.mass, 7)\n",
-                "    for p, i in PARTICLE_TO_ID.items()\n",
-                "}\n",
-                "dpd_model.parameter_defaults.update(masses)\n",
-                "Latex(aslatex(masses))"
+                "Latex(aslatex(DPD_MODEL.variables))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "jp-MarkdownHeadingCollapsed": true,
                 "tags": []
@@ -391,18 +280,20 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "model_builder = ampform.get_builder(reaction)\n",
+                "model_builder = ampform.get_builder(REACTION)\n",
                 "model_builder.use_helicity_couplings = False\n",
-                "ampform_model = model_builder.formulate()\n",
-                "ampform_model.intensity"
+                "model_builder.config.scalar_initial_state_mass = True\n",
+                "model_builder.config.stable_final_state_ids = [0, 1, 2]\n",
+                "AMPFORM_MODEL = model_builder.formulate()\n",
+                "AMPFORM_MODEL.intensity"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -411,15 +302,15 @@
                 "tags": [
                     "hide-input",
                     "full-width"
                 ]
             },
             "outputs": [],
             "source": [
-                "Latex(aslatex(ampform_model.amplitudes))"
+                "Latex(aslatex(AMPFORM_MODEL.amplitudes))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -427,15 +318,15 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "Latex(aslatex(ampform_model.kinematic_variables))"
+                "Latex(aslatex(AMPFORM_MODEL.kinematic_variables))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "jp-MarkdownHeadingCollapsed": true,
                 "tags": []
@@ -444,44 +335,45 @@
                 "## Phase space sample"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
+                "jupyter": {
+                    "source_hidden": true
+                },
                 "mystnb": {
                     "code_prompt_show": "Formulate kinematic variables in terms of four-momenta"
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "p1, p2, p3 = tuple(FourMomentumSymbol(f\"p{i}\", shape=[]) for i in (0, 1, 2))\n",
-                "s1, s2, s3 = sp.symbols(\"sigma1:4\", nonnegative=True)\n",
+                "s1, s2, s3 = sorted(DPD_MODEL.invariants, key=str)\n",
                 "mass_definitions = {\n",
+                "    **DPD_MODEL.masses,\n",
                 "    s1: InvariantMass(p2 + p3) ** 2,\n",
                 "    s2: InvariantMass(p1 + p3) ** 2,\n",
                 "    s3: InvariantMass(p1 + p2) ** 2,\n",
                 "    sp.Symbol(\"m_01\", nonnegative=True): InvariantMass(p1 + p2),\n",
                 "    sp.Symbol(\"m_02\", nonnegative=True): InvariantMass(p1 + p3),\n",
                 "    sp.Symbol(\"m_12\", nonnegative=True): InvariantMass(p2 + p3),\n",
                 "}\n",
                 "dpd_variables = {\n",
-                "    sp.Symbol(f\"m{i}\", nonnegative=True): sp.Float(p.mass)\n",
-                "    for i, p in enumerate(PARTICLE_TO_ID)\n",
+                "    symbol: expr.doit().xreplace(DPD_MODEL.variables).xreplace(mass_definitions)\n",
+                "    for symbol, expr in DPD_MODEL.variables.items()\n",
                 "}\n",
-                "for symbol, expr in dpd_model.variables.items():\n",
-                "    expr = expr.doit().xreplace(mass_definitions).xreplace(dpd_variables)\n",
-                "    dpd_variables[symbol] = expr\n",
                 "dpd_transformer = SympyDataTransformer.from_sympy(dpd_variables, backend=\"jax\")\n",
                 "\n",
                 "ampform_transformer = SympyDataTransformer.from_sympy(\n",
-                "    ampform_model.kinematic_variables, backend=\"jax\"\n",
+                "    AMPFORM_MODEL.kinematic_variables, backend=\"jax\"\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -494,15 +386,15 @@
                 "    phsp_generator = TFPhaseSpaceGenerator(\n",
                 "        initial_state_mass=reaction.initial_state[-1].mass,\n",
                 "        final_state_masses={i: p.mass for i, p in reaction.final_state.items()},\n",
                 "    )\n",
                 "    return phsp_generator.generate(size, rng)\n",
                 "\n",
                 "\n",
-                "phsp = generate_phase_space(ampform_model.reaction_info, size=100_000)\n",
+                "phsp = generate_phase_space(AMPFORM_MODEL.reaction_info, size=100_000)\n",
                 "ampform_phsp = ampform_transformer(phsp)\n",
                 "dpd_phsp = dpd_transformer(phsp)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -525,33 +417,33 @@
                 "    unfolded_intensity = perform_cached_doit(model.intensity)\n",
                 "    unfolded_amplitudes = {\n",
                 "        symbol: perform_cached_doit(expr) for symbol, expr in model.amplitudes.items()\n",
                 "    }\n",
                 "    return unfolded_intensity.xreplace(unfolded_amplitudes)\n",
                 "\n",
                 "\n",
-                "ampform_intensity_expr = unfold_intensity(ampform_model)\n",
-                "dpd_intensity_expr = unfold_intensity(dpd_model)"
+                "ampform_intensity_expr = unfold_intensity(AMPFORM_MODEL)\n",
+                "dpd_intensity_expr = unfold_intensity(DPD_MODEL)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "ampform_func = perform_cached_lambdify(\n",
                 "    ampform_intensity_expr,\n",
-                "    parameters=ampform_model.parameter_defaults,\n",
+                "    parameters=AMPFORM_MODEL.parameter_defaults,\n",
                 ")\n",
                 "dpd_func = perform_cached_lambdify(\n",
                 "    dpd_intensity_expr,\n",
-                "    parameters=dpd_model.parameter_defaults,\n",
+                "    parameters=DPD_MODEL.parameter_defaults,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -617,16 +509,16 @@
                     "hide-input",
                     "scroll-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "def create_sliders() -> dict[str, ToggleButtons]:\n",
-                "    all_parameters = dict(ampform_model.parameter_defaults.items())\n",
-                "    all_parameters.update(dpd_model.parameter_defaults)\n",
+                "    all_parameters = dict(AMPFORM_MODEL.parameter_defaults.items())\n",
+                "    all_parameters.update(DPD_MODEL.parameter_defaults)\n",
                 "    sliders = {}\n",
                 "    for symbol, value in all_parameters.items():\n",
                 "        value = \"+1\"\n",
                 "        if (\n",
                 "            symbol.name.startswith(R\"\\mathcal{H}^\\mathrm{decay}\") and \"+\" in symbol.name\n",
                 "        ) and any(s in symbol.name for s in [\"{1}\", \"*\", \"rho\"]):\n",
                 "            value = \"-1\"\n",
@@ -703,14 +595,15 @@
                 "jupyter": {
                     "source_hidden": true
                 },
                 "mystnb": {
                     "code_prompt_show": "Generate comparison widget"
                 },
                 "tags": [
+                    "full-width",
                     "hide-input",
                     "scroll-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
@@ -719,25 +612,26 @@
                 "fig.canvas.toolbar_visible = False\n",
                 "fig.canvas.header_visible = False\n",
                 "fig.canvas.footer_visible = False\n",
                 "(\n",
                 "    (ax_s1, ax_s2, ax_s3),\n",
                 "    (ax_t1, ax_t2, ax_t3),\n",
                 ") = axes\n",
-                "final_state = ampform_model.reaction_info.final_state\n",
                 "for ax in axes[:, 0].flatten():\n",
                 "    ax.set_ylabel(\"Intensity (a.u.)\")\n",
                 "for ax in axes[:, 1:].flatten():\n",
                 "    ax.set_yticks([])\n",
-                "ax_s1.set_xlabel(f\"$m({FINAL_STATE[1].latex}, {FINAL_STATE[2].latex})$\")\n",
-                "ax_s2.set_xlabel(f\"$m({FINAL_STATE[0].latex}, {FINAL_STATE[2].latex})$\")\n",
-                "ax_s3.set_xlabel(f\"$m({FINAL_STATE[0].latex}, {FINAL_STATE[1].latex})$\")\n",
-                "ax_t1.set_xlabel(Rf\"$\\theta({FINAL_STATE[1].latex}, {FINAL_STATE[2].latex})$\")\n",
-                "ax_t2.set_xlabel(Rf\"$\\theta({FINAL_STATE[0].latex}, {FINAL_STATE[2].latex})$\")\n",
-                "ax_t3.set_xlabel(Rf\"$\\theta({FINAL_STATE[0].latex}, {FINAL_STATE[1].latex})$\")\n",
+                "\n",
+                "final_state = DECAY.final_state\n",
+                "ax_s1.set_xlabel(f\"$m({final_state[2].latex}, {final_state[3].latex})$\")\n",
+                "ax_s2.set_xlabel(f\"$m({final_state[1].latex}, {final_state[3].latex})$\")\n",
+                "ax_s3.set_xlabel(f\"$m({final_state[1].latex}, {final_state[2].latex})$\")\n",
+                "ax_t1.set_xlabel(Rf\"$\\theta({final_state[2].latex}, {final_state[3].latex})$\")\n",
+                "ax_t2.set_xlabel(Rf\"$\\theta({final_state[1].latex}, {final_state[3].latex})$\")\n",
+                "ax_t3.set_xlabel(Rf\"$\\theta({final_state[1].latex}, {final_state[2].latex})$\")\n",
                 "fig.suptitle(f'Selected resonances: ${\", \".join(resonance_selector.value)}$')\n",
                 "fig.tight_layout()\n",
                 "\n",
                 "lines = None\n",
                 "\n",
                 "__EXPRS: dict[int, sp.Expr] = {}\n",
                 "\n",
@@ -926,21 +820,21 @@
                 "    if hide_expressions.value:\n",
                 "        clear_output()\n",
                 "    else:\n",
                 "        if simplify_expressions.value:\n",
                 "            ampform_expr = _simplify(\n",
                 "                ampform_intensity_expr,\n",
                 "                ampform_pars,\n",
-                "                ampform_model.kinematic_variables,\n",
+                "                AMPFORM_MODEL.kinematic_variables,\n",
                 "                selected_resonances,\n",
                 "            )\n",
                 "            dpd_expr = _simplify(\n",
                 "                dpd_intensity_expr,\n",
                 "                dpd_pars,\n",
-                "                dpd_model.variables,\n",
+                "                DPD_MODEL.variables,\n",
                 "                selected_resonances,\n",
                 "            )\n",
                 "        else:\n",
                 "            ampform_expr = ampform_intensity_expr\n",
                 "            dpd_expr = dpd_intensity_expr\n",
                 "        src = Rf\"\"\"\n",
                 "        \\begin{{eqnarray}}\n",
@@ -959,34 +853,14 @@
                 "        \"resonance_selector\": resonance_selector,\n",
                 "        \"hide_expressions\": hide_expressions,\n",
                 "        \"simplify_expressions\": simplify_expressions,\n",
                 "    },\n",
                 ")\n",
                 "display(output, ui)"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "jupyter": {
-                    "source_hidden": true
-                },
-                "tags": [
-                    "remove-input",
-                    "full-width"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "if NO_TQDM:\n",
-                "    filename = \"jpsi2phipipi-comparison.svg\"\n",
-                "    plt.savefig(filename)\n",
-                "    display(SVG(filename))"
-            ]
         }
     ],
     "metadata": {
         "colab": {
             "toc_visible": true
         },
         "kernelspec": {
@@ -1000,13 +874,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.17"
+            "version": "3.9.19"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `ampform-dpd-0.1.6/docs/comparison/jpsi2pipipi.ipynb` & `ampform_dpd-0.1.7/docs/comparison/jpsi2pipipi.ipynb`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9830456477452008%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict([('tags', [])])}}, 1: {'source': {insert: [(4, "*

 * *            "'import warnings\\n'), (6, 'from typing import TYPE_CHECKING\\n'), (17, 'from "*

 * *            "IPython.display import Latex, Markdown, clear_output, display\\n'), (35, 'from "*

 * *            "ampform_dpd.adapter.qrules import normalize_state_ids, to_three_body_decay\\n'), (36, "*

 * *            "'from ampform_dpd.decay import Particle\\n'), (53, "*

 * *            '\'warnings.simplefilter("ignore")\\n\')], de […]*

```diff
@@ -1,12 +1,14 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
                 "# J/\u03c8 \u2192 \u03c0\u2070 \u03c0\u207a \u03c0\u207b\n",
                 "\n",
                 "```{autolink-concat}\n",
                 "```\n",
                 "\n",
                 "The decay $J/\\psi \\to \\pi^0 \\pi^+ \\pi^-$ has an initial state with spin, but has a spinless final state. This is a follow-up to {doc}`d2kkk`, where there were no alignment Wigner-$D$ functions."
@@ -27,30 +29,30 @@
                     "scroll-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "from __future__ import annotations\n",
                 "\n",
-                "import itertools\n",
                 "import logging\n",
                 "import os\n",
+                "import warnings\n",
                 "from textwrap import dedent\n",
-                "from typing import TYPE_CHECKING, Iterable\n",
+                "from typing import TYPE_CHECKING\n",
                 "\n",
                 "import ampform\n",
                 "import graphviz\n",
                 "import ipywidgets\n",
                 "import jax.numpy as jnp\n",
                 "import matplotlib.pyplot as plt\n",
                 "import qrules\n",
                 "import sympy as sp\n",
                 "from ampform.kinematics.lorentz import FourMomentumSymbol, InvariantMass\n",
                 "from ampform.sympy import perform_cached_doit\n",
-                "from IPython.display import SVG, Latex, Markdown, clear_output, display\n",
+                "from IPython.display import Latex, Markdown, clear_output, display\n",
                 "from ipywidgets import (\n",
                 "    Accordion,\n",
                 "    Checkbox,\n",
                 "    GridBox,\n",
                 "    HBox,\n",
                 "    Layout,\n",
                 "    SelectMultiple,\n",
@@ -60,32 +62,33 @@
                 "    interactive_output,\n",
                 ")\n",
                 "from tensorwaves.data.phasespace import TFPhaseSpaceGenerator\n",
                 "from tensorwaves.data.rng import TFUniformRealNumberGenerator\n",
                 "from tensorwaves.data.transform import SympyDataTransformer\n",
                 "\n",
                 "from ampform_dpd import DalitzPlotDecompositionBuilder\n",
-                "from ampform_dpd.decay import IsobarNode, Particle, ThreeBodyDecay, ThreeBodyDecayChain\n",
+                "from ampform_dpd.adapter.qrules import normalize_state_ids, to_three_body_decay\n",
+                "from ampform_dpd.decay import Particle\n",
                 "from ampform_dpd.io import (\n",
                 "    as_markdown_table,\n",
                 "    aslatex,\n",
                 "    get_readable_hash,\n",
                 "    perform_cached_lambdify,\n",
                 "    simplify_latex_rendering,\n",
                 ")\n",
-                "from ampform_dpd.spin import filter_parity_violating_ls, generate_ls_couplings\n",
                 "\n",
                 "if TYPE_CHECKING:\n",
                 "    from ampform.helicity import HelicityModel\n",
                 "    from qrules.transition import ReactionInfo\n",
                 "    from tensorwaves.interface import DataSample, ParameterValue, ParametrizedFunction\n",
                 "\n",
                 "simplify_latex_rendering()\n",
                 "logging.getLogger(\"jax\").setLevel(logging.ERROR)  # mute JAX\n",
                 "os.environ[\"TF_CPP_MIN_LOG_LEVEL\"] = \"3\"  # mute TF\n",
+                "warnings.simplefilter(\"ignore\")\n",
                 "NO_TQDM = \"EXECUTE_NB\" in os.environ\n",
                 "if NO_TQDM:\n",
                 "    logging.getLogger(\"ampform.sympy\").setLevel(logging.ERROR)\n",
                 "    logging.getLogger(\"ampform_dpd.io\").setLevel(logging.ERROR)"
             ]
         },
         {
@@ -98,73 +101,50 @@
                 "## Decay definition"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "jupyter": {
-                    "source_hidden": true
-                },
                 "mystnb": {
-                    "code_prompt_show": "Define initial and final state"
+                    "code_prompt_show": "Generate transitions"
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "PDG = qrules.load_pdg()\n",
-                "PARTICLE_DB = {\n",
-                "    p.name: Particle(\n",
-                "        name=p.name,\n",
-                "        latex=p.latex,\n",
-                "        spin=p.spin,\n",
-                "        parity=int(p.parity),\n",
-                "        mass=p.mass,\n",
-                "        width=p.width,\n",
-                "    )\n",
-                "    for p in PDG\n",
-                "    if p.parity is not None\n",
-                "}\n",
-                "INITIAL_STATE = PARTICLE_DB[\"J/psi(1S)\"]\n",
-                "FS_zero = PARTICLE_DB[\"pi0\"]\n",
-                "FS_neg = PARTICLE_DB[\"pi-\"]\n",
-                "FS_pos = PARTICLE_DB[\"pi+\"]\n",
-                "PARTICLE_TO_ID = {INITIAL_STATE: 0, FS_zero: 1, FS_neg: 2, FS_pos: 3}\n",
-                "_, *FINAL_STATE = PARTICLE_TO_ID\n",
-                "Markdown(as_markdown_table(list(PARTICLE_TO_ID)))"
+                "REACTION = qrules.generate_transitions(\n",
+                "    initial_state=\"J/psi(1S)\",\n",
+                "    final_state=[\"pi0\", \"pi-\", \"pi+\"],\n",
+                "    allowed_intermediate_particles=[\"a(0)(980)\", \"rho(770)\"],\n",
+                "    mass_conservation_factor=0,\n",
+                "    formalism=\"helicity\",\n",
+                ")\n",
+                "REACTION123 = normalize_state_ids(REACTION)\n",
+                "dot = qrules.io.asdot(REACTION123, collapse_graphs=True)\n",
+                "graphviz.Source(dot)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
                     "source_hidden": true
                 },
-                "mystnb": {
-                    "code_prompt_show": "Generate transitions"
-                },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "reaction = qrules.generate_transitions(\n",
-                "    initial_state=INITIAL_STATE.name,\n",
-                "    final_state=[p.name for p in FINAL_STATE],\n",
-                "    allowed_intermediate_particles=[\"a(0)(980)\", \"rho(770)\"],\n",
-                "    mass_conservation_factor=0,\n",
-                "    formalism=\"helicity\",\n",
-                ")\n",
-                "dot = qrules.io.asdot(reaction, collapse_graphs=True)\n",
-                "graphviz.Source(dot)"
+                "DECAY = to_three_body_decay(REACTION123.transitions, min_ls=True)\n",
+                "Markdown(as_markdown_table([DECAY.initial_state, *DECAY.final_state.values()]))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -172,109 +152,35 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "qrules_resonances = sorted(\n",
-                "    reaction.get_intermediate_particles(),\n",
-                "    key=lambda p: (p.charge, p.mass, p.name),\n",
+                "resonances = sorted(\n",
+                "    {t.resonance for t in DECAY.chains},\n",
+                "    key=lambda p: (p.name[0], p.mass),\n",
                 ")\n",
-                "resonance_names = [p.name for p in qrules_resonances]\n",
-                "resonances = [PARTICLE_DB[name] for name in resonance_names]\n",
+                "resonance_names = [p.name for p in resonances]\n",
                 "Markdown(as_markdown_table(resonances))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
                     "source_hidden": true
                 },
                 "tags": [
-                    "hide-input",
-                    "scroll-input"
+                    "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "def load_three_body_decay(\n",
-                "    resonance_names: Iterable[str],\n",
-                "    particle_definitions: dict[str, Particle],\n",
-                "    min_ls: bool = True,\n",
-                ") -> ThreeBodyDecay:\n",
-                "    _resonances = [particle_definitions[name] for name in resonance_names]\n",
-                "    chains: list[ThreeBodyDecayChain] = []\n",
-                "    for res in _resonances:\n",
-                "        chains.extend(_create_isobar(res, min_ls))\n",
-                "    return ThreeBodyDecay(\n",
-                "        states={state_id: particle for particle, state_id in PARTICLE_TO_ID.items()},\n",
-                "        chains=tuple(chains),\n",
-                "    )\n",
-                "\n",
-                "\n",
-                "def _create_isobar(resonance: Particle, min_ls: bool) -> list[ThreeBodyDecayChain]:\n",
-                "    if resonance.name.endswith(\"-\"):\n",
-                "        child1, child2, spectator = FS_zero, FS_neg, FS_pos\n",
-                "    elif resonance.name.endswith(\"+\"):\n",
-                "        child1, child2, spectator = FS_pos, FS_zero, FS_neg\n",
-                "    else:\n",
-                "        child1, child2, spectator = FS_neg, FS_pos, FS_zero\n",
-                "    prod_ls_couplings = _generate_ls(\n",
-                "        INITIAL_STATE, resonance, spectator, conserve_parity=False\n",
-                "    )\n",
-                "    dec_ls_couplings = _generate_ls(resonance, child1, child2, conserve_parity=True)\n",
-                "    if min_ls:\n",
-                "        decay = IsobarNode(\n",
-                "            parent=INITIAL_STATE,\n",
-                "            child1=IsobarNode(\n",
-                "                parent=resonance,\n",
-                "                child1=child1,\n",
-                "                child2=child2,\n",
-                "                interaction=min(dec_ls_couplings),\n",
-                "            ),\n",
-                "            child2=spectator,\n",
-                "            interaction=min(prod_ls_couplings),\n",
-                "        )\n",
-                "        return [ThreeBodyDecayChain(decay)]\n",
-                "    chains = []\n",
-                "    for dec_ls, prod_ls in itertools.product(dec_ls_couplings, prod_ls_couplings):\n",
-                "        decay = IsobarNode(\n",
-                "            parent=INITIAL_STATE,\n",
-                "            child1=IsobarNode(\n",
-                "                parent=resonance,\n",
-                "                child1=child1,\n",
-                "                child2=child2,\n",
-                "                interaction=dec_ls,\n",
-                "            ),\n",
-                "            child2=spectator,\n",
-                "            interaction=prod_ls,\n",
-                "        )\n",
-                "        chains.append(ThreeBodyDecayChain(decay))\n",
-                "    return chains\n",
-                "\n",
-                "\n",
-                "def _generate_ls(\n",
-                "    parent: Particle, child1: Particle, child2: Particle, conserve_parity: bool\n",
-                ") -> list[tuple[int, sp.Rational]]:\n",
-                "    ls = generate_ls_couplings(parent.spin, child1.spin, child2.spin)\n",
-                "    if conserve_parity:\n",
-                "        return filter_parity_violating_ls(\n",
-                "            ls, parent.parity, child1.parity, child2.parity\n",
-                "        )\n",
-                "    return ls\n",
-                "\n",
-                "\n",
-                "DECAY = load_three_body_decay(\n",
-                "    resonance_names,\n",
-                "    particle_definitions=PARTICLE_DB,\n",
-                "    min_ls=True,\n",
-                ")\n",
                 "Latex(aslatex(DECAY, with_jp=True))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "tags": []
@@ -297,22 +203,24 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
                     "source_hidden": true
                 },
                 "tags": [
+                    "full-width",
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "model_builder = DalitzPlotDecompositionBuilder(DECAY, min_ls=True)\n",
-                "dpd_model = model_builder.formulate(reference_subsystem=1)\n",
-                "dpd_model.intensity"
+                "DPD_MODEL = model_builder.formulate(reference_subsystem=1)\n",
+                "del model_builder\n",
+                "DPD_MODEL.intensity.cleanup()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -321,38 +229,24 @@
                 "tags": [
                     "hide-input",
                     "full-width"
                 ]
             },
             "outputs": [],
             "source": [
-                "Latex(aslatex(dpd_model.amplitudes))"
+                "Latex(aslatex(DPD_MODEL.amplitudes))"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "There is an isobar Wigner-$d$ function, which takes the following helicity angles as argument:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
             "metadata": {
-                "jupyter": {
-                    "source_hidden": true
-                },
-                "tags": [
-                    "hide-input"
-                ]
+                "tags": []
             },
-            "outputs": [],
             "source": [
-                "Latex(aslatex(dpd_model.variables))"
+                "There is an isobar Wigner-$d$ function, which takes the following helicity angles as argument:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -360,20 +254,15 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "masses = {\n",
-                "    sp.Symbol(f\"m{i}\", nonnegative=True): round(p.mass, 7)\n",
-                "    for p, i in PARTICLE_TO_ID.items()\n",
-                "}\n",
-                "dpd_model.parameter_defaults.update(masses)\n",
-                "Latex(aslatex(masses))"
+                "Latex(aslatex(DPD_MODEL.variables))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "jp-MarkdownHeadingCollapsed": true,
                 "tags": []
@@ -391,18 +280,20 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "model_builder = ampform.get_builder(reaction)\n",
+                "model_builder = ampform.get_builder(REACTION)\n",
                 "model_builder.use_helicity_couplings = False\n",
-                "ampform_model = model_builder.formulate()\n",
-                "ampform_model.intensity"
+                "model_builder.config.scalar_initial_state_mass = True\n",
+                "model_builder.config.stable_final_state_ids = [0, 1, 2]\n",
+                "AMPFORM_MODEL = model_builder.formulate()\n",
+                "AMPFORM_MODEL.intensity"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -411,15 +302,15 @@
                 "tags": [
                     "hide-input",
                     "full-width"
                 ]
             },
             "outputs": [],
             "source": [
-                "Latex(aslatex(ampform_model.amplitudes))"
+                "Latex(aslatex(AMPFORM_MODEL.amplitudes))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -427,15 +318,15 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "Latex(aslatex(ampform_model.kinematic_variables))"
+                "Latex(aslatex(AMPFORM_MODEL.kinematic_variables))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "jp-MarkdownHeadingCollapsed": true,
                 "tags": []
@@ -444,44 +335,45 @@
                 "## Phase space sample"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
+                "jupyter": {
+                    "source_hidden": true
+                },
                 "mystnb": {
                     "code_prompt_show": "Formulate kinematic variables in terms of four-momenta"
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "p1, p2, p3 = tuple(FourMomentumSymbol(f\"p{i}\", shape=[]) for i in (0, 1, 2))\n",
-                "s1, s2, s3 = sp.symbols(\"sigma1:4\", nonnegative=True)\n",
+                "s1, s2, s3 = sorted(DPD_MODEL.invariants, key=str)\n",
                 "mass_definitions = {\n",
+                "    **DPD_MODEL.masses,\n",
                 "    s1: InvariantMass(p2 + p3) ** 2,\n",
                 "    s2: InvariantMass(p1 + p3) ** 2,\n",
                 "    s3: InvariantMass(p1 + p2) ** 2,\n",
                 "    sp.Symbol(\"m_01\", nonnegative=True): InvariantMass(p1 + p2),\n",
                 "    sp.Symbol(\"m_02\", nonnegative=True): InvariantMass(p1 + p3),\n",
                 "    sp.Symbol(\"m_12\", nonnegative=True): InvariantMass(p2 + p3),\n",
                 "}\n",
                 "dpd_variables = {\n",
-                "    sp.Symbol(f\"m{i}\", nonnegative=True): sp.Float(p.mass)\n",
-                "    for i, p in enumerate(PARTICLE_TO_ID)\n",
+                "    symbol: expr.doit().xreplace(DPD_MODEL.variables).xreplace(mass_definitions)\n",
+                "    for symbol, expr in DPD_MODEL.variables.items()\n",
                 "}\n",
-                "for symbol, expr in dpd_model.variables.items():\n",
-                "    expr = expr.doit().xreplace(mass_definitions).xreplace(dpd_variables)\n",
-                "    dpd_variables[symbol] = expr\n",
                 "dpd_transformer = SympyDataTransformer.from_sympy(dpd_variables, backend=\"jax\")\n",
                 "\n",
                 "ampform_transformer = SympyDataTransformer.from_sympy(\n",
-                "    ampform_model.kinematic_variables, backend=\"jax\"\n",
+                "    AMPFORM_MODEL.kinematic_variables, backend=\"jax\"\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
@@ -494,15 +386,15 @@
                 "    phsp_generator = TFPhaseSpaceGenerator(\n",
                 "        initial_state_mass=reaction.initial_state[-1].mass,\n",
                 "        final_state_masses={i: p.mass for i, p in reaction.final_state.items()},\n",
                 "    )\n",
                 "    return phsp_generator.generate(size, rng)\n",
                 "\n",
                 "\n",
-                "phsp = generate_phase_space(ampform_model.reaction_info, size=100_000)\n",
+                "phsp = generate_phase_space(AMPFORM_MODEL.reaction_info, size=100_000)\n",
                 "ampform_phsp = ampform_transformer(phsp)\n",
                 "dpd_phsp = dpd_transformer(phsp)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
@@ -525,33 +417,33 @@
                 "    unfolded_intensity = perform_cached_doit(model.intensity)\n",
                 "    unfolded_amplitudes = {\n",
                 "        symbol: perform_cached_doit(expr) for symbol, expr in model.amplitudes.items()\n",
                 "    }\n",
                 "    return unfolded_intensity.xreplace(unfolded_amplitudes)\n",
                 "\n",
                 "\n",
-                "ampform_intensity_expr = unfold_intensity(ampform_model)\n",
-                "dpd_intensity_expr = unfold_intensity(dpd_model)"
+                "ampform_intensity_expr = unfold_intensity(AMPFORM_MODEL)\n",
+                "dpd_intensity_expr = unfold_intensity(DPD_MODEL)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "ampform_func = perform_cached_lambdify(\n",
                 "    ampform_intensity_expr,\n",
-                "    parameters=ampform_model.parameter_defaults,\n",
+                "    parameters=AMPFORM_MODEL.parameter_defaults,\n",
                 ")\n",
                 "dpd_func = perform_cached_lambdify(\n",
                 "    dpd_intensity_expr,\n",
-                "    parameters=dpd_model.parameter_defaults,\n",
+                "    parameters=DPD_MODEL.parameter_defaults,\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -617,16 +509,16 @@
                     "hide-input",
                     "scroll-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "def create_sliders() -> dict[str, ToggleButtons]:\n",
-                "    all_parameters = dict(ampform_model.parameter_defaults.items())\n",
-                "    all_parameters.update(dpd_model.parameter_defaults)\n",
+                "    all_parameters = dict(AMPFORM_MODEL.parameter_defaults.items())\n",
+                "    all_parameters.update(DPD_MODEL.parameter_defaults)\n",
                 "    sliders = {}\n",
                 "    for symbol, value in all_parameters.items():\n",
                 "        value = \"+1\"\n",
                 "        if (\n",
                 "            symbol.name.startswith(R\"\\mathcal{H}^\\mathrm{decay}\") and \"+\" in symbol.name\n",
                 "        ) and any(s in symbol.name for s in [\"{1}\", \"*\", \"rho\"]):\n",
                 "            value = \"-1\"\n",
@@ -703,14 +595,15 @@
                 "jupyter": {
                     "source_hidden": true
                 },
                 "mystnb": {
                     "code_prompt_show": "Generate comparison widget"
                 },
                 "tags": [
+                    "full-width",
                     "hide-input",
                     "scroll-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "%matplotlib widget\n",
@@ -719,25 +612,26 @@
                 "fig.canvas.toolbar_visible = False\n",
                 "fig.canvas.header_visible = False\n",
                 "fig.canvas.footer_visible = False\n",
                 "(\n",
                 "    (ax_s1, ax_s2, ax_s3),\n",
                 "    (ax_t1, ax_t2, ax_t3),\n",
                 ") = axes\n",
-                "final_state = ampform_model.reaction_info.final_state\n",
                 "for ax in axes[:, 0].flatten():\n",
                 "    ax.set_ylabel(\"Intensity (a.u.)\")\n",
                 "for ax in axes[:, 1:].flatten():\n",
                 "    ax.set_yticks([])\n",
-                "ax_s1.set_xlabel(f\"$m({FINAL_STATE[1].latex}, {FINAL_STATE[2].latex})$\")\n",
-                "ax_s2.set_xlabel(f\"$m({FINAL_STATE[0].latex}, {FINAL_STATE[2].latex})$\")\n",
-                "ax_s3.set_xlabel(f\"$m({FINAL_STATE[0].latex}, {FINAL_STATE[1].latex})$\")\n",
-                "ax_t1.set_xlabel(Rf\"$\\theta({FINAL_STATE[1].latex}, {FINAL_STATE[2].latex})$\")\n",
-                "ax_t2.set_xlabel(Rf\"$\\theta({FINAL_STATE[0].latex}, {FINAL_STATE[2].latex})$\")\n",
-                "ax_t3.set_xlabel(Rf\"$\\theta({FINAL_STATE[0].latex}, {FINAL_STATE[1].latex})$\")\n",
+                "\n",
+                "final_state = DECAY.final_state\n",
+                "ax_s1.set_xlabel(f\"$m({final_state[2].latex}, {final_state[3].latex})$\")\n",
+                "ax_s2.set_xlabel(f\"$m({final_state[1].latex}, {final_state[3].latex})$\")\n",
+                "ax_s3.set_xlabel(f\"$m({final_state[1].latex}, {final_state[2].latex})$\")\n",
+                "ax_t1.set_xlabel(Rf\"$\\theta({final_state[2].latex}, {final_state[3].latex})$\")\n",
+                "ax_t2.set_xlabel(Rf\"$\\theta({final_state[1].latex}, {final_state[3].latex})$\")\n",
+                "ax_t3.set_xlabel(Rf\"$\\theta({final_state[1].latex}, {final_state[2].latex})$\")\n",
                 "fig.suptitle(f'Selected resonances: ${\", \".join(resonance_selector.value)}$')\n",
                 "fig.tight_layout()\n",
                 "\n",
                 "lines = None\n",
                 "\n",
                 "__EXPRS: dict[int, sp.Expr] = {}\n",
                 "\n",
@@ -924,21 +818,21 @@
                 "    if hide_expressions.value:\n",
                 "        clear_output()\n",
                 "    else:\n",
                 "        if simplify_expressions.value:\n",
                 "            ampform_expr = _simplify(\n",
                 "                ampform_intensity_expr,\n",
                 "                ampform_pars,\n",
-                "                ampform_model.kinematic_variables,\n",
+                "                AMPFORM_MODEL.kinematic_variables,\n",
                 "                selected_resonances,\n",
                 "            )\n",
                 "            dpd_expr = _simplify(\n",
                 "                dpd_intensity_expr,\n",
                 "                dpd_pars,\n",
-                "                dpd_model.variables,\n",
+                "                DPD_MODEL.variables,\n",
                 "                selected_resonances,\n",
                 "            )\n",
                 "        else:\n",
                 "            ampform_expr = ampform_intensity_expr\n",
                 "            dpd_expr = dpd_intensity_expr\n",
                 "        src = Rf\"\"\"\n",
                 "        \\begin{{eqnarray}}\n",
@@ -957,34 +851,14 @@
                 "        \"resonance_selector\": resonance_selector,\n",
                 "        \"hide_expressions\": hide_expressions,\n",
                 "        \"simplify_expressions\": simplify_expressions,\n",
                 "    },\n",
                 ")\n",
                 "display(output, ui)"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "jupyter": {
-                    "source_hidden": true
-                },
-                "tags": [
-                    "remove-input",
-                    "full-width"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "if NO_TQDM:\n",
-                "    filename = \"jpsi2pipipi-comparison.svg\"\n",
-                "    plt.savefig(filename)\n",
-                "    display(SVG(filename))"
-            ]
         }
     ],
     "metadata": {
         "colab": {
             "toc_visible": true
         },
         "kernelspec": {
@@ -998,13 +872,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.17"
+            "version": "3.9.19"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `ampform-dpd-0.1.6/docs/conf.py` & `ampform_dpd-0.1.7/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,26 +32,29 @@
 BINDER_LINK = f"https://mybinder.org/v2/gh/{ORGANIZATION}/{REPO_NAME}/{BRANCH}?filepath=docs/usage"
 EXECUTE_NB = get_execution_mode() != "off"
 
 
 add_module_names = False
 api_github_repo = f"{ORGANIZATION}/{REPO_NAME}"
 api_target_substitutions: dict[str, str | tuple[str, str]] = {
-    "Literal[(-1, 1)]": "typing.Literal",
+    "FrozenTransition": "qrules.topology.FrozenTransition",
     "Literal[-1, 1]": "typing.Literal",
+    "Literal[(-1, 1)]": "typing.Literal",
     "OuterStates": ("obj", "ampform_dpd.decay.OuterStates"),
     "ParameterValue": ("obj", "tensorwaves.interface.ParameterValue"),
     "ParametrizedBackendFunction": "tensorwaves.function.ParametrizedBackendFunction",
     "PoolSum": "ampform.sympy.PoolSum",
     "PositionalArgumentFunction": "tensorwaves.function.PositionalArgumentFunction",
+    "qrules.topology.EdgeType": "typing.TypeVar",
+    "qrules.topology.NodeType": "typing.TypeVar",
+    "sp.acos": "sympy.functions.elementary.trigonometric.acos",
     "sp.Expr": "sympy.core.expr.Expr",
     "sp.Indexed": "sympy.tensor.indexed.Indexed",
     "sp.Rational": "sympy.core.numbers.Rational",
     "sp.Symbol": "sympy.core.symbol.Symbol",
-    "sp.acos": "sympy.functions.elementary.trigonometric.acos",
 }
 api_target_types: dict[str, str] = {}
 author = "Common Partial Wave Analysis"
 autodoc_default_options = {
     "exclude-members": ", ".join([
         "default_assumptions",
         "doit",
@@ -60,15 +63,14 @@
         "is_extended_real",
     ]),
     "members": True,
     "undoc-members": True,
     "show-inheritance": True,
 }
 autodoc_member_order = "bysource"
-autodoc_type_aliases = {}
 autodoc_typehints_format = "short"
 autosectionlabel_prefix_document = True
 autosectionlabel_maxdepth = 2
 bibtex_bibfiles = ["references.bib"]
 bibtex_default_style = "unsrt_et_al"
 codeautolink_concat_default = True
 copybutton_prompt_is_regexp = True
@@ -84,15 +86,14 @@
 extensions = [
     "myst_nb",
     "sphinx.ext.autosectionlabel",
     "sphinx.ext.doctest",
     "sphinx.ext.githubpages",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
-    "sphinx.ext.viewcode",
     "sphinx_api_relink",
     "sphinx_book_theme",
     "sphinx_codeautolink",
     "sphinx_copybutton",
     "sphinx_design",
     "sphinx_pybtex_etal_style",
     "sphinx_togglebutton",
```

### Comparing `ampform-dpd-0.1.6/docs/index.md` & `ampform_dpd-0.1.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `ampform-dpd-0.1.6/docs/jpsi2ksp.ipynb` & `ampform_dpd-0.1.7/docs/jpsi2ksp.ipynb`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9700886883802903%*

 * *Differences: {"'cells'": "{0: {'metadata': {replace: OrderedDict([('tags', [])])}}, 1: {'source': {insert: [(4, "*

 * *            "'import warnings\\n'), (5, 'from typing import TYPE_CHECKING\\n'), (7, 'import "*

 * *            "graphviz\\n'), (12, 'from ampform.dynamics import BlattWeisskopfSquared, "*

 * *            "EnergyDependentWidth\\n'), (13, 'from ampform.sympy import perform_cached_doit\\n'), "*

 * *            "(18, 'from ampform_dpd import DalitzPlotDecompositionBuilder, get_particle\\n'), (19, "*

 * *            "'from ampform_d […]*

```diff
@@ -1,12 +1,14 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
                 "# J/\u03c8 \u2192 K\u2070 \u03a3\u207a p\u0305\n",
                 "\n",
                 "```{autolink-concat}\n",
                 "```"
             ]
         },
@@ -22,68 +24,66 @@
                     "scroll-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "from __future__ import annotations\n",
                 "\n",
-                "import itertools\n",
                 "import logging\n",
                 "import os\n",
-                "from typing import TYPE_CHECKING, Any, Iterable\n",
+                "import warnings\n",
+                "from typing import TYPE_CHECKING\n",
                 "\n",
+                "import graphviz\n",
                 "import jax.numpy as jnp\n",
                 "import matplotlib.pyplot as plt\n",
                 "import qrules\n",
                 "import sympy as sp\n",
-                "from ampform.dynamics import EnergyDependentWidth, formulate_form_factor\n",
-                "from ampform.kinematics.phasespace import compute_third_mandelstam\n",
-                "from ampform.sympy import perform_cached_doit, unevaluated\n",
+                "from ampform.dynamics import BlattWeisskopfSquared, EnergyDependentWidth\n",
+                "from ampform.sympy import perform_cached_doit\n",
                 "from IPython.display import Latex, Markdown\n",
                 "from tensorwaves.data.transform import SympyDataTransformer\n",
                 "from tqdm.auto import tqdm\n",
                 "\n",
-                "from ampform_dpd import DalitzPlotDecompositionBuilder, _get_particle\n",
-                "from ampform_dpd.decay import IsobarNode, Particle, ThreeBodyDecay, ThreeBodyDecayChain\n",
+                "from ampform_dpd import DalitzPlotDecompositionBuilder, get_particle\n",
+                "from ampform_dpd.adapter.qrules import normalize_state_ids, to_three_body_decay\n",
+                "from ampform_dpd.decay import IsobarNode, Particle, ThreeBodyDecayChain\n",
+                "from ampform_dpd.dynamics import FormFactor, RelativisticBreitWigner\n",
                 "from ampform_dpd.io import (\n",
                 "    as_markdown_table,\n",
                 "    aslatex,\n",
                 "    perform_cached_lambdify,\n",
                 "    simplify_latex_rendering,\n",
                 ")\n",
-                "from ampform_dpd.spin import filter_parity_violating_ls, generate_ls_couplings\n",
-                "\n",
-                "if TYPE_CHECKING:\n",
-                "    from tensorwaves.interface import DataSample, ParametrizedFunction\n",
                 "\n",
                 "simplify_latex_rendering()\n",
                 "logging.getLogger(\"absl\").setLevel(logging.ERROR)  # mute JAX\n",
+                "warnings.simplefilter(\"ignore\")\n",
+                "\n",
                 "NO_TQDM = \"EXECUTE_NB\" in os.environ\n",
                 "if NO_TQDM:\n",
-                "    logging.getLogger(\"ampform_dpd.io\").setLevel(logging.ERROR)"
+                "    logging.getLogger(\"ampform_dpd.io\").setLevel(logging.ERROR)\n",
+                "if TYPE_CHECKING:\n",
+                "    from tensorwaves.interface import DataSample, ParametrizedFunction"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "jp-MarkdownHeadingCollapsed": true
+            },
             "source": [
                 "## Decay definition"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "We follow [this example](https://qrules.readthedocs.io/en/0.9.7/usage.html#investigate-intermediate-resonances), which was generated with QRules, and leave out the $K$-resonances and the resonances that lie far outside of phase space:\n",
-                "\n",
-                "![](https://qrules.readthedocs.io/en/0.9.7/_images/usage_9_0.svg)\n",
-                "\n",
-                ":::{warning}\n",
-                "In the above figure, the final states are labeled `0`, `1`, `2`, but in the DPD formalism, the final states are labeled `1`, `2`, `3`.\n",
-                ":::"
+                "We follow [this example](https://qrules.readthedocs.io/en/0.10.1/usage.html#investigate-intermediate-resonances), which was generated with QRules, and leave out the $K$-resonances and the resonances that lie far outside of phase space."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -91,33 +91,24 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "PDG = qrules.load_pdg()\n",
-                "PARTICLE_DB = {\n",
-                "    p.name: Particle(\n",
-                "        name=p.name,\n",
-                "        latex=p.latex,\n",
-                "        spin=p.spin,\n",
-                "        parity=int(p.parity),\n",
-                "        mass=p.mass,\n",
-                "        width=p.width,\n",
-                "    )\n",
-                "    for p in PDG\n",
-                "    if p.parity is not None\n",
-                "}\n",
-                "Jpsi = PARTICLE_DB[\"J/psi(1S)\"]\n",
-                "K = PARTICLE_DB[\"K0\"]\n",
-                "\u03a3 = PARTICLE_DB[\"Sigma+\"]\n",
-                "pbar = PARTICLE_DB[\"p~\"]\n",
-                "PARTICLE_TO_ID = {Jpsi: 0, K: 1, \u03a3: 2, pbar: 3}\n",
-                "Markdown(as_markdown_table(list(PARTICLE_TO_ID)))"
+                "REACTION = qrules.generate_transitions(\n",
+                "    initial_state=\"J/psi(1S)\",\n",
+                "    final_state=[\"K0\", \"Sigma+\", \"p~\"],\n",
+                "    allowed_interaction_types=\"strong\",\n",
+                "    formalism=\"canonical-helicity\",\n",
+                "    mass_conservation_factor=0.05,\n",
+                ")\n",
+                "REACTION = normalize_state_ids(REACTION)\n",
+                "dot = qrules.io.asdot(REACTION, collapse_graphs=True)\n",
+                "graphviz.Source(dot)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -125,26 +116,16 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "resonance_names = [\n",
-                "    \"Sigma(1660)~-\",\n",
-                "    \"Sigma(1670)~-\",\n",
-                "    \"Sigma(1750)~-\",\n",
-                "    \"Sigma(1775)~-\",\n",
-                "    \"Sigma(1910)~-\",\n",
-                "    \"N(1700)+\",\n",
-                "    \"N(1710)+\",\n",
-                "    \"N(1720)+\",\n",
-                "]\n",
-                "resonances = [PARTICLE_DB[name] for name in resonance_names]\n",
-                "Markdown(as_markdown_table(resonances))"
+                "DECAY = to_three_body_decay(REACTION.transitions, min_ls=True)\n",
+                "Markdown(as_markdown_table([DECAY.initial_state, *DECAY.final_state.values()]))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -152,230 +133,100 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "def load_three_body_decay(\n",
-                "    resonance_names: Iterable[str],\n",
-                "    particle_definitions: dict[str, Particle],\n",
-                "    min_ls: bool = True,\n",
-                ") -> ThreeBodyDecay:\n",
-                "    resonances = [particle_definitions[name] for name in resonance_names]\n",
-                "    chains: list[ThreeBodyDecayChain] = []\n",
-                "    for res in resonances:\n",
-                "        chains.extend(_create_isobar(res, min_ls))\n",
-                "    return ThreeBodyDecay(\n",
-                "        states={state_id: particle for particle, state_id in PARTICLE_TO_ID.items()},\n",
-                "        chains=tuple(chains),\n",
-                "    )\n",
-                "\n",
-                "\n",
-                "def _create_isobar(resonance: Particle, min_ls: bool) -> list[ThreeBodyDecayChain]:\n",
-                "    if resonance.name.startswith(\"Sigma\"):\n",
-                "        child1, child2, spectator = pbar, K, \u03a3\n",
-                "    elif resonance.name.startswith(\"N\"):\n",
-                "        child1, child2, spectator = K, \u03a3, pbar\n",
-                "    elif resonance.name.startswith(\"K\"):\n",
-                "        child1, child2, spectator = \u03a3, pbar, K\n",
-                "    else:\n",
-                "        raise NotImplementedError\n",
-                "    prod_ls_couplings = _generate_ls(Jpsi, resonance, spectator, conserve_parity=False)\n",
-                "    dec_ls_couplings = _generate_ls(resonance, child1, child2, conserve_parity=True)\n",
-                "    if min_ls:\n",
-                "        decay = IsobarNode(\n",
-                "            parent=Jpsi,\n",
-                "            child1=IsobarNode(\n",
-                "                parent=resonance,\n",
-                "                child1=child1,\n",
-                "                child2=child2,\n",
-                "                interaction=min(dec_ls_couplings),\n",
-                "            ),\n",
-                "            child2=spectator,\n",
-                "            interaction=min(prod_ls_couplings),\n",
-                "        )\n",
-                "        return [ThreeBodyDecayChain(decay)]\n",
-                "    chains = []\n",
-                "    for dec_ls, prod_ls in itertools.product(dec_ls_couplings, prod_ls_couplings):\n",
-                "        decay = IsobarNode(\n",
-                "            parent=Jpsi,\n",
-                "            child1=IsobarNode(\n",
-                "                parent=resonance,\n",
-                "                child1=child1,\n",
-                "                child2=child2,\n",
-                "                interaction=dec_ls,\n",
-                "            ),\n",
-                "            child2=spectator,\n",
-                "            interaction=prod_ls,\n",
-                "        )\n",
-                "        chains.append(ThreeBodyDecayChain(decay))\n",
-                "    return chains\n",
-                "\n",
-                "\n",
-                "def _generate_ls(\n",
-                "    parent: Particle, child1: Particle, child2: Particle, conserve_parity: bool\n",
-                ") -> list[tuple[int, sp.Rational]]:\n",
-                "    ls = generate_ls_couplings(parent.spin, child1.spin, child2.spin)\n",
-                "    if conserve_parity:\n",
-                "        return filter_parity_violating_ls(\n",
-                "            ls, parent.parity, child1.parity, child2.parity\n",
-                "        )\n",
-                "    return ls\n",
-                "\n",
-                "\n",
-                "DECAY = load_three_body_decay(\n",
-                "    resonance_names,\n",
-                "    particle_definitions=PARTICLE_DB,\n",
-                "    min_ls=True,\n",
+                "resonances = sorted(\n",
+                "    {t.resonance for t in DECAY.chains},\n",
+                "    key=lambda p: (p.name[0], p.mass),\n",
                 ")\n",
-                "Latex(aslatex(DECAY, with_jp=True))"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "## Lineshapes for dynamics"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                ":::{note}\n",
-                "As opposed to [AmpForm](https://ampform.rtfd.io), AmpForm-DPD defines dynamics over the **entire decay chain**, not a single isobar node. The dynamics classes and the corresponding builders would have to be extended to implement other dynamics lineshapes.\n",
-                ":::"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "In the following, we define the **relativistic Breit-Wigner function** as:"
+                "resonance_names = [p.name for p in resonances]\n",
+                "Markdown(as_markdown_table(resonances))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "jupyter": {
-                    "source_hidden": true
-                },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "@unevaluated\n",
-                "class RelativisticBreitWigner(sp.Expr):\n",
-                "    s: Any\n",
-                "    mass0: Any\n",
-                "    gamma0: Any\n",
-                "    m1: Any\n",
-                "    m2: Any\n",
-                "    angular_momentum: Any\n",
-                "    meson_radius: Any\n",
-                "    _latex_repr_ = (\n",
-                "        R\"\\mathcal{{R}}_{{{angular_momentum}}}\\left({s}, {mass0}, {gamma0}\\right)\"\n",
-                "    )\n",
-                "\n",
-                "    def evaluate(self):\n",
-                "        s, m0, w0, m1, m2, angular_momentum, meson_radius = self.args\n",
-                "        width = EnergyDependentWidth(\n",
-                "            s=s,\n",
-                "            mass0=m0,\n",
-                "            gamma0=w0,\n",
-                "            m_a=m1,\n",
-                "            m_b=m2,\n",
-                "            angular_momentum=angular_momentum,\n",
-                "            meson_radius=meson_radius,\n",
-                "            name=Rf\"\\Gamma_{{{sp.latex(angular_momentum)}}}\",\n",
-                "        )\n",
-                "        return (m0 * w0) / (m0**2 - s - width * m0 * sp.I)\n",
-                "\n",
-                "\n",
-                "bw = RelativisticBreitWigner(*sp.symbols(\"s m0 Gamma0 m1 m2 L R\"))\n",
-                "Latex(aslatex({bw: bw.doit(deep=False)}))"
+                "Latex(aslatex(DECAY, with_jp=True))"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "metadata": {
+                "jp-MarkdownHeadingCollapsed": true
+            },
+            "source": [
+                "## Lineshapes for dynamics"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "with $\\Gamma_0(s)$ a {class}`~ampform.dynamics.EnergyDependentWidth`, and we define the **form factor** as:"
+                ":::{note}\n",
+                "As opposed to [AmpForm](https://ampform.rtfd.io), AmpForm-DPD defines dynamics over the **entire decay chain**, not a single isobar node. The dynamics classes and the corresponding builders would have to be extended to implement other dynamics lineshapes.\n",
+                ":::"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
                     "source_hidden": true
                 },
                 "tags": [
-                    "hide-input"
+                    "hide-input",
+                    "full-width"
                 ]
             },
             "outputs": [],
             "source": [
-                "@unevaluated\n",
-                "class FormFactor(sp.Expr):\n",
-                "    s: Any\n",
-                "    m1: Any\n",
-                "    m2: Any\n",
-                "    angular_momentum: Any\n",
-                "    meson_radius: Any\n",
-                "\n",
-                "    _latex_repr_ = R\"\\mathcal{{F}}_{{{angular_momentum}}}\\left({s}, {m1}, {m1}\\right)\"\n",
-                "\n",
-                "    def evaluate(self):\n",
-                "        s, m1, m2, angular_momentum, meson_radius = self.args\n",
-                "        return formulate_form_factor(\n",
-                "            s=s,\n",
-                "            m_a=m1,\n",
-                "            m_b=m2,\n",
-                "            angular_momentum=angular_momentum,\n",
-                "            meson_radius=meson_radius,\n",
-                "        )\n",
-                "\n",
-                "\n",
-                "ff = FormFactor(*sp.symbols(\"s m1 m2 L R\"))\n",
-                "Latex(aslatex({ff: ff.doit(deep=False)}))"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "Here, $B_L^2$ is a {class}`~ampform.dynamics.BlattWeisskopfSquared`."
+                "s, m0, w0, m1, m2, L, R, z = sp.symbols(\"s m0 Gamma0 m1 m2 L R z\")\n",
+                "exprs = [\n",
+                "    RelativisticBreitWigner(s, m0, w0, m1, m2, L, R),\n",
+                "    EnergyDependentWidth(s, m0, w0, m1, m2, L, R),\n",
+                "    FormFactor(s, m1, m2, L, R),\n",
+                "    BlattWeisskopfSquared(z, L),\n",
+                "]\n",
+                "Latex(aslatex({e: e.doit(deep=False) for e in exprs}))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
                     "source_hidden": true
                 },
+                "mystnb": {
+                    "code_prompt_show": "Define dynamics builder functions"
+                },
                 "tags": [
                     "hide-input",
                     "scroll-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "def formulate_breit_wigner_with_ff(\n",
                 "    decay_chain: ThreeBodyDecayChain,\n",
                 ") -> tuple[sp.Expr, dict[sp.Symbol, float]]:\n",
                 "    production_node = decay_chain.decay\n",
                 "    assert isinstance(production_node.child1, IsobarNode), \"Not a 3-body isobar decay\"\n",
                 "    decay_node = production_node.child1\n",
-                "\n",
                 "    s = _get_mandelstam_s(decay_chain)\n",
                 "    parameter_defaults = {}\n",
                 "    production_ff, new_pars = _create_form_factor(s, production_node)\n",
                 "    parameter_defaults.update(new_pars)\n",
                 "    decay_ff, new_pars = _create_form_factor(s, decay_node)\n",
                 "    parameter_defaults.update(new_pars)\n",
                 "    breit_wigner, new_pars = _create_breit_wigner(s, decay_node)\n",
@@ -386,28 +237,35 @@
                 "    )\n",
                 "\n",
                 "\n",
                 "def _create_form_factor(\n",
                 "    s: sp.Symbol, isobar: IsobarNode\n",
                 ") -> tuple[sp.Expr, dict[sp.Symbol, float]]:\n",
                 "    assert isobar.interaction is not None, \"Need LS-couplings\"\n",
-                "    inv_mass = _create_mass_symbol(isobar.parent)\n",
+                "    if isobar.parent.name == \"J/psi(1S)\":\n",
+                "        inv_mass = sp.Symbol(\"m0\", nonnegative=True)\n",
+                "    else:\n",
+                "        inv_mass = _get_mandelstam_s(isobar)\n",
                 "    outgoing_state_mass1 = _create_mass_symbol(isobar.child1)\n",
                 "    outgoing_state_mass2 = _create_mass_symbol(isobar.child2)\n",
                 "    meson_radius = _create_meson_radius_symbol(isobar.parent)\n",
                 "    form_factor = FormFactor(\n",
                 "        s=inv_mass**2,\n",
                 "        m1=outgoing_state_mass1,\n",
                 "        m2=outgoing_state_mass2,\n",
                 "        angular_momentum=isobar.interaction.L,\n",
                 "        meson_radius=meson_radius,\n",
                 "    )\n",
                 "    parameter_defaults = {\n",
                 "        meson_radius: 1,\n",
+                "        outgoing_state_mass1: get_particle(isobar.child1).mass,\n",
+                "        outgoing_state_mass2: get_particle(isobar.child2).mass,\n",
                 "    }\n",
+                "    if not inv_mass.name.startswith(\"s\"):\n",
+                "        parameter_defaults[inv_mass] = get_particle(isobar).mass\n",
                 "    return form_factor, parameter_defaults\n",
                 "\n",
                 "\n",
                 "def _create_breit_wigner(\n",
                 "    s: sp.Symbol, isobar: IsobarNode\n",
                 ") -> tuple[sp.Expr, dict[sp.Symbol, float]]:\n",
                 "    assert isobar.interaction is not None, \"Need LS-couplings\"\n",
@@ -432,44 +290,50 @@
                 "        res_width: isobar.parent.width,\n",
                 "        meson_radius: 1,\n",
                 "    }\n",
                 "    return breit_wigner_expr, parameter_defaults\n",
                 "\n",
                 "\n",
                 "def _create_meson_radius_symbol(isobar: IsobarNode) -> sp.Symbol:\n",
-                "    if _get_particle(isobar) is Jpsi:\n",
+                "    if get_particle(isobar).name == \"J/psi(1S)\":\n",
                 "        return sp.Symbol(R\"R_{J/\\psi}\")\n",
                 "    return sp.Symbol(R\"R_\\mathrm{res}\")\n",
                 "\n",
                 "\n",
                 "def _create_mass_symbol(particle: IsobarNode | Particle) -> sp.Symbol:\n",
-                "    particle = _get_particle(particle)\n",
-                "    state_id = PARTICLE_TO_ID.get(particle)\n",
-                "    if state_id is not None:\n",
-                "        return sp.Symbol(f\"m{state_id}\", nonnegative=True)\n",
+                "    particle = get_particle(particle)\n",
                 "    return sp.Symbol(f\"m_{{{particle.latex}}}\", nonnegative=True)\n",
                 "\n",
                 "\n",
-                "def _get_mandelstam_s(decay: ThreeBodyDecayChain) -> sp.Symbol:\n",
+                "def _get_mandelstam_s(decay: ThreeBodyDecayChain | IsobarNode) -> sp.Symbol:\n",
                 "    s1, s2, s3 = sp.symbols(\"sigma1:4\", nonnegative=True)\n",
-                "    m1, m2, m3 = map(_create_mass_symbol, [K, \u03a3, pbar])\n",
-                "    decay_masses = {_create_mass_symbol(p) for p in decay.decay_products}\n",
-                "    if decay_masses == {m2, m3}:\n",
+                "    decay_products = {p.name for p in _get_decay_products(decay)}\n",
+                "    if decay_products == {\"Sigma+\", \"p~\"}:\n",
                 "        return s1\n",
-                "    if decay_masses == {m1, m3}:\n",
+                "    if decay_products == {\"K0\", \"p~\"}:\n",
                 "        return s2\n",
-                "    if decay_masses == {m1, m2}:\n",
+                "    if decay_products == {\"K0\", \"Sigma+\"}:\n",
                 "        return s3\n",
-                "    msg = f\"Cannot find Mandelstam variable for {''.join(decay_masses)}\"\n",
-                "    raise NotImplementedError(msg)"
+                "    msg = f\"Cannot find Mandelstam variable for {', '.join(decay_products)}\"\n",
+                "    raise NotImplementedError(msg)\n",
+                "\n",
+                "\n",
+                "def _get_decay_products(\n",
+                "    decay: ThreeBodyDecayChain | IsobarNode,\n",
+                ") -> tuple[Particle, Particle]:\n",
+                "    if isinstance(decay, ThreeBodyDecayChain):\n",
+                "        return decay.decay_products\n",
+                "    return decay.children"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "jp-MarkdownHeadingCollapsed": true
+            },
             "source": [
                 "## Model formulation"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -516,64 +380,40 @@
             },
             "outputs": [],
             "source": [
                 "Latex(aslatex(model.variables))"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {
-                "jupyter": {
-                    "source_hidden": true
-                },
-                "tags": [
-                    "hide-input"
-                ]
-            },
-            "outputs": [],
-            "source": [
-                "masses = {\n",
-                "    _create_mass_symbol(Jpsi): Jpsi.mass,\n",
-                "    _create_mass_symbol(K): K.mass,\n",
-                "    _create_mass_symbol(\u03a3): \u03a3.mass,\n",
-                "    _create_mass_symbol(pbar): pbar.mass,\n",
-                "}\n",
-                "model.parameter_defaults.update(masses)\n",
-                "Latex(aslatex(masses))"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Each **unaligned** amplitude is defined as follows:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "jupyter": {
-                    "source_hidden": true
-                },
                 "tags": [
                     "hide-input",
                     "full-width",
                     "hide-output"
                 ]
             },
             "outputs": [],
             "source": [
-                "Latex(aslatex(model.amplitudes))"
+                "Latex(aslatex({k: v for k, v in model.amplitudes.items() if v}))"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
                 "## Preparing for input data"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
@@ -591,62 +431,43 @@
                 "full_intensity_expr = perform_cached_doit(\n",
                 "    unfolded_intensity_expr.xreplace(model.amplitudes)\n",
                 ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "We set each helicity coupling to $1$, so that each each parameter {class}`~sympy.core.symbol.Symbol` in the expression has a definition:"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "couplings = {\n",
-                "    s: 1\n",
-                "    for s in full_intensity_expr.free_symbols\n",
-                "    if isinstance(s, sp.Indexed)\n",
-                "    if \"production\" in str(s) or \"decay\" in str(s)\n",
-                "}\n",
-                "model.parameter_defaults.update(couplings)"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
                 "With this, the remaining {class}`~sympy.core.symbol.Symbol`s in the full expression are kinematic variables.[^1]\n",
                 "\n",
                 "[^1]: Yes, there are still $\\mathcal{H}^\\mathrm{production}$ and $\\mathcal{H}^\\mathrm{decay}$, but these are the {attr}`~sympy.tensor.indexed.Indexed.base`s of the {class}`~sympy.tensor.indexed.Indexed` coupling symbols. They should **NOT** be substituted."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "jupyter": {
-                    "source_hidden": true
-                },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "sp.Array(full_intensity_expr.free_symbols - set(model.parameter_defaults))"
+                "sp.Array(\n",
+                "    sorted(full_intensity_expr.free_symbols - set(model.parameter_defaults), key=str)\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
                 "The $\\theta$ and $\\zeta$ angles are defined by the {attr}`~.AmplitudeModel.variables` attribute (they are shown under {ref}`jpsi2ksp:Model formulation`). Those definitions allow us to create a converter that computes kinematic variables from masses and Mandelstam variables:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -666,28 +487,32 @@
             "metadata": {},
             "source": [
                 "## Dalitz plot"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
                 "The data input for this data transformer can be several things. One can compute them from a (generated) data sample of four-momenta. Or one can compute them for a Dalitz plane. We do the latter in this section.\n",
                 "\n",
                 "First, the data transformer defined above expects values for the masses. We have already defined these values above, but we need to convert them from {mod}`sympy` objects to numerical data:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
-                "dalitz_data = {str(s): float(v) for s, v in masses.items()}"
+                "dalitz_data = {str(s): float(v) for s, v in model.masses.items()}"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "Next, we define a grid of data points over Mandelstam (Dalitz) variables $\\sigma_2=m_{13}, \\sigma_3=m_{12}$:"
@@ -706,41 +531,40 @@
                 ")\n",
                 "dalitz_data[\"sigma3\"] = X\n",
                 "dalitz_data[\"sigma2\"] = Y"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
                 "The remaining Mandelstam variable can be expressed in terms of the others as follows:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
-                "jupyter": {
-                    "source_hidden": true
-                },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "s1, s2, s3 = sp.symbols(\"sigma1:4\", nonnegative=True)\n",
-                "m0, m1, m2, m3 = sorted(masses, key=str)\n",
-                "s1_expr = compute_third_mandelstam(s3, s2, m0, m1, m2, m3)\n",
+                "(s1, s1_expr), *_ = model.invariants.items()\n",
                 "Latex(aslatex({s1: s1_expr}))"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
                 "That completes the data sample over which we want to evaluate the intensity model defined above:"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -754,23 +578,27 @@
                 "sigma1_func = perform_cached_lambdify(s1_expr, backend=\"jax\")\n",
                 "dalitz_data[\"sigma1\"] = sigma1_func(dalitz_data)\n",
                 "dalitz_data"
             ]
         },
         {
             "cell_type": "markdown",
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "source": [
                 "We can now extend the sample with angle definitions so that we have a data sample over which the intensity can be evaluated."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "angle_data = masses_to_angles(dalitz_data)\n",
                 "dalitz_data.update(angle_data)"
             ]
         },
         {
@@ -786,15 +614,17 @@
                 "for k, v in dalitz_data.items():\n",
                 "    assert not jnp.all(jnp.isnan(v)), f\"All values for {k} are NaN\""
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "metadata": {},
+            "metadata": {
+                "tags": []
+            },
             "outputs": [],
             "source": [
                 "free_parameters = {\n",
                 "    k: v\n",
                 "    for k, v in model.parameter_defaults.items()\n",
                 "    if isinstance(k, sp.Indexed)\n",
                 "    if \"production\" in str(k) or \"decay\" in str(k)\n",
@@ -909,22 +739,22 @@
                 "    ax.autoscale(enable=False, axis=\"x\")\n",
                 "ax1.set_ylabel(\"Normalized intensity (a.u.)\")\n",
                 "ax1.set_xlabel(R\"$M\\left(K^0\\Sigma^+\\right)$\")\n",
                 "ax2.set_xlabel(R\"$M\\left(K^0\\bar{p}\\right)$\")\n",
                 "i1, i2 = 0, 0\n",
                 "for chain in tqdm(model.decay.chains, disable=NO_TQDM):\n",
                 "    resonance = chain.resonance\n",
-                "    decay_product = set(chain.decay_products)\n",
-                "    if decay_product == {K, \u03a3}:\n",
+                "    decay_product = {p.name for p in chain.decay_products}\n",
+                "    if decay_product == {\"K0\", \"Sigma+\"}:\n",
                 "        ax = ax1\n",
                 "        i1 += 1\n",
                 "        i = i1\n",
                 "        projection_axis = 0\n",
                 "        x_data = x\n",
-                "    elif decay_product == {K, pbar}:\n",
+                "    elif decay_product == {\"K0\", \"p~\"}:\n",
                 "        ax = ax2\n",
                 "        i2 += 1\n",
                 "        i = i2\n",
                 "        projection_axis = 1\n",
                 "        x_data = y\n",
                 "    else:\n",
                 "        continue\n",
@@ -956,13 +786,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.18"
+            "version": "3.9.19"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `ampform-dpd-0.1.6/docs/lc2pkpi.ipynb` & `ampform_dpd-0.1.7/docs/lc2pkpi.ipynb`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9843323129861592%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(0, '# Λ<sub>c</sub>⁺ → p π⁺ K⁻\\n')], delete: [0]}}, 1: "*

 * *            "{'source': {insert: [(2, 'import warnings\\n'), (4, 'import graphviz\\n'), (9, 'from "*

 * *            "ampform_dpd import DalitzPlotDecompositionBuilder, get_particle\\n'), (10, 'from "*

 * *            "ampform_dpd.adapter.qrules import (\\n'), (11, '    load_particles,\\n'), (12, '    "*

 * *            "normalize_state_ids,\\n'), (13, '    to_three_body_decay,\\n'), (14, ')\\n'), (15, "*

 * *            "'from amp […]*

```diff
@@ -1,14 +1,14 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# \u039bc\u207a \u2192 p \u03c0\u207a K\u207b\n",
+                "# \u039b<sub>c</sub>\u207a \u2192 p \u03c0\u207a K\u207b\n",
                 "\n",
                 "```{autolink-concat}\n",
                 "```"
             ]
         },
         {
             "cell_type": "code",
@@ -22,28 +22,33 @@
                     "scroll-input"
                 ]
             },
             "outputs": [],
             "source": [
                 "from __future__ import annotations\n",
                 "\n",
-                "import itertools\n",
-                "from typing import Iterable\n",
+                "import warnings\n",
                 "\n",
+                "import graphviz\n",
                 "import qrules\n",
                 "import sympy as sp\n",
                 "from IPython.display import Latex, Markdown\n",
                 "\n",
-                "from ampform_dpd import DalitzPlotDecompositionBuilder\n",
-                "from ampform_dpd.decay import IsobarNode, Particle, ThreeBodyDecay, ThreeBodyDecayChain\n",
+                "from ampform_dpd import DalitzPlotDecompositionBuilder, get_particle\n",
+                "from ampform_dpd.adapter.qrules import (\n",
+                "    load_particles,\n",
+                "    normalize_state_ids,\n",
+                "    to_three_body_decay,\n",
+                ")\n",
+                "from ampform_dpd.decay import IsobarNode, Particle, ThreeBodyDecayChain\n",
                 "from ampform_dpd.dynamics import BreitWignerMinL\n",
                 "from ampform_dpd.io import as_markdown_table, aslatex, simplify_latex_rendering\n",
-                "from ampform_dpd.spin import filter_parity_violating_ls, generate_ls_couplings\n",
                 "\n",
-                "simplify_latex_rendering()"
+                "simplify_latex_rendering()\n",
+                "warnings.simplefilter(\"ignore\")"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Decay definition"
@@ -58,41 +63,43 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "PDG = qrules.load_pdg()\n",
-                "PARTICLE_DB = {\n",
-                "    p.name: Particle(\n",
-                "        name=p.name,\n",
-                "        latex=p.latex,\n",
-                "        spin=p.spin,\n",
-                "        parity=int(p.parity),\n",
-                "        mass=p.mass,\n",
-                "        width=p.width,\n",
-                "    )\n",
-                "    for p in PDG\n",
-                "    if p.parity is not None\n",
-                "}\n",
-                "PARTICLE_DB[\"Lambda(2000)\"] = Particle(\n",
-                "    name=\"Lambda(2000)\",\n",
-                "    latex=R\"\\Lambda(2000)\",\n",
-                "    spin=0.5,\n",
-                "    parity=-1,\n",
-                "    mass=2.0,\n",
-                "    width=(0.020 + 0.400) / 2,\n",
+                "PARTICLES = load_particles()\n",
+                "for name in [\n",
+                "    \"K*(1410)~0\",\n",
+                "    \"K(2)*(1430)~0\",\n",
+                "    \"K*(1680)~0\",\n",
+                "    \"Delta(1620)++\",\n",
+                "    \"Delta(1900)++\",\n",
+                "    \"Delta(1910)++\",\n",
+                "    \"Delta(1920)++\",\n",
+                "    \"Lambda(1800)\",\n",
+                "    \"Lambda(1810)\",\n",
+                "    \"Lambda(1890)\",\n",
+                "]:\n",
+                "    PARTICLES.remove(PARTICLES[name])\n",
+                "STM = qrules.StateTransitionManager(\n",
+                "    initial_state=[\"Lambda(c)+\"],\n",
+                "    final_state=[\"p\", \"K-\", \"pi+\"],\n",
+                "    mass_conservation_factor=3,\n",
+                "    allowed_intermediate_particles=[\"K\", \"Delta\", \"Lambda\"],\n",
+                "    particle_db=PARTICLES,\n",
+                "    max_angular_momentum=2,\n",
+                "    formalism=\"canonical-helicity\",\n",
                 ")\n",
-                "\u039bc = PARTICLE_DB[\"Lambda(c)+\"]\n",
-                "p = PARTICLE_DB[\"p\"]\n",
-                "\u03c0 = PARTICLE_DB[\"pi+\"]\n",
-                "K = PARTICLE_DB[\"K-\"]\n",
-                "PARTICLE_TO_ID = {\u039bc: 0, p: 1, \u03c0: 2, K: 3}\n",
-                "Markdown(as_markdown_table(list(PARTICLE_TO_ID)))"
+                "STM.set_allowed_interaction_types([qrules.InteractionType.STRONG], node_id=1)\n",
+                "problem_sets = STM.create_problem_sets()\n",
+                "REACTION = STM.find_solutions(problem_sets)\n",
+                "REACTION = normalize_state_ids(REACTION)\n",
+                "dot = qrules.io.asdot(REACTION, collapse_graphs=True)\n",
+                "graphviz.Source(dot)"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -100,30 +107,16 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "resonance_names = [\n",
-                "    \"Lambda(1405)\",\n",
-                "    \"Lambda(1520)\",\n",
-                "    \"Lambda(1600)\",\n",
-                "    \"Lambda(1670)\",\n",
-                "    \"Lambda(1690)\",\n",
-                "    \"Lambda(2000)\",\n",
-                "    \"Delta(1232)+\",\n",
-                "    \"Delta(1600)+\",\n",
-                "    \"Delta(1700)+\",\n",
-                "    \"K(0)*(700)+\",\n",
-                "    \"K*(892)0\",\n",
-                "    \"K(2)*(1430)0\",\n",
-                "]\n",
-                "resonances = [PARTICLE_DB[name] for name in resonance_names]\n",
-                "Markdown(as_markdown_table(resonances))"
+                "DECAY = to_three_body_decay(REACTION.transitions, min_ls=True)\n",
+                "Markdown(as_markdown_table([DECAY.initial_state, *DECAY.final_state.values()]))"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {
                 "jupyter": {
@@ -131,86 +124,32 @@
                 },
                 "tags": [
                     "hide-input"
                 ]
             },
             "outputs": [],
             "source": [
-                "def load_three_body_decay(\n",
-                "    resonance_names: Iterable[str],\n",
-                "    particle_definitions: dict[str, Particle],\n",
-                "    min_ls: bool = True,\n",
-                ") -> ThreeBodyDecay:\n",
-                "    resonances = [particle_definitions[name] for name in resonance_names]\n",
-                "    chains: list[ThreeBodyDecayChain] = []\n",
-                "    for res in resonances:\n",
-                "        chains.extend(_create_isobar(res, min_ls))\n",
-                "    return ThreeBodyDecay(\n",
-                "        states={state_id: particle for particle, state_id in PARTICLE_TO_ID.items()},\n",
-                "        chains=tuple(chains),\n",
-                "    )\n",
-                "\n",
-                "\n",
-                "def _create_isobar(resonance: Particle, min_ls: bool) -> list[ThreeBodyDecayChain]:\n",
-                "    if resonance.name.startswith(\"K\"):\n",
-                "        child1, child2, spectator = \u03c0, K, p\n",
-                "    elif resonance.name.startswith(\"L\"):\n",
-                "        child1, child2, spectator = K, p, \u03c0\n",
-                "    elif resonance.name.startswith(\"D\"):\n",
-                "        child1, child2, spectator = p, \u03c0, K\n",
-                "    else:\n",
-                "        raise NotImplementedError\n",
-                "    prod_ls_couplings = _generate_ls(\u039bc, resonance, spectator, conserve_parity=False)\n",
-                "    dec_ls_couplings = _generate_ls(resonance, child1, child2, conserve_parity=True)\n",
-                "    if min_ls:\n",
-                "        decay = IsobarNode(\n",
-                "            parent=\u039bc,\n",
-                "            child1=IsobarNode(\n",
-                "                parent=resonance,\n",
-                "                child1=child1,\n",
-                "                child2=child2,\n",
-                "                interaction=min(dec_ls_couplings),\n",
-                "            ),\n",
-                "            child2=spectator,\n",
-                "            interaction=min(prod_ls_couplings),\n",
-                "        )\n",
-                "        return [ThreeBodyDecayChain(decay)]\n",
-                "    chains = []\n",
-                "    for dec_ls, prod_ls in itertools.product(dec_ls_couplings, prod_ls_couplings):\n",
-                "        decay = IsobarNode(\n",
-                "            parent=\u039bc,\n",
-                "            child1=IsobarNode(\n",
-                "                parent=resonance,\n",
-                "                child1=child1,\n",
-                "                child2=child2,\n",
-                "                interaction=dec_ls,\n",
-                "            ),\n",
-                "            child2=spectator,\n",
-                "            interaction=prod_ls,\n",
-                "        )\n",
-                "        chains.append(ThreeBodyDecayChain(decay))\n",
-                "    return chains\n",
-                "\n",
-                "\n",
-                "def _generate_ls(\n",
-                "    parent: Particle, child1: Particle, child2: Particle, conserve_parity: bool\n",
-                ") -> list[tuple[int, sp.Rational]]:\n",
-                "    ls = generate_ls_couplings(parent.spin, child1.spin, child2.spin)\n",
-                "    if conserve_parity:\n",
-                "        return filter_parity_violating_ls(\n",
-                "            ls, parent.parity, child1.parity, child2.parity\n",
-                "        )\n",
-                "    return ls\n",
-                "\n",
-                "\n",
-                "DECAY = load_three_body_decay(\n",
-                "    resonance_names,\n",
-                "    particle_definitions=PARTICLE_DB,\n",
-                "    min_ls=True,\n",
+                "resonances = sorted(\n",
+                "    {t.resonance for t in DECAY.chains},\n",
+                "    key=lambda p: (p.name[0], p.mass),\n",
                 ")\n",
+                "resonance_names = [p.name for p in resonances]\n",
+                "Markdown(as_markdown_table(resonances))"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "metadata": {
+                "tags": [
+                    "hide-input"
+                ]
+            },
+            "outputs": [],
+            "source": [
                 "Latex(aslatex(DECAY, with_jp=True))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -252,21 +191,23 @@
             },
             "outputs": [],
             "source": [
                 "def formulate_breit_wigner(\n",
                 "    decay_chain: ThreeBodyDecayChain,\n",
                 ") -> tuple[BreitWignerMinL, dict[sp.Symbol, float]]:\n",
                 "    s = _get_mandelstam_s(decay_chain)\n",
-                "    child1_mass, child2_mass = map(_to_mass_symbol, decay_chain.decay_products)\n",
+                "    child1_mass, child2_mass = map(_create_mass_symbol, decay_chain.decay_products)\n",
                 "    l_dec = sp.Rational(decay_chain.outgoing_ls.L)\n",
                 "    l_prod = sp.Rational(decay_chain.incoming_ls.L)\n",
-                "    parent_mass = sp.Symbol(f\"m_{{{decay_chain.parent.latex}}}\")\n",
-                "    spectator_mass = sp.Symbol(f\"m_{{{decay_chain.spectator.latex}}}\")\n",
-                "    resonance_mass = sp.Symbol(f\"m_{{{decay_chain.resonance.latex}}}\")\n",
-                "    resonance_width = sp.Symbol(Rf\"\\Gamma_{{{decay_chain.resonance.latex}}}\")\n",
+                "    parent_mass = sp.Symbol(f\"m_{{{decay_chain.parent.latex}}}\", nonnegative=True)\n",
+                "    spectator_mass = sp.Symbol(f\"m_{{{decay_chain.spectator.latex}}}\", nonnegative=True)\n",
+                "    resonance_mass = sp.Symbol(f\"m_{{{decay_chain.resonance.latex}}}\", nonnegative=True)\n",
+                "    resonance_width = sp.Symbol(\n",
+                "        Rf\"\\Gamma_{{{decay_chain.resonance.latex}}}\", nonnegative=True\n",
+                "    )\n",
                 "    R_dec = sp.Symbol(R\"R_\\mathrm{res}\")\n",
                 "    R_prod = sp.Symbol(R\"R_{\\Lambda_c}\")\n",
                 "    parameter_defaults = {\n",
                 "        parent_mass: decay_chain.parent.mass,\n",
                 "        spectator_mass: decay_chain.spectator.mass,\n",
                 "        resonance_mass: decay_chain.resonance.mass,\n",
                 "        resonance_width: decay_chain.resonance.width,\n",
@@ -288,33 +229,36 @@
                 "        l_prod,\n",
                 "        R_dec,\n",
                 "        R_prod,\n",
                 "    )\n",
                 "    return dynamics, parameter_defaults\n",
                 "\n",
                 "\n",
-                "def _get_mandelstam_s(decay: ThreeBodyDecayChain) -> sp.Symbol:\n",
+                "def _create_mass_symbol(particle: IsobarNode | Particle) -> sp.Symbol:\n",
+                "    particle = get_particle(particle)\n",
+                "    return sp.Symbol(f\"m_{{{particle.latex}}}\", nonnegative=True)\n",
+                "\n",
+                "\n",
+                "def _get_mandelstam_s(decay: ThreeBodyDecayChain | IsobarNode) -> sp.Symbol:\n",
                 "    s1, s2, s3 = sp.symbols(\"sigma1:4\", nonnegative=True)\n",
-                "    m1, m2, m3 = map(_to_mass_symbol, [p, \u03c0, K])\n",
-                "    decay_masses = {_to_mass_symbol(p) for p in decay.decay_products}\n",
-                "    if decay_masses == {m2, m3}:\n",
+                "    decay_products = {p.name for p in _get_decay_products(decay)}\n",
+                "    if decay_products == {\"p\", \"pi+\"}:\n",
                 "        return s1\n",
-                "    if decay_masses == {m1, m3}:\n",
+                "    if decay_products == {\"pi+\", \"K-\"}:\n",
                 "        return s2\n",
-                "    if decay_masses == {m1, m2}:\n",
+                "    if decay_products == {\"K-\", \"p\"}:\n",
                 "        return s3\n",
-                "    msg = f\"Cannot find Mandelstam variable for {''.join(decay_masses)}\"\n",
+                "    msg = f\"Cannot find Mandelstam variable for {', '.join(decay_products)}\"\n",
                 "    raise NotImplementedError(msg)\n",
                 "\n",
                 "\n",
-                "def _to_mass_symbol(particle: Particle) -> sp.Symbol:\n",
-                "    state_id = PARTICLE_TO_ID.get(particle)\n",
-                "    if state_id is not None:\n",
-                "        return sp.Symbol(f\"m{state_id}\", nonnegative=True)\n",
-                "    return sp.Symbol(f\"m_{{{particle.latex}}}\", nonnegative=True)"
+                "def _get_decay_products(decay: ThreeBodyDecayChain | IsobarNode) -> list[Particle]:\n",
+                "    if isinstance(decay, ThreeBodyDecayChain):\n",
+                "        return decay.decay_products\n",
+                "    return decay.children"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Model formulation"
@@ -367,13 +311,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.8.17"
+            "version": "3.9.19"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `ampform-dpd-0.1.6/docs/references.bib` & `ampform_dpd-0.1.7/docs/references.bib`

 * *Files identical despite different names*

### Comparing `ampform-dpd-0.1.6/pyproject.toml` & `ampform_dpd-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     "Topic :: Scientific/Engineering",
     "Typing :: Typed",
 ]
 dependencies = [
     "ampform >=0.14.8", # Kibble and Kallen functions, perform_cached_doit, @unevaluated
     "attrs >=20.1.0", # on_setattr and https://www.attrs.org/en/stable/api.html#next-gen
     "cloudpickle",
+    "qrules >=0.10.0",
     "sympy >=1.10", # module sympy.printing.numpy and array expressions with shape kwarg
     "tensorwaves[jax]",
 ]
 description = "Symbolic expressions for Dalitz-Plot Decomposition"
 dynamic = ["version"]
 license = {text = "GPLv3 or later"}
 name = "ampform-dpd"
@@ -81,14 +82,15 @@
     "python-lsp-server[rope]",
 ]
 numba = [
     "tensorwaves[numba]",
 ]
 sty = [
     "ampform-dpd[types]",
+    "mypy",
     "pre-commit >=1.4.0",
     "ruff",
 ]
 tensorflow = [
     "ampform-dpd[tf]",
 ]
 test = [
@@ -129,14 +131,29 @@
 [tool.setuptools.packages.find]
 namespaces = false
 where = ["src"]
 
 [tool.setuptools_scm]
 write_to = "src/ampform_dpd/version.py"
 
+[tool.mypy]
+exclude = "_build"
+show_error_codes = true
+warn_unused_configs = true
+
+[[tool.mypy.overrides]]
+ignore_missing_imports = true
+module = ["cloudpickle.*"]
+
+[[tool.mypy.overrides]]
+check_untyped_defs = true
+disallow_incomplete_defs = false
+disallow_untyped_defs = false
+module = ["tests.*"]
+
 [tool.pyright]
 reportArgumentType = false
 reportAssignmentType = false
 reportAttributeAccessIssue = false
 reportCallIssue = false
 reportGeneralTypeIssues = false
 reportImportCycles = false
```

### Comparing `ampform-dpd-0.1.6/src/ampform_dpd/__init__.py` & `ampform_dpd-0.1.7/src/ampform_dpd/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,30 +18,31 @@
 from ampform_dpd.decay import (
     IsobarNode,
     LSCoupling,
     Particle,
     ThreeBodyDecay,
     ThreeBodyDecayChain,
     get_decay_product_ids,
+    get_particle,
 )
 from ampform_dpd.io import (
     simplify_latex_rendering,  # noqa: F401  # pyright:ignore[reportUnusedImport]
 )
 from ampform_dpd.spin import create_spin_range
 
 
 @frozen
 class AmplitudeModel:
     decay: ThreeBodyDecay
     intensity: sp.Expr = sp.S.One
     amplitudes: dict[sp.Indexed, sp.Expr] = field(factory=dict)
     variables: dict[sp.Symbol, sp.Expr] = field(factory=dict)
-    parameter_defaults: dict[sp.Symbol, float] = field(factory=dict)
-    masses: dict[sp.Symbol, float] = field(factory=dict)
-    invariants: dict[sp.Symbol, float] = field(factory=dict)
+    parameter_defaults: dict[sp.Symbol, float | complex] = field(factory=dict)
+    masses: dict[sp.Symbol, float | complex] = field(factory=dict)
+    invariants: dict[sp.Symbol, sp.Expr] = field(factory=dict)
 
     @property
     def full_expression(self) -> sp.Expr:
         return self.intensity.doit().xreplace(self.amplitudes)
 
 
 class DalitzPlotDecompositionBuilder:
@@ -75,42 +76,45 @@
             raise NotImplementedError(msg, min_ls)
 
     def formulate(
         self,
         reference_subsystem: Literal[1, 2, 3] = 1,
         cleanup_summations: bool = False,
     ) -> AmplitudeModel:
-        helicity_symbols = sp.symbols("lambda:4", rational=True)
+        helicity_symbols: tuple[sp.Symbol, sp.Symbol, sp.Symbol, sp.Symbol] = (
+            sp.symbols("lambda:4", rational=True)
+        )
         allowed_helicities = {
-            symbol: create_spin_range(self.decay.states[i].spin)
+            symbol: create_spin_range(self.decay.states[i].spin)  # type:ignore[index]
             for i, symbol in enumerate(helicity_symbols)
         }
         amplitude_definitions = {}
         angle_definitions = {}
         parameter_defaults = {}
-        for args in product(*allowed_helicities.values()):
-            for sub_system in [1, 2, 3]:
-                chain_model = self.formulate_subsystem_amplitude(*args, sub_system)
+        args: tuple[sp.Rational, sp.Rational, sp.Rational, sp.Rational]
+        for args in product(*allowed_helicities.values()):  # type:ignore[assignment]
+            for sub_system in (1, 2, 3):
+                chain_model = self.formulate_subsystem_amplitude(*args, sub_system)  # type:ignore[arg-type]
                 amplitude_definitions.update(chain_model.amplitudes)
                 angle_definitions.update(chain_model.variables)
                 parameter_defaults.update(chain_model.parameter_defaults)
         aligned_amp, zeta_defs = self.formulate_aligned_amplitude(
             *helicity_symbols, reference_subsystem
         )
         angle_definitions.update(zeta_defs)
         masses = create_mass_symbol_mapping(self.decay)
         parameter_defaults.update(masses)
         if cleanup_summations:
-            aligned_amp = aligned_amp.cleanup()
+            aligned_amp = aligned_amp.cleanup()  # type:ignore[assignment]
         intensity = PoolSum(
             sp.Abs(aligned_amp) ** 2,
             *allowed_helicities.items(),
         )
         if cleanup_summations:
-            intensity = intensity.cleanup()
+            intensity = intensity.cleanup()  # type:ignore[assignment]
         return AmplitudeModel(
             decay=self.decay,
             intensity=PoolSum(
                 sp.Abs(aligned_amp) ** 2,
                 *allowed_helicities.items(),
             ),
             amplitudes=amplitude_definitions,
@@ -161,16 +165,16 @@
                 h_dec = _create_coupling_symbol(
                     self.use_decay_helicity_couplings,
                     resonance=R,
                     helicities=(λ[i], λ[j]),
                     interaction=chain.outgoing_ls,
                     typ="decay",
                 )
-                parameter_defaults[h_prod] = 1 + 0j
-                parameter_defaults[h_dec] = 1
+                parameter_defaults[h_prod] = 1 + 0j  # type:ignore[index]
+                parameter_defaults[h_dec] = 1  # type:ignore[index]
             sub_amp_expr = (
                 sp.KroneckerDelta(λ[0], λR - λ[k])
                 * (-1) ** (spin[k] - λ[k])
                 * dynamics
                 * Wigner.d(resonance_spin, λR, λ[i] - λ[j], θij)
                 * _create_coupling_symbol(
                     self.use_production_helicity_couplings,
@@ -185,17 +189,16 @@
                     helicities=(λ[i], λ[j]),
                     interaction=chain.outgoing_ls,
                     typ="decay",
                 )
                 * (-1) ** (spin[j] - λ[j])
             )
             if not self.use_decay_helicity_couplings:
-                resonance_isobar = chain.decay.child1
                 sub_amp_expr *= _formulate_clebsch_gordan_factors(
-                    resonance_isobar,
+                    chain.decay_node,
                     helicities={
                         self.decay.final_state[i]: λ[i],
                         self.decay.final_state[j]: λ[j],
                     },
                 )
             if not self.use_production_helicity_couplings:
                 production_isobar = chain.decay
@@ -251,28 +254,31 @@
             * wigner_generator(j2, _λ2, λ2, rotated_state=2, aligned_subsystem=3)
             * wigner_generator(j3, _λ3, λ3, rotated_state=3, aligned_subsystem=3),
             (_λ0, create_spin_range(j0)),
             (_λ1, create_spin_range(j1)),
             (_λ2, create_spin_range(j2)),
             (_λ3, create_spin_range(j3)),
         )
-        return amp_expr, wigner_generator.angle_definitions
+        return amp_expr, wigner_generator.angle_definitions  # type:ignore[return-value]
 
 
 def _create_coupling_symbol(
     helicity_coupling: bool,
     resonance: Str,
     helicities: tuple[sp.Basic, sp.Basic],
-    interaction: LSCoupling,
+    interaction: LSCoupling | None,
     typ: Literal["production", "decay"],
 ) -> sp.Indexed:
     H = _get_coupling_base(helicity_coupling, typ)
     if helicity_coupling:
         λi, λj = helicities
         return H[resonance, λi, λj]
+    if interaction is None:
+        msg = "Cannot formulate LS-coupling without LS combinations"
+        raise ValueError(msg)
     return H[resonance, interaction.L, interaction.S]
 
 
 @lru_cache(maxsize=None)
 def _get_coupling_base(
     helicity_coupling: bool, typ: Literal["production", "decay"]
 ) -> sp.IndexedBase:
@@ -286,16 +292,16 @@
     helicities: dict[Particle, sp.Rational | sp.Symbol],
 ) -> sp.Expr:
     if isobar.interaction is None:
         msg = "Cannot formulate amplitude model in LS-basis if LS-couplings are missing"
         raise ValueError(msg)
     # https://github.com/ComPWA/ampform/blob/65b4efa/src/ampform/helicity/__init__.py#L785-L802
     # and supplementary material p.1 (https://cds.cern.ch/record/2824328/files)
-    child1 = _get_particle(isobar.child1)
-    child2 = _get_particle(isobar.child2)
+    child1 = get_particle(isobar.child1)
+    child2 = get_particle(isobar.child2)
     child1_helicity = helicities[child1]
     child2_helicity = helicities[child2]
     cg_ss = CG(
         j1=child1.spin,
         m1=child1_helicity,
         j2=child2.spin,
         m2=-child2_helicity,
@@ -310,35 +316,29 @@
         j3=isobar.parent.spin,
         m3=child1_helicity - child2_helicity,
     )
     sqrt_factor = sp.sqrt((2 * isobar.interaction.L + 1) / (2 * isobar.parent.spin + 1))
     return sqrt_factor * cg_ll * cg_ss
 
 
-def _get_particle(isobar: IsobarNode | Particle) -> Particle:
-    if isinstance(isobar, IsobarNode):
-        return isobar.parent
-    return isobar
-
-
 @lru_cache(maxsize=None)
 def _generate_amplitude_index_bases() -> dict[Literal[1, 2, 3], sp.IndexedBase]:
-    return dict(enumerate(sp.symbols(R"A^(1:4)", cls=sp.IndexedBase), 1))
+    return dict(enumerate(sp.symbols(R"A^(1:4)", cls=sp.IndexedBase), 1))  # type:ignore[arg-type]
 
 
 class _AlignmentWignerGenerator:
     def __init__(self, reference_subsystem: Literal[1, 2, 3] = 1) -> None:
         self.angle_definitions: dict[sp.Symbol, sp.acos] = {}
         self.reference_subsystem = reference_subsystem
 
     def __call__(
         self,
         j: sp.Rational,
-        m: sp.Rational,
-        m_prime: sp.Rational,
+        m: sp.Rational | sp.Symbol,
+        m_prime: sp.Rational | sp.Symbol,
         rotated_state: int,
         aligned_subsystem: int,
     ) -> sp.Rational | WignerD:
         if j == 0:
             return sp.Rational(1)
         zeta, zeta_expr = formulate_zeta_angle(
             rotated_state, aligned_subsystem, self.reference_subsystem
@@ -376,26 +376,28 @@
     def decay(self) -> ThreeBodyDecay:
         return self.__decay
 
 
 class DynamicsBuilder(Protocol):
     def __call__(
         self, decay_chain: ThreeBodyDecayChain
-    ) -> tuple[sp.Expr, dict[sp.Symbol, float]]: ...
+    ) -> tuple[sp.Expr, dict[sp.Symbol, float | complex]]: ...
 
 
 def formulate_non_resonant(
     decay_chain: ThreeBodyDecayChain,
-) -> tuple[sp.Expr, dict[sp.Symbol, float]]:
+) -> tuple[sp.Expr, dict[sp.Symbol, float | complex]]:
     return sp.Rational(1), {}
 
 
-def create_mass_symbol_mapping(decay: ThreeBodyDecay) -> dict[sp.Symbol, float]:
+def create_mass_symbol_mapping(
+    decay: ThreeBodyDecay,
+) -> dict[sp.Symbol, float | complex]:
     return {
-        sp.Symbol(f"m{i}"): decay.states[i].mass
+        sp.Symbol(f"m{i}", nonnegative=True): decay.states[i].mass
         for i in sorted(decay.states)  # ensure that dict keys are sorted by state ID
     }
 
 
 def formulate_invariants(decay: ThreeBodyDecay) -> dict[sp.Symbol, sp.Expr]:
     s1, s2, s3 = sp.symbols("sigma1:4", nonnegative=True)
     return {
```

### Comparing `ampform-dpd-0.1.6/src/ampform_dpd/_cache.py` & `ampform_dpd-0.1.7/src/ampform_dpd/_cache.py`

 * *Files identical despite different names*

### Comparing `ampform-dpd-0.1.6/src/ampform_dpd/angles.py` & `ampform_dpd-0.1.7/src/ampform_dpd/angles.py`

 * *Files identical despite different names*

### Comparing `ampform-dpd-0.1.6/src/ampform_dpd/dynamics.py` & `ampform_dpd-0.1.7/src/ampform_dpd/dynamics/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,50 @@
 """Functions for dynamics lineshapes and kinematics."""
 
 from __future__ import annotations
 
 from typing import Any
 
 import sympy as sp
+from ampform.dynamics import formulate_form_factor
 from ampform.kinematics.phasespace import Kallen
 from ampform.sympy import unevaluated
 
 
 @unevaluated
+class RelativisticBreitWigner(sp.Expr):
+    s: Any
+    mass0: Any
+    gamma0: Any
+    m1: Any
+    m2: Any
+    angular_momentum: Any
+    meson_radius: Any
+    _latex_repr_ = (
+        R"\mathcal{{R}}_{{{angular_momentum}}}\left({s}, {mass0}, {gamma0}\right)"
+    )
+
+    def evaluate(self):
+        from ampform.dynamics import EnergyDependentWidth  # noqa: PLC0415
+
+        s, m0, w0, m1, m2, angular_momentum, meson_radius = self.args
+        width = EnergyDependentWidth(
+            s=s,
+            mass0=m0,
+            gamma0=w0,
+            m_a=m1,
+            m_b=m2,
+            angular_momentum=angular_momentum,
+            meson_radius=meson_radius,
+            name=Rf"\Gamma_{{{sp.latex(angular_momentum)}}}",
+        )
+        return (m0 * w0) / (m0**2 - s - width * m0 * sp.I)
+
+
+@unevaluated
 class P(sp.Expr):
     s: Any
     mi: Any
     mj: Any
     _latex_repr_ = R"p_{{{mi},{mj}}}\left({s}\right)"
 
     def evaluate(self):
@@ -140,13 +171,34 @@
     L: Any
     _latex_repr_ = R"F_{{{L}}}\left({z}\right)"
 
     def evaluate(self) -> sp.Piecewise:
         z, L = self.args
         cases = {
             0: 1,
-            1: 1 / (1 + z**2),
-            2: 1 / (9 + 3 * z**2 + z**4),
+            1: 1 / (1 + z**2),  # type:ignore[operator]
+            2: 1 / (9 + 3 * z**2 + z**4),  # type:ignore[operator]
         }
         return sp.Piecewise(*[
             (sp.sqrt(expr), sp.Eq(L, l_val)) for l_val, expr in cases.items()
         ])
+
+
+@unevaluated
+class FormFactor(sp.Expr):
+    s: Any
+    m1: Any
+    m2: Any
+    angular_momentum: Any
+    meson_radius: Any
+
+    _latex_repr_ = R"\mathcal{{F}}_{{{angular_momentum}}}\left({s}, {m1}, {m2}\right)"
+
+    def evaluate(self):
+        s, m1, m2, angular_momentum, meson_radius = self.args
+        return formulate_form_factor(
+            s=s,
+            m_a=m1,
+            m_b=m2,
+            angular_momentum=angular_momentum,
+            meson_radius=meson_radius,
+        )
```

### Comparing `ampform-dpd-0.1.6/src/ampform_dpd/io.py` & `ampform_dpd-0.1.7/src/ampform_dpd/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from __future__ import annotations
 
 import logging
 import pickle
 from collections import abc
 from importlib.metadata import version
 from pathlib import Path
-from typing import TYPE_CHECKING, Iterable, Mapping, Sequence, overload
+from typing import TYPE_CHECKING, Any, Iterable, Mapping, Sequence, overload
 
 import cloudpickle
 import sympy as sp
 from ampform.io import aslatex
 from ampform.sympy import (
     perform_cached_doit,  # noqa: F401  # pyright:ignore[reportUnusedImport]
 )
@@ -132,19 +132,19 @@
     else:
         spin = Rf"\frac{{{particle.spin.numerator}}}{{{particle.spin.denominator}}}"
     return f"{spin}^{parity}"
 
 
 def as_markdown_table(obj: Sequence) -> str:
     """Render objects a `str` suitable for generating a table."""
+    if isinstance(obj, ThreeBodyDecay):
+        return _as_decay_markdown_table(obj.chains)
     item_type = _determine_item_type(obj)
     if item_type is Particle:
         return _as_resonance_markdown_table(obj)
-    if item_type is ThreeBodyDecay:
-        return _as_decay_markdown_table(obj.chains)
     if item_type is ThreeBodyDecayChain:
         return _as_decay_markdown_table(obj)
     msg = (
         f"Cannot render a sequence with {item_type.__name__} items as a Markdown table"
     )
     raise NotImplementedError(msg)
 
@@ -169,17 +169,17 @@
         "$J^P$",
         "mass (MeV)",
         "width (MeV)",
     ]
     src = _create_markdown_table_header(column_names)
     for particle in items:
         row_items = [
-            particle.name,
+            f"`{particle.name}`",
             f"${particle.latex}$",
-            Rf"${aslatex(particle, only_jp=True)}$",
+            Rf"${aslatex(particle, only_jp=True)}$",  # type:ignore[call-arg]
             f"{int(1e3 * particle.mass):,.0f}",
             f"{int(1e3 * particle.width):,.0f}",
         ]
         src += _create_markdown_table_row(row_items)
     return src
 
 
@@ -191,22 +191,24 @@
         R"width (MeV)",
         R"$L_\mathrm{dec}^\mathrm{min}$",
         R"$L_\mathrm{prod}^\mathrm{min}$",
     ]
     src = _create_markdown_table_header(column_names)
     for chain in decay_chains:
         child1, child2 = map(aslatex, chain.decay_products)
-        row_items = [
+        row_items: list = [
             Rf"${chain.resonance.latex} \to {child1} {child2}$",
-            Rf"${aslatex(chain.resonance, only_jp=True)}$",
+            Rf"${aslatex(chain.resonance, only_jp=True)}$",  # type:ignore[call-arg]
             f"{int(1e3 * chain.resonance.mass):,.0f}",
             f"{int(1e3 * chain.resonance.width):,.0f}",
-            chain.outgoing_ls.L,
-            chain.incoming_ls.L,
         ]
+        if chain.outgoing_ls is not None:
+            row_items.append(chain.outgoing_ls.L)
+        if chain.incoming_ls is not None:
+            row_items.append(chain.incoming_ls.L)
         src += _create_markdown_table_row(row_items)
     return src
 
 
 def _create_markdown_table_header(column_names: list[str]):
     src = _create_markdown_table_row(column_names)
     src += _create_markdown_table_row(["---" for _ in column_names])
@@ -230,15 +232,15 @@
     expr: sp.Expr,
     parameters: Mapping[sp.Symbol, ParameterValue],
     backend: str = "jax",
     directory: str | None = None,
 ) -> ParametrizedBackendFunction: ...
 
 
-def perform_cached_lambdify(  # pyright: ignore[reportInconsistentOverload]
+def perform_cached_lambdify(  # type:ignore[misc]  # pyright:ignore[reportInconsistentOverload]
     expr: sp.Expr,
     parameters: Mapping[sp.Symbol, ParameterValue] | None = None,
     backend: str = "jax",
     cache_directory: Path | str | None = None,
 ) -> ParametrizedFunction | Function:
     """Lambdify a SymPy `~sympy.core.expr.Expr` and cache the result to disk.
 
@@ -270,26 +272,27 @@
         cache_directory = (
             Path(system_cache_dir) / "ampform_dpd" / f"{backend}-v{backend_version}"
         )
     if not isinstance(cache_directory, Path):
         cache_directory = Path(cache_directory)
     cache_directory.mkdir(exist_ok=True, parents=True)
     if parameters is None:
-        hash_obj = expr
+        hash_obj: Any = expr
     else:
         hash_obj = (
             expr,
             tuple((s, parameters[s]) for s in sorted(parameters, key=str)),
         )
     h = get_readable_hash(hash_obj)
     filename = cache_directory / f"{h}.pkl"
     if filename.exists():
         with open(filename, "rb") as f:
             return pickle.load(f)
     _LOGGER.warning(f"Cached function file {filename} not found, lambdifying...")
+    func: ParametrizedFunction | Function
     if parameters is None:
         func = create_function(expr, backend)
     else:
         func = create_parametrized_function(expr, parameters, backend)
     with open(filename, "wb") as f:
         cloudpickle.dump(func, f)
     return func
@@ -299,8 +302,8 @@
     """Improve LaTeX rendering of an `~sympy.tensor.indexed.Indexed` object."""
 
     def _print_Indexed_latex(self, printer, *args):  # noqa: N802
         base = printer._print(self.base)
         indices = ", ".join(map(printer._print, self.indices))
         return f"{base}_{{{indices}}}"
 
-    sp.Indexed._latex = _print_Indexed_latex
+    sp.Indexed._latex = _print_Indexed_latex  # type:ignore[attr-defined]
```

### Comparing `ampform-dpd-0.1.6/src/ampform_dpd/spin.py` & `ampform_dpd-0.1.7/src/ampform_dpd/spin.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 def create_spin_range(spin: SupportsFloat) -> list[sp.Rational]:
     """Create a range of allowed spin projections.
 
     >>> create_spin_range(1.5)
     [-3/2, -1/2, 1/2, 3/2]
     """
-    return create_rational_range(-spin, spin)
+    return create_rational_range(-float(spin), +float(spin))
 
 
 def create_rational_range(
     __from: SupportsFloat, __to: SupportsFloat
 ) -> list[sp.Rational]:
     """Create a range of rational numbers, especially useful for spin projections.
```

### Comparing `ampform-dpd-0.1.6/src/ampform_dpd.egg-info/PKG-INFO` & `ampform_dpd-0.1.7/src/ampform_dpd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampform-dpd
-Version: 0.1.6
+Version: 0.1.7
 Summary: Symbolic expressions for Dalitz-Plot Decomposition
 Author-email: Common Partial Wave Analysis <compwa-admin@ep1.rub.de>
 License: GPLv3 or later
 Project-URL: Changelog, https://github.com/ComPWA/ampform-dpd/releases
 Project-URL: Documentation, https://compwa.github.io/ampform-dpd
 Project-URL: Source, https://github.com/ComPWA/ampform-dpd
 Project-URL: Tracker, https://github.com/ComPWA/ampform-dpd/issues
@@ -26,14 +26,15 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ampform>=0.14.8
 Requires-Dist: attrs>=20.1.0
 Requires-Dist: cloudpickle
+Requires-Dist: qrules>=0.10.0
 Requires-Dist: sympy>=1.10
 Requires-Dist: tensorwaves[jax]
 Provides-Extra: dev
 Requires-Dist: ampform-dpd[doc]; extra == "dev"
 Requires-Dist: ampform-dpd[jupyter]; extra == "dev"
 Requires-Dist: ampform-dpd[sty]; extra == "dev"
 Requires-Dist: ampform-dpd[test]; extra == "dev"
@@ -69,14 +70,15 @@
 Requires-Dist: jupyterlab-myst; extra == "jupyter"
 Requires-Dist: python-lsp-ruff; extra == "jupyter"
 Requires-Dist: python-lsp-server[rope]; extra == "jupyter"
 Provides-Extra: numba
 Requires-Dist: tensorwaves[numba]; extra == "numba"
 Provides-Extra: sty
 Requires-Dist: ampform-dpd[types]; extra == "sty"
+Requires-Dist: mypy; extra == "sty"
 Requires-Dist: pre-commit>=1.4.0; extra == "sty"
 Requires-Dist: ruff; extra == "sty"
 Provides-Extra: tensorflow
 Requires-Dist: ampform-dpd[tf]; extra == "tensorflow"
 Provides-Extra: test
 Requires-Dist: nbmake; extra == "test"
 Requires-Dist: numpy; extra == "test"
```

### Comparing `ampform-dpd-0.1.6/src/ampform_dpd.egg-info/SOURCES.txt` & `ampform_dpd-0.1.7/src/ampform_dpd.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -40,20 +40,25 @@
 docs/comparison/jpsi2phipipi.ipynb
 docs/comparison/jpsi2pipipi.ipynb
 src/ampform_dpd/__init__.py
 src/ampform_dpd/_attrs.py
 src/ampform_dpd/_cache.py
 src/ampform_dpd/angles.py
 src/ampform_dpd/decay.py
-src/ampform_dpd/dynamics.py
 src/ampform_dpd/io.py
+src/ampform_dpd/particle-definitions.yml
 src/ampform_dpd/py.typed
 src/ampform_dpd/spin.py
 src/ampform_dpd/version.py
 src/ampform_dpd.egg-info/PKG-INFO
 src/ampform_dpd.egg-info/SOURCES.txt
 src/ampform_dpd.egg-info/dependency_links.txt
 src/ampform_dpd.egg-info/requires.txt
 src/ampform_dpd.egg-info/top_level.txt
+src/ampform_dpd/adapter/__init__.py
+src/ampform_dpd/adapter/qrules.py
+src/ampform_dpd/dynamics/__init__.py
 tests/test_angles.py
 tests/test_decay.py
-tests/test_io.py
+tests/test_io.py
+tests/adapter/__init__.py
+tests/adapter/test_qrules.py
```

### Comparing `ampform-dpd-0.1.6/src/ampform_dpd.egg-info/requires.txt` & `ampform_dpd-0.1.7/src/ampform_dpd.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ampform>=0.14.8
 attrs>=20.1.0
 cloudpickle
+qrules>=0.10.0
 sympy>=1.10
 tensorwaves[jax]
 
 [dev]
 ampform-dpd[doc]
 ampform-dpd[jupyter]
 ampform-dpd[sty]
@@ -46,14 +47,15 @@
 python-lsp-server[rope]
 
 [numba]
 tensorwaves[numba]
 
 [sty]
 ampform-dpd[types]
+mypy
 pre-commit>=1.4.0
 ruff
 
 [tensorflow]
 ampform-dpd[tf]
 
 [test]
```

### Comparing `ampform-dpd-0.1.6/tests/test_angles.py` & `ampform_dpd-0.1.7/tests/test_angles.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             _, ζi_ki = formulate_zeta_angle(i, k, i)
             _, ζi_kk = formulate_zeta_angle(i, k, k)
             assert ζi_ki == ζi_k0
             assert ζi_kk == 0
 
 
 @pytest.mark.parametrize(
-    ("ζ1", "ζ2", "ζ3"),
+    ("ζ1_expr", "ζ2_expr", "ζ3_expr"),
     [
         (
             formulate_zeta_angle(1, 2, 3)[1],
             formulate_zeta_angle(1, 2, 1)[1],
             formulate_zeta_angle(1, 1, 3)[1],
         ),
         (
@@ -64,18 +64,18 @@
         (
             formulate_zeta_angle(3, 1, 2)[1],
             formulate_zeta_angle(3, 1, 3)[1],
             formulate_zeta_angle(3, 3, 2)[1],
         ),
     ],
 )
-def test_formulate_zeta_angle_sum_rule(ζ1: sp.Expr, ζ2: sp.Expr, ζ3: sp.Expr):
+def test_formulate_zeta_angle_sum(ζ1_expr: sp.Expr, ζ2_expr: sp.Expr, ζ3_expr: sp.Expr):
     """Test Eq.
 
     (A9), https://journals.aps.org/prd/pdf/10.1103/PhysRevD.101.034033#page=11.
     """
     σ3_expr = compute_third_mandelstam(σ1, σ2, m0, m1, m2, m3)
     masses = {m0: 2.3, m1: 0.94, m2: 0.14, m3: 0.49, σ1: 1.2, σ2: 3.0, σ3: σ3_expr}
-    ζ1 = float(ζ1.doit().xreplace(masses).xreplace(masses))
-    ζ2 = float(ζ2.doit().xreplace(masses).xreplace(masses))
-    ζ3 = float(ζ3.doit().xreplace(masses).xreplace(masses))
+    ζ1 = float(ζ1_expr.doit().xreplace(masses).xreplace(masses))
+    ζ2 = float(ζ2_expr.doit().xreplace(masses).xreplace(masses))
+    ζ3 = float(ζ3_expr.doit().xreplace(masses).xreplace(masses))
     np.testing.assert_almost_equal(ζ1, ζ2 + ζ3, decimal=14)
```

### Comparing `ampform-dpd-0.1.6/tests/test_decay.py` & `ampform_dpd-0.1.7/tests/test_decay.py`

 * *Files identical despite different names*

### Comparing `ampform-dpd-0.1.6/tests/test_io.py` & `ampform_dpd-0.1.7/tests/test_io.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     if python_hash_seed is None or not python_hash_seed.isdigit():
         assert h[:7] == "bbc9833"
         if _warn_about_unsafe_hash.cache_info().hits == 0:
             assert "PYTHONHASHSEED has not been set." in caplog.text
             caplog.clear()
     elif python_hash_seed == "0":
         if sys.version_info < (3, 11):
-            expected_hash = expected_hash[0]
+            expected_hash = expected_hash[0]  # type:ignore[assignment]
         else:
             expected_hash = expected_hash[1]
         expected = f"pythonhashseed-0{expected_hash:+d}"
         assert h == expected
     else:
         pytest.skip("PYTHONHASHSEED has been set, but is not 0")
     assert not caplog.text
```

### Comparing `ampform-dpd-0.1.6/tox.ini` & `ampform_dpd-0.1.7/tox.ini`

 * *Files identical despite different names*

