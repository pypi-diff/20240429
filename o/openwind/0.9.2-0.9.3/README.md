# Comparing `tmp/openwind-0.9.2.tar.gz` & `tmp/openwind-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openwind-0.9.2.tar", last modified: Tue Jan  3 10:45:59 2023, max compression
+gzip compressed data, was "dist/openwind-0.9.3.tar", last modified: Wed Feb  8 14:52:10 2023, max compression
```

## Comparing `openwind-0.9.2.tar` & `openwind-0.9.3.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-01-03 10:45:59.000000 openwind-0.9.2/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      971 2023-01-03 10:43:30.000000 openwind-0.9.2/setup.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-01-03 10:45:59.000000 openwind-0.9.2/openwind/
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-01-03 10:45:59.000000 openwind-0.9.2/openwind/inversion/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     9404 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/inversion/observation.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    13478 2022-04-07 13:53:26.000000 openwind-0.9.2/openwind/inversion/display_inversion.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    55300 2023-01-03 10:32:59.000000 openwind-0.9.2/openwind/inversion/inverse_frequential_response.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      948 2021-03-09 10:33:40.000000 openwind-0.9.2/openwind/inversion/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     6059 2021-12-14 16:32:36.000000 openwind-0.9.2/openwind/tracker.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-01-03 10:45:59.000000 openwind-0.9.2/openwind/discretization/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    15282 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/discretization/mesh.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    12741 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/discretization/discretized_pipe.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4304 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/discretization/element.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1038 2021-03-09 10:33:40.000000 openwind-0.9.2/openwind/discretization/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     6752 2021-12-14 16:32:36.000000 openwind-0.9.2/openwind/discretization/glQuad.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-01-03 10:45:59.000000 openwind-0.9.2/openwind/technical/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    80866 2023-01-03 10:32:59.000000 openwind-0.9.2/openwind/technical/instrument_geometry.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     4452 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/technical/default_excitator_parameters.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8839 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/technical/score.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    18773 2021-12-14 16:32:36.000000 openwind-0.9.2/openwind/technical/temporal_curves.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     9987 2023-01-03 10:32:59.000000 openwind-0.9.2/openwind/technical/fingering_chart.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    10069 2022-01-28 10:35:11.000000 openwind-0.9.2/openwind/technical/player.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1119 2021-12-14 16:32:36.000000 openwind-0.9.2/openwind/technical/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    11073 2023-01-03 10:32:59.000000 openwind-0.9.2/openwind/technical/parser.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6496 2021-12-14 16:32:36.000000 openwind-0.9.2/openwind/technical/proto_geometry.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11168 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/technical/adjust_instrument_geometry.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    28558 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/algo_optimization.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-01-03 10:45:59.000000 openwind-0.9.2/openwind/frequential/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     9368 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/frequential/frequential_component.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    12876 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/frequential/frequential_pipe_diffusive_representation.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     3013 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/frequential/frequential_source.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4058 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/frequential/frequential_radiation.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4428 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/frequential/frequential_junction_simple.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    12768 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/frequential/tmm_tools.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    59019 2023-01-03 10:32:59.000000 openwind-0.9.2/openwind/frequential/frequential_solver.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6503 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/frequential/frequential_pressure_condition.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    11579 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/frequential/frequential_pipe_fem.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     7748 2023-01-03 10:32:59.000000 openwind-0.9.2/openwind/frequential/frequential_junction_tjoint.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     9932 2022-05-23 10:21:16.000000 openwind-0.9.2/openwind/frequential/frequential_pipe_tmm.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2025 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/frequential/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     7366 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/frequential/frequential_junction_switch.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     6104 2021-03-09 10:33:40.000000 openwind-0.9.2/openwind/frequential/peakfinder.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5617 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/frequential/frequential_junction_discontinuity.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5804 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/frequential/frequential_radiation1dof.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    13196 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/frequential/frequential_interpolation.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    19759 2023-01-03 10:32:59.000000 openwind-0.9.2/openwind/impedance_tools.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    26991 2023-01-03 10:32:59.000000 openwind-0.9.2/openwind/impedance_computation.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    15520 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/parsing_tools.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1496 2023-01-03 10:43:30.000000 openwind-0.9.2/openwind/__init__.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-01-03 10:45:59.000000 openwind-0.9.2/openwind/continuous/
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    22897 2023-01-03 10:32:59.000000 openwind-0.9.2/openwind/continuous/junction.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    15847 2021-06-23 09:03:17.000000 openwind-0.9.2/openwind/continuous/excitator.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    11449 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/continuous/radiation_from_data.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5420 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/continuous/radiation_pulsating_sphere.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4790 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/continuous/scaling.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    33240 2023-01-03 10:32:59.000000 openwind-0.9.2/openwind/continuous/instrument_physics.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    25609 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/continuous/pipe.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4343 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/continuous/physics.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    18160 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/continuous/physical_radiation.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4966 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/continuous/radiation_model.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2749 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/continuous/__init__.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    17413 2021-12-14 16:32:36.000000 openwind-0.9.2/openwind/continuous/netlist.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    39775 2023-01-03 10:32:59.000000 openwind-0.9.2/openwind/continuous/thermoviscous_models.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    13192 2022-01-28 10:35:11.000000 openwind-0.9.2/openwind/continuous/radiation_silva.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8279 2023-01-03 10:32:59.000000 openwind-0.9.2/openwind/temporal_simulation.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-01-03 10:45:59.000000 openwind-0.9.2/openwind/temporal/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4727 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/temporal/execute_score.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2956 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/temporal/tsimplejunction.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    17260 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/temporal/tpipe_lossy.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3644 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/temporal/tflow_condition.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    18315 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/temporal/tpipe.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5572 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/temporal/tcomponent.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    18797 2021-12-14 16:32:36.000000 openwind-0.9.2/openwind/temporal/temporal_solver.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    15515 2021-12-14 16:32:36.000000 openwind-0.9.2/openwind/temporal/tjunction.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6431 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/temporal/tradiation.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1684 2021-12-14 16:32:36.000000 openwind-0.9.2/openwind/temporal/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     7400 2022-04-07 13:53:26.000000 openwind-0.9.2/openwind/temporal/treed1dof.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2608 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/temporal/tpressure_condition.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3465 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/temporal/utils.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     4902 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/temporal/recording_device.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3453 2022-09-02 09:01:43.000000 openwind-0.9.2/openwind/compute_transfer_matrix.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-01-03 10:45:59.000000 openwind-0.9.2/openwind/design/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     7433 2022-05-23 10:21:16.000000 openwind-0.9.2/openwind/design/exponential.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5809 2022-05-23 10:21:16.000000 openwind-0.9.2/openwind/design/cone.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    13391 2022-05-23 10:21:16.000000 openwind-0.9.2/openwind/design/design_shape.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    12478 2023-01-03 10:32:59.000000 openwind-0.9.2/openwind/design/bessel.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    10497 2022-05-23 10:21:16.000000 openwind-0.9.2/openwind/design/circle.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1637 2021-05-27 12:49:37.000000 openwind-0.9.2/openwind/design/__init__.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5590 2022-05-23 10:21:16.000000 openwind-0.9.2/openwind/design/shape_slice.py
--rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    22912 2022-05-23 10:21:16.000000 openwind-0.9.2/openwind/design/design_parameter.py
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    15723 2022-05-23 10:21:16.000000 openwind-0.9.2/openwind/design/spline.py
-drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-01-03 10:45:59.000000 openwind-0.9.2/openwind.egg-info/
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     3199 2023-01-03 10:45:59.000000 openwind-0.9.2/openwind.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2389 2023-01-03 10:45:59.000000 openwind-0.9.2/openwind.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)       20 2023-01-03 10:45:59.000000 openwind-0.9.2/openwind.egg-info/entry_points.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        1 2023-01-03 10:45:59.000000 openwind-0.9.2/openwind.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)       23 2023-01-03 10:45:59.000000 openwind-0.9.2/openwind.egg-info/requires.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        9 2023-01-03 10:45:59.000000 openwind-0.9.2/openwind.egg-info/top_level.txt
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2389 2023-01-03 10:45:59.000000 openwind-0.9.2/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)       38 2023-01-03 10:45:59.000000 openwind-0.9.2/setup.cfg
--rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1654 2021-12-14 16:32:36.000000 openwind-0.9.2/README.md
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-02-08 14:52:10.000000 openwind-0.9.3/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      971 2023-02-08 14:43:57.000000 openwind-0.9.3/setup.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-02-08 14:52:10.000000 openwind-0.9.3/openwind/
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-02-08 14:52:10.000000 openwind-0.9.3/openwind/inversion/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     9404 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/inversion/observation.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    13478 2022-04-07 13:53:26.000000 openwind-0.9.3/openwind/inversion/display_inversion.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    55300 2023-01-03 10:32:59.000000 openwind-0.9.3/openwind/inversion/inverse_frequential_response.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)      948 2021-03-09 10:33:40.000000 openwind-0.9.3/openwind/inversion/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     6059 2021-12-14 16:32:36.000000 openwind-0.9.3/openwind/tracker.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-02-08 14:52:10.000000 openwind-0.9.3/openwind/discretization/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    15282 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/discretization/mesh.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    12741 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/discretization/discretized_pipe.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4304 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/discretization/element.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1038 2021-03-09 10:33:40.000000 openwind-0.9.3/openwind/discretization/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     6752 2021-12-14 16:32:36.000000 openwind-0.9.3/openwind/discretization/glQuad.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-02-08 14:52:10.000000 openwind-0.9.3/openwind/technical/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    80875 2023-02-08 14:43:57.000000 openwind-0.9.3/openwind/technical/instrument_geometry.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     4452 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/technical/default_excitator_parameters.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8839 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/technical/score.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    18773 2021-12-14 16:32:36.000000 openwind-0.9.3/openwind/technical/temporal_curves.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     9987 2023-01-03 10:32:59.000000 openwind-0.9.3/openwind/technical/fingering_chart.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    10069 2022-01-28 10:35:11.000000 openwind-0.9.3/openwind/technical/player.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1119 2021-12-14 16:32:36.000000 openwind-0.9.3/openwind/technical/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    11052 2023-02-08 14:43:57.000000 openwind-0.9.3/openwind/technical/parser.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6496 2021-12-14 16:32:36.000000 openwind-0.9.3/openwind/technical/proto_geometry.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    11168 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/technical/adjust_instrument_geometry.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    28558 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/algo_optimization.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-02-08 14:52:10.000000 openwind-0.9.3/openwind/frequential/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     9368 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/frequential/frequential_component.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    12876 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/frequential/frequential_pipe_diffusive_representation.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     3013 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/frequential/frequential_source.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4058 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/frequential/frequential_radiation.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4428 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/frequential/frequential_junction_simple.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    12768 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/frequential/tmm_tools.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    59019 2023-01-03 10:32:59.000000 openwind-0.9.3/openwind/frequential/frequential_solver.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6503 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/frequential/frequential_pressure_condition.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    11579 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/frequential/frequential_pipe_fem.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     7748 2023-01-03 10:32:59.000000 openwind-0.9.3/openwind/frequential/frequential_junction_tjoint.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     9932 2022-05-23 10:21:16.000000 openwind-0.9.3/openwind/frequential/frequential_pipe_tmm.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2025 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/frequential/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     7366 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/frequential/frequential_junction_switch.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     6104 2021-03-09 10:33:40.000000 openwind-0.9.3/openwind/frequential/peakfinder.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5617 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/frequential/frequential_junction_discontinuity.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5804 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/frequential/frequential_radiation1dof.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    13196 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/frequential/frequential_interpolation.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    19759 2023-01-03 10:32:59.000000 openwind-0.9.3/openwind/impedance_tools.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    27492 2023-02-08 14:43:57.000000 openwind-0.9.3/openwind/impedance_computation.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    15520 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/parsing_tools.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1496 2023-02-08 14:43:57.000000 openwind-0.9.3/openwind/__init__.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-02-08 14:52:10.000000 openwind-0.9.3/openwind/continuous/
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    22897 2023-01-03 10:32:59.000000 openwind-0.9.3/openwind/continuous/junction.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    15847 2021-06-23 09:03:17.000000 openwind-0.9.3/openwind/continuous/excitator.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    11449 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/continuous/radiation_from_data.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     5420 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/continuous/radiation_pulsating_sphere.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4790 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/continuous/scaling.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    33240 2023-01-03 10:32:59.000000 openwind-0.9.3/openwind/continuous/instrument_physics.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    25609 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/continuous/pipe.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4343 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/continuous/physics.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    18160 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/continuous/physical_radiation.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4966 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/continuous/radiation_model.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2749 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/continuous/__init__.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    17413 2021-12-14 16:32:36.000000 openwind-0.9.3/openwind/continuous/netlist.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    39775 2023-01-03 10:32:59.000000 openwind-0.9.3/openwind/continuous/thermoviscous_models.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    13192 2022-01-28 10:35:11.000000 openwind-0.9.3/openwind/continuous/radiation_silva.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     8279 2023-01-03 10:32:59.000000 openwind-0.9.3/openwind/temporal_simulation.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-02-08 14:52:10.000000 openwind-0.9.3/openwind/temporal/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     4727 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/temporal/execute_score.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2956 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/temporal/tsimplejunction.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    17260 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/temporal/tpipe_lossy.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3644 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/temporal/tflow_condition.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    18315 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/temporal/tpipe.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5572 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/temporal/tcomponent.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    18797 2021-12-14 16:32:36.000000 openwind-0.9.3/openwind/temporal/temporal_solver.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    15515 2021-12-14 16:32:36.000000 openwind-0.9.3/openwind/temporal/tjunction.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     6431 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/temporal/tradiation.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     1684 2021-12-14 16:32:36.000000 openwind-0.9.3/openwind/temporal/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     7400 2022-04-07 13:53:26.000000 openwind-0.9.3/openwind/temporal/treed1dof.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     2608 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/temporal/tpressure_condition.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3465 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/temporal/utils.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     4902 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/temporal/recording_device.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)     3453 2022-09-02 09:01:43.000000 openwind-0.9.3/openwind/compute_transfer_matrix.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-02-08 14:52:10.000000 openwind-0.9.3/openwind/design/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     7433 2022-05-23 10:21:16.000000 openwind-0.9.3/openwind/design/exponential.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5809 2022-05-23 10:21:16.000000 openwind-0.9.3/openwind/design/cone.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    13391 2022-05-23 10:21:16.000000 openwind-0.9.3/openwind/design/design_shape.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    12478 2023-01-03 10:32:59.000000 openwind-0.9.3/openwind/design/bessel.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    10497 2022-05-23 10:21:16.000000 openwind-0.9.3/openwind/design/circle.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1637 2021-05-27 12:49:37.000000 openwind-0.9.3/openwind/design/__init__.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     5590 2022-05-23 10:21:16.000000 openwind-0.9.3/openwind/design/shape_slice.py
+-rwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)    22912 2022-05-23 10:21:16.000000 openwind-0.9.3/openwind/design/design_parameter.py
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)    15723 2022-05-23 10:21:16.000000 openwind-0.9.3/openwind/design/spline.py
+drwxrwxr-x   0 gitlab-runner   (999) gitlab-runner   (999)        0 2023-02-08 14:52:10.000000 openwind-0.9.3/openwind.egg-info/
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     3199 2023-02-08 14:52:09.000000 openwind-0.9.3/openwind.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2389 2023-02-08 14:52:08.000000 openwind-0.9.3/openwind.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)       20 2023-02-08 14:52:08.000000 openwind-0.9.3/openwind.egg-info/entry_points.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        1 2023-02-08 14:52:08.000000 openwind-0.9.3/openwind.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)       23 2023-02-08 14:52:08.000000 openwind-0.9.3/openwind.egg-info/requires.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)        9 2023-02-08 14:52:08.000000 openwind-0.9.3/openwind.egg-info/top_level.txt
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     2389 2023-02-08 14:52:10.000000 openwind-0.9.3/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)       38 2023-02-08 14:52:10.000000 openwind-0.9.3/setup.cfg
+-rw-rw-r--   0 gitlab-runner   (999) gitlab-runner   (999)     1654 2021-12-14 16:32:36.000000 openwind-0.9.3/README.md
```

### Comparing `openwind-0.9.2/setup.py` & `openwind-0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="openwind",
-    version="0.9.2",
+    version="0.9.3",
     description="Open source library to design wind instruments",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://files.inria.fr/openwind/docs",
     author="Makutu",
     author_email="openwind-contact@inria.fr",
     license="GPLv3",
```

### Comparing `openwind-0.9.2/openwind/inversion/observation.py` & `openwind-0.9.3/openwind/inversion/observation.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/inversion/display_inversion.py` & `openwind-0.9.3/openwind/inversion/display_inversion.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/inversion/inverse_frequential_response.py` & `openwind-0.9.3/openwind/inversion/inverse_frequential_response.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/inversion/__init__.py` & `openwind-0.9.3/openwind/inversion/__init__.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/tracker.py` & `openwind-0.9.3/openwind/tracker.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/discretization/mesh.py` & `openwind-0.9.3/openwind/discretization/mesh.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/discretization/discretized_pipe.py` & `openwind-0.9.3/openwind/discretization/discretized_pipe.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/discretization/element.py` & `openwind-0.9.3/openwind/discretization/element.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/discretization/__init__.py` & `openwind-0.9.3/openwind/discretization/__init__.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/discretization/glQuad.py` & `openwind-0.9.3/openwind/discretization/glQuad.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/technical/instrument_geometry.py` & `openwind-0.9.3/openwind/technical/instrument_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1644,19 +1644,20 @@
     def write_single_file(self, name, digit=5, unit='m', diameter=False, disp_optim=True, comments=''):
         """
         Write a unique file where everything is indicated (main bore, holes and fing chart)
 
         Each block of data is separated by a title such as
 
         .. code-block:: shell
+        
             **********Main Bore**********
             ...
             **********Side Components**********
             ...
-            **********Fingeirng Chart**********
+            **********Fingering Chart**********
             ...
 
         Parameters
         ----------
         name : string
             The name of the file where save the geometry.
         extension : string, optional
```

### Comparing `openwind-0.9.2/openwind/technical/default_excitator_parameters.py` & `openwind-0.9.3/openwind/technical/default_excitator_parameters.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/technical/score.py` & `openwind-0.9.3/openwind/technical/score.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/technical/temporal_curves.py` & `openwind-0.9.3/openwind/technical/temporal_curves.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/technical/fingering_chart.py` & `openwind-0.9.3/openwind/technical/fingering_chart.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/technical/player.py` & `openwind-0.9.3/openwind/technical/player.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/technical/__init__.py` & `openwind-0.9.3/openwind/technical/__init__.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/technical/parser.py` & `openwind-0.9.3/openwind/technical/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     if not (isinstance(bore_file, str) or isinstance(bore_file, list)):
         raise TypeError(f'Main bore data: expected "str" or "list" instance, not "{type(bore_file).__name__}"')
     if not (isinstance(hole_file, str) or isinstance(hole_file, list)):
         raise TypeError(f'Holes/Valves data: expected "str" or "list" instance, not "{type(hole_file).__name__}"')
     # if not (isinstance(fing_file, str) or isinstance(fing_file, list)):
     #     raise TypeError(f'Fing. Chart data: expected "str" or "list" instance, not "{type(fing_file).__name__}"')
-        
+
     # main bore and single file
     if isinstance(bore_file, list):
         bore_list = bore_file
         bore_opt = dict()
         hole_list = list()
         hole_opt = dict()
         fing_list = list()
@@ -97,15 +97,15 @@
 
     # fing_chart
     fing_list2 = interpret_data(fing_file)[0]
     if len(fing_list)>0 and len(fing_list2)>0:
         warnings.warn('The fingering data from the "single file" are ignored. Only the one from the "fingering chart file/list" are kept.')
         fing_list = fing_list2
     if not (isinstance(fing_list2, list) and len(fing_list2)==0):
-        fing_list = fing_list2 
+        fing_list = fing_list2
     return bore_list, hole_list, fing_list, bore_opt, hole_opt
 
 def interpret_single_file_lines(bore_lines:list):
     """
     Convert the lines of the unique file into the corresponding list and dict
 
     Parameters
@@ -170,15 +170,15 @@
     """
     if isinstance(data, str):  # We can chose to take real csv files as inputs
         with open(data) as file:
             lines = file.readlines()
         return interpret_lines(lines)
     else:
         return data, dict()             # or using directly lists or ow object
-        
+
 
 def interpret_lines(lines):
     """
     Transcript list of lines from file in a list of data raw.
 
     It is a very general method which only read each line, split the
     text w.r. to whitespaces and organise it in a list of list.
@@ -316,15 +316,15 @@
                                                                                   openwind.__version__))
 
 def get_comments_from_lines(lines):
     bore_header = ['x0', 'x1', 'type']
     comment_lines = [s[1:].strip() for s in lines if s.startswith('#')
                      and not all(head in s[1:].split() for head in bore_header)] # exclude the header line of the main bore
     return '\n'.join(comment_lines)
-    
+
 def get_comments_from_file(filename):
     with open(filename) as file:
         lines = file.readlines()
     return get_comments_from_lines(lines)
 
 def clean_label(label):
     """
```

### Comparing `openwind-0.9.2/openwind/technical/proto_geometry.py` & `openwind-0.9.3/openwind/technical/proto_geometry.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/technical/adjust_instrument_geometry.py` & `openwind-0.9.3/openwind/technical/adjust_instrument_geometry.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/algo_optimization.py` & `openwind-0.9.3/openwind/algo_optimization.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/frequential_component.py` & `openwind-0.9.3/openwind/frequential/frequential_component.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/frequential_pipe_diffusive_representation.py` & `openwind-0.9.3/openwind/frequential/frequential_pipe_diffusive_representation.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/frequential_source.py` & `openwind-0.9.3/openwind/frequential/frequential_source.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/frequential_radiation.py` & `openwind-0.9.3/openwind/frequential/frequential_radiation.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/frequential_junction_simple.py` & `openwind-0.9.3/openwind/frequential/frequential_junction_simple.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/tmm_tools.py` & `openwind-0.9.3/openwind/frequential/tmm_tools.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/frequential_solver.py` & `openwind-0.9.3/openwind/frequential/frequential_solver.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/frequential_pressure_condition.py` & `openwind-0.9.3/openwind/frequential/frequential_pressure_condition.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/frequential_pipe_fem.py` & `openwind-0.9.3/openwind/frequential/frequential_pipe_fem.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/frequential_junction_tjoint.py` & `openwind-0.9.3/openwind/frequential/frequential_junction_tjoint.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/frequential_pipe_tmm.py` & `openwind-0.9.3/openwind/frequential/frequential_pipe_tmm.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/__init__.py` & `openwind-0.9.3/openwind/frequential/__init__.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/frequential_junction_switch.py` & `openwind-0.9.3/openwind/frequential/frequential_junction_switch.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/peakfinder.py` & `openwind-0.9.3/openwind/frequential/peakfinder.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/frequential_junction_discontinuity.py` & `openwind-0.9.3/openwind/frequential/frequential_junction_discontinuity.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/frequential_radiation1dof.py` & `openwind-0.9.3/openwind/frequential/frequential_radiation1dof.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/frequential/frequential_interpolation.py` & `openwind-0.9.3/openwind/frequential/frequential_interpolation.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/impedance_tools.py` & `openwind-0.9.3/openwind/impedance_tools.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/impedance_computation.py` & `openwind-0.9.3/openwind/impedance_computation.py`

 * *Files 1% similar despite different names*

```diff
@@ -507,16 +507,14 @@
         """
         return self.__freq_model.resonance_frequencies(k)
 
     def resonance_peaks(self,k=5):
         """
         The resonance frequencies, quality factors and values of the impedance
 
-        Only available for the solving method 'modal'
-
         Parameters
         ----------
         k : int, optional
             The number of resonances included. The default is 5.
 
         Returns
         -------
@@ -526,14 +524,36 @@
             The quality factors (float)
 
             The impedance value at the resonance frequencies (complex)
 
         """
         return self.__freq_model.resonance_peaks(k)
 
+    def antiresonance_peaks(self,k=5):
+        """
+        The antiresonance frequencies, quality factors and values of the impedance
+
+
+        Parameters
+        ----------
+        k : int, optional
+            The number of resonances included. The default is 5.
+
+        Returns
+        -------
+        tuple of 3 lists
+            The antiresonance frequencies (float)
+
+            The quality factors (float)
+
+            The impedance value at the resonance frequencies (complex)
+
+        """
+        return self.__freq_model.antiresonance_peaks(k)
+
     def match_peaks_with_notes(self, concert_pitch_A=440, transposition = 0, k=5, display=False):
         """
         Matches resonance frequencies with notes frequencies in Hz, deviation in cents and notes names
         The user can specify a concert pitch and a transposing behavior for the instrument.
 
         Parameters
         ----------
```

### Comparing `openwind-0.9.2/openwind/parsing_tools.py` & `openwind-0.9.3/openwind/parsing_tools.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/__init__.py` & `openwind-0.9.3/openwind/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 __author__ = ["Juliette Chabassier", "Augustin Ernoult", "Olivier Geber",
               "Alexis Thibault", "Tobias Van Baarsel"]
 __copyright__ = "Copyright 2020, Inria"
 __credits__ = ["Juliette Chabassier", "Augustin Ernoult", "Olivier Geber",
                "Alexis Thibault", "Tobias Van Baarsel"]
 __license__ = "GPL 3.0"
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 __email__ = "openwind-contact@inria.fr"
 __status__ = "Dev"
 
 
 from .technical import InstrumentGeometry, Player
 from .continuous import InstrumentPhysics, Physics
 from .impedance_computation import ImpedanceComputation
```

### Comparing `openwind-0.9.2/openwind/continuous/junction.py` & `openwind-0.9.3/openwind/continuous/junction.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/continuous/excitator.py` & `openwind-0.9.3/openwind/continuous/excitator.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/continuous/radiation_from_data.py` & `openwind-0.9.3/openwind/continuous/radiation_from_data.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/continuous/radiation_pulsating_sphere.py` & `openwind-0.9.3/openwind/continuous/radiation_pulsating_sphere.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/continuous/scaling.py` & `openwind-0.9.3/openwind/continuous/scaling.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/continuous/instrument_physics.py` & `openwind-0.9.3/openwind/continuous/instrument_physics.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/continuous/pipe.py` & `openwind-0.9.3/openwind/continuous/pipe.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/continuous/physics.py` & `openwind-0.9.3/openwind/continuous/physics.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/continuous/physical_radiation.py` & `openwind-0.9.3/openwind/continuous/physical_radiation.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/continuous/radiation_model.py` & `openwind-0.9.3/openwind/continuous/radiation_model.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/continuous/__init__.py` & `openwind-0.9.3/openwind/continuous/__init__.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/continuous/netlist.py` & `openwind-0.9.3/openwind/continuous/netlist.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/continuous/thermoviscous_models.py` & `openwind-0.9.3/openwind/continuous/thermoviscous_models.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/continuous/radiation_silva.py` & `openwind-0.9.3/openwind/continuous/radiation_silva.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/temporal_simulation.py` & `openwind-0.9.3/openwind/temporal_simulation.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/temporal/execute_score.py` & `openwind-0.9.3/openwind/temporal/execute_score.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/temporal/tsimplejunction.py` & `openwind-0.9.3/openwind/temporal/tsimplejunction.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/temporal/tpipe_lossy.py` & `openwind-0.9.3/openwind/temporal/tpipe_lossy.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/temporal/tflow_condition.py` & `openwind-0.9.3/openwind/temporal/tflow_condition.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/temporal/tpipe.py` & `openwind-0.9.3/openwind/temporal/tpipe.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/temporal/tcomponent.py` & `openwind-0.9.3/openwind/temporal/tcomponent.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/temporal/temporal_solver.py` & `openwind-0.9.3/openwind/temporal/temporal_solver.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/temporal/tjunction.py` & `openwind-0.9.3/openwind/temporal/tjunction.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/temporal/tradiation.py` & `openwind-0.9.3/openwind/temporal/tradiation.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/temporal/__init__.py` & `openwind-0.9.3/openwind/temporal/__init__.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/temporal/treed1dof.py` & `openwind-0.9.3/openwind/temporal/treed1dof.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/temporal/tpressure_condition.py` & `openwind-0.9.3/openwind/temporal/tpressure_condition.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/temporal/utils.py` & `openwind-0.9.3/openwind/temporal/utils.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/temporal/recording_device.py` & `openwind-0.9.3/openwind/temporal/recording_device.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/compute_transfer_matrix.py` & `openwind-0.9.3/openwind/compute_transfer_matrix.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/design/exponential.py` & `openwind-0.9.3/openwind/design/exponential.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/design/cone.py` & `openwind-0.9.3/openwind/design/cone.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/design/design_shape.py` & `openwind-0.9.3/openwind/design/design_shape.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/design/bessel.py` & `openwind-0.9.3/openwind/design/bessel.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/design/circle.py` & `openwind-0.9.3/openwind/design/circle.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/design/__init__.py` & `openwind-0.9.3/openwind/design/__init__.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/design/shape_slice.py` & `openwind-0.9.3/openwind/design/shape_slice.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/design/design_parameter.py` & `openwind-0.9.3/openwind/design/design_parameter.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind/design/spline.py` & `openwind-0.9.3/openwind/design/spline.py`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind.egg-info/SOURCES.txt` & `openwind-0.9.3/openwind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openwind-0.9.2/openwind.egg-info/PKG-INFO` & `openwind-0.9.3/openwind.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwind
-Version: 0.9.2
+Version: 0.9.3
 Summary: Open source library to design wind instruments
 Home-page: https://files.inria.fr/openwind/docs
 Author: Makutu
 Author-email: openwind-contact@inria.fr
 License: GPLv3
 Description: # Open Wind Instrument Design
```

### Comparing `openwind-0.9.2/PKG-INFO` & `openwind-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openwind
-Version: 0.9.2
+Version: 0.9.3
 Summary: Open source library to design wind instruments
 Home-page: https://files.inria.fr/openwind/docs
 Author: Makutu
 Author-email: openwind-contact@inria.fr
 License: GPLv3
 Description: # Open Wind Instrument Design
```

### Comparing `openwind-0.9.2/README.md` & `openwind-0.9.3/README.md`

 * *Files identical despite different names*

