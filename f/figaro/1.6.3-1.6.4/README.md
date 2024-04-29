# Comparing `tmp/figaro-1.6.3.tar.gz` & `tmp/figaro-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figaro-1.6.3.tar", last modified: Tue Apr 23 15:24:31 2024, max compression
+gzip compressed data, was "figaro-1.6.4.tar", last modified: Mon Apr 29 10:57:10 2024, max compression
```

## Comparing `figaro-1.6.3.tar` & `figaro-1.6.4.tar`

### file list

```diff
@@ -1,69 +1,70 @@
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-23 15:24:31.911923 figaro-1.6.3/
--rw-r--r--   0 rinaldi    (503) staff       (20)     1072 2023-11-15 13:14:25.000000 figaro-1.6.3/LICENSE
--rw-r--r--   0 rinaldi    (503) staff       (20)       67 2024-02-10 17:20:30.000000 figaro-1.6.3/MANIFEST.in
--rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-23 15:24:31.911707 figaro-1.6.3/PKG-INFO
--rw-r--r--   0 rinaldi    (503) staff       (20)     4154 2024-02-15 08:23:51.000000 figaro-1.6.3/README.md
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-23 15:24:31.897190 figaro-1.6.3/docs/
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-23 15:24:31.901881 figaro-1.6.3/docs/source/
--rw-r--r--   0 rinaldi    (503) staff       (20)      317 2024-02-15 08:23:51.000000 figaro-1.6.3/docs/source/api.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/figaro.cosmology.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      159 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/figaro.credible_regions.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/figaro.cumulative.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/figaro.decorators.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/figaro.diagnostic.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/figaro.load.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      133 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/figaro.marginal.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      130 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/figaro.mixture.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/figaro.montecarlo.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/figaro.plot.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      293 2024-02-15 08:23:51.000000 figaro-1.6.3/docs/source/figaro.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/figaro.transform.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      124 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/figaro.utils.rst
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-23 15:24:31.904022 figaro-1.6.3/docs/source/generated/
--rw-r--r--   0 rinaldi    (503) staff       (20)      207 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/generated/figaro.cosmology.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      363 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/generated/figaro.credible_regions.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      231 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/generated/figaro.cumulative.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      263 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/generated/figaro.decorators.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      397 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/generated/figaro.diagnostic.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      267 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/generated/figaro.load.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      211 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/generated/figaro.marginal.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      225 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/generated/figaro.mixture.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      201 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/generated/figaro.montecarlo.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      357 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/generated/figaro.plot.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      385 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/generated/figaro.transform.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      320 2023-11-15 13:14:25.000000 figaro-1.6.3/docs/source/generated/figaro.utils.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)     1009 2024-02-15 08:23:51.000000 figaro-1.6.3/docs/source/index.rst
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-23 15:24:31.909175 figaro-1.6.3/figaro/
--rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-01-16 16:50:38.000000 figaro-1.6.3/figaro/__init__.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     5008 2024-04-16 11:57:13.000000 figaro-1.6.3/figaro/_likelihood.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1612 2024-03-15 18:23:44.000000 figaro-1.6.3/figaro/_numba_functions.py
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-23 15:24:31.911086 figaro-1.6.3/figaro/_pipelines/
--rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-02-10 17:20:30.000000 figaro-1.6.3/figaro/_pipelines/__init__.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    19853 2024-04-23 15:23:17.000000 figaro-1.6.3/figaro/_pipelines/hierarchical_inference.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    23315 2024-04-23 15:23:41.000000 figaro-1.6.3/figaro/_pipelines/par_hierarchical_inference.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    10386 2024-04-18 07:25:21.000000 figaro-1.6.3/figaro/_pipelines/par_probability_density.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     9221 2024-04-18 07:25:04.000000 figaro-1.6.3/figaro/_pipelines/probability_density.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     2818 2024-04-18 07:51:37.000000 figaro-1.6.3/figaro/cosmology.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     7490 2024-02-10 17:20:30.000000 figaro-1.6.3/figaro/credible_regions.py
--rw-r--r--   0 rinaldi    (503) staff       (20)      785 2024-04-22 12:27:42.000000 figaro-1.6.3/figaro/cumulative.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1304 2024-04-17 14:55:45.000000 figaro-1.6.3/figaro/decorators.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     8460 2024-02-10 17:20:30.000000 figaro-1.6.3/figaro/diagnostic.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1249 2024-02-06 14:42:23.000000 figaro-1.6.3/figaro/exceptions.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    34199 2024-04-22 14:26:21.000000 figaro-1.6.3/figaro/load.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     6348 2024-04-16 13:52:44.000000 figaro-1.6.3/figaro/marginal.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    55429 2024-04-22 14:27:23.000000 figaro-1.6.3/figaro/mixture.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     2590 2024-02-10 17:20:30.000000 figaro-1.6.3/figaro/montecarlo.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    40427 2024-04-22 10:30:10.000000 figaro-1.6.3/figaro/plot.py
--rw-r--r--   0 rinaldi    (503) staff       (20)      933 2024-02-06 14:42:23.000000 figaro-1.6.3/figaro/plot_settings.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    12098 2024-04-23 13:33:43.000000 figaro-1.6.3/figaro/rate.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     3462 2024-02-13 11:17:19.000000 figaro-1.6.3/figaro/transform.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    16046 2024-04-17 08:40:42.000000 figaro-1.6.3/figaro/utils.py
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-23 15:24:31.911450 figaro-1.6.3/figaro.egg-info/
--rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-23 15:24:31.000000 figaro-1.6.3/figaro.egg-info/PKG-INFO
--rw-r--r--   0 rinaldi    (503) staff       (20)     1761 2024-04-23 15:24:31.000000 figaro-1.6.3/figaro.egg-info/SOURCES.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)        1 2024-04-23 15:24:31.000000 figaro-1.6.3/figaro.egg-info/dependency_links.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)      290 2024-04-23 15:24:31.000000 figaro-1.6.3/figaro.egg-info/entry_points.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)       76 2024-04-23 15:24:31.000000 figaro-1.6.3/figaro.egg-info/requires.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)        7 2024-04-23 15:24:31.000000 figaro-1.6.3/figaro.egg-info/top_level.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)     1988 2024-04-23 15:23:54.000000 figaro-1.6.3/pyproject.toml
--rw-r--r--   0 rinaldi    (503) staff       (20)       38 2024-04-23 15:24:31.911968 figaro-1.6.3/setup.cfg
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-29 10:57:10.433303 figaro-1.6.4/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1072 2023-11-15 13:14:25.000000 figaro-1.6.4/LICENSE
+-rw-r--r--   0 rinaldi    (503) staff       (20)       67 2024-02-10 17:20:30.000000 figaro-1.6.4/MANIFEST.in
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-29 10:57:10.433081 figaro-1.6.4/PKG-INFO
+-rw-r--r--   0 rinaldi    (503) staff       (20)     4154 2024-02-15 08:23:51.000000 figaro-1.6.4/README.md
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-29 10:57:10.416997 figaro-1.6.4/docs/
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-29 10:57:10.422284 figaro-1.6.4/docs/source/
+-rw-r--r--   0 rinaldi    (503) staff       (20)      317 2024-02-15 08:23:51.000000 figaro-1.6.4/docs/source/api.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.cosmology.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      159 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.credible_regions.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.cumulative.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.decorators.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.diagnostic.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2024-04-24 14:23:00.000000 figaro-1.6.4/docs/source/figaro.load.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      133 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.marginal.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      130 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.mixture.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.montecarlo.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.plot.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2024-04-24 14:23:08.000000 figaro-1.6.4/docs/source/figaro.rate.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      293 2024-02-15 08:23:51.000000 figaro-1.6.4/docs/source/figaro.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.transform.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      124 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/figaro.utils.rst
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-29 10:57:10.424393 figaro-1.6.4/docs/source/generated/
+-rw-r--r--   0 rinaldi    (503) staff       (20)      207 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.cosmology.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      363 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.credible_regions.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      231 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.cumulative.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      263 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.decorators.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      397 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.diagnostic.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      267 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.load.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      211 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.marginal.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      225 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.mixture.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      201 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.montecarlo.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      357 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.plot.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      385 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.transform.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      320 2023-11-15 13:14:25.000000 figaro-1.6.4/docs/source/generated/figaro.utils.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1009 2024-02-15 08:23:51.000000 figaro-1.6.4/docs/source/index.rst
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-29 10:57:10.430426 figaro-1.6.4/figaro/
+-rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-01-16 16:50:38.000000 figaro-1.6.4/figaro/__init__.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     5008 2024-04-16 11:57:13.000000 figaro-1.6.4/figaro/_likelihood.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1612 2024-03-15 18:23:44.000000 figaro-1.6.4/figaro/_numba_functions.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-29 10:57:10.432496 figaro-1.6.4/figaro/_pipelines/
+-rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-02-10 17:20:30.000000 figaro-1.6.4/figaro/_pipelines/__init__.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    19853 2024-04-23 15:23:17.000000 figaro-1.6.4/figaro/_pipelines/hierarchical_inference.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    23315 2024-04-26 15:10:23.000000 figaro-1.6.4/figaro/_pipelines/par_hierarchical_inference.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    10411 2024-04-29 10:56:16.000000 figaro-1.6.4/figaro/_pipelines/par_probability_density.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     9221 2024-04-18 07:25:04.000000 figaro-1.6.4/figaro/_pipelines/probability_density.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2818 2024-04-18 07:51:37.000000 figaro-1.6.4/figaro/cosmology.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     7490 2024-02-10 17:20:30.000000 figaro-1.6.4/figaro/credible_regions.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)      785 2024-04-22 12:27:42.000000 figaro-1.6.4/figaro/cumulative.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1304 2024-04-17 14:55:45.000000 figaro-1.6.4/figaro/decorators.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     8460 2024-02-10 17:20:30.000000 figaro-1.6.4/figaro/diagnostic.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1249 2024-02-06 14:42:23.000000 figaro-1.6.4/figaro/exceptions.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    34199 2024-04-22 14:26:21.000000 figaro-1.6.4/figaro/load.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6348 2024-04-16 13:52:44.000000 figaro-1.6.4/figaro/marginal.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    55429 2024-04-22 14:27:23.000000 figaro-1.6.4/figaro/mixture.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2590 2024-02-10 17:20:30.000000 figaro-1.6.4/figaro/montecarlo.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    40563 2024-04-26 15:09:38.000000 figaro-1.6.4/figaro/plot.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)      933 2024-04-23 20:48:47.000000 figaro-1.6.4/figaro/plot_settings.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    12084 2024-04-24 15:08:47.000000 figaro-1.6.4/figaro/rate.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     3462 2024-02-13 11:17:19.000000 figaro-1.6.4/figaro/transform.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    16046 2024-04-17 08:40:42.000000 figaro-1.6.4/figaro/utils.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-29 10:57:10.432811 figaro-1.6.4/figaro.egg-info/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-29 10:57:10.000000 figaro-1.6.4/figaro.egg-info/PKG-INFO
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1789 2024-04-29 10:57:10.000000 figaro-1.6.4/figaro.egg-info/SOURCES.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)        1 2024-04-29 10:57:10.000000 figaro-1.6.4/figaro.egg-info/dependency_links.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)      290 2024-04-29 10:57:10.000000 figaro-1.6.4/figaro.egg-info/entry_points.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)       76 2024-04-29 10:57:10.000000 figaro-1.6.4/figaro.egg-info/requires.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)        7 2024-04-29 10:57:10.000000 figaro-1.6.4/figaro.egg-info/top_level.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1988 2024-04-29 10:56:50.000000 figaro-1.6.4/pyproject.toml
+-rw-r--r--   0 rinaldi    (503) staff       (20)       38 2024-04-29 10:57:10.433352 figaro-1.6.4/setup.cfg
```

### Comparing `figaro-1.6.3/LICENSE` & `figaro-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/PKG-INFO` & `figaro-1.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.6.3
+Version: 1.6.4
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Author-email: Stefano Rinaldi <stefano.rinaldi@uni-heidelberg.de>, Walter Del Pozzo <walter.delpozzo@unipi.it>, Daniele Sanfratello <daniele.sanfratello@studenti.unipi.it>
 License: MIT License
         
         Copyright (c) 2022 Stefano Rinaldi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `figaro-1.6.3/README.md` & `figaro-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/docs/source/index.rst` & `figaro-1.6.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/_likelihood.py` & `figaro-1.6.4/figaro/_likelihood.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/_numba_functions.py` & `figaro-1.6.4/figaro/_numba_functions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/_pipelines/hierarchical_inference.py` & `figaro-1.6.4/figaro/_pipelines/hierarchical_inference.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/_pipelines/par_hierarchical_inference.py` & `figaro-1.6.4/figaro/_pipelines/par_hierarchical_inference.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/_pipelines/par_probability_density.py` & `figaro-1.6.4/figaro/_pipelines/par_probability_density.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pathlib import Path
 from tqdm import tqdm
 
 from figaro.mixture import DPGMM
 from figaro.utils import save_options, load_options, get_priors
 from figaro.plot import plot_median_cr, plot_multidim
-from figaro.load import load_single_event, save_density, load_density, supported_extensions, supported_pars
+from figaro.load import load_single_event, save_density, load_density, supported_extensions, supported_pars, load_selection_function
 
 import ray
 from ray.util import ActorPool
 
 @ray.remote
 class worker:
     def __init__(self, bounds,
```

### Comparing `figaro-1.6.3/figaro/_pipelines/probability_density.py` & `figaro-1.6.4/figaro/_pipelines/probability_density.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/cosmology.py` & `figaro-1.6.4/figaro/cosmology.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/credible_regions.py` & `figaro-1.6.4/figaro/credible_regions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/cumulative.py` & `figaro-1.6.4/figaro/cumulative.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/decorators.py` & `figaro-1.6.4/figaro/decorators.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/diagnostic.py` & `figaro-1.6.4/figaro/diagnostic.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/exceptions.py` & `figaro-1.6.4/figaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/load.py` & `figaro-1.6.4/figaro/load.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/marginal.py` & `figaro-1.6.4/figaro/marginal.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/mixture.py` & `figaro-1.6.4/figaro/mixture.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/montecarlo.py` & `figaro-1.6.4/figaro/montecarlo.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/plot.py` & `figaro-1.6.4/figaro/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,15 +261,16 @@
             np.savetxt(Path(txt_folder, 'prob_observed_{0}.txt'.format(name)), np.array([x, p[50], p[5], p[16], p[84], p[95]]).T, header = 'x 50 5 16 84 95')
     if show:
         ax.set_yscale('linear')
         ax.autoscale(True)
         if samples is not None:
             ax.set_xlim(xlim)
         plt.show()
-    plt.close()
+    if (save or show):
+        plt.close()
     
     # If selection function is available, plot reweighted distribution
     if selfunc is not None:
         for perc in percentiles:
             p[perc] = np.percentile((probs/f_x).T, perc, axis = 1)
         norm = p[50].sum()*dx
         for perc in percentiles:
@@ -301,14 +302,16 @@
             ax.autoscale(True)
             fig.savefig(Path(plot_folder, 'intrinsic_{0}.pdf'.format(name)), bbox_inches = 'tight')
             np.savetxt(Path(txt_folder, 'prob_intrinsic_{0}.txt'.format(name)), np.array([x, p[50], p[5], p[16], p[84], p[95]]).T, header = 'x 50 5 16 84 95')
         if show:
             ax.set_yscale('linear')
             ax.autoscale(True)
             plt.show()
+    
+    if (save or show):
         plt.close()
     return fig
 
 def plot_multidim(draws, samples = None, bounds = None, out_folder = '.', name = 'density', labels = None, units = None, hierarchical = False, show = False, save = True, subfolder = False, n_pts = 200, true_value = None, levels = [0.5, 0.68, 0.9], scatter_points = False, median_label = None, fig = None, colors = ['steelblue', 'darkturquoise', 'mediumturquoise'], colormap = 'Blues'):
     """
     Plot the recovered multidimensional distribution along with samples from the true distribution (if available) as corner plot.
     
@@ -543,15 +546,16 @@
         else:
             if not Path(out_folder, 'density').exists():
                 try:
                     Path(out_folder, 'density').mkdir()
                 except FileExistsError:
                     pass
             fig.savefig(Path(out_folder, 'density', '{0}.pdf'.format(name)), bbox_inches = 'tight')
-    plt.close()
+    if (save or show):
+        plt.close()
     return fig
     
 def plot_1d_dist(x, draws, injected = None, samples = None, out_folder = '.', name = 'density', label = None, unit = None, show = False, save = True, subfolder = False, true_value = None, true_value_label = '\mathrm{True\ value}', injected_label = '\mathrm{Simulated}', median_label = '\mathrm{Median}', logx = False, logy = False, colors = ['steelblue','darkturquoise','mediumturquoise'], fig = None):
     """
     Plot a 1D distribution along with samples from the true distribution (if available).
     Differently from plot_median_cr, this method requires the distribution to be already evaluated.
     For FIGARO mixture instances, please use plot_median_cr.
@@ -662,15 +666,16 @@
         fig.savefig(Path(plot_folder, '{0}.pdf'.format(name)), bbox_inches = 'tight')
         np.savetxt(Path(txt_folder, 'prob_{0}.txt'.format(name)), np.array([x, p[50], p[5], p[16], p[84], p[95]]).T, header = 'x 50 5 16 84 95')
     if show:
         ax.autoscale(True)
         if samples is not None:
             ax.set_xlim(xlim)
         plt.show()
-    plt.close()
+    if (save or show):
+        plt.close()
     return fig
 
 def plot_n_clusters_alpha(n_cl, alpha, out_folder = '.', name = 'event', show = False, save = True):
     """
     Plot the number of clusters and the concentration parameter as functions of the number of samples.
     
     Arguments:
@@ -785,15 +790,16 @@
     # Maquillage
     ax.set_xlabel('$P$')
     ax.set_ylabel('$\mathrm{Fraction\ of\ events\ within\ }CR_P$')
     if show:
         plt.show()
     if save:
         fig.savefig(Path(out_folder, '{0}_ppplot.pdf'.format(name)), bbox_inches = 'tight')
-    plt.close()
+    if (save or show):
+        plt.close()
     return fig
 
 def joyplot(draws, x_values, y_values, credible_regions = False, fill = True, solid = False, overlap = 1., xlabel = None, ylabel = None, xunit = None, yunit = None, colormap = 'coolwarm', out_folder = '.', name = 'joyplot', subfolder = False, show = False, save = True, joy = False):
     """
     Make a joyplot (also known as ridgeline plot) of a set of distributions.
     Heavily inspired by leotac's JoyPy (https://github.com/leotac/joypy).
```

### Comparing `figaro-1.6.3/figaro/plot_settings.py` & `figaro-1.6.4/figaro/plot_settings.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/rate.py` & `figaro-1.6.4/figaro/rate.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     VT_dist = []
     for d in draws:
         ss     = d.rvs(int(n_draws))
         comvol = dvdz(ss[:,z_index])
         sf     = selfunc(ss)
         VT_s   = T*sf*comvol/(1+ss[:,z_index])
         VT     = np.mean(VT_s)
-        S      = np.sqrt((0.3*VT)**2 + np.cov(VT_s)/n_draws)
+        S      = np.sqrt(np.cov(VT_s)/n_draws)
         VT_dist.append(norm(np.log(VT),S/VT))
     if each:
         return np.array([np.exp(VT_i.mean()) for VT_i in VT_dist])
     else:
         idx     = np.random.choice(np.arange(len(draws)), size = int(size))
         ctr     = Counter(idx)
         samples = np.empty(shape = (1,))
```

### Comparing `figaro-1.6.3/figaro/transform.py` & `figaro-1.6.4/figaro/transform.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro/utils.py` & `figaro-1.6.4/figaro/utils.py`

 * *Files identical despite different names*

### Comparing `figaro-1.6.3/figaro.egg-info/PKG-INFO` & `figaro-1.6.4/figaro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.6.3
+Version: 1.6.4
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Author-email: Stefano Rinaldi <stefano.rinaldi@uni-heidelberg.de>, Walter Del Pozzo <walter.delpozzo@unipi.it>, Daniele Sanfratello <daniele.sanfratello@studenti.unipi.it>
 License: MIT License
         
         Copyright (c) 2022 Stefano Rinaldi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `figaro-1.6.3/figaro.egg-info/SOURCES.txt` & `figaro-1.6.4/figaro.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 docs/source/figaro.decorators.rst
 docs/source/figaro.diagnostic.rst
 docs/source/figaro.load.rst
 docs/source/figaro.marginal.rst
 docs/source/figaro.mixture.rst
 docs/source/figaro.montecarlo.rst
 docs/source/figaro.plot.rst
+docs/source/figaro.rate.rst
 docs/source/figaro.rst
 docs/source/figaro.transform.rst
 docs/source/figaro.utils.rst
 docs/source/index.rst
 docs/source/generated/figaro.cosmology.rst
 docs/source/generated/figaro.credible_regions.rst
 docs/source/generated/figaro.cumulative.rst
```

### Comparing `figaro-1.6.3/pyproject.toml` & `figaro-1.6.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [tool.setuptools]
 packages = ['figaro', 'figaro._pipelines']
 
 [project]
 name = 'figaro'
 description = 'FIGARO: Fast Inference for GW Astronomy, Research & Observations'
-version = '1.6.3'
+version = '1.6.4'
 requires-python = '< 3.12'
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ['DPGMM', 'figaro', 'hierarchical', 'inference', 'HDPGMM']
 authors = [
   {name = "Stefano Rinaldi", email = "stefano.rinaldi@uni-heidelberg.de"},
   {name = "Walter Del Pozzo", email = "walter.delpozzo@unipi.it"},
```

