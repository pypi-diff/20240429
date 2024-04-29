# Comparing `tmp/napari_psf_analysis-1.1.2.tar.gz` & `tmp/napari_psf_analysis-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_psf_analysis-1.1.2.tar", last modified: Thu Nov  9 08:53:08 2023, max compression
+gzip compressed data, was "napari_psf_analysis-1.1.3.tar", last modified: Mon Apr 29 08:04:36 2024, max compression
```

## Comparing `napari_psf_analysis-1.1.2.tar` & `napari_psf_analysis-1.1.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.302337 napari_psf_analysis-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.278337 napari_psf_analysis-1.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.282337 napari_psf_analysis-1.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/.github/workflows/documentation.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      168 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2023-11-09 08:53:08.302337 napari_psf_analysis-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.282337 napari_psf_analysis-1.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.282337 napari_psf_analysis-1.1.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.282337 napari_psf_analysis-1.1.2/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/docs/source/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/docs/source/license.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.282337 napari_psf_analysis-1.1.2/docs/source/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     4081 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/docs/source/resources/html_logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/docs/source/resources/html_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)    17037 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/docs/source/resources/logoipsum-258.svg
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/docs/source/setup.md
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.282337 napari_psf_analysis-1.1.2/figs/
--rw-r--r--   0 runner    (1001) docker     (127)  7453045 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/figs/napari-psf-analysis_demo.gif
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      220 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2023-11-09 08:53:08.302337 napari_psf_analysis-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.294337 napari_psf_analysis-1.1.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.294337 napari_psf_analysis-1.1.2/src/napari_psf_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25763 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_dock_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.294337 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.294337 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.294337 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/extract/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/extract/test_BeadExtractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.298337 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/fit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fit_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fit_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fit_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/test_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/test_psf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/test_dock_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-09 08:53:08.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.298337 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9530 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.298337 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/extract/
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/extract/BeadExtractor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/extract/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.298337 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/fit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/fit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/fit/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/fit/fit_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/fit/fit_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/fit/fit_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8222 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/fit/fitter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/image.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    21977 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/psf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/records.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.298337 napari_psf_analysis-1.1.2/src/napari_psf_analysis/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    36344 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/resources/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    14915 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis/resources/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 08:53:08.294337 napari_psf_analysis-1.1.2/src/napari_psf_analysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6446 2023-11-09 08:53:08.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2023-11-09 08:53:08.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 08:53:08.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-09 08:53:08.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-11-09 08:53:08.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-09 08:53:08.000000 napari_psf_analysis-1.1.2/src/napari_psf_analysis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      912 2023-11-09 08:52:52.000000 napari_psf_analysis-1.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.701293 napari_psf_analysis-1.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.677293 napari_psf_analysis-1.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.681293 napari_psf_analysis-1.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/.github/workflows/documentation.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-04-29 08:04:36.701293 napari_psf_analysis-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.681293 napari_psf_analysis-1.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.685293 napari_psf_analysis-1.1.3/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.685293 napari_psf_analysis-1.1.3/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/docs/source/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/docs/source/license.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.685293 napari_psf_analysis-1.1.3/docs/source/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/docs/source/resources/html_logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/docs/source/resources/html_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    17037 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/docs/source/resources/logoipsum-258.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/docs/source/setup.md
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.685293 napari_psf_analysis-1.1.3/figs/
+-rw-r--r--   0 runner    (1001) docker     (127)  7453045 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/figs/napari-psf-analysis_demo.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-29 08:04:36.701293 napari_psf_analysis-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.693293 napari_psf_analysis-1.1.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.693293 napari_psf_analysis-1.1.3/src/napari_psf_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25756 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_dock_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.697293 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.697293 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.697293 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/extract/test_BeadExtractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.697293 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/fit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fit_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fit_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fit_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/test_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/test_psf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/test_dock_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 08:04:36.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.697293 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9530 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.701293 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/extract/BeadExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/extract/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.701293 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/fit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/fit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/fit/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/fit/fit_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/fit/fit_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/fit/fit_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8222 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/fit/fitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21977 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/psf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/records.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.701293 napari_psf_analysis-1.1.3/src/napari_psf_analysis/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    36344 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/resources/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis/resources/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:04:36.701293 napari_psf_analysis-1.1.3/src/napari_psf_analysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-04-29 08:04:36.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-29 08:04:36.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 08:04:36.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-29 08:04:36.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-29 08:04:36.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-29 08:04:36.000000 napari_psf_analysis-1.1.3/src/napari_psf_analysis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-29 08:04:26.000000 napari_psf_analysis-1.1.3/tox.ini
```

### Comparing `napari_psf_analysis-1.1.2/.github/workflows/documentation.yaml` & `napari_psf_analysis-1.1.3/.github/workflows/documentation.yaml`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/.github/workflows/test_and_deploy.yml` & `napari_psf_analysis-1.1.3/.github/workflows/test_and_deploy.yml`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 jobs:
   test:
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
       matrix:
         platform: [ubuntu-latest, windows-latest, macos-latest]
-        python-version: ['3.8', '3.9', '3.10']
+        python-version: ['3.9', '3.10', '3.11']
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
```

### Comparing `napari_psf_analysis-1.1.2/.gitignore` & `napari_psf_analysis-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/.pre-commit-config.yaml` & `napari_psf_analysis-1.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/LICENSE` & `napari_psf_analysis-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/PKG-INFO` & `napari_psf_analysis-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari_psf_analysis
-Version: 1.1.2
+Version: 1.1.3
 Summary: A plugin to analyse point spread functions (PSFs).
 Home-page: https://github.com/fmi-faim/napari-psf-analysis.git
 Author: Tim-Oliver Buchholz
 Author-email: tim-oliver.buchholz@fmi.ch
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/fmi-faim/napari-psf-analysis/issues
 Project-URL: Documentation, https://github.com/fmi-faim/napari-psf-analysis#README.md
@@ -15,15 +15,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bfio
 Requires-Dist: matplotlib
 Requires-Dist: matplotlib-scalebar
 Requires-Dist: napari
 Requires-Dist: numpy
```

### Comparing `napari_psf_analysis-1.1.2/README.md` & `napari_psf_analysis-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/docs/Makefile` & `napari_psf_analysis-1.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/docs/make.bat` & `napari_psf_analysis-1.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/docs/source/conf.py` & `napari_psf_analysis-1.1.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/docs/source/resources/html_logo.png` & `napari_psf_analysis-1.1.3/docs/source/resources/html_logo.png`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/docs/source/resources/html_logo.svg` & `napari_psf_analysis-1.1.3/docs/source/resources/html_logo.svg`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/docs/source/resources/logoipsum-258.svg` & `napari_psf_analysis-1.1.3/docs/source/resources/logoipsum-258.svg`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/figs/napari-psf-analysis_demo.gif` & `napari_psf_analysis-1.1.3/figs/napari-psf-analysis_demo.gif`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/setup.cfg` & `napari_psf_analysis-1.1.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 	bfio
 	matplotlib
 	matplotlib-scalebar
 	napari
 	numpy
 	pandas
 	scikit-image
-python_requires = >=3.8
+python_requires = >=3.9
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = 
 	setuptools-scm
 
 [options.packages.find]
```

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/_dock_widget.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/_dock_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,15 @@
                     scale=measurement_scale,
                 )
                 self._viewer.dims.set_point(0, 0)
                 self._viewer.reset_view()
                 self.summary_figs = measurement_stack
             _reset_state()
 
-        def _update_progress(progress: float):
+        def _update_progress(progress: int):
             self.progressbar.setValue(progress)
             if self.cancel_extraction:
                 worker.quit()
 
         def _reset_state():
             if self.cancel_extraction:
                 self.progressbar.setValue(0)
@@ -492,17 +492,17 @@
         worker.start()
 
         self.extract_psfs.setEnabled(False)
         self.cancel.setEnabled(True)
 
     def _setup_progressbar(self, point_data):
         self.progressbar.reset()
-        self.progressbar.setMaximum(0)
+        self.progressbar.setMinimum(0)
         self.progressbar.setMaximum(len(point_data))
-        self.progressbar.setValue(0.0001)
+        self.progressbar.setValue(0)
 
     def _get_img_name(self):
         img_layer = None
         for layer in self._viewer.layers:
             if str(layer) == self.cbox_img.currentText():
                 img_layer = layer
```

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/extract/test_BeadExtractor.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/extract/test_BeadExtractor.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fit_1d.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fit_1d.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fit_2d.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fit_2d.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fit_3d.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fit_3d.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fitter.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/fit/test_fitter.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/test_analyzer.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/test_analyzer.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/test_psf.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/test_psf.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/psf_analysis/test_utils.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/psf_analysis/test_utils.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/_tests/test_dock_widget.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/_tests/test_dock_widget.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/analyzer.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/analyzer.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/extract/BeadExtractor.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/extract/BeadExtractor.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/fit/estimator.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/fit/estimator.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/fit/fit_1d.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/fit/fit_1d.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/fit/fit_2d.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/fit/fit_2d.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/fit/fit_3d.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/fit/fit_3d.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/fit/fitter.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/fit/fitter.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/image.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/image.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/parameters.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/parameters.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/psf.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/psf.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/records.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/records.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/sample.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/sample.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/psf_analysis/utils.py` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/psf_analysis/utils.py`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/resources/logo.png` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/resources/logo.png`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis/resources/logo.svg` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis/resources/logo.svg`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis.egg-info/PKG-INFO` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: napari-psf-analysis
-Version: 1.1.2
+Name: napari_psf_analysis
+Version: 1.1.3
 Summary: A plugin to analyse point spread functions (PSFs).
 Home-page: https://github.com/fmi-faim/napari-psf-analysis.git
 Author: Tim-Oliver Buchholz
 Author-email: tim-oliver.buchholz@fmi.ch
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/fmi-faim/napari-psf-analysis/issues
 Project-URL: Documentation, https://github.com/fmi-faim/napari-psf-analysis#README.md
@@ -15,15 +15,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bfio
 Requires-Dist: matplotlib
 Requires-Dist: matplotlib-scalebar
 Requires-Dist: napari
 Requires-Dist: numpy
```

### Comparing `napari_psf_analysis-1.1.2/src/napari_psf_analysis.egg-info/SOURCES.txt` & `napari_psf_analysis-1.1.3/src/napari_psf_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_psf_analysis-1.1.2/tox.ini` & `napari_psf_analysis-1.1.3/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # For more information about tox, see https://tox.readthedocs.io/en/latest/
 [tox]
-envlist = py{38,39,310}-{linux,macos,windows}
+envlist = py{39,310,311}-{linux,macos,windows}
 isolated_build=true
 
 [gh-actions]
 python =
-    3.8: py38
     3.9: py39
     3.10: py310
+    3.11: py311
 
 [gh-actions:env]
 PLATFORM =
     ubuntu-latest: linux
     macos-latest: macos
     windows-latest: windows
```

