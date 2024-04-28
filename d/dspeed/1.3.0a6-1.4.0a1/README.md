# Comparing `tmp/dspeed-1.3.0a6.tar.gz` & `tmp/dspeed-1.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspeed-1.3.0a6.tar", last modified: Fri Apr 26 17:53:20 2024, max compression
+gzip compressed data, was "dspeed-1.4.0a1.tar", last modified: Sun Apr 28 22:38:08 2024, max compression
```

## Comparing `dspeed-1.3.0a6.tar` & `dspeed-1.4.0a1.tar`

### file list

```diff
@@ -1,102 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.284431 dspeed-1.3.0a6/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-26 17:53:20.284431 dspeed-1.3.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-26 17:53:20.284431 dspeed-1.3.0a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.264430 dspeed-1.3.0a6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.268431 dspeed-1.3.0a6/src/dspeed/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/build_dsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    91711 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processing_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.276430 dspeed-1.3.0a6/src/dspeed/processors/
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/bl_subtract.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/dwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/energy_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/fftw.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/fixed_time_pickoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/gaussian_filter1d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/get_multi_local_extrema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/get_wf_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/linear_slope_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/log_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/min_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/moving_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/multi_a_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/multi_t_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/param_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/peak_snr_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/pole_zero.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/poly_fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/presum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/pulse_injector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/rc_cr2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/round_to_nearest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/saturation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/soft_pileup_corr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/svm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/time_over_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)    16670 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/time_point_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/transfer_function_convolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/trap_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/upsampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/wf_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/wiener_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/processors/windower.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/units.py
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.276430 dspeed-1.3.0a6/src/dspeed/vis/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/vis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23174 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/src/dspeed/vis/waveform_browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.284431 dspeed-1.3.0a6/src/dspeed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5261 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 17:53:20.000000 dspeed-1.3.0a6/src/dspeed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.276430 dspeed-1.3.0a6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.280431 dspeed-1.3.0a6/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (127)    10388 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/configs/icpc-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/configs/icpc-dsp-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/configs/numpy-parsing.json
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/configs/sipm-dplms-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/configs/sipm-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.280431 dspeed-1.3.0a6/tests/processors/
--rw-r--r--   0 runner    (1001) docker     (127)    14296 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/dplms_noise_mat.dat
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_dplms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_dwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_fftw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_fixed_time_pickoff.py
--rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_get_multi_local_extrema.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_get_wf_centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_min_max_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_pole_zero.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_rc_cr2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13231 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_time_point_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_transfer_function_convolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/processors/test_wf_alignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/test_build_dsp.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/test_list_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/test_numpy_constants_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/test_processing_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.280431 dspeed-1.3.0a6/tests/vis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 17:53:20.280431 dspeed-1.3.0a6/tests/vis/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/vis/configs/hpge-dsp-config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-26 17:53:16.000000 dspeed-1.3.0a6/tests/vis/test_waveform_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:38:08.836009 dspeed-1.4.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-28 22:38:08.836009 dspeed-1.4.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-28 22:38:08.836009 dspeed-1.4.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:38:08.820009 dspeed-1.4.0a1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:38:08.824009 dspeed-1.4.0a1/src/dspeed/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-28 22:38:08.000000 dspeed-1.4.0a1/src/dspeed/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7408 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/build_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91577 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processing_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:38:08.832009 dspeed-1.4.0a1/src/dspeed/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/bl_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/dwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/energy_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/fixed_time_pickoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/gaussian_filter1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/get_multi_local_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/get_wf_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/linear_slope_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/log_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/min_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/moving_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/multi_a_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/multi_t_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/param_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/peak_snr_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5469 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/pole_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/poly_fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/presum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/pulse_injector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/rc_cr2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/round_to_nearest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/saturation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/soft_pileup_corr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/svm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/time_over_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17186 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/time_point_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/transfer_function_convolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8479 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/trap_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/upsampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/wf_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/wiener_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/processors/windower.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:38:08.832009 dspeed-1.4.0a1/src/dspeed/vis/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23174 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/src/dspeed/vis/waveform_browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:38:08.836009 dspeed-1.4.0a1/src/dspeed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5239 2024-04-28 22:38:08.000000 dspeed-1.4.0a1/src/dspeed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-28 22:38:08.000000 dspeed-1.4.0a1/src/dspeed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 22:38:08.000000 dspeed-1.4.0a1/src/dspeed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-28 22:38:08.000000 dspeed-1.4.0a1/src/dspeed.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 22:38:08.000000 dspeed-1.4.0a1/src/dspeed.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-28 22:38:08.000000 dspeed-1.4.0a1/src/dspeed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-28 22:38:08.000000 dspeed-1.4.0a1/src/dspeed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:38:08.832009 dspeed-1.4.0a1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:38:08.832009 dspeed-1.4.0a1/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)    10014 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/configs/icpc-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7121 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/configs/icpc-dsp-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/configs/numpy-parsing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/configs/sipm-dplms-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/configs/sipm-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:38:08.836009 dspeed-1.4.0a1/tests/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)    14296 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/processors/dplms_noise_mat.dat
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/processors/test_dplms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/processors/test_dwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/processors/test_fixed_time_pickoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10333 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/processors/test_get_multi_local_extrema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/processors/test_get_wf_centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/processors/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/processors/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/processors/test_min_max_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/processors/test_pole_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/processors/test_rc_cr2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13824 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/processors/test_time_point_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/processors/test_transfer_function_convolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/processors/test_wf_alignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/test_build_dsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/test_list_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/test_numpy_constants_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9890 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/test_processing_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:38:08.836009 dspeed-1.4.0a1/tests/vis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:38:08.836009 dspeed-1.4.0a1/tests/vis/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/vis/configs/hpge-dsp-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-28 22:38:05.000000 dspeed-1.4.0a1/tests/vis/test_waveform_browser.py
```

### Comparing `dspeed-1.3.0a6/LICENSE` & `dspeed-1.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/PKG-INFO` & `dspeed-1.4.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspeed
-Version: 1.3.0a6
+Version: 1.4.0a1
 Summary: Fast Digital Signal Processing for particle detectors in Python
 Home-page: https://github.com/legend-exp/dspeed
 Author: Ian Guinn
 Author-email: guinnis@ornl.gov
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
@@ -32,15 +32,14 @@
 Requires-Dist: iminuit
 Requires-Dist: legend-pydataobj>=1.5.0a1
 Requires-Dist: matplotlib
 Requires-Dist: numba!=0.53.*,!=0.54.*
 Requires-Dist: parse
 Requires-Dist: pint
 Requires-Dist: pyarrow
-Requires-Dist: pyfftw
 Requires-Dist: scipy
 Requires-Dist: tqdm>=4.27
 Provides-Extra: all
 Requires-Dist: dspeed[docs,test]; extra == "all"
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: jupyter; extra == "docs"
```

### Comparing `dspeed-1.3.0a6/README.md` & `dspeed-1.4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/setup.cfg` & `dspeed-1.4.0a1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 	iminuit
 	legend-pydataobj>=1.5.0a1
 	matplotlib
 	numba!=0.53.*,!=0.54.*
 	parse
 	pint
 	pyarrow
-	pyfftw
 	scipy
 	tqdm>=4.27
 python_requires = >=3.9
 include_package_data = True
 package_dir = 
 	= src
 zip_safe = False
```

### Comparing `dspeed-1.3.0a6/src/dspeed/build_dsp.py` & `dspeed-1.4.0a1/src/dspeed/build_dsp.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/cli.py` & `dspeed-1.4.0a1/src/dspeed/cli.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/errors.py` & `dspeed-1.4.0a1/src/dspeed/errors.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/logging.py` & `dspeed-1.4.0a1/src/dspeed/logging.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processing_chain.py` & `dspeed-1.4.0a1/src/dspeed/processing_chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -779,20 +779,14 @@
                 ast.literal_eval(expr[node.col_offset : node.end_col_offset])
             )
             if len(npparr.shape) == 1:
                 return npparr
             else:
                 ProcessingChainError("only 1D arrays are supported: " + expr)
 
-        elif isinstance(node, ast.Num):
-            return node.n
-
-        elif isinstance(node, ast.Str):
-            return node.s
-
         elif isinstance(node, ast.Constant):
             return node.value
 
         # look for name in variable dictionary
         elif isinstance(node, ast.Name):
             # check if it is a unit
             if node.id in ureg:
```

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/__init__.py` & `dspeed-1.4.0a1/src/dspeed/processors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,14 @@
    to use functions that operate in place as much as possible!
 """
 
 from .bl_subtract import bl_subtract
 from .convolutions import convolve_wf, fft_convolve_wf
 from .dwt import discrete_wavelet_transform
 from .energy_kernels import cusp_filter, dplms, zac_filter
-from .fftw import dft, inv_dft, psd
 from .fixed_time_pickoff import fixed_time_pickoff
 from .gaussian_filter1d import gaussian_filter1d
 from .get_multi_local_extrema import get_multi_local_extrema
 from .get_wf_centroid import get_wf_centroid
 from .histogram import histogram, histogram_stats
 from .kernels import moving_slope, step, t0_filter
 from .linear_slope_fit import linear_slope_diff, linear_slope_fit
@@ -111,17 +110,14 @@
     "bl_subtract",
     "convolve_wf",
     "fft_convolve_wf",
     "cusp_filter",
     "t0_filter",
     "zac_filter",
     "discrete_wavelet_transform",
-    "dft",
-    "inv_dft",
-    "psd",
     "fixed_time_pickoff",
     "gaussian_filter1d",
     "get_multi_local_extrema",
     "histogram",
     "histogram_stats",
     "linear_slope_fit",
     "linear_slope_diff",
```

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/bl_subtract.py` & `dspeed-1.4.0a1/src/dspeed/processors/bl_subtract.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/convolutions.py` & `dspeed-1.4.0a1/src/dspeed/processors/convolutions.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/dwt.py` & `dspeed-1.4.0a1/src/dspeed/processors/dwt.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/energy_kernels.py` & `dspeed-1.4.0a1/src/dspeed/processors/energy_kernels.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/fixed_time_pickoff.py` & `dspeed-1.4.0a1/src/dspeed/processors/fixed_time_pickoff.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/gaussian_filter1d.py` & `dspeed-1.4.0a1/src/dspeed/processors/gaussian_filter1d.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/get_multi_local_extrema.py` & `dspeed-1.4.0a1/src/dspeed/processors/get_multi_local_extrema.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/get_wf_centroid.py` & `dspeed-1.4.0a1/src/dspeed/processors/get_wf_centroid.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/histogram.py` & `dspeed-1.4.0a1/src/dspeed/processors/histogram.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/kernels.py` & `dspeed-1.4.0a1/src/dspeed/processors/kernels.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/linear_slope_fit.py` & `dspeed-1.4.0a1/src/dspeed/processors/linear_slope_fit.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/log_check.py` & `dspeed-1.4.0a1/src/dspeed/processors/log_check.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/min_max.py` & `dspeed-1.4.0a1/src/dspeed/processors/min_max.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/moving_windows.py` & `dspeed-1.4.0a1/src/dspeed/processors/moving_windows.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/multi_a_filter.py` & `dspeed-1.4.0a1/src/dspeed/processors/multi_a_filter.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/multi_t_filter.py` & `dspeed-1.4.0a1/src/dspeed/processors/multi_t_filter.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/optimize.py` & `dspeed-1.4.0a1/src/dspeed/processors/optimize.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/param_lookup.py` & `dspeed-1.4.0a1/src/dspeed/processors/param_lookup.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/peak_snr_threshold.py` & `dspeed-1.4.0a1/src/dspeed/processors/peak_snr_threshold.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/pole_zero.py` & `dspeed-1.4.0a1/src/dspeed/processors/pole_zero.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/poly_fit.py` & `dspeed-1.4.0a1/src/dspeed/processors/poly_fit.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/presum.py` & `dspeed-1.4.0a1/src/dspeed/processors/presum.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/pulse_injector.py` & `dspeed-1.4.0a1/src/dspeed/processors/pulse_injector.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/rc_cr2.py` & `dspeed-1.4.0a1/src/dspeed/processors/rc_cr2.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/round_to_nearest.py` & `dspeed-1.4.0a1/src/dspeed/processors/round_to_nearest.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/saturation.py` & `dspeed-1.4.0a1/src/dspeed/processors/saturation.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/soft_pileup_corr.py` & `dspeed-1.4.0a1/src/dspeed/processors/soft_pileup_corr.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/svm.py` & `dspeed-1.4.0a1/src/dspeed/processors/svm.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/time_over_threshold.py` & `dspeed-1.4.0a1/src/dspeed/processors/time_over_threshold.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/time_point_thresh.py` & `dspeed-1.4.0a1/src/dspeed/processors/time_point_thresh.py`

 * *Files 3% similar despite different names*

```diff
@@ -367,26 +367,27 @@
                 if i_tp < 0:
                     break
                 idx = sorted_idx[i_tp]
 
 
 @guvectorize(
     [
-        "void(float32[:], float32, float32, float32, float32, float32[:], float32[:])",
-        "void(float64[:], float64, float64, float64, float64, float64[:], float64[:])",
+        "void(float32[:], float32, float32, float32, float32, uint32[:], float32[:], float32[:])",
+        "void(float64[:], float64, float64, float64, float64, uint32[:], float64[:], float64[:])",
     ],
-    "(n),(),(),(),(),(m),(m)",
+    "(n),(),(),(),(),(),(m),(m)",
     **nb_kwargs,
 )
 def bi_level_zero_crossing_time_points(
     w_in: np.ndarray,
     a_pos_threshold_in: float,
     a_neg_threshold_in: float,
     gate_time_in: int,
     t_start_in: int,
+    n_crossings_out: int,
     polarity_out: np.array,
     t_trig_times_out: np.array,
 ) -> None:
     """
     Find the indices where a waveform value crosses 0 after crossing the threshold and reaching the next threshold within some gate time.
     Works on positive and negative polarity waveforms.
     Useful for finding pileup events with the RC-CR^2 filter.
@@ -399,14 +400,16 @@
         the positive threshold value.
     a_neg_threshold_in
         the negative threshold value.
     gate_time_in
         The number of samples that the next threshold crossing has to be within in order to count a 0 crossing
     t_start_in
         the starting index.
+    n_crossings_out
+        the number of zero-crossings found. Note: if there are more zeros than elements in output arrays, this will continue to increment but the polarity and trigger time will not be added to the output buffers
     polarity_out
         An array holding the polarity of identified pulses. 0 for negative and 1 for positive
     t_trig_times_out
         the indices where the waveform value has crossed the threshold and returned to 0.
         Arrays of fixed length (padded with :any:`numpy.nan`) that hold the
         indices of the identified trigger times.
 
@@ -414,15 +417,15 @@
     --------------------------
 
     .. code-block :: json
 
         "trig_times_out": {
             "function": "multi_trigger_time",
             "module": "dspeed.processors",
-            "args": ["wf_rc_cr2", "5", "-10", 0, "polarity_out(20)", "trig_times_out(20)"],
+            "args": ["wf_rc_cr2", "5", "-10", 0, "n_crossings", "polarity_out(20, vector_len=n_crossings)", "trig_times_out(20, vector_len=n_crossings)"],
             "unit": "ns"
         }
     """
     # prepare output
     t_trig_times_out[:] = np.nan
     polarity_out[:] = np.nan
 
@@ -445,27 +448,28 @@
         raise DSPFatal("The output arrays are of different lengths.")
 
     gate_time_in = int(gate_time_in)  # make sure this is an integer!
     # Perform the processing
     is_above_thresh = False
     is_below_thresh = False
     crossed_zero = False
-    trig_array_idx = 0
+    n_crossings_out[0] = 0
     for i in range(int(t_start_in), len(w_in) - 1, 1):
         if is_below_thresh and (w_in[i] <= 0 < w_in[i + 1]):
             crossed_zero = True
             neg_trig_time_candidate = i
 
         # Either we go above threshold
         if w_in[i] <= a_pos_threshold_in < w_in[i + 1]:
             if crossed_zero and is_below_thresh:
                 if i - is_below_thresh < gate_time_in:
-                    t_trig_times_out[trig_array_idx] = neg_trig_time_candidate
-                    polarity_out[trig_array_idx] = 0
-                    trig_array_idx += 1
+                    if n_crossings_out[0] < len(polarity_out):
+                        t_trig_times_out[n_crossings_out[0]] = neg_trig_time_candidate
+                        polarity_out[n_crossings_out[0]] = 0
+                    n_crossings_out[0] += 1
                 else:
                     is_above_thresh = i
 
                 is_below_thresh = False
                 crossed_zero = False
             else:
                 is_above_thresh = i
@@ -474,16 +478,17 @@
             crossed_zero = True
             pos_trig_time_candidate = i
 
         # Or we go below threshold
         if w_in[i] >= a_neg_threshold_in > w_in[i + 1]:
             if crossed_zero and is_above_thresh:
                 if i - is_above_thresh < gate_time_in:
-                    t_trig_times_out[trig_array_idx] = pos_trig_time_candidate
-                    polarity_out[trig_array_idx] = 1
-                    trig_array_idx += 1
+                    if n_crossings_out[0] < len(polarity_out):
+                        t_trig_times_out[n_crossings_out[0]] = pos_trig_time_candidate
+                        polarity_out[n_crossings_out[0]] = 1
+                    n_crossings_out[0] += 1
                 else:
                     is_below_thresh = i
                 is_above_thresh = False
                 crossed_zero = False
             else:
                 is_below_thresh = i
```

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/transfer_function_convolver.py` & `dspeed-1.4.0a1/src/dspeed/processors/transfer_function_convolver.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/trap_filters.py` & `dspeed-1.4.0a1/src/dspeed/processors/trap_filters.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/upsampler.py` & `dspeed-1.4.0a1/src/dspeed/processors/upsampler.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/wf_alignment.py` & `dspeed-1.4.0a1/src/dspeed/processors/wf_alignment.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/wiener_filter.py` & `dspeed-1.4.0a1/src/dspeed/processors/wiener_filter.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/processors/windower.py` & `dspeed-1.4.0a1/src/dspeed/processors/windower.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/utils.py` & `dspeed-1.4.0a1/src/dspeed/utils.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed/vis/waveform_browser.py` & `dspeed-1.4.0a1/src/dspeed/vis/waveform_browser.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/src/dspeed.egg-info/PKG-INFO` & `dspeed-1.4.0a1/src/dspeed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspeed
-Version: 1.3.0a6
+Version: 1.4.0a1
 Summary: Fast Digital Signal Processing for particle detectors in Python
 Home-page: https://github.com/legend-exp/dspeed
 Author: Ian Guinn
 Author-email: guinnis@ornl.gov
 Maintainer: The LEGEND Collaboration
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
@@ -32,15 +32,14 @@
 Requires-Dist: iminuit
 Requires-Dist: legend-pydataobj>=1.5.0a1
 Requires-Dist: matplotlib
 Requires-Dist: numba!=0.53.*,!=0.54.*
 Requires-Dist: parse
 Requires-Dist: pint
 Requires-Dist: pyarrow
-Requires-Dist: pyfftw
 Requires-Dist: scipy
 Requires-Dist: tqdm>=4.27
 Provides-Extra: all
 Requires-Dist: dspeed[docs,test]; extra == "all"
 Provides-Extra: docs
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: jupyter; extra == "docs"
```

### Comparing `dspeed-1.3.0a6/src/dspeed.egg-info/SOURCES.txt` & `dspeed-1.4.0a1/src/dspeed.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 src/dspeed.egg-info/requires.txt
 src/dspeed.egg-info/top_level.txt
 src/dspeed/processors/__init__.py
 src/dspeed/processors/bl_subtract.py
 src/dspeed/processors/convolutions.py
 src/dspeed/processors/dwt.py
 src/dspeed/processors/energy_kernels.py
-src/dspeed/processors/fftw.py
 src/dspeed/processors/fixed_time_pickoff.py
 src/dspeed/processors/gaussian_filter1d.py
 src/dspeed/processors/get_multi_local_extrema.py
 src/dspeed/processors/get_wf_centroid.py
 src/dspeed/processors/histogram.py
 src/dspeed/processors/kernels.py
 src/dspeed/processors/linear_slope_fit.py
@@ -70,15 +69,14 @@
 tests/configs/icpc-dsp-config.yaml
 tests/configs/numpy-parsing.json
 tests/configs/sipm-dplms-config.json
 tests/configs/sipm-dsp-config.json
 tests/processors/dplms_noise_mat.dat
 tests/processors/test_dplms.py
 tests/processors/test_dwt.py
-tests/processors/test_fftw.py
 tests/processors/test_fixed_time_pickoff.py
 tests/processors/test_get_multi_local_extrema.py
 tests/processors/test_get_wf_centroid.py
 tests/processors/test_histogram.py
 tests/processors/test_import.py
 tests/processors/test_min_max_norm.py
 tests/processors/test_pole_zero.py
```

### Comparing `dspeed-1.3.0a6/tests/configs/icpc-dsp-config.json` & `dspeed-1.4.0a1/tests/configs/icpc-dsp-config.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9825588474025975%*

 * *Differences: {"'outputs'": '{delete: [34]}',*

 * * "'processors'": "{'QDrift': 'trapQftp * 16', 'dt_eff': {'function': 'QDrift/trapTmax', delete: "*

 * *                 "['module', 'args']}, delete: ['wf_psd']}"}*

```diff
@@ -29,28 +29,18 @@
         "tp_aoe_max",
         "tp_aoe_samp",
         "trapEmax",
         "trapEftp",
         "cuspEmax",
         "zacEmax",
         "zacEftp",
-        "cuspEftp",
-        "wf_psd"
+        "cuspEftp"
     ],
     "processors": {
-        "QDrift": {
-            "args": [
-                "trapQftp",
-                "(4*us)/waveform.period",
-                "QDrift"
-            ],
-            "function": "multiply",
-            "module": "numpy",
-            "unit": "ADC"
-        },
+        "QDrift": "trapQftp * 16",
         "aoe_t_min, tp_aoe_max, A_min, A_max": {
             "args": [
                 "curr_av",
                 "aoe_t_min",
                 "tp_aoe_max",
                 "A_min",
                 "A_max"
@@ -173,21 +163,15 @@
                 "db.pz.tau": "450*us"
             },
             "function": "cusp_filter",
             "module": "dspeed.processors",
             "unit": "ADC"
         },
         "dt_eff": {
-            "args": [
-                "QDrift",
-                "trapTmax",
-                "dt_eff"
-            ],
-            "function": "divide",
-            "module": "numpy",
+            "function": "QDrift/trapTmax",
             "unit": "ns"
         },
         "pz_mean , pz_std, pz_slope, pz_intercept": {
             "args": [
                 "wf_pz[1500:]",
                 "pz_mean",
                 "pz_std",
@@ -485,26 +469,14 @@
                 "tp_0_est",
                 "wf_le(301, 'f')"
             ],
             "function": "windower",
             "module": "dspeed.processors",
             "unit": "ADC"
         },
-        "wf_psd": {
-            "args": [
-                "wf_blsub",
-                "wf_psd"
-            ],
-            "function": "psd",
-            "init_args": [
-                "wf_blsub",
-                "wf_psd"
-            ],
-            "module": "dspeed.processors"
-        },
         "wf_pz": {
             "args": [
                 "wf_blsub",
                 "db.pz.tau",
                 "wf_pz"
             ],
             "defaults": {
```

### Comparing `dspeed-1.3.0a6/tests/configs/icpc-dsp-config.yaml` & `dspeed-1.4.0a1/tests/configs/icpc-dsp-config.yaml`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/configs/numpy-parsing.json` & `dspeed-1.4.0a1/tests/configs/numpy-parsing.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/configs/sipm-dplms-config.json` & `dspeed-1.4.0a1/tests/configs/sipm-dplms-config.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/configs/sipm-dsp-config.json` & `dspeed-1.4.0a1/tests/configs/sipm-dsp-config.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/conftest.py` & `dspeed-1.4.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/processors/dplms_noise_mat.dat` & `dspeed-1.4.0a1/tests/processors/dplms_noise_mat.dat`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/processors/test_dplms.py` & `dspeed-1.4.0a1/tests/processors/test_dplms.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/processors/test_dwt.py` & `dspeed-1.4.0a1/tests/processors/test_dwt.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/processors/test_fixed_time_pickoff.py` & `dspeed-1.4.0a1/tests/processors/test_fixed_time_pickoff.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/processors/test_get_multi_local_extrema.py` & `dspeed-1.4.0a1/tests/processors/test_get_multi_local_extrema.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/processors/test_get_wf_centroid.py` & `dspeed-1.4.0a1/tests/processors/test_get_wf_centroid.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/processors/test_histogram.py` & `dspeed-1.4.0a1/tests/processors/test_histogram.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/processors/test_min_max_norm.py` & `dspeed-1.4.0a1/tests/processors/test_min_max_norm.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/processors/test_pole_zero.py` & `dspeed-1.4.0a1/tests/processors/test_pole_zero.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/processors/test_rc_cr2.py` & `dspeed-1.4.0a1/tests/processors/test_rc_cr2.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/processors/test_time_point_thresh.py` & `dspeed-1.4.0a1/tests/processors/test_time_point_thresh.py`

 * *Files 6% similar despite different names*

```diff
@@ -190,45 +190,46 @@
 
 
 def test_bi_level_zero_crossing_time_points(compare_numba_vs_python):
     # Test exceptions and initial checks
     # ensure that if there is a nan in w_in, all nans are outputted
     w_in = np.ones(100)
     w_in[4] = np.nan
+    n_out = np.zeros(1, "uint32")
     t_out = np.zeros(5)
     pol_out = np.zeros(5)
-    bi_level_zero_crossing_time_points(w_in, 100, 100, 100, 0, pol_out, t_out)
+    bi_level_zero_crossing_time_points(w_in, 100, 100, 100, 0, n_out, pol_out, t_out)
     assert np.isnan(t_out).all()
 
     # ensure the ValueError is raised if the polarity output array is different length than the time point output array
     t_start_in = 1.02
     with pytest.raises(ValueError):
         bi_level_zero_crossing_time_points(
-            np.ones(9), 100, 100, 100, t_start_in, pol_out, np.zeros(1)
+            np.ones(9), 100, 100, 100, t_start_in, n_out, pol_out, np.zeros(1)
         )
 
     # ensure the DSPFatal is raised if initial timepoint is not an integer
     t_start_in = 1.02
     with pytest.raises(DSPFatal):
         bi_level_zero_crossing_time_points(
-            np.ones(9), 100, 100, 100, t_start_in, pol_out, t_out
+            np.ones(9), 100, 100, 100, t_start_in, n_out, pol_out, t_out
         )
 
     # ensure the DSPFatal is raised if initial timepoint is not negative
     t_start_in = -2
     with pytest.raises(DSPFatal):
         bi_level_zero_crossing_time_points(
-            np.ones(9), 100, 100, 100, t_start_in, pol_out, t_out
+            np.ones(9), 100, 100, 100, t_start_in, n_out, pol_out, t_out
         )
 
     # ensure the DSPFatal is raised if initial timepoint is outside length of waveform
     t_start_in = 100
     with pytest.raises(DSPFatal):
         bi_level_zero_crossing_time_points(
-            np.ones(9), 100, 100, 100, t_start_in, pol_out, t_out
+            np.ones(9), 100, 100, 100, t_start_in, n_out, pol_out, t_out
         )
 
     early_trig = 500  # start pulse1 500 samples from the start of the wf
     late_trig = 200  # start pulse2 200 samples after the midpoint of 8192 length wf
     zeta = 30000  # the decay time constant of a pulse, in samples
     amplitude = 1750
     tau = 100  # the RC-CR^2 filter time constant
@@ -256,15 +257,15 @@
 
     gate_time = 1000
     # Test that the filter reproduces 0 crossings at the expected points
     # Test on positive polarity
     t_trig_times_out = np.zeros(5)
     pol_out = np.zeros(5)
     bi_level_zero_crossing_time_points(
-        pulse, 2000, -2000, gate_time, 0, pol_out, t_trig_times_out
+        pulse, 2000, -2000, gate_time, 0, n_out, pol_out, t_trig_times_out
     )
 
     cross_1 = early_trig + 2 * tau - 1  # minus 1 from delay?
     cross_2 = (
         8192 // 2 + late_trig + 2 * tau - 2
     )  # minus 1 from 1st pulse delay and again
     assert np.allclose(int(t_trig_times_out[0]), cross_1, rtol=1)
@@ -272,97 +273,114 @@
     assert int(pol_out[0]) == 1
     assert int(pol_out[1]) == 1
 
     # Check on negative polarity pulses
     t_trig_times_out = np.zeros(5)
     pol_out = np.zeros(5)
     bi_level_zero_crossing_time_points(
-        -1 * pulse, 2000, -2000, gate_time, 0, pol_out, t_trig_times_out
+        -1 * pulse, 2000, -2000, gate_time, 0, n_out, pol_out, t_trig_times_out
     )
     assert np.allclose(int(t_trig_times_out[0]), cross_1, rtol=1)
     assert np.allclose(int(t_trig_times_out[1]), cross_2, rtol=1)
     assert int(pol_out[0]) == 0
     assert int(pol_out[1]) == 0
 
     # Check positive polarity pulses that cross 0 and never reach negative threshold return all nan
     t_trig_times_out = np.zeros(5)
     pol_out = np.zeros(5)
     bi_level_zero_crossing_time_points(
-        pulse, 2000, -300000, gate_time, 0, pol_out, t_trig_times_out
+        pulse, 2000, -300000, gate_time, 0, n_out, pol_out, t_trig_times_out
     )
     assert np.isnan(t_trig_times_out).all()
     assert np.isnan(pol_out).all()
 
     # Check negative polarity pulses that cross 0 and never reach positive threshold return all nan
     t_trig_times_out = np.zeros(5)
     pol_out = np.zeros(5)
     bi_level_zero_crossing_time_points(
-        -1 * pulse, 300000, -2000, gate_time, 0, pol_out, t_trig_times_out
+        -1 * pulse, 300000, -2000, gate_time, 0, n_out, pol_out, t_trig_times_out
     )
     assert np.isnan(t_trig_times_out).all()
     assert np.isnan(pol_out).all()
 
     # Check that pulses that never reach either threshold return all nan
     t_trig_times_out = np.zeros(5)
     pol_out = np.zeros(5)
     bi_level_zero_crossing_time_points(
-        pulse, 300000, 300000, gate_time, 0, pol_out, t_trig_times_out
+        pulse, 300000, 300000, gate_time, 0, n_out, pol_out, t_trig_times_out
     )
     assert np.isnan(t_trig_times_out).all()
     assert np.isnan(pol_out).all()
 
     # Check that pulses that go up and never cross zero again return all nan
     t_trig_times_out = np.zeros(5)
     pol_out = np.zeros(5)
     bi_level_zero_crossing_time_points(
-        np.linspace(-1, 100, 101), 4, -4, gate_time, 0, pol_out, t_trig_times_out
+        np.linspace(-1, 100, 101), 4, -4, gate_time, 0, n_out, pol_out, t_trig_times_out
     )
     assert np.isnan(t_trig_times_out).all()
     assert np.isnan(pol_out).all()
 
     # Check that pulses that go down and never cross zero again return all nan
     t_trig_times_out = np.zeros(5)
     pol_out = np.zeros(5)
     bi_level_zero_crossing_time_points(
-        -1 * np.linspace(-1, 100, 101), 4, -4, gate_time, 0, pol_out, t_trig_times_out
+        -1 * np.linspace(-1, 100, 101),
+        4,
+        -4,
+        gate_time,
+        0,
+        n_out,
+        pol_out,
+        t_trig_times_out,
     )
     assert np.isnan(t_trig_times_out).all()
     assert np.isnan(pol_out).all()
 
     # Check positive polarity pulses where only 2nd peak crosses the threshold
     scale_arr = np.full(8192 // 2, 1)
     scale_arr = np.insert(scale_arr, -1, np.full(8192 // 2, 5))
     t_trig_times_out = np.zeros(5)
     pol_out = np.zeros(5)
     bi_level_zero_crossing_time_points(
-        pulse * scale_arr, 2000, -20000, gate_time, 0, pol_out, t_trig_times_out
+        pulse * scale_arr, 2000, -20000, gate_time, 0, n_out, pol_out, t_trig_times_out
     )
     assert np.allclose(
         int(t_trig_times_out[0]), cross_2, rtol=1
     )  # only the 2nd time point should have been crossed
     assert int(pol_out[0]) == 1
 
     # Check positive polarity pulses where only 1st peak crosses the threshold
     scale_arr = np.full(8192 // 2, 5)
     scale_arr = np.insert(scale_arr, -1, np.full(8192 // 2, 1))
     t_trig_times_out = np.zeros(5)
     pol_out = np.zeros(5)
     bi_level_zero_crossing_time_points(
-        pulse * scale_arr, 2000, -20000, gate_time, 0, pol_out, t_trig_times_out
+        pulse * scale_arr, 2000, -20000, gate_time, 0, n_out, pol_out, t_trig_times_out
     )
     assert np.allclose(
         int(t_trig_times_out[0]), cross_1, rtol=1
     )  # only the 1st time point should have been crossed
     assert int(pol_out[0]) == 1
 
     # Check positive polarity pulses where only 2nd peak crosses both thresholds, but 1st peak passes negative but not within gate
     scale_arr = np.full(8192 // 2, 1)
     scale_arr = np.insert(scale_arr, -1, np.full(8192 // 2, 5))
     t_trig_times_out = np.zeros(5)
     pol_out = np.zeros(5)
     bi_level_zero_crossing_time_points(
-        pulse * scale_arr, 50000, -2000, gate_time, 0, pol_out, t_trig_times_out
+        pulse * scale_arr, 50000, -2000, gate_time, 0, n_out, pol_out, t_trig_times_out
     )
     assert np.allclose(
         int(t_trig_times_out[0]), cross_2, rtol=1
     )  # only the 2nd time point should have been crossed
     assert int(pol_out[0]) == 1
+
+    # Check for overflow. This should not fail and should return n_crossings greater than the length of the outputs
+    w_in = np.zeros(100, "float") * 10
+    w_in[::2] = -10
+    w_in[1::2] = 10
+    pol_out = np.zeros(30)
+    t_trig_out = np.zeros(30)
+    bi_level_zero_crossing_time_points(w_in, 1, 1, 10, 0, n_out, pol_out, t_trig_out)
+    assert np.all(pol_out == 0)
+    assert n_out[0] == 49
```

### Comparing `dspeed-1.3.0a6/tests/processors/test_transfer_function_convolver.py` & `dspeed-1.4.0a1/tests/processors/test_transfer_function_convolver.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/processors/test_wf_alignment.py` & `dspeed-1.4.0a1/tests/processors/test_wf_alignment.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/test_build_dsp.py` & `dspeed-1.4.0a1/tests/test_build_dsp.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/test_cli.py` & `dspeed-1.4.0a1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/test_list_parsing.py` & `dspeed-1.4.0a1/tests/test_list_parsing.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/test_numpy_constants_parsing.py` & `dspeed-1.4.0a1/tests/test_numpy_constants_parsing.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/test_processing_chain.py` & `dspeed-1.4.0a1/tests/test_processing_chain.py`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/vis/configs/hpge-dsp-config.json` & `dspeed-1.4.0a1/tests/vis/configs/hpge-dsp-config.json`

 * *Files identical despite different names*

### Comparing `dspeed-1.3.0a6/tests/vis/test_waveform_browser.py` & `dspeed-1.4.0a1/tests/vis/test_waveform_browser.py`

 * *Files identical despite different names*

