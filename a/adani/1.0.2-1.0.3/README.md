# Comparing `tmp/adani-1.0.2.tar.gz` & `tmp/adani-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adani-1.0.2.tar", last modified: Mon Apr  8 16:54:31 2024, max compression
+gzip compressed data, was "adani-1.0.3.tar", last modified: Mon Apr 29 09:50:13 2024, max compression
```

## Comparing `adani-1.0.2.tar` & `adani-1.0.3.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.653259 adani-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-08 16:54:24.000000 adani-1.0.2/.clang-format
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 16:54:24.000000 adani-1.0.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.633259 adani-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.637259 adani-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-08 16:54:24.000000 adani-1.0.2/.github/workflows/pip.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-08 16:54:24.000000 adani-1.0.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-08 16:54:24.000000 adani-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-08 16:54:24.000000 adani-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-04-08 16:54:24.000000 adani-1.0.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-08 16:54:24.000000 adani-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-08 16:54:31.653259 adani-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-08 16:54:24.000000 adani-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.637259 adani-1.0.2/bin/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-08 16:54:24.000000 adani-1.0.2/bin/adani-config.in
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-08 16:54:24.000000 adani-1.0.2/bin/adani.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.641259 adani-1.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)  2182791 2024-04-08 16:54:24.000000 adani-1.0.2/docs/Tesi_Laurenti.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   150134 2024-04-08 16:54:24.000000 adani-1.0.2/docs/approximation_smallx_nll.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    21151 2024-04-08 16:54:24.000000 adani-1.0.2/docs/approximation_smallx_nll.tex
--rw-r--r--   0 runner    (1001) docker     (127)    98460 2024-04-08 16:54:24.000000 adani-1.0.2/docs/montecarlointegration.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-08 16:54:24.000000 adani-1.0.2/docs/montecarlointegration.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.641259 adani-1.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-08 16:54:24.000000 adani-1.0.2/examples/test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-08 16:54:24.000000 adani-1.0.2/examples/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.637259 adani-1.0.2/inc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.645259 adani-1.0.2/inc/adani/
--rw-r--r--   0 runner    (1001) docker     (127)     5681 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/ApproximateCoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/AsymptoticCoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/CoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/Constants.h
--rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/Convolution.h
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/ExactCoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)    11125 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/HighEnergyCoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/HighScaleCoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/HighScaleSplitLogs.h
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/MasslessCoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/MatchingCondition.h
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/SpecialFunctions.h
--rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/SplittingFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/ThresholdCoefficientFunction.h
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/Value.h
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24502 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/adani.h
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 16:54:24.000000 adani-1.0.2/inc/adani/version.h.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.653259 adani-1.0.2/inc/adani.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-08 16:54:31.000000 adani-1.0.2/inc/adani.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-08 16:54:31.000000 adani-1.0.2/inc/adani.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 16:54:31.000000 adani-1.0.2/inc/adani.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-08 16:54:31.000000 adani-1.0.2/inc/adani.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.645259 adani-1.0.2/output/
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-08 16:54:24.000000 adani-1.0.2/output/Q.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-08 16:54:24.000000 adani-1.0.2/output/output_grid.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-08 16:54:24.000000 adani-1.0.2/output/output_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.649259 adani-1.0.2/output/runcards/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 16:54:24.000000 adani-1.0.2/output/runcards/runcard_2g.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 16:54:24.000000 adani-1.0.2/output/runcards/runcard_2q.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 16:54:24.000000 adani-1.0.2/output/runcards/runcard_Lg.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 16:54:24.000000 adani-1.0.2/output/runcards/runcard_Lq.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-08 16:54:24.000000 adani-1.0.2/output/x.txt
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-08 16:54:24.000000 adani-1.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.649259 adani-1.0.2/pywrap/
--rw-r--r--   0 runner    (1001) docker     (127)    13346 2024-04-08 16:54:24.000000 adani-1.0.2/pywrap/pywrap.cc
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 16:54:31.653259 adani-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-08 16:54:24.000000 adani-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.653259 adani-1.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)    16310 2024-04-08 16:54:24.000000 adani-1.0.2/src/ApproximateCoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-08 16:54:24.000000 adani-1.0.2/src/AsymptoticCoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-04-08 16:54:24.000000 adani-1.0.2/src/CoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)    21313 2024-04-08 16:54:24.000000 adani-1.0.2/src/Convolution.cc
--rw-r--r--   0 runner    (1001) docker     (127)    22470 2024-04-08 16:54:24.000000 adani-1.0.2/src/ExactCoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)    45692 2024-04-08 16:54:24.000000 adani-1.0.2/src/HighEnergyCoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)   235407 2024-04-08 16:54:24.000000 adani-1.0.2/src/HighScaleCoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)   215112 2024-04-08 16:54:24.000000 adani-1.0.2/src/HighScaleSplitLogs.cc
--rw-r--r--   0 runner    (1001) docker     (127)   210010 2024-04-08 16:54:24.000000 adani-1.0.2/src/MasslessCoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)    47102 2024-04-08 16:54:24.000000 adani-1.0.2/src/MatchingCondition.cc
--rw-r--r--   0 runner    (1001) docker     (127)    12537 2024-04-08 16:54:24.000000 adani-1.0.2/src/SpecialFunctions.cc
--rw-r--r--   0 runner    (1001) docker     (127)    23998 2024-04-08 16:54:24.000000 adani-1.0.2/src/SplittingFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-08 16:54:24.000000 adani-1.0.2/src/ThresholdCoefficientFunction.cc
--rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-04-08 16:54:24.000000 adani-1.0.2/src/Value.cc
--rw-r--r--   0 runner    (1001) docker     (127)   546646 2024-04-08 16:54:24.000000 adani-1.0.2/src/hplog.f
--rw-r--r--   0 runner    (1001) docker     (127)   747023 2024-04-08 16:54:24.000000 adani-1.0.2/src/hqcoef.f
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 16:54:31.653259 adani-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_approx_coeff_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_asy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_exact_coeff_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_high_scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     8517 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_highenergy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_massless.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_mc_integral.py
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_splitting_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-08 16:54:24.000000 adani-1.0.2/tests/test_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-08 16:54:24.000000 adani-1.0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:50:13.758546 adani-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-29 09:50:08.000000 adani-1.0.3/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-29 09:50:08.000000 adani-1.0.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:50:13.742545 adani-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:50:13.742545 adani-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-29 09:50:08.000000 adani-1.0.3/.github/workflows/pip.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-29 09:50:08.000000 adani-1.0.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-29 09:50:08.000000 adani-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-29 09:50:08.000000 adani-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-29 09:50:08.000000 adani-1.0.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-29 09:50:08.000000 adani-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-29 09:50:13.758546 adani-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-04-29 09:50:08.000000 adani-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:50:13.742545 adani-1.0.3/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-29 09:50:08.000000 adani-1.0.3/bin/adani-config.in
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-29 09:50:08.000000 adani-1.0.3/bin/adani.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:50:13.746545 adani-1.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)  2182791 2024-04-29 09:50:09.000000 adani-1.0.3/docs/Tesi_Laurenti.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   150134 2024-04-29 09:50:09.000000 adani-1.0.3/docs/approximation_smallx_nll.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    21151 2024-04-29 09:50:09.000000 adani-1.0.3/docs/approximation_smallx_nll.tex
+-rw-r--r--   0 runner    (1001) docker     (127)    98460 2024-04-29 09:50:09.000000 adani-1.0.3/docs/montecarlointegration.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-29 09:50:09.000000 adani-1.0.3/docs/montecarlointegration.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:50:13.746545 adani-1.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-29 09:50:09.000000 adani-1.0.3/examples/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-29 09:50:09.000000 adani-1.0.3/examples/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-29 09:50:09.000000 adani-1.0.3/format.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:50:13.742545 adani-1.0.3/inc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:50:13.750546 adani-1.0.3/inc/adani/
+-rw-r--r--   0 runner    (1001) docker     (127)     5765 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/ApproximateCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/AsymptoticCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2898 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/CoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/Constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/Convolution.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/ExactCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11053 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/HighEnergyCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5087 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/HighScaleCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/HighScaleSplitLogs.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/MasslessCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/MatchingCondition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/SpecialFunctions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/SplittingFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/ThresholdCoefficientFunction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/Value.h
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24502 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/adani.h
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-29 09:50:09.000000 adani-1.0.3/inc/adani/version.h.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:50:13.758546 adani-1.0.3/inc/adani.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-29 09:50:13.000000 adani-1.0.3/inc/adani.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-29 09:50:13.000000 adani-1.0.3/inc/adani.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 09:50:13.000000 adani-1.0.3/inc/adani.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 09:50:13.000000 adani-1.0.3/inc/adani.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:50:13.750546 adani-1.0.3/output/
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-29 09:50:09.000000 adani-1.0.3/output/Q.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11028 2024-04-29 09:50:09.000000 adani-1.0.3/output/output_grid.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10115 2024-04-29 09:50:09.000000 adani-1.0.3/output/output_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:50:13.754546 adani-1.0.3/output/runcards/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-29 09:50:09.000000 adani-1.0.3/output/runcards/runcard_2g.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-29 09:50:09.000000 adani-1.0.3/output/runcards/runcard_2q.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-29 09:50:09.000000 adani-1.0.3/output/runcards/runcard_Lg.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-29 09:50:09.000000 adani-1.0.3/output/runcards/runcard_Lq.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-29 09:50:09.000000 adani-1.0.3/output/x.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-29 09:50:09.000000 adani-1.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:50:13.754546 adani-1.0.3/pywrap/
+-rw-r--r--   0 runner    (1001) docker     (127)    19812 2024-04-29 09:50:09.000000 adani-1.0.3/pywrap/pywrap.cc
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 09:50:13.758546 adani-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-29 09:50:09.000000 adani-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:50:13.758546 adani-1.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    16616 2024-04-29 09:50:09.000000 adani-1.0.3/src/ApproximateCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-29 09:50:09.000000 adani-1.0.3/src/AsymptoticCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-29 09:50:09.000000 adani-1.0.3/src/CoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    20673 2024-04-29 09:50:09.000000 adani-1.0.3/src/Convolution.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    23537 2024-04-29 09:50:09.000000 adani-1.0.3/src/ExactCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    45684 2024-04-29 09:50:09.000000 adani-1.0.3/src/HighEnergyCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   235407 2024-04-29 09:50:09.000000 adani-1.0.3/src/HighScaleCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   215112 2024-04-29 09:50:09.000000 adani-1.0.3/src/HighScaleSplitLogs.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   210010 2024-04-29 09:50:09.000000 adani-1.0.3/src/MasslessCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    47004 2024-04-29 09:50:09.000000 adani-1.0.3/src/MatchingCondition.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    12537 2024-04-29 09:50:09.000000 adani-1.0.3/src/SpecialFunctions.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    31252 2024-04-29 09:50:09.000000 adani-1.0.3/src/SplittingFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-29 09:50:09.000000 adani-1.0.3/src/ThresholdCoefficientFunction.cc
+-rw-r--r--   0 runner    (1001) docker     (127)     7172 2024-04-29 09:50:09.000000 adani-1.0.3/src/Value.cc
+-rw-r--r--   0 runner    (1001) docker     (127)   546646 2024-04-29 09:50:09.000000 adani-1.0.3/src/hplog.f
+-rw-r--r--   0 runner    (1001) docker     (127)   747023 2024-04-29 09:50:09.000000 adani-1.0.3/src/hqcoef.f
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 09:50:13.758546 adani-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-04-29 09:50:09.000000 adani-1.0.3/tests/test_approx_coeff_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-04-29 09:50:09.000000 adani-1.0.3/tests/test_asy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-29 09:50:09.000000 adani-1.0.3/tests/test_exact_coeff_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2024-04-29 09:50:09.000000 adani-1.0.3/tests/test_high_scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-04-29 09:50:09.000000 adani-1.0.3/tests/test_highenergy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-04-29 09:50:09.000000 adani-1.0.3/tests/test_massless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-29 09:50:09.000000 adani-1.0.3/tests/test_mc_integral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-29 09:50:09.000000 adani-1.0.3/tests/test_splitting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-29 09:50:09.000000 adani-1.0.3/tests/test_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-29 09:50:09.000000 adani-1.0.3/versioneer.py
```

### Comparing `adani-1.0.2/.clang-format` & `adani-1.0.3/.clang-format`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/.github/workflows/pip.yml` & `adani-1.0.3/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/.github/workflows/tests.yml` & `adani-1.0.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/CMakeLists.txt` & `adani-1.0.3/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # define project name and its language
 project(adani)
 
 # define c++ standard and issue all the warning demanded by this standard
 set(CMAKE_CXX_STANDARD 14)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Wextra -fPIC")
-# set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Wextra -fPIC -lgsl -lgslcblas -lm")
+
 enable_language(Fortran)
 set(CMAKE_Fortran_FLAGS "${CMAKE_Fortran_FLAGS} -fPIC")
 
 if (NOT DEFINED CMAKE_MACOSX_RPATH)
     set(CMAKE_MACOSX_RPATH 0)
 endif()
 
@@ -84,16 +84,15 @@
         src/MasslessCoefficientFunction.cc
         src/MatchingCondition.cc
         src/SpecialFunctions.cc
         src/SplittingFunction.cc
         src/ThresholdCoefficientFunction.cc
         src/Value.cc
     )
-    target_link_libraries(_core PRIVATE GSL::gsl GSL::gslcblas)
-    # target_link_libraries(_core PRIVATE gsl gslcblas)
+    target_link_libraries(_core PRIVATE GSL::gsl)
     target_compile_definitions(_core PRIVATE VERSION_INFO=${PROJECT_VERSION})
     install(TARGETS _core DESTINATION .)
 
 else(PYTHON_ONLY)
     add_library(
         adani SHARED
         src/ApproximateCoefficientFunction.cc
@@ -111,16 +110,15 @@
         src/SpecialFunctions.cc
         src/SplittingFunction.cc
         src/ThresholdCoefficientFunction.cc
         src/Value.cc
     )
 
     # define libraries to be linked
-    target_link_libraries(adani GSL::gsl GSL::gslcblas)
-    # target_link_libraries(adani gsl gslcblas)
+    target_link_libraries(adani GSL::gsl)
 
     # install
     install(FILES ${PROJECT_SOURCE_DIR}/bin/adani-config
     DESTINATION bin PERMISSIONS OWNER_READ OWNER_WRITE OWNER_EXECUTE GROUP_READ GROUP_EXECUTE WORLD_READ WORLD_EXECUTE)
     install(FILES ${PROJECT_SOURCE_DIR}/bin/adani.pc DESTINATION lib/pkgconfig)
     install(DIRECTORY inc/adani DESTINATION include)
     install(TARGETS adani DESTINATION lib)
```

### Comparing `adani-1.0.2/LICENSE` & `adani-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/PKG-INFO` & `adani-1.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: adani
-Version: 1.0.2
-Summary: Code computing approximate DIS N3LO coefficients
-Author: Niccolò Laurenti
-License: AGPLv3
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # ADANI
 
 ADANI (Approximate DIS At N3LO Implementation) is a C++ code that computes an approximation for the DIS coefficient functions at N3LO in heavy quark production, that are not fully known yet.
 
 ## Citation Policy
 
 When using this code please cite [![arXiv](https://img.shields.io/badge/arXiv-2401.12139-b31b1b?labelColor=222222)](https://arxiv.org/abs/2401.12139)
@@ -27,18 +17,26 @@
 In order to install the C++ library run
 ```bash
 mkdir build && cd build
 cmake -DCMAKE_INSTALL_PREFIX=/your/installation/path/ ..
 make && make install
 ```
 
-The Python package is available in the PyPI <a href="https://pypi.org/project/adani/"><img alt="PyPI" src="https://img.shields.io/pypi/v/adani"/></a>. Install it with
+The Python package is available via:
+- PyPI <a href="https://pypi.org/project/adani/"><img alt="PyPI" src="https://img.shields.io/pypi/v/adani"/></a>. Install it with
 ```bash
 pip install adani
 ```
+- conda-forge: [![Conda Version](https://img.shields.io/conda/vn/conda-forge/adani.svg)](https://anaconda.org/conda-forge/adani).
+Install it with
+```bash
+conda install adani
+```
+At the moment there is a problem in the conda package: to fix it run also ```conda install conda-forge::gsl```.
+
 For installing the Python module from source run
 ```bash
 pip install .
 ```
 
 ## Compile a C++ program
 
@@ -51,15 +49,18 @@
 g++ -Wall -I/your/installation/path/include -L/your/installation/path/lib/ -o test.exe test.cpp -ladani
 ```
 In both cases remember to run
 ```bash
 export PATH=$PATH:/your/installation/path/bin
 export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/your/installation/path/lib
 ```
-For MacOS users: add the flags ```-std=c++17 -stdlib=libc++```.
+For MacOS users: add the flags ```-std=c++17 -stdlib=libc++``` and run also
+```bash
+export DYLD_LIBRARY_PATH=$DYLD_LIBRARY_PATH:/your/installation/path/lib
+```
 
 ## Import the Python module
 
 In order to use the Python module add
 ```bash
 import adani
 ```
```

#### html2text {}

```diff
@@ -1,45 +1,48 @@
-Metadata-Version: 2.1 Name: adani Version: 1.0.2 Summary: Code computing
-approximate DIS N3LO coefficients Author: NiccolÃ² Laurenti License: AGPLv3
-Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
-LICENSE # ADANI ADANI (Approximate DIS At N3LO Implementation) is a C++ code
-that computes an approximation for the DIS coefficient functions at N3LO in
-heavy quark production, that are not fully known yet. ## Citation Policy When
-using this code please cite [![arXiv](https://img.shields.io/badge/arXiv-
-2401.12139-b31b1b?labelColor=222222)](https://arxiv.org/abs/2401.12139) ##
-Dependencies The code depends on the public library ```gsl```. Optional
-dependencies are the library ```pybind11``` and the Python module ```scikit-
-build``` (both public), that are required for building the Python bindings. ##
-Installation In order to install the C++ library run ```bash mkdir build && cd
-build cmake -DCMAKE_INSTALL_PREFIX=/your/installation/path/ .. make && make
-install ``` The Python package is available in the PyPI _[_P_y_P_I_]. Install it with
-```bash pip install adani ``` For installing the Python module from source run
-```bash pip install . ``` ## Compile a C++ program In order to compile a simple
-program run ```bash g++ -Wall -o test.exe test.cpp -ladani `adani-config --
-cppflags --ldflags --cxxflags` ``` or ```bash g++ -Wall -I/your/installation/
-path/include -L/your/installation/path/lib/ -o test.exe test.cpp -ladani ``` In
-both cases remember to run ```bash export PATH=$PATH:/your/installation/path/
-bin export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/your/installation/path/lib ``` For
-MacOS users: add the flags ```-std=c++17 -stdlib=libc++```. ## Import the
-Python module In order to use the Python module add ```bash import adani ``` to
-a Python program. ## Contributing If you want to report a (possible) bug or
-want to ask for a new feature, please raise an issue: _[_G_i_t_H_u_b_ _i_s_s_u_e_s_]##
-Contacts Contact me at niclaurenti@gmail.com. ## Words of our prophet > La
-garra charrÃºa! L'ultima parola agli uruguagi, sempre loro! L'ultima parola nel
-calcio Ã¨ la loro: hanno un cuore differente, lo capisci o no? L'artiglio che
-graffia, > che lascia il segno nella storia dell'Inter: questa Ã¨ la storia che
-si ripete! [...] Il graffio che aveva portato l'Inter in Champions serve per
-rimarcare il territorio: > questo Ã¨ l'Uruguay quando va in campo con tutto se
-stesso...ecco chi Ã¨ Vecino: stanco, si, ma lascia in campo Vecino che parla
-alla fine, lascialo in campo, che la dice > lui l'ultima cosa nel calcio!
-Stanno a insegnare cos'Ã¨ il calcio agli uruguagi, ma vedi un po' te. > > 18/
-09/2018 > Messi! Messi! Leo Messi! Il sinistro migliore del mondo. Da Di Maria
-a Messi, dalla Bajada alla Perdriel sempre Rosario, la cittÃ  del calcio. Uno
-per l'altro. Si sblocca > la partita. Football! [...] Tutti in piedi per il
-miglior giocatore del mondo. Rispetto per il numero uno. [...] Rosario, cittÃ 
-del calcio, per questo calciatore che troppe > volte Ã¨ stato criticato. Anche
-quando era a Barcellona, quando Ã¨ arrivato, sofferente, da giovane, non ha mai
-dimenticato l'argentino. Parla rosarino, sente l'argentino nel > sangue, ha
-pianto per la Seleccion ed Ã¨ lui che la tiene in vita. [...] La mistica che
-entra in campo. Abbiamo nominato Diego [Armando Maradona] 10 minuti fa. Con
-Diego dentro > tutto Ã¨ possibile ed Ã¨ col pianto dell'Argentina e gli occhi
-spiritati del miglior giocatore del mondo. [...] VAMO! > > 26/11/2022
+# ADANI ADANI (Approximate DIS At N3LO Implementation) is a C++ code that
+computes an approximation for the DIS coefficient functions at N3LO in heavy
+quark production, that are not fully known yet. ## Citation Policy When using
+this code please cite [![arXiv](https://img.shields.io/badge/arXiv-2401.12139-
+b31b1b?labelColor=222222)](https://arxiv.org/abs/2401.12139) ## Dependencies
+The code depends on the public library ```gsl```. Optional dependencies are the
+library ```pybind11``` and the Python module ```scikit-build``` (both public),
+that are required for building the Python bindings. ## Installation In order to
+install the C++ library run ```bash mkdir build && cd build cmake -
+DCMAKE_INSTALL_PREFIX=/your/installation/path/ .. make && make install ``` The
+Python package is available via: - PyPI _[_P_y_P_I_]. Install it with ```bash pip
+install adani ``` - conda-forge: [![Conda Version](https://img.shields.io/
+conda/vn/conda-forge/adani.svg)](https://anaconda.org/conda-forge/adani).
+Install it with ```bash conda install adani ``` At the moment there is a
+problem in the conda package: to fix it run also ```conda install conda-forge::
+gsl```. For installing the Python module from source run ```bash pip install .
+``` ## Compile a C++ program In order to compile a simple program run ```bash
+g++ -Wall -o test.exe test.cpp -ladani `adani-config --cppflags --ldflags --
+cxxflags` ``` or ```bash g++ -Wall -I/your/installation/path/include -L/your/
+installation/path/lib/ -o test.exe test.cpp -ladani ``` In both cases remember
+to run ```bash export PATH=$PATH:/your/installation/path/bin export
+LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/your/installation/path/lib ``` For MacOS
+users: add the flags ```-std=c++17 -stdlib=libc++``` and run also ```bash
+export DYLD_LIBRARY_PATH=$DYLD_LIBRARY_PATH:/your/installation/path/lib ``` ##
+Import the Python module In order to use the Python module add ```bash import
+adani ``` to a Python program. ## Contributing If you want to report a
+(possible) bug or want to ask for a new feature, please raise an issue: _[_G_i_t_H_u_b
+_i_s_s_u_e_s_]## Contacts Contact me at niclaurenti@gmail.com. ## Words of our prophet
+> La garra charrÃºa! L'ultima parola agli uruguagi, sempre loro! L'ultima
+parola nel calcio Ã¨ la loro: hanno un cuore differente, lo capisci o no?
+L'artiglio che graffia, > che lascia il segno nella storia dell'Inter: questa
+Ã¨ la storia che si ripete! [...] Il graffio che aveva portato l'Inter in
+Champions serve per rimarcare il territorio: > questo Ã¨ l'Uruguay quando va in
+campo con tutto se stesso...ecco chi Ã¨ Vecino: stanco, si, ma lascia in campo
+Vecino che parla alla fine, lascialo in campo, che la dice > lui l'ultima cosa
+nel calcio! Stanno a insegnare cos'Ã¨ il calcio agli uruguagi, ma vedi un po'
+te. > > 18/09/2018 > Messi! Messi! Leo Messi! Il sinistro migliore del mondo.
+Da Di Maria a Messi, dalla Bajada alla Perdriel sempre Rosario, la cittÃ  del
+calcio. Uno per l'altro. Si sblocca > la partita. Football! [...] Tutti in
+piedi per il miglior giocatore del mondo. Rispetto per il numero uno. [...]
+Rosario, cittÃ  del calcio, per questo calciatore che troppe > volte Ã¨ stato
+criticato. Anche quando era a Barcellona, quando Ã¨ arrivato, sofferente, da
+giovane, non ha mai dimenticato l'argentino. Parla rosarino, sente l'argentino
+nel > sangue, ha pianto per la Seleccion ed Ã¨ lui che la tiene in vita. [...]
+La mistica che entra in campo. Abbiamo nominato Diego [Armando Maradona] 10
+minuti fa. Con Diego dentro > tutto Ã¨ possibile ed Ã¨ col pianto
+dell'Argentina e gli occhi spiritati del miglior giocatore del mondo. [...]
+VAMO! > > 26/11/2022
```

### Comparing `adani-1.0.2/README.md` & `adani-1.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: adani
+Version: 1.0.3
+Summary: Code computing approximate DIS N3LO coefficients
+Author: Niccolò Laurenti
+License: AGPLv3
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # ADANI
 
 ADANI (Approximate DIS At N3LO Implementation) is a C++ code that computes an approximation for the DIS coefficient functions at N3LO in heavy quark production, that are not fully known yet.
 
 ## Citation Policy
 
 When using this code please cite [![arXiv](https://img.shields.io/badge/arXiv-2401.12139-b31b1b?labelColor=222222)](https://arxiv.org/abs/2401.12139)
@@ -17,18 +27,26 @@
 In order to install the C++ library run
 ```bash
 mkdir build && cd build
 cmake -DCMAKE_INSTALL_PREFIX=/your/installation/path/ ..
 make && make install
 ```
 
-The Python package is available in the PyPI <a href="https://pypi.org/project/adani/"><img alt="PyPI" src="https://img.shields.io/pypi/v/adani"/></a>. Install it with
+The Python package is available via:
+- PyPI <a href="https://pypi.org/project/adani/"><img alt="PyPI" src="https://img.shields.io/pypi/v/adani"/></a>. Install it with
 ```bash
 pip install adani
 ```
+- conda-forge: [![Conda Version](https://img.shields.io/conda/vn/conda-forge/adani.svg)](https://anaconda.org/conda-forge/adani).
+Install it with
+```bash
+conda install adani
+```
+At the moment there is a problem in the conda package: to fix it run also ```conda install conda-forge::gsl```.
+
 For installing the Python module from source run
 ```bash
 pip install .
 ```
 
 ## Compile a C++ program
 
@@ -41,15 +59,18 @@
 g++ -Wall -I/your/installation/path/include -L/your/installation/path/lib/ -o test.exe test.cpp -ladani
 ```
 In both cases remember to run
 ```bash
 export PATH=$PATH:/your/installation/path/bin
 export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/your/installation/path/lib
 ```
-For MacOS users: add the flags ```-std=c++17 -stdlib=libc++```.
+For MacOS users: add the flags ```-std=c++17 -stdlib=libc++``` and run also
+```bash
+export DYLD_LIBRARY_PATH=$DYLD_LIBRARY_PATH:/your/installation/path/lib
+```
 
 ## Import the Python module
 
 In order to use the Python module add
 ```bash
 import adani
 ```
```

#### html2text {}

```diff
@@ -1,42 +1,51 @@
-# ADANI ADANI (Approximate DIS At N3LO Implementation) is a C++ code that
-computes an approximation for the DIS coefficient functions at N3LO in heavy
-quark production, that are not fully known yet. ## Citation Policy When using
-this code please cite [![arXiv](https://img.shields.io/badge/arXiv-2401.12139-
-b31b1b?labelColor=222222)](https://arxiv.org/abs/2401.12139) ## Dependencies
-The code depends on the public library ```gsl```. Optional dependencies are the
-library ```pybind11``` and the Python module ```scikit-build``` (both public),
-that are required for building the Python bindings. ## Installation In order to
-install the C++ library run ```bash mkdir build && cd build cmake -
-DCMAKE_INSTALL_PREFIX=/your/installation/path/ .. make && make install ``` The
-Python package is available in the PyPI _[_P_y_P_I_]. Install it with ```bash pip
-install adani ``` For installing the Python module from source run ```bash pip
-install . ``` ## Compile a C++ program In order to compile a simple program run
-```bash g++ -Wall -o test.exe test.cpp -ladani `adani-config --cppflags --
+Metadata-Version: 2.1 Name: adani Version: 1.0.3 Summary: Code computing
+approximate DIS N3LO coefficients Author: NiccolÃ² Laurenti License: AGPLv3
+Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
+LICENSE # ADANI ADANI (Approximate DIS At N3LO Implementation) is a C++ code
+that computes an approximation for the DIS coefficient functions at N3LO in
+heavy quark production, that are not fully known yet. ## Citation Policy When
+using this code please cite [![arXiv](https://img.shields.io/badge/arXiv-
+2401.12139-b31b1b?labelColor=222222)](https://arxiv.org/abs/2401.12139) ##
+Dependencies The code depends on the public library ```gsl```. Optional
+dependencies are the library ```pybind11``` and the Python module ```scikit-
+build``` (both public), that are required for building the Python bindings. ##
+Installation In order to install the C++ library run ```bash mkdir build && cd
+build cmake -DCMAKE_INSTALL_PREFIX=/your/installation/path/ .. make && make
+install ``` The Python package is available via: - PyPI _[_P_y_P_I_]. Install it with
+```bash pip install adani ``` - conda-forge: [![Conda Version](https://
+img.shields.io/conda/vn/conda-forge/adani.svg)](https://anaconda.org/conda-
+forge/adani). Install it with ```bash conda install adani ``` At the moment
+there is a problem in the conda package: to fix it run also ```conda install
+conda-forge::gsl```. For installing the Python module from source run ```bash
+pip install . ``` ## Compile a C++ program In order to compile a simple program
+run ```bash g++ -Wall -o test.exe test.cpp -ladani `adani-config --cppflags --
 ldflags --cxxflags` ``` or ```bash g++ -Wall -I/your/installation/path/include
 -L/your/installation/path/lib/ -o test.exe test.cpp -ladani ``` In both cases
 remember to run ```bash export PATH=$PATH:/your/installation/path/bin export
 LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/your/installation/path/lib ``` For MacOS
-users: add the flags ```-std=c++17 -stdlib=libc++```. ## Import the Python
-module In order to use the Python module add ```bash import adani ``` to a
-Python program. ## Contributing If you want to report a (possible) bug or want
-to ask for a new feature, please raise an issue: _[_G_i_t_H_u_b_ _i_s_s_u_e_s_]## Contacts
-Contact me at niclaurenti@gmail.com. ## Words of our prophet > La garra
-charrÃºa! L'ultima parola agli uruguagi, sempre loro! L'ultima parola nel
-calcio Ã¨ la loro: hanno un cuore differente, lo capisci o no? L'artiglio che
-graffia, > che lascia il segno nella storia dell'Inter: questa Ã¨ la storia che
-si ripete! [...] Il graffio che aveva portato l'Inter in Champions serve per
-rimarcare il territorio: > questo Ã¨ l'Uruguay quando va in campo con tutto se
-stesso...ecco chi Ã¨ Vecino: stanco, si, ma lascia in campo Vecino che parla
-alla fine, lascialo in campo, che la dice > lui l'ultima cosa nel calcio!
-Stanno a insegnare cos'Ã¨ il calcio agli uruguagi, ma vedi un po' te. > > 18/
-09/2018 > Messi! Messi! Leo Messi! Il sinistro migliore del mondo. Da Di Maria
-a Messi, dalla Bajada alla Perdriel sempre Rosario, la cittÃ  del calcio. Uno
-per l'altro. Si sblocca > la partita. Football! [...] Tutti in piedi per il
-miglior giocatore del mondo. Rispetto per il numero uno. [...] Rosario, cittÃ 
-del calcio, per questo calciatore che troppe > volte Ã¨ stato criticato. Anche
-quando era a Barcellona, quando Ã¨ arrivato, sofferente, da giovane, non ha mai
-dimenticato l'argentino. Parla rosarino, sente l'argentino nel > sangue, ha
-pianto per la Seleccion ed Ã¨ lui che la tiene in vita. [...] La mistica che
-entra in campo. Abbiamo nominato Diego [Armando Maradona] 10 minuti fa. Con
-Diego dentro > tutto Ã¨ possibile ed Ã¨ col pianto dell'Argentina e gli occhi
-spiritati del miglior giocatore del mondo. [...] VAMO! > > 26/11/2022
+users: add the flags ```-std=c++17 -stdlib=libc++``` and run also ```bash
+export DYLD_LIBRARY_PATH=$DYLD_LIBRARY_PATH:/your/installation/path/lib ``` ##
+Import the Python module In order to use the Python module add ```bash import
+adani ``` to a Python program. ## Contributing If you want to report a
+(possible) bug or want to ask for a new feature, please raise an issue: _[_G_i_t_H_u_b
+_i_s_s_u_e_s_]## Contacts Contact me at niclaurenti@gmail.com. ## Words of our prophet
+> La garra charrÃºa! L'ultima parola agli uruguagi, sempre loro! L'ultima
+parola nel calcio Ã¨ la loro: hanno un cuore differente, lo capisci o no?
+L'artiglio che graffia, > che lascia il segno nella storia dell'Inter: questa
+Ã¨ la storia che si ripete! [...] Il graffio che aveva portato l'Inter in
+Champions serve per rimarcare il territorio: > questo Ã¨ l'Uruguay quando va in
+campo con tutto se stesso...ecco chi Ã¨ Vecino: stanco, si, ma lascia in campo
+Vecino che parla alla fine, lascialo in campo, che la dice > lui l'ultima cosa
+nel calcio! Stanno a insegnare cos'Ã¨ il calcio agli uruguagi, ma vedi un po'
+te. > > 18/09/2018 > Messi! Messi! Leo Messi! Il sinistro migliore del mondo.
+Da Di Maria a Messi, dalla Bajada alla Perdriel sempre Rosario, la cittÃ  del
+calcio. Uno per l'altro. Si sblocca > la partita. Football! [...] Tutti in
+piedi per il miglior giocatore del mondo. Rispetto per il numero uno. [...]
+Rosario, cittÃ  del calcio, per questo calciatore che troppe > volte Ã¨ stato
+criticato. Anche quando era a Barcellona, quando Ã¨ arrivato, sofferente, da
+giovane, non ha mai dimenticato l'argentino. Parla rosarino, sente l'argentino
+nel > sangue, ha pianto per la Seleccion ed Ã¨ lui che la tiene in vita. [...]
+La mistica che entra in campo. Abbiamo nominato Diego [Armando Maradona] 10
+minuti fa. Con Diego dentro > tutto Ã¨ possibile ed Ã¨ col pianto
+dell'Argentina e gli occhi spiritati del miglior giocatore del mondo. [...]
+VAMO! > > 26/11/2022
```

### Comparing `adani-1.0.2/bin/adani-config.in` & `adani-1.0.3/bin/adani-config.in`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/docs/Tesi_Laurenti.pdf` & `adani-1.0.3/docs/Tesi_Laurenti.pdf`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/docs/approximation_smallx_nll.pdf` & `adani-1.0.3/docs/approximation_smallx_nll.pdf`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/docs/approximation_smallx_nll.tex` & `adani-1.0.3/docs/approximation_smallx_nll.tex`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/docs/montecarlointegration.pdf` & `adani-1.0.3/docs/montecarlointegration.pdf`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/docs/montecarlointegration.tex` & `adani-1.0.3/docs/montecarlointegration.tex`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/examples/test.cpp` & `adani-1.0.3/examples/test.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -15,24 +15,24 @@
     double dlogx = (logx_max - logx_min) / N;
     double dlogQ = (logQ_max - logQ_min) / N;
 
     double m = 4.92, m2Q2, m2mu2;
     int nf = 4;
 
     ApproximateCoefficientFunction F2g(
-        3, '2', 'g', true, "abmp", 1e-3, 1e-3, 1000, false, 25000
+        3, '2', 'g', true, "abmp", 1e-3, 1e-3, 1000, "analytical", 25000
     );
     ApproximateCoefficientFunction FLg(
-        3, 'L', 'g', true, "abmp", 1e-3, 1e-3, 1000, false, 25000
+        3, 'L', 'g', true, "abmp", 1e-3, 1e-3, 1000, "analytical", 25000
     );
     ApproximateCoefficientFunction F2q(
-        3, '2', 'q', true, "exact", 1e-3, 1e-3, 1000, false, 25000
+        3, '2', 'q', true, "exact", 1e-3, 1e-3, 1000
     );
     ApproximateCoefficientFunction FLq(
-        3, 'L', 'q', true, "exact", 1e-3, 1e-3, 1000, false, 25000
+        3, 'L', 'q', true, "exact", 1e-3, 1e-3, 1000
     );
 
     for (int i = 0; i < N; i++) {
         for (int j = 0; j < N; j++) {
 
             logx = logx_min + i * dlogx;
             x = pow(10, logx);
```

### Comparing `adani-1.0.2/examples/test.py` & `adani-1.0.3/examples/test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import adani as ad
 import numpy as np
 
 nf = 4
 m = 4.92
 
-F2g = ad.ApproximateCoefficientFunction(3, '2', 'g', True, "abmp", 1e-3, 1e-3, 1000, False, 25000)
-FLg = ad.ApproximateCoefficientFunction(3, 'L', 'g', True, "abmp", 1e-3, 1e-3, 1000, False, 25000)
-F2q = ad.ApproximateCoefficientFunction(3, '2', 'q', True, "exact", 1e-3, 1e-3, 1000, False, 25000)
-FLq = ad.ApproximateCoefficientFunction(3, 'L', 'q', True, "exact", 1e-3, 1e-3, 1000, False, 25000)
+F2g = ad.ApproximateCoefficientFunction(3, '2', 'g', True, "abmp", 1e-3, 1e-3, 1000, "analytical", 25000)
+FLg = ad.ApproximateCoefficientFunction(3, 'L', 'g', True, "abmp", 1e-3, 1e-3, 1000, "analytical", 25000)
+F2q = ad.ApproximateCoefficientFunction(3, '2', 'q', True, "exact", 1e-3, 1e-3, 1000)
+FLq = ad.ApproximateCoefficientFunction(3, 'L', 'q', True, "exact", 1e-3, 1e-3, 1000)
 
 for x in np.geomspace(1e-4, 1, 5):
     for Q in np.geomspace(10, 100, 5):
         m2Q2 = m**2 / Q**2
         m2mu2 = m2Q2
         print("C2_g^(3)(x=", x, ", Q=", Q, ") = ", F2g.fx(x, m2Q2, m2mu2, nf))
         print("C2_ps^(3)(x=", x, ", Q=", Q, ") = ", F2g.fx(x, m2Q2, m2mu2, nf))
```

### Comparing `adani-1.0.2/inc/adani/ApproximateCoefficientFunction.h` & `adani-1.0.3/inc/adani/ApproximateCoefficientFunction.h`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,16 @@
 //------------------------------------------------------------------------------------------//
 
 class AbstractApproximate : public CoefficientFunction {
     public:
         AbstractApproximate(
             const int &order, const char &kind, const char &channel,
             const double &abserr = 1e-3, const double &relerr = 1e-3,
-            const int &dim = 1000, const bool &MCintegral = false,
+            const int &dim = 1000,
+            const string &double_int_method = "analytical",
             const int &MCcalls = 25000
         );
         ~AbstractApproximate();
 
         double MuIndependentTerms(double x, double m2Q2, int nf) const override;
 
         Value
@@ -87,15 +88,16 @@
 
 class ApproximateCoefficientFunction : public AbstractApproximate {
     public:
         ApproximateCoefficientFunction(
             const int &order, const char &kind, const char &channel,
             const bool &NLL = true, const string &highscale_version = "klmv",
             const double &abserr = 1e-3, const double &relerr = 1e-3,
-            const int &dim = 1000, const bool &MCintegral = false,
+            const int &dim = 1000,
+            const string &double_int_method = "analytical",
             const int &MCcalls = 25000
         );
         ~ApproximateCoefficientFunction() override;
 
         Value MuIndependentTermsBand(
             double x, double m2Q2, int nf
         ) const override;
@@ -120,15 +122,16 @@
 
 class ApproximateCoefficientFunctionKLMV : public AbstractApproximate {
     public:
         ApproximateCoefficientFunctionKLMV(
             const int &order, const char &kind, const char &channel,
             const string &highscale_version = "klmv", const bool &lowxi = false,
             const double &abserr = 1e-3, const double &relerr = 1e-3,
-            const int &dim = 1000, const bool &MCintegral = false,
+            const int &dim = 1000,
+            const string &double_int_method = "analytical",
             const int &MCcalls = 25000
         );
         ~ApproximateCoefficientFunctionKLMV() override;
 
         Value MuIndependentTermsBand(
             double x, double m2Q2, int nf
         ) const override;
```

### Comparing `adani-1.0.2/inc/adani/AsymptoticCoefficientFunction.h` & `adani-1.0.3/inc/adani/AsymptoticCoefficientFunction.h`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/inc/adani/CoefficientFunction.h` & `adani-1.0.3/inc/adani/CoefficientFunction.h`

 * *Files 4% similar despite different names*

```diff
@@ -65,19 +65,14 @@
         ) const;
 
         // get methods
         int GetOrder() const { return order_; };
         char GetKind() const { return kind_; };
         char GetChannel() const { return channel_; };
 
-        // set methods
-        void SetOrder(const int &order);
-        void SetKind(const char &kind);
-        void SetChannel(const char &channel);
-
     private:
-        int order_;    // order = 1, 2, or 3
-        char kind_;    // kind_ = '2' for F2 and 'L' for FL
-        char channel_; // channel_ = 'g' for Cg and 'q' for Cq
+        const int order_;    // order = 1, 2, or 3
+        const char kind_;    // kind_ = '2' for F2 and 'L' for FL
+        const char channel_; // channel_ = 'g' for Cg and 'q' for Cq
 };
 
 #endif
```

### Comparing `adani-1.0.2/inc/adani/Constants.h` & `adani-1.0.3/inc/adani/Constants.h`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/inc/adani/Convolution.h` & `adani-1.0.3/inc/adani/Convolution.h`

 * *Files 2% similar despite different names*

```diff
@@ -59,20 +59,20 @@
         gsl_integration_workspace *GetWorkspace() const { return w_; };
         CoefficientFunction *GetCoeffFunc() const { return coefffunc_; };
         AbstractSplittingFunction *GetSplitFunc() const { return splitfunc_; };
 
         // set methods
         void SetAbserr(const double &abserr);
         void SetRelerr(const double &relerr);
-        void SetDim(const int &dim);
 
     private:
         double abserr_;
         double relerr_;
-        int dim_;
+        const int dim_;
+
         gsl_integration_workspace *w_;
 
     protected:
         CoefficientFunction *coefffunc_;
         AbstractSplittingFunction *splitfunc_;
 };
 
@@ -150,29 +150,28 @@
         double LocalPart(double x, double m2Q2, int nf) const override;
 
         // get methods
         bool GetMCintegral() const { return MCintegral_; };
         int GetMCcalls() const { return MCcalls_; };
 
         // set methods
-        void SetMCintegral(const bool &MCintegral);
         void SetMCcalls(const int &MCcalls);
 
         // support function for the integral. it is static in order to be passed
         // to gsl
         static double regular1_integrand(double z[], size_t /*dim*/, void *p);
         static double regular2_integrand(double z[], size_t /*dim*/, void *p);
         static double regular3_integrand(double z, void *p);
 
         static double singular1_integrand(double z[], size_t /*dim*/, void *p);
         static double singular2_integrand(double z[], size_t /*dim*/, void *p);
         static double singular3_integrand(double z, void *p);
 
     private:
-        bool MCintegral_;
+        const bool MCintegral_;
         int MCcalls_;
         gsl_monte_vegas_state *s_;
         gsl_rng *r_;
 
         Convolution *convolution_;
         ConvolutedCoefficientFunction *conv_coeff_;
 };
```

### Comparing `adani-1.0.2/inc/adani/ExactCoefficientFunction.h` & `adani-1.0.3/inc/adani/ExactCoefficientFunction.h`

 * *Files 3% similar despite different names*

```diff
@@ -18,16 +18,19 @@
 #define Exact_h
 
 #include "adani/AsymptoticCoefficientFunction.h"
 #include "adani/CoefficientFunction.h"
 #include "adani/Convolution.h"
 #include "adani/SplittingFunction.h"
 
+#include <string>
 #include <vector>
 
+using std::string;
+
 //==========================================================================================//
 //  forward declaration of class ThresholdCoefficientFunction to avoid circular
 //  dependencies
 //------------------------------------------------------------------------------------------//
 
 class ThresholdCoefficientFunction;
 
@@ -37,15 +40,16 @@
 
 class ExactCoefficientFunction : public CoefficientFunction {
 
     public:
         ExactCoefficientFunction(
             const int &order, const char &kind, const char &channel,
             const double &abserr = 1e-3, const double &relerr = 1e-3,
-            const int &dim = 1000, const bool &MCintegral = false,
+            const int &dim = 1000,
+            const string &double_int_method = "analytical",
             const int &MCcalls = 25000
         );
         ~ExactCoefficientFunction() override;
 
         double fx(double x, double m2Q2, double m2mu2, int nf) const override;
         double MuIndependentTerms(double x, double m2Q2, int nf) const override;
         double MuDependentTerms(
@@ -80,14 +84,15 @@
         SplittingFunction *Pgq1_;
         SplittingFunction *Pqq0_;
         ConvolutedSplittingFunctions *Pgg0Pgq0_;
         ConvolutedSplittingFunctions *Pqq0Pgq0_;
         SplittingFunction *Pgg1_;
         SplittingFunction *Pqg0_;
         ConvolutedSplittingFunctions *Pgq0Pqg0_;
+        ConvolutedSplittingFunctions *Pgg0Pgg0_;
 
         Delta *delta_;
 
         //==========================================================================================//
         //                      Exact massive coefficient functions
         //                      O(as)
         //------------------------------------------------------------------------------------------//
```

### Comparing `adani-1.0.2/inc/adani/HighEnergyCoefficientFunction.h` & `adani-1.0.3/inc/adani/HighEnergyCoefficientFunction.h`

 * *Files 1% similar despite different names*

```diff
@@ -39,19 +39,16 @@
             const bool &NLL = true
         );
         ~AbstractHighEnergyCoefficientFunction() override{};
 
         // get methods
         bool GetNLL() const { return NLL_; };
 
-        // set methods
-        void SetNLL(const bool &NLL) { NLL_ = NLL; };
-
     private:
-        bool NLL_;
+        const bool NLL_;
 
         //==========================================================================================//
         //                  Color factors O(as^3)
         //------------------------------------------------------------------------------------------//
 
     protected:
         double a_10(int nf) const;
```

### Comparing `adani-1.0.2/inc/adani/HighScaleCoefficientFunction.h` & `adani-1.0.3/inc/adani/HighScaleCoefficientFunction.h`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 
 #include "adani/CoefficientFunction.h"
 #include "adani/MasslessCoefficientFunction.h"
 #include "adani/MatchingCondition.h"
 
 //==========================================================================================//
 //                      The notation used is the following:
+//
 //                      C^{(k)} = k-th order expansion in
-//                      terms of \alpha_s^{[nf]} D^{(k)} =
-//                      k-th order expansion in terms of
+//                      terms of \alpha_s^{[nf]}
+//
+//                      D^{(k)} = k-th order expansion in terms of
 //                      \alpha_s^{[nf+1]}
 //------------------------------------------------------------------------------------------//
 
 //==========================================================================================//
 //  class HighScaleCoefficientFunction
 //------------------------------------------------------------------------------------------//
```

### Comparing `adani-1.0.2/inc/adani/HighScaleSplitLogs.h` & `adani-1.0.3/inc/adani/HighScaleSplitLogs.h`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/inc/adani/MasslessCoefficientFunction.h` & `adani-1.0.3/inc/adani/MasslessCoefficientFunction.h`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/inc/adani/MatchingCondition.h` & `adani-1.0.3/inc/adani/MatchingCondition.h`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,16 @@
  * =====================================================================================
  *
  *       Filename:  MatchingCondition.h
  *
  *    Description:  Header file for the
  * MatchingCondition.cc file.
  *
- *         Author:  Vamo!!
+ *         Author:  Non credo esista una persona che analizzi il calcio meglio
+ * di me.
  *
  *  In this file there are the matching conditions.
  *
  * =====================================================================================
  */
 
 #ifndef Match_h
@@ -30,23 +31,27 @@
     public:
         MatchingCondition(
             const int &order, const char &entry1, const char &entry2,
             const string &version
         );
         ~MatchingCondition(){};
 
+        int GetOrder() const { return order_; };
+        char GetEntry1() const { return entry1_; };
+        char GetEntry2() const { return entry2_; };
+        string GetVersion() const { return version_; };
+
         Value MuIndependentNfIndependentTerm(double x) const;
         vector<double> NotOrdered(double x) const;
 
     private:
-        int order_;
-        char entry1_;
-        char entry2_;
-
-        string version_;
+        const int order_;
+        const char entry1_;
+        const char entry2_;
+        const string version_;
 
         //==========================================================================================//
         //  Matching conditions O(as)
         //------------------------------------------------------------------------------------------//
 
         // double K_Qg1(double x, double m2mu2) const;
         // double K_gg1_local(double m2mu2) const ;
```

### Comparing `adani-1.0.2/inc/adani/SpecialFunctions.h` & `adani-1.0.3/inc/adani/SpecialFunctions.h`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/inc/adani/SplittingFunction.h` & `adani-1.0.3/inc/adani/SplittingFunction.h`

 * *Files 4% similar despite different names*

```diff
@@ -70,17 +70,17 @@
 
         // get methods
         double GetOrder() const { return order_; };
         char GetEntry1() const { return entry1_; };
         char GetEntry2() const { return entry2_; };
 
     private:
-        int order_;
-        char entry1_;
-        char entry2_;
+        const int order_;
+        const char entry1_;
+        const char entry2_;
 
         double (SplittingFunction::*reg_)(double, int) const;
         double (SplittingFunction::*sing_)(double, int) const;
         double (SplittingFunction::*sing_int_)(double, int) const;
         double (SplittingFunction::*loc_)(int) const;
 
         //==========================================================================================//
@@ -136,51 +136,54 @@
 
 class ConvolutedSplittingFunctions : public AbstractSplittingFunction {
     public:
         ConvolutedSplittingFunctions(
             const int &order1, const char &entry1, const char &entry2,
             const int &order2, const char &entry3, const char &entry4
         );
-        ~ConvolutedSplittingFunctions() override{};
+        ~ConvolutedSplittingFunctions() override;
 
         // overloading operators
         ConvolutedSplittingFunctions operator*(const double &rhs) const;
         friend ConvolutedSplittingFunctions operator*(
             const double &lhs, const ConvolutedSplittingFunctions &rhs
         );
         ConvolutedSplittingFunctions operator/(const double &rhs) const;
 
         // Components of the Convoluted Splitting Function
         double Regular(double x, int nf) const override;
-        double Singular(double /*x*/, int /*nf*/) const override { return 0.; };
-        double Local(int /*nf*/) const override { return 0.; };
+        double Singular(double x, int nf) const override;
+        double Local(int nf) const override;
         // Integral from 0 to x of the Singular part
-        double SingularIntegrated(double /*x*/, int /*nf*/) const override {
-            return 0.;
-        };
+        double SingularIntegrated(double x, int nf) const override;
 
         void SetFunctions();
 
         // get methods
         double GetOrder1() const { return order1_; };
         char GetEntry1() const { return entry1_; };
         char GetEntry2() const { return entry2_; };
         double GetOrder2() const { return order2_; };
         char GetEntry3() const { return entry3_; };
         char GetEntry4() const { return entry4_; };
 
     private:
-        int order1_;
-        char entry1_;
-        char entry2_;
-        int order2_;
-        char entry3_;
-        char entry4_;
+        const int order1_;
+        const char entry1_;
+        const char entry2_;
+        const int order2_;
+        const char entry3_;
+        const char entry4_;
 
         double (ConvolutedSplittingFunctions::*reg_)(double, int) const;
+        double (ConvolutedSplittingFunctions::*sing_)(double, int) const;
+        double (ConvolutedSplittingFunctions::*sing_int_)(double, int) const;
+        double (ConvolutedSplittingFunctions::*loc_)(int) const;
+
+        SplittingFunction *Pgg0_;
 
         //==========================================================================================//
         //  Convolution between the splitting functions Pgg0/Pqq0
         //  and Pgq0
         //------------------------------------------------------------------------------------------//
 
         double Pgg0_x_Pgq0(double x, int nf) const;
@@ -189,14 +192,30 @@
         //==========================================================================================//
         //  Convolution between the splitting functions Pgq0 and Pqg0
         //------------------------------------------------------------------------------------------//
 
         double Pgq0_x_Pqg0(double x, int nf) const;
 
         //==========================================================================================//
+        //  Convolution between the splitting functions Pgg0 and Pgg0
+        //------------------------------------------------------------------------------------------//
+
+        double Pgg0reg_x_Pgg0reg(double x) const;
+        double Pgg0reg_x_Pgg0sing(double x) const;
+        double Pgg0sing_x_Pgg0sing_reg(double x) const;
+        double Pgg0sing_x_Pgg0sing_sing(double x) const;
+        double Pgg0sing_x_Pgg0sing_sing_integrated(double x) const;
+        double Pgg0sing_x_Pgg0sing_loc() const;
+
+        double Pgg0_x_Pgg0_reg(double x, int nf) const;
+        double Pgg0_x_Pgg0_sing(double x, int nf) const;
+        double Pgg0_x_Pgg0_sing_integrated(double x, int nf) const;
+        double Pgg0_x_Pgg0_loc(int nf) const;
+
+        //==========================================================================================//
         //  Function needed to return a zero function
         //------------------------------------------------------------------------------------------//
 
         double ZeroFunction_x_nf(double /*x*/, int /*nf*/) const { return 0.; };
         double ZeroFunction_nf(int /*nf*/) const { return 0.; };
 };
```

### Comparing `adani-1.0.2/inc/adani/ThresholdCoefficientFunction.h` & `adani-1.0.3/inc/adani/ThresholdCoefficientFunction.h`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/inc/adani/Value.h` & `adani-1.0.3/inc/adani/Value.h`

 * *Files 17% similar despite different names*

```diff
@@ -2,16 +2,15 @@
  * =====================================================================================
  *
  *       Filename:  Value.h
  *
  *    Description:  Header file for the
  *                  Value.cc file.
  *
- *         Author: Non credo esista una persona che analizzi il calcio meglio di
- * me
+ *         Author: La fatica chiama e noi fedeli dobbiamo abbracciarla
  *
  *  In this file there is the class Value
  *
  * =====================================================================================
  */
 
 #ifndef Value_h
```

### Comparing `adani-1.0.2/inc/adani/_version.py` & `adani-1.0.3/inc/adani/_version.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/inc/adani/adani.h` & `adani-1.0.3/inc/adani/adani.h`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/inc/adani.egg-info/PKG-INFO` & `adani-1.0.3/inc/adani.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adani
-Version: 1.0.2
+Version: 1.0.3
 Summary: Code computing approximate DIS N3LO coefficients
 Author: Niccolò Laurenti
 License: AGPLv3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -27,18 +27,26 @@
 In order to install the C++ library run
 ```bash
 mkdir build && cd build
 cmake -DCMAKE_INSTALL_PREFIX=/your/installation/path/ ..
 make && make install
 ```
 
-The Python package is available in the PyPI <a href="https://pypi.org/project/adani/"><img alt="PyPI" src="https://img.shields.io/pypi/v/adani"/></a>. Install it with
+The Python package is available via:
+- PyPI <a href="https://pypi.org/project/adani/"><img alt="PyPI" src="https://img.shields.io/pypi/v/adani"/></a>. Install it with
 ```bash
 pip install adani
 ```
+- conda-forge: [![Conda Version](https://img.shields.io/conda/vn/conda-forge/adani.svg)](https://anaconda.org/conda-forge/adani).
+Install it with
+```bash
+conda install adani
+```
+At the moment there is a problem in the conda package: to fix it run also ```conda install conda-forge::gsl```.
+
 For installing the Python module from source run
 ```bash
 pip install .
 ```
 
 ## Compile a C++ program
 
@@ -51,15 +59,18 @@
 g++ -Wall -I/your/installation/path/include -L/your/installation/path/lib/ -o test.exe test.cpp -ladani
 ```
 In both cases remember to run
 ```bash
 export PATH=$PATH:/your/installation/path/bin
 export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/your/installation/path/lib
 ```
-For MacOS users: add the flags ```-std=c++17 -stdlib=libc++```.
+For MacOS users: add the flags ```-std=c++17 -stdlib=libc++``` and run also
+```bash
+export DYLD_LIBRARY_PATH=$DYLD_LIBRARY_PATH:/your/installation/path/lib
+```
 
 ## Import the Python module
 
 In order to use the Python module add
 ```bash
 import adani
 ```
```

#### html2text {}

```diff
@@ -1,45 +1,51 @@
-Metadata-Version: 2.1 Name: adani Version: 1.0.2 Summary: Code computing
+Metadata-Version: 2.1 Name: adani Version: 1.0.3 Summary: Code computing
 approximate DIS N3LO coefficients Author: NiccolÃ² Laurenti License: AGPLv3
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE # ADANI ADANI (Approximate DIS At N3LO Implementation) is a C++ code
 that computes an approximation for the DIS coefficient functions at N3LO in
 heavy quark production, that are not fully known yet. ## Citation Policy When
 using this code please cite [![arXiv](https://img.shields.io/badge/arXiv-
 2401.12139-b31b1b?labelColor=222222)](https://arxiv.org/abs/2401.12139) ##
 Dependencies The code depends on the public library ```gsl```. Optional
 dependencies are the library ```pybind11``` and the Python module ```scikit-
 build``` (both public), that are required for building the Python bindings. ##
 Installation In order to install the C++ library run ```bash mkdir build && cd
 build cmake -DCMAKE_INSTALL_PREFIX=/your/installation/path/ .. make && make
-install ``` The Python package is available in the PyPI _[_P_y_P_I_]. Install it with
-```bash pip install adani ``` For installing the Python module from source run
-```bash pip install . ``` ## Compile a C++ program In order to compile a simple
-program run ```bash g++ -Wall -o test.exe test.cpp -ladani `adani-config --
-cppflags --ldflags --cxxflags` ``` or ```bash g++ -Wall -I/your/installation/
-path/include -L/your/installation/path/lib/ -o test.exe test.cpp -ladani ``` In
-both cases remember to run ```bash export PATH=$PATH:/your/installation/path/
-bin export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/your/installation/path/lib ``` For
-MacOS users: add the flags ```-std=c++17 -stdlib=libc++```. ## Import the
-Python module In order to use the Python module add ```bash import adani ``` to
-a Python program. ## Contributing If you want to report a (possible) bug or
-want to ask for a new feature, please raise an issue: _[_G_i_t_H_u_b_ _i_s_s_u_e_s_]##
-Contacts Contact me at niclaurenti@gmail.com. ## Words of our prophet > La
-garra charrÃºa! L'ultima parola agli uruguagi, sempre loro! L'ultima parola nel
-calcio Ã¨ la loro: hanno un cuore differente, lo capisci o no? L'artiglio che
-graffia, > che lascia il segno nella storia dell'Inter: questa Ã¨ la storia che
-si ripete! [...] Il graffio che aveva portato l'Inter in Champions serve per
-rimarcare il territorio: > questo Ã¨ l'Uruguay quando va in campo con tutto se
-stesso...ecco chi Ã¨ Vecino: stanco, si, ma lascia in campo Vecino che parla
-alla fine, lascialo in campo, che la dice > lui l'ultima cosa nel calcio!
-Stanno a insegnare cos'Ã¨ il calcio agli uruguagi, ma vedi un po' te. > > 18/
-09/2018 > Messi! Messi! Leo Messi! Il sinistro migliore del mondo. Da Di Maria
-a Messi, dalla Bajada alla Perdriel sempre Rosario, la cittÃ  del calcio. Uno
-per l'altro. Si sblocca > la partita. Football! [...] Tutti in piedi per il
-miglior giocatore del mondo. Rispetto per il numero uno. [...] Rosario, cittÃ 
-del calcio, per questo calciatore che troppe > volte Ã¨ stato criticato. Anche
-quando era a Barcellona, quando Ã¨ arrivato, sofferente, da giovane, non ha mai
-dimenticato l'argentino. Parla rosarino, sente l'argentino nel > sangue, ha
-pianto per la Seleccion ed Ã¨ lui che la tiene in vita. [...] La mistica che
-entra in campo. Abbiamo nominato Diego [Armando Maradona] 10 minuti fa. Con
-Diego dentro > tutto Ã¨ possibile ed Ã¨ col pianto dell'Argentina e gli occhi
-spiritati del miglior giocatore del mondo. [...] VAMO! > > 26/11/2022
+install ``` The Python package is available via: - PyPI _[_P_y_P_I_]. Install it with
+```bash pip install adani ``` - conda-forge: [![Conda Version](https://
+img.shields.io/conda/vn/conda-forge/adani.svg)](https://anaconda.org/conda-
+forge/adani). Install it with ```bash conda install adani ``` At the moment
+there is a problem in the conda package: to fix it run also ```conda install
+conda-forge::gsl```. For installing the Python module from source run ```bash
+pip install . ``` ## Compile a C++ program In order to compile a simple program
+run ```bash g++ -Wall -o test.exe test.cpp -ladani `adani-config --cppflags --
+ldflags --cxxflags` ``` or ```bash g++ -Wall -I/your/installation/path/include
+-L/your/installation/path/lib/ -o test.exe test.cpp -ladani ``` In both cases
+remember to run ```bash export PATH=$PATH:/your/installation/path/bin export
+LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/your/installation/path/lib ``` For MacOS
+users: add the flags ```-std=c++17 -stdlib=libc++``` and run also ```bash
+export DYLD_LIBRARY_PATH=$DYLD_LIBRARY_PATH:/your/installation/path/lib ``` ##
+Import the Python module In order to use the Python module add ```bash import
+adani ``` to a Python program. ## Contributing If you want to report a
+(possible) bug or want to ask for a new feature, please raise an issue: _[_G_i_t_H_u_b
+_i_s_s_u_e_s_]## Contacts Contact me at niclaurenti@gmail.com. ## Words of our prophet
+> La garra charrÃºa! L'ultima parola agli uruguagi, sempre loro! L'ultima
+parola nel calcio Ã¨ la loro: hanno un cuore differente, lo capisci o no?
+L'artiglio che graffia, > che lascia il segno nella storia dell'Inter: questa
+Ã¨ la storia che si ripete! [...] Il graffio che aveva portato l'Inter in
+Champions serve per rimarcare il territorio: > questo Ã¨ l'Uruguay quando va in
+campo con tutto se stesso...ecco chi Ã¨ Vecino: stanco, si, ma lascia in campo
+Vecino che parla alla fine, lascialo in campo, che la dice > lui l'ultima cosa
+nel calcio! Stanno a insegnare cos'Ã¨ il calcio agli uruguagi, ma vedi un po'
+te. > > 18/09/2018 > Messi! Messi! Leo Messi! Il sinistro migliore del mondo.
+Da Di Maria a Messi, dalla Bajada alla Perdriel sempre Rosario, la cittÃ  del
+calcio. Uno per l'altro. Si sblocca > la partita. Football! [...] Tutti in
+piedi per il miglior giocatore del mondo. Rispetto per il numero uno. [...]
+Rosario, cittÃ  del calcio, per questo calciatore che troppe > volte Ã¨ stato
+criticato. Anche quando era a Barcellona, quando Ã¨ arrivato, sofferente, da
+giovane, non ha mai dimenticato l'argentino. Parla rosarino, sente l'argentino
+nel > sangue, ha pianto per la Seleccion ed Ã¨ lui che la tiene in vita. [...]
+La mistica che entra in campo. Abbiamo nominato Diego [Armando Maradona] 10
+minuti fa. Con Diego dentro > tutto Ã¨ possibile ed Ã¨ col pianto
+dell'Argentina e gli occhi spiritati del miglior giocatore del mondo. [...]
+VAMO! > > 26/11/2022
```

### Comparing `adani-1.0.2/inc/adani.egg-info/SOURCES.txt` & `adani-1.0.3/inc/adani.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .clang-format
 .gitattributes
 .gitignore
 .pre-commit-config.yaml
 CMakeLists.txt
 LICENSE
 README.md
+format.sh
 pyproject.toml
 setup.py
 versioneer.py
 .github/workflows/pip.yml
 .github/workflows/tests.yml
 bin/adani-config.in
 bin/adani.pc.in
```

### Comparing `adani-1.0.2/output/Q.txt` & `adani-1.0.3/output/Q.txt`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/output/x.txt` & `adani-1.0.3/output/x.txt`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/setup.py` & `adani-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/src/ApproximateCoefficientFunction.cc` & `adani-1.0.3/src/ApproximateCoefficientFunction.cc`

 * *Files 8% similar despite different names*

```diff
@@ -16,29 +16,33 @@
 //==========================================================================================//
 //  AbstractApproximate: constructor
 //------------------------------------------------------------------------------------------//
 
 AbstractApproximate::AbstractApproximate(
     const int &order, const char &kind, const char &channel,
     const double &abserr, const double &relerr, const int &dim,
-    const bool &MCintegral, const int &MCcalls
+    const string &double_int_method, const int &MCcalls
 )
     : CoefficientFunction(order, kind, channel) {
 
     muterms_ = new ExactCoefficientFunction(
-        order, kind, channel, abserr, relerr, dim, MCintegral, MCcalls
+        order, kind, channel, abserr, relerr, dim, double_int_method, MCcalls
     );
 }
 
 //==========================================================================================//
 //  AbstractApproximate: destructor
 //------------------------------------------------------------------------------------------//
 
 AbstractApproximate::~AbstractApproximate() { delete muterms_; }
 
+//==========================================================================================//
+//  AbstractApproximate: central value of the mu-independent terms
+//------------------------------------------------------------------------------------------//
+
 double AbstractApproximate::MuIndependentTerms(
     double x, double m2Q2, int nf
 ) const {
     return MuIndependentTermsBand(x, m2Q2, nf).GetCentral();
 }
 
 //==========================================================================================//
@@ -92,18 +96,18 @@
 //==========================================================================================//
 //  ApproximateCoefficientFunction: constructor
 //------------------------------------------------------------------------------------------//
 
 ApproximateCoefficientFunction::ApproximateCoefficientFunction(
     const int &order, const char &kind, const char &channel, const bool &NLL,
     const string &highscale_version, const double &abserr, const double &relerr,
-    const int &dim, const bool &MCintegral, const int &MCcalls
+    const int &dim, const string &double_int_method, const int &MCcalls
 )
     : AbstractApproximate(
-          order, kind, channel, abserr, relerr, dim, MCintegral, MCcalls
+          order, kind, channel, abserr, relerr, dim, double_int_method, MCcalls
       ) {
 
     threshold_ = new ThresholdCoefficientFunction(order, kind, channel);
     asymptotic_ = new AsymptoticCoefficientFunction(
         order, kind, channel, NLL, highscale_version
     );
 
@@ -258,19 +262,19 @@
 //==========================================================================================//
 //  ApproximateCoefficientFunctionKLMV: constructor
 //------------------------------------------------------------------------------------------//
 
 ApproximateCoefficientFunctionKLMV::ApproximateCoefficientFunctionKLMV(
     const int &order, const char &kind, const char &channel,
     const string &highscale_version, const bool &lowxi, const double &abserr,
-    const double &relerr, const int &dim, const bool &MCintegral,
+    const double &relerr, const int &dim, const string &double_int_method,
     const int &MCcalls
 )
     : AbstractApproximate(
-          order, kind, channel, abserr, relerr, dim, MCintegral, MCcalls
+          order, kind, channel, abserr, relerr, dim, double_int_method, MCcalls
       ) {
     if (GetOrder() == 1) {
         cout << "Error: KLMV approximation is not implemented at O(as)!"
              << endl;
         exit(-1);
     }
     if (GetKind() == 'L') {
```

### Comparing `adani-1.0.2/src/AsymptoticCoefficientFunction.cc` & `adani-1.0.3/src/AsymptoticCoefficientFunction.cc`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/src/CoefficientFunction.cc` & `adani-1.0.3/src/CoefficientFunction.cc`

 * *Files 13% similar despite different names*

```diff
@@ -5,72 +5,48 @@
 
 //==========================================================================================//
 //  CoefficientFunction: constructor
 //------------------------------------------------------------------------------------------//
 
 CoefficientFunction::CoefficientFunction(
     const int &order, const char &kind, const char &channel
-) {
+)
+    : order_(order), kind_(kind), channel_(channel) {
 
-    SetOrder(order);
-    SetKind(kind);
-    SetChannel(channel);
-}
-
-//==========================================================================================//
-//  CoefficientFunction: destructor
-//------------------------------------------------------------------------------------------//
-
-CoefficientFunction::~CoefficientFunction(){};
-
-//==========================================================================================//
-//  CoefficientFunction: set method for order: order = 1, 2, 3
-//------------------------------------------------------------------------------------------//
-
-void CoefficientFunction::SetOrder(const int &order) {
     // check order
     if (order < 1 || order > 3) {
         cout << "Error: order must be 1, 2 or 3. Got: " << order << endl;
         exit(-1);
     }
-    order_ = order;
-}
 
-//==========================================================================================//
-//  CoefficientFunction: set method for kind: kind = '2', 'L'
-//------------------------------------------------------------------------------------------//
-
-void CoefficientFunction::SetKind(const char &kind) {
     // check kind
     if (kind != '2' && kind != 'L') {
         cout << "Error: kind must be 2 or L. Got: " << kind << endl;
         exit(-1);
     }
-    kind_ = kind;
-}
-
-//==========================================================================================//
-//  CoefficientFunction: set method for channel: channel = 'g', 'q'
-//------------------------------------------------------------------------------------------//
 
-void CoefficientFunction::SetChannel(const char &channel) {
     // check channel
     if (channel != 'g' && channel != 'q') {
         cout << "Error: channel must be g or q. Got: " << channel << endl;
         exit(-1);
     }
     if (channel_ == 'q' && order_ == 1) {
         cout << "Error: quark coefficient function at O(as) doesn't exist!"
              << endl;
         exit(-1);
     }
-    channel_ = channel;
 }
 
 //==========================================================================================//
+//  CoefficientFunction: destructor
+//------------------------------------------------------------------------------------------//
+
+CoefficientFunction::~CoefficientFunction(){};
+
+//==========================================================================================//
 //  CoefficientFunction: central value of fx
 //------------------------------------------------------------------------------------------//
 
 double
     CoefficientFunction::fx(double x, double m2Q2, double m2mu2, int nf) const {
     return fxBand(x, m2Q2, m2mu2, nf).GetCentral();
 }
```

### Comparing `adani-1.0.2/src/Convolution.cc` & `adani-1.0.3/src/Convolution.cc`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,25 @@
 //==========================================================================================//
 //  AbstractConvolution: constructor
 //------------------------------------------------------------------------------------------//
 
 AbstractConvolution::AbstractConvolution(
     CoefficientFunction *coefffunc, AbstractSplittingFunction *splitfunc,
     const double &abserr, const double &relerr, const int &dim
-) {
-    abserr_ = abserr;
-    relerr_ = relerr;
-    dim_ = dim;
+)
+    : dim_(dim) {
+
+    SetAbserr(abserr);
+    SetRelerr(relerr);
+
+    // check dim
+    if (dim <= 0) {
+        cout << "Error: dim must be positive. Got " << dim << endl;
+        exit(-1);
+    }
 
     w_ = gsl_integration_workspace_alloc(dim);
 
     coefffunc_ = coefffunc;
     splitfunc_ = splitfunc;
 }
 
@@ -59,27 +66,14 @@
         cout << "Error: relerr must be positive. Got " << relerr << endl;
         exit(-1);
     }
     relerr_ = relerr;
 }
 
 //==========================================================================================//
-//  AbstractConvolution: set method for dim
-//------------------------------------------------------------------------------------------//
-
-void AbstractConvolution::SetDim(const int &dim) {
-    // check dim
-    if (dim <= 0) {
-        cout << "Error: dim must be positive. Got " << dim << endl;
-        exit(-1);
-    }
-    dim_ = dim;
-}
-
-//==========================================================================================//
 //  AbstractConvolution: convolute splitting function with coefficient function
 //------------------------------------------------------------------------------------------//
 
 double AbstractConvolution::Convolute(double x, double m2Q2, int nf) const {
     return RegularPart(x, m2Q2, nf) + SingularPart(x, m2Q2, nf)
            + LocalPart(x, m2Q2, nf);
 }
@@ -270,17 +264,17 @@
 //------------------------------------------------------------------------------------------//
 
 DoubleConvolution::DoubleConvolution(
     CoefficientFunction *coefffunc, AbstractSplittingFunction *splitfunc,
     const double &abserr, const double &relerr, const int &dim,
     const bool &MCintegral, const int &MCcalls
 )
-    : AbstractConvolution(coefffunc, splitfunc, abserr, relerr, dim) {
+    : AbstractConvolution(coefffunc, splitfunc, abserr, relerr, dim),
+      MCintegral_(MCintegral) {
 
-    SetMCintegral(MCintegral);
     SetMCcalls(MCcalls);
 
     if (MCintegral) {
         convolution_ =
             new Convolution(coefffunc, splitfunc, abserr, relerr, dim);
         conv_coeff_ = nullptr;
 
@@ -309,23 +303,14 @@
     }
 
     delete convolution_;
     delete conv_coeff_;
 }
 
 //==========================================================================================//
-//  DoubleConvolution: set method for method_flag
-//------------------------------------------------------------------------------------------//
-
-void DoubleConvolution::SetMCintegral(const bool &MCintegral) {
-
-    MCintegral_ = MCintegral;
-}
-
-//==========================================================================================//
 //  DoubleConvolution: set method for MCcalls
 //------------------------------------------------------------------------------------------//
 
 void DoubleConvolution::SetMCcalls(const int &MCcalls) {
     // check dim
     if (MCcalls <= 0) {
         cout << "Error: MCcalls must be positive. Got " << MCcalls << endl;
```

### Comparing `adani-1.0.2/src/ExactCoefficientFunction.cc` & `adani-1.0.3/src/ExactCoefficientFunction.cc`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 //==========================================================================================//
 //  ExactCoefficientFunction: constructor
 //------------------------------------------------------------------------------------------//
 
 ExactCoefficientFunction::ExactCoefficientFunction(
     const int &order, const char &kind, const char &channel,
     const double &abserr, const double &relerr, const int &dim,
-    const bool &MCintegral, const int &MCcalls
+    const string &double_int_method, const int &MCcalls
 )
     : CoefficientFunction(order, kind, channel) {
 
     gluon_as1_ = nullptr;
     gluon_as2_ = nullptr;
     quark_as2_ = nullptr;
 
@@ -29,17 +29,28 @@
     Pgq1_ = nullptr;
     Pqq0_ = nullptr;
     Pgg0Pgq0_ = nullptr;
     Pqq0Pgq0_ = nullptr;
     Pgg1_ = nullptr;
     Pqg0_ = nullptr;
     Pgq0Pqg0_ = nullptr;
+    Pgg0Pgg0_ = nullptr;
 
     delta_ = nullptr;
 
+    // check double_int_method
+    if (double_int_method != "analytical"
+        && double_int_method != "double_numerical"
+        && double_int_method != "monte_carlo") {
+        cout << "Error in ExactCoefficientFunction: double_int_method must be "
+                "'analytical', 'double_numerical' or 'monte_carlo'! Got "
+             << double_int_method << endl;
+        exit(-1);
+    }
+
     if (GetOrder() == 2) {
         asy_ = new AsymptoticCoefficientFunction(order, kind, channel);
         thr_ = new ThresholdCoefficientFunction(order, kind, channel);
     } else {
         asy_ = nullptr;
         thr_ = nullptr;
     }
@@ -58,14 +69,17 @@
         Pgq1_ = new SplittingFunction(1, 'g', 'q');
         Pqq0_ = new SplittingFunction(0, 'q', 'q');
         Pgg0Pgq0_ = new ConvolutedSplittingFunctions(0, 'g', 'g', 0, 'g', 'q');
         Pqq0Pgq0_ = new ConvolutedSplittingFunctions(0, 'q', 'q', 0, 'g', 'q');
         Pgg1_ = new SplittingFunction(1, 'g', 'g');
         Pqg0_ = new SplittingFunction(0, 'q', 'g');
         Pgq0Pqg0_ = new ConvolutedSplittingFunctions(0, 'g', 'q', 0, 'q', 'g');
+        if (double_int_method == "analytical")
+            Pgg0Pgg0_ =
+                new ConvolutedSplittingFunctions(0, 'g', 'g', 0, 'g', 'g');
     }
 
     if (GetOrder() == 2) {
         if (GetChannel() == 'q') {
             convolutions_lmu1_.push_back(
                 new Convolution(gluon_as1_, Pgq0_, abserr, relerr, dim)
             );
@@ -106,17 +120,27 @@
                 new Convolution(quark_as2_, Pqg0_, abserr, relerr, dim)
             );
             convolutions_lmu1_.push_back(
                 new Convolution(gluon_as2_, Pgg0_, abserr, relerr, dim)
             );
             convolutions_lmu1_.push_back(new Convolution(gluon_as2_, delta_));
 
-            convolutions_lmu2_.push_back(new DoubleConvolution(
-                gluon_as1_, Pgg0_, abserr, relerr, dim, MCintegral, MCcalls
-            ));
+            if (double_int_method == "monte_carlo") {
+                convolutions_lmu2_.push_back(new DoubleConvolution(
+                    gluon_as1_, Pgg0_, abserr, relerr, dim, true, MCcalls
+                ));
+            } else if (double_int_method == "double_numerical") {
+                convolutions_lmu2_.push_back(new DoubleConvolution(
+                    gluon_as1_, Pgg0_, abserr, relerr, dim, false, MCcalls
+                ));
+            } else {
+                convolutions_lmu2_.push_back(
+                    new Convolution(gluon_as1_, Pgg0Pgg0_, abserr, relerr, dim)
+                );
+            }
             convolutions_lmu2_.push_back(
                 new Convolution(gluon_as1_, Pgq0Pqg0_, abserr, relerr, dim)
             );
             convolutions_lmu2_.push_back(
                 new Convolution(gluon_as1_, Pgg0_, abserr, relerr, dim)
             );
             convolutions_lmu2_.push_back(new Convolution(gluon_as1_, delta_));
@@ -149,14 +173,15 @@
     delete Pgq1_;
     delete Pqq0_;
     delete Pgg0Pgq0_;
     delete Pqq0Pgq0_;
     delete Pgg1_;
     delete Pqg0_;
     delete Pgq0Pqg0_;
+    delete Pgg0Pgg0_;
 
     delete delta_;
 
     delete asy_;
     delete thr_;
 }
```

### Comparing `adani-1.0.2/src/HighEnergyCoefficientFunction.cc` & `adani-1.0.3/src/HighEnergyCoefficientFunction.cc`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,15 @@
 //==========================================================================================//
 //  AbstractHighEnergyCoefficientFunction: constructor
 //------------------------------------------------------------------------------------------//
 
 AbstractHighEnergyCoefficientFunction::AbstractHighEnergyCoefficientFunction(
     const int &order, const char &kind, const char &channel, const bool &NLL
 )
-    : CoefficientFunction(order, kind, channel) {
-
-    SetNLL(NLL);
-}
+    : CoefficientFunction(order, kind, channel), NLL_(NLL){};
 
 //==========================================================================================//
 //  HighEnergyCoefficientFunction: constructor
 //------------------------------------------------------------------------------------------//
 
 HighEnergyCoefficientFunction::HighEnergyCoefficientFunction(
     const int &order, const char &kind, const char &channel, const bool &NLL
```

### Comparing `adani-1.0.2/src/HighScaleCoefficientFunction.cc` & `adani-1.0.3/src/HighScaleCoefficientFunction.cc`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/src/HighScaleSplitLogs.cc` & `adani-1.0.3/src/HighScaleSplitLogs.cc`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/src/MasslessCoefficientFunction.cc` & `adani-1.0.3/src/MasslessCoefficientFunction.cc`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/src/MatchingCondition.cc` & `adani-1.0.3/src/MatchingCondition.cc`

 * *Files 0% similar despite different names*

```diff
@@ -11,36 +11,34 @@
 //==========================================================================================//
 //  MatchingCondition: constructor
 //------------------------------------------------------------------------------------------//
 
 MatchingCondition::MatchingCondition(
     const int &order, const char &entry1, const char &entry2,
     const string &version
-) {
+)
+    : order_(order), entry1_(entry1), entry2_(entry2), version_(version) {
     // check order
     if (order != 3) {
         cout << "Error: only order = 3 is implemented. Got " << order << endl;
         exit(-1);
     }
-    order_ = order;
 
     // check entry1
     if (entry1 != 'Q') {
         cout << "Error: only entry1 = 'Q' is implemented. Got " << entry1
              << endl;
         exit(-1);
     }
-    entry1_ = entry1;
 
     // check entry2
     if (entry2 != 'g' && entry2 != 'q') {
         cout << "Error: entry2 must be g or q. Got " << entry2 << endl;
         exit(-1);
     }
-    entry2_ = entry2;
 
     // check version
     if (version != "exact" && version != "abmp" && version != "klmv"
         && version != "gm") {
         cout << "Error: version must be 'exact', 'abmp', 'gm' or "
                 "'klmv'! Got "
              << version << endl;
@@ -54,16 +52,14 @@
 
     if (entry2 == 'q' && (version == "abmp" || version == "gm")) {
         cout << "Error: aQq channel doesn't have 'abmp' or 'gm' "
                 "version!"
              << endl;
         exit(-1);
     }
-
-    version_ = version;
 }
 
 //==========================================================================================//
 //  MatchingCondition: nf independent part of the a_Qi (i=q,q) term.
 //  a_Qi is the mu independent part of the unrenormalized OMA
 //------------------------------------------------------------------------------------------//
 
@@ -283,21 +279,21 @@
         cout << "a_Qg_30 exact is not known/implemented yet!" << endl;
         exit(-1);
     } else if (v == 1) {
         return (
             354.1002 * L13 + 479.3838 * L12 - 7856.784 * (2. - x)
             - 6233.530 * L2 + 9416.621 / x + 1548.891 / x * L
         );
-    } else if (v == -1) { // Updated version w.r.t v==-12
+    } else if (v == -1) {
         return (
             226.3840 * L13 - 652.2045 * L12 - 2686.387 * L1
             - 7714.786 * (2. - x) - 2841.851 * L2 + 7721.120 / x
             + 1548.891 / x * L
         );
-    } else if (v == -12) { // Version of the paper (used only for benchamrk)
+    } else if (v == -12) {
         return (
             -2658.323 * L12 - 7449.948 * L1 - 7460.002 * (2. - x)
             + 3178.819 * L2 + 4710.725 / x + 1548.891 / x * L
         );
     } else if (v == 2) {
         double L14 = L13 * L1;
         double L15 = L14 * L1;
```

### Comparing `adani-1.0.2/src/SpecialFunctions.cc` & `adani-1.0.3/src/SpecialFunctions.cc`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/src/SplittingFunction.cc` & `adani-1.0.3/src/SplittingFunction.cc`

 * *Files 13% similar despite different names*

```diff
@@ -17,36 +17,36 @@
 //==========================================================================================//
 //  SplittingFunction: constructor
 //------------------------------------------------------------------------------------------//
 
 SplittingFunction::SplittingFunction(
     const int &order, const char &entry1, const char &entry2
 )
-    : AbstractSplittingFunction() {
+    : AbstractSplittingFunction(),
+      order_(order),
+      entry1_(entry1),
+      entry2_(entry2) {
 
     // check order
     if (order != 0 && order != 1) {
         cout << "Error: order must be 0 or 1. Got " << order << endl;
         exit(-1);
     }
-    order_ = order;
 
     // check entry1
     if (entry1 != 'g' && entry1 != 'q') {
         cout << "Error: entry1 must be g or q. Got " << entry1 << endl;
         exit(-1);
     }
-    entry1_ = entry1;
 
     // check entry2
     if (entry2 != 'g' && entry2 != 'q') {
         cout << "Error: entry2 must be g or q. Got " << entry2 << endl;
         exit(-1);
     }
-    entry2_ = entry2;
 
     SetFunctions();
 }
 
 //==========================================================================================//
 //  SplittingFunction: Regular part
 //------------------------------------------------------------------------------------------//
@@ -183,70 +183,104 @@
 //  ConvolutedSplittingFunctions: constructor
 //------------------------------------------------------------------------------------------//
 
 ConvolutedSplittingFunctions::ConvolutedSplittingFunctions(
     const int &order1, const char &entry1, const char &entry2,
     const int &order2, const char &entry3, const char &entry4
 )
-    : AbstractSplittingFunction() {
+    : AbstractSplittingFunction(),
+      order1_(order1),
+      entry1_(entry1),
+      entry2_(entry2),
+      order2_(order2),
+      entry3_(entry3),
+      entry4_(entry4) {
 
     // check order
     if (order1 != 0 && order1 != 1) {
         cout << "Error: order1 must be 0 or 1. Got " << order1 << endl;
         exit(-1);
     }
-    order1_ = order1;
 
     // check order
     if (order2 != 0 && order2 != 1) {
         cout << "Error: order2 must be 0 or 1. Got " << order2 << endl;
         exit(-1);
     }
-    order2_ = order2;
 
     // check entry1
     if (entry1 != 'g' && entry1 != 'q') {
         cout << "Error: entry1 must be g or q. Got " << entry1 << endl;
         exit(-1);
     }
-    entry1_ = entry1;
 
     // check entry2
     if (entry2 != 'g' && entry2 != 'q') {
         cout << "Error: entry2 must be g or q. Got " << entry2 << endl;
         exit(-1);
     }
-    entry2_ = entry2;
 
     // check entry3
     if (entry3 != 'g' && entry3 != 'q') {
         cout << "Error: entry3 must be g or q. Got " << entry3 << endl;
         exit(-1);
     }
-    entry3_ = entry3;
 
     // check entry4
     if (entry4 != 'g' && entry4 != 'q') {
         cout << "Error: entry3 must be g or q. Got " << entry4 << endl;
         exit(-1);
     }
-    entry4_ = entry4;
+
+    if (order1_ == 0 && entry1_ == 'g' && entry2_ == 'g' && order2_ == 0
+        && entry3_ == 'g' && entry4_ == 'g') {
+        Pgg0_ = new SplittingFunction(0, 'g', 'g');
+    } else {
+        Pgg0_ = nullptr;
+    }
 
     SetFunctions();
 }
 
+ConvolutedSplittingFunctions::~ConvolutedSplittingFunctions() { delete Pgg0_; }
+
 //==========================================================================================//
 //  ConvolutedSplittingFunctions: regular part
 //------------------------------------------------------------------------------------------//
 
 double ConvolutedSplittingFunctions::Regular(double x, int nf) const {
     return GetMultFact() * (this->*reg_)(x, nf);
 }
 
 //==========================================================================================//
+//  ConvolutedSplittingFunctions: singular part
+//------------------------------------------------------------------------------------------//
+
+double ConvolutedSplittingFunctions::Singular(double x, int nf) const {
+    return GetMultFact() * (this->*sing_)(x, nf);
+}
+
+//==========================================================================================//
+//  ConvolutedSplittingFunctions: integral from 0 to x of the singular part
+//------------------------------------------------------------------------------------------//
+
+double
+    ConvolutedSplittingFunctions::SingularIntegrated(double x, int nf) const {
+    return GetMultFact() * (this->*sing_int_)(x, nf);
+}
+
+//==========================================================================================//
+//  ConvolutedSplittingFunctions: local part
+//------------------------------------------------------------------------------------------//
+
+double ConvolutedSplittingFunctions::Local(int nf) const {
+    return GetMultFact() * (this->*loc_)(nf);
+}
+
+//==========================================================================================//
 //  ConvolutedSplittingFunctions: overload of operator * double
 //------------------------------------------------------------------------------------------//
 
 ConvolutedSplittingFunctions
     ConvolutedSplittingFunctions::operator*(const double &rhs) const {
     ConvolutedSplittingFunctions res(
         order1_, entry1_, entry2_, order2_, entry3_, entry4_
@@ -287,23 +321,39 @@
 //  function
 //------------------------------------------------------------------------------------------//
 
 void ConvolutedSplittingFunctions::SetFunctions() {
 
     if (order1_ == 0 && order2_ == 0) {
         if (entry1_ == 'g' && entry2_ == 'q' && entry3_ == 'q'
-            && entry4_ == 'g')
+            && entry4_ == 'g') {
             reg_ = &ConvolutedSplittingFunctions::Pgq0_x_Pqg0;
-        else if (entry1_ == 'g' && entry2_ == 'g' && entry3_ == 'g'
-                 && entry4_ == 'q')
+            sing_ = &ConvolutedSplittingFunctions::ZeroFunction_x_nf;
+            sing_int_ = &ConvolutedSplittingFunctions::ZeroFunction_x_nf;
+            loc_ = &ConvolutedSplittingFunctions::ZeroFunction_nf;
+        } else if (entry1_ == 'g' && entry2_ == 'g' && entry3_ == 'g'
+                   && entry4_ == 'q') {
             reg_ = &ConvolutedSplittingFunctions::Pgg0_x_Pgq0;
-        else if (entry1_ == 'q' && entry2_ == 'q' && entry3_ == 'g'
-                 && entry4_ == 'q')
+            sing_ = &ConvolutedSplittingFunctions::ZeroFunction_x_nf;
+            sing_int_ = &ConvolutedSplittingFunctions::ZeroFunction_x_nf;
+            loc_ = &ConvolutedSplittingFunctions::ZeroFunction_nf;
+        } else if (entry1_ == 'q' && entry2_ == 'q' && entry3_ == 'g'
+                   && entry4_ == 'q') {
             reg_ = &ConvolutedSplittingFunctions::Pqq0_x_Pgq0;
-        else {
+            sing_ = &ConvolutedSplittingFunctions::ZeroFunction_x_nf;
+            sing_int_ = &ConvolutedSplittingFunctions::ZeroFunction_x_nf;
+            loc_ = &ConvolutedSplittingFunctions::ZeroFunction_nf;
+        } else if (entry1_ == 'g' && entry2_ == 'g' && entry3_ == 'g'
+                   && entry4_ == 'g') {
+            reg_ = &ConvolutedSplittingFunctions::Pgg0_x_Pgg0_reg;
+            sing_ = &ConvolutedSplittingFunctions::Pgg0_x_Pgg0_sing;
+            sing_int_ =
+                &ConvolutedSplittingFunctions::Pgg0_x_Pgg0_sing_integrated;
+            loc_ = &ConvolutedSplittingFunctions::Pgg0_x_Pgg0_loc;
+        } else {
             cout << "Error: P" << entry1_ << entry2_ << order1_ << " x P"
                  << entry3_ << entry4_ << order2_ << " is not implemented!"
                  << endl;
             exit(-1);
         }
     } else {
         cout << "Error: P" << entry1_ << entry2_ << order1_ << " x P" << entry3_
@@ -623,7 +673,121 @@
 //------------------------------------------------------------------------------------------//
 
 double ConvolutedSplittingFunctions::Pgq0_x_Pqg0(double x, int nf) const {
 
     return 4. * CF * nf
            * (1. + 4. / 3 / x - x - 4. * x * x / 3 + 2. * (1 + x) * log(x));
 }
+
+//==========================================================================================//
+//  Analytical convolution between the splitting functions Pgg0reg and Pgg0reg
+//------------------------------------------------------------------------------------------//
+
+double ConvolutedSplittingFunctions::Pgg0reg_x_Pgg0reg(double x) const {
+
+    return 16 * CA * CA
+           * ((-1. + x) * (11. + x * (5. + 2. * x))
+              - 3. * (1. + x * (4. + x + x * x)) * log(x))
+           / (3. * x);
+}
+
+//==========================================================================================//
+//  Analytical convolution between the splitting functions Pgg0reg and Pgg0sing
+//------------------------------------------------------------------------------------------//
+
+double ConvolutedSplittingFunctions::Pgg0reg_x_Pgg0sing(double x) const {
+
+    return 16. * CA * CA
+           * (0.5 * (1. - 4. * x + 3. * x * x)
+              + (-2. + 1. / x + x - x * x) * log(1. - x)
+              + (2. - x + x * x) * log(x));
+}
+
+//==========================================================================================//
+//  Regular part of the analytical convolution between the splitting functions
+//  Pgg0sing and Pgg0sing
+//------------------------------------------------------------------------------------------//
+
+double ConvolutedSplittingFunctions::Pgg0sing_x_Pgg0sing_reg(double x) const {
+
+    return -16 * CA * CA * log(x) / (1. - x);
+}
+
+//==========================================================================================//
+//  Singular part of the analytical convolution between the splitting functions
+//  Pgg0sing and Pgg0sing
+//------------------------------------------------------------------------------------------//
+
+double ConvolutedSplittingFunctions::Pgg0sing_x_Pgg0sing_sing(double x) const {
+
+    return 16 * CA * CA * 2. * log(1. - x) / (1. - x);
+}
+
+//==========================================================================================//
+//  Integral from 0 to x of the singular part of the analytical convolution
+//  between the splitting functions Pgg0sing and Pgg0sing
+//------------------------------------------------------------------------------------------//
+
+double ConvolutedSplittingFunctions::Pgg0sing_x_Pgg0sing_sing_integrated(
+    double x
+) const {
+
+    double L1 = log(1. - x);
+    return -16. * CA * CA * L1 * L1;
+}
+
+//==========================================================================================//
+//  Local part of the analytical convolution between the splitting functions
+//  Pgg0sing and Pgg0sing
+//------------------------------------------------------------------------------------------//
+
+double ConvolutedSplittingFunctions::Pgg0sing_x_Pgg0sing_loc() const {
+
+    return -16 * CA * CA * zeta2;
+}
+
+//==========================================================================================//
+//  Regular part of the analytical convolution between the splitting functions
+//  Pgg0 and Pgg0
+//------------------------------------------------------------------------------------------//
+
+double ConvolutedSplittingFunctions::Pgg0_x_Pgg0_reg(double x, int nf) const {
+
+    return Pgg0reg_x_Pgg0reg(x) + 2 * Pgg0reg_x_Pgg0sing(x)
+           + 2 * Pgg0_->Regular(x, nf) * Pgg0_->Local(nf)
+           + Pgg0sing_x_Pgg0sing_reg(x);
+}
+
+//==========================================================================================//
+//  Singular part of the analytical convolution between the splitting functions
+//  Pgg0 and Pgg0
+//------------------------------------------------------------------------------------------//
+
+double ConvolutedSplittingFunctions::Pgg0_x_Pgg0_sing(double x, int nf) const {
+
+    return Pgg0sing_x_Pgg0sing_sing(x)
+           + 2 * Pgg0_->Singular(x, nf) * Pgg0_->Local(nf);
+}
+
+//==========================================================================================//
+//  Integral from 0 to x of the singular part of the analytical convolution
+//  between the splitting functions Pgg0 and Pgg0
+//------------------------------------------------------------------------------------------//
+
+double ConvolutedSplittingFunctions::Pgg0_x_Pgg0_sing_integrated(
+    double x, int nf
+) const {
+
+    return Pgg0sing_x_Pgg0sing_sing_integrated(x)
+           + 2 * Pgg0_->SingularIntegrated(x, nf) * Pgg0_->Local(nf);
+}
+
+//==========================================================================================//
+//  Local part of the analytical convolution between the splitting functions
+//  Pgg0 and Pgg0
+//------------------------------------------------------------------------------------------//
+
+double ConvolutedSplittingFunctions::Pgg0_x_Pgg0_loc(int nf) const {
+
+    double loc = Pgg0_->Local(nf);
+    return Pgg0sing_x_Pgg0sing_loc() + loc * loc;
+}
```

### Comparing `adani-1.0.2/src/ThresholdCoefficientFunction.cc` & `adani-1.0.3/src/ThresholdCoefficientFunction.cc`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/src/Value.cc` & `adani-1.0.3/src/Value.cc`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/src/hplog.f` & `adani-1.0.3/src/hplog.f`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/src/hqcoef.f` & `adani-1.0.3/src/hqcoef.f`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/tests/test_approx_coeff_func.py` & `adani-1.0.3/tests/test_approx_coeff_func.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,30 @@
 import adani as ad
 import oldadani as oldad
 import numpy as np
 
+def test_coeff_func():
+    for order in range(1, 3 + 1):
+        for kind in ["2", "L"]:
+            for channel in ["q", "g"]:
+                if order == 1 and channel == "q":
+                    continue
+                app = ad.ApproximateCoefficientFunction(order, kind, channel)
+                assert app.GetOrder() == order
+                assert app.GetKind() == kind
+                assert app.GetChannel() == channel
+                del app
+
 def test_mudependent_terms():
     for order in [2, 3]:
         for channel in ['g', 'q']:
             for kind in ['2', 'L']:
                 for dim in [1000]:
                     for MCcalls in [20000]:
-                        for mf in [False, True]:
+                        for mf in ["analytical", "double_numerical", "monte_carlo"]:
                             for abserr in [1e-3]:
                                 relerr = abserr
                                 massive = ad.ExactCoefficientFunction(order, kind, channel, abserr, relerr, dim, mf, MCcalls)
                                 app = ad.ApproximateCoefficientFunction(order, kind, channel, True, "klmv", abserr, relerr, dim, mf, MCcalls)
                                 x = np.geomspace(1e-5, 1., 5, endpoint=True)
                                 for xi in np.geomspace(1e-2, 1e4, 4, endpoint=True):
                                     for nf in [4, 5]:
```

### Comparing `adani-1.0.2/tests/test_asy.py` & `adani-1.0.3/tests/test_asy.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/tests/test_exact_coeff_func.py` & `adani-1.0.3/tests/test_exact_coeff_func.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/tests/test_high_scale.py` & `adani-1.0.3/tests/test_high_scale.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/tests/test_highenergy.py` & `adani-1.0.3/tests/test_highenergy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 import adani as ad
 import oldadani as old
 import numpy as np
 
+def test_nll():
+    for nll in [True, False]:
+        he = ad.HighEnergyCoefficientFunction(3, "2", "g", NLL=nll)
+        hehs = ad.HighEnergyHighScaleCoefficientFunction(3, "2", "g", NLL=nll)
+        pt = ad.PowerTermsCoefficientFunction(3, "2", "g", NLL=nll)
+        assert he.GetNLL() == nll
+        assert hehs.GetNLL() == nll
+        assert pt.GetNLL() == nll
+
 def test_highenergy_as2_oldadani():
     for kind in ['2', 'L']:
         for channel in ['g', 'q']:
             he = ad.HighEnergyCoefficientFunction(2, kind, channel)
             for x in np.geomspace(1e-5, 1., 100, endpoint=False):
                 for m2Q2 in np.geomspace(1e-4, 1e-2, 10):
                     for m2mu2 in np.geomspace(1e-4, 1e-2, 10):
@@ -113,14 +122,16 @@
                                 res2 = old.CL_ps3_power_terms(x, m2Q2, m2mu2, nf, 0)
                             np.testing.assert_allclose(res1, res2, rtol=1e-7)
 
 def test_powerterms():
     for order in range(1, 3 + 1):
         for kind in ['2', 'L']:
             for channel in ['g', 'q']:
+                if channel == 'q' and order == 1:
+                    continue
                 for NLL in [True, False]:
                     he = ad.HighEnergyCoefficientFunction(order, kind, channel, NLL)
                     hehs = ad.HighEnergyHighScaleCoefficientFunction(order, kind, channel, NLL)
                     pt = ad.PowerTermsCoefficientFunction(order, kind, channel, NLL)
                     for nf in range(1, 6 + 1):
                         for m2mu2 in np.geomspace(1e-4, 1e2, 10):
                             for m2Q2 in np.geomspace(1e-4, 1e2, 10):
```

### Comparing `adani-1.0.2/tests/test_massless.py` & `adani-1.0.3/tests/test_massless.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/tests/test_mc_integral.py` & `adani-1.0.3/tests/test_mc_integral.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import adani as ad
 import numpy as np
 
 nf=4
 
 def test_mc_integrals():
     for kind in ['2', 'L']:
-        massive_mc = ad.ExactCoefficientFunction(3, kind, 'g', 1e-3, 1e-3, 1000, True, 1000000)
-        massive_nomc = ad.ExactCoefficientFunction(3, kind, 'g', 1e-3, 1e-3, 1000, False, 25000)
+        massive_mc = ad.ExactCoefficientFunction(3, kind, 'g', 1e-3, 1e-3, 1000, "monte_carlo", 1000000)
+        massive_nomc = ad.ExactCoefficientFunction(3, kind, 'g', 1e-3, 1e-3, 1000, "double_numerical", 25000)
+        massive_analytical = ad.ExactCoefficientFunction(3, kind, 'g', 1e-3, 1e-3, 1000, "analytical")
         for xi in np.geomspace(1e-2, 1e4, 4, endpoint=True):
             m2Q2 = 1/xi
             xmax = 1. / (1. + 4 * m2Q2)
             for x in np.geomspace(1e-5, xmax, 5, endpoint=False):
                     for nf in range(1, 6 + 1):
                         res1 = massive_mc.MuDependentTerms(x, m2Q2, m2Q2, nf)
                         res2 = massive_nomc.MuDependentTerms(x, m2Q2, m2Q2, nf)
+                        res3 = massive_analytical.MuDependentTerms(x, m2Q2, m2Q2, nf)
                         np.testing.assert_allclose(res1, res2, rtol=5e-3)
+                        np.testing.assert_allclose(res2, res3, 1e-3)
```

### Comparing `adani-1.0.2/tests/test_splitting_functions.py` & `adani-1.0.3/tests/test_splitting_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import adani as ad
 import oldadani as old
 import numpy as np
 
 CA = 3
 CF = 4./3
 
+def test_get_methods():
+    for entry1 in ["q", "g"]:
+        for entry2 in ["q", "g"]:
+            sf = ad.SplittingFunction(0, entry1, entry2)
+            assert sf.GetOrder() == 0
+            assert sf.GetEntry1() == entry1
+            assert sf.GetEntry2() == entry2
+
 def test_Pgq0():
 
     sf = ad.SplittingFunction(0, 'g', 'q')
 
     for x in np.geomspace(1e-5, 1., 10, endpoint=True):
         for nf in range(1, 6 + 1):
             np.testing.assert_allclose(old.Pgq0(x), sf.Regular(x, nf), rtol = 1e-7)
```

### Comparing `adani-1.0.2/tests/test_threshold.py` & `adani-1.0.3/tests/test_threshold.py`

 * *Files identical despite different names*

### Comparing `adani-1.0.2/versioneer.py` & `adani-1.0.3/versioneer.py`

 * *Files identical despite different names*

