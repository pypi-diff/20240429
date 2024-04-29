# Comparing `tmp/swiftest-2024.4.2.tar.gz` & `tmp/swiftest-2024.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swiftest-2024.4.2.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "swiftest-2024.4.3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `swiftest-2024.4.2.tar` & `swiftest-2024.4.3.tar`

### file list

```diff
@@ -1,242 +1,242 @@
--rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 swiftest-2024.4.2/.dockerignore
--rw-r--r--   0        0        0     1404 2022-11-09 12:37:21.000000 swiftest-2024.4.2/.github/workflows/build_wheels.yml
--rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 swiftest-2024.4.2/.github/workflows/build_wheels_debug.yml
--rw-r--r--   0        0        0     1082 2022-11-09 12:37:21.000000 swiftest-2024.4.2/.gitignore
--rw-r--r--   0        0        0      684 2022-11-09 12:37:21.000000 swiftest-2024.4.2/.readthedocs.yaml
--rw-r--r--   0        0        0     1916 2022-11-09 12:37:21.000000 swiftest-2024.4.2/.zenodo.json
--rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 swiftest-2024.4.2/CITATION.cff
--rw-r--r--   0        0        0     8672 2022-11-09 12:37:21.000000 swiftest-2024.4.2/CMakeLists.txt
--rw-r--r--   0        0        0    35149 2022-11-09 12:37:21.000000 swiftest-2024.4.2/COPYING
--rw-r--r--   0        0        0     3003 2022-11-09 12:37:21.000000 swiftest-2024.4.2/Dockerfile.GNU-Linux
--rw-r--r--   0        0        0     3849 2022-11-09 12:37:21.000000 swiftest-2024.4.2/Dockerfile.Intel
--rw-r--r--   0        0        0      784 2022-11-09 12:37:21.000000 swiftest-2024.4.2/LICENSE
--rw-r--r--   0        0        0     1644 2022-11-09 12:37:21.000000 swiftest-2024.4.2/README.md
--rw-r--r--   0        0        0     6148 2022-11-09 12:37:21.000000 swiftest-2024.4.2/README_figs/.DS_Store
--rw-r--r--   0        0        0     3990 2022-11-09 12:37:21.000000 swiftest-2024.4.2/README_tables/add_body_kwargs.md
--rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 swiftest-2024.4.2/README_tables/save_kwargs.md
--rw-r--r--   0        0        0    18321 2022-11-09 12:37:21.000000 swiftest-2024.4.2/README_tables/simulation_kwargs.md
--rw-r--r--   0        0        0      817 2022-11-09 12:37:21.000000 swiftest-2024.4.2/README_tables/write_param_kwargs.md
--rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 swiftest-2024.4.2/apptainer/.gitignore
--rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 swiftest-2024.4.2/buildscripts/.gitignore
--rw-r--r--   0        0        0     2128 2022-11-09 12:37:21.000000 swiftest-2024.4.2/buildscripts/windows/hdf5-cacheinit-windows.cmake
--rw-r--r--   0        0        0     2732 2022-11-09 12:37:21.000000 swiftest-2024.4.2/buildscripts/windows/netcdf-c-cacheinit-windows.cmake
--rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 swiftest-2024.4.2/buildscripts/windows/netcdf-fortran-cacheinit-windows.cmake
--rw-r--r--   0        0        0     3227 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/FindCoarray_Fortran.cmake
--rw-r--r--   0        0        0     1437 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/FindFFTW3.cmake
--rw-r--r--   0        0        0    11765 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/FindNETCDF_Fortran.cmake
--rw-r--r--   0        0        0     4867 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/FindOpenMP_Fortran.cmake
--rw-r--r--   0        0        0     1681 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/FindSHTOOLS.cmake
--rw-r--r--   0        0        0     4175 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/SetCompileFlag.cmake
--rw-r--r--   0        0        0     1220 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/SetParallelizationLibrary.cmake
--rw-r--r--   0        0        0    29637 2022-11-09 12:37:21.000000 swiftest-2024.4.2/cmake/Modules/SetSwiftestFlags.cmake
--rw-r--r--   0        0        0     3360 2022-11-09 12:37:21.000000 swiftest-2024.4.2/distclean.cmake
--rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docker/.gitignore
--rw-r--r--   0        0        0     8651 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/Makefile
--rw-r--r--   0        0        0    29037 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/basic_simulation_a_vs_t_plot.png
--rw-r--r--   0        0        0    35772 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/index_api_reference.svg
--rw-r--r--   0        0        0   159139 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/index_contribute.svg
--rw-r--r--   0        0        0    99515 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/index_getting_started.svg
--rw-r--r--   0        0        0   115443 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/index_user_guide.svg
--rw-r--r--   0        0        0   223959 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/logos/swiftest_logo.png
--rw-r--r--   0        0        0   148144 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/logos/swiftest_logo.svg
--rw-r--r--   0        0        0   115926 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/logos/swiftest_social_preview.png
--rw-r--r--   0        0        0   145924 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/logos/swiftest_social_preview.svg
--rw-r--r--   0        0        0     5908 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/style.css
--rw-r--r--   0        0        0   636626 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_static/symba_gr.png
--rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_templates/autosummary/accessor.rst
--rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_templates/autosummary/accessor_attribute.rst
--rw-r--r--   0        0        0      168 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_templates/autosummary/accessor_callable.rst
--rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/_templates/autosummary/accessor_method.rst
--rw-r--r--   0        0        0     6339 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/api.rst
--rw-r--r--   0        0        0     6065 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/conf.py
--rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/contributing.rst
--rw-r--r--   0        0        0      976 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/environment.yml
--rw-r--r--   0        0        0    14169 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/getting-started-guide/index.rst
--rw-r--r--   0        0        0     2411 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/index.rst
--rw-r--r--   0        0        0      444 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/requirements.txt
--rw-r--r--   0        0        0    10302 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/user-guide/basic-simulation.rst
--rw-r--r--   0        0        0    11642 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/user-guide/detailed-simulation-setup.rst
--rw-r--r--   0        0        0     9035 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/user-guide/gravitational-harmonics.rst
--rw-r--r--   0        0        0      894 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/user-guide/index.rst
--rw-r--r--   0        0        0     7169 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/user-guide/planetocentric-init_cond.rst
--rw-r--r--   0        0        0     2465 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/user-guide/standalone-executable.rst
--rw-r--r--   0        0        0    18192 2022-11-09 12:37:21.000000 swiftest-2024.4.2/docs/whats-new.rst
--rw-r--r--   0        0        0      712 2022-11-09 12:37:21.000000 swiftest-2024.4.2/environment.yml
--rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/.gitignore
--rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Basic_Simulation/.gitignore
--rw-r--r--   0        0        0     1431 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Basic_Simulation/README.txt
--rwxr-xr-x   0        0        0     4167 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Basic_Simulation/basic_simulation.py
--rw-r--r--   0        0        0     1974 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Basic_Simulation/output_reader.py
--rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Chambers2013/.gitignore
--rw-r--r--   0        0        0     1400 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Chambers2013/README.txt
--rwxr-xr-x   0        0        0     6612 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Chambers2013/initial_conditions.py
--rwxr-xr-x   0        0        0     1350 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Chambers2013/run_simulation.py
--rwxr-xr-x   0        0        0     6462 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Chambers2013/scattermovie.py
--rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Coarray_Test_Particles/.gitignore
--rwxr-xr-x   0        0        0     2075 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Coarray_Test_Particles/initial_conditions.py
--rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Fragmentation/.gitignore
--rwxr-xr-x   0        0        0    17766 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Fragmentation/Fragmentation_Movie.py
--rw-r--r--   0        0        0     1288 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Fragmentation/README.txt
--rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Multibody_Fragmentation/.gitignore
--rwxr-xr-x   0        0        0    13106 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Multibody_Fragmentation/Multibody_Movie.py
--rw-r--r--   0        0        0     1230 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Multibody_Fragmentation/README.txt
--rw-r--r--   0        0        0       35 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/.gitignore
--rw-r--r--   0        0        0      203 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/.gitignore
--rw-r--r--   0        0        0     2212 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/README.txt
--rw-r--r--   0        0        0      910 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/cb.in
--rw-r--r--   0        0        0     1441 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/param.swifter.in
--rw-r--r--   0        0        0     1924 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/param.swiftest.in
--rw-r--r--   0        0        0    21054 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/pl.swifter.in
--rw-r--r--   0        0        0    22140 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/pl.swiftest.in
--rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/swifter_start.in
--rw-r--r--   0        0        0    34765 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.eps
--rw-r--r--   0        0        0     3751 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.py
--rw-r--r--   0        0        0     6870 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/tp.swifter.in
--rw-r--r--   0        0        0     7523 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/tp.swiftest.in
--rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/.gitignore
--rw-r--r--   0        0        0     2091 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/README.txt
--rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/cb.swiftest.in
--rwxr-xr-x   0        0        0     5753 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/init_cond.py
--rw-r--r--   0        0        0     1488 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/param.swifter.in
--rw-r--r--   0        0        0     1763 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/param.swiftest.in
--rw-r--r--   0        0        0     2577 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/pl.swifter.in
--rw-r--r--   0        0        0     2567 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/pl.swiftest.in
--rw-r--r--   0        0        0   142336 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/swiftest_symba_vs_swifter_symba.ipynb
--rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/tp.swifter.in
--rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/tp.swiftest.in
--rw-r--r--   0        0        0       25 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/escape_from_the_solar_system/.gitignore
--rwxr-xr-x   0        0        0     1736 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/escape_from_the_solar_system/escape.py
--rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/helio_gr_test/.gitignore
--rw-r--r--   0        0        0     1207 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/helio_gr_test/README.txt
--rwxr-xr-x   0        0        0     5104 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/helio_gr_test/helio_gr_test.py
--rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/.gitignore
--rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/1pl_1tp_encounter/.gitignore
--rwxr-xr-x   0        0        0     1455 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/1pl_1tp_encounter/init_cond.py
--rw-r--r--   0        0        0    40129 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/1pl_1tp_encounter/swiftest_vs_swifter.ipynb
--rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/1pl_1tp_encounter/swiftest_vs_swifter.py
--rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/8pl_16tp_encounters/.gitignore
--rwxr-xr-x   0        0        0     1379 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/8pl_16tp_encounters/init_cond.py
--rw-r--r--   0        0        0   100370 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/8pl_16tp_encounters/swiftest_vs_swifter.ipynb
--rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/rmvs_swifter_comparison/8pl_16tp_encounters/swiftest_vs_swifter.py
--rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/solar_impact/.gitignore
--rw-r--r--   0        0        0     1197 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/solar_impact/README.txt
--rwxr-xr-x   0        0        0     3267 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/solar_impact/sundiver.py
--rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/spherical_harmonics_cb/.gitignore
--rw-r--r--   0        0        0     4247 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/spherical_harmonics_cb/J2_test_pl_and_tp.py
--rw-r--r--   0        0        0     3478 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/spherical_harmonics_cb/J2_test_tp.py
--rw-r--r--   0        0        0     4194 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/spherical_harmonics_cb/spherical_harmonics_cb.py
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/whm_gr_test/.gitignore
--rw-r--r--   0        0        0     1197 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/whm_gr_test/README.txt
--rwxr-xr-x   0        0        0     4981 2022-11-09 12:37:21.000000 swiftest-2024.4.2/examples/whm_gr_test/whm_gr_test.py
--rw-r--r--   0        0        0     1034 2022-11-09 12:37:21.000000 swiftest-2024.4.2/fortran_docs.md
--rw-r--r--   0        0        0     6194 2022-11-09 12:37:21.000000 swiftest-2024.4.2/paper/paper.bib
--rw-r--r--   0        0        0     8716 2022-11-09 12:37:21.000000 swiftest-2024.4.2/paper/paper.md
--rw-r--r--   0        0        0   239689 2022-11-09 12:37:21.000000 swiftest-2024.4.2/paper/performance.png
--rw-r--r--   0        0        0     5139 2022-11-09 12:37:21.000000 swiftest-2024.4.2/pyproject.toml
--rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 swiftest-2024.4.2/singularity/.gitignore
--rw-r--r--   0        0        0    11563 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/CMakeLists.txt
--rw-r--r--   0        0        0    92405 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/base/base_module.f90
--rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/bindings/.gitignore
--rw-r--r--   0        0        0    12309 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/bindings/bindings_module.f90
--rw-r--r--   0        0        0     7017 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/coarray/coarray_clone.f90
--rw-r--r--   0        0        0     7442 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/coarray/coarray_collect.f90
--rw-r--r--   0        0        0     3367 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/coarray/coarray_module.f90
--rw-r--r--   0        0        0    13092 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/collision/collision_check.f90
--rw-r--r--   0        0        0    13302 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/collision/collision_generate.f90
--rw-r--r--   0        0        0    36608 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/collision/collision_io.f90
--rw-r--r--   0        0        0    47339 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/collision/collision_module.f90
--rw-r--r--   0        0        0    22624 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/collision/collision_regime.f90
--rw-r--r--   0        0        0    39593 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/collision/collision_resolve.f90
--rw-r--r--   0        0        0    50559 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/collision/collision_util.f90
--rw-r--r--   0        0        0    51642 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/encounter/encounter_check.f90
--rw-r--r--   0        0        0    18165 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/encounter/encounter_io.f90
--rw-r--r--   0        0        0    27454 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/encounter/encounter_module.f90
--rw-r--r--   0        0        0    29506 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/encounter/encounter_util.f90
--rw-r--r--   0        0        0    49238 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/fraggle/fraggle_generate.f90
--rw-r--r--   0        0        0     7479 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/fraggle/fraggle_module.f90
--rw-r--r--   0        0        0    12594 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/fraggle/fraggle_util.f90
--rw-r--r--   0        0        0       23 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/globals/.gitignore
--rw-r--r--   0        0        0     8954 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/globals/globals_module.f90
--rw-r--r--   0        0        0     8970 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/globals/globals_module.f90.in
--rw-r--r--   0        0        0     8126 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/helio/helio_drift.f90
--rw-r--r--   0        0        0     5145 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/helio/helio_gr.f90
--rw-r--r--   0        0        0     7481 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/helio/helio_kick.f90
--rw-r--r--   0        0        0    13088 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/helio/helio_module.f90
--rw-r--r--   0        0        0     5331 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/helio/helio_step.f90
--rw-r--r--   0        0        0     2201 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/helio/helio_util.f90
--rw-r--r--   0        0        0     1534 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/main/main.f90
--rw-r--r--   0        0        0     3835 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/misc/io_progress_bar_module.f90
--rw-r--r--   0        0        0    12298 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/misc/lambda_function_module.f90
--rw-r--r--   0        0        0    13165 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/misc/solver_module.f90
--rw-r--r--   0        0        0     7388 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/netcdf_io/netcdf_io_implementations.f90
--rw-r--r--   0        0        0    17666 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/netcdf_io/netcdf_io_module.f90
--rw-r--r--   0        0        0     6828 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/operator/operator_cross.f90
--rw-r--r--   0        0        0     3114 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/operator/operator_mag.f90
--rw-r--r--   0        0        0     8949 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/operator/operator_module.f90
--rw-r--r--   0        0        0     3998 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/operator/operator_unit.f90
--rw-r--r--   0        0        0     4439 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/rmvs/rmvs_discard.f90
--rw-r--r--   0        0        0     3089 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/rmvs/rmvs_encounter_check.f90
--rw-r--r--   0        0        0     5853 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/rmvs/rmvs_kick.f90
--rw-r--r--   0        0        0    24137 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/rmvs/rmvs_module.f90
--rw-r--r--   0        0        0    33566 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/rmvs/rmvs_step.f90
--rw-r--r--   0        0        0    26209 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/rmvs/rmvs_util.f90
--rw-r--r--   0        0        0     7694 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/shgrav/shgrav_accel.f90
--rw-r--r--   0        0        0     1458 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/shgrav/shgrav_module.f90
--rw-r--r--   0        0        0    16114 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_coarray.f90
--rw-r--r--   0        0        0    20114 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_discard.f90
--rw-r--r--   0        0        0    25136 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_drift.f90
--rw-r--r--   0        0        0     9216 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_driver.f90
--rw-r--r--   0        0        0    12386 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_gr.f90
--rw-r--r--   0        0        0   190418 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_io.f90
--rw-r--r--   0        0        0    20673 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_kick.f90
--rw-r--r--   0        0        0   141061 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_module.f90
--rw-r--r--   0        0        0    15415 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_obl.f90
--rw-r--r--   0        0        0    38438 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_orbel.f90
--rw-r--r--   0        0        0     1770 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_user.f90
--rw-r--r--   0        0        0   148284 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/swiftest/swiftest_util.f90
--rw-r--r--   0        0        0    21950 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_discard.f90
--rw-r--r--   0        0        0     2960 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_drift.f90
--rw-r--r--   0        0        0    13228 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_encounter_check.f90
--rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_gr.f90
--rw-r--r--   0        0        0    14491 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_kick.f90
--rw-r--r--   0        0        0    28069 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_module.f90
--rw-r--r--   0        0        0    14590 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_step.f90
--rw-r--r--   0        0        0    21903 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/symba/symba_util.f90
--rw-r--r--   0        0        0     3183 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/tides/tides_getacch_pl.f90
--rw-r--r--   0        0        0     4566 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/tides/tides_module.f90
--rw-r--r--   0        0        0     4546 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/tides/tides_spin_step.f90
--rw-r--r--   0        0        0     5031 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/walltime/walltime_implementations.f90
--rw-r--r--   0        0        0     4557 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/walltime/walltime_module.f90
--rw-r--r--   0        0        0     5011 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/whm/whm_coord.f90
--rw-r--r--   0        0        0     2795 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/whm/whm_drift.f90
--rw-r--r--   0        0        0     5480 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/whm/whm_gr.f90
--rw-r--r--   0        0        0    12284 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/whm/whm_kick.f90
--rw-r--r--   0        0        0    23268 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/whm/whm_module.f90
--rw-r--r--   0        0        0     4928 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/whm/whm_step.f90
--rw-r--r--   0        0        0    13175 2022-11-09 12:37:21.000000 swiftest-2024.4.2/src/whm/whm_util.f90
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/.gitignore
--rw-r--r--   0        0        0     2295 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/CMakeLists.txt
--rw-r--r--   0        0        0      964 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/__init__.py
--rw-r--r--   0        0        0     1466 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/cli.py
--rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/cli_caf.py
--rw-r--r--   0        0        0     1434 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/constants.py
--rw-r--r--   0        0        0      576 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/core.h
--rw-r--r--   0        0        0     9852 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/core.pyx
--rw-r--r--   0        0        0    15976 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/data.py
--rw-r--r--   0        0        0    21140 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/init_cond.py
--rw-r--r--   0        0        0    61003 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/io.py
--rw-r--r--   0        0        0     7098 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/shgrav.py
--rw-r--r--   0        0        0   195796 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/simulation.py
-lrwxr-xr-x   0        0        0        0 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/swiftest -> ../build/bin/swiftest
--rw-r--r--   0        0        0     4239 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/tool.py
--rw-r--r--   0        0        0     1594 2022-11-09 12:37:21.000000 swiftest-2024.4.2/swiftest/visualize.py
--rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/.gitignore
--rw-r--r--   0        0        0     9389 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/test_collisions.py
--rw-r--r--   0        0        0    12156 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/test_fraggle.py
--rwxr-xr-x   0        0        0     7841 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/test_integration.py
--rwxr-xr-x   0        0        0    24776 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/test_io.py
--rw-r--r--   0        0        0     2189 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/test_particle_type.py
--rwxr-xr-x   0        0        0     2255 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/test_units.py
--rw-r--r--   0        0        0     2665 2022-11-09 12:37:21.000000 swiftest-2024.4.2/tests/test_xv2el2xv_dims.py
--rw-r--r--   0        0        0        8 2022-11-09 12:37:21.000000 swiftest-2024.4.2/version.txt
--rw-r--r--   0        0        0     3932 2022-11-09 12:37:21.000000 swiftest-2024.4.2/PKG-INFO
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 swiftest-2024.4.3/.dockerignore
+-rw-r--r--   0        0        0     1404 2022-11-09 12:37:21.000000 swiftest-2024.4.3/.github/workflows/build_wheels.yml
+-rw-r--r--   0        0        0      544 2022-11-09 12:37:21.000000 swiftest-2024.4.3/.github/workflows/build_wheels_debug.yml
+-rw-r--r--   0        0        0     1082 2022-11-09 12:37:21.000000 swiftest-2024.4.3/.gitignore
+-rw-r--r--   0        0        0      684 2022-11-09 12:37:21.000000 swiftest-2024.4.3/.readthedocs.yaml
+-rw-r--r--   0        0        0     1916 2022-11-09 12:37:21.000000 swiftest-2024.4.3/.zenodo.json
+-rw-r--r--   0        0        0      597 2022-11-09 12:37:21.000000 swiftest-2024.4.3/CITATION.cff
+-rw-r--r--   0        0        0     8672 2022-11-09 12:37:21.000000 swiftest-2024.4.3/CMakeLists.txt
+-rw-r--r--   0        0        0    35149 2022-11-09 12:37:21.000000 swiftest-2024.4.3/COPYING
+-rw-r--r--   0        0        0     3003 2022-11-09 12:37:21.000000 swiftest-2024.4.3/Dockerfile.GNU-Linux
+-rw-r--r--   0        0        0     3849 2022-11-09 12:37:21.000000 swiftest-2024.4.3/Dockerfile.Intel
+-rw-r--r--   0        0        0      784 2022-11-09 12:37:21.000000 swiftest-2024.4.3/LICENSE
+-rw-r--r--   0        0        0     1644 2022-11-09 12:37:21.000000 swiftest-2024.4.3/README.md
+-rw-r--r--   0        0        0     6148 2022-11-09 12:37:21.000000 swiftest-2024.4.3/README_figs/.DS_Store
+-rw-r--r--   0        0        0     3990 2022-11-09 12:37:21.000000 swiftest-2024.4.3/README_tables/add_body_kwargs.md
+-rw-r--r--   0        0        0      974 2022-11-09 12:37:21.000000 swiftest-2024.4.3/README_tables/save_kwargs.md
+-rw-r--r--   0        0        0    18321 2022-11-09 12:37:21.000000 swiftest-2024.4.3/README_tables/simulation_kwargs.md
+-rw-r--r--   0        0        0      817 2022-11-09 12:37:21.000000 swiftest-2024.4.3/README_tables/write_param_kwargs.md
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 swiftest-2024.4.3/apptainer/.gitignore
+-rw-r--r--   0        0        0       22 2022-11-09 12:37:21.000000 swiftest-2024.4.3/buildscripts/.gitignore
+-rw-r--r--   0        0        0     2128 2022-11-09 12:37:21.000000 swiftest-2024.4.3/buildscripts/windows/hdf5-cacheinit-windows.cmake
+-rw-r--r--   0        0        0     2732 2022-11-09 12:37:21.000000 swiftest-2024.4.3/buildscripts/windows/netcdf-c-cacheinit-windows.cmake
+-rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 swiftest-2024.4.3/buildscripts/windows/netcdf-fortran-cacheinit-windows.cmake
+-rw-r--r--   0        0        0     3227 2022-11-09 12:37:21.000000 swiftest-2024.4.3/cmake/Modules/FindCoarray_Fortran.cmake
+-rw-r--r--   0        0        0     1437 2022-11-09 12:37:21.000000 swiftest-2024.4.3/cmake/Modules/FindFFTW3.cmake
+-rw-r--r--   0        0        0    11765 2022-11-09 12:37:21.000000 swiftest-2024.4.3/cmake/Modules/FindNETCDF_Fortran.cmake
+-rw-r--r--   0        0        0     4867 2022-11-09 12:37:21.000000 swiftest-2024.4.3/cmake/Modules/FindOpenMP_Fortran.cmake
+-rw-r--r--   0        0        0     1681 2022-11-09 12:37:21.000000 swiftest-2024.4.3/cmake/Modules/FindSHTOOLS.cmake
+-rw-r--r--   0        0        0     4175 2022-11-09 12:37:21.000000 swiftest-2024.4.3/cmake/Modules/SetCompileFlag.cmake
+-rw-r--r--   0        0        0     1220 2022-11-09 12:37:21.000000 swiftest-2024.4.3/cmake/Modules/SetParallelizationLibrary.cmake
+-rw-r--r--   0        0        0    29637 2022-11-09 12:37:21.000000 swiftest-2024.4.3/cmake/Modules/SetSwiftestFlags.cmake
+-rw-r--r--   0        0        0     3360 2022-11-09 12:37:21.000000 swiftest-2024.4.3/distclean.cmake
+-rw-r--r--   0        0        0       45 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docker/.gitignore
+-rw-r--r--   0        0        0     8651 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/Makefile
+-rw-r--r--   0        0        0    29037 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/_static/basic_simulation_a_vs_t_plot.png
+-rw-r--r--   0        0        0    35772 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/_static/index_api_reference.svg
+-rw-r--r--   0        0        0   159139 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/_static/index_contribute.svg
+-rw-r--r--   0        0        0    99515 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/_static/index_getting_started.svg
+-rw-r--r--   0        0        0   115443 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/_static/index_user_guide.svg
+-rw-r--r--   0        0        0   223959 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/_static/logos/swiftest_logo.png
+-rw-r--r--   0        0        0   148144 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/_static/logos/swiftest_logo.svg
+-rw-r--r--   0        0        0   115926 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/_static/logos/swiftest_social_preview.png
+-rw-r--r--   0        0        0   145924 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/_static/logos/swiftest_social_preview.svg
+-rw-r--r--   0        0        0     5908 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/_static/style.css
+-rw-r--r--   0        0        0   636626 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/_static/symba_gr.png
+-rw-r--r--   0        0        0      151 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/_templates/autosummary/accessor.rst
+-rw-r--r--   0        0        0      160 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/_templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0        0        0      168 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/_templates/autosummary/accessor_callable.rst
+-rw-r--r--   0        0        0      157 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/_templates/autosummary/accessor_method.rst
+-rw-r--r--   0        0        0     6339 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/api.rst
+-rw-r--r--   0        0        0     6065 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/conf.py
+-rw-r--r--   0        0        0      202 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/contributing.rst
+-rw-r--r--   0        0        0      976 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/environment.yml
+-rw-r--r--   0        0        0    14169 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/getting-started-guide/index.rst
+-rw-r--r--   0        0        0     2411 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/index.rst
+-rw-r--r--   0        0        0      444 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/requirements.txt
+-rw-r--r--   0        0        0    10302 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/user-guide/basic-simulation.rst
+-rw-r--r--   0        0        0    11642 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/user-guide/detailed-simulation-setup.rst
+-rw-r--r--   0        0        0     9035 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/user-guide/gravitational-harmonics.rst
+-rw-r--r--   0        0        0      894 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/user-guide/index.rst
+-rw-r--r--   0        0        0     7169 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/user-guide/planetocentric-init_cond.rst
+-rw-r--r--   0        0        0     2465 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/user-guide/standalone-executable.rst
+-rw-r--r--   0        0        0    18635 2022-11-09 12:37:21.000000 swiftest-2024.4.3/docs/whats-new.rst
+-rw-r--r--   0        0        0      712 2022-11-09 12:37:21.000000 swiftest-2024.4.3/environment.yml
+-rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/.gitignore
+-rw-r--r--   0        0        0       76 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Basic_Simulation/.gitignore
+-rw-r--r--   0        0        0     1431 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Basic_Simulation/README.txt
+-rwxr-xr-x   0        0        0     4167 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Basic_Simulation/basic_simulation.py
+-rw-r--r--   0        0        0     1974 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Basic_Simulation/output_reader.py
+-rw-r--r--   0        0        0       85 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Chambers2013/.gitignore
+-rw-r--r--   0        0        0     1400 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Chambers2013/README.txt
+-rwxr-xr-x   0        0        0     6612 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Chambers2013/initial_conditions.py
+-rwxr-xr-x   0        0        0     1350 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Chambers2013/run_simulation.py
+-rwxr-xr-x   0        0        0     6462 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Chambers2013/scattermovie.py
+-rw-r--r--   0        0        0       37 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Coarray_Test_Particles/.gitignore
+-rwxr-xr-x   0        0        0     2075 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Coarray_Test_Particles/initial_conditions.py
+-rw-r--r--   0        0        0       50 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Fragmentation/.gitignore
+-rwxr-xr-x   0        0        0    17766 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Fragmentation/Fragmentation_Movie.py
+-rw-r--r--   0        0        0     1288 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Fragmentation/README.txt
+-rw-r--r--   0        0        0       46 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Multibody_Fragmentation/.gitignore
+-rwxr-xr-x   0        0        0    13106 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Multibody_Fragmentation/Multibody_Movie.py
+-rw-r--r--   0        0        0     1230 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Multibody_Fragmentation/README.txt
+-rw-r--r--   0        0        0       35 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/.gitignore
+-rw-r--r--   0        0        0      203 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/.gitignore
+-rw-r--r--   0        0        0     2212 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/README.txt
+-rw-r--r--   0        0        0      910 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/cb.in
+-rw-r--r--   0        0        0     1441 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/param.swifter.in
+-rw-r--r--   0        0        0     1924 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/param.swiftest.in
+-rw-r--r--   0        0        0    21054 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/pl.swifter.in
+-rw-r--r--   0        0        0    22140 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/pl.swiftest.in
+-rw-r--r--   0        0        0      790 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/swifter_start.in
+-rw-r--r--   0        0        0    34765 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.eps
+-rw-r--r--   0        0        0     3751 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.py
+-rw-r--r--   0        0        0     6870 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/tp.swifter.in
+-rw-r--r--   0        0        0     7523 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/tp.swiftest.in
+-rw-r--r--   0        0        0      194 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/.gitignore
+-rw-r--r--   0        0        0     2091 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/README.txt
+-rw-r--r--   0        0        0      805 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/cb.swiftest.in
+-rwxr-xr-x   0        0        0     5753 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/init_cond.py
+-rw-r--r--   0        0        0     1488 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/param.swifter.in
+-rw-r--r--   0        0        0     1763 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/param.swiftest.in
+-rw-r--r--   0        0        0     2577 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/pl.swifter.in
+-rw-r--r--   0        0        0     2567 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/pl.swiftest.in
+-rw-r--r--   0        0        0   142336 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/swiftest_symba_vs_swifter_symba.ipynb
+-rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/tp.swifter.in
+-rw-r--r--   0        0        0      751 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/tp.swiftest.in
+-rw-r--r--   0        0        0       25 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/escape_from_the_solar_system/.gitignore
+-rwxr-xr-x   0        0        0     1736 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/escape_from_the_solar_system/escape.py
+-rw-r--r--   0        0        0       44 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/helio_gr_test/.gitignore
+-rw-r--r--   0        0        0     1207 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/helio_gr_test/README.txt
+-rwxr-xr-x   0        0        0     5104 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/helio_gr_test/helio_gr_test.py
+-rw-r--r--   0        0        0       54 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/rmvs_swifter_comparison/.gitignore
+-rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/rmvs_swifter_comparison/1pl_1tp_encounter/.gitignore
+-rwxr-xr-x   0        0        0     1455 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/rmvs_swifter_comparison/1pl_1tp_encounter/init_cond.py
+-rw-r--r--   0        0        0    40129 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/rmvs_swifter_comparison/1pl_1tp_encounter/swiftest_vs_swifter.ipynb
+-rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/rmvs_swifter_comparison/1pl_1tp_encounter/swiftest_vs_swifter.py
+-rw-r--r--   0        0        0       79 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/rmvs_swifter_comparison/8pl_16tp_encounters/.gitignore
+-rwxr-xr-x   0        0        0     1379 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/rmvs_swifter_comparison/8pl_16tp_encounters/init_cond.py
+-rw-r--r--   0        0        0   100370 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/rmvs_swifter_comparison/8pl_16tp_encounters/swiftest_vs_swifter.ipynb
+-rw-r--r--   0        0        0      412 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/rmvs_swifter_comparison/8pl_16tp_encounters/swiftest_vs_swifter.py
+-rw-r--r--   0        0        0       39 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/solar_impact/.gitignore
+-rw-r--r--   0        0        0     1197 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/solar_impact/README.txt
+-rwxr-xr-x   0        0        0     3267 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/solar_impact/sundiver.py
+-rw-r--r--   0        0        0       63 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/spherical_harmonics_cb/.gitignore
+-rw-r--r--   0        0        0     4247 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/spherical_harmonics_cb/J2_test_pl_and_tp.py
+-rw-r--r--   0        0        0     3478 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/spherical_harmonics_cb/J2_test_tp.py
+-rw-r--r--   0        0        0     4194 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/spherical_harmonics_cb/spherical_harmonics_cb.py
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/whm_gr_test/.gitignore
+-rw-r--r--   0        0        0     1197 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/whm_gr_test/README.txt
+-rwxr-xr-x   0        0        0     4981 2022-11-09 12:37:21.000000 swiftest-2024.4.3/examples/whm_gr_test/whm_gr_test.py
+-rw-r--r--   0        0        0     1034 2022-11-09 12:37:21.000000 swiftest-2024.4.3/fortran_docs.md
+-rw-r--r--   0        0        0     6194 2022-11-09 12:37:21.000000 swiftest-2024.4.3/paper/paper.bib
+-rw-r--r--   0        0        0     8716 2022-11-09 12:37:21.000000 swiftest-2024.4.3/paper/paper.md
+-rw-r--r--   0        0        0   239689 2022-11-09 12:37:21.000000 swiftest-2024.4.3/paper/performance.png
+-rw-r--r--   0        0        0     5139 2022-11-09 12:37:21.000000 swiftest-2024.4.3/pyproject.toml
+-rw-r--r--   0        0        0       32 2022-11-09 12:37:21.000000 swiftest-2024.4.3/singularity/.gitignore
+-rw-r--r--   0        0        0    11563 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/CMakeLists.txt
+-rw-r--r--   0        0        0    92405 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/base/base_module.f90
+-rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/bindings/.gitignore
+-rw-r--r--   0        0        0    12309 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/bindings/bindings_module.f90
+-rw-r--r--   0        0        0     7017 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/coarray/coarray_clone.f90
+-rw-r--r--   0        0        0     7442 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/coarray/coarray_collect.f90
+-rw-r--r--   0        0        0     3367 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/coarray/coarray_module.f90
+-rw-r--r--   0        0        0    13092 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/collision/collision_check.f90
+-rw-r--r--   0        0        0    13302 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/collision/collision_generate.f90
+-rw-r--r--   0        0        0    36608 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/collision/collision_io.f90
+-rw-r--r--   0        0        0    47339 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/collision/collision_module.f90
+-rw-r--r--   0        0        0    22624 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/collision/collision_regime.f90
+-rw-r--r--   0        0        0    39648 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/collision/collision_resolve.f90
+-rw-r--r--   0        0        0    50559 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/collision/collision_util.f90
+-rw-r--r--   0        0        0    51642 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/encounter/encounter_check.f90
+-rw-r--r--   0        0        0    18165 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/encounter/encounter_io.f90
+-rw-r--r--   0        0        0    27454 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/encounter/encounter_module.f90
+-rw-r--r--   0        0        0    29506 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/encounter/encounter_util.f90
+-rw-r--r--   0        0        0    49238 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/fraggle/fraggle_generate.f90
+-rw-r--r--   0        0        0     7479 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/fraggle/fraggle_module.f90
+-rw-r--r--   0        0        0    12594 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/fraggle/fraggle_util.f90
+-rw-r--r--   0        0        0       23 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/globals/.gitignore
+-rw-r--r--   0        0        0     8954 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/globals/globals_module.f90
+-rw-r--r--   0        0        0     8970 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/globals/globals_module.f90.in
+-rw-r--r--   0        0        0     8126 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/helio/helio_drift.f90
+-rw-r--r--   0        0        0     5145 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/helio/helio_gr.f90
+-rw-r--r--   0        0        0     7481 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/helio/helio_kick.f90
+-rw-r--r--   0        0        0    13088 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/helio/helio_module.f90
+-rw-r--r--   0        0        0     5331 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/helio/helio_step.f90
+-rw-r--r--   0        0        0     2201 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/helio/helio_util.f90
+-rw-r--r--   0        0        0     1534 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/main/main.f90
+-rw-r--r--   0        0        0     3835 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/misc/io_progress_bar_module.f90
+-rw-r--r--   0        0        0    12298 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/misc/lambda_function_module.f90
+-rw-r--r--   0        0        0    13165 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/misc/solver_module.f90
+-rw-r--r--   0        0        0     7388 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/netcdf_io/netcdf_io_implementations.f90
+-rw-r--r--   0        0        0    17666 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/netcdf_io/netcdf_io_module.f90
+-rw-r--r--   0        0        0     6828 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/operator/operator_cross.f90
+-rw-r--r--   0        0        0     3114 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/operator/operator_mag.f90
+-rw-r--r--   0        0        0     8949 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/operator/operator_module.f90
+-rw-r--r--   0        0        0     3998 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/operator/operator_unit.f90
+-rw-r--r--   0        0        0     4497 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/rmvs/rmvs_discard.f90
+-rw-r--r--   0        0        0     3089 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/rmvs/rmvs_encounter_check.f90
+-rw-r--r--   0        0        0     5853 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/rmvs/rmvs_kick.f90
+-rw-r--r--   0        0        0    24137 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/rmvs/rmvs_module.f90
+-rw-r--r--   0        0        0    33566 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/rmvs/rmvs_step.f90
+-rw-r--r--   0        0        0    26209 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/rmvs/rmvs_util.f90
+-rw-r--r--   0        0        0     7694 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/shgrav/shgrav_accel.f90
+-rw-r--r--   0        0        0     1458 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/shgrav/shgrav_module.f90
+-rw-r--r--   0        0        0    16114 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/swiftest/swiftest_coarray.f90
+-rw-r--r--   0        0        0    20255 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/swiftest/swiftest_discard.f90
+-rw-r--r--   0        0        0    25136 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/swiftest/swiftest_drift.f90
+-rw-r--r--   0        0        0     9216 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/swiftest/swiftest_driver.f90
+-rw-r--r--   0        0        0    12386 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/swiftest/swiftest_gr.f90
+-rw-r--r--   0        0        0   190418 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/swiftest/swiftest_io.f90
+-rw-r--r--   0        0        0    20673 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/swiftest/swiftest_kick.f90
+-rw-r--r--   0        0        0   141061 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/swiftest/swiftest_module.f90
+-rw-r--r--   0        0        0    15415 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/swiftest/swiftest_obl.f90
+-rw-r--r--   0        0        0    38438 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/swiftest/swiftest_orbel.f90
+-rw-r--r--   0        0        0     1770 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/swiftest/swiftest_user.f90
+-rw-r--r--   0        0        0   148284 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/swiftest/swiftest_util.f90
+-rw-r--r--   0        0        0    22002 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/symba/symba_discard.f90
+-rw-r--r--   0        0        0     2960 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/symba/symba_drift.f90
+-rw-r--r--   0        0        0    13228 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/symba/symba_encounter_check.f90
+-rw-r--r--   0        0        0     3241 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/symba/symba_gr.f90
+-rw-r--r--   0        0        0    14491 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/symba/symba_kick.f90
+-rw-r--r--   0        0        0    28069 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/symba/symba_module.f90
+-rw-r--r--   0        0        0    14590 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/symba/symba_step.f90
+-rw-r--r--   0        0        0    21903 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/symba/symba_util.f90
+-rw-r--r--   0        0        0     3183 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/tides/tides_getacch_pl.f90
+-rw-r--r--   0        0        0     4566 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/tides/tides_module.f90
+-rw-r--r--   0        0        0     4546 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/tides/tides_spin_step.f90
+-rw-r--r--   0        0        0     5031 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/walltime/walltime_implementations.f90
+-rw-r--r--   0        0        0     4557 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/walltime/walltime_module.f90
+-rw-r--r--   0        0        0     5011 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/whm/whm_coord.f90
+-rw-r--r--   0        0        0     2795 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/whm/whm_drift.f90
+-rw-r--r--   0        0        0     5480 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/whm/whm_gr.f90
+-rw-r--r--   0        0        0    12284 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/whm/whm_kick.f90
+-rw-r--r--   0        0        0    23268 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/whm/whm_module.f90
+-rw-r--r--   0        0        0     4928 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/whm/whm_step.f90
+-rw-r--r--   0        0        0    13175 2022-11-09 12:37:21.000000 swiftest-2024.4.3/src/whm/whm_util.f90
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/.gitignore
+-rw-r--r--   0        0        0     2295 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/CMakeLists.txt
+-rw-r--r--   0        0        0      964 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/__init__.py
+-rw-r--r--   0        0        0     1466 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/cli.py
+-rw-r--r--   0        0        0     1393 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/cli_caf.py
+-rw-r--r--   0        0        0     1434 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/constants.py
+-rw-r--r--   0        0        0      576 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/core.h
+-rw-r--r--   0        0        0     9852 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/core.pyx
+-rw-r--r--   0        0        0    15976 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/data.py
+-rw-r--r--   0        0        0    21140 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/init_cond.py
+-rw-r--r--   0        0        0    61003 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/io.py
+-rw-r--r--   0        0        0     7098 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/shgrav.py
+-rw-r--r--   0        0        0   195796 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/simulation.py
+lrwxr-xr-x   0        0        0        0 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/swiftest -> ../build/bin/swiftest
+-rw-r--r--   0        0        0     4239 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/tool.py
+-rw-r--r--   0        0        0     1594 2022-11-09 12:37:21.000000 swiftest-2024.4.3/swiftest/visualize.py
+-rw-r--r--   0        0        0       42 2022-11-09 12:37:21.000000 swiftest-2024.4.3/tests/.gitignore
+-rw-r--r--   0        0        0    10156 2022-11-09 12:37:21.000000 swiftest-2024.4.3/tests/test_collisions.py
+-rw-r--r--   0        0        0    12156 2022-11-09 12:37:21.000000 swiftest-2024.4.3/tests/test_fraggle.py
+-rwxr-xr-x   0        0        0     7841 2022-11-09 12:37:21.000000 swiftest-2024.4.3/tests/test_integration.py
+-rwxr-xr-x   0        0        0    24776 2022-11-09 12:37:21.000000 swiftest-2024.4.3/tests/test_io.py
+-rw-r--r--   0        0        0     2189 2022-11-09 12:37:21.000000 swiftest-2024.4.3/tests/test_particle_type.py
+-rwxr-xr-x   0        0        0     2255 2022-11-09 12:37:21.000000 swiftest-2024.4.3/tests/test_units.py
+-rw-r--r--   0        0        0     2665 2022-11-09 12:37:21.000000 swiftest-2024.4.3/tests/test_xv2el2xv_dims.py
+-rw-r--r--   0        0        0        8 2022-11-09 12:37:21.000000 swiftest-2024.4.3/version.txt
+-rw-r--r--   0        0        0     3932 2022-11-09 12:37:21.000000 swiftest-2024.4.3/PKG-INFO
```

### Comparing `swiftest-2024.4.2/.github/workflows/build_wheels.yml` & `swiftest-2024.4.3/.github/workflows/build_wheels.yml`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/.github/workflows/build_wheels_debug.yml` & `swiftest-2024.4.3/.github/workflows/build_wheels_debug.yml`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/.gitignore` & `swiftest-2024.4.3/.gitignore`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/.readthedocs.yaml` & `swiftest-2024.4.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/.zenodo.json` & `swiftest-2024.4.3/.zenodo.json`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/CITATION.cff` & `swiftest-2024.4.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/CMakeLists.txt` & `swiftest-2024.4.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/COPYING` & `swiftest-2024.4.3/COPYING`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/Dockerfile.GNU-Linux` & `swiftest-2024.4.3/Dockerfile.GNU-Linux`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/Dockerfile.Intel` & `swiftest-2024.4.3/Dockerfile.Intel`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/LICENSE` & `swiftest-2024.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/README.md` & `swiftest-2024.4.3/README.md`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/README_figs/.DS_Store` & `swiftest-2024.4.3/README_figs/.DS_Store`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/README_tables/add_body_kwargs.md` & `swiftest-2024.4.3/README_tables/add_body_kwargs.md`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/README_tables/save_kwargs.md` & `swiftest-2024.4.3/README_tables/save_kwargs.md`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/README_tables/simulation_kwargs.md` & `swiftest-2024.4.3/README_tables/simulation_kwargs.md`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/README_tables/write_param_kwargs.md` & `swiftest-2024.4.3/README_tables/write_param_kwargs.md`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/buildscripts/windows/hdf5-cacheinit-windows.cmake` & `swiftest-2024.4.3/buildscripts/windows/hdf5-cacheinit-windows.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/buildscripts/windows/netcdf-c-cacheinit-windows.cmake` & `swiftest-2024.4.3/buildscripts/windows/netcdf-c-cacheinit-windows.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/buildscripts/windows/netcdf-fortran-cacheinit-windows.cmake` & `swiftest-2024.4.3/buildscripts/windows/netcdf-fortran-cacheinit-windows.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/cmake/Modules/FindCoarray_Fortran.cmake` & `swiftest-2024.4.3/cmake/Modules/FindCoarray_Fortran.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/cmake/Modules/FindFFTW3.cmake` & `swiftest-2024.4.3/cmake/Modules/FindFFTW3.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/cmake/Modules/FindNETCDF_Fortran.cmake` & `swiftest-2024.4.3/cmake/Modules/FindNETCDF_Fortran.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/cmake/Modules/FindOpenMP_Fortran.cmake` & `swiftest-2024.4.3/cmake/Modules/FindOpenMP_Fortran.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/cmake/Modules/FindSHTOOLS.cmake` & `swiftest-2024.4.3/cmake/Modules/FindSHTOOLS.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/cmake/Modules/SetCompileFlag.cmake` & `swiftest-2024.4.3/cmake/Modules/SetCompileFlag.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/cmake/Modules/SetParallelizationLibrary.cmake` & `swiftest-2024.4.3/cmake/Modules/SetParallelizationLibrary.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/cmake/Modules/SetSwiftestFlags.cmake` & `swiftest-2024.4.3/cmake/Modules/SetSwiftestFlags.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/distclean.cmake` & `swiftest-2024.4.3/distclean.cmake`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/Makefile` & `swiftest-2024.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/_static/basic_simulation_a_vs_t_plot.png` & `swiftest-2024.4.3/docs/_static/basic_simulation_a_vs_t_plot.png`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/_static/index_api_reference.svg` & `swiftest-2024.4.3/docs/_static/index_api_reference.svg`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/_static/index_contribute.svg` & `swiftest-2024.4.3/docs/_static/index_contribute.svg`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/_static/index_getting_started.svg` & `swiftest-2024.4.3/docs/_static/index_getting_started.svg`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/_static/index_user_guide.svg` & `swiftest-2024.4.3/docs/_static/index_user_guide.svg`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/_static/logos/swiftest_logo.png` & `swiftest-2024.4.3/docs/_static/logos/swiftest_logo.png`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/_static/logos/swiftest_logo.svg` & `swiftest-2024.4.3/docs/_static/logos/swiftest_logo.svg`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/_static/logos/swiftest_social_preview.png` & `swiftest-2024.4.3/docs/_static/logos/swiftest_social_preview.png`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/_static/logos/swiftest_social_preview.svg` & `swiftest-2024.4.3/docs/_static/logos/swiftest_social_preview.svg`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/_static/style.css` & `swiftest-2024.4.3/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/_static/symba_gr.png` & `swiftest-2024.4.3/docs/_static/symba_gr.png`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/api.rst` & `swiftest-2024.4.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/conf.py` & `swiftest-2024.4.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/environment.yml` & `swiftest-2024.4.3/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/getting-started-guide/index.rst` & `swiftest-2024.4.3/docs/getting-started-guide/index.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/index.rst` & `swiftest-2024.4.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/user-guide/basic-simulation.rst` & `swiftest-2024.4.3/docs/user-guide/basic-simulation.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/user-guide/detailed-simulation-setup.rst` & `swiftest-2024.4.3/docs/user-guide/detailed-simulation-setup.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/user-guide/gravitational-harmonics.rst` & `swiftest-2024.4.3/docs/user-guide/gravitational-harmonics.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/user-guide/index.rst` & `swiftest-2024.4.3/docs/user-guide/index.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/user-guide/planetocentric-init_cond.rst` & `swiftest-2024.4.3/docs/user-guide/planetocentric-init_cond.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/user-guide/standalone-executable.rst` & `swiftest-2024.4.3/docs/user-guide/standalone-executable.rst`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/docs/whats-new.rst` & `swiftest-2024.4.3/docs/whats-new.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 .. currentmodule:: swiftest
 
 What's New
 ==========
 
+.. _whats-new.2024.04.3:
+
+`v2024.04.3`_
+-------------
+.. _v2024.04.3: https:///github.com/MintonGroup/swiftest/releases/tag/v2024.04.3
+
+
+Bug Fixes
+~~~~~~~~~
+- Fixed bug that was causing discards to fail when there were more than one discard in a single step. This was due to not deallocating the `ldiscard` or ``ldiscard_tp`` / ``ldiscard_pl`` arrays after they were used. `GH40`_
+
+.. _GH40: https://github.com/MintonGroup/swiftest/issues/40
+
 .. _whats-new.2024.04.2:
 
 `v2024.04.2`_
 -------------
 .. _v2024.04.2: https://github.com/MintonGroup/swiftest/releases/tag/v2024.04.2
 
 Bug Fixes
```

### Comparing `swiftest-2024.4.2/environment.yml` & `swiftest-2024.4.3/environment.yml`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Basic_Simulation/README.txt` & `swiftest-2024.4.3/examples/Basic_Simulation/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Basic_Simulation/basic_simulation.py` & `swiftest-2024.4.3/examples/Basic_Simulation/basic_simulation.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Basic_Simulation/output_reader.py` & `swiftest-2024.4.3/examples/Basic_Simulation/output_reader.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Chambers2013/README.txt` & `swiftest-2024.4.3/examples/Chambers2013/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Chambers2013/initial_conditions.py` & `swiftest-2024.4.3/examples/Chambers2013/initial_conditions.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Chambers2013/run_simulation.py` & `swiftest-2024.4.3/examples/Chambers2013/run_simulation.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Chambers2013/scattermovie.py` & `swiftest-2024.4.3/examples/Chambers2013/scattermovie.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Coarray_Test_Particles/initial_conditions.py` & `swiftest-2024.4.3/examples/Coarray_Test_Particles/initial_conditions.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Fragmentation/Fragmentation_Movie.py` & `swiftest-2024.4.3/examples/Fragmentation/Fragmentation_Movie.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Fragmentation/README.txt` & `swiftest-2024.4.3/examples/Fragmentation/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Multibody_Fragmentation/Multibody_Movie.py` & `swiftest-2024.4.3/examples/Multibody_Fragmentation/Multibody_Movie.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Multibody_Fragmentation/README.txt` & `swiftest-2024.4.3/examples/Multibody_Fragmentation/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/README.txt` & `swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/cb.in` & `swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/cb.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/param.swifter.in` & `swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/param.swifter.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/param.swiftest.in` & `swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/param.swiftest.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/pl.swifter.in` & `swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/pl.swifter.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/pl.swiftest.in` & `swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/pl.swiftest.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/swifter_start.in` & `swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/swifter_start.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.eps` & `swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.eps`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.py` & `swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/swifter_swiftest_comp.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/tp.swifter.in` & `swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/tp.swifter.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/108pl_50tp/tp.swiftest.in` & `swiftest-2024.4.3/examples/Swifter_Swiftest/108pl_50tp/tp.swiftest.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/README.txt` & `swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/cb.swiftest.in` & `swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/cb.swiftest.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/init_cond.py` & `swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/init_cond.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/param.swifter.in` & `swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/param.swifter.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/param.swiftest.in` & `swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/param.swiftest.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/pl.swifter.in` & `swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/pl.swifter.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/pl.swiftest.in` & `swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/pl.swiftest.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/swiftest_symba_vs_swifter_symba.ipynb` & `swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/swiftest_symba_vs_swifter_symba.ipynb`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/tp.swifter.in` & `swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/tp.swifter.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/Swifter_Swiftest/8pl_0tp/tp.swiftest.in` & `swiftest-2024.4.3/examples/Swifter_Swiftest/8pl_0tp/tp.swiftest.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/escape_from_the_solar_system/escape.py` & `swiftest-2024.4.3/examples/escape_from_the_solar_system/escape.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/helio_gr_test/README.txt` & `swiftest-2024.4.3/examples/helio_gr_test/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/helio_gr_test/helio_gr_test.py` & `swiftest-2024.4.3/examples/helio_gr_test/helio_gr_test.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/rmvs_swifter_comparison/1pl_1tp_encounter/init_cond.py` & `swiftest-2024.4.3/examples/rmvs_swifter_comparison/1pl_1tp_encounter/init_cond.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/rmvs_swifter_comparison/1pl_1tp_encounter/swiftest_vs_swifter.ipynb` & `swiftest-2024.4.3/examples/rmvs_swifter_comparison/1pl_1tp_encounter/swiftest_vs_swifter.ipynb`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/rmvs_swifter_comparison/8pl_16tp_encounters/init_cond.py` & `swiftest-2024.4.3/examples/rmvs_swifter_comparison/8pl_16tp_encounters/init_cond.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/rmvs_swifter_comparison/8pl_16tp_encounters/swiftest_vs_swifter.ipynb` & `swiftest-2024.4.3/examples/rmvs_swifter_comparison/8pl_16tp_encounters/swiftest_vs_swifter.ipynb`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/solar_impact/README.txt` & `swiftest-2024.4.3/examples/solar_impact/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/solar_impact/sundiver.py` & `swiftest-2024.4.3/examples/solar_impact/sundiver.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/spherical_harmonics_cb/J2_test_pl_and_tp.py` & `swiftest-2024.4.3/examples/spherical_harmonics_cb/J2_test_pl_and_tp.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/spherical_harmonics_cb/J2_test_tp.py` & `swiftest-2024.4.3/examples/spherical_harmonics_cb/J2_test_tp.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/spherical_harmonics_cb/spherical_harmonics_cb.py` & `swiftest-2024.4.3/examples/spherical_harmonics_cb/spherical_harmonics_cb.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/whm_gr_test/README.txt` & `swiftest-2024.4.3/examples/whm_gr_test/README.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/examples/whm_gr_test/whm_gr_test.py` & `swiftest-2024.4.3/examples/whm_gr_test/whm_gr_test.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/fortran_docs.md` & `swiftest-2024.4.3/fortran_docs.md`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/paper/paper.bib` & `swiftest-2024.4.3/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/paper/paper.md` & `swiftest-2024.4.3/paper/paper.md`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/paper/performance.png` & `swiftest-2024.4.3/paper/performance.png`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/pyproject.toml` & `swiftest-2024.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "swiftest"
-version = "2024.4.2"
+version = "2024.4.3"
 authors=[
     {name = 'David A. Minton', email='daminton@purdue.edu'},
     {name = 'Carlisle Wishard'},
     {name = 'Jennifer Pouplin'},
     {name = 'Jake Elliott'},
     {name = 'Dana Singh'},
     {name = 'Kaustub Anand'},
```

### Comparing `swiftest-2024.4.2/src/CMakeLists.txt` & `swiftest-2024.4.3/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/base/base_module.f90` & `swiftest-2024.4.3/src/base/base_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/bindings/bindings_module.f90` & `swiftest-2024.4.3/src/bindings/bindings_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/coarray/coarray_clone.f90` & `swiftest-2024.4.3/src/coarray/coarray_clone.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/coarray/coarray_collect.f90` & `swiftest-2024.4.3/src/coarray/coarray_collect.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/coarray/coarray_module.f90` & `swiftest-2024.4.3/src/coarray/coarray_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/collision/collision_check.f90` & `swiftest-2024.4.3/src/collision/collision_check.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/collision/collision_generate.f90` & `swiftest-2024.4.3/src/collision/collision_generate.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/collision/collision_io.f90` & `swiftest-2024.4.3/src/collision/collision_io.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/collision/collision_module.f90` & `swiftest-2024.4.3/src/collision/collision_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/collision/collision_regime.f90` & `swiftest-2024.4.3/src/collision/collision_regime.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/collision/collision_resolve.f90` & `swiftest-2024.4.3/src/collision/collision_resolve.f90`

 * *Files 1% similar despite different names*

```diff
@@ -768,14 +768,16 @@
                  
                   ! Save the system snapshot
                   call tp%save_discard(ldiscard_pl,nbody_system,collider%before)
                   call pl%save_discard(ldiscard_tp,nbody_system,collider%before)
                   call collision_history%take_snapshot(param,nbody_system, t, "before") 
                   call pl%save_discard(ldiscard_tp,nbody_system,collider%after)
                   call collision_history%take_snapshot(param,nbody_system, t, "after") 
+
+                  deallocate(ldiscard_pl,ldiscard_tp)
                end do
 
                ! Destroy the collision list now that the collisions are resolved
                call pltp_collision%setup(0_I8B)
 
             end associate
          end associate
```

### Comparing `swiftest-2024.4.2/src/collision/collision_util.f90` & `swiftest-2024.4.3/src/collision/collision_util.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/encounter/encounter_check.f90` & `swiftest-2024.4.3/src/encounter/encounter_check.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/encounter/encounter_io.f90` & `swiftest-2024.4.3/src/encounter/encounter_io.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/encounter/encounter_module.f90` & `swiftest-2024.4.3/src/encounter/encounter_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/encounter/encounter_util.f90` & `swiftest-2024.4.3/src/encounter/encounter_util.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/fraggle/fraggle_generate.f90` & `swiftest-2024.4.3/src/fraggle/fraggle_generate.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/fraggle/fraggle_module.f90` & `swiftest-2024.4.3/src/fraggle/fraggle_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/fraggle/fraggle_util.f90` & `swiftest-2024.4.3/src/fraggle/fraggle_util.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/globals/globals_module.f90` & `swiftest-2024.4.3/src/globals/globals_module.f90`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
    integer(I4B), parameter :: LOWERCASE_BEGIN  = iachar('a') !! ASCII character set parameter for lower to upper conversion - start 
                                                              !! of lowercase
    integer(I4B), parameter :: LOWERCASE_END    = iachar('z') !! ASCII character set parameter for lower to upper conversion - end of 
                                                              !! lowercase
    integer(I4B), parameter :: UPPERCASE_OFFSET = iachar('A') - iachar('a') !! ASCII character set parameter for lower to upper 
                                                                            !! conversion - offset between upper and lower
 
-   character(*), parameter :: VERSION = "2024.4.2" !! Swiftest version
+   character(*), parameter :: VERSION = "2024.4.3" !! Swiftest version
 
    !> Symbolic name for integrator types
    character(*), parameter :: UNKNOWN_INTEGRATOR = "UKNOWN INTEGRATOR"
    character(*), parameter :: INT_BS                 = "Bulirsch-Stoer"
    character(*), parameter :: INT_HELIO              = "Democratic Heliocentric"
    character(*), parameter :: INT_RA15               = "Radau 15th order"
    character(*), parameter :: INT_TU4                = "T+U 4th order"
```

### Comparing `swiftest-2024.4.2/src/globals/globals_module.f90.in` & `swiftest-2024.4.3/src/globals/globals_module.f90.in`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/helio/helio_drift.f90` & `swiftest-2024.4.3/src/helio/helio_drift.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/helio/helio_gr.f90` & `swiftest-2024.4.3/src/helio/helio_gr.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/helio/helio_kick.f90` & `swiftest-2024.4.3/src/helio/helio_kick.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/helio/helio_module.f90` & `swiftest-2024.4.3/src/helio/helio_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/helio/helio_step.f90` & `swiftest-2024.4.3/src/helio/helio_step.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/helio/helio_util.f90` & `swiftest-2024.4.3/src/helio/helio_util.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/main/main.f90` & `swiftest-2024.4.3/src/main/main.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/misc/io_progress_bar_module.f90` & `swiftest-2024.4.3/src/misc/io_progress_bar_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/misc/lambda_function_module.f90` & `swiftest-2024.4.3/src/misc/lambda_function_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/misc/solver_module.f90` & `swiftest-2024.4.3/src/misc/solver_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/netcdf_io/netcdf_io_implementations.f90` & `swiftest-2024.4.3/src/netcdf_io/netcdf_io_implementations.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/netcdf_io/netcdf_io_module.f90` & `swiftest-2024.4.3/src/netcdf_io/netcdf_io_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/operator/operator_cross.f90` & `swiftest-2024.4.3/src/operator/operator_cross.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/operator/operator_mag.f90` & `swiftest-2024.4.3/src/operator/operator_mag.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/operator/operator_module.f90` & `swiftest-2024.4.3/src/operator/operator_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/operator/operator_unit.f90` & `swiftest-2024.4.3/src/operator/operator_unit.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/rmvs/rmvs_discard.f90` & `swiftest-2024.4.3/src/rmvs/rmvs_discard.f90`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
                      ldiscard_tp(i) = .true.
                      ldiscard_pl(iplperP) = .true.
                      call tp%save_discard(ldiscard_tp,nbody_system,collider%before)
                      call pl%save_discard(ldiscard_pl,nbody_system,collider%before)
                      call collision_history%take_snapshot(param,nbody_system, t, "before") 
                      call pl%save_discard(ldiscard_pl,nbody_system,collider%after)
                      call collision_history%take_snapshot(param,nbody_system, t, "after") 
+                     deallocate(ldiscard_tp, ldiscard_pl)
                   end if
                end if
             end associate
          end do
          ! Call the base method that this overrides
          call swiftest_discard_tp(tp, nbody_system, param)
       end associate
```

### Comparing `swiftest-2024.4.2/src/rmvs/rmvs_encounter_check.f90` & `swiftest-2024.4.3/src/rmvs/rmvs_encounter_check.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/rmvs/rmvs_kick.f90` & `swiftest-2024.4.3/src/rmvs/rmvs_kick.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/rmvs/rmvs_module.f90` & `swiftest-2024.4.3/src/rmvs/rmvs_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/rmvs/rmvs_step.f90` & `swiftest-2024.4.3/src/rmvs/rmvs_step.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/rmvs/rmvs_util.f90` & `swiftest-2024.4.3/src/rmvs/rmvs_util.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/shgrav/shgrav_accel.f90` & `swiftest-2024.4.3/src/shgrav/shgrav_accel.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/shgrav/shgrav_module.f90` & `swiftest-2024.4.3/src/shgrav/shgrav_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/swiftest/swiftest_coarray.f90` & `swiftest-2024.4.3/src/swiftest/swiftest_coarray.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/swiftest/swiftest_discard.f90` & `swiftest-2024.4.3/src/swiftest/swiftest_discard.f90`

 * *Files 0% similar despite different names*

```diff
@@ -205,14 +205,15 @@
                if (body%ldiscard(i)) then
                   allocate(ldiscard, mold=body%ldiscard(:))
                   ldiscard(:) = .false.
                   ldiscard(i) = .true.
                   call body%save_discard(ldiscard,nbody_system,collider%before)
                   ! The base class doesn't do a before/after comparison, so we just save the before snapshot
                   call collision_history%take_snapshot(param,nbody_system, t, "particle") 
+                  deallocate(ldiscard)
                end if
             end if
          end do
       end associate
 
       return
    end subroutine swiftest_discard_cb_body
@@ -276,14 +277,15 @@
 
                         ! Save the system snapshot
                         impactors%regime = REGIME_CB_IMPACT
                         allocate(ldiscard, mold=body%ldiscard(:))
                         ldiscard(:) = .false.
                         ldiscard(i) = .true.
                         call body%save_discard(ldiscard,nbody_system,collider%before)
+                        deallocate(ldiscard)
                         call collision_history%take_snapshot(param,nbody_system, t, "particle") 
                      end if
                   end if
                end if
             end if
          end do
       end associate
@@ -344,25 +346,25 @@
                      tp%ldiscard(i) = .true.
                      call tp%info(i)%set_value(status="DISCARDED_PLR", discard_time=nbody_system%t, discard_rh=tp%rh(:,i), &
                                                discard_vh=tp%vh(:,i), discard_body_id=pl%id(j))
 
                      ! Save the system snapshot
                      impactors%regime = COLLRESOLVE_REGIME_MERGE
                      allocate(ldiscard_tp, mold=tp%ldiscard(:))
-                     allocate(ldiscard_Pl, mold=Pl%ldiscard(:))
+                     allocate(ldiscard_pl, mold=Pl%ldiscard(:))
                      ldiscard_tp(:) = .false.
                      ldiscard_pl(:) = .false.
                      ldiscard_tp(i) = .true.
                      ldiscard_pl(j) = .true.
                      call tp%save_discard(ldiscard_pl,nbody_system,collider%before)
                      call pl%save_discard(ldiscard_tp,nbody_system,collider%before)
                      call collision_history%take_snapshot(param,nbody_system, t, "before") 
                      call pl%save_discard(ldiscard_tp,nbody_system,collider%after)
                      call collision_history%take_snapshot(param,nbody_system, t, "after") 
-
+                     deallocate(ldiscard_tp, ldiscard_pl)
                      exit
                   end if
                end do
             end if
          end do
       end associate
```

### Comparing `swiftest-2024.4.2/src/swiftest/swiftest_drift.f90` & `swiftest-2024.4.3/src/swiftest/swiftest_drift.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/swiftest/swiftest_driver.f90` & `swiftest-2024.4.3/src/swiftest/swiftest_driver.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/swiftest/swiftest_gr.f90` & `swiftest-2024.4.3/src/swiftest/swiftest_gr.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/swiftest/swiftest_io.f90` & `swiftest-2024.4.3/src/swiftest/swiftest_io.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/swiftest/swiftest_kick.f90` & `swiftest-2024.4.3/src/swiftest/swiftest_kick.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/swiftest/swiftest_module.f90` & `swiftest-2024.4.3/src/swiftest/swiftest_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/swiftest/swiftest_obl.f90` & `swiftest-2024.4.3/src/swiftest/swiftest_obl.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/swiftest/swiftest_orbel.f90` & `swiftest-2024.4.3/src/swiftest/swiftest_orbel.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/swiftest/swiftest_user.f90` & `swiftest-2024.4.3/src/swiftest/swiftest_user.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/swiftest/swiftest_util.f90` & `swiftest-2024.4.3/src/swiftest/swiftest_util.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/symba/symba_discard.f90` & `swiftest-2024.4.3/src/symba/symba_discard.f90`

 * *Files 0% similar despite different names*

```diff
@@ -386,14 +386,16 @@
                call symba_discard_nonplpl_conservation(self, nbody_system, param)
 
                call pl%rearray(nbody_system, param)
 
                ldiscard(:) = .false.
                call pl%save_discard(ldiscard,nbody_system,collider%after) ! This ensures that the Sun gets saved in the "after" slot
                call collision_history%take_snapshot(param,nbody_system, t, "after") 
+               
+               deallocate(ldiscard)
 
                if (param%lenergy) then
                   call collision_history%save_energy_snapshot("before", nbody_system, &
                                                               collision_history%iframe,collision_history%iframe)
                   call nbody_system%get_energy_and_momentum(param)
                   E_orbit_after = nbody_system%te
                   nbody_system%E_collisions = nbody_system%E_collisions + (E_orbit_after - E_orbit_before)
```

### Comparing `swiftest-2024.4.2/src/symba/symba_drift.f90` & `swiftest-2024.4.3/src/symba/symba_drift.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/symba/symba_encounter_check.f90` & `swiftest-2024.4.3/src/symba/symba_encounter_check.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/symba/symba_gr.f90` & `swiftest-2024.4.3/src/symba/symba_gr.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/symba/symba_kick.f90` & `swiftest-2024.4.3/src/symba/symba_kick.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/symba/symba_module.f90` & `swiftest-2024.4.3/src/symba/symba_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/symba/symba_step.f90` & `swiftest-2024.4.3/src/symba/symba_step.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/symba/symba_util.f90` & `swiftest-2024.4.3/src/symba/symba_util.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/tides/tides_getacch_pl.f90` & `swiftest-2024.4.3/src/tides/tides_getacch_pl.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/tides/tides_module.f90` & `swiftest-2024.4.3/src/tides/tides_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/tides/tides_spin_step.f90` & `swiftest-2024.4.3/src/tides/tides_spin_step.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/walltime/walltime_implementations.f90` & `swiftest-2024.4.3/src/walltime/walltime_implementations.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/walltime/walltime_module.f90` & `swiftest-2024.4.3/src/walltime/walltime_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/whm/whm_coord.f90` & `swiftest-2024.4.3/src/whm/whm_coord.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/whm/whm_drift.f90` & `swiftest-2024.4.3/src/whm/whm_drift.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/whm/whm_gr.f90` & `swiftest-2024.4.3/src/whm/whm_gr.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/whm/whm_kick.f90` & `swiftest-2024.4.3/src/whm/whm_kick.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/whm/whm_module.f90` & `swiftest-2024.4.3/src/whm/whm_module.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/whm/whm_step.f90` & `swiftest-2024.4.3/src/whm/whm_step.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/src/whm/whm_util.f90` & `swiftest-2024.4.3/src/whm/whm_util.f90`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/swiftest/CMakeLists.txt` & `swiftest-2024.4.3/swiftest/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/swiftest/__init__.py` & `swiftest-2024.4.3/swiftest/__init__.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/swiftest/cli.py` & `swiftest-2024.4.3/swiftest/cli.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/swiftest/cli_caf.py` & `swiftest-2024.4.3/swiftest/cli_caf.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/swiftest/constants.py` & `swiftest-2024.4.3/swiftest/constants.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/swiftest/core.h` & `swiftest-2024.4.3/swiftest/core.h`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/swiftest/core.pyx` & `swiftest-2024.4.3/swiftest/core.pyx`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/swiftest/data.py` & `swiftest-2024.4.3/swiftest/data.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/swiftest/init_cond.py` & `swiftest-2024.4.3/swiftest/init_cond.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/swiftest/io.py` & `swiftest-2024.4.3/swiftest/io.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/swiftest/shgrav.py` & `swiftest-2024.4.3/swiftest/shgrav.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/swiftest/simulation.py` & `swiftest-2024.4.3/swiftest/simulation.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/swiftest/tool.py` & `swiftest-2024.4.3/swiftest/tool.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/swiftest/visualize.py` & `swiftest-2024.4.3/swiftest/visualize.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/tests/test_collisions.py` & `swiftest-2024.4.3/tests/test_collisions.py`

 * *Files 6% similar despite different names*

```diff
@@ -181,11 +181,32 @@
             dLtot=ds.Ltot_mag.diff('stage').values[0]
             self.assertAlmostEqual(dLtot,0,places=8, msg=f"Angular momentum not conserved: {dLtot}")
         
             # Check that energy was lost
             dEtot=ds.TE.diff('stage').values[0]
             self.assertLess(dEtot,0, msg=f"Energy not lost: {dEtot}")        
         
-             
+    def test_multi_collision(self):
+        """
+        Tests that multiple collisions are handled correctly
+        """              
+        
+        sim = swiftest.Simulation(simdir=self.simdir)
+        
+
+        sim.add_solar_system_body(['Sun', 'Earth'])
+
+        # add bodies that both impact the CB at the same time
+        sim.add_body(name = ['close'], rh = [0, 0, sim.param['CHK_RMIN'] * 1.1], vh = [0, 0, 0.0001])
+        sim.add_body(name = ['close2'], rh = [0, 0, sim.param['CHK_RMIN'] * 1.11], vh = [0, 0, 0.0001])
+
+        try:
+            sim.run(tstop = 10, dt = 0.01, tstep_out = 1)
+        except Exception as e:
+            self.fail(f"Multiple collisions not handled correctly: {e}")
+            
+        self.assertEqual(sim.collisions.collision_id.size,2)
+
+
 if __name__ == '__main__':
     os.environ["HDF5_USE_FILE_LOCKING"]="FALSE"
     unittest.main()
```

### Comparing `swiftest-2024.4.2/tests/test_fraggle.py` & `swiftest-2024.4.3/tests/test_fraggle.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/tests/test_integration.py` & `swiftest-2024.4.3/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/tests/test_io.py` & `swiftest-2024.4.3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/tests/test_particle_type.py` & `swiftest-2024.4.3/tests/test_particle_type.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/tests/test_units.py` & `swiftest-2024.4.3/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/tests/test_xv2el2xv_dims.py` & `swiftest-2024.4.3/tests/test_xv2el2xv_dims.py`

 * *Files identical despite different names*

### Comparing `swiftest-2024.4.2/PKG-INFO` & `swiftest-2024.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swiftest
-Version: 2024.4.2
+Version: 2024.4.3
 Keywords: astronomy,astrophysics,planetary,n-body,integrator,symplectic,wisdom-holman,symba
 Author: Carlisle Wishard, Jennifer Pouplin, Jake Elliott, Dana Singh, Kaustub Anand
 Author-Email: "David A. Minton" <daminton@purdue.edu>
 Maintainer-Email: "David A. Minton" <daminton@purdue.edu>
 License: Copyright 2023 - David Minton 
         The Swiftest development team: David Minton, Carlisle Wishard, Jennifer Pouplin, Jake Elliott, Dana Singh, & Kaustub Anand
```

