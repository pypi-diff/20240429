# Comparing `tmp/petitRADTRANS-2.7.6.tar.gz` & `tmp/petitRADTRANS-2.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petitRADTRANS-2.7.6.tar", last modified: Thu Nov 30 15:42:19 2023, max compression
+gzip compressed data, was "petitRADTRANS-2.7.7.tar", last modified: Mon Apr 29 09:47:11 2024, max compression
```

## Comparing `petitRADTRANS-2.7.6.tar` & `petitRADTRANS-2.7.7.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-11-30 15:42:19.953568 petitRADTRANS-2.7.6/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1062 2023-09-08 11:16:26.000000 petitRADTRANS-2.7.6/LICENSE
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1171 2023-11-30 15:42:19.953790 petitRADTRANS-2.7.6/PKG-INFO
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)      901 2023-09-08 11:16:26.000000 petitRADTRANS-2.7.6/README.rst
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-11-30 15:42:19.916942 petitRADTRANS-2.7.6/petitRADTRANS/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1960 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/__file_conversion.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)      420 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    17117 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/_read_opacities.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-11-30 15:42:19.922376 petitRADTRANS-2.7.6/petitRADTRANS/ccf/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-09-08 11:16:26.000000 petitRADTRANS-2.7.6/petitRADTRANS/ccf/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    31295 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/ccf/ccf.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3945 2023-09-08 11:16:26.000000 petitRADTRANS-2.7.6/petitRADTRANS/ccf/ccf_core.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-11-30 15:42:19.925543 petitRADTRANS-2.7.6/petitRADTRANS/cli/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-09-08 11:16:26.000000 petitRADTRANS-2.7.6/petitRADTRANS/cli/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     8878 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/cli/eso_etc_cli.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    16595 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/cli/eso_skycalc_cli.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-11-30 15:42:19.926834 petitRADTRANS-2.7.6/petitRADTRANS/config/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)       29 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/config/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     2408 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/config/configuration.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-11-30 15:42:19.928588 petitRADTRANS-2.7.6/petitRADTRANS/containers/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/containers/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    56238 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/containers/planet.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)   125896 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/containers/spectral_model.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    32158 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/fort_input.f90
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3936 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/fort_rebin.f90
--rwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)   124384 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/fort_spec.f90
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     9998 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/nat_cst.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    25524 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/physics.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-11-30 15:42:19.929589 petitRADTRANS-2.7.6/petitRADTRANS/poor_mans_nonequ_chem/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)       55 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/poor_mans_nonequ_chem/__init__.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-11-30 15:42:19.931029 petitRADTRANS-2.7.6/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)       56 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     4272 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/chem_fortran_util.f90
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-11-30 15:42:19.932139 petitRADTRANS-2.7.6/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)       63 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     4326 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/poor_mans_nonequ_chem.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     6934 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/pyth_input.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)   106780 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/radtrans.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-11-30 15:42:19.941676 petitRADTRANS-2.7.6/petitRADTRANS/retrieval/
--rwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)      362 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/retrieval/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    14758 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/retrieval/chemistry.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    29427 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/retrieval/cloud_cond.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    28405 2023-11-30 15:40:19.000000 petitRADTRANS-2.7.6/petitRADTRANS/retrieval/data.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    85769 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/retrieval/models.py
--rwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)     2516 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/retrieval/parameter.py
--rwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1661 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/retrieval/plot_style.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    32153 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/retrieval/plotting.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    21787 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/retrieval/preparing.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    12062 2023-11-30 15:40:20.000000 petitRADTRANS-2.7.6/petitRADTRANS/retrieval/psis.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3126 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/retrieval/rebin_give_width.f90
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)   155229 2023-11-30 15:40:20.000000 petitRADTRANS-2.7.6/petitRADTRANS/retrieval/retrieval.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    30182 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/retrieval/retrieval_config.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    12418 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/retrieval/util.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    13417 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/petitRADTRANS/utils.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)       18 2023-11-30 15:40:20.000000 petitRADTRANS-2.7.6/petitRADTRANS/version.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-11-30 15:42:19.920799 petitRADTRANS-2.7.6/petitRADTRANS.egg-info/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1171 2023-11-30 15:42:19.000000 petitRADTRANS-2.7.6/petitRADTRANS.egg-info/PKG-INFO
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     2422 2023-11-30 15:42:19.000000 petitRADTRANS-2.7.6/petitRADTRANS.egg-info/SOURCES.txt
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)        1 2023-11-30 15:42:19.000000 petitRADTRANS-2.7.6/petitRADTRANS.egg-info/dependency_links.txt
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)        1 2023-11-30 15:42:19.000000 petitRADTRANS-2.7.6/petitRADTRANS.egg-info/not-zip-safe
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)       84 2023-11-30 15:42:19.000000 petitRADTRANS-2.7.6/petitRADTRANS.egg-info/requires.txt
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)       20 2023-11-30 15:42:19.000000 petitRADTRANS-2.7.6/petitRADTRANS.egg-info/top_level.txt
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)      184 2023-11-30 15:42:19.954611 petitRADTRANS-2.7.6/setup.cfg
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3055 2023-11-30 15:40:20.000000 petitRADTRANS-2.7.6/setup.py
-drwxr-xr-x   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-11-30 15:42:19.953136 petitRADTRANS-2.7.6/tests/
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)        0 2023-09-08 11:16:26.000000 petitRADTRANS-2.7.6/tests/__init__.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3008 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/_test_CO_line_lists.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3070 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/_test_H2O_line_lists.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3263 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/_test_TiO_line_lists.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     2628 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/_test_data.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1698 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/_test_high_res.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3567 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/_test_line_shapes_alkalis.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1190 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/context.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    42081 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/reference_files_generators.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3695 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/test_chemistry.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)      536 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/test_fortran_modules.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     1449 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/test_planet.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    14456 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/test_radtrans_correlated_k.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     9466 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/test_radtrans_correlated_k_scattering.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     3139 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/test_radtrans_correlated_k_surface_scattering.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    15440 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/test_radtrans_line_by_line.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     2967 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/test_radtrans_line_by_line_sampling.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    11355 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/test_retrieval.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)     2660 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/test_utility_functions.py
--rw-r--r--   0 molliere (1984917825) MPIA\Domain Users (1357073302)    14324 2023-11-30 15:39:50.000000 petitRADTRANS-2.7.6/tests/utils.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2024-04-29 09:47:11.701710 petitRADTRANS-2.7.7/
+-rw-r--r--   0 molliere (1984917825) 1357073302     1062 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/LICENSE
+-rw-r--r--   0 molliere (1984917825) 1357073302     1420 2024-04-29 09:47:11.701563 petitRADTRANS-2.7.7/PKG-INFO
+-rw-r--r--   0 molliere (1984917825) 1357073302      901 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/README.rst
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2024-04-29 09:47:11.672165 petitRADTRANS-2.7.7/petitRADTRANS/
+-rw-r--r--   0 molliere (1984917825) 1357073302     1960 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/__file_conversion.py
+-rw-r--r--   0 molliere (1984917825) 1357073302      420 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    17117 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/_read_opacities.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2024-04-29 09:47:11.675631 petitRADTRANS-2.7.7/petitRADTRANS/ccf/
+-rw-r--r--   0 molliere (1984917825) 1357073302        0 2023-09-08 11:16:26.000000 petitRADTRANS-2.7.7/petitRADTRANS/ccf/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    31295 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/ccf/ccf.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3945 2023-09-08 11:16:26.000000 petitRADTRANS-2.7.7/petitRADTRANS/ccf/ccf_core.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2024-04-29 09:47:11.677176 petitRADTRANS-2.7.7/petitRADTRANS/cli/
+-rw-r--r--   0 molliere (1984917825) 1357073302        0 2023-09-08 11:16:26.000000 petitRADTRANS-2.7.7/petitRADTRANS/cli/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     8878 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/cli/eso_etc_cli.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    16595 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/cli/eso_skycalc_cli.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2024-04-29 09:47:11.678794 petitRADTRANS-2.7.7/petitRADTRANS/config/
+-rw-r--r--   0 molliere (1984917825) 1357073302       29 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/config/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     2408 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/config/configuration.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2024-04-29 09:47:11.680488 petitRADTRANS-2.7.7/petitRADTRANS/containers/
+-rw-r--r--   0 molliere (1984917825) 1357073302        0 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/containers/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    56238 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/containers/planet.py
+-rw-r--r--   0 molliere (1984917825) 1357073302   125896 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/containers/spectral_model.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    32158 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/fort_input.f90
+-rw-r--r--   0 molliere (1984917825) 1357073302     3936 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/fort_rebin.f90
+-rwxr-xr-x   0 molliere (1984917825) 1357073302   124384 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/fort_spec.f90
+-rw-r--r--   0 molliere (1984917825) 1357073302     9998 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/nat_cst.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    25524 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/physics.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2024-04-29 09:47:11.682248 petitRADTRANS-2.7.7/petitRADTRANS/poor_mans_nonequ_chem/
+-rw-r--r--   0 molliere (1984917825) 1357073302       55 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/poor_mans_nonequ_chem/__init__.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2024-04-29 09:47:11.683015 petitRADTRANS-2.7.7/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/
+-rw-r--r--   0 molliere (1984917825) 1357073302       56 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     4272 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/chem_fortran_util.f90
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2024-04-29 09:47:11.683777 petitRADTRANS-2.7.7/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/
+-rw-r--r--   0 molliere (1984917825) 1357073302       63 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     4326 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/poor_mans_nonequ_chem.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     6934 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/pyth_input.py
+-rw-r--r--   0 molliere (1984917825) 1357073302   106780 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/radtrans.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2024-04-29 09:47:11.692388 petitRADTRANS-2.7.7/petitRADTRANS/retrieval/
+-rwxr-xr-x   0 molliere (1984917825) 1357073302      362 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/retrieval/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    14758 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/retrieval/chemistry.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    29427 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/retrieval/cloud_cond.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    28405 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/retrieval/data.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    85769 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/retrieval/models.py
+-rwxr-xr-x   0 molliere (1984917825) 1357073302     2516 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/retrieval/parameter.py
+-rwxr-xr-x   0 molliere (1984917825) 1357073302     1661 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/retrieval/plot_style.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    32153 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/retrieval/plotting.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    21787 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/retrieval/preparing.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    12062 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/retrieval/psis.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3126 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/retrieval/rebin_give_width.f90
+-rw-r--r--   0 molliere (1984917825) 1357073302   155229 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/retrieval/retrieval.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    30182 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/retrieval/retrieval_config.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    12418 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/retrieval/util.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    13417 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/utils.py
+-rw-r--r--   0 molliere (1984917825) 1357073302       18 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/petitRADTRANS/version.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2024-04-29 09:47:11.674456 petitRADTRANS-2.7.7/petitRADTRANS.egg-info/
+-rw-r--r--   0 molliere (1984917825) 1357073302     1420 2024-04-29 09:47:11.000000 petitRADTRANS-2.7.7/petitRADTRANS.egg-info/PKG-INFO
+-rw-r--r--   0 molliere (1984917825) 1357073302     2422 2024-04-29 09:47:11.000000 petitRADTRANS-2.7.7/petitRADTRANS.egg-info/SOURCES.txt
+-rw-r--r--   0 molliere (1984917825) 1357073302        1 2024-04-29 09:47:11.000000 petitRADTRANS-2.7.7/petitRADTRANS.egg-info/dependency_links.txt
+-rw-r--r--   0 molliere (1984917825) 1357073302        1 2024-04-29 09:47:11.000000 petitRADTRANS-2.7.7/petitRADTRANS.egg-info/not-zip-safe
+-rw-r--r--   0 molliere (1984917825) 1357073302       84 2024-04-29 09:47:11.000000 petitRADTRANS-2.7.7/petitRADTRANS.egg-info/requires.txt
+-rw-r--r--   0 molliere (1984917825) 1357073302       20 2024-04-29 09:47:11.000000 petitRADTRANS-2.7.7/petitRADTRANS.egg-info/top_level.txt
+-rw-r--r--   0 molliere (1984917825) 1357073302      184 2024-04-29 09:47:11.702158 petitRADTRANS-2.7.7/setup.cfg
+-rw-r--r--   0 molliere (1984917825) 1357073302     3055 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/setup.py
+drwxr-xr-x   0 molliere (1984917825) 1357073302        0 2024-04-29 09:47:11.700820 petitRADTRANS-2.7.7/tests/
+-rw-r--r--   0 molliere (1984917825) 1357073302        0 2023-09-08 11:16:26.000000 petitRADTRANS-2.7.7/tests/__init__.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3008 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/_test_CO_line_lists.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3070 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/_test_H2O_line_lists.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3263 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/_test_TiO_line_lists.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     2628 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/_test_data.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     1698 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/_test_high_res.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3567 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/_test_line_shapes_alkalis.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     1190 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/context.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    42081 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/reference_files_generators.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3695 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/test_chemistry.py
+-rw-r--r--   0 molliere (1984917825) 1357073302      536 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/test_fortran_modules.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     1449 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/test_planet.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    14456 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/test_radtrans_correlated_k.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     9466 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/test_radtrans_correlated_k_scattering.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     3139 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/test_radtrans_correlated_k_surface_scattering.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    15440 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/test_radtrans_line_by_line.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     2967 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/test_radtrans_line_by_line_sampling.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    11355 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/test_retrieval.py
+-rw-r--r--   0 molliere (1984917825) 1357073302     2660 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/test_utility_functions.py
+-rw-r--r--   0 molliere (1984917825) 1357073302    14324 2024-04-29 09:42:38.000000 petitRADTRANS-2.7.7/tests/utils.py
```

### Comparing `petitRADTRANS-2.7.6/LICENSE` & `petitRADTRANS-2.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/PKG-INFO` & `petitRADTRANS-2.7.7/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: petitRADTRANS
-Version: 2.7.6
-Summary: Exoplanet spectral synthesis tool for retrievals
-Home-page: https://gitlab.com/mauricemolli/petitRADTRANS
-Author: Paul Mollière
-Author-email: molliere@mpia.de
-License: MIT License
-License-File: LICENSE
-
 petitRADTRANS
 =============
 
 **An easy-to-use Python package for calculating exoplanet spectra**
 
 Welcome to the repository of petitRADTRANS, an easy-to-use code for the calculation of exoplanet spectra.
 petitRADTRANS allows the calculation of emission or transmission spectra, at low or high resolution, clear or cloudy,
```

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/__file_conversion.py` & `petitRADTRANS-2.7.7/petitRADTRANS/__file_conversion.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/_read_opacities.py` & `petitRADTRANS-2.7.7/petitRADTRANS/_read_opacities.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/ccf/ccf.py` & `petitRADTRANS-2.7.7/petitRADTRANS/ccf/ccf.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/ccf/ccf_core.py` & `petitRADTRANS-2.7.7/petitRADTRANS/ccf/ccf_core.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/cli/eso_etc_cli.py` & `petitRADTRANS-2.7.7/petitRADTRANS/cli/eso_etc_cli.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/cli/eso_skycalc_cli.py` & `petitRADTRANS-2.7.7/petitRADTRANS/cli/eso_skycalc_cli.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/config/configuration.py` & `petitRADTRANS-2.7.7/petitRADTRANS/config/configuration.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/containers/planet.py` & `petitRADTRANS-2.7.7/petitRADTRANS/containers/planet.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/containers/spectral_model.py` & `petitRADTRANS-2.7.7/petitRADTRANS/containers/spectral_model.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/fort_input.f90` & `petitRADTRANS-2.7.7/petitRADTRANS/fort_input.f90`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/fort_rebin.f90` & `petitRADTRANS-2.7.7/petitRADTRANS/fort_rebin.f90`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/fort_spec.f90` & `petitRADTRANS-2.7.7/petitRADTRANS/fort_spec.f90`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/nat_cst.py` & `petitRADTRANS-2.7.7/petitRADTRANS/nat_cst.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/physics.py` & `petitRADTRANS-2.7.7/petitRADTRANS/physics.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/chem_fortran_util.f90` & `petitRADTRANS-2.7.7/petitRADTRANS/poor_mans_nonequ_chem/chem_fortran_util/chem_fortran_util.f90`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/poor_mans_nonequ_chem.py` & `petitRADTRANS-2.7.7/petitRADTRANS/poor_mans_nonequ_chem/poor_mans_nonequ_chem/poor_mans_nonequ_chem.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/pyth_input.py` & `petitRADTRANS-2.7.7/petitRADTRANS/pyth_input.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/radtrans.py` & `petitRADTRANS-2.7.7/petitRADTRANS/radtrans.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/retrieval/chemistry.py` & `petitRADTRANS-2.7.7/petitRADTRANS/retrieval/chemistry.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/retrieval/cloud_cond.py` & `petitRADTRANS-2.7.7/petitRADTRANS/retrieval/cloud_cond.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/retrieval/data.py` & `petitRADTRANS-2.7.7/petitRADTRANS/retrieval/data.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/retrieval/models.py` & `petitRADTRANS-2.7.7/petitRADTRANS/retrieval/models.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/retrieval/parameter.py` & `petitRADTRANS-2.7.7/petitRADTRANS/retrieval/parameter.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/retrieval/plot_style.py` & `petitRADTRANS-2.7.7/petitRADTRANS/retrieval/plot_style.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/retrieval/plotting.py` & `petitRADTRANS-2.7.7/petitRADTRANS/retrieval/plotting.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/retrieval/preparing.py` & `petitRADTRANS-2.7.7/petitRADTRANS/retrieval/preparing.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/retrieval/psis.py` & `petitRADTRANS-2.7.7/petitRADTRANS/retrieval/psis.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/retrieval/rebin_give_width.f90` & `petitRADTRANS-2.7.7/petitRADTRANS/retrieval/rebin_give_width.f90`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/retrieval/retrieval.py` & `petitRADTRANS-2.7.7/petitRADTRANS/retrieval/retrieval.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/retrieval/retrieval_config.py` & `petitRADTRANS-2.7.7/petitRADTRANS/retrieval/retrieval_config.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/retrieval/util.py` & `petitRADTRANS-2.7.7/petitRADTRANS/retrieval/util.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS/utils.py` & `petitRADTRANS-2.7.7/petitRADTRANS/utils.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/petitRADTRANS.egg-info/SOURCES.txt` & `petitRADTRANS-2.7.7/petitRADTRANS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/setup.py` & `petitRADTRANS-2.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 
 def setup_function():
     # from petitRADTRANS.version import version  # future, this cannot be done right now due to the imports in __init__
 
     setup(
         name='petitRADTRANS',
-        version='2.7.6',
+        version='2.7.7',
         description='Exoplanet spectral synthesis tool for retrievals',
         long_description=open(os.path.join(
           os.path.dirname(__file__), 'README.rst')).read(),
         # long_description_content_type='test/x-rst',
         url='https://gitlab.com/mauricemolli/petitRADTRANS',
         author='Paul Mollière',
         author_email='molliere@mpia.de',
```

### Comparing `petitRADTRANS-2.7.6/tests/_test_CO_line_lists.py` & `petitRADTRANS-2.7.7/tests/_test_CO_line_lists.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/_test_H2O_line_lists.py` & `petitRADTRANS-2.7.7/tests/_test_H2O_line_lists.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/_test_TiO_line_lists.py` & `petitRADTRANS-2.7.7/tests/_test_TiO_line_lists.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/_test_data.py` & `petitRADTRANS-2.7.7/tests/_test_data.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/_test_high_res.py` & `petitRADTRANS-2.7.7/tests/_test_high_res.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/_test_line_shapes_alkalis.py` & `petitRADTRANS-2.7.7/tests/_test_line_shapes_alkalis.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/context.py` & `petitRADTRANS-2.7.7/tests/context.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/reference_files_generators.py` & `petitRADTRANS-2.7.7/tests/reference_files_generators.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/test_chemistry.py` & `petitRADTRANS-2.7.7/tests/test_chemistry.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/test_fortran_modules.py` & `petitRADTRANS-2.7.7/tests/test_fortran_modules.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/test_planet.py` & `petitRADTRANS-2.7.7/tests/test_planet.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/test_radtrans_correlated_k.py` & `petitRADTRANS-2.7.7/tests/test_radtrans_correlated_k.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/test_radtrans_correlated_k_scattering.py` & `petitRADTRANS-2.7.7/tests/test_radtrans_correlated_k_scattering.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/test_radtrans_correlated_k_surface_scattering.py` & `petitRADTRANS-2.7.7/tests/test_radtrans_correlated_k_surface_scattering.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/test_radtrans_line_by_line.py` & `petitRADTRANS-2.7.7/tests/test_radtrans_line_by_line.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/test_radtrans_line_by_line_sampling.py` & `petitRADTRANS-2.7.7/tests/test_radtrans_line_by_line_sampling.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/test_retrieval.py` & `petitRADTRANS-2.7.7/tests/test_retrieval.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/test_utility_functions.py` & `petitRADTRANS-2.7.7/tests/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `petitRADTRANS-2.7.6/tests/utils.py` & `petitRADTRANS-2.7.7/tests/utils.py`

 * *Files identical despite different names*

