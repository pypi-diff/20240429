# Comparing `tmp/mri_nufft-0.7.0.tar.gz` & `tmp/mri_nufft-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mri_nufft-0.7.0.tar", last modified: Wed Apr 24 13:22:02 2024, max compression
+gzip compressed data, was "mri_nufft-0.8.0.tar", last modified: Mon Apr 29 16:11:01 2024, max compression
```

## Comparing `mri_nufft-0.7.0.tar` & `mri_nufft-0.8.0.tar`

### file list

```diff
@@ -1,117 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.968195 mri_nufft-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.944195 mri_nufft-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.948195 mri_nufft-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/.github/workflows/master-cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/.github/workflows/tags-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/.github/workflows/test-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-24 13:22:02.968195 mri_nufft-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.952195 mri_nufft-0.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.944195 mri_nufft-0.7.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.952195 mri_nufft-0.7.0/docs/_static/logos/
--rw-r--r--   0 runner    (1001) docker     (127)    16114 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/_static/logos/mri-nufft-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    42804 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/_static/logos/mri-nufft.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.944195 mri_nufft-0.7.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.952195 mri_nufft-0.7.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/_templates/autosummary/function.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.952195 mri_nufft-0.7.0/docs/misc/
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/misc/code_of_conduct.rst
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/misc/contributors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/misc/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/misc/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/misc/related.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/nufft.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/docs/trajectory_gradspec.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.956195 mri_nufft-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    20674 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_2D_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)    27864 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_3D_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_display_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_gif_2D.py
--rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_gif_3D.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_stacked.py
--rw-r--r--   0 runner    (1001) docker     (127)    26645 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/examples/example_trajectory_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:22:02.968195 mri_nufft-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.948195 mri_nufft-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.964195 mri_nufft-0.7.0/src/mri_nufft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-24 13:22:02.000000 mri_nufft-0.7.0/src/mri_nufft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-24 13:22:02.000000 mri_nufft-0.7.0/src/mri_nufft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:22:02.000000 mri_nufft-0.7.0/src/mri_nufft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-24 13:22:02.000000 mri_nufft-0.7.0/src/mri_nufft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 13:22:02.000000 mri_nufft-0.7.0/src/mri_nufft.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.956195 mri_nufft-0.7.0/src/mrinufft/
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 13:22:02.000000 mri_nufft-0.7.0/src/mrinufft/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.956195 mri_nufft-0.7.0/src/mrinufft/density/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/density/geometry_based.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/density/nufft_based.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/density/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.956195 mri_nufft-0.7.0/src/mrinufft/io/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/io/cfl.py
--rw-r--r--   0 runner    (1001) docker     (127)    13563 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/io/nsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.956195 mri_nufft-0.7.0/src/mrinufft/operators/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.960195 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/_cupy_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/bart.py
--rw-r--r--   0 runner    (1001) docker     (127)    28594 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/cufinufft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/finufft.py
--rw-r--r--   0 runner    (1001) docker     (127)    18609 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/gpunufft.py
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/nfft.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/nudft_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/pynufft_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/sigpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/tfnufft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.960195 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/css_color.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/gpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/off_resonnance.py
--rw-r--r--   0 runner    (1001) docker     (127)    30205 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/operators/stacked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.960195 mri_nufft-0.7.0/src/mrinufft/trajectories/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/trajectories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23371 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/trajectories/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/trajectories/maths.py
--rw-r--r--   0 runner    (1001) docker     (127)    18665 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/trajectories/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/trajectories/trajectory2D.py
--rw-r--r--   0 runner    (1001) docker     (127)    23461 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/trajectories/trajectory3D.py
--rw-r--r--   0 runner    (1001) docker     (127)    13997 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/src/mrinufft/trajectories/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.964195 mri_nufft-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/case_trajectories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.964195 mri_nufft-0.7.0/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/helpers/asserts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/helpers/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:22:02.964195 mri_nufft-0.7.0/tests/operators/
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/operators/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/operators/test_bindings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/operators/test_gpunufft.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/operators/test_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/operators/test_stacked.py
--rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/operators/test_stacked_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/test_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-24 13:21:40.000000 mri_nufft-0.7.0/tests/test_ndft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.800830 mri_nufft-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.772829 mri_nufft-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.776829 mri_nufft-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/.github/workflows/master-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/.github/workflows/tags-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/.github/workflows/test-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-29 16:11:01.800830 mri_nufft-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.776829 mri_nufft-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.776829 mri_nufft-0.8.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.780830 mri_nufft-0.8.0/docs/_static/logos/
+-rw-r--r--   0 runner    (1001) docker     (127)    16114 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/_static/logos/mri-nufft-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42804 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/_static/logos/mri-nufft.png
+-rw-r--r--   0 runner    (1001) docker     (127)  2581573 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/_static/mri-nufft-scheme.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.772829 mri_nufft-0.8.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.780830 mri_nufft-0.8.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.784829 mri_nufft-0.8.0/docs/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/misc/code_of_conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/misc/contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/misc/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/misc/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/misc/related.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10064 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/nufft.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/docs/trajectory_gradspec.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.784829 mri_nufft-0.8.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/examples/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/examples/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20674 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/examples/example_2D_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27864 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/examples/example_3D_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/examples/example_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/examples/example_display_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/examples/example_gif_2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9786 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/examples/example_gif_3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/examples/example_readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/examples/example_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26645 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/examples/example_trajectory_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 16:11:01.800830 mri_nufft-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.772829 mri_nufft-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.796830 mri_nufft-0.8.0/src/mri_nufft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-29 16:11:01.000000 mri_nufft-0.8.0/src/mri_nufft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-29 16:11:01.000000 mri_nufft-0.8.0/src/mri_nufft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:11:01.000000 mri_nufft-0.8.0/src/mri_nufft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-29 16:11:01.000000 mri_nufft-0.8.0/src/mri_nufft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 16:11:01.000000 mri_nufft-0.8.0/src/mri_nufft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.788830 mri_nufft-0.8.0/src/mrinufft/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 16:11:01.000000 mri_nufft-0.8.0/src/mrinufft/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.788830 mri_nufft-0.8.0/src/mrinufft/density/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/density/geometry_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/density/nufft_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/density/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.788830 mri_nufft-0.8.0/src/mrinufft/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/io/cfl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/io/nsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.788830 mri_nufft-0.8.0/src/mrinufft/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/autodiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22420 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.792830 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/_cupy_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/bart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28594 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/cufinufft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/finufft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21678 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/gpunufft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/nfft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/nudft_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/pynufft_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/sigpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/tfnufft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.792830 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/utils/css_color.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/utils/gpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/interfaces/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/off_resonnance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30205 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/operators/stacked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.792830 mri_nufft-0.8.0/src/mrinufft/trajectories/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/trajectories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23371 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/trajectories/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/trajectories/maths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18665 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/trajectories/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12507 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/trajectories/trajectory2D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23461 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/trajectories/trajectory3D.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13997 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/src/mrinufft/trajectories/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.796830 mri_nufft-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/case_trajectories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.796830 mri_nufft-0.8.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/helpers/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/helpers/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:11:01.796830 mri_nufft-0.8.0/tests/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/operators/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/operators/test_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/operators/test_gpunufft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/operators/test_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/operators/test_operator_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/operators/test_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4916 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/operators/test_stacked_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/test_autodiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/test_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-29 16:10:41.000000 mri_nufft-0.8.0/tests/test_ndft.py
```

### Comparing `mri_nufft-0.7.0/.github/workflows/master-cd.yml` & `mri_nufft-0.8.0/.github/workflows/master-cd.yml`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/.github/workflows/style.yml` & `mri_nufft-0.8.0/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/.github/workflows/tags-release.yml` & `mri_nufft-0.8.0/.github/workflows/tags-release.yml`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/.github/workflows/test-ci.yml` & `mri_nufft-0.8.0/.github/workflows/test-ci.yml`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
           cache: pip
 
       - name: Install Python deps
         shell: bash
         run: |
           python -m pip install --upgrade pip
           python -m pip install -e .[test,dev]
-          python -m pip install finufft pooch brainweb-dl
+          python -m pip install finufft pooch brainweb-dl torch
 
       - name: Run examples
         shell: bash
         run: |
           export COVERAGE_FILE=coverage_plots
           pytest examples tests -k="not operators" --cov --cov-branch --cov-report=term
```

### Comparing `mri_nufft-0.7.0/LICENSE.txt` & `mri_nufft-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/PKG-INFO` & `mri_nufft-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mri-nufft
-Version: 0.7.0
+Version: 0.8.0
 Summary: MRI Non-Cartesian Fourier Operators with multiple computation backends.
 Author-email: Pierre-antoine Comby <pierre-antoine.comby@crans.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
@@ -19,14 +19,16 @@
 Provides-Extra: finufft
 Requires-Dist: finufft; extra == "finufft"
 Provides-Extra: pynfft
 Requires-Dist: pynfft2; extra == "pynfft"
 Requires-Dist: cython<3.0.0; extra == "pynfft"
 Provides-Extra: pynufft
 Requires-Dist: pynufft; extra == "pynufft"
+Provides-Extra: io
+Requires-Dist: pymapvbvd; extra == "io"
 Provides-Extra: test
 Requires-Dist: pytest<8.0.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: pytest-sugar; extra == "test"
 Requires-Dist: pytest-cases; extra == "test"
 Provides-Extra: dev
```

### Comparing `mri_nufft-0.7.0/README.rst` & `mri_nufft-0.8.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,27 @@
         :target: https://pypi.org/project/mri-nufft/
 
 
 This python package extends various NUFFT (Non-Uniform Fast Fourier Transform) python bindings used for MRI reconstruction.
 
 In particular, it provides a unified interface for all the methods, with extra features such as coil sensitivity, density compensated adjoint and off-resonance corrections (for static B0 inhomogeneities).
 
+.. raw:: html 
+   
+   <div align="center">
+
+.. image:: https://github.com/mind-inria/mri-nufft/raw/master/docs/_static/mri-nufft-scheme.svg
+   :width: 700
+   :align: center
+
+Modularity and Integration of MRI-nufft with the python computing libraries.
+
+.. raw:: html 
+   
+   </div>
 
 Usage
 =====
 
 .. TODO use a include file directive.
 .. code-block:: python
 
@@ -60,15 +73,15 @@
 
 For best image quality, embed these steps in a more complex reconstruction pipeline (for instance using `PySAP <https://github.com/CEA-COSMIC/pysap-mri>`_).
 
 Want to see more ?
 
 - Check the `Documentation <https://mind-inria.github.io/mri-nufft/>`_
 
-- Or go visit the `Examples <https://mind-inria.github.io/mri-nufft/autoexamples/index.html>`_
+- Or go visit the `Examples <https://mind-inria.github.io/mri-nufft/generated/autoexamples/index.html>`_
 
 
 Installation
 ------------
 
 MRI-nufft is available on Pypi and can be installed with::
```

### Comparing `mri_nufft-0.7.0/docs/Makefile` & `mri_nufft-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/docs/_static/logos/mri-nufft-icon.png` & `mri_nufft-0.8.0/docs/_static/logos/mri-nufft-icon.png`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/docs/_static/logos/mri-nufft.png` & `mri_nufft-0.8.0/docs/_static/logos/mri-nufft.png`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/docs/_templates/autosummary/class.rst` & `mri_nufft-0.8.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/docs/_templates/autosummary/module.rst` & `mri_nufft-0.8.0/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/docs/conf.py` & `mri_nufft-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/docs/getting_started.rst` & `mri_nufft-0.8.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/docs/index.rst` & `mri_nufft-0.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/docs/misc/code_of_conduct.rst` & `mri_nufft-0.8.0/docs/misc/code_of_conduct.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/docs/misc/development.rst` & `mri_nufft-0.8.0/docs/misc/development.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/docs/nufft.rst` & `mri_nufft-0.8.0/docs/nufft.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/docs/trajectory_gradspec.rst` & `mri_nufft-0.8.0/docs/trajectory_gradspec.rst`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/examples/conftest.py` & `mri_nufft-0.8.0/examples/conftest.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/examples/example_2D_trajectories.py` & `mri_nufft-0.8.0/examples/example_2D_trajectories.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/examples/example_3D_trajectories.py` & `mri_nufft-0.8.0/examples/example_3D_trajectories.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/examples/example_density.py` & `mri_nufft-0.8.0/examples/example_density.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/examples/example_display_config.py` & `mri_nufft-0.8.0/examples/example_display_config.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/examples/example_gif_2D.py` & `mri_nufft-0.8.0/examples/example_gif_2D.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/examples/example_gif_3D.py` & `mri_nufft-0.8.0/examples/example_gif_3D.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/examples/example_readme.py` & `mri_nufft-0.8.0/examples/example_readme.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/examples/example_stacked.py` & `mri_nufft-0.8.0/examples/example_stacked.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/examples/example_trajectory_tools.py` & `mri_nufft-0.8.0/examples/example_trajectory_tools.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/pyproject.toml` & `mri_nufft-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 [project.optional-dependencies]
 
 gpunufft = ["gpuNUFFT>=0.7.5", "cupy-cuda11x"]
 cufinufft = ["cufinufft", "cupy-cuda11x"]
 finufft = ["finufft"]
 pynfft = ["pynfft2", "cython<3.0.0"]
 pynufft = ["pynufft"]
+io = ["pymapvbvd"]
 
 test = ["pytest<8.0.0", "pytest-cov", "pytest-xdist", "pytest-sugar", "pytest-cases"]
 dev = ["black", "isort", "ruff"]
 doc = ["sphinx-book-theme","sphinx-copybutton", "sphinx-gallery", "matplotlib", "pooch", "brainweb-dl"]
 # pooch is for scipy.datasets
 
 [build-system]
```

### Comparing `mri_nufft-0.7.0/src/mri_nufft.egg-info/PKG-INFO` & `mri_nufft-0.8.0/src/mri_nufft.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mri-nufft
-Version: 0.7.0
+Version: 0.8.0
 Summary: MRI Non-Cartesian Fourier Operators with multiple computation backends.
 Author-email: Pierre-antoine Comby <pierre-antoine.comby@crans.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
@@ -19,14 +19,16 @@
 Provides-Extra: finufft
 Requires-Dist: finufft; extra == "finufft"
 Provides-Extra: pynfft
 Requires-Dist: pynfft2; extra == "pynfft"
 Requires-Dist: cython<3.0.0; extra == "pynfft"
 Provides-Extra: pynufft
 Requires-Dist: pynufft; extra == "pynufft"
+Provides-Extra: io
+Requires-Dist: pymapvbvd; extra == "io"
 Provides-Extra: test
 Requires-Dist: pytest<8.0.0; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-xdist; extra == "test"
 Requires-Dist: pytest-sugar; extra == "test"
 Requires-Dist: pytest-cases; extra == "test"
 Provides-Extra: dev
```

### Comparing `mri_nufft-0.7.0/src/mri_nufft.egg-info/SOURCES.txt` & `mri_nufft-0.8.0/src/mri_nufft.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/getting_started.rst
 docs/index.rst
 docs/nufft.rst
 docs/trajectory_gradspec.rst
+docs/_static/mri-nufft-scheme.svg
 docs/_static/logos/mri-nufft-icon.png
 docs/_static/logos/mri-nufft.png
 docs/_templates/autosummary/base.rst
 docs/_templates/autosummary/class.rst
 docs/_templates/autosummary/function.rst
 docs/_templates/autosummary/module.rst
 docs/misc/code_of_conduct.rst
@@ -47,15 +48,17 @@
 src/mrinufft/density/__init__.py
 src/mrinufft/density/geometry_based.py
 src/mrinufft/density/nufft_based.py
 src/mrinufft/density/utils.py
 src/mrinufft/io/__init__.py
 src/mrinufft/io/cfl.py
 src/mrinufft/io/nsp.py
+src/mrinufft/io/utils.py
 src/mrinufft/operators/__init__.py
+src/mrinufft/operators/autodiff.py
 src/mrinufft/operators/base.py
 src/mrinufft/operators/off_resonnance.py
 src/mrinufft/operators/stacked.py
 src/mrinufft/operators/interfaces/__init__.py
 src/mrinufft/operators/interfaces/_cupy_kernels.py
 src/mrinufft/operators/interfaces/bart.py
 src/mrinufft/operators/interfaces/cufinufft.py
@@ -75,19 +78,21 @@
 src/mrinufft/trajectories/maths.py
 src/mrinufft/trajectories/tools.py
 src/mrinufft/trajectories/trajectory2D.py
 src/mrinufft/trajectories/trajectory3D.py
 src/mrinufft/trajectories/utils.py
 tests/case_trajectories.py
 tests/conftest.py
+tests/test_autodiff.py
 tests/test_density.py
 tests/test_io.py
 tests/test_ndft.py
 tests/helpers/__init__.py
 tests/helpers/asserts.py
 tests/helpers/factories.py
 tests/operators/test_batch.py
 tests/operators/test_bindings.py
 tests/operators/test_gpunufft.py
 tests/operators/test_interfaces.py
+tests/operators/test_operator_ref.py
 tests/operators/test_stacked.py
 tests/operators/test_stacked_gpu.py
```

### Comparing `mri_nufft-0.7.0/src/mrinufft/__init__.py` & `mri_nufft-0.8.0/src/mrinufft/__init__.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/_utils.py` & `mri_nufft-0.8.0/src/mrinufft/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from functools import wraps
 import numpy as np
 from numpy.typing import DTypeLike
 
 
 ARRAY_LIBS = {
     "numpy": (np, np.ndarray),
-    "cupy": None,
-    "torch": None,
-    "tensorflow": None,
+    "cupy": (None, None),
+    "torch": (None, None),
+    "tensorflow": (None, None),
 }
 try:
     import cupy
 
     ARRAY_LIBS["cupy"] = (cupy, cupy.ndarray)
 except ImportError:
     pass
```

### Comparing `mri_nufft-0.7.0/src/mrinufft/density/geometry_based.py` & `mri_nufft-0.8.0/src/mrinufft/density/geometry_based.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/density/nufft_based.py` & `mri_nufft-0.8.0/src/mrinufft/density/nufft_based.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/density/utils.py` & `mri_nufft-0.8.0/src/mrinufft/density/utils.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/io/cfl.py` & `mri_nufft-0.8.0/src/mrinufft/io/cfl.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/__init__.py` & `mri_nufft-0.8.0/src/mrinufft/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/base.py` & `mri_nufft-0.8.0/src/mrinufft/operators/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,32 @@
 """
 
 import warnings
 from abc import ABC, abstractmethod
 from functools import partial, wraps
 import numpy as np
 from mrinufft._utils import power_method, auto_cast, get_array_module
-from mrinufft.operators.interfaces.utils import is_cuda_array
+from mrinufft.operators.interfaces.utils import is_cuda_array, is_host_array
 
 from mrinufft.density import get_density
 
 CUPY_AVAILABLE = True
 try:
     import cupy as cp
 except ImportError:
     CUPY_AVAILABLE = False
 
+AUTOGRAD_AVAILABLE = True
+try:
+    import torch
+    from mrinufft.operators.autodiff import MRINufftAutoGrad
+except ImportError:
+    AUTOGRAD_AVAILABLE = False
+
+
 # Mapping between numpy float and complex types.
 DTYPE_R2C = {"float32": "complex64", "float64": "complex128"}
 
 
 def check_backend(backend_name: str):
     """Check if a specific backend is available."""
     backend_name = backend_name.lower()
@@ -46,21 +54,26 @@
     return [
         name
         for name, (available, _) in FourierOperatorBase.interfaces.items()
         if available or not available_only
     ]
 
 
-def get_operator(backend_name: str, *args, **kwargs):
+def get_operator(backend_name: str, *args, autograd=None, **kwargs):
     """Return an MRI Fourier operator interface using the correct backend.
 
     Parameters
     ----------
     backend_name: str
         Backend name
+
+    autograd: str, default None
+        if set to "data" will provide an operator with autodiff capabilities with
+        respect to it.
+
     *args, **kwargs:
         Arguments to pass to the operator constructor.
 
     Returns
     -------
     FourierOperator
         class or instance of class if args or kwargs are given.
@@ -84,14 +97,20 @@
         operator = partial(operator, backend=backend)
 
     if not available:
         raise ValueError(f"backend {backend_name} found, but dependencies are not met.")
 
     if args or kwargs:
         operator = operator(*args, **kwargs)
+
+    if autograd:
+        if isinstance(operator, FourierOperatorBase):
+            operator = operator.make_autograd(variable=autograd)
+        else:  # partial
+            operator = partial(operator.with_autograd, variable=autograd)
     return operator
 
 
 def with_numpy(fun):
     """Ensure the function works internally with numpy array."""
 
     @wraps(fun)
@@ -135,14 +154,22 @@
             # Move to numpy
             data_ = data.to("cpu").numpy()
             output_ = output.to("cpu").numpy() if output is not None else None
         else:
             data_ = data
             output_ = output
 
+        if output_ is not None:
+            if not (
+                (is_host_array(data_) and is_host_array(output_))
+                or (is_cuda_array(data_) and is_cuda_array(output_))
+            ):
+                raise ValueError(
+                    "input data and output should be " "on the same memory space."
+                )
         ret_ = fun(self, data_, output_, *args, **kwargs)
 
         if xp.__name__ == "torch" and is_cuda_array(data):
             return xp.as_tensor(ret_, device=data.device)
 
         if xp.__name__ == "torch":
             if data.is_cpu:
@@ -222,14 +249,39 @@
 
     def with_off_resonnance_correction(self, B, C, indices):
         """Return a new operator with Off Resonnance Correction."""
         from ..off_resonnance import MRIFourierCorrected
 
         return MRIFourierCorrected(self, B, C, indices)
 
+    def make_autograd(self, variable="data"):
+        """Make a new Operator with autodiff support.
+
+        Parameters
+        ----------
+        variable: str, default data
+            variable on which the gradient is computed with respect to.
+
+        Returns
+        -------
+        torch.nn.module
+            A NUFFT operator with autodiff capabilities.
+
+        Raises
+        ------
+        ValueError
+            If autograd is not available.
+        """
+        if not AUTOGRAD_AVAILABLE:
+            raise ValueError("Autograd not available, ensure torch is installed.")
+        if variable == "data":
+            return MRINufftAutoGrad(self)
+        else:
+            raise ValueError(f"Autodiff with respect to {variable} is not supported.")
+
     def compute_density(self, method=None):
         """Compute the density compensation weights and set it.
 
         Parameters
         ----------
         method: str or callable or array or dict
             The method to use to compute the density compensation.
@@ -391,14 +443,19 @@
             f"  shape: {self.shape}\n"
             f"  n_coils: {self.n_coils}\n"
             f"  n_samples: {self.n_samples}\n"
             f"  uses_sense: {self.uses_sense}\n"
             ")"
         )
 
+    @classmethod
+    def with_autograd(cls, variable, *args, **kwargs):
+        """Return a Fourier operator with autograd capabilities."""
+        return cls(*args, **kwargs).make_autograd(variable)
+
 
 class FourierOperatorCPU(FourierOperatorBase):
     """Base class for CPU-based NUFFT operator.
 
     The NUFFT operation will be done sequentially and looped over coils and batches.
 
     Parameters
```

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/_cupy_kernels.py` & `mri_nufft-0.8.0/src/mrinufft/operators/interfaces/_cupy_kernels.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/bart.py` & `mri_nufft-0.8.0/src/mrinufft/operators/interfaces/bart.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/cufinufft.py` & `mri_nufft-0.8.0/src/mrinufft/operators/interfaces/cufinufft.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/finufft.py` & `mri_nufft-0.8.0/src/mrinufft/operators/interfaces/finufft.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/gpunufft.py` & `mri_nufft-0.8.0/src/mrinufft/operators/interfaces/gpunufft.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Interface to the GPU NUFFT library."""
 
 import numpy as np
 import warnings
 from ..base import FourierOperatorBase, with_numpy_cupy
-from mrinufft._utils import proper_trajectory, get_array_module
-from mrinufft.operators.interfaces.utils import is_cuda_array
+from mrinufft._utils import proper_trajectory, get_array_module, auto_cast
+from mrinufft.operators.interfaces.utils import is_cuda_array, is_host_array, check_size
 
 GPUNUFFT_AVAILABLE = True
 try:
     from gpuNUFFT import NUFFTOp
 except ImportError:
     GPUNUFFT_AVAILABLE = False
 
@@ -254,15 +254,15 @@
         np.copyto(self.pinned_image, self._reshape_image(image))
         new_ksp = self.operator.op(
             self.pinned_image,
             kspace,
             interpolate_data,
         )
         if make_copy_back:
-            new_ksp = cp.copy(new_ksp)
+            new_ksp = np.copy(new_ksp)
         return new_ksp
 
     def adj_op(self, coeffs, image=None, grid_data=False):
         """Compute adjoint of non-uniform Fourier transform.
 
         Parameters
         ----------
@@ -287,14 +287,16 @@
         if make_copy_back:
             new_image = np.copy(new_image)
         return self._reshape_image(new_image, "adjoint")
 
     def adj_op_direct(self, coeffs, image=None, grid_data=False):
         """Compute adjoint of non-uniform Fourier transform.
 
+        The incoming data is on GPU already and we return a GPU array.
+
         Parameters
         ----------
         coeff: np.ndarray
             masked non-uniform Fourier transform data.
         grid_data: bool, default False
             if True, the kspace data is gridded and returned,
             this is used for density compensation
@@ -310,15 +312,15 @@
         if image is None:
             image = cp.empty(
                 (np.prod(self.shape), C),
                 dtype=cp.complex64,
                 order="F",
             )
         self.operator.adj_op_direct(coeffs.data.ptr, image.data.ptr, grid_data)
-        image = image.reshape(C, *self.shape[::-1])
+        image = image.T.reshape(C, *self.shape[::-1], order="C")
         return self._reshape_image(image, "adjoint")
 
 
 class MRIGpuNUFFT(FourierOperatorBase):
     """Interface for the gpuNUFFT backend.
 
     Parameters
@@ -366,15 +368,16 @@
         if GPUNUFFT_AVAILABLE is False:
             raise ValueError(
                 "gpuNUFFT library is not installed, "
                 "please refer to README"
                 "or use cpu for implementation"
             )
         self.shape = shape
-        self.samples = proper_trajectory(samples, normalize="unit")
+
+        self.samples = proper_trajectory(samples.astype(np.float32), normalize="unit")
         self.dtype = self.samples.dtype
         self.n_coils = n_coils
         self.n_batchs = n_batchs
         self.smaps = smaps
         self.squeeze_dims = squeeze_dims
         self.compute_density(density)
         self.impl = RawGpuNUFFT(
@@ -538,7 +541,78 @@
             except ValueError:
                 pass
             try:
                 arr = arr.squeeze(axis=0)
             except ValueError:
                 pass
         return arr
+
+    @with_numpy_cupy
+    def data_consistency(self, image_data, obs_data):
+        """Compute the data consistency estimation directly on gpu.
+
+        This mixes the op and adj_op method to perform F_adj(F(x-y))
+        on a per coil basis. By doing the computation coil wise,
+        it uses less memory than the naive call to adj_op(op(x)-y)
+
+        Parameters
+        ----------
+        image: array
+            Image on which the gradient operation will be evaluated.
+            N_coil x Image shape is not using sense.
+        obs_data: array
+            Observed data.
+        """
+        obs_data = auto_cast(obs_data, self.cpx_dtype)
+        image_data = auto_cast(image_data, self.cpx_dtype)
+
+        B, C = self.n_batchs, self.n_coils
+        K, XYZ = self.n_samples, self.shape
+
+        check_size(obs_data, (B, C, K))
+        if self.uses_sense:
+            check_size(image_data, (B, *XYZ))
+        else:
+            check_size(image_data, (B, C, *XYZ))
+
+        # dispatch
+        if is_host_array(image_data) and is_host_array(obs_data):
+            grad_func = self._dc_host
+        elif is_cuda_array(image_data) and is_cuda_array(obs_data):
+            if B > 1 or (C > 1 and not self.uses_sense):
+                warnings.warn(
+                    "Having all the batches / coils on GPU could be faster, "
+                    "but is memory inefficient!"
+                )
+            grad_func = super().data_consistency
+            if not self.impl.use_gpu_direct:
+                warnings.warn(
+                    "Using direct GPU array without passing "
+                    "`use_gpu_direct=True`, this is memory inefficient."
+                )
+        ret = grad_func(image_data, obs_data)
+        return self._safe_squeeze(ret)
+
+    def _dc_host(self, image_data, obs_data):
+        B, C, XYZ, K = self.n_batchs, self.n_coils, self.shape, self.n_samples
+        image_data_ = image_data.reshape((B, 1 if self.uses_sense else C, *XYZ))
+        obs_data_ = obs_data.reshape((B, C, K))
+
+        obs_data_tmp = cp.zeros((C, K), dtype=self.cpx_dtype)
+        tmp_img = cp.zeros((1 if self.uses_sense else C, *XYZ), dtype=np.complex64)
+        final_img = np.zeros_like(image_data_)
+        for i in range(B):
+            tmp_img.set(image_data_[i])
+            obs_data_tmp.set(obs_data_[i])
+            ksp_tmp = self.impl.op_direct(tmp_img)
+            ksp_tmp -= obs_data_tmp
+            final_img[i] = self.impl.adj_op_direct(ksp_tmp).get()
+        return final_img
+
+    # TODO : For data consistency the workflow is currently:
+    # op coil 1 / .../ op coil N / data_consistency / adj_op coil 1 / adj_op coil n
+    #
+    # By modifying c++ code and exposing it it should be possible to do
+    # op coil 1 / data_consistency 1 / adj_op coil 1 / ... / op_coil N /
+    # data_consistency N / adj_op coil n
+    #
+    # This should bring some performance improvements, due to the asynchronous stuff.
```

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/nfft.py` & `mri_nufft-0.8.0/src/mrinufft/operators/interfaces/nfft.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/pynufft_cpu.py` & `mri_nufft-0.8.0/src/mrinufft/operators/interfaces/pynufft_cpu.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/sigpy.py` & `mri_nufft-0.8.0/src/mrinufft/operators/interfaces/sigpy.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/tfnufft.py` & `mri_nufft-0.8.0/src/mrinufft/operators/interfaces/tfnufft.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/css_color.txt` & `mri_nufft-0.8.0/src/mrinufft/operators/interfaces/utils/css_color.txt`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/gpu_utils.py` & `mri_nufft-0.8.0/src/mrinufft/operators/interfaces/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/interfaces/utils/utils.py` & `mri_nufft-0.8.0/src/mrinufft/operators/interfaces/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/off_resonnance.py` & `mri_nufft-0.8.0/src/mrinufft/operators/off_resonnance.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/operators/stacked.py` & `mri_nufft-0.8.0/src/mrinufft/operators/stacked.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/trajectories/__init__.py` & `mri_nufft-0.8.0/src/mrinufft/trajectories/__init__.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/trajectories/display.py` & `mri_nufft-0.8.0/src/mrinufft/trajectories/display.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/trajectories/maths.py` & `mri_nufft-0.8.0/src/mrinufft/trajectories/maths.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/trajectories/tools.py` & `mri_nufft-0.8.0/src/mrinufft/trajectories/tools.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/trajectories/trajectory2D.py` & `mri_nufft-0.8.0/src/mrinufft/trajectories/trajectory2D.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/trajectories/trajectory3D.py` & `mri_nufft-0.8.0/src/mrinufft/trajectories/trajectory3D.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/src/mrinufft/trajectories/utils.py` & `mri_nufft-0.8.0/src/mrinufft/trajectories/utils.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/tests/case_trajectories.py` & `mri_nufft-0.8.0/tests/case_trajectories.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/tests/conftest.py` & `mri_nufft-0.8.0/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         "--backend",
         action="append",
         default=[],
         help="NUFFT backend on which the tests are performed.",
     )
     parser.addoption(
         "--ref",
-        default="pynfft",
+        default="finufft",
         help="Reference backend on which the tests are performed.",
     )
 
 
 def pytest_configure(config):
     """Configure hook for pytest."""
     available = {b: FourierOperatorBase.interfaces[b][0] for b in list_backends()}
```

### Comparing `mri_nufft-0.7.0/tests/helpers/__init__.py` & `mri_nufft-0.8.0/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/tests/helpers/asserts.py` & `mri_nufft-0.8.0/tests/helpers/asserts.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,17 +49,17 @@
     """Assert the correlation between two arrays."""
     slope_reg, intercept, rvalue, stderr, intercept_stderr = sp.stats.linregress(
         a.flatten(), b.flatten()
     )
     abs_slope_reg = abs(slope_reg)
     if r_value_err is not None and abs(rvalue - 1) > r_value_err:
         raise AssertionError(
-            f"RValue {rvalue} != 1 +- {r_value_err}\n "
+            f"RValue {rvalue} != 1 ± {r_value_err}\n "
             f"intercept={intercept}, stderr={stderr}, "
             f"intercept_stderr={intercept_stderr}"
         )
     if slope_err is not None and abs(abs_slope_reg - slope) > slope_err:
         raise AssertionError(
-            f"Slope {abs_slope_reg} != {slope} +- {slope_err}\n r={rvalue},"
+            f"Slope {abs_slope_reg} != {slope} ± {slope_err}\n r={rvalue},"
             f"intercept={intercept}, stderr={stderr}, "
             f"intercept_stderr={intercept_stderr}"
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mri_nufft-0.7.0/tests/helpers/factories.py` & `mri_nufft-0.8.0/tests/helpers/factories.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/tests/operators/test_batch.py` & `mri_nufft-0.8.0/tests/operators/test_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         (3, 4, 2, True),
         (3, 4, 2, False),
     ],
 )
 @parametrize_with_cases(
     "kspace_locs, shape",
     cases=CasesTrajectories,
-    glob="*random*",
+    glob="*nyquist_radial*",
 )
 @parametrize(backend=["gpunufft", "finufft", "cufinufft"])
 def operator(
     request,
     kspace_locs,
     shape,
     n_coils=1,
@@ -181,20 +181,23 @@
     #    npt.assert_allclose(res.squeeze(), res2.squeeze(), atol=1e-4, rtol=1e-1)
     res = res.reshape(-1, *operator.shape)
     res2 = res2.reshape(-1, *operator.shape)
 
     res = from_interface(res, array_interface)
     res2 = from_interface(res2, array_interface)
     slope_err = 1e-3
+    r_value_err = 1e-3
     # FIXME 2D Sense is not very accurate...
     if len(operator.shape) == 2 and operator.uses_sense:
+        print("Reduced accuracy for 2D Sense")
         slope_err = 1e-1
+        r_value_err = 1e-1
 
     for i in range(len(res)):
-        assert_correlate(res[i], res2[i], slope_err=slope_err)
+        assert_correlate(res[i], res2[i], slope_err=slope_err, r_value_err=r_value_err)
 
 
 def test_data_consistency_readonly(operator, image_data, kspace_data):
     """Test that the data consistency does not modify the input parameters data."""
     kspace_tmp = kspace_data.copy()
     image_tmp = image_data.copy()
     kspace_tmp.setflags(write=False)
```

### Comparing `mri_nufft-0.7.0/tests/operators/test_bindings.py` & `mri_nufft-0.8.0/tests/operators/test_bindings.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/tests/operators/test_gpunufft.py` & `mri_nufft-0.8.0/tests/operators/test_gpunufft.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/tests/operators/test_interfaces.py` & `mri_nufft-0.8.0/tests/operators/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/tests/operators/test_stacked.py` & `mri_nufft-0.8.0/tests/operators/test_stacked.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/tests/operators/test_stacked_gpu.py` & `mri_nufft-0.8.0/tests/operators/test_stacked_gpu.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/tests/test_density.py` & `mri_nufft-0.8.0/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `mri_nufft-0.7.0/tests/test_io.py` & `mri_nufft-0.8.0/tests/test_io.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Test the trajectories io module."""
 
 import numpy as np
 from mrinufft.io import read_trajectory, write_trajectory
+from mrinufft.io.utils import add_phase_to_kspace_with_shifts
 from mrinufft.trajectories.trajectory2D import initialize_2D_radial
 from mrinufft.trajectories.trajectory3D import initialize_3D_cones
 from pytest_cases import parametrize_with_cases
+from case_trajectories import CasesTrajectories
 
 
 class CasesIO:
     """Cases 2 for IO tests, each has different parameters."""
 
     def case_trajectory_2D(self):
         """Test the 2D trajectory."""
@@ -63,7 +65,25 @@
     assert params["TE"] == (0.5 if in_out else 0)
     assert params["gamma"] == gamma
     assert params["recon_tag"] == recon_tag
     assert params["min_osf"] == min_osf
     np.testing.assert_almost_equal(params["FOV"], FOV, decimal=6)
     np.testing.assert_equal(params["img_size"], img_size)
     np.testing.assert_almost_equal(read_traj, trajectory, decimal=5)
+
+
+@parametrize_with_cases(
+    "kspace_loc, shape",
+    cases=[CasesTrajectories.case_random2D, CasesTrajectories.case_random3D],
+)
+def test_add_shift(kspace_loc, shape):
+    """Test the add_phase_to_kspace_with_shifts function."""
+    n_samples = np.prod(kspace_loc.shape[:-1])
+    kspace_data = np.random.randn(n_samples) + 1j * np.random.randn(n_samples)
+    shifts = np.random.rand(kspace_loc.shape[-1])
+
+    shifted_data = add_phase_to_kspace_with_shifts(kspace_data, kspace_loc, shifts)
+
+    assert np.allclose(np.abs(shifted_data), np.abs(kspace_data))
+
+    phase = np.exp(-2 * np.pi * 1j * np.sum(kspace_loc * shifts, axis=-1))
+    np.testing.assert_almost_equal(shifted_data / phase, kspace_data, decimal=5)
```

### Comparing `mri_nufft-0.7.0/tests/test_ndft.py` & `mri_nufft-0.8.0/tests/test_ndft.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,39 +9,15 @@
     implicit_type1_ndft,
     implicit_type2_ndft,
     RawNDFT,
 )
 
 from case_trajectories import CasesTrajectories, case_grid1D
 from helpers import assert_almost_allclose
-
-
-@parametrize_with_cases(
-    "kspace_grid, shape",
-    cases=[
-        case_grid1D,
-        CasesTrajectories.case_grid2D,
-    ],  # 3D is ignored (too much possibility for the reordering)
-)
-def test_ndft_grid_matrix(kspace_grid, shape):
-    """Test that  the ndft matrix is a good matrix for doing fft."""
-    ndft_matrix = get_fourier_matrix(kspace_grid, shape)
-    # Create a random image
-    fft_matrix = [None] * len(shape)
-    for i in range(len(shape)):
-        fft_matrix[i] = sp.fft.fft(np.eye(shape[i]))
-    fft_mat = fft_matrix[0]
-    if len(shape) == 2:
-        fft_mat = fft_matrix[0].flatten()[:, None] @ fft_matrix[1].flatten()[None, :]
-        fft_mat = (
-            fft_mat.reshape(shape * 2)
-            .transpose(2, 0, 1, 3)
-            .reshape((np.prod(shape),) * 2)
-        )
-    assert np.allclose(ndft_matrix, fft_mat)
+from mrinufft import get_operator
 
 
 @parametrize_with_cases(
     "kspace, shape",
     cases=[
         CasesTrajectories.case_random2D,
         CasesTrajectories.case_grid2D,
@@ -52,15 +28,15 @@
     """Test matching of explicit and implicit matrix for ndft."""
     matrix = get_fourier_matrix(kspace, shape)
     random_image = np.random.randn(*shape) + 1j * np.random.randn(*shape)
 
     linop_coef = implicit_type2_ndft(kspace, random_image.flatten(), shape)
     matrix_coef = matrix @ random_image.flatten()
 
-    assert np.allclose(linop_coef, matrix_coef)
+    assert_almost_allclose(linop_coef, matrix_coef, atol=1e-4, rtol=1e-4, mismatch=5)
 
 
 @parametrize_with_cases(
     "kspace, shape",
     cases=[
         CasesTrajectories.case_random2D,
         CasesTrajectories.case_grid2D,
@@ -72,15 +48,15 @@
     matrix = get_fourier_matrix(kspace, shape)
     random_kspace = 1j * np.random.randn(len(kspace))
     random_kspace += np.random.randn(len(kspace))
 
     linop_coef = implicit_type1_ndft(kspace, random_kspace.flatten(), shape)
     matrix_coef = matrix.conj().T @ random_kspace.flatten()
 
-    assert np.allclose(linop_coef, matrix_coef)
+    assert_almost_allclose(linop_coef, matrix_coef, atol=1e-4, rtol=1e-4, mismatch=5)
 
 
 @parametrize_with_cases(
     "kspace_grid, shape",
     cases=[
         case_grid1D,
         CasesTrajectories.case_grid2D,
@@ -94,10 +70,9 @@
     img = (np.random.randn(*shape) + 1j * np.random.randn(*shape)).astype(np.complex64)
     kspace = np.empty(ndft_op.n_samples, dtype=img.dtype)
     ndft_op.op(kspace, img)
     # Reshape the kspace to be on a grid (because the ndft is not doing it)
     kspace = kspace.reshape(img.shape)
     if len(shape) >= 2:
         kspace = kspace.swapaxes(0, 1)
-    kspace_fft = sp.fft.fftn(img)
-
-    assert_almost_allclose(kspace, kspace_fft, atol=1e-5, rtol=1e-5, mismatch=5)
+    kspace_fft = sp.fft.fftn(sp.fft.fftshift(img))
+    assert_almost_allclose(kspace, kspace_fft, atol=1e-4, rtol=1e-4, mismatch=5)
```

