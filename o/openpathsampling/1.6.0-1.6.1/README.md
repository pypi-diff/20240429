# Comparing `tmp/openpathsampling-1.6.0.tar.gz` & `tmp/openpathsampling-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openpathsampling-1.6.0.tar", last modified: Fri Jan  5 23:22:16 2024, max compression
+gzip compressed data, was "openpathsampling-1.6.1.tar", last modified: Mon Apr 29 14:38:38 2024, max compression
```

## Comparing `openpathsampling-1.6.0.tar` & `openpathsampling-1.6.1.tar`

### file list

```diff
@@ -1,355 +1,374 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.596125 openpathsampling-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-01-05 23:22:16.596125 openpathsampling-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.536125 openpathsampling-1.6.0/openpathsampling/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-01-05 23:22:16.000000 openpathsampling-1.6.0/openpathsampling/_installed_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.540125 openpathsampling-1.6.0/openpathsampling/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17242 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/channel_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/ensemble_representation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16272 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/path_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/reactive_flux_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    18908 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/replica_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    12649 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/shooting_point_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/sshooting_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.540125 openpathsampling-1.6.0/openpathsampling/analysis/tis/
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/tis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15834 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/tis/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/tis/crossing_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/tis/flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/tis/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15647 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/tis/standard_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    15698 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/analysis/trajectory_transition_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.540125 openpathsampling-1.6.0/openpathsampling/beta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/beta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16334 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/beta/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/bias_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    24689 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/collectivevariable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.540125 openpathsampling-1.6.0/openpathsampling/collectivevariables/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/collectivevariables/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/collectivevariables/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12322 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/collectivevariables/plumed_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    10807 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/deprecations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.544125 openpathsampling-1.6.0/openpathsampling/engines/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/delayedinterrupt.py
--rw-r--r--   0 runner    (1001) docker     (127)    27435 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/dynamics_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/external_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.544125 openpathsampling-1.6.0/openpathsampling/engines/external_snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/external_snapshots/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/external_snapshots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.544125 openpathsampling-1.6.0/openpathsampling/engines/external_snapshots/features/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/external_snapshots/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/external_snapshots/features/box_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/external_snapshots/features/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/external_snapshots/features/file_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/external_snapshots/features/velocities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/external_snapshots/snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.548125 openpathsampling-1.6.0/openpathsampling/engines/features/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/features/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/features/box_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/features/coordinates.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/features/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/features/kinetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/features/numpydoctools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9424 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/features/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/features/statics.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/features/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/features/velocities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.548125 openpathsampling-1.6.0/openpathsampling/engines/gromacs/
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/gromacs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14183 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/gromacs/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.548125 openpathsampling-1.6.0/openpathsampling/engines/openmm/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/openmm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17373 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/openmm/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.548125 openpathsampling-1.6.0/openpathsampling/engines/openmm/features/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/openmm/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/openmm/features/instantaneous_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/openmm/features/masses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/openmm/features/traj_quantities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/openmm/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    14322 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/openmm/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/openmm/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.548125 openpathsampling-1.6.0/openpathsampling/engines/toy/
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/toy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/toy/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.548125 openpathsampling-1.6.0/openpathsampling/engines/toy/features/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/toy/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/toy/features/instantaneous_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/toy/integrators.py
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/toy/pes.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/toy/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/toy/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/engines/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)   116957 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.552125 openpathsampling-1.6.0/openpathsampling/ensembles/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/ensembles/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/ensembles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/ensembles/visit_all_states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.552125 openpathsampling-1.6.0/openpathsampling/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.556125 openpathsampling-1.6.0/openpathsampling/experimental/simstore/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/attribute_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/callable_codec.py
--rw-r--r--   0 runner    (1001) docker     (127)    17636 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/class_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/class_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/custom_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/dict_serialization_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/memory_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/my_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.556125 openpathsampling-1.6.0/openpathsampling/experimental/simstore/regressions/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/regressions/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/regressions/test_numpy_sfrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/serialization_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    25640 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/sql_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    21480 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/storable_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    28000 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/tags_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_attribute_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_callable_codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     8737 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_class_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_custom_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_dict_serialization_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_serialization_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_sql_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    19305 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_storable_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    11247 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_storable_function_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_tags_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_type_ident.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/type_ident.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/uuids.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/simstore/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.560125 openpathsampling-1.6.0/openpathsampling/experimental/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/collective_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/mdtraj_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/monkey_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)    14961 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/ops_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/simtk_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/snapshots_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/test_collective_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/test_mdtraj_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/test_monkey_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/test_pathsampling.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/test_regressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/test_simtk_unit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/test_snapshot_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/test_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/experimental/storage/test_snapshots_table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.564125 openpathsampling-1.6.0/openpathsampling/high_level/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/high_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14534 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/high_level/interface_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    38608 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/high_level/move_scheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    46314 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/high_level/move_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/high_level/ms_outer_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    39531 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/high_level/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/high_level/part_in_b_tps.py
--rw-r--r--   0 runner    (1001) docker     (127)    20564 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/high_level/transition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/integration_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/logging.conf
--rw-r--r--   0 runner    (1001) docker     (127)    18289 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/movechange.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.564125 openpathsampling-1.6.0/openpathsampling/netcdfplus/
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15340 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    12401 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13834 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/chaindict.py
--rw-r--r--   0 runner    (1001) docker     (127)    27698 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/dictify.py
--rw-r--r--   0 runner    (1001) docker     (127)    43227 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/netcdfplus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.568125 openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/indexed.py
--rw-r--r--   0 runner    (1001) docker     (127)    18069 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/named.py
--rw-r--r--   0 runner    (1001) docker     (127)    39528 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/netcdfplus/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.568125 openpathsampling-1.6.0/openpathsampling/numerics/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/numerics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26899 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/numerics/histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/numerics/lookup_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/numerics/resampling_statistics.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20330 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/numerics/wham.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/ops_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    87413 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/pathmover.py
--rw-r--r--   0 runner    (1001) docker     (127)    16615 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/pathmover_inout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.568125 openpathsampling-1.6.0/openpathsampling/pathmovers/
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/pathmovers/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/pathmovers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/pathmovers/move_schemes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/pathmovers/move_strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)    22342 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/pathmovers/spring_shooting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.568125 openpathsampling-1.6.0/openpathsampling/pathsimulators/
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/pathsimulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13754 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/pathsimulators/bootstrap_init_conds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/pathsimulators/direct_md.py
--rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/pathsimulators/path_sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/pathsimulators/path_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/pathsimulators/reactive_flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     9823 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/pathsimulators/shoot_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/pathsimulators/sshooting_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    10380 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/range_logic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.572125 openpathsampling-1.6.0/openpathsampling/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/resources/debug_logging.conf
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/resources/engine_debug.conf
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/resources/logging.conf
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/resources/vis.css
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/rng.py
--rw-r--r--   0 runner    (1001) docker     (127)    33381 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/shooting.py
--rw-r--r--   0 runner    (1001) docker     (127)    20477 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/snapshot_modifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/step_visualizer_2D.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.572125 openpathsampling-1.6.0/openpathsampling/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/storage/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)    17720 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/storage/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.572125 openpathsampling-1.6.0/openpathsampling/storage/stores/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/storage/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/storage/stores/collectivevariable.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/storage/stores/mcstep.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/storage/stores/movechange.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/storage/stores/pathsimulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/storage/stores/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/storage/stores/snapshot_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/storage/stores/snapshot_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/storage/stores/snapshot_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    25070 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/storage/stores/snapshot_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/storage/stores/trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/storage/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.572125 openpathsampling-1.6.0/openpathsampling/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/strategies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.584125 openpathsampling-1.6.0/openpathsampling/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.584125 openpathsampling-1.6.0/openpathsampling/tests/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/analysis/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.588125 openpathsampling-1.6.0/openpathsampling/tests/analysis/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/analysis/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/analysis/utils/fixture_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/analysis/utils/mock_movers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/analysis/utils/test_fixture_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    13319 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/analysis/utils/test_mock_movers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.588125 openpathsampling-1.6.0/openpathsampling/tests/external_engine/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/external_engine/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/external_engine/engine.c
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/external_engine/microtest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.588125 openpathsampling-1.6.0/openpathsampling/tests/pathsimulators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/pathsimulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21783 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/pathsimulators/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)    15385 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_bias_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    16126 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_channel_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    12519 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_collectivevariable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.588125 openpathsampling-1.6.0/openpathsampling/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)  1338434 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_data/ala_small_traj.pdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.592125 openpathsampling-1.6.0/openpathsampling/tests/test_data/apis/
--rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_data/apis/ops1x0_api.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.592125 openpathsampling-1.6.0/openpathsampling/tests/test_data/gromacs_engine/
--rw-r--r--   0 runner    (1001) docker     (127)    74370 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_data/gromacs_engine/conf.gro
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_data/gromacs_engine/md.mdp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.592125 openpathsampling-1.6.0/openpathsampling/tests/test_data/gromacs_engine/project_trr/
--rw-r--r--   0 runner    (1001) docker     (127)   158976 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_data/gromacs_engine/project_trr/0000000.trr
--rw-r--r--   0 runner    (1001) docker     (127)  2026563 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_data/gromacs_engine/project_trr/0000099.trr
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_data/gromacs_engine/topol.top
--rw-r--r--   0 runner    (1001) docker     (127)   158976 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_data/gromacs_engine/traj.trr
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.596125 openpathsampling-1.6.0/openpathsampling/tests/test_data/plumed_wrapper/
--rwxr-xr-x   0 runner    (1001) docker     (127)   134196 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_data/plumed_wrapper/AD_initial_frame.pdb
--rwxr-xr-x   0 runner    (1001) docker     (127)     2225 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_data/plumed_wrapper/AD_plumed_rmsd.pdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.596125 openpathsampling-1.6.0/openpathsampling/tests/test_data/reduce_box_vects/
--rw-r--r--   0 runner    (1001) docker     (127)    34418 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_data/reduce_box_vects/dna.gro
--rw-r--r--   0 runner    (1001) docker     (127)    36768 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_data/reduce_box_vects/dna.trr
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_data/tip4p_water.pdb
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_dynamicsengine.py
--rw-r--r--   0 runner    (1001) docker     (127)   107463 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_external_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_external_snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    17373 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_gromacs_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    10793 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_integration_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9150 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_interface_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5160 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_lookup_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_mdtraj_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    49245 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_movescheme.py
--rw-r--r--   0 runner    (1001) docker     (127)    61361 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_movestrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6895 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_ms_outer_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_netcdfplus_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    25143 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    10510 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_openmm_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_openmm_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_openmm_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_part_in_b_tps.py
--rw-r--r--   0 runner    (1001) docker     (127)    11862 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_path_histogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    62878 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_pathmover.py
--rw-r--r--   0 runner    (1001) docker     (127)    38374 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_pathsimulator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8249 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_plumed_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_pyemma_cv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_range_logic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10270 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_reactive_flux_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_resampling_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_rng.py
--rw-r--r--   0 runner    (1001) docker     (127)     7975 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_shooting.py
--rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_shooting_point_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    31385 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_snapshot_modifier.py
--rw-r--r--   0 runner    (1001) docker     (127)    18031 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_spring_shooting.py
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_sshooting_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_sshooting_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13697 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    48655 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_tis_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    14271 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_toy_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_toy_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_trajectory_transition_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_transitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_visit_all_states.py
--rw-r--r--   0 runner    (1001) docker     (127)    16495 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tests/test_wham.py
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    14599 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/treelogic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    92848 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/visualize.py
--rw-r--r--   0 runner    (1001) docker     (127)    21931 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/openpathsampling/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 23:22:16.596125 openpathsampling-1.6.0/openpathsampling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-01-05 23:22:16.000000 openpathsampling-1.6.0/openpathsampling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14475 2024-01-05 23:22:16.000000 openpathsampling-1.6.0/openpathsampling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 23:22:16.000000 openpathsampling-1.6.0/openpathsampling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-05 23:22:16.000000 openpathsampling-1.6.0/openpathsampling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-05 23:22:16.000000 openpathsampling-1.6.0/openpathsampling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-01-05 23:22:16.600125 openpathsampling-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-01-05 23:22:04.000000 openpathsampling-1.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.847593 openpathsampling-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-29 14:38:27.000000 openpathsampling-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-29 14:38:27.000000 openpathsampling-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-29 14:38:38.847593 openpathsampling-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-29 14:38:27.000000 openpathsampling-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.787594 openpathsampling-1.6.1/devtools/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-29 14:38:27.000000 openpathsampling-1.6.1/devtools/autorelease_check.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.787594 openpathsampling-1.6.1/devtools/ci/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2258 2024-04-29 14:38:27.000000 openpathsampling-1.6.1/devtools/ci/push-docs-to-s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-29 14:38:27.000000 openpathsampling-1.6.1/devtools/setup_cfg_reqs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.787594 openpathsampling-1.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    11452 2024-04-29 14:38:27.000000 openpathsampling-1.6.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.787594 openpathsampling-1.6.1/docs/copyfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-29 14:38:27.000000 openpathsampling-1.6.1/docs/copyfiles/copyfiles.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      821 2024-04-29 14:38:27.000000 openpathsampling-1.6.1/docs/premake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.787594 openpathsampling-1.6.1/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)     7851 2024-04-29 14:38:27.000000 openpathsampling-1.6.1/docs/sphinxext/notebook_sphinxext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-29 14:38:27.000000 openpathsampling-1.6.1/docs/sphinxext/pandoc_sphinxext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.787594 openpathsampling-1.6.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.787594 openpathsampling-1.6.1/examples/alanine_dipeptide_mstis/
+-rw-r--r--   0 runner    (1001) docker     (127)     7508 2024-04-29 14:38:27.000000 openpathsampling-1.6.1/examples/alanine_dipeptide_mstis/alatools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/examples/prep_example_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.787594 openpathsampling-1.6.1/examples/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     3957 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/examples/resources/toy_plot_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.791594 openpathsampling-1.6.1/openpathsampling/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-29 14:38:38.000000 openpathsampling-1.6.1/openpathsampling/_installed_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.795594 openpathsampling-1.6.1/openpathsampling/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17242 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/channel_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/ensemble_representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16272 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/path_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/reactive_flux_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18908 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/replica_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12649 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/shooting_point_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10214 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/sshooting_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.795594 openpathsampling-1.6.1/openpathsampling/analysis/tis/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/tis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15834 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/tis/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/tis/crossing_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14062 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/tis/flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/tis/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15647 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/tis/standard_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15698 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/analysis/trajectory_transition_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.795594 openpathsampling-1.6.1/openpathsampling/beta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/beta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16334 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/beta/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12928 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/bias_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24734 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/collectivevariable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.795594 openpathsampling-1.6.1/openpathsampling/collectivevariables/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/collectivevariables/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/collectivevariables/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12322 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/collectivevariables/plumed_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/deprecations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.795594 openpathsampling-1.6.1/openpathsampling/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/delayedinterrupt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27435 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/dynamics_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12066 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/external_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.799594 openpathsampling-1.6.1/openpathsampling/engines/external_snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/external_snapshots/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/external_snapshots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.799594 openpathsampling-1.6.1/openpathsampling/engines/external_snapshots/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/external_snapshots/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/external_snapshots/features/box_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/external_snapshots/features/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/external_snapshots/features/file_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/external_snapshots/features/velocities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/external_snapshots/snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.799594 openpathsampling-1.6.1/openpathsampling/engines/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/features/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/features/box_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/features/coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/features/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/features/kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6302 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/features/numpydoctools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9424 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/features/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/features/statics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/features/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/features/velocities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.799594 openpathsampling-1.6.1/openpathsampling/engines/gromacs/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/gromacs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14183 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/gromacs/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.803594 openpathsampling-1.6.1/openpathsampling/engines/openmm/
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/openmm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17373 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/openmm/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.803594 openpathsampling-1.6.1/openpathsampling/engines/openmm/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/openmm/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/openmm/features/instantaneous_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/openmm/features/masses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/openmm/features/traj_quantities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/openmm/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14322 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/openmm/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/openmm/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7827 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.803594 openpathsampling-1.6.1/openpathsampling/engines/toy/
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/toy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/toy/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.803594 openpathsampling-1.6.1/openpathsampling/engines/toy/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/toy/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/toy/features/instantaneous_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/toy/integrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/toy/pes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/toy/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/toy/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18497 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/engines/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116957 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.803594 openpathsampling-1.6.1/openpathsampling/ensembles/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/ensembles/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/ensembles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/ensembles/visit_all_states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.803594 openpathsampling-1.6.1/openpathsampling/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.811594 openpathsampling-1.6.1/openpathsampling/experimental/simstore/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/attribute_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/callable_codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17636 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/class_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/class_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/custom_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/dict_serialization_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/memory_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/my_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.811594 openpathsampling-1.6.1/openpathsampling/experimental/simstore/regressions/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/regressions/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/regressions/test_numpy_sfrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/serialization_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25640 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/sql_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21480 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/storable_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28000 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/tags_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1755 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_attribute_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_callable_codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8737 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_class_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_custom_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_dict_serialization_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5844 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10635 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_serialization_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_sql_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19305 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_storable_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11247 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_storable_function_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_tags_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_type_ident.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/type_ident.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/uuids.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/simstore/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.815594 openpathsampling-1.6.1/openpathsampling/experimental/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4682 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/collective_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/mdtraj_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/monkey_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14961 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/ops_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/simtk_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/snapshots_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/test_collective_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/test_mdtraj_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/test_monkey_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/test_pathsampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/test_simtk_unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/test_snapshot_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/test_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/experimental/storage/test_snapshots_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.815594 openpathsampling-1.6.1/openpathsampling/high_level/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/high_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14534 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/high_level/interface_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38608 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/high_level/move_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46314 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/high_level/move_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/high_level/ms_outer_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39531 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/high_level/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/high_level/part_in_b_tps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20564 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/high_level/transition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/integration_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/logging.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    18289 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/movechange.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.819594 openpathsampling-1.6.1/openpathsampling/netcdfplus/
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15337 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12401 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13834 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/chaindict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27698 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/dictify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43227 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/netcdfplus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.819594 openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5990 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/indexed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18069 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/named.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39528 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/netcdfplus/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.819594 openpathsampling-1.6.1/openpathsampling/numerics/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/numerics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26899 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/numerics/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/numerics/lookup_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/numerics/resampling_statistics.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20330 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/numerics/wham.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/ops_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87413 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/pathmover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16615 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/pathmover_inout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.819594 openpathsampling-1.6.1/openpathsampling/pathmovers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/pathmovers/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/pathmovers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/pathmovers/move_schemes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/pathmovers/move_strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22342 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/pathmovers/spring_shooting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.823593 openpathsampling-1.6.1/openpathsampling/pathsimulators/
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/pathsimulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13754 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/pathsimulators/bootstrap_init_conds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/pathsimulators/direct_md.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/pathsimulators/path_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/pathsimulators/path_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/pathsimulators/reactive_flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9823 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/pathsimulators/shoot_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/pathsimulators/sshooting_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10380 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/range_logic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.823593 openpathsampling-1.6.1/openpathsampling/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/resources/debug_logging.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/resources/engine_debug.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/resources/logging.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/resources/vis.css
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/rng.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33381 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/shooting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20477 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/snapshot_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4280 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/step_visualizer_2D.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.823593 openpathsampling-1.6.1/openpathsampling/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/storage/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17720 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/storage/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.827593 openpathsampling-1.6.1/openpathsampling/storage/stores/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/storage/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/storage/stores/collectivevariable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/storage/stores/mcstep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/storage/stores/movechange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/storage/stores/pathsimulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/storage/stores/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/storage/stores/snapshot_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/storage/stores/snapshot_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/storage/stores/snapshot_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25070 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/storage/stores/snapshot_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/storage/stores/trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/storage/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.827593 openpathsampling-1.6.1/openpathsampling/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/strategies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.835593 openpathsampling-1.6.1/openpathsampling/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.835593 openpathsampling-1.6.1/openpathsampling/tests/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/analysis/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.839593 openpathsampling-1.6.1/openpathsampling/tests/analysis/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/analysis/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/analysis/utils/fixture_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/analysis/utils/mock_movers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/analysis/utils/test_fixture_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13319 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/analysis/utils/test_mock_movers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.839593 openpathsampling-1.6.1/openpathsampling/tests/external_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/external_engine/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/external_engine/engine.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/external_engine/microtest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.839593 openpathsampling-1.6.1/openpathsampling/tests/pathsimulators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/pathsimulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21562 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/pathsimulators/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_bias_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15831 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_channel_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12471 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_collectivevariable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.839593 openpathsampling-1.6.1/openpathsampling/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1338434 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_data/ala_small_traj.pdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.839593 openpathsampling-1.6.1/openpathsampling/tests/test_data/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)    10794 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_data/apis/ops1x0_api.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.843593 openpathsampling-1.6.1/openpathsampling/tests/test_data/gromacs_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)    74370 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_data/gromacs_engine/conf.gro
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_data/gromacs_engine/md.mdp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.843593 openpathsampling-1.6.1/openpathsampling/tests/test_data/gromacs_engine/project_trr/
+-rw-r--r--   0 runner    (1001) docker     (127)   158976 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_data/gromacs_engine/project_trr/0000000.trr
+-rw-r--r--   0 runner    (1001) docker     (127)  2026563 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_data/gromacs_engine/project_trr/0000099.trr
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_data/gromacs_engine/topol.top
+-rw-r--r--   0 runner    (1001) docker     (127)   158976 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_data/gromacs_engine/traj.trr
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.847593 openpathsampling-1.6.1/openpathsampling/tests/test_data/plumed_wrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   134196 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_data/plumed_wrapper/AD_initial_frame.pdb
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2225 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_data/plumed_wrapper/AD_plumed_rmsd.pdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.847593 openpathsampling-1.6.1/openpathsampling/tests/test_data/reduce_box_vects/
+-rw-r--r--   0 runner    (1001) docker     (127)    34418 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_data/reduce_box_vects/dna.gro
+-rw-r--r--   0 runner    (1001) docker     (127)    36768 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_data/reduce_box_vects/dna.trr
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_data/tip4p_water.pdb
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_dynamicsengine.py
+-rw-r--r--   0 runner    (1001) docker     (127)   106442 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_external_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_external_snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17523 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_gromacs_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_integration_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8804 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_interface_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4988 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_lookup_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_mdtraj_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48731 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_movescheme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60390 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_movestrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_ms_outer_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_netcdfplus_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23766 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_openmm_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_openmm_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_openmm_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_part_in_b_tps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11573 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_path_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62878 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_pathmover.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37594 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_pathsimulator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8249 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_plumed_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_pyemma_cv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_range_logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_reactive_flux_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_resampling_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_rng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7658 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10498 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_shooting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_shooting_point_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31385 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_snapshot_modifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17835 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_spring_shooting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_sshooting_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_sshooting_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13594 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48189 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_tis_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14115 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_toy_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_toy_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11840 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_trajectory_transition_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_transitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_visit_all_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16495 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8999 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tests/test_wham.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14587 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/treelogic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    92848 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21931 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/openpathsampling/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:38:38.847593 openpathsampling-1.6.1/openpathsampling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-29 14:38:38.000000 openpathsampling-1.6.1/openpathsampling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14806 2024-04-29 14:38:38.000000 openpathsampling-1.6.1/openpathsampling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:38:38.000000 openpathsampling-1.6.1/openpathsampling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-29 14:38:38.000000 openpathsampling-1.6.1/openpathsampling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-29 14:38:38.000000 openpathsampling-1.6.1/openpathsampling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-29 14:38:38.847593 openpathsampling-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-29 14:38:28.000000 openpathsampling-1.6.1/setup.py
```

### Comparing `openpathsampling-1.6.0/LICENSE` & `openpathsampling-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/PKG-INFO` & `openpathsampling-1.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpathsampling
-Version: 1.6.0
+Version: 1.6.1
 Summary: A Python package for path sampling simulations
 Home-page: https://github.com/openpathsampling/openpathsampling
 Author: David W.H. Swenson, Jan-Hendrik Prinz, John D. Chodera, and Peter G. Bolhuis
 Author-email: dwhs@hyperblazer.net
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -16,37 +16,36 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: <3.12,>3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: future
 Requires-Dist: psutil
-Requires-Dist: numpy
+Requires-Dist: numpy<2.0
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: netcdf4
 Requires-Dist: svgwrite
 Requires-Dist: networkx
 Requires-Dist: matplotlib
 Requires-Dist: ujson>=4.0.2
 Requires-Dist: dill
+Requires-Dist: sqlalchemy>=1.4.1
 Requires-Dist: mdtraj
 Provides-Extra: test
-Requires-Dist: nose; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: coveralls; extra == "test"
-Requires-Dist: nbval!=0.10.0; extra == "test"
+Requires-Dist: nbval>=0.10.0; extra == "test"
 Provides-Extra: simstore
-Requires-Dist: sqlalchemy>=1.4.1; extra == "simstore"
 
 [![Tests](https://github.com/openpathsampling/openpathsampling/workflows/Tests/badge.svg?branch=master)](https://github.com/openpathsampling/openpathsampling/actions?query=workflow%3ATests)
 [![codecov](https://codecov.io/gh/openpathsampling/openpathsampling/branch/master/graph/badge.svg?token=9W18VHasdb)](https://codecov.io/gh/openpathsampling/openpathsampling)
 
 # OpenPathSampling
 
 An open source Python framework for transition interface and path sampling
```

### Comparing `openpathsampling-1.6.0/README.md` & `openpathsampling-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/__init__.py` & `openpathsampling-1.6.1/openpathsampling/__init__.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/analysis/channel_analysis.py` & `openpathsampling-1.6.1/openpathsampling/analysis/channel_analysis.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/analysis/path_histogram.py` & `openpathsampling-1.6.1/openpathsampling/analysis/path_histogram.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/analysis/reactive_flux_analysis.py` & `openpathsampling-1.6.1/openpathsampling/analysis/reactive_flux_analysis.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/analysis/replica_network.py` & `openpathsampling-1.6.1/openpathsampling/analysis/replica_network.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/analysis/shooting_point_analysis.py` & `openpathsampling-1.6.1/openpathsampling/analysis/shooting_point_analysis.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/analysis/sshooting_analysis.py` & `openpathsampling-1.6.1/openpathsampling/analysis/sshooting_analysis.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/analysis/tis/core.py` & `openpathsampling-1.6.1/openpathsampling/analysis/tis/core.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/analysis/tis/crossing_probability.py` & `openpathsampling-1.6.1/openpathsampling/analysis/tis/crossing_probability.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/analysis/tis/flux.py` & `openpathsampling-1.6.1/openpathsampling/analysis/tis/flux.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/analysis/tis/misc.py` & `openpathsampling-1.6.1/openpathsampling/analysis/tis/misc.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/analysis/tis/standard_analysis.py` & `openpathsampling-1.6.1/openpathsampling/analysis/tis/standard_analysis.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/analysis/tools.py` & `openpathsampling-1.6.1/openpathsampling/analysis/tools.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/analysis/trajectory_transition_analysis.py` & `openpathsampling-1.6.1/openpathsampling/analysis/trajectory_transition_analysis.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/beta/hooks.py` & `openpathsampling-1.6.1/openpathsampling/beta/hooks.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/bias_function.py` & `openpathsampling-1.6.1/openpathsampling/bias_function.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/collectivevariable.py` & `openpathsampling-1.6.1/openpathsampling/collectivevariable.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import openpathsampling.netcdfplus.chaindict as cd
 from openpathsampling.integration_tools import md, error_if_no_mdtraj
 from openpathsampling.engines.openmm.tools import trajectory_to_mdtraj
 from openpathsampling.netcdfplus import WeakKeyCache, \
     ObjectJSON, create_to_dict, ObjectStore, PseudoAttribute
 
 from openpathsampling.deprecations import (has_deprecations, deprecate,
-                                           MSMBUILDER)
+                                           MSMBUILDER, PYEMMA)
 
 import sys
 if sys.version_info > (3, ):
     get_code = lambda func: func.__code__
 else:
     get_code = lambda func: func.func_code
 
@@ -668,14 +668,16 @@
             'topology': self.topology,
             'kwargs': self.kwargs,
             'cv_wrap_numpy_array': self.cv_wrap_numpy_array,
             'cv_scalarize_numpy_singletons': self.cv_scalarize_numpy_singletons
         }
 
 
+@has_deprecations
+@deprecate(PYEMMA)
 class PyEMMAFeaturizerCV(MSMBFeaturizerCV):
     """Make a CV from a function that takes mdtraj.trajectory as input.
 
     This is identical to :class:`CoordinateGeneratorCV` except that the
     function is called with an :class:`mdraj.Trajetory` object instead of the
     :class:`openpathsampling.Trajectory` one using ``fnc(traj.to_mdtraj(),
     **kwargs)``
```

### Comparing `openpathsampling-1.6.0/openpathsampling/collectivevariables/plumed_wrapper.py` & `openpathsampling-1.6.1/openpathsampling/collectivevariables/plumed_wrapper.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/deprecations.py` & `openpathsampling-1.6.1/openpathsampling/deprecations.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,22 @@
     problem=("MSMBuilder is no longer maintained. "
              + "MSMBFeaturizer is no longer officially supported."),
     remedy="Create a CoordinateFunctionCV based on MSMBuilderFeaturizers.",
     remove_version=(2, 0),
     deprecated_in=(1, 1, 0)
 )
 
+PYEMMA = Deprecation(
+    problem=("PyEMMA is no longer maintained. "
+             "PyEMMAFeaturizerCV is no longer officially supported."),
+    remedy="Create a CoordinateFunctionCV to represent the same function.",
+    remove_version=(2, 0),
+    deprecated_in=(1, 6, 1)
+)
+
 OPENMM_MDTRAJTOPOLOGY = Deprecation(
     problem=("openpathsampling.engines.openmm.topology.MDTrajTopology "
              "has been moved."),
     remedy=("Import MDTrajTopology from openpathsampling.engines instead."),
     remove_version=(2, 0),
     deprecated_in=(1, 5, 0)
 )
```

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/delayedinterrupt.py` & `openpathsampling-1.6.1/openpathsampling/engines/delayedinterrupt.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/dynamics_engine.py` & `openpathsampling-1.6.1/openpathsampling/engines/dynamics_engine.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/external_engine.py` & `openpathsampling-1.6.1/openpathsampling/engines/external_engine.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/external_snapshots/features/velocities.py` & `openpathsampling-1.6.1/openpathsampling/engines/external_snapshots/features/velocities.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/external_snapshots/snapshot.py` & `openpathsampling-1.6.1/openpathsampling/engines/external_snapshots/snapshot.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/features/base.py` & `openpathsampling-1.6.1/openpathsampling/engines/features/base.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/features/coordinates.py` & `openpathsampling-1.6.1/openpathsampling/engines/features/coordinates.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/features/engine.py` & `openpathsampling-1.6.1/openpathsampling/engines/features/engine.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/features/kinetics.py` & `openpathsampling-1.6.1/openpathsampling/engines/features/kinetics.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/features/numpydoctools.py` & `openpathsampling-1.6.1/openpathsampling/engines/features/numpydoctools.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/features/shared.py` & `openpathsampling-1.6.1/openpathsampling/engines/features/shared.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/features/statics.py` & `openpathsampling-1.6.1/openpathsampling/engines/features/statics.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/features/velocities.py` & `openpathsampling-1.6.1/openpathsampling/engines/features/velocities.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/gromacs/engine.py` & `openpathsampling-1.6.1/openpathsampling/engines/gromacs/engine.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/openmm/__init__.py` & `openpathsampling-1.6.1/openpathsampling/engines/openmm/__init__.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/openmm/engine.py` & `openpathsampling-1.6.1/openpathsampling/engines/openmm/engine.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/openmm/features/instantaneous_temperature.py` & `openpathsampling-1.6.1/openpathsampling/engines/openmm/features/instantaneous_temperature.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/openmm/features/masses.py` & `openpathsampling-1.6.1/openpathsampling/engines/openmm/features/masses.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/openmm/features/traj_quantities.py` & `openpathsampling-1.6.1/openpathsampling/engines/openmm/features/traj_quantities.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/openmm/snapshot.py` & `openpathsampling-1.6.1/openpathsampling/engines/openmm/snapshot.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/openmm/tools.py` & `openpathsampling-1.6.1/openpathsampling/engines/openmm/tools.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/snapshot.py` & `openpathsampling-1.6.1/openpathsampling/engines/snapshot.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/topology.py` & `openpathsampling-1.6.1/openpathsampling/engines/topology.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/toy/__init__.py` & `openpathsampling-1.6.1/openpathsampling/engines/toy/__init__.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/toy/engine.py` & `openpathsampling-1.6.1/openpathsampling/engines/toy/engine.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/toy/features/instantaneous_temperature.py` & `openpathsampling-1.6.1/openpathsampling/engines/toy/features/instantaneous_temperature.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/toy/integrators.py` & `openpathsampling-1.6.1/openpathsampling/engines/toy/integrators.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/toy/pes.py` & `openpathsampling-1.6.1/openpathsampling/engines/toy/pes.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/toy/snapshot.py` & `openpathsampling-1.6.1/openpathsampling/engines/toy/snapshot.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/toy/topology.py` & `openpathsampling-1.6.1/openpathsampling/engines/toy/topology.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/engines/trajectory.py` & `openpathsampling-1.6.1/openpathsampling/engines/trajectory.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/ensemble.py` & `openpathsampling-1.6.1/openpathsampling/ensemble.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/ensembles/visit_all_states.py` & `openpathsampling-1.6.1/openpathsampling/ensembles/visit_all_states.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/README.md` & `openpathsampling-1.6.1/openpathsampling/experimental/README.md`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/__init__.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/__init__.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/attribute_handlers.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/attribute_handlers.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/backend.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/backend.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/callable_codec.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/callable_codec.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/class_info.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/class_info.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/class_lookup.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/class_lookup.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/custom_json.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/custom_json.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/dict_serialization_helpers.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/dict_serialization_helpers.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/memory_backend.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/memory_backend.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/my_types.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/my_types.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/proxy.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/proxy.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/regressions/test_numpy_sfrs.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/regressions/test_numpy_sfrs.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/serialization.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/serialization.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/serialization_helpers.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/serialization_helpers.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/sql_backend.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/sql_backend.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/storable_functions.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/storable_functions.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/storage.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/storage.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/tags_table.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/tags_table.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_attribute_handlers.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_attribute_handlers.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_callable_codec.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_callable_codec.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_class_info.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_class_info.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_custom_json.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_custom_json.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_dict_serialization_helpers.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_dict_serialization_helpers.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_serialization.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_serialization.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_serialization_helpers.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_serialization_helpers.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_sql_backend.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_sql_backend.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_storable_function.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_storable_function.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_storable_function_integration.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_storable_function_integration.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_storage.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_storage.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_tags_table.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_tags_table.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_tools.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_tools.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_type_ident.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_type_ident.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/test_utils.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/test_utils.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/tools.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/tools.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/type_ident.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/type_ident.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/simstore/uuids.py` & `openpathsampling-1.6.1/openpathsampling/experimental/simstore/uuids.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/collective_variables.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/collective_variables.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/mdtraj_json.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/mdtraj_json.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/monkey_patches.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/monkey_patches.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/ops_storage.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/ops_storage.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/simtk_unit.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/simtk_unit.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/snapshots.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/snapshots.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/snapshots_table.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/snapshots_table.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/test_collective_variables.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/test_collective_variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 except ImportError:
     pass
 else:
     HAS_MDTRAJ = True
 
 
 class TestCollectiveVariable(object):
-    def setup(self):
+    def setup_method(self):
         self.cv = CollectiveVariable(lambda x: x.xyz[0][0])
         self.traj = make_1d_traj([1.0, 2.0, 3.0])
         ensemble = paths.LengthEnsemble(3)
         self.sample = paths.Sample(replica=0,
                                    trajectory=self.traj,
                                    ensemble=ensemble)
         self.snap = self.traj[0]
@@ -43,15 +43,15 @@
         inp = {'traj': self.traj, 'samp': self.sample}[inp_type]
         assert self.cv.is_scalar(inp) is False
 
 
 # TODO: It turns out that trajectories don't currently store their reversed
 # partners. This test won't work until that idea is implemented.
 # class TestReversibleStorableFunction(object):
-    # def setup(self):
+    # def setup_method(self):
         # self.func = ReversibleStorableFunction(
             # func=mock.MagicMock(return_value=3.0),
             # result_type='float'
         # )
         # self.traj = make_1d_traj([1.0, 2.0, 3.0])
         # _ = self.func(self.traj)  # evaluate once; it should be cached
         # # TODO: set up a mock storage, and store results in there
@@ -68,15 +68,15 @@
 
     # def test_get_storage(self):
         # # this will first clear the cache on self.func, and then try to load
         # pytest.skip()
 
 
 class TestCoordinateFunctionCV(object):
-    def setup(self):
+    def setup_method(self):
         # On using side_effect: https://stackoverflow.com/a/16162114
         mock_func = mock.MagicMock(side_effect=lambda s: s.xyz[0][0])
         self.func = CoordinateFunctionCV(mock_func)
         values = [1.0, 2.0, 3.0]
         traj = make_1d_traj(values)
         self.inputs = {'traj': traj.reversed, 'snap': traj[0].reversed}
         self.expected = {'traj': list(reversed(values)), 'snap': values[0]}
@@ -113,15 +113,15 @@
         self.func.func.assert_not_called()
         loop = {'snap': [inputs], 'traj': inputs}[inp_type]
         for item in loop:
             assert self.storage.backend.called_load[get_uuid(item)] == 1
 
 
 class TestMDTrajFunctionCV(object):
-    def setup(self):
+    def setup_method(self):
         if not HAS_MDTRAJ:
             pytest.skip("Unable to import MDTraj")
         pytest.importorskip('simtk.unit')
 
         self.mdt = md.load(data_filename("ala_small_traj.pdb"))
         top = MDTrajTopology(self.mdt.topology)
         self.traj = ops_omm.tools.trajectory_from_mdtraj(self.mdt)
```

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/test_mdtraj_json.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/test_mdtraj_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from ..simstore.custom_json import bytes_codec, numpy_codec, custom_json_factory
 from ..simstore.test_custom_json import CustomJSONCodingTest
 
 from openpathsampling.tests.test_helpers import data_filename
 
 class MDTrajCodingTest(CustomJSONCodingTest):
-    def setup(self):
+    def setup_method(self):
         if not HAS_MDTRAJ:
             pytest.skip()
 
         self.filename = data_filename('ala_small_traj.pdb')
 
     def test_default(self):
         # custom for handling numpy
@@ -32,31 +32,31 @@
     def test_round_trip(self):
         codecs = [numpy_codec, bytes_codec] + mdtraj_codecs
         encoder, decoder = custom_json_factory(codecs)
         self._test_round_trip(encoder, decoder)
 
 
 class TestTopologyCoding(MDTrajCodingTest):
-    def setup(self):
-        super(TestTopologyCoding, self).setup()
+    def setup_method(self):
+        super(TestTopologyCoding, self).setup_method()
         self.codec = top_codec
         top = md.load(self.filename).topology
         dataframe, bonds = top.to_dataframe()
         self.objs = [top]
         self.dcts = [{
             '__class__': 'Topology',
             '__module__': 'mdtraj.core.topology',
             'atoms': dataframe.to_json(),
             'bonds': bonds
         }]
 
 
 class TestTrajectoryCoding(MDTrajCodingTest):
-    def setup(self):
-        super(TestTrajectoryCoding, self).setup()
+    def setup_method(self):
+        super(TestTrajectoryCoding, self).setup_method()
         self.codec = traj_codec
         traj = md.load(self.filename)
         self.objs = [traj]
         self.dcts = [{
             '__class__': 'Trajectory',
             '__module__': 'mdtraj.core.trajectory',
             'xyz': traj.xyz,
```

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/test_monkey_patches.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/test_monkey_patches.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/test_pathsampling.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/test_pathsampling.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/test_regressions.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/test_regressions.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/test_simtk_unit.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/test_simtk_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ..storage import Storage
 
 from .simtk_unit import *
 
 from openpathsampling.integration_tools import HAS_SIMTK_UNIT, unit
 
 class TestSimtkUnitCodec(object):
-    def setup(self):
+    def setup_method(self):
         if not HAS_SIMTK_UNIT:
             pytest.skip("openmm.unit not installed")
         my_unit = unit.nanometer / unit.picosecond**2
         self.values = {
             'float': 1.0 * my_unit,
             'array': np.array([1.0, 2.0]) * my_unit,
         }
@@ -33,15 +33,15 @@
             np.testing.assert_array_equal(obj, deser)
         else:
             assert obj == deser
         assert ser == reser
 
 
 class TestSimtkQuantityHandler(object):
-    def setup(self):
+    def setup_method(self):
         pytest.importorskip('simtk.unit')
         self.handlers = {
             'float': SimtkQuantityHandler(
                 ('unit.nanometer/unit.picosecond**2', 'float')
             ),
             'array': SimtkQuantityHandler(
                 ('unit.nanometer', 'ndarray.float32(2,3)')
```

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/test_snapshot_integrations.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/test_snapshot_integrations.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/test_snapshots.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/test_snapshots.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/experimental/storage/test_snapshots_table.py` & `openpathsampling-1.6.1/openpathsampling/experimental/storage/test_snapshots_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         return [self.uuid_map[uuid] for uuid in uuids]
 
     def save(self, snapshot):
         self.saved.append(snapshot)
 
 
 class TestSnapshotsTable(object):
-    def setup(self):
+    def setup_method(self):
         self.engine_1 = make_engine()
         self.engine_2 = make_engine()
         snap_1_0 = toys.Snapshot(coordinates=np.array([0.0, 0.0]),
                                  velocities=np.array([0.0, 0.0]),
                                  engine=self.engine_1)
         snap_1_1 = toys.Snapshot(coordinates=np.array([1.0, 0.0]),
                                  velocities=np.array([1.0, 0.0]),
```

### Comparing `openpathsampling-1.6.0/openpathsampling/high_level/interface_set.py` & `openpathsampling-1.6.1/openpathsampling/high_level/interface_set.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/high_level/move_scheme.py` & `openpathsampling-1.6.1/openpathsampling/high_level/move_scheme.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/high_level/move_strategy.py` & `openpathsampling-1.6.1/openpathsampling/high_level/move_strategy.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/high_level/ms_outer_interface.py` & `openpathsampling-1.6.1/openpathsampling/high_level/ms_outer_interface.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/high_level/network.py` & `openpathsampling-1.6.1/openpathsampling/high_level/network.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/high_level/part_in_b_tps.py` & `openpathsampling-1.6.1/openpathsampling/high_level/part_in_b_tps.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/high_level/transition.py` & `openpathsampling-1.6.1/openpathsampling/high_level/transition.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/integration_tools.py` & `openpathsampling-1.6.1/openpathsampling/integration_tools.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/logging.conf` & `openpathsampling-1.6.1/openpathsampling/logging.conf`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/movechange.py` & `openpathsampling-1.6.1/openpathsampling/movechange.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/netcdfplus/__init__.py` & `openpathsampling-1.6.1/openpathsampling/netcdfplus/__init__.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/netcdfplus/attribute.py` & `openpathsampling-1.6.1/openpathsampling/netcdfplus/attribute.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,15 +226,15 @@
             with `c`. Either for class creation or for calling the function
 
         Notes
         -----
         This function is abstract and need _eval to be implemented to work.
         Problem is that there are two types of callable functions:
         1. direct functions: these can be called and give the wanted value
-           `c(object, \**kwargs)` would be the typical call
+           `c(object, **kwargs)` would be the typical call
         2. a generating function: a function the creates the callable object
            `c(**kwargs)(object)` is the typical call. This is usually used
            for classes. Create the instance and then use it.
 
         This function is very powerful, but need some explanation if you want
         the function to be stored alongside all other information in your
         storage. The problem is that a python function relies (usually) on
@@ -404,15 +404,15 @@
         return self.cv_callable(items, **self.kwargs)
 
 
 class GeneratorPseudoAttribute(CallablePseudoAttribute):
     """Turn a callable class or function generating a callable object into a CV
 
     The class instance will be called with objects. The instance itself
-    will be created using the given \**kwargs.
+    will be created using the given **kwargs.
     """
 
     def __init__(
             self,
             name,
             key_class,
             generator,
@@ -430,15 +430,15 @@
             a class where instances have a `__call__` attribute
         cv_requires_lists
         cv_wrap_numpy_array
         cv_scalarize_numpy_singletons
         kwargs
             additional arguments which should be given to `c` (for example, the
             atoms which define a specific distance/angle). Finally an instance
-            `instance = cls(\**kwargs)` is create when the CV is created and
+            `instance = cls(**kwargs)` is create when the CV is created and
             using the CV will call `instance(objects)`
 
         Notes
         -----
         Right now you cannot store user-defined classes. Only classes
         from external packages can be used.
         """
```

### Comparing `openpathsampling-1.6.0/openpathsampling/netcdfplus/base.py` & `openpathsampling-1.6.1/openpathsampling/netcdfplus/base.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/netcdfplus/cache.py` & `openpathsampling-1.6.1/openpathsampling/netcdfplus/cache.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/netcdfplus/chaindict.py` & `openpathsampling-1.6.1/openpathsampling/netcdfplus/chaindict.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/netcdfplus/dictify.py` & `openpathsampling-1.6.1/openpathsampling/netcdfplus/dictify.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/netcdfplus/netcdfplus.py` & `openpathsampling-1.6.1/openpathsampling/netcdfplus/netcdfplus.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/netcdfplus/proxy.py` & `openpathsampling-1.6.1/openpathsampling/netcdfplus/proxy.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/attribute.py` & `openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/attribute.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/dict.py` & `openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/dict.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/indexed.py` & `openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/indexed.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/named.py` & `openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/named.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/object.py` & `openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/object.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/value.py` & `openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/value.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/netcdfplus/stores/variable.py` & `openpathsampling-1.6.1/openpathsampling/netcdfplus/stores/variable.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/numerics/histogram.py` & `openpathsampling-1.6.1/openpathsampling/numerics/histogram.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/numerics/lookup_function.py` & `openpathsampling-1.6.1/openpathsampling/numerics/lookup_function.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/numerics/resampling_statistics.py` & `openpathsampling-1.6.1/openpathsampling/numerics/resampling_statistics.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/numerics/wham.py` & `openpathsampling-1.6.1/openpathsampling/numerics/wham.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/ops_logging.py` & `openpathsampling-1.6.1/openpathsampling/ops_logging.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/pathmover.py` & `openpathsampling-1.6.1/openpathsampling/pathmover.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/pathmover_inout.py` & `openpathsampling-1.6.1/openpathsampling/pathmover_inout.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/pathmovers/README.md` & `openpathsampling-1.6.1/openpathsampling/pathmovers/README.md`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/pathmovers/spring_shooting.py` & `openpathsampling-1.6.1/openpathsampling/pathmovers/spring_shooting.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/pathsimulators/bootstrap_init_conds.py` & `openpathsampling-1.6.1/openpathsampling/pathsimulators/bootstrap_init_conds.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/pathsimulators/direct_md.py` & `openpathsampling-1.6.1/openpathsampling/pathsimulators/direct_md.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/pathsimulators/path_sampling.py` & `openpathsampling-1.6.1/openpathsampling/pathsimulators/path_sampling.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/pathsimulators/path_simulator.py` & `openpathsampling-1.6.1/openpathsampling/pathsimulators/path_simulator.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/pathsimulators/reactive_flux.py` & `openpathsampling-1.6.1/openpathsampling/pathsimulators/reactive_flux.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/pathsimulators/shoot_snapshots.py` & `openpathsampling-1.6.1/openpathsampling/pathsimulators/shoot_snapshots.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/pathsimulators/sshooting_simulator.py` & `openpathsampling-1.6.1/openpathsampling/pathsimulators/sshooting_simulator.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/progress.py` & `openpathsampling-1.6.1/openpathsampling/progress.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/range_logic.py` & `openpathsampling-1.6.1/openpathsampling/range_logic.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/resources/debug_logging.conf` & `openpathsampling-1.6.1/openpathsampling/resources/debug_logging.conf`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/resources/logging.conf` & `openpathsampling-1.6.1/openpathsampling/resources/logging.conf`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/resources/vis.css` & `openpathsampling-1.6.1/openpathsampling/resources/vis.css`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/rng.py` & `openpathsampling-1.6.1/openpathsampling/rng.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/sample.py` & `openpathsampling-1.6.1/openpathsampling/sample.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/shooting.py` & `openpathsampling-1.6.1/openpathsampling/shooting.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/snapshot_modifier.py` & `openpathsampling-1.6.1/openpathsampling/snapshot_modifier.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/step_visualizer_2D.py` & `openpathsampling-1.6.1/openpathsampling/step_visualizer_2D.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/storage/distributed.py` & `openpathsampling-1.6.1/openpathsampling/storage/distributed.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/storage/storage.py` & `openpathsampling-1.6.1/openpathsampling/storage/storage.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/storage/stores/collectivevariable.py` & `openpathsampling-1.6.1/openpathsampling/storage/stores/collectivevariable.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/storage/stores/mcstep.py` & `openpathsampling-1.6.1/openpathsampling/storage/stores/mcstep.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/storage/stores/movechange.py` & `openpathsampling-1.6.1/openpathsampling/storage/stores/movechange.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/storage/stores/sample.py` & `openpathsampling-1.6.1/openpathsampling/storage/stores/sample.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/storage/stores/snapshot_base.py` & `openpathsampling-1.6.1/openpathsampling/storage/stores/snapshot_base.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/storage/stores/snapshot_feature.py` & `openpathsampling-1.6.1/openpathsampling/storage/stores/snapshot_feature.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/storage/stores/snapshot_value.py` & `openpathsampling-1.6.1/openpathsampling/storage/stores/snapshot_value.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/storage/stores/snapshot_wrapper.py` & `openpathsampling-1.6.1/openpathsampling/storage/stores/snapshot_wrapper.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/storage/stores/trajectory.py` & `openpathsampling-1.6.1/openpathsampling/storage/stores/trajectory.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/storage/util.py` & `openpathsampling-1.6.1/openpathsampling/storage/util.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/__init__.py` & `openpathsampling-1.6.1/openpathsampling/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/analysis/conftest.py` & `openpathsampling-1.6.1/openpathsampling/tests/analysis/conftest.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/analysis/utils/fixture_classes.py` & `openpathsampling-1.6.1/openpathsampling/tests/analysis/utils/fixture_classes.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/analysis/utils/mock_movers.py` & `openpathsampling-1.6.1/openpathsampling/tests/analysis/utils/mock_movers.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/analysis/utils/test_fixture_classes.py` & `openpathsampling-1.6.1/openpathsampling/tests/analysis/utils/test_fixture_classes.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/analysis/utils/test_mock_movers.py` & `openpathsampling-1.6.1/openpathsampling/tests/analysis/utils/test_mock_movers.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/external_engine/engine.c` & `openpathsampling-1.6.1/openpathsampling/tests/external_engine/engine.c`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/external_engine/microtest.py` & `openpathsampling-1.6.1/openpathsampling/tests/external_engine/microtest.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/pathsimulators/test_hooks.py` & `openpathsampling-1.6.1/openpathsampling/tests/pathsimulators/test_hooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 from __future__ import absolute_import
-from nose.tools import (assert_equal, assert_not_equal, assert_almost_equal,
-                        raises)
-from nose.plugins.skip import Skip, SkipTest
 
 import io
 import sys
 """
 import time
 import re
 if ((sys.version_info.major < 3)
@@ -101,76 +98,76 @@
 class TestPathSimulatorHook(object):
     # includes tests for attach_hook and run_hook
     def test_attach_hooks_class(self):
         hook = StupidHook()
         sim = TrivialPathSimulator(storage=None)
         sim.attach_hook(hook)
         for k in sim.hook_names:
-            assert_equal(len(sim.hooks[k]), 1)
+            assert len(sim.hooks[k]) == 1
 
     def test_attach_hooks_method(self):
         hook_instance = StupiderHook()
         sim = NoStepHookPathSimulator(storage=None)
         sim.attach_hook(hook_instance.hook_method, hook_for='extra_hook')
-        assert_not_equal(hook_instance.foo, "foo")
+        assert hook_instance.foo != "foo"
         sim.run(1)
-        assert_equal(hook_instance.foo, "foo")
+        assert hook_instance.foo == "foo"
 
     def test_trivial_simulation_hooks(self):
         sim = TrivialPathSimulator(storage=None)
         stupid = StupidHook()
         stupider = StupiderHook()
         sim.attach_hook(stupid)
         extra = lambda sim, hook_state: stupider.hook_method(sim,
                                                              hook_state,
                                                              "foo")
         sim.attach_hook(extra, hook_for='after_simulation')
         # before running, check that state is as expected
-        assert_equal(stupid.began_simulation, False)
-        assert_equal(stupid.finished_simulation, False)
-        assert_equal(stupid.began_steps, 0)
-        assert_equal(stupid.finished_steps, 0)
-        assert_not_equal(stupider.foo, "foo")
+        assert stupid.began_simulation is False
+        assert stupid.finished_simulation is False
+        assert stupid.began_steps == 0
+        assert stupid.finished_steps == 0
+        assert stupider.foo != "foo"
         # run
         sim.run(3)
         # check results
-        assert_equal(stupid.began_simulation, True)
-        assert_equal(stupid.finished_simulation, True)
-        assert_equal(stupid.began_steps, 3)
-        assert_equal(stupid.finished_steps, 3)
-        assert_equal(stupider.foo, "foo")
+        assert stupid.began_simulation is True
+        assert stupid.finished_simulation is True
+        assert stupid.began_steps == 3
+        assert stupid.finished_steps == 3
+        assert stupider.foo == "foo"
 
-    @raises(TypeError)
     def test_bad_extra_hook_method(self):
         sim = NoStepHookPathSimulator(storage=None)
         stupid = StupidHook()
-        sim.attach_hook(stupid)
+        with pytest.raises(TypeError):
+            sim.attach_hook(stupid)
 
-    @raises(TypeError)
     def test_bad_hook_name(self):
         sim = NoStepHookPathSimulator(storage=None)
         stupider = StupiderHook()
-        sim.attach_hook(stupider.hook_method, "blah")
+        with pytest.raises(TypeError):
+            sim.attach_hook(stupider.hook_method, "blah")
 
     def test_no_step_hook_simulation_hooks(self):
         sim = NoStepHookPathSimulator(storage=None)
         stupid = StupidHook()
         stupider = StupiderHook()
         sim.attach_hook(stupid.before_simulation,
                         hook_for='before_simulation')
         sim.attach_hook(stupider.hook_method, hook_for='extra_hook')
-        assert_equal(len(sim.hooks), len(sim.hook_names))
+        assert len(sim.hooks) == len(sim.hook_names)
         for hook in sim.hooks:
-            assert_equal(len(sim.hooks[hook]), 1)
+            assert len(sim.hooks[hook]) == 1
 
-        assert_equal(stupid.began_simulation, False)
-        assert_not_equal(stupider.foo, "foo")
+        assert stupid.began_simulation is False
+        assert stupider.foo != "foo"
         sim.run(1)
-        assert_equal(stupid.began_simulation, True)
-        assert_equal(stupider.foo, "foo")
+        assert stupid.began_simulation is True
+        assert stupider.foo == "foo"
 
 
 class TestSelfOrSimProperty(object):
     def setup_method(self):
         self.attr_name = "test_attr"
         self.simulation = MagicMock(test_attr="sim_attr")
         self.sans_attr_sans_sim = MagicMock(_test_attr=None, _simulation=None)
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_api.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_attribute.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_attribute.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """
 @author David W.H. Swenson
 """
 
 from .test_helpers import data_filename, assert_close_unit, make_1d_traj, md
 import pytest
 
-from nose.plugins.skip import SkipTest
-
 import openpathsampling.engines.openmm as peng
 from openpathsampling.netcdfplus import FunctionPseudoAttribute
 
 import openpathsampling as paths
 import os
 
 
 class TestFunctionPseudoAttribute(object):
     def setup_method(self):
         if not md:
-            raise SkipTest("mdtraj not installed")
+            pytest.skip("mdtraj not installed")
         self.mdtraj = md.load(data_filename("ala_small_traj.pdb"))
         pytest.importorskip("simtk.unit")
         self.traj_topology = peng.trajectory_from_mdtraj(self.mdtraj)
         self.traj_simple = peng.trajectory_from_mdtraj(
             self.mdtraj,
             simple_topology=True)
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_bias_function.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_bias_function.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import division
 from __future__ import print_function
 from __future__ import absolute_import
 from builtins import range
 from builtins import object
 from past.utils import old_div
-from nose.tools import (assert_equal, assert_not_equal, assert_almost_equal,
-                        raises, assert_in)
 
-from nose.plugins.skip import Skip, SkipTest
+import pytest
+import numpy.testing as npt
+
 from .test_helpers import true_func, assert_equal_array_array, make_1d_traj
 
 import numpy as np
 
 import openpathsampling as paths
 from openpathsampling.bias_function import *
 
@@ -82,15 +82,15 @@
             self.change_12 : old_div(0.2, 0.5),
             self.change_10 : old_div(1.0, 0.5),
             self.change_20 : old_div(1.0, 0.2),
             self.change_21 : old_div(0.5, 0.2)
         }
         for change in list(change_vals.keys()):
             test_val = min(1.0, change_vals[change])
-            assert_almost_equal(
+            npt.assert_almost_equal(
                 self.bias.probability_new_to_old(self.sample_set, change),
                 test_val
             )
 
     def test_bias_ensemble_old_to_new(self):
         # The n->o change is the numerator of the ratio.
 
@@ -102,15 +102,15 @@
             self.change_21 : old_div(0.2, 0.5),
             self.change_01 : old_div(1.0, 0.5),
             self.change_02 : old_div(1.0, 0.2),
             self.change_12 : old_div(0.5, 0.2)
         }
         for change in list(change_vals.keys()):
             test_val = min(1.0, change_vals[change])
-            assert_almost_equal(
+            npt.assert_almost_equal(
                 self.bias.probability_old_to_new(self.sample_set, change),
                 test_val
             )
 
     def test_combo_bias(self):
         #TODO: we don't support this yet, but we need to at some point
         # test what happens if you have more than one sample in the change
@@ -130,21 +130,21 @@
         # all upstream move
         move_210 = paths.SequentialMover([
             paths.EnsembleHopMover(ensembles[2], ensembles[1]),
             paths.EnsembleHopMover(ensembles[1], ensembles[0])
         ])
         change_210 = move_210.move(self.sample_set)
 
-        # assert_almost_equal(
+        # npt.assert_almost_equal(
             # self.bias.probability_old_to_new(change_210, self.sample_set), 1.0
         # )
-        # assert_almost_equal(
+        # npt.assert_almost_equal(
             # self.bias.probability_new_to_old(change_210, self.sample_set), 0.2
         # )
-        raise SkipTest
+        pytest.skip()
 
     def test_add_biases(self):
         # this is where we combine multiple biases into one
         ifacesA = self.ifacesA[:-1]
         xval2 = paths.FunctionCV(name="xB", f=lambda s : 0.5-s.xyz[0][0])
         ifacesB = paths.VolumeInterfaceSet(xval2, float("-inf"),
                                            [0.0, 0.1, 0.2])
@@ -176,20 +176,20 @@
                   ens_C[2]: 0.2}
 
         bias_A = BiasEnsembleTable.ratios_from_dictionary(dict_A)
         bias_B = BiasEnsembleTable.ratios_from_dictionary(dict_B)
         bias_C = BiasEnsembleTable.ratios_from_dictionary(dict_C)
         bias_AB = bias_A + bias_B
         # check the ensembles_to_ids
-        assert_equal(len(bias_AB.ensembles_to_ids), 7)
+        assert len(bias_AB.ensembles_to_ids) == 7
         for ens in ens_A:
-            assert_in(bias_AB.ensembles_to_ids[ens], [0, 1, 2])
+            assert bias_AB.ensembles_to_ids[ens] in [0, 1, 2]
         for ens in ens_B:
-            assert_in(bias_AB.ensembles_to_ids[ens], [3, 4, 5])
-        assert_equal(bias_AB.ensembles_to_ids[ms_outer], 6)
+            assert bias_AB.ensembles_to_ids[ens] in [3, 4, 5]
+        assert bias_AB.ensembles_to_ids[ms_outer] == 6
 
         # check values
         df_A = bias_A.dataframe
         df_B = bias_B.dataframe
         df_AB = bias_AB.dataframe
         col_A_msouter = bias_A.ensembles_to_ids[ms_outer]
         col_B_msouter = bias_B.ensembles_to_ids[ms_outer]
@@ -199,39 +199,39 @@
             idx_A = bias_A.ensembles_to_ids[ens1]
             idx_AB = bias_AB.ensembles_to_ids[ens1]
             for ens2 in ens_A:
                 col_A = bias_A.ensembles_to_ids[ens2]
                 col_AB = bias_AB.ensembles_to_ids[ens2]
                 val_A = df_A.loc[idx_A, col_A]
                 val_AB = df_AB.loc[idx_AB, col_AB]
-                assert_equal(val_A, val_AB)
+                assert val_A == val_AB
             for ens2 in ens_B:
                 col_AB = bias_AB.ensembles_to_ids[ens2]
-                assert_equal(np.isnan(df_AB.loc[idx_AB, col_AB]), True)
-            assert_equal(df_A.loc[idx_A, col_A_msouter],
-                         df_AB.loc[idx_AB, col_AB_msouter])
-            assert_equal(df_A.loc[col_A_msouter, idx_A],
-                         df_AB.loc[col_AB_msouter, idx_AB])
+                assert np.isnan(df_AB.loc[idx_AB, col_AB])
+            assert (df_A.loc[idx_A, col_A_msouter]
+                    == df_AB.loc[idx_AB, col_AB_msouter])
+            assert (df_A.loc[col_A_msouter, idx_A]
+                    == df_AB.loc[col_AB_msouter, idx_AB])
 
         for ens1 in ens_B:
             idx_B = bias_B.ensembles_to_ids[ens1]
             idx_AB = bias_AB.ensembles_to_ids[ens1]
             for ens2 in ens_B:
                 col_B = bias_B.ensembles_to_ids[ens2]
                 col_AB = bias_AB.ensembles_to_ids[ens2]
                 val_B = df_B.loc[idx_B, col_B]
                 val_AB = df_AB.loc[idx_AB, col_AB]
-                assert_equal(val_B, val_AB)
+                assert val_B == val_AB
             for ens2 in ens_A:
                 col_AB = bias_AB.ensembles_to_ids[ens2]
-                assert_equal(np.isnan(df_AB.loc[idx_AB, col_AB]), True)
-            assert_equal(df_B.loc[idx_B, col_B_msouter],
-                         df_AB.loc[idx_AB, col_AB_msouter])
-            assert_equal(df_B.loc[col_B_msouter, idx_B],
-                         df_AB.loc[col_AB_msouter, idx_AB])
+                assert np.isnan(df_AB.loc[idx_AB, col_AB])
+            assert (df_B.loc[idx_B, col_B_msouter]
+                    == df_AB.loc[idx_AB, col_AB_msouter])
+            assert (df_B.loc[col_B_msouter, idx_B]
+                    == df_AB.loc[col_AB_msouter, idx_AB])
 
         # just to make sure no errors raise when there are NaNs in table
         bias_ABC = bias_A + bias_B + bias_C
 
 class TestSRTISBiasFromNetwork(object):
     def setup_method(self):
         paths.InterfaceSet._reset()
@@ -261,44 +261,44 @@
         network.sampling_transitions[0].tcp = self.tcp_A
         bias = paths.SRTISBiasFromNetwork(network)
         transition = list(network.transitions.values())[0]  # only one
 
         # check reciprocal of symmetric partners
         for i in range(4):
             for j in range(i, 4):
-                assert_equal(bias.dataframe.loc[i, j],
-                             old_div(1.0, bias.dataframe.loc[j, i]))
+                assert (bias.dataframe.loc[i, j]
+                        == old_div(1.0, bias.dataframe.loc[j, i]))
 
         for i in range(len(transition.ensembles) - 1):
             ens_to = transition.ensembles[i]
             ens_from = transition.ensembles[i + 1]
-            assert_equal(bias.bias_value(ens_from, ens_to), 0.5)
+            assert bias.bias_value(ens_from, ens_to) == 0.5
 
         for i in range(len(transition.ensembles) - 2):
             ens_to = transition.ensembles[i]
             ens_from = transition.ensembles[i + 2]
-            assert_equal(bias.bias_value(ens_from, ens_to), 0.25)
+            assert bias.bias_value(ens_from, ens_to) == 0.25
 
-    @raises(RuntimeError)
     def test_fail_without_tcp(self):
         network = paths.MISTISNetwork([
             (self.stateA, self.ifacesA, self.stateB)
         ])
-        bias = paths.SRTISBiasFromNetwork(network)
+        with pytest.raises(RuntimeError):
+            bias = paths.SRTISBiasFromNetwork(network)
 
-    @raises(RuntimeError)
     def test_fail_without_lambdas(self):
         fake_ifaceA = paths.InterfaceSet(cv=self.ifacesA.cv,
                                          volumes=self.ifacesA.volumes,
                                          direction=self.ifacesA.direction)
         network = paths.MISTISNetwork([
             (self.stateA, fake_ifaceA, self.stateB)
         ])
         network.sampling_transitions[0].tcp = self.tcp_A
-        bias = paths.SRTISBiasFromNetwork(network)
+        with pytest.raises(RuntimeError):
+            bias = paths.SRTISBiasFromNetwork(network)
 
     def test_bias_from_ms_network(self):
         ms_outer = paths.MSOuterTISInterface.from_lambdas(
             {self.ifacesA : -0.1, self.ifacesB : 0.1}
         )
         network = paths.MISTISNetwork(
             [(self.stateA, self.ifacesA, self.stateB),
@@ -329,31 +329,29 @@
                         bias.dataframe.loc[i, j],
                         old_div(1.0, bias.dataframe.loc[j, i])
                     )
 
         for i in range(len(transition_AB.ensembles) - 1):
             ens_to = transition_AB.ensembles[i]
             ens_from = transition_AB.ensembles[i + 1]
-            assert_almost_equal(bias.bias_value(ens_from, ens_to), 0.5)
+            npt.assert_almost_equal(bias.bias_value(ens_from, ens_to), 0.5)
 
         for i in range(len(transition_BA.ensembles) - 1):
             ens_to = transition_BA.ensembles[i]
             ens_from = transition_BA.ensembles[i + 1]
-            assert_almost_equal(bias.bias_value(ens_from, ens_to), 0.2)
+            npt.assert_almost_equal(bias.bias_value(ens_from, ens_to), 0.2)
 
         for ensA in transition_AB.ensembles:
             for ensB in transition_BA.ensembles:
-                assert_equal(np.isnan(bias.bias_value(ensA, ensB)), True)
-                assert_equal(np.isnan(bias.bias_value(ensB, ensA)), True)
+                assert np.isnan(bias.bias_value(ensA, ensB))
+                assert np.isnan(bias.bias_value(ensB, ensA))
 
-        assert_almost_equal(bias.bias_value(transition_BA.ensembles[-1],
-                                            network.ms_outers[0]),
+        npt.assert_almost_equal(bias.bias_value(transition_BA.ensembles[-1],
+                                                network.ms_outers[0]),
                             old_div(5.0, 2))
-        assert_almost_equal(bias.bias_value(transition_AB.ensembles[-1],
-                                            network.ms_outers[0]),
+        npt.assert_almost_equal(bias.bias_value(transition_AB.ensembles[-1],
+                                                network.ms_outers[0]),
                             old_div(2.0, 2))
 
 
 
 
-
-        raise SkipTest
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_channel_analysis.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_channel_analysis.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import absolute_import
 from builtins import object
-from nose.tools import (assert_equal, assert_not_equal, raises,
-                        assert_almost_equal)
-from nose.plugins.skip import SkipTest
+import pytest
+
 from numpy.testing import assert_array_almost_equal
 from .test_helpers import make_1d_traj, data_filename, assert_items_equal
 
 import openpathsampling as paths
 import numpy as np
 import random
 import os
@@ -81,178 +80,182 @@
         storage.save(self.incr_1[0])  # template snapshot
         storage.tag['analyzer'] = analyzer
         storage.sync()
         storage.close()
 
         new_store = paths.Storage(data_filename('test.nc'), 'r')
         reloaded = storage.tag['analyzer']
-        assert_equal(reloaded._results, self.toy_results)
+        assert reloaded._results == self.toy_results
 
         if os.path.isfile(data_filename('test.nc')):
             os.remove(data_filename('test.nc'))
 
     def test_analyze_incr_decr(self):
         steps = [
             paths.MCStep(mccycle=0, active=self.incr_1),
             paths.MCStep(mccycle=1, active=self.decr_1)
         ]
         results = paths.ChannelAnalysis(steps, self.channels)
-        assert_equal(results._results,
-                     {'incr': [(0,1)], 'decr': [(1,2)], None: []})
+        expected = {'incr': [(0,1)], 'decr': [(1,2)], None: []}
+        assert results._results == expected
 
     def test_analyze_incr_incr(self):
         steps = [
             paths.MCStep(mccycle=0, active=self.incr_1),
             paths.MCStep(mccycle=1, active=self.incr_2)
         ]
         results = paths.ChannelAnalysis(steps, self.channels)
-        assert_equal(results._results,
-                     {'incr': [(0,2)], 'decr': [], None: []})
+        assert results._results == {'incr': [(0,2)], 'decr': [], None: []}
 
     def test_analyze_incr_both_decr(self):
         steps = [
             paths.MCStep(mccycle=0, active=self.incr_1),
             paths.MCStep(mccycle=1, active=self.both_1),
             paths.MCStep(mccycle=2, active=self.both_2),
             paths.MCStep(mccycle=3, active=self.decr_1)
         ]
         results = paths.ChannelAnalysis(steps, self.channels)
-        assert_equal(results._results,
-                     {'incr': [(0,3)], 'decr': [(1,4)], None: []})
+        expected = {'incr': [(0,3)], 'decr': [(1,4)], None: []}
+        assert results._results == expected
 
     def test_analyze_incr_both_incr(self):
         steps = [
             paths.MCStep(mccycle=0, active=self.incr_1),
             paths.MCStep(mccycle=1, active=self.both_1),
             paths.MCStep(mccycle=2, active=self.incr_2)
         ]
         results = paths.ChannelAnalysis(steps, self.channels)
-        assert_equal(results._results,
-                     {'incr': [(0,3)], 'decr': [(1,2)], None: []})
+        expected = {'incr': [(0,3)], 'decr': [(1,2)], None: []}
+        assert results._results == expected
 
     def test_analyze_incr_same_decr(self):
         steps = [
             paths.MCStep(mccycle=0, active=self.incr_1),
             paths.MCStep(mccycle=1, active=self.incr_1),
             paths.MCStep(mccycle=2, active=self.incr_2)
         ]
         results = paths.ChannelAnalysis(steps, self.channels)
-        assert_equal(results._results,
-                     {'incr': [(0,3)], 'decr': [], None: []})
+        expected = {'incr': [(0,3)], 'decr': [], None: []}
+        assert results._results == expected
 
     def test_analyze_incr_none_incr(self):
         steps = [
             paths.MCStep(mccycle=0, active=self.incr_1),
             paths.MCStep(mccycle=1, active=self.none_1),
             paths.MCStep(mccycle=2, active=self.incr_2)
         ]
         results = paths.ChannelAnalysis(steps, self.channels)
-        assert_equal(results._results,
-                     {'incr': [(0,1), (2,3)], 'decr': [], None: [(1,2)]})
+        expected = {'incr': [(0,1), (2,3)], 'decr': [], None: [(1,2)]}
+        assert results._results == expected
 
     def test_analyze_incr_none_decr(self):
         steps = [
             paths.MCStep(mccycle=0, active=self.incr_1),
             paths.MCStep(mccycle=1, active=self.none_1),
             paths.MCStep(mccycle=2, active=self.decr_1)
         ]
         results = paths.ChannelAnalysis(steps, self.channels)
-        assert_equal(results._results,
-                     {'incr': [(0,1)], 'decr': [(2,3)], None: [(1,2)]})
+        expected = {'incr': [(0,1)], 'decr': [(2,3)], None: [(1,2)]}
+        assert results._results == expected
 
     def test_expand_results(self):
         expanded = paths.ChannelAnalysis._expand_results(self.toy_results)
-        assert_equal(expanded, self.toy_expanded_results)
+        assert expanded == self.toy_expanded_results
 
     def test_labels_by_step_newest(self):
         test_set = self.toy_expanded_results
         relabeled = paths.ChannelAnalysis._labels_by_step_newest(test_set)
-        assert_equal(relabeled, [(0, 3, self.set_a), (3, 7, self.set_b),
-                                 (7, 8, self.set_c), (8, 10, self.set_a)])
+        expected = [(0, 3, self.set_a), (3, 7, self.set_b),
+                    (7, 8, self.set_c), (8, 10, self.set_a)]
+        assert relabeled == expected
 
         test_set = self.expanded_results_simultaneous_ending
         relabeled = paths.ChannelAnalysis._labels_by_step_newest(test_set)
-        assert_equal(relabeled, [(0, 3, self.set_a), (3, 7, self.set_b),
-                                 (7, 8, self.set_c), (8, 10, self.set_a)])
+        expected =  [(0, 3, self.set_a), (3, 7, self.set_b),
+                     (7, 8, self.set_c), (8, 10, self.set_a)]
+        assert relabeled == expected
 
     def test_labels_by_step_oldest(self):
         test_set = self.toy_expanded_results
         relabeled = paths.ChannelAnalysis._labels_by_step_oldest(test_set)
-        assert_equal(relabeled, [(0, 5, self.set_a), (5, 9, self.set_b),
-                                 (9, 10, self.set_a)])
+        expected = [(0, 5, self.set_a), (5, 9, self.set_b),
+                    (9, 10, self.set_a)]
+        assert relabeled == expected
 
         test_set = self.expanded_results_simultaneous_ending
         relabeled = paths.ChannelAnalysis._labels_by_step_oldest(test_set)
-        assert_equal(relabeled, [(0, 5, self.set_a), (5, 9, self.set_b),
-                                 (9, 10, self.set_c)])
+        expected = [(0, 5, self.set_a), (5, 9, self.set_b),
+                    (9, 10, self.set_c)]
+        assert relabeled == expected
 
         test_set = self.expanded_oldest_skips_internal
         relabeled = paths.ChannelAnalysis._labels_by_step_oldest(test_set)
-        assert_equal(relabeled, [(0, 5, self.set_a), (5, 9, self.set_b),
-                                 (9, 10, self.set_a), (10, 11, self.set_b)])
+        expected = [(0, 5, self.set_a), (5, 9, self.set_b),
+                    (9, 10, self.set_a), (10, 11, self.set_b)]
+        assert relabeled == expected
 
 
     def test_labels_by_step_multiple(self):
         test_set = self.toy_expanded_results
         relabeled = paths.ChannelAnalysis._labels_by_step_multiple(test_set)
-        assert_equal(relabeled,
-                     [(0, 3, self.set_a),
-                      (3, 5, self.set_a | self.set_b),
-                      (5, 7, self.set_b),
-                      (7, 8, self.set_b | self.set_c),
-                      (8, 9, self.set_b | self.set_c | self.set_a),
-                      (9, 10, self.set_a)])
+        expected = [(0, 3, self.set_a),
+                    (3, 5, self.set_a | self.set_b),
+                    (5, 7, self.set_b),
+                    (7, 8, self.set_b | self.set_c),
+                    (8, 9, self.set_b | self.set_c | self.set_a),
+                    (9, 10, self.set_a)]
+        assert relabeled == expected
 
     def test_empty(self):
         obj = paths.ChannelAnalysis(steps=None, channels=self.channels)
         empty_results = {c: [] for c in list(self.channels.keys()) + [None]}
-        assert_equal(obj._results, empty_results)
+        assert obj._results == empty_results
 
     def test_treat_multiples(self):
         obj = paths.ChannelAnalysis(steps=None, channels=self.channels)
-        assert_equal(obj.treat_multiples, 'all')
+        assert obj.treat_multiples == 'all'
         obj.treat_multiples = 'oldest'
-        assert_equal(obj.treat_multiples, 'oldest')
+        assert obj.treat_multiples == 'oldest'
         obj.treat_multiples = 'newest'
-        assert_equal(obj.treat_multiples, 'newest')
+        assert obj.treat_multiples == 'newest'
         obj.treat_multiples = 'multiple'
-        assert_equal(obj.treat_multiples, 'multiple')
+        assert obj.treat_multiples == 'multiple'
         obj.treat_multiples = 'all'
-        assert_equal(obj.treat_multiples, 'all')
+        assert obj.treat_multiples == 'all'
 
-    @raises(ValueError)
     def test_bad_treat_multiples(self):
         obj = paths.ChannelAnalysis(steps=None, channels=self.channels)
-        assert_equal(obj.treat_multiples, 'all')
-        obj.treat_multiples = 'bad_string'
+        assert obj.treat_multiples == 'all'
+        with pytest.raises(ValueError):
+            obj.treat_multiples = 'bad_string'
 
     def test_labels_as_sets_sort_function(self):
         sort_key = paths.ChannelAnalysis._labels_as_sets_sort_function
 
         inp_list = [self.set_b, self.set_c, self.set_a]
         sorted_set_list = sorted(inp_list, key=sort_key)
         sorted_labels = [paths.ChannelAnalysis.label_to_string(e)
                          for e in sorted_set_list]
-        assert_equal(sorted_labels, ['a', 'b', 'c'])
+        assert sorted_labels == ['a', 'b', 'c']
 
         inp_list = [self.set_a, self.set_a | self.set_b, self.set_b,
                     self.set_c | self.set_b,
                     self.set_a | self.set_b | self.set_c]
         sorted_set_list = sorted(inp_list, key=sort_key)
         sorted_labels = [paths.ChannelAnalysis.label_to_string(e)
                          for e in sorted_set_list]
-        assert_equal(sorted_labels, ['a', 'b', 'a,b', 'b,c', 'a,b,c'])
+        assert sorted_labels == ['a', 'b', 'a,b', 'b,c', 'a,b,c']
 
     def test_labels_sort_function_with_none(self):
         sort_key = paths.ChannelAnalysis._labels_as_sets_sort_function
         inp_list = [self.set_b, self.set_a, set([None])]
         sorted_set_list = sorted(inp_list, key=sort_key)
         sorted_labels = [paths.ChannelAnalysis.label_to_string(e)
                          for e in sorted_set_list]
-        assert_equal(sorted_labels, ['None', 'a', 'b'])
+        assert sorted_labels == ['None', 'a', 'b']
 
     def test_switching(self):
         analysis = paths.ChannelAnalysis(steps=None, channels=self.channels)
         analysis._results = self.toy_results
         #nan = float('nan')
         nan = 0  # self transitions are 0
 
@@ -295,91 +298,90 @@
 
     def test_residence_times(self):
         analysis = paths.ChannelAnalysis(steps=None, channels=self.channels)
         analysis._results = self.toy_results
 
         analysis.treat_multiples = 'newest'
         residence_times = analysis.residence_times
-        assert_equal(residence_times, {'a': [3, 2], 'b': [4], 'c': [1]})
+        assert residence_times == {'a': [3, 2], 'b': [4], 'c': [1]}
 
         analysis.treat_multiples = 'oldest'
         residence_times = analysis.residence_times
-        assert_equal(residence_times, {'a': [5, 1], 'b': [4]})
+        assert residence_times == {'a': [5, 1], 'b': [4]}
 
         analysis.treat_multiples = 'all'
         residence_times = analysis.residence_times
-        assert_equal(residence_times, {'a': [5, 2], 'b': [6], 'c': [2]})
+        assert residence_times == {'a': [5, 2], 'b': [6], 'c': [2]}
 
         analysis.treat_multiples = 'multiple'
         residence_times = analysis.residence_times
-        assert_equal(residence_times, {'a': [3, 1], 'b': [2], 'a,b': [2],
-                                       'b,c': [1], 'a,b,c': [1]})
+        assert residence_times == {
+            'a': [3, 1], 'b': [2], 'a,b': [2], 'b,c': [1], 'a,b,c': [1]
+        }
 
     def test_residence_times_with_none(self):
         analysis = paths.ChannelAnalysis(steps=None, channels=self.channels)
         analysis._results = self.results_with_none
 
         residence_times = analysis.residence_times
-        assert_equal(residence_times,
-                     {'a': [2, 3], 'b': [2, 1], 'None': [3]})
+        assert residence_times == {'a': [2, 3], 'b': [2, 1], 'None': [3]}
 
     def test_total_time(self):
         analysis = paths.ChannelAnalysis(steps=None, channels=self.channels)
         analysis._results = self.toy_results
 
         analysis.treat_multiples = 'newest'
         total_time = analysis.total_time
-        assert_equal(total_time, {'a': 5, 'b': 4, 'c': 1})
+        assert total_time == {'a': 5, 'b': 4, 'c': 1}
 
         analysis.treat_multiples = 'oldest'
         total_time = analysis.total_time
-        assert_equal(total_time, {'a': 6, 'b': 4})
-        assert_equal(total_time['c'], 0)
+        assert total_time == {'a': 6, 'b': 4}
+        assert total_time['c'] == 0
 
         analysis.treat_multiples = 'all'
         total_time = analysis.total_time
-        assert_equal(total_time, {'a': 7, 'b': 6, 'c': 2})
+        assert total_time == {'a': 7, 'b': 6, 'c': 2}
 
         analysis.treat_multiples = 'multiple'
         total_time = analysis.total_time
-        assert_equal(total_time, {'a': 4, 'b': 2, 'a,b': 2, 'b,c': 1,
-                                  'a,b,c': 1})
+        assert total_time == {'a': 4, 'b': 2, 'a,b': 2, 'b,c': 1, 'a,b,c': 1}
 
     def test_total_time_with_none(self):
         analysis = paths.ChannelAnalysis(steps=None, channels=self.channels)
         analysis._results = self.results_with_none
 
         total_time = analysis.total_time
-        assert_equal(total_time, {'a': 5, 'b': 3, 'None': 3})
+        assert total_time == {'a': 5, 'b': 3, 'None': 3}
 
 
     def test_status(self):
         analysis = paths.ChannelAnalysis(steps=None, channels=self.channels)
         analysis._results = self.toy_results
 
         analysis.treat_multiples = 'newest'
-        assert_equal(analysis.status(4), 'b')
-        assert_equal(analysis.status(8), 'a')
+        assert analysis.status(4) == 'b'
+        assert analysis.status(8) == 'a'
 
         analysis.treat_multiples = 'oldest'
-        assert_equal(analysis.status(4), 'a')
-        assert_equal(analysis.status(8), 'b')
+        assert analysis.status(4) == 'a'
+        assert analysis.status(8) == 'b'
 
         analysis.treat_multiples = 'multiple'
-        assert_equal(analysis.status(4), 'a,b')
-        assert_equal(analysis.status(8), 'a,b,c')
+        assert analysis.status(4) == 'a,b'
+        assert analysis.status(8) == 'a,b,c'
 
         analysis.treat_multiples = 'all'
-        assert_equal(analysis.status(4), 'a,b')
-        assert_equal(analysis.status(8), 'a,b,c')
+        assert analysis.status(4) == 'a,b'
+        assert analysis.status(8) == 'a,b,c'
 
     def test_status_with_none(self):
         analysis = paths.ChannelAnalysis(steps=None, channels=self.channels)
         analysis._results = self.results_with_none
-        assert_equal(analysis.status(4), 'None')
+        assert analysis.status(4) == 'None'
 
-    @raises(RuntimeError)
     def test_bad_status_number(self):
         analysis = paths.ChannelAnalysis(steps=None, channels=self.channels)
         analysis._results = self.toy_results
 
-        analysis.status(10)
+        with pytest.raises(RuntimeError):
+            analysis.status(10)
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_collectivevariable.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_collectivevariable.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from __future__ import absolute_import
 
 from builtins import zip
 from builtins import object
 from .test_helpers import data_filename, assert_close_unit, md
 
 import pytest
-from nose.plugins.skip import SkipTest
 
 import numpy as np
 
 import openpathsampling.collectivevariable as op
 import openpathsampling.engines.openmm as peng
 from openpathsampling.netcdfplus import NetCDFPlus
 
@@ -27,15 +26,15 @@
 from openpathsampling.tests.test_helpers import make_1d_traj
 import os
 
 
 class TestFunctionCV(object):
     def setup_method(self):
         if not md:
-            raise SkipTest("mdtraj not installed")
+            pytest.skip("mdtraj not installed")
         self.mdtraj = md.load(data_filename("ala_small_traj.pdb"))
         _ = pytest.importorskip('simtk.unit')
         self.traj_topology = peng.trajectory_from_mdtraj(self.mdtraj)
         self.traj_simple = peng.trajectory_from_mdtraj(
             self.mdtraj,
             simple_topology=True)
 
@@ -83,15 +82,15 @@
             md_dihed.reshape(md_dihed.shape[:-1]),
             my_dihed, rtol=10 ** -6, atol=10 ** -10)
 
     def test_atom_pair_featurizer(self):
         """ Create an atom pair collectivevariable using MSMSBuilder3 """
 
         if not has_msmbuilder:
-            raise SkipTest("MSMBuilder not installed")
+            pytest.skip("MSMBuilder not installed")
         atom_pairs = [[0, 1], [10, 14]]
         atom_pair_op = op.MSMBFeaturizerCV(
             "atom_pairs",
             AtomPairsFeaturizer,
             topology=self.topology,
             pair_indices=atom_pairs)
 
@@ -101,15 +100,15 @@
 
         np.testing.assert_allclose(md_distances, my_distances, rtol=10 ** -6,
                                    atol=10 ** -10)
 
     def test_return_parameters_from_template(self):
 
         if not has_msmbuilder:
-            raise SkipTest("MSMBuilder not installed")
+            pytest.skip("MSMBuilder not installed")
         atom_pairs = [[0, 1], [10, 14]]
         atom_pair_op = op.MSMBFeaturizerCV(
             "atom_pairs",
             AtomPairsFeaturizer,
             topology=self.topology,
             pair_indices=atom_pairs)
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_data/ala_small_traj.pdb` & `openpathsampling-1.6.1/openpathsampling/tests/test_data/ala_small_traj.pdb`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_data/apis/ops1x0_api.txt` & `openpathsampling-1.6.1/openpathsampling/tests/test_data/apis/ops1x0_api.txt`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_data/gromacs_engine/conf.gro` & `openpathsampling-1.6.1/openpathsampling/tests/test_data/gromacs_engine/conf.gro`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_data/gromacs_engine/md.mdp` & `openpathsampling-1.6.1/openpathsampling/tests/test_data/gromacs_engine/md.mdp`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_data/gromacs_engine/project_trr/0000000.trr` & `openpathsampling-1.6.1/openpathsampling/tests/test_data/gromacs_engine/project_trr/0000000.trr`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_data/gromacs_engine/project_trr/0000099.trr` & `openpathsampling-1.6.1/openpathsampling/tests/test_data/gromacs_engine/project_trr/0000099.trr`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_data/gromacs_engine/topol.top` & `openpathsampling-1.6.1/openpathsampling/tests/test_data/gromacs_engine/topol.top`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_data/gromacs_engine/traj.trr` & `openpathsampling-1.6.1/openpathsampling/tests/test_data/gromacs_engine/traj.trr`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_data/plumed_wrapper/AD_initial_frame.pdb` & `openpathsampling-1.6.1/openpathsampling/tests/test_data/plumed_wrapper/AD_initial_frame.pdb`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_data/plumed_wrapper/AD_plumed_rmsd.pdb` & `openpathsampling-1.6.1/openpathsampling/tests/test_data/plumed_wrapper/AD_plumed_rmsd.pdb`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_data/reduce_box_vects/dna.gro` & `openpathsampling-1.6.1/openpathsampling/tests/test_data/reduce_box_vects/dna.gro`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_data/reduce_box_vects/dna.trr` & `openpathsampling-1.6.1/openpathsampling/tests/test_data/reduce_box_vects/dna.trr`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_deprecations.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_deprecations.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_dynamicsengine.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_dynamicsengine.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import absolute_import
 from builtins import object
 import pytest
 import openpathsampling as paths
 
-from nose.tools import (assert_equal, assert_not_equal, raises, assert_true)
-from nose.plugins.skip import SkipTest
 from .test_helpers import make_1d_traj, raises_with_message_like
 
 try:
     from unittest import mock
 except ImportError:
     import mock
 
@@ -54,24 +52,24 @@
             snapshot_dimensions=snapshot_dimensions
         )
         self.descriptor = descriptor
         self.engine = paths.engines.DynamicsEngine(options, descriptor)
         self.stupid = StupidEngine(options, descriptor)
 
     def test_getattr_from_options(self):
-        assert_equal(self.stupid.random_option, True)
+        assert self.stupid.random_option is True
 
     def test_getattr_property_fails(self):
         # py2: "'newobject' object has no attribute 'b'"
         # py3: "'object' object has no attribute 'b'"
         error_string_end = "object' object has no attribute 'b'"
         try:
             self.stupid.bad_property
         except AttributeError as e:
-            assert_true(str(e).endswith(error_string_end))
+            assert str(e).endswith(error_string_end)
 
         else:
             raise AssertionError("Did not raise appropriate AttributeError")
 
 
     @raises_with_message_like(AttributeError,
                               "Unknown problem occurred in property")
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_ensemble.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_ensemble.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from __future__ import absolute_import
 from builtins import zip
 from builtins import map
 from builtins import str
 from builtins import range
 from builtins import object
-from nose.tools import (assert_equal, assert_not_equal, raises, assert_true,
-                        assert_false)
-from nose.plugins.skip import SkipTest
+import pytest
 from .test_helpers import (CallIdentity, prepend_exception_message,
                           make_1d_traj, raises_with_message_like,
                           CalvinistDynamics)
 
 import openpathsampling as paths
 import openpathsampling.engines.openmm as peng
 from openpathsampling.ensemble import *
@@ -41,17 +39,17 @@
     for i in range(length - (len(traj)+start)):
         outtraj.append(traj[-1])
     return outtraj
 
 def test_wrap_traj():
     """Testing wrap_traj (oh gods, the meta! a test for a test function!)"""
     intraj = [1, 2, 3]
-    assert_equal(wrap_traj(intraj, 3, 6), [1, 1, 1, 1, 2, 3])
-    assert_equal(wrap_traj(intraj, 3, 8), [1, 1, 1, 1, 2, 3, 3, 3])
-    assert_equal(wrap_traj(intraj, 3, 8)[slice(3, 6)], intraj)
+    assert wrap_traj(intraj, 3, 6) == [1, 1, 1, 1, 2, 3]
+    assert wrap_traj(intraj, 3, 8) == [1, 1, 1, 1, 2, 3, 3, 3]
+    assert wrap_traj(intraj, 3, 8)[slice(3, 6)] == intraj
 
 def build_trajdict(trajtypes, lower, upper):
     upperadddict = {'a' : 'in', 'b' : 'out', 'c' : 'cross', 'o' : 'hit'}
     loweradddict = {'a' : 'out', 'b' : 'in', 'c' : 'in', 'o' : 'hit'}
     lowersubdict = {'a' : 'in', 'b' : 'out', 'c' : 'cross', 'o' : 'hit'}
     uppersubdict = {'a' : 'out', 'b' : 'in', 'c' : 'in', 'o' : 'hit'}
     adjustdict = {'a' : (lambda x: -0.05*x), 'b' : (lambda x: 0.05*x),
@@ -139,15 +137,15 @@
             elif to_append != res[-1]:
                 res.append(to_append)
     return res
 
 class EnsembleTest(object):
     def _single_test(self, ensemble_fcn, traj, res, failmsg):
         try:
-            assert_equal(ensemble_fcn(traj), res)
+            assert ensemble_fcn(traj) == res
         except AssertionError as e:
             prepend_exception_message(e, failmsg)
             raise
 
     def _test_everything(self, test_fcn, non_default=[], default=False):
         """
         Runs tests using *all* the trajectory test suite. This is the
@@ -228,22 +226,22 @@
         self._test_everything(self.leaveX.strict_can_append, default=True)
 
     def test_strict_can_prepend(self):
         self._test_everything(self.leaveX.strict_can_prepend, default=True)
 
     def test_leaveX_0(self):
         """PartOutXEnsemble treatment of zero-length trajectory"""
-        assert_equal(self.leaveX(paths.Trajectory([])), False)
-        assert_equal(self.leaveX.can_append(paths.Trajectory([])), True)
-        assert_equal(self.leaveX.can_prepend(paths.Trajectory([])), True)
+        assert self.leaveX(paths.Trajectory([])) is False
+        assert self.leaveX.can_append(paths.Trajectory([])) is True
+        assert self.leaveX.can_prepend(paths.Trajectory([])) is True
 
     def test_leaveX_str(self):
         volstr = "{x|Id(x) in [0.1, 0.5]}"
-        assert_equal(self.leaveX.__str__(),
-                     "exists t such that x[t] in (not "+volstr+")")
+        expected_str = "exists t such that x[t] in (not "+volstr+")"
+        assert self.leaveX.__str__() == expected_str
 
 class TestAllInXEnsemble(EnsembleTest):
     def setup_method(self):
         self.inX = AllInXEnsemble(vol1)
 
     def test_inX(self):
         """AllInXEnsemble passes the trajectory test suite"""
@@ -292,22 +290,21 @@
                 res = True
             failmsg = "Failure in "+test+"("+str(ttraj[test])+"): "
             self._single_test(self.inX.strict_can_prepend, ttraj[test], res,
                               failmsg)
 
     def test_inX_0(self):
         """AllInXEnsemble treatment of zero-length trajectory"""
-        assert_equal(self.inX(paths.Trajectory([])), False)
-        assert_equal(self.inX.can_append(paths.Trajectory([])), True)
-        assert_equal(self.inX.can_prepend(paths.Trajectory([])), True)
+        assert self.inX(paths.Trajectory([])) is False
+        assert self.inX.can_append(paths.Trajectory([])) is True
+        assert self.inX.can_prepend(paths.Trajectory([])) is True
 
     def test_inX_str(self):
         volstr = "{x|Id(x) in [0.1, 0.5]}"
-        assert_equal(self.inX.__str__(),
-                     "x[t] in "+volstr+" for all t")
+        assert self.inX.__str__() == "x[t] in "+volstr+" for all t"
 
 class TestAllOutXEnsemble(EnsembleTest):
     def setup_method(self):
         self.outX = AllOutXEnsemble(vol1)
 
     def test_outX(self):
         """AllOutXEnsemble passes the trajectory test suite"""
@@ -355,22 +352,21 @@
                 res = True
             failmsg = "Failure in "+test+"("+str(ttraj[test])+"): "
             self._single_test(self.outX.strict_can_prepend, ttraj[test],
                               res, failmsg)
 
     def test_outX_0(self):
         """AllOutXEnsemble treatment of zero-length trajectory"""
-        assert_equal(self.outX(paths.Trajectory([])), False)
-        assert_equal(self.outX.can_append(paths.Trajectory([])), True)
-        assert_equal(self.outX.can_prepend(paths.Trajectory([])), True)
+        assert self.outX(paths.Trajectory([])) is False
+        assert self.outX.can_append(paths.Trajectory([])) is True
+        assert self.outX.can_prepend(paths.Trajectory([])) is True
 
     def test_outX_str(self):
         volstr = "{x|Id(x) in [0.1, 0.5]}"
-        assert_equal(self.outX.__str__(),
-                     "x[t] in (not "+volstr+") for all t")
+        assert self.outX.__str__() == "x[t] in (not "+volstr+") for all t"
 
 class TestPartInXEnsemble(EnsembleTest):
     def setup_method(self):
         self.hitX = PartInXEnsemble(vol1)
 
     def test_hitX(self):
         """PartInXEnsemble passes the trajectory test suite"""
@@ -392,22 +388,21 @@
         self._test_everything(self.hitX.strict_can_append, default=True)
 
     def test_strict_can_prepend(self):
         self._test_everything(self.hitX.strict_can_prepend, default=True)
 
     def test_hitX_0(self):
         """PartInXEnsemble treatment of zero-length trajectory"""
-        assert_equal(self.hitX(paths.Trajectory([])), False)
-        assert_equal(self.hitX.can_append(paths.Trajectory([])), True)
-        assert_equal(self.hitX.can_prepend(paths.Trajectory([])), True)
+        assert self.hitX(paths.Trajectory([])) is False
+        assert self.hitX.can_append(paths.Trajectory([])) is True
+        assert self.hitX.can_prepend(paths.Trajectory([])) is True
 
     def test_hitX_str(self):
         volstr = "{x|Id(x) in [0.1, 0.5]}"
-        assert_equal(self.hitX.__str__(),
-                     "exists t such that x[t] in "+volstr)
+        assert self.hitX.__str__() == "exists t such that x[t] in " + volstr
 
 
 class TestSequentialEnsemble(EnsembleTest):
     def setup_method(self):
         self.inX = AllInXEnsemble(vol1)
         self.outX = AllOutXEnsemble(vol1)
         self.hitX = PartInXEnsemble(vol1)
@@ -432,58 +427,60 @@
         )
         self.tis = SequentialEnsemble([
             self.inX & self.length1,
             self.outX & self.leaveX0,
             self.inX & self.length1,
         ])
 
-    @raises(ValueError)
     def test_maxminoverlap_size(self):
         """SequentialEnsemble errors if max/min overlap sizes different"""
-        SequentialEnsemble([self.inX, self.outX, self.inX], (0,0), (0,0,0))
+        with pytest.raises(ValueError):
+            SequentialEnsemble([self.inX, self.outX, self.inX],
+                               (0,0), (0,0,0))
 
-    @raises(ValueError)
     def test_maxoverlap_ensemble_size(self):
         """SequentialEnsemble errors if overlap sizes don't match ensemble size"""
-        SequentialEnsemble([self.inX, self.outX, self.inX], (0,0,0), (0,0,0))
+        with pytest.raises(ValueError):
+            SequentialEnsemble([self.inX, self.outX, self.inX],
+                               (0,0,0), (0,0,0))
 
-    @raises(ValueError)
     def test_minmax_order(self):
         """SequentialEnsemble errors if min_overlap > max_overlap"""
-        SequentialEnsemble([self.inX, self.outX, self.inX], (0,1), (0,0))
+        with pytest.raises(ValueError):
+            SequentialEnsemble([self.inX, self.outX, self.inX], (0,1), (0,0))
 
     def test_allowed_initializations(self):
         """SequentialEnsemble initializes correctly with defaults"""
         A = SequentialEnsemble([self.inX, self.outX, self.inX], (0,0), (0,0))
         B = SequentialEnsemble([self.inX, self.outX, self.inX],0,0)
         C = SequentialEnsemble([self.inX, self.outX, self.inX])
-        assert_equal(A.min_overlap,B.min_overlap)
-        assert_equal(A.min_overlap,C.min_overlap)
-        assert_equal(A.max_overlap,B.max_overlap)
-        assert_equal(A.max_overlap,C.max_overlap)
+        assert A.min_overlap == B.min_overlap
+        assert A.min_overlap == C.min_overlap
+        assert A.max_overlap == B.max_overlap
+        assert A.max_overlap == C.max_overlap
 
     def test_overlap_max(self):
         """SequentialEnsemble allows overlaps up to overlap max, no more"""
-        raise SkipTest
+        pytest.skip()
 
     def test_overlap_min(self):
         """SequentialEnsemble requires overlaps of at least overlap min"""
-        raise SkipTest
+        pytest.skip()
 
     def test_overlap_max_inf(self):
         """SequentialEnsemble works if max overlap in infinite"""
-        raise SkipTest
+        pytest.skip()
 
     def test_overlap_min_gap(self):
         """SequentialEnsemble works in mix overlap is negative (gap)"""
-        raise SkipTest
+        pytest.skip()
 
     def test_overlap_max_gap(self):
         """SequentialEnsemble works if max overlap is negative (gap)"""
-        raise SkipTest
+        pytest.skip()
 
     def test_seqens_order_combo(self):
         # regression test for #229
         import numpy as np
         op = paths.FunctionCV(name="x", f=lambda snap : snap.xyz[0][0])
         bigvol = paths.CVDefinedVolume(collectivevariable=op,
                                     lambda_min=-100.0, lambda_max=100.0)
@@ -500,21 +497,21 @@
 
         combo1 = vol_ens & len_ens
         combo2 = len_ens & vol_ens
 
         seq1 = SequentialEnsemble([combo1])
         seq2 = SequentialEnsemble([combo2])
         logger.debug("Checking combo1")
-        assert_equal(combo1.can_append(traj), True)
+        assert combo1.can_append(traj) is True
         logger.debug("Checking combo2")
-        assert_equal(combo2.can_append(traj), True)
+        assert combo2.can_append(traj) is True
         logger.debug("Checking seq1")
-        assert_equal(seq1.can_append(traj), True)
+        assert seq1.can_append(traj) is True
         logger.debug("Checking seq2")
-        assert_equal(seq2.can_append(traj), True)
+        assert seq2.can_append(traj) is True
 
 
     def test_can_append_tis(self):
         """SequentialEnsemble as TISEnsemble knows when it can append"""
         results =   {   'upper_in_out' : True,
                         'lower_in_out' : True,
                         'upper_in_out_in' : False,
@@ -918,20 +915,20 @@
             )
             self._single_test(ensemble.can_append, ttraj[test],
                               append_results[test], failmsg)
 
     def test_sequential_enter_exit(self):
         """SequentialEnsembles based on Enters/ExitsXEnsemble"""
         # TODO: this includes a test of the overlap ability
-        raise SkipTest
+        pytest.skip()
 
 
 
     def test_str(self):
-        assert_equal(self.pseudo_tis.__str__(), """[
+        assert self.pseudo_tis.__str__() == """[
 (
   x[t] in {x|Id(x) in [0.1, 0.5]} for all t
 )
 and
 (
   len(x) = 1
 ),
@@ -939,15 +936,15 @@
 (
   x[t] in {x|Id(x) in [0.1, 0.5]} for all t
 )
 and
 (
   len(x) = 1
 )
-]""")
+]"""
 
 
 class TestSequentialEnsembleCombination(EnsembleTest):
     # testing EnsembleCombinations of SequentialEnsembles -- this is mainly
     # useful to making sure that the ensemble combination of strict_can_*
     # works correctly, since this is where strict and normal have a
     # distinction
@@ -1189,30 +1186,30 @@
         self.tis = TISEnsemble(vol1, vol3, vol2, op)
         self.traj = ttraj['upper_in_out_cross_out_in']
         self.minl = min(op(self.traj))
         self.maxl = max(op(self.traj))
 
     def test_tis_trajectory_summary(self):
         summ = self.tis.trajectory_summary(self.traj)
-        assert_equal(summ['initial_state'], 0)
-        assert_equal(summ['final_state'], 0)
-        assert_equal(summ['max_lambda'], self.maxl)
-        assert_equal(summ['min_lambda'], self.minl)
+        assert summ['initial_state'] == 0
+        assert summ['final_state'] == 0
+        assert summ['max_lambda'] == self.maxl
+        assert summ['min_lambda'] == self.minl
 
     def test_tis_trajectory_summary_str(self):
         mystr = self.tis.trajectory_summary_str(self.traj)
         teststr = ("initial_state=stateA final_state=stateA min_lambda=" +
                    str(self.minl) + " max_lambda=" + str(self.maxl) + " ")
-        assert_equal(mystr, teststr)
+        assert mystr == teststr
 
     def test_no_frame_after_interface(self):
         traj_3 = make_1d_traj([0.2, 0.6,  2.1])
-        assert_equal(self.tis(traj_3), True)
+        assert self.tis(traj_3) is True
         traj_2 = make_1d_traj([0.2, 2.1])
-        assert_equal(self.tis(traj_2), True)
+        assert self.tis(traj_2) is True
 
     def test_tis_ensemble_candidate(self):
         tis = TISEnsemble(vol1, vol3, vol2, op, lambda_i=0.7)
         test_f = lambda t: tis(t, candidate=True)
         results = {}
         upper_keys = [k for k in list(ttraj.keys()) if k[:6] == "upper_"]
         for test in upper_keys:
@@ -1271,102 +1268,102 @@
 class TestEnsembleCache(EnsembleCacheTest):
     def setup_method(self):
         self.fwd = EnsembleCache(direction=+1)
         self.rev = EnsembleCache(direction=-1)
         self.traj = ttraj['lower_in_out_in_in_out_in']
 
     def test_initially_reset(self):
-        assert_equal(self._was_cache_reset(self.fwd), True)
-        assert_equal(self._was_cache_reset(self.rev), True)
+        assert self._was_cache_reset(self.fwd) is True
+        assert self._was_cache_reset(self.rev) is True
 
     def test_change_trajectory(self):
         traj2 = ttraj['lower_in_out_in']
         # tests for forward
         self.fwd.contents = { 'test' : 'object' }
-        assert_equal(self._was_cache_reset(self.fwd), False)
+        assert self._was_cache_reset(self.fwd) is False
         self.fwd.check(self.traj)
-        assert_equal(self._was_cache_reset(self.fwd), True)
+        assert self._was_cache_reset(self.fwd) is True
         self.fwd.contents['ens_num'] = 1
-        assert_equal(self._was_cache_reset(self.fwd), False)
+        assert self._was_cache_reset(self.fwd) is False
         self.fwd.check(traj2)
-        assert_equal(self._was_cache_reset(self.fwd), True)
+        assert self._was_cache_reset(self.fwd) is True
         # tests for backward
         self.rev.contents = { 'test' : 'object' }
-        assert_equal(self._was_cache_reset(self.rev), False)
+        assert self._was_cache_reset(self.rev) is False
         self.rev.check(self.traj)
-        assert_equal(self._was_cache_reset(self.rev), True)
+        assert self._was_cache_reset(self.rev) is True
         self.rev.contents['ens_num'] = 1
-        assert_equal(self._was_cache_reset(self.rev), False)
+        assert self._was_cache_reset(self.rev) is False
         self.rev.check(traj2)
-        assert_equal(self._was_cache_reset(self.rev), True)
+        assert self._was_cache_reset(self.rev) is True
 
     def test_trajectory_by_frame(self):
         # tests for forward
         self.fwd.check(self.traj[0:1])
-        assert_equal(self._was_cache_reset(self.fwd), True)
+        assert self._was_cache_reset(self.fwd) is True
         self.fwd.contents = { 'test' : 'object' }
-        assert_equal(self._was_cache_reset(self.fwd), False)
+        assert self._was_cache_reset(self.fwd) is False
         self.fwd.check(self.traj[0:2])
-        assert_equal(self._was_cache_reset(self.fwd), False)
+        assert self._was_cache_reset(self.fwd) is False
         # tests for backward
         self.rev.check(self.traj[-1:])
-        assert_equal(self._was_cache_reset(self.rev), True)
+        assert self._was_cache_reset(self.rev) is True
         self.rev.contents = { 'test' : 'object' }
-        assert_equal(self._was_cache_reset(self.rev), False)
+        assert self._was_cache_reset(self.rev) is False
         self.rev.check(self.traj[-2:])
-        assert_equal(self._was_cache_reset(self.rev), False)
+        assert self._was_cache_reset(self.rev) is False
 
     def test_same_traj_twice_no_reset(self):
         # tests for forward
         self.fwd.check(self.traj)
-        assert_equal(self._was_cache_reset(self.fwd), True)
+        assert self._was_cache_reset(self.fwd) is True
         self.fwd.contents = { 'test' : 'object' }
         self.fwd.check(self.traj)
-        assert_equal(self._was_cache_reset(self.fwd), False)
+        assert self._was_cache_reset(self.fwd) is False
         # tests for backward
         self.rev.check(self.traj)
-        assert_equal(self._was_cache_reset(self.rev), True)
+        assert self._was_cache_reset(self.rev) is True
         self.rev.contents = { 'test' : 'object' }
         self.rev.check(self.traj)
-        assert_equal(self._was_cache_reset(self.rev), False)
+        assert self._was_cache_reset(self.rev) is False
 
 
     def test_trajectory_skips_frame(self):
         # tests for forward
         self.fwd.check(self.traj[0:1])
-        assert_equal(self._was_cache_reset(self.fwd), True)
+        assert self._was_cache_reset(self.fwd) is True
         self.fwd.contents = { 'test' : 'object' }
-        assert_equal(self._was_cache_reset(self.fwd), False)
+        assert self._was_cache_reset(self.fwd) is False
         self.fwd.check(self.traj[0:3])
-        assert_equal(self._was_cache_reset(self.fwd), True)
+        assert self._was_cache_reset(self.fwd) is True
         # tests for backward
         self.rev.check(self.traj[-1:])
-        assert_equal(self._was_cache_reset(self.rev), True)
+        assert self._was_cache_reset(self.rev) is True
         self.rev.contents = { 'test' : 'object' }
-        assert_equal(self._was_cache_reset(self.rev), False)
+        assert self._was_cache_reset(self.rev) is False
         self.rev.check(self.traj[-3:])
-        assert_equal(self._was_cache_reset(self.rev), True)
+        assert self._was_cache_reset(self.rev) is True
 
     def test_trajectory_middle_frame_changes(self):
         # tests for forward
         self.fwd.check(self.traj[0:2])
-        assert_equal(self._was_cache_reset(self.fwd), True)
+        assert self._was_cache_reset(self.fwd) is True
         self.fwd.contents = { 'test' : 'object' }
-        assert_equal(self._was_cache_reset(self.fwd), False)
+        assert self._was_cache_reset(self.fwd) is False
         new_traj = self.traj[0:1] + self.traj[3:5]
         self.fwd.check(new_traj)
-        assert_equal(self._was_cache_reset(self.fwd), True)
+        assert self._was_cache_reset(self.fwd) is True
         # tests for backward
         self.rev.check(self.traj[0:2])
-        assert_equal(self._was_cache_reset(self.rev), True)
+        assert self._was_cache_reset(self.rev) is True
         self.rev.contents = { 'test' : 'object' }
-        assert_equal(self._was_cache_reset(self.rev), False)
+        assert self._was_cache_reset(self.rev) is False
         new_traj = self.traj[-4:-2] + self.traj[-1:]
         self.rev.check(new_traj)
-        assert_equal(self._was_cache_reset(self.rev), True)
+        assert self._was_cache_reset(self.rev) is True
 
 
 class TestSequentialEnsembleCache(EnsembleCacheTest):
     def setup_method(self):
         self.inX = AllInXEnsemble(vol1)
         self.outX = AllOutXEnsemble(vol1)
         self.length1 = LengthEnsemble(1)
@@ -1379,111 +1376,113 @@
         ])
         self.traj = ttraj['lower_in_out_in_in_out_in']
 
     def test_all_in_as_seq_can_append(self):
         ens = SequentialEnsemble([AllInXEnsemble(vol1 | vol2 | vol3)])
         cache = ens._cache_can_append
         traj = ttraj['upper_in_in_out_out_in_in']
-        assert_equal(ens.can_append(traj[0:1]), True)
-        assert_equal(ens.can_append(traj[0:2]), True)
-        assert_equal(ens.can_append(traj[0:3]), True)
-        assert_equal(ens.can_append(traj[0:4]), True)
-        assert_equal(ens.can_append(traj[0:5]), True)
-        assert_equal(ens.can_append(traj[0:6]), True)
+        assert ens.can_append(traj[0:1]) is True
+        assert ens.can_append(traj[0:2]) is True
+        assert ens.can_append(traj[0:3]) is True
+        assert ens.can_append(traj[0:4]) is True
+        assert ens.can_append(traj[0:5]) is True
+        assert ens.can_append(traj[0:6]) is True
 
     def test_sequential_caching_can_append(self):
         cache = self.pseudo_minus._cache_can_append
-        assert_equal(self.pseudo_minus.can_append(self.traj[0:1]), True)
-        assert_equal(cache.contents['ens_num'], 1)
-        assert_equal(cache.contents['ens_from'], 0)
-        assert_equal(cache.contents['subtraj_from'], 1)
+        assert self.pseudo_minus.can_append(self.traj[0:1]) is True
+        assert cache.contents['ens_num'] == 1
+        assert cache.contents['ens_from'] == 0
+        assert cache.contents['subtraj_from'] == 1
         logging.getLogger('openpathsampling.ensemble').debug("Starting [0:2]")
-        assert_equal(self.pseudo_minus.can_append(self.traj[0:2]), True)
-        assert_equal(cache.contents['ens_num'], 1)
-        assert_equal(cache.contents['ens_from'], 0)
-        assert_equal(cache.contents['subtraj_from'], 1)
+        assert self.pseudo_minus.can_append(self.traj[0:2]) is True
+        assert cache.contents['ens_num'] == 1
+        assert cache.contents['ens_from'] == 0
+        assert cache.contents['subtraj_from'] == 1
         logging.getLogger('openpathsampling.ensemble').debug("Starting [0:3]")
-        assert_equal(self.pseudo_minus.can_append(self.traj[0:3]), True)
-        assert_equal(cache.contents['ens_num'], 2)
-        assert_equal(cache.contents['ens_from'], 0)
-        assert_equal(cache.contents['subtraj_from'], 2)
+        assert self.pseudo_minus.can_append(self.traj[0:3]) is True
+        assert cache.contents['ens_num'] == 2
+        assert cache.contents['ens_from'] == 0
+        assert cache.contents['subtraj_from'] == 2
         logging.getLogger('openpathsampling.ensemble').debug("Starting [0:4]")
-        assert_equal(self.pseudo_minus.can_append(self.traj[0:4]), True)
-        assert_equal(cache.contents['ens_num'], 2)
-        assert_equal(cache.contents['ens_from'], 0)
-        assert_equal(cache.contents['subtraj_from'], 2)
+        assert self.pseudo_minus.can_append(self.traj[0:4]) is True
+        assert cache.contents['ens_num'] == 2
+        assert cache.contents['ens_from'] == 0
+        assert cache.contents['subtraj_from'] == 2
         logging.getLogger('openpathsampling.ensemble').debug("Starting [0:5]")
-        assert_equal(self.pseudo_minus.can_append(self.traj[0:5]), True)
-        assert_equal(cache.contents['ens_num'], 3)
-        assert_equal(cache.contents['ens_from'], 0)
-        assert_equal(cache.contents['subtraj_from'], 4)
+        assert self.pseudo_minus.can_append(self.traj[0:5]) is True
+        assert cache.contents['ens_num'] == 3
+        assert cache.contents['ens_from'] == 0
+        assert cache.contents['subtraj_from'] == 4
         logging.getLogger('openpathsampling.ensemble').debug("Starting [0:6]")
-        assert_equal(self.pseudo_minus.can_append(self.traj[0:6]), False)
-        assert_equal(cache.contents['ens_num'], 4)
-        assert_equal(cache.contents['ens_from'], 0)
-        assert_equal(cache.contents['subtraj_from'], 5)
+        assert self.pseudo_minus.can_append(self.traj[0:6]) is False
+        assert cache.contents['ens_num'] == 4
+        assert cache.contents['ens_from'] == 0
+        assert cache.contents['subtraj_from'] == 5
 
     def test_sequential_caching_resets(self):
         #cache = self.pseudo_minus._cache_can_append
-        assert_equal(self.pseudo_minus.can_append(self.traj[2:3]), True)
-        assert_equal(self.pseudo_minus(self.traj[2:3]), False)
+        assert self.pseudo_minus.can_append(self.traj[2:3]) is True
+        assert self.pseudo_minus(self.traj[2:3]) is False
         #assert_equal(self._was_cache_reset(cache), True)
-        assert_equal(self.pseudo_minus.can_append(self.traj[2:4]), True)
-        assert_equal(self.pseudo_minus(self.traj[2:4]), False)
+        assert self.pseudo_minus.can_append(self.traj[2:4]) is True
+        assert self.pseudo_minus(self.traj[2:4]) is False
         #assert_equal(self._was_cache_reset(cache), True)
         for i in range(4, len(self.traj)-1):
-            assert_equal(self.pseudo_minus.can_append(self.traj[2:i+1]), True)
-            assert_equal(self.pseudo_minus(self.traj[2:i+1]), False)
+            assert self.pseudo_minus.can_append(self.traj[2:i+1]) is True
+            assert self.pseudo_minus(self.traj[2:i+1]) is False
             #assert_equal(self._was_cache_reset(cache), False)
-        assert_equal(self.pseudo_minus.can_append(self.traj[2:]), False)
-        assert_equal(self.pseudo_minus(self.traj[2:]), False)
+        assert self.pseudo_minus.can_append(self.traj[2:]) is False
+        assert self.pseudo_minus(self.traj[2:]) is False
         #assert_equal(self._was_cache_reset(cache), False)
+
+    def test_sequential_caching_resets_backward(self):
         # TODO: same story backward
-        raise SkipTest
+        pytest.skip()
 
     def test_sequential_caching_call(self):
-        raise SkipTest
+        pytest.skip()
 
     def test_sequential_caching_can_prepend(self):
         cache = self.pseudo_minus._cache_can_prepend
-        assert_equal(self.pseudo_minus.can_prepend(self.traj[5:6]), True)
-        assert_equal(cache.contents['ens_num'], 3)
-        assert_equal(cache.contents['ens_from'], 4)
-        assert_equal(cache.contents['subtraj_from'], -1)
-        assert_equal(self.pseudo_minus.can_prepend(self.traj[4:6]), True)
-        assert_equal(cache.contents['ens_num'], 3)
-        assert_equal(cache.contents['ens_from'], 4)
-        assert_equal(cache.contents['subtraj_from'], -1)
-        assert_equal(self.pseudo_minus.can_prepend(self.traj[3:6]), True)
-        assert_equal(cache.contents['ens_num'], 2)
-        assert_equal(cache.contents['ens_from'], 4)
-        assert_equal(cache.contents['subtraj_from'], -2)
-        assert_equal(self.pseudo_minus.can_prepend(self.traj[2:6]), True)
-        assert_equal(cache.contents['ens_num'], 2)
-        assert_equal(cache.contents['ens_from'], 4)
-        assert_equal(cache.contents['subtraj_from'], -2)
-        assert_equal(self.pseudo_minus.can_prepend(self.traj[1:6]), True)
-        assert_equal(cache.contents['ens_num'], 1)
-        assert_equal(cache.contents['ens_from'], 4)
-        assert_equal(cache.contents['subtraj_from'], -4)
-        assert_equal(self.pseudo_minus.can_prepend(self.traj[0:6]), False)
-        assert_equal(cache.contents['ens_num'], 0)
-        assert_equal(cache.contents['ens_from'], 4)
-        assert_equal(cache.contents['subtraj_from'], -5)
+        assert self.pseudo_minus.can_prepend(self.traj[5:6]) is True
+        assert cache.contents['ens_num'] == 3
+        assert cache.contents['ens_from'] == 4
+        assert cache.contents['subtraj_from'] == -1
+        assert self.pseudo_minus.can_prepend(self.traj[4:6]) is True
+        assert cache.contents['ens_num'] == 3
+        assert cache.contents['ens_from'] == 4
+        assert cache.contents['subtraj_from'] == -1
+        assert self.pseudo_minus.can_prepend(self.traj[3:6]) is True
+        assert cache.contents['ens_num'] == 2
+        assert cache.contents['ens_from'] == 4
+        assert cache.contents['subtraj_from'] == -2
+        assert self.pseudo_minus.can_prepend(self.traj[2:6]) is True
+        assert cache.contents['ens_num'] == 2
+        assert cache.contents['ens_from'] == 4
+        assert cache.contents['subtraj_from'] == -2
+        assert self.pseudo_minus.can_prepend(self.traj[1:6]) is True
+        assert cache.contents['ens_num'] == 1
+        assert cache.contents['ens_from'] == 4
+        assert cache.contents['subtraj_from'] == -4
+        assert self.pseudo_minus.can_prepend(self.traj[0:6]) is False
+        assert cache.contents['ens_num'] == 0
+        assert cache.contents['ens_from'] == 4
+        assert cache.contents['subtraj_from'] == -5
 
 
 
 
 class TestSlicedTrajectoryEnsemble(EnsembleTest):
     def test_sliced_ensemble_init(self):
         init_as_int = SlicedTrajectoryEnsemble(AllInXEnsemble(vol1), 3)
         init_as_slice = SlicedTrajectoryEnsemble(AllInXEnsemble(vol1),
                                                  slice(3, 4))
-        assert_equal(init_as_int, init_as_slice)
-        assert_equal(init_as_slice.region, init_as_int.region)
+        assert init_as_int == init_as_slice
+        assert init_as_slice.region == init_as_int.region
 
     def test_sliced_as_TISEnsemble(self):
         '''SlicedTrajectory and Sequential give same TIS results'''
         sliced_tis = (
             SlicedTrajectoryEnsemble(AllInXEnsemble(vol1), 0) &
             SlicedTrajectoryEnsemble(AllOutXEnsemble(vol1 | vol3), slice(1,-1)) &
             SlicedTrajectoryEnsemble(PartOutXEnsemble(vol2), slice(1,-1)) &
@@ -1503,15 +1502,15 @@
                               sequential_tis(ttraj[test]), failmsg)
 
     def test_slice_outside_trajectory_range(self):
         ens = SlicedTrajectoryEnsemble(AllInXEnsemble(vol1), slice(5,9))
         test = 'upper_in'
         # the slice should return the empty trajectory, and therefore should
         # return false
-        assert_equal(ens(ttraj[test]), False)
+        assert ens(ttraj[test]) is False
 
     def test_even_sliced_trajectory(self):
         even_slice = slice(None, None, 2)
         ens = SlicedTrajectoryEnsemble(AllInXEnsemble(vol1), even_slice)
         bare_results = {'in' : True,
                         'in_in' : True,
                         'in_in_in' : True,
@@ -1587,22 +1586,22 @@
     def test_sliced_str(self):
         even_slice = slice(None,None, 2)
         slice_1_10 = slice(1, 10)
         slice_1_end = slice(1,None)
         slice_no_ends = slice(1, -1)
         inX = AllInXEnsemble(vol1)
         inXstr = "x[t] in {x|Id(x) in [0.1, 0.5]} for all t"
-        assert_equal(SlicedTrajectoryEnsemble(inX, even_slice).__str__(),
-                     "("+inXstr+" in {:} every 2)")
-        assert_equal(SlicedTrajectoryEnsemble(inX, slice_1_10).__str__(),
-                     "("+inXstr+" in {1:10})")
-        assert_equal(SlicedTrajectoryEnsemble(inX, slice_1_end).__str__(),
-                     "("+inXstr+" in {1:})")
-        assert_equal(SlicedTrajectoryEnsemble(inX, slice_no_ends).__str__(),
-                     "("+inXstr+" in {1:-1})")
+        assert (SlicedTrajectoryEnsemble(inX, even_slice).__str__()
+                == "("+inXstr+" in {:} every 2)")
+        assert (SlicedTrajectoryEnsemble(inX, slice_1_10).__str__()
+                == "("+inXstr+" in {1:10})")
+        assert (SlicedTrajectoryEnsemble(inX, slice_1_end).__str__()
+                == "("+inXstr+" in {1:})")
+        assert (SlicedTrajectoryEnsemble(inX, slice_no_ends).__str__()
+                == "("+inXstr+" in {1:-1})")
 
 class TestOptionalEnsemble(EnsembleTest):
     def setup_method(self):
         self.start_opt = SequentialEnsemble([
             OptionalEnsemble(AllOutXEnsemble(vol1)),
             AllInXEnsemble(vol1),
             AllOutXEnsemble(vol1)
@@ -1850,86 +1849,86 @@
             failmsg = "Failure in "+test+"("+tstr(ttraj[test])+"): "
             self._single_test(fcn, ttraj[test], results[test], failmsg)
 
 
     def test_optional_str(self):
         inX = AllInXEnsemble(vol1)
         opt_inX = OptionalEnsemble(inX)
-        assert_equal(opt_inX.__str__(), "{"+inX.__str__()+"} (OPTIONAL)")
+        assert opt_inX.__str__() == "{"+inX.__str__()+"} (OPTIONAL)"
 
 class TestPrefixTrajectoryEnsemble(EnsembleTest):
     def setup_method(self):
         self.inX = AllInXEnsemble(vol1)
 
     def test_bad_start_traj(self):
         traj = ttraj['upper_out_in_in_in']
         ens = PrefixTrajectoryEnsemble(
             SequentialEnsemble([self.inX]),
             traj[0:2]
         )
-        assert_equal(ens.can_append(traj[0:3]), False)
-        assert_equal(ens.strict_can_append(traj[0:3]), False)
-        assert_equal(ens(traj[0:3]), False)
+        assert ens.can_append(traj[0:3]) is False
+        assert ens.strict_can_append(traj[0:3]) is False
+        assert ens(traj[0:3]) is False
 
     def test_good_start_traj(self):
         traj = ttraj['upper_in_in_in']
         ens = PrefixTrajectoryEnsemble(
             SequentialEnsemble([self.inX]),
             traj[0:2]
         )
-        assert_equal(ens.can_append(traj[2:3]), True)
-        assert_equal(ens.strict_can_append(traj[2:3]), True)
-        assert_equal(ens(traj[2:3]), True)
+        assert ens.can_append(traj[2:3]) is True
+        assert ens.strict_can_append(traj[2:3]) is True
+        assert ens(traj[2:3]) is True
 
-    @raises(RuntimeError)
     def test_can_prepend(self):
         traj = ttraj['upper_in_in_in']
         ens = PrefixTrajectoryEnsemble(
             SequentialEnsemble([self.inX]),
             traj[0:2]
         )
-        ens.can_prepend(traj[2:3])
+        with pytest.raises(RuntimeError):
+            ens.can_prepend(traj[2:3])
 
-    @raises(RuntimeError)
     def test_strict_can_prepend(self):
         traj = ttraj['upper_in_in_in']
         ens = PrefixTrajectoryEnsemble(
             SequentialEnsemble([self.inX]),
             traj[0:2]
         )
-        ens.strict_can_prepend(traj[2:3])
+        with pytest.raises(RuntimeError):
+            ens.strict_can_prepend(traj[2:3])
 
     def test_caching_in_fwdapp_seq(self):
         inX = AllInXEnsemble(vol1)
         outX = AllOutXEnsemble(vol1)
         length1 = LengthEnsemble(1)
         pseudo_minus = SequentialEnsemble([
             inX & length1,
             outX,
             inX,
             outX,
             inX & length1
         ])
         traj = ttraj['upper_in_out_in_in_out_in']
         ens = PrefixTrajectoryEnsemble(pseudo_minus, traj[0:2])
-        assert_equal(ens.can_append(traj[2:3]), True)
-        assert_equal(ens._cached_trajectory, traj[0:3])
-        assert_equal(ens._cache_can_append.trusted, False)
-
-        assert_equal(ens.can_append(traj[2:4]), True)
-        assert_equal(ens._cached_trajectory, traj[0:4])
-        assert_equal(ens._cache_can_append.trusted, True)
-
-        assert_equal(ens.can_append(traj[2:5]), True)
-        assert_equal(ens._cached_trajectory, traj[0:5])
-        assert_equal(ens._cache_can_append.trusted, True)
-
-        assert_equal(ens.can_append(traj[2:6]), False)
-        assert_equal(ens._cached_trajectory, traj[0:6])
-        assert_equal(ens._cache_can_append.trusted, True)
+        assert ens.can_append(traj[2:3]) is True
+        assert ens._cached_trajectory == traj[0:3]
+        assert ens._cache_can_append.trusted is False
+
+        assert ens.can_append(traj[2:4]) is True
+        assert ens._cached_trajectory == traj[0:4]
+        assert ens._cache_can_append.trusted is True
+
+        assert ens.can_append(traj[2:5]) is True
+        assert ens._cached_trajectory == traj[0:5]
+        assert ens._cache_can_append.trusted is True
+
+        assert ens.can_append(traj[2:6]) is False
+        assert ens._cached_trajectory == traj[0:6]
+        assert ens._cache_can_append.trusted is True
 
 
 class TestSuffixTrajectoryEnsemble(EnsembleTest):
     def setup_method(self):
         xval = paths.FunctionCV("x", lambda s : s.xyz[0][0])
         vol = paths.CVDefinedVolume(xval, 0.1, 0.5)
         self.inX = AllInXEnsemble(vol)
@@ -1937,80 +1936,80 @@
 
     def test_bad_end_traj(self):
         traj = ttraj['upper_in_in_in_out']
         ens = SuffixTrajectoryEnsemble(
             SequentialEnsemble([self.inX]),
             traj[-2:]
         )
-        assert_equal(ens.can_prepend(traj[-3:2]), False)
-        assert_equal(ens.strict_can_prepend(traj[-3:2]), False)
-        assert_equal(ens(traj[-3:2]), False)
+        assert ens.can_prepend(traj[-3:2]) is False
+        assert ens.strict_can_prepend(traj[-3:2]) is False
+        assert ens(traj[-3:2]) is False
 
     def test_good_end_traj(self):
         traj = ttraj['upper_out_in_in_in']
         ens = SuffixTrajectoryEnsemble(
             SequentialEnsemble([self.inX]),
             traj[-2:]
         )
-        assert_equal(ens.can_prepend(traj[-3:-2]), True)
-        assert_equal(ens.strict_can_prepend(traj[-3:-2]), True)
-        assert_equal(ens(traj[-3:-2]), True)
-        assert_equal(ens.can_prepend(traj[-4:-2]), False)
-        assert_equal(ens.strict_can_prepend(traj[-4:-2]), False)
-        assert_equal(ens(traj[-4:-2]), False)
+        assert ens.can_prepend(traj[-3:-2]) is True
+        assert ens.strict_can_prepend(traj[-3:-2]) is True
+        assert ens(traj[-3:-2]) is True
+        assert ens.can_prepend(traj[-4:-2]) is False
+        assert ens.strict_can_prepend(traj[-4:-2]) is False
+        assert ens(traj[-4:-2]) is False
 
-    @raises(RuntimeError)
     def test_can_append(self):
         traj = ttraj['upper_out_in_in_in']
         ens = SuffixTrajectoryEnsemble(
             SequentialEnsemble([self.inX]),
             traj[-2:]
         )
-        ens.can_append(traj)
+        with pytest.raises(RuntimeError):
+            ens.can_append(traj)
 
-    @raises(RuntimeError)
     def test_strict_can_append(self):
         traj = ttraj['upper_out_in_in_in']
         ens = SuffixTrajectoryEnsemble(
             SequentialEnsemble([self.inX]),
             traj[-2:]
         )
-        ens.strict_can_append(traj)
+        with pytest.raises(RuntimeError):
+            ens.strict_can_append(traj)
 
     def test_caching_in_bkwdprep_seq(self):
         length1 = LengthEnsemble(1)
         pseudo_minus = SequentialEnsemble([
             self.inX & length1,
             self.outX,
             self.inX,
             self.outX,
             self.inX & length1
         ])
         traj = ttraj['upper_in_out_in_in_out_in']
 
         # sanity checks before running the suffixed version
-        assert_equal(pseudo_minus(traj), True)
+        assert pseudo_minus(traj) is True
         for i in range(-1, -6):
-            assert_equal(pseudo_minus.can_prepend(traj[i:]), True)
+            assert pseudo_minus.can_prepend(traj[i:]) is True
 
         logger.debug("alltraj " + str([id(i) for i in traj]))
         ens = SuffixTrajectoryEnsemble(pseudo_minus, traj[-3:])
-        assert_equal(len(ens._cached_trajectory), 3)
+        assert len(ens._cached_trajectory) == 3
 
-        assert_equal(ens.can_prepend(traj[-4:-3].reversed), True)
-        assert_equal(len(ens._cached_trajectory), 4)
-        assert_equal(ens._cache_can_prepend.trusted, False)
-
-        assert_equal(ens.can_prepend(traj[-5:-3].reversed), True)
-        assert_equal(len(ens._cached_trajectory), 5)
-        assert_equal(ens._cache_can_prepend.trusted, True)
-
-        assert_equal(ens.can_prepend(traj[-6:-3].reversed), False)
-        assert_equal(len(ens._cached_trajectory), 6)
-        assert_equal(ens._cache_can_prepend.trusted, True)
+        assert ens.can_prepend(traj[-4:-3].reversed) is True
+        assert len(ens._cached_trajectory) == 4
+        assert ens._cache_can_prepend.trusted is False
+
+        assert ens.can_prepend(traj[-5:-3].reversed) is True
+        assert len(ens._cached_trajectory) == 5
+        assert ens._cache_can_prepend.trusted is True
+
+        assert ens.can_prepend(traj[-6:-3].reversed) is False
+        assert len(ens._cached_trajectory) == 6
+        assert ens._cache_can_prepend.trusted is True
 
 class TestMinusInterfaceEnsemble(EnsembleTest):
     def setup_method(self):
         # Mostly we use minus ensembles where the state matches the first
         # interface. We also test the case where that isn't in, in which
         # case there's an interstitial zone. (Only test it for nl=2 to keep
         # things easier.)
@@ -2030,21 +2029,21 @@
             n_l=3
         )
 
     def test_dict_round_trip(self):
         dct = self.minus_nl2.to_dict()
         rebuilt = MinusInterfaceEnsemble.from_dict(dct)
         dct2 = rebuilt.to_dict()
-        assert_equal(dct, dct2)
+        assert dct == dct2
 
-    @raises(ValueError)
     def test_minus_nl1_fail(self):
-        minus_nl1 = MinusInterfaceEnsemble(state_vol=vol1,
-                                           innermost_vols=vol2,
-                                           n_l=1)
+        with pytest.raises(ValueError):
+            minus_nl1 = MinusInterfaceEnsemble(state_vol=vol1,
+                                               innermost_vols=vol2,
+                                               n_l=1)
 
 
     def test_minus_nl2_ensemble(self):
         non_default = [
             'in_cross_in_cross_in',
             'in_out_in_in_out_in',
             'in_out_in_out_in'
@@ -2307,37 +2306,37 @@
         predestined_snaps = [trajB[-1]]+ttraj['upper_out_in']
         predestined_traj = [s.xyz[0][0] for s in predestined_snaps]
         engine = CalvinistDynamics(predestined_traj)
         sample = self.minus_nl2.extend_sample_from_trajectories(
             sset, replica=-1, engine=engine, level='complex'
         )
 
-        assert_equal(sample.ensemble(sample.trajectory), True)
-        assert_equal(sample.ensemble, self.minus_nl2)
-        assert_equal(sample.replica, -1)
-        assert_equal(len(sample.trajectory), 5)
+        assert sample.ensemble(sample.trajectory) is True
+        assert sample.ensemble == self.minus_nl2
+        assert sample.replica == -1
+        assert len(sample.trajectory) == 5
         expected = trajB + ttraj['upper_out_in']
         for (t, b) in zip(sample.trajectory, expected):
-            assert_equal(t.xyz[0][0], b.xyz[0][0])
+            assert t.xyz[0][0] == b.xyz[0][0]
 
         # test with a different trajectory
         predestined_snaps = [trajB[-1]]+ttraj['upper_in_out_in']
         predestined_traj = [s.xyz[0][0] for s in predestined_snaps]
         engine = CalvinistDynamics(predestined_traj)
         sample = self.minus_nl2.extend_sample_from_trajectories(
             sset, replica=-1, engine=engine, level='complex'
         )
 
-        assert_equal(sample.ensemble(sample.trajectory), True)
-        assert_equal(sample.ensemble, self.minus_nl2)
-        assert_equal(sample.replica, -1)
-        assert_equal(len(sample.trajectory), 6)
+        assert sample.ensemble(sample.trajectory) is True
+        assert sample.ensemble == self.minus_nl2
+        assert sample.replica == -1
+        assert len(sample.trajectory) == 6
         expected = trajB + ttraj['upper_in_out_in']
         for (t, b) in zip(sample.trajectory, expected):
-            assert_equal(t.xyz[0][0], b.xyz[0][0])
+            assert t.xyz[0][0] == b.xyz[0][0]
 
 
 # TODO: this whole class should become a single test in SeqEns
 class TestSingleEnsembleSequentialEnsemble(EnsembleTest):
     def setup_method(self):
         #self.inner_ens = AllInXEnsemble(vol1 | vol2)
         self.inner_ens = LengthEnsemble(3) & AllInXEnsemble( vol1 | vol2 )
@@ -2356,99 +2355,98 @@
 
 class TestEnsembleSplit(EnsembleTest):
     def setup_method(self):
         self.inA = AllInXEnsemble(vol1)
         self.outA = AllOutXEnsemble(vol1)
 
     def test_split(self):
-#        raise SkipTest
         traj1 = ttraj['upper_in_out_in_in']
         # print [s for s in traj1]
         subtrajs_in_1 = self.inA.split(traj1)
         # print subtrajs_in_1
         # print [[s for s in t] for t in subtrajs_in_1]
-        assert_equal(len(subtrajs_in_1), 2)
-        assert_equal(len(subtrajs_in_1[0]), 1)
-        assert_equal(len(subtrajs_in_1[1]), 2)
+        assert len(subtrajs_in_1) == 2
+        assert len(subtrajs_in_1[0]) == 1
+        assert len(subtrajs_in_1[1]) == 2
         subtrajs_out_1 = self.outA.split(traj1)
-        assert_equal(len(subtrajs_out_1), 1)
+        assert len(subtrajs_out_1) == 1
 
         traj2 = ttraj['upper_in_out_in_in_out_in']
         # print [s for s in traj2]
         subtrajs_in_2 = self.inA.split(traj2)
         # print [[s for s in t] for t in subtrajs_in_2]
-        assert_equal(len(subtrajs_in_2), 3)
-        assert_equal(len(subtrajs_in_2[0]), 1)
-        assert_equal(len(subtrajs_in_2[1]), 2)
-        assert_equal(len(subtrajs_in_2[2]), 1)
+        assert len(subtrajs_in_2) == 3
+        assert len(subtrajs_in_2[0]) == 1
+        assert len(subtrajs_in_2[1]) == 2
+        assert len(subtrajs_in_2[2]) == 1
         subtrajs_out_2 = self.outA.split(traj2)
-        assert_equal(len(subtrajs_out_2), 2)
-        assert_equal(len(subtrajs_out_2[0]), 1)
-        assert_equal(len(subtrajs_out_2[1]), 1)
+        assert len(subtrajs_out_2) == 2
+        assert len(subtrajs_out_2[0]) == 1
+        assert len(subtrajs_out_2[1]) == 1
 
         ensembleAXA = paths.SequentialEnsemble([
             self.inA,
             self.outA,
             self.inA
         ])
 
         traj3 = make_1d_traj(coordinates=[0.3, 0.6, 0.3, 0.6, 0.3])
 
         assert(self.inA(paths.Trajectory([traj3[0]])))
         assert(self.outA(paths.Trajectory([traj3[1]])))
 
         subtrajs_in_3 = ensembleAXA.split(traj3)
-        assert_equal((len(subtrajs_in_3)), 2)
-        assert_equal((len(subtrajs_in_3[0])), 3)
-        assert_equal((len(subtrajs_in_3[1])), 3)
+        assert (len(subtrajs_in_3)) == 2
+        assert (len(subtrajs_in_3[0])) == 3
+        assert (len(subtrajs_in_3[1])) == 3
         assert(traj3.subtrajectory_indices(subtrajs_in_3[0]) == [0, 1, 2])
         assert(traj3.subtrajectory_indices(subtrajs_in_3[1]) == [2, 3, 4])
 
         subtrajs_in_3 = ensembleAXA.split(traj3, reverse=True)
-        assert_equal((len(subtrajs_in_3)), 2)
-        assert_equal((len(subtrajs_in_3[0])), 3)
-        assert_equal((len(subtrajs_in_3[1])), 3)
+        assert (len(subtrajs_in_3)) == 2
+        assert (len(subtrajs_in_3[0])) == 3
+        assert (len(subtrajs_in_3[1])) == 3
         assert(traj3.subtrajectory_indices(subtrajs_in_3[0]) == [2, 3, 4])
         assert(traj3.subtrajectory_indices(subtrajs_in_3[1]) == [0, 1, 2])
 
         subtrajs_in_3 = ensembleAXA.split(traj3, overlap=0)
-        assert_equal((len(subtrajs_in_3)), 1)
-        assert_equal((len(subtrajs_in_3[0])), 3)
+        assert (len(subtrajs_in_3)) == 1
+        assert (len(subtrajs_in_3[0])) == 3
         assert(traj3.subtrajectory_indices(subtrajs_in_3[0]) == [0, 1, 2])
 
         subtrajs_in_3 = ensembleAXA.split(traj3, reverse=True, overlap=0)
-        assert_equal((len(subtrajs_in_3)), 1)
-        assert_equal((len(subtrajs_in_3[0])), 3)
+        assert (len(subtrajs_in_3)) == 1
+        assert (len(subtrajs_in_3[0])) == 3
         assert(traj3.subtrajectory_indices(subtrajs_in_3[0]) == [2, 3, 4])
 
         subtrajs_in_3 = ensembleAXA.split(traj3, overlap=1, max_length=2)
-        assert_equal((len(subtrajs_in_3)), 0)
+        assert (len(subtrajs_in_3)) == 0
 
         subtrajs_in_3 = ensembleAXA.split(traj3, reverse=True, max_length=2)
-        assert_equal((len(subtrajs_in_3)), 0)
+        assert (len(subtrajs_in_3)) == 0
 
         subtrajs_in_3 = ensembleAXA.split(traj3, max_length=3)
-        assert_equal(len(subtrajs_in_3), 2)
-        assert_equal((len(subtrajs_in_3[0])), 3)
-        assert_equal((len(subtrajs_in_3[1])), 3)
+        assert len(subtrajs_in_3) == 2
+        assert (len(subtrajs_in_3[0])) == 3
+        assert (len(subtrajs_in_3[1])) == 3
         assert(traj3.subtrajectory_indices(subtrajs_in_3[0]) == [0, 1, 2])
         assert(traj3.subtrajectory_indices(subtrajs_in_3[1]) == [2, 3, 4])
 
         subtrajs_in_3 = ensembleAXA.split(traj3, reverse=True, max_length=3)
-        assert_equal((len(subtrajs_in_3)), 2)
-        assert_equal((len(subtrajs_in_3[0])), 3)
-        assert_equal((len(subtrajs_in_3[1])), 3)
+        assert (len(subtrajs_in_3)) == 2
+        assert (len(subtrajs_in_3[0])) == 3
+        assert (len(subtrajs_in_3[1])) == 3
         assert(traj3.subtrajectory_indices(subtrajs_in_3[1]) == [0, 1, 2])
         assert(traj3.subtrajectory_indices(subtrajs_in_3[0]) == [2, 3, 4])
 
         subtrajs_in_3 = ensembleAXA.split(traj3, reverse=False, min_length=4)
-        assert_equal((len(subtrajs_in_3)), 0)
+        assert (len(subtrajs_in_3)) == 0
 
         subtrajs_in_3 = ensembleAXA.split(traj3, reverse=True, min_length=4)
-        assert_equal((len(subtrajs_in_3)), 0)
+        assert (len(subtrajs_in_3)) == 0
 
         sub_traj = ensembleAXA.find_first_subtrajectory(traj3)
         assert(traj3.subtrajectory_indices(sub_traj) == [0,1,2])
 
         sub_traj = ensembleAXA.find_last_subtrajectory(traj3)
         assert(traj3.subtrajectory_indices(sub_traj) == [2,3,4])
 
@@ -2488,34 +2486,34 @@
             if direction > 0:
                 start = 0
                 end = start + (i+start_traj_len)
             elif direction < 0:
                 end = len(trajectory)
                 start = end - (i+start_traj_len)
             # test untrusted
-            assert_equal(function(trajectory[start:end]), results[i])
+            assert function(trajectory[start:end]) == results[i]
             # test trusted
             trusted_val = function(trajectory[start:end], trusted=True)
             # print i, "["+str(start)+":"+str(end)+"]", trusted_val, results[i]
-            assert_equal(trusted_val, results[i])
+            assert trusted_val == results[i]
             for cache in list(cache_results.keys()):
                 # TODO: this is currently very specific to the caches used
                 # by volumes ensembles. That should be generalized by
                 # allowing several different tags within contents.
                 # cache_results could {cache : {'content_key' : [values]}}
                 if cache_results[cache][i] is not None:
                     #print "cache", cache_results.keys().index(cache),
                     try:
                         contents = cache.contents['previous']
                     except KeyError:
                         contents = None
                     #print contents, cache_results[cache][i]
 
-                    assert_equal(cache.contents['previous'],
-                                 cache_results[cache][i])
+                    assert (cache.contents['previous']
+                            == cache_results[cache][i])
 
     def test_call_outA_or_outB(self):
         # print self.local_ttraj['upper_out_in_out_out_cross'].xyz[:,0,0]
         self._test_trusted(
             trajectory=self.local_ttraj['upper_out_in_out_out_cross'],
             function=self.outA_or_outB,
             results=[True, True, True, True, False],
@@ -2718,12 +2716,12 @@
     # generic tests for ensemble equality; we use the EmptyEnsemble as
     # example. See:
     # * https://github.com/openpathsampling/openpathsampling/issues/700
     # * https://github.com/openpathsampling/openpathsampling/issues/701
     def test_empty_ensemble_equality(self):
         ens1 = paths.EmptyEnsemble()
         ens2 = paths.EmptyEnsemble()
-        assert_true(ens1 == ens2)
-        assert_false(ens1 != ens2)
+        assert ens1 == ens2
+        assert not ens1 != ens2  # needed __ne__ tested in the Py27 days
 
     # TODO: may add tests for other ensembles, or may move this test
     # somewhere else
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_external_engine.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_external_engine.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_external_snapshots.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_external_snapshots.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_features.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_features.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import absolute_import
 from builtins import hex
 from builtins import object
-from nose.tools import raises
 
-from nose.plugins.skip import SkipTest
+import pytest
 from .test_helpers import u
 
 import logging
 
 import numpy as np
 import numpy.testing as npt
 try:
@@ -38,15 +37,15 @@
         toy_copy = toy_snap.copy_with_replacement(velocities=rep_vel)
 
         assert(toy_snap.velocities[1] == 4.0)
         assert(toy_copy.velocities[1] == 1.0)
 
     def test_copy_with_replacement_openmm(self):
         if not paths.integration_tools.HAS_OPENMM or omt is None:
-            raise SkipTest
+            pytest.skip()
         # test an openmm snapshot
         sys = omt.testsystems.AlanineDipeptideVacuum()
         omm_snap = omm_engine.snapshot_from_testsystem(sys)
 
         rep_vel = omm_snap.velocities * 2.0
         omm_copy = omm_snap.copy_with_replacement(
             velocities=rep_vel)
@@ -59,14 +58,14 @@
         omm_copy = omm_snap.copy_with_replacement(
             coordinates=[1.0, 2.0, 3.0] * u.nanometer,
             box_vectors=[1.0, 1.0, 1.0] * u.nanometer)
 
         assert(hex(id(omm_snap.kinetics)) == hex(id(omm_copy.kinetics)))
         assert(hex(id(omm_snap.statics)) != hex(id(omm_copy.statics)))
 
-    @raises(TypeError)
     def test_parameter_error(self):
         init_coord = np.array([1.0, 2.0])
         init_vel = np.array([3.0, 4.0])
         toy_snap = toy_engine.Snapshot(
             coordinates=init_coord, velocities=init_vel)
-        toy_snap.copy_with_replacement(dummy=0)
+        with pytest.raises(TypeError):
+            toy_snap.copy_with_replacement(dummy=0)
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_gromacs_engine.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_gromacs_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 import pytest
 import numpy.testing as npt
-from nose.tools import (assert_equal, assert_not_equal, assert_almost_equal,
-                        raises, assert_true)
-from nose.plugins.skip import Skip, SkipTest
-import numpy.testing as npt
 import tempfile
 
 from .test_helpers import data_filename, assert_items_equal
 
 import openpathsampling as paths
 try:
     import mdtraj as md
@@ -109,38 +105,38 @@
         shutil.rmtree(self.engine.prefix + "_log")
         shutil.rmtree(self.engine.prefix + "_edr")
 
     def test_read_frame_from_file_success(self):
         # when the frame is present, we should return it
         fname = os.path.join(self.test_dir, "project_trr", "0000000.trr")
         result = self.engine.read_frame_from_file(fname, 0)
-        assert_true(isinstance(result, ExternalMDSnapshot))
-        assert_equal(result.file_name, fname)
-        assert_equal(result.file_position, 0)
+        assert isinstance(result, ExternalMDSnapshot)
+        assert result.file_name == fname
+        assert result.file_position == 0
         # TODO: add caching of xyz, vel, box; check that we have it now
 
         fname = os.path.join(self.test_dir, "project_trr", "0000000.trr")
         result = self.engine.read_frame_from_file(fname, 3)
-        assert_true(isinstance(result, ExternalMDSnapshot))
-        assert_equal(result.file_name, fname)
-        assert_equal(result.file_position, 3)
+        assert isinstance(result, ExternalMDSnapshot)
+        assert result.file_name == fname
+        assert result.file_position == 3
 
     def test_read_frame_from_file_partial(self):
         # if a frame is partial, return 'partial'
         fname = os.path.join(self.test_dir, "project_trr", "0000099.trr")
         frame_2 = self.engine.read_frame_from_file(fname, 49)
-        assert_true(isinstance(frame_2, ExternalMDSnapshot))
+        assert isinstance(frame_2, ExternalMDSnapshot)
         frame_3 = self.engine.read_frame_from_file(fname, 50)
-        assert_equal(frame_3, "partial")
+        assert frame_3 == "partial"
 
     def test_read_frame_from_file_none(self):
         # if a frame is beyond the last frame, return None
         fname = os.path.join(self.test_dir, "project_trr", "0000000.trr")
         result = self.engine.read_frame_from_file(fname, 4)
-        assert_equal(result, None)
+        assert result is None
 
     def test_write_frame_to_file_read_back(self):
         # write random frame; read back
         # sinfully, we start by reading in a frame to get the correct dims
         fname = os.path.join(self.test_dir, "project_trr", "0000000.trr")
         tmp = self.engine.read_frame_from_file(fname, 0)
         shape = tmp.xyz.shape
@@ -154,16 +150,16 @@
         file_49 = os.path.join(self.test_dir, "project_trr", "0000049.trr")
         snap = ExternalMDSnapshot(file_name=file_49, file_position=2,
                                   engine=self.engine)
         snap.set_details(xyz, vel, box)
         self.engine.write_frame_to_file(traj_50, snap)
 
         snap2 = self.engine.read_frame_from_file(traj_50, 0)
-        assert_equal(snap2.file_name, traj_50)
-        assert_equal(snap2.file_position, 0)
+        assert snap2.file_name == traj_50
+        assert snap2.file_position == 0
         npt.assert_array_almost_equal(snap.xyz, snap2.xyz)
         npt.assert_array_almost_equal(snap.velocities, snap2.velocities)
         npt.assert_array_almost_equal(snap.box_vectors, snap2.box_vectors)
 
         if os.path.isfile(traj_50):
             os.remove(traj_50)
 
@@ -172,28 +168,33 @@
                              base_dir=self.test_dir, options={},
                              prefix="proj")
         test_engine.set_filenames(0)
         assert test_engine.input_file == \
                 os.path.join(self.test_dir, "initial_frame.trr")
         assert test_engine.output_file == \
                 os.path.join(self.test_dir, "proj_trr", "0000001.trr")
-        assert_equal(test_engine.edr_file,
-                     os.path.join(self.test_dir, "proj_edr", "0000001.edr"))
-        assert_equal(test_engine.log_file,
-                     os.path.join(self.test_dir, "proj_log", "0000001.log"))
+        assert test_engine.edr_file == os.path.join(self.test_dir,
+                                                    "proj_edr",
+                                                    "0000001.edr")
+        assert test_engine.log_file == os.path.join(self.test_dir,
+                                                    "proj_log",
+                                                    "0000001.log")
 
         test_engine.set_filenames(99)
-        assert_equal(test_engine.input_file,
-                     os.path.join(self.test_dir, "initial_frame.trr"))
-        assert_equal(test_engine.output_file,
-                     os.path.join(self.test_dir, "proj_trr", "0000100.trr"))
-        assert_equal(test_engine.edr_file,
-                     os.path.join(self.test_dir, "proj_edr", "0000100.edr"))
-        assert_equal(test_engine.log_file,
-                     os.path.join(self.test_dir, "proj_log", "0000100.log"))
+        assert test_engine.input_file == os.path.join(self.test_dir,
+                                                      "initial_frame.trr")
+        assert test_engine.output_file == os.path.join(self.test_dir,
+                                                       "proj_trr",
+                                                       "0000100.trr")
+        assert test_engine.edr_file == os.path.join(self.test_dir,
+                                                    "proj_edr",
+                                                    "0000100.edr")
+        assert test_engine.log_file == os.path.join(self.test_dir,
+                                                    "proj_log",
+                                                    "0000100.log")
 
     def test_set_filenames_fixed(self):
         test_engine = Engine(gro="conf.gro", mdp="md.mdp", top="topol.top",
                              base_dir=self.test_dir, options={},
                              prefix="proj")
         test_engine.set_filenames('foo')
         assert test_engine.input_file == \
@@ -230,34 +231,34 @@
 
         traj_0 = self.engine.trajectory_filename(0)
         snap = self.engine.read_frame_from_file(traj_0, 0)
         self.engine.filename_setter.reset(0)
 
         ens = paths.LengthEnsemble(5)
         traj = self.engine.generate(snap, running=[ens.can_append])
-        assert_equal(self.engine.proc.is_running(), False)
-        assert_equal(len(traj), 5)
+        assert self.engine.proc.is_running() is False
+        assert len(traj) == 5
         ttraj = md.load(self.engine.trajectory_filename(1),
                         top=self.engine.gro)
         # the mdp suggests a max length of 100 frames
-        assert_true(len(ttraj) < 100)
+        assert len(ttraj) < 100
 
     def test_prepare(self):
         if not has_gmx:
             pytest.skip("gmx not found. Skipping test.")
         self.engine.set_filenames(0)
         traj_0 = self.engine.trajectory_filename(0)
         snap = self.engine.read_frame_from_file(traj_0, 0)
         self.engine.write_frame_to_file(self.engine.input_file, snap)
         files = ['topol.tpr', 'mdout.mdp']
         for f in files:
             if os.path.isfile(f):
                 raise AssertionError("File " + str(f) + " already exists!")
 
-        assert_equal(self.engine.prepare(), 0)
+        assert self.engine.prepare() == 0
         for f in files:
             if not os.path.isfile(f):
                 raise AssertionError("File " + str(f) + " was not created!")
 
         for f in files:
             os.remove(f)
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_helpers.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,18 @@
 
     def generate_next_frame(self):
         self._current_snapshot = None
         return self.current_snapshot
 
 def raises_with_message_like(err, message=None):
     """
-    Decorator that allows to run nosetests with raises and testing if the message starts with a txt.
+    Decorator that allows to run tests with raises and testing if the
+    message starts with a txt.
+
+    TODO: this should be deprecated in favor of pytest functionality
 
     Notes
     -----
     We use this to check for abstract classes using
     >>> @raises_with_message_like(TypeError, "Can't instantiate abstract class")
     """
     def decorator(fnc):
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_histogram.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_histogram.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_interface_set.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_interface_set.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import absolute_import
 from builtins import zip
 from builtins import range
 from builtins import object
-from nose.tools import (assert_equal, assert_not_equal, assert_almost_equal,
-                        raises)
-from nose.plugins.skip import Skip, SkipTest
+
+import pytest
 from .test_helpers import (
     true_func, assert_equal_array_array, make_1d_traj, data_filename,
     assert_items_equal
 )
 
 import openpathsampling as paths
 from openpathsampling.high_level.interface_set import GenericVolumeInterfaceSet
@@ -31,80 +30,80 @@
                                                 self.lambdas)
         self.decreasing = paths.InterfaceSet(list(reversed(self.volumes)),
                                              self.cv,
                                              list(reversed(self.lambdas)))
         self.no_lambda_set = paths.InterfaceSet(self.volumes, self.cv)
 
     def test_direction(self):
-        assert_equal(self.interface_set.direction, 1)
-        assert_equal(self.no_lambda_set.direction, 0)
-        assert_equal(self.decreasing.direction, -1)
+        assert self.interface_set.direction == 1
+        assert self.no_lambda_set.direction == 0
+        assert self.decreasing.direction == -1
 
     def test_get_lambda(self):
         for (v, l) in zip(self.volumes, self.lambdas):
-            assert_equal(self.interface_set.get_lambda(v), l)
-            assert_equal(self.no_lambda_set.get_lambda(v), None)
+            assert self.interface_set.get_lambda(v) == l
+            assert self.no_lambda_set.get_lambda(v) is None
 
     def test_list_behavior(self):
         # len
-        assert_equal(len(self.interface_set), 4)
-        assert_equal(len(self.no_lambda_set), 4)
+        assert len(self.interface_set) == 4
+        assert len(self.no_lambda_set) == 4
         # getitem, contains
         for i in range(4):
-            assert_equal(self.volumes[i], self.interface_set[i])
-            assert_equal(self.volumes[i] in self.interface_set, True)
+            assert self.volumes[i] == self.interface_set[i]
+            assert self.volumes[i] in self.interface_set
         # getitem for slices
         sliced = self.interface_set[0:2]
         for vol in sliced:
-            assert_equal(sliced.get_lambda(vol),
-                         self.interface_set.get_lambda(vol))
+            assert (sliced.get_lambda(vol)
+                    == self.interface_set.get_lambda(vol))
         # special case of -1 needs to work (used frequently!)
-        assert_equal(self.volumes[-1], self.interface_set[-1])
+        assert self.volumes[-1] == self.interface_set[-1]
         # iter
         for vol in self.interface_set:
-            assert_equal(vol in self.volumes, True)
+            assert vol in self.volumes
         # reversed
         i = 0
         for vol in reversed(self.interface_set):
-            assert_equal(vol, self.volumes[3-i])
+            assert vol == self.volumes[3-i]
             i += 1
 
     def test_no_direction_possible(self):
         min_vals=[-0.1, -0.2, -0.3]
         max_vals=[0.1, 0.2, 0.3]
         volumes = [paths.CVDefinedVolume(self.cv, min_v, max_v)
                    for min_v, max_v in zip(min_vals, max_vals)]
         ifaces = paths.InterfaceSet(volumes)
-        assert_equal(ifaces.cv, None)
-        assert_equal(ifaces.cv_max, None)
-        assert_equal(ifaces.direction, 0)
+        assert ifaces.cv is None
+        assert ifaces.cv_max is None
+        assert ifaces.direction == 0
 
 
 class TestGenericVolumeInterfaceSet(object):
     def test_sanitize_input(self):
         # this is just to make the rest a little more readable
         sanitize = GenericVolumeInterfaceSet._sanitize_input
-        assert_equal(([float("-inf")]*3, [0.0, 0.1, 0.2], 1),
-                     sanitize(float("-inf"), [0.0, 0.1, 0.2]))
-        assert_equal(([0.2, 0.1, 0.0], [float("inf")]*3, -1),
-                     sanitize([0.2, 0.1, 0.0], float("inf")))
-        assert_equal(([-0.1, -0.2], [0.1, 0.2], 0),
-                     sanitize([-0.1, -0.2], [0.1, 0.2]))
-        assert_equal(([0.0, 0.0], [0.1, 0.2], 1),
-                     sanitize([0.0, 0.0], [0.1, 0.2]))
-        assert_equal(([-0.1, -0.2], [0.0, 0.0], -1),
-                     sanitize([-0.1, -0.2], [0.0, 0.0]))
+        assert (([float("-inf")]*3, [0.0, 0.1, 0.2], 1)
+                 == sanitize(float("-inf"), [0.0, 0.1, 0.2]))
+        assert (([0.2, 0.1, 0.0], [float("inf")]*3, -1)
+                 == sanitize([0.2, 0.1, 0.0], float("inf")))
+        assert (([-0.1, -0.2], [0.1, 0.2], 0)
+                 == sanitize([-0.1, -0.2], [0.1, 0.2]))
+        assert (([0.0, 0.0], [0.1, 0.2], 1)
+                 == sanitize([0.0, 0.0], [0.1, 0.2]))
+        assert (([-0.1, -0.2], [0.0, 0.0], -1)
+                 == sanitize([-0.1, -0.2], [0.0, 0.0]))
         # and the idiot case:
-        assert_equal(([-0.1, -0.1], [0.1, 0.1], 0),
-                     sanitize([-0.1, -0.1], [0.1, 0.1]))
+        assert (([-0.1, -0.1], [0.1, 0.1], 0)
+                 == sanitize([-0.1, -0.1], [0.1, 0.1]))
 
-    @raises(RuntimeError)
     def test_bad_sanitize(self):
-        GenericVolumeInterfaceSet._sanitize_input([0.0, -0.1],
-                                                  [0.1, 0.2, 0.3])
+        with pytest.raises(RuntimeError):
+            GenericVolumeInterfaceSet._sanitize_input([0.0, -0.1],
+                                                      [0.1, 0.2, 0.3])
 
 
 class TestVolumeInterfaceSet(object):
     def setup_method(self):
         paths.InterfaceSet._reset()
         self.cv = paths.FunctionCV(name="x", f=lambda s: s.xyz[0][0])
         self.increasing_set = paths.VolumeInterfaceSet(cv=self.cv,
@@ -114,39 +113,39 @@
                                                        minvals=[0.0, -0.1],
                                                        maxvals=float("inf"))
         self.weird_set = paths.VolumeInterfaceSet(cv=self.cv,
                                                   minvals=[-0.1, -0.2],
                                                   maxvals=[0.1, 0.2])
 
     def test_initialization(self):
-        assert_equal(len(paths.InterfaceSet._cv_max_dict), 1)
+        assert len(paths.InterfaceSet._cv_max_dict) == 1
         cv_max = list(paths.InterfaceSet._cv_max_dict.values())[0]
 
-        assert_equal(len(self.increasing_set), 2)
-        assert_equal(self.increasing_set.direction, 1)
-        assert_equal(self.increasing_set.lambdas, [0.0, 0.1])
-        assert_equal(self.increasing_set.cv_max, cv_max)
-
-        assert_equal(len(self.decreasing_set), 2)
-        assert_equal(self.decreasing_set.direction, -1)
-        assert_equal(self.decreasing_set.lambdas, [0.0, -0.1])
+        assert len(self.increasing_set) == 2
+        assert self.increasing_set.direction == 1
+        assert self.increasing_set.lambdas == [0.0, 0.1]
+        assert self.increasing_set.cv_max == cv_max
+
+        assert len(self.decreasing_set) == 2
+        assert self.decreasing_set.direction == -1
+        assert self.decreasing_set.lambdas == [0.0, -0.1]
         # TODO: decide what to do about cv_max for decreasing/weird
 
-        assert_equal(len(self.weird_set), 2)
-        assert_equal(self.weird_set.direction, 0)
-        assert_equal(self.weird_set.lambdas, None)
+        assert len(self.weird_set) == 2
+        assert self.weird_set.direction == 0
+        assert self.weird_set.lambdas is None
 
     def test_new_interface(self):
         new_iface = self.increasing_set.new_interface(0.25)
         expected = paths.CVDefinedVolume(self.cv, float("-inf"), 0.25)
-        assert_equal(expected, new_iface)
+        assert expected == new_iface
 
-    @raises(TypeError)
     def test_bad_new_interface(self):
-        self.weird_set.new_interface(0.25)
+        with pytest.raises(TypeError):
+            self.weird_set.new_interface(0.25)
 
     def test_storage(self):
         import os
         fname = data_filename("interface_set_storage_test.nc")
         if os.path.isfile(fname):
             os.remove(fname)
         template_traj = make_1d_traj([0.0])
@@ -157,18 +156,18 @@
         storage_w.close()
 
         storage_r = paths.AnalysisStorage(fname)
         reloaded = storage_r.interfacesets[0]
 
         assert_items_equal(reloaded.lambdas, self.increasing_set.lambdas)
         for (truth, beauty) in zip(self.increasing_set, reloaded):
-            assert_equal(truth, beauty)
+            assert truth == beauty
 
         for (v, l) in zip(reloaded.volumes, reloaded.lambdas):
-            assert_equal(reloaded.get_lambda(v), l)
+            assert reloaded.get_lambda(v) == l
 
         if os.path.isfile(fname):
             os.remove(fname)
 
 
 class TestPeriodicVolumeInterfaceSet(object):
     def setup_method(self):
@@ -179,22 +178,22 @@
             minvals=0.0,
             maxvals=[100, 150, 200-360],
             period_min=-180,
             period_max=180
         )
 
     def test_initialization(self):
-        assert_equal(self.increasing_set.direction, 1)
-        assert_equal(len(self.increasing_set), 3)
-        assert_equal(self.increasing_set.lambdas, [100, 150, -160])
+        assert self.increasing_set.direction == 1
+        assert len(self.increasing_set) == 3
+        assert self.increasing_set.lambdas == [100, 150, -160]
 
     def test_new_interface(self):
         new_iface = self.increasing_set.new_interface(-140)
         expected = paths.PeriodicCVDefinedVolume(self.cv, 0.0, -140, -180, 180)
-        assert_equal(new_iface, expected)
+        assert new_iface == expected
 
     def test_storage(self):
         import os
         fname = data_filename("interface_set_storage_test.nc")
         if os.path.isfile(fname):
             os.remove(fname)
         template_traj = make_1d_traj([0.0])
@@ -204,20 +203,20 @@
         storage_w.save(self.increasing_set)
         storage_w.sync_all()
 
         storage_r = paths.AnalysisStorage(fname)
         reloaded = storage_r.interfacesets[0]
 
         assert_items_equal(reloaded.lambdas, self.increasing_set.lambdas)
-        assert_equal(reloaded.period_min, self.increasing_set.period_min)
-        assert_equal(reloaded.period_max, self.increasing_set.period_max)
+        assert reloaded.period_min == self.increasing_set.period_min
+        assert reloaded.period_max == self.increasing_set.period_max
         for (truth, beauty) in zip(self.increasing_set, reloaded):
-            assert_equal(truth, beauty)
+            assert truth == beauty
 
         for (v, l) in zip(reloaded.volumes, reloaded.lambdas):
-            assert_equal(reloaded.get_lambda(v), l)
+            assert reloaded.get_lambda(v) == l
 
         storage_r.close()
         storage_w.close()
 
         if os.path.isfile(fname):
             os.remove(fname)
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_lookup_function.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_lookup_function.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import absolute_import
 from builtins import object
-from nose.tools import (assert_equal, assert_not_equal, assert_almost_equal,
-                        raises, assert_in)
-from nose.plugins.skip import SkipTest
 from numpy import isnan
+from numpy.testing import assert_almost_equal
 from .test_helpers import assert_items_almost_equal, assert_items_equal
 import collections
+import pytest
 
 import logging
 
 from openpathsampling.numerics import (
     LookupFunction, LookupFunctionGroup, VoxelLookupFunction
 )
 
@@ -80,61 +79,61 @@
                                        (-1,-1): 5.0})
         self.lookup = VoxelLookupFunction(left_bin_edges=(-1.0, 1.0),
                                           bin_widths=(0.5, 0.25),
                                           counter=counter)
 
     def test_keys(self):
         keys = [(0,0), (0,2), (1,4), (-1,-1)]
-        assert_equal(len(list(self.lookup.keys())), len(keys))
+        assert len(list(self.lookup.keys())) == len(keys)
         for key in list(self.lookup.keys()):
-            assert_in(key, keys)
+            assert key in keys
 
     def test_values(self):
         values = [1.0, 2.0, 4.0, 5.0]
-        assert_equal(len(list(self.lookup.values())), len(values))
+        assert len(list(self.lookup.values())) == len(values)
         for val in list(self.lookup.values()):
-            assert_in(val, values)
+            assert val in values
 
     def test_bin_to_left_edge(self):
         assert_items_equal(self.lookup.bin_to_left_edge((0,0)), (-1.0, 1.0))
         assert_items_equal(self.lookup.bin_to_left_edge((2,-1)), (0.0, 0.75))
 
     def test_val_to_bin(self):
         result_bin = self.lookup.val_to_bin((-0.25, 2.0))
-        assert_equal(len(result_bin), 2)
+        assert len(result_bin) == 2
         assert_items_equal(result_bin, [1.5, 4.0])
 
     def test_counter_by_bin_edges(self):
         bin_edge_counter = self.lookup.counter_by_bin_edges
         expected = {(-1.0, 1.0): 1.0, (-1.0,1.5): 2.0, (-0.5, 2.0): 4.0,
                     (-1.5, 0.75): 5.0}
-        assert_equal(len(expected), len(bin_edge_counter))
+        assert len(expected) == len(bin_edge_counter)
         for k in list(expected.keys()):
-            assert_equal(bin_edge_counter[k], expected[k])
+            assert bin_edge_counter[k] == expected[k]
 
     def test_df_2d(self):
         df1 = self.lookup.df_2d()
         assert_items_equal(df1.index, [-1, 0, 1])
         assert_items_equal(df1.columns, [-1, 0, 2, 4])
-        assert_equal(df1.at[-1, -1], 5.0)
-        assert_equal(isnan(df1.at[0, 4]), True)
+        assert df1.at[-1, -1] == 5.0
+        assert isnan(df1.at[0, 4])
 
         df2 = self.lookup.df_2d(x_range=(-1, 3), y_range=(-1, 4))
         assert_items_equal(df2.index, [-1, 0, 1, 2, 3])
         assert_items_equal(df2.columns, [-1, 0, 1, 2, 3, 4])
-        assert_equal(df2.at[-1, -1], 5.0)
-        assert_equal(isnan(df2.at[0, 4]), True)
-        assert_equal(isnan(df2.at[2, 3]), True)
+        assert df2.at[-1, -1] == 5.0
+        assert isnan(df2.at[0, 4])
+        assert isnan(df2.at[2, 3])
 
-    @raises(RuntimeError)
     def test_df_2d_not_2d(self):
         counter = collections.Counter({(0,0,0): 1.0})
         luf = VoxelLookupFunction(left_bin_edges=(0,0,0),
                                   bin_widths=(1,1,1),
                                   counter=counter)
-        luf.df_2d()
+        with pytest.raises(RuntimeError):
+            luf.df_2d()
 
     def test_call(self):
-        assert_equal(self.lookup((0.0, 0.0)), 0.0)   # no bin
-        assert_equal(self.lookup((-0.5, 2.0)), 4.0)  # bin edge
-        assert_equal(self.lookup((-0.4, 2.1)), 4.0)  # in bin
+        assert self.lookup((0.0, 0.0)) == 0.0   # no bin
+        assert self.lookup((-0.5, 2.0)) == 4.0  # bin edge
+        assert self.lookup((-0.4, 2.1)) == 4.0  # in bin
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_mdtraj_support.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_mdtraj_support.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from __future__ import absolute_import
 from builtins import object
 import logging
 
 import pytest
 
-from nose.tools import (
-    assert_equal, assert_not_equal, raises
-)
-from nose.plugins.skip import SkipTest
 import numpy.testing as nptest
 from .test_helpers import data_filename, assert_items_equal, md, u
 
 import openpathsampling as paths
 import numpy as np
 
 from openpathsampling.engines.openmm.tools import (
@@ -25,15 +21,15 @@
 
 # Includes tests of trajectory conversion to and from MDTraj; should also
 # add tests for topology conversions as well
 
 class TestMDTrajSupport(object):
     def setup_method(self):
         if not md:
-            raise SkipTest("mdtraj not installed")
+            pytest.skip("mdtraj not installed")
         self.md_trajectory = md.load(data_filename("ala_small_traj.pdb"))
         _ = pytest.importorskip("simtk.unit")
         self.ops_trajectory = trajectory_from_mdtraj(self.md_trajectory)
         self.md_topology = self.ops_trajectory.topology.mdtraj
 
     def test_trajectory_mdtraj_round_trip(self):
         # first test that the ops trajectory works
@@ -45,24 +41,24 @@
         # switch back to mdtraj
         md_trajectory_2 = trajectory_to_mdtraj(self.ops_trajectory,
                                                self.md_topology)
         nptest.assert_allclose(self.md_trajectory.xyz, md_trajectory_2.xyz)
         nptest.assert_allclose(self.md_trajectory.unitcell_vectors,
                                md_trajectory_2.unitcell_vectors)
 
-    @raises(ValueError)
     def test_empty_traj_to_mdtraj(self):
         empty = paths.Trajectory([])
-        empty.to_mdtraj()
+        with pytest.raises(ValueError):
+            empty.to_mdtraj()
 
     def test_trajectory_to_mdtraj_other_input(self):
         snap = self.ops_trajectory[0]
         md1 = trajectory_to_mdtraj(snap)
         md2 = trajectory_to_mdtraj([snap])
-        assert_equal(md1, md2)
+        assert md1 == md2
 
     def test_ops_load_trajectory_pdb(self):
         pdb_file = data_filename("ala_small_traj.pdb")
         ops_trajectory = ops_load_trajectory(pdb_file)
         # TODO: we should add tests to make sure this also works correctly
         # with other file formats (e.g., gromacs, where `top` kw is req'd)
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_movescheme.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_movescheme.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from __future__ import division
 from __future__ import print_function
 from __future__ import absolute_import
 from builtins import zip
 from builtins import range
 from builtins import object
 from past.utils import old_div
-from nose.tools import (assert_equal, assert_not_equal, assert_almost_equal,
-                        assert_in, raises, assert_is, assert_is_not,
-                        assert_true)
-from nose.plugins.skip import Skip, SkipTest
+from numpy.testing import assert_almost_equal
 from .test_helpers import (true_func, assert_equal_array_array,
                            make_1d_traj, assert_items_equal)
 
 import copy
 
 import math
 
@@ -410,77 +407,77 @@
         )
         self.scheme = MoveScheme(network)
 
     def test_append_individuals_default_levels(self):
         shootstrat = OneWayShootingStrategy()
         repexstrat = NearestNeighborRepExStrategy()
         defaultstrat = OrganizeByMoveGroupStrategy()
-        assert_equal(len(list(self.scheme.strategies.keys())), 0)
+        assert len(list(self.scheme.strategies.keys())) == 0
         self.scheme.append(shootstrat)
         self.scheme.append(repexstrat)
         self.scheme.append(defaultstrat)
 
         strats = self.scheme.strategies
-        assert_equal(len(list(strats.keys())), 3)
+        assert len(list(strats.keys())) == 3
         pairs = [(levels.MOVER, shootstrat), (levels.SIGNATURE, repexstrat),
                  (levels.GLOBAL, defaultstrat)]
         for (k, v) in pairs:
-            assert_in(v, strats[k])
+            assert v in strats[k]
 
     def test_append_groups_default_levels(self):
         shootstrat = OneWayShootingStrategy()
         repexstrat = NearestNeighborRepExStrategy()
         defaultstrat = OrganizeByMoveGroupStrategy()
-        assert_equal(len(list(self.scheme.strategies.keys())), 0)
+        assert len(list(self.scheme.strategies.keys())) == 0
         self.scheme.append([shootstrat, repexstrat, defaultstrat])
 
         strats = self.scheme.strategies
-        assert_equal(len(list(strats.keys())), 3)
+        assert len(list(strats.keys())) == 3
         pairs = [(levels.MOVER, shootstrat), (levels.SIGNATURE, repexstrat),
                  (levels.GLOBAL, defaultstrat)]
         for (k, v) in pairs:
-            assert_in(v, strats[k])
+            assert v in strats[k]
 
 
     def test_append_individuals_custom_levels(self):
         shootstrat = OneWayShootingStrategy()
         repexstrat = NearestNeighborRepExStrategy()
         defaultstrat = OrganizeByMoveGroupStrategy()
-        assert_equal(len(list(self.scheme.strategies.keys())), 0)
+        assert len(list(self.scheme.strategies.keys())) == 0
         self.scheme.append(shootstrat, 60)
         self.scheme.append(repexstrat, 60)
         self.scheme.append(defaultstrat, 60)
 
         strats = self.scheme.strategies
-        assert_equal(len(list(strats.keys())), 1)
+        assert len(list(strats.keys())) == 1
         assert_items_equal(strats[60], [shootstrat, repexstrat, defaultstrat])
 
     def test_append_groups_same_custom_level(self):
         shootstrat = OneWayShootingStrategy()
         repexstrat = NearestNeighborRepExStrategy()
         defaultstrat = OrganizeByMoveGroupStrategy()
-        assert_equal(len(list(self.scheme.strategies.keys())), 0)
+        assert len(list(self.scheme.strategies.keys())) == 0
         self.scheme.append([shootstrat, repexstrat, defaultstrat], 60)
 
         strats = self.scheme.strategies
-        assert_equal(len(list(strats.keys())), 1)
+        assert len(list(strats.keys())) == 1
         assert_items_equal(strats[60], [shootstrat, repexstrat, defaultstrat])
 
     def test_append_group_different_custom_levels(self):
         shootstrat = OneWayShootingStrategy()
         repexstrat = NearestNeighborRepExStrategy()
         defaultstrat = OrganizeByMoveGroupStrategy()
-        assert_equal(len(list(self.scheme.strategies.keys())), 0)
+        assert len(list(self.scheme.strategies.keys())) == 0
         self.scheme.append([shootstrat, repexstrat, defaultstrat],
                            [45, 55, 65])
 
         strats = self.scheme.strategies
-        assert_equal(len(list(strats.keys())), 3)
+        assert len(list(strats.keys())) == 3
         for (k, v) in [(45, shootstrat), (55, repexstrat), (65, defaultstrat)]:
-            assert_in(v, strats[k])
+            assert v in strats[k]
 
     def test_apply_strategy(self):
         if self.scheme.movers == {}:
             print("Full support of MoveStrategy implemented?")
             print("Time to remove legacy from tests.")
         else:
             self.scheme.movers = {}
@@ -496,188 +493,188 @@
             ),
             replace=False
         )
         shoot_strat_3 = OneWayShootingStrategy(replace=True)
 
         self.scheme.apply_strategy(shoot_strat_1)
         assert_items_equal(list(self.scheme.movers.keys()), ['shooting'])
-        assert_equal(len(self.scheme.movers['shooting']), 3)
+        assert len(self.scheme.movers['shooting']) == 3
 
         self.scheme.apply_strategy(shoot_strat_2)
         assert_items_equal(list(self.scheme.movers.keys()), ['shooting'])
-        assert_equal(len(self.scheme.movers['shooting']), 7)
+        assert len(self.scheme.movers['shooting']) == 7
         old_movers = copy.copy(self.scheme.movers['shooting'])
 
         self.scheme.apply_strategy(shoot_strat_3)
         assert_items_equal(list(self.scheme.movers.keys()), ['shooting'])
-        assert_equal(len(self.scheme.movers['shooting']), 7)
+        assert len(self.scheme.movers['shooting']) == 7
         new_movers = self.scheme.movers['shooting']
         for (o, n) in zip(old_movers, new_movers):
-            assert_equal(o is n, False)
+            assert o is not n
 
         shoot_strat_3.replace_signatures = True
         self.scheme.apply_strategy(shoot_strat_3)
-        assert_equal(len(self.scheme.movers['shooting']), 6)
+        assert len(self.scheme.movers['shooting']) == 6
 
         self.scheme.movers = {}
         shoot_strat_1.set_replace(True)
         self.scheme.apply_strategy(shoot_strat_1)
-        assert_equal(len(self.scheme.movers['shooting']), 3)
+        assert len(self.scheme.movers['shooting']) == 3
         old_movers = copy.copy(self.scheme.movers['shooting'])
 
         shoot_strat_3.replace_signatures = False
         self.scheme.apply_strategy(shoot_strat_3)
-        assert_equal(len(self.scheme.movers['shooting']), 6)
+        assert len(self.scheme.movers['shooting']) == 6
         new_movers = self.scheme.movers['shooting']
         for (o, n) in zip(old_movers, new_movers):
-            assert_equal(o is n, False)
+            assert o is not n
 
     def test_move_decision_tree(self):
         shoot = OneWayShootingStrategy()
         repex = NearestNeighborRepExStrategy()
         default = OrganizeByMoveGroupStrategy()
         self.scheme.append([default, shoot, repex])
 
-        assert_equal(self.scheme.root_mover, None)
+        assert self.scheme.root_mover is None
         root = self.scheme.move_decision_tree()
-        assert_not_equal(self.scheme.root_mover, None)
+        assert self.scheme.root_mover is not None
 
-        assert_equal(len(root.movers), 2)
+        assert len(root.movers) == 2
         names = ['ShootingChooser', 'RepexChooser']
         name_dict = {root.movers[i].name : i for i in range(len(root.movers))}
         for name in names:
-            assert_in(name, list(name_dict.keys()))
+            assert name in list(name_dict.keys())
 
-        assert_equal(len(root.movers[name_dict['ShootingChooser']].movers), 6)
-        assert_equal(len(root.movers[name_dict['RepexChooser']].movers), 4)
+        assert len(root.movers[name_dict['ShootingChooser']].movers) == 6
+        assert len(root.movers[name_dict['RepexChooser']].movers) == 4
 
         new_root = self.scheme.move_decision_tree()
-        assert_is(new_root, root)
+        assert new_root is root
 
         new_root = self.scheme.move_decision_tree(rebuild=True)
-        assert_is_not(new_root, root)
+        assert new_root is not root
 
     def test_repex_style_switching(self):
         nn_repex = NearestNeighborRepExStrategy()
         all_repex = AllSetRepExStrategy()
         default = OrganizeByMoveGroupStrategy()
 
         self.scheme.append([default, nn_repex])
         root = self.scheme.move_decision_tree(rebuild=True)
-        assert_equal(len(self.scheme.movers['repex']), 4)
+        assert len(self.scheme.movers['repex']) == 4
 
         self.scheme.append(all_repex, force=True)
         root = self.scheme.move_decision_tree(rebuild=True)
-        assert_equal(len(self.scheme.movers['repex']), 6)
+        assert len(self.scheme.movers['repex']) == 6
 
         self.scheme.append(nn_repex, force=True)
         root = self.scheme.move_decision_tree(rebuild=True)
-        assert_equal(len(self.scheme.movers['repex']), 4)
+        assert len(self.scheme.movers['repex']) == 4
 
     def test_build_balance_partners(self):
         ensA = self.scheme.network.sampling_transitions[0].ensembles[0]
         ensB = self.scheme.network.sampling_transitions[0].ensembles[1]
         hopAB = paths.EnsembleHopMover(ensemble=ensA, target_ensemble=ensB)
         hopBA = paths.EnsembleHopMover(ensemble=ensB, target_ensemble=ensA)
         self.scheme.movers['hop'] = [hopAB, hopBA]
         self.scheme.append(strategies.OrganizeByMoveGroupStrategy())
         root = self.scheme.move_decision_tree()
         self.scheme.build_balance_partners()
-        assert_equal(self.scheme.balance_partners[hopAB], [hopBA])
-        assert_equal(self.scheme.balance_partners[hopBA], [hopAB])
+        assert self.scheme.balance_partners[hopAB] == [hopBA]
+        assert self.scheme.balance_partners[hopBA] == [hopAB]
 
-    @raises(RuntimeWarning)
     def test_build_balance_partners_premature(self):
         self.scheme.movers = {}
-        self.scheme.build_balance_partners()
+        with pytest.raises(RuntimeWarning):
+            self.scheme.build_balance_partners()
 
-    @raises(RuntimeWarning)
     def test_build_balance_partners_no_partner(self):
         ensA = self.scheme.network.sampling_transitions[0].ensembles[0]
         ensB = self.scheme.network.sampling_transitions[0].ensembles[1]
         hopAB = paths.EnsembleHopMover(ensemble=ensA, target_ensemble=ensB)
         hopBA = paths.EnsembleHopMover(ensemble=ensB, target_ensemble=ensA)
         self.scheme.movers['hop'] = [hopAB]
         self.scheme.append(strategies.OrganizeByMoveGroupStrategy())
         root = self.scheme.move_decision_tree()
-        self.scheme.build_balance_partners()
+        with pytest.raises(RuntimeWarning):
+            self.scheme.build_balance_partners()
 
-    @raises(RuntimeWarning)
     def test_build_balance_partners_two_partners(self):
         ensA = self.scheme.network.sampling_transitions[0].ensembles[0]
         ensB = self.scheme.network.sampling_transitions[0].ensembles[1]
         hopAB = paths.EnsembleHopMover(ensemble=ensA, target_ensemble=ensB)
         hopAB2 = paths.EnsembleHopMover(ensemble=ensA, target_ensemble=ensB)
         hopBA = paths.EnsembleHopMover(ensemble=ensB, target_ensemble=ensA)
         self.scheme.movers['hop'] = [hopAB, hopBA, hopAB2]
         self.scheme.append(strategies.OrganizeByMoveGroupStrategy())
         root = self.scheme.move_decision_tree()
-        self.scheme.build_balance_partners()
+        with pytest.raises(RuntimeWarning):
+            self.scheme.build_balance_partners()
 
     def test_sanity_check_sane(self):
         self.scheme.append([NearestNeighborRepExStrategy(),
                             OneWayShootingStrategy(),
                             OrganizeByMoveGroupStrategy()])
         root = self.scheme.move_decision_tree()
         self.scheme.sanity_check()
 
-    @raises(AssertionError)
     def test_sanity_check_unused_sampling(self):
         ensemble_subset = self.scheme.network.sampling_transitions[0].ensembles
         self.scheme.append([
             OneWayShootingStrategy(ensembles=ensemble_subset),
             OrganizeByMoveGroupStrategy()
         ])
         root = self.scheme.move_decision_tree()
-        self.scheme.sanity_check()
+        with pytest.raises(AssertionError):
+            self.scheme.sanity_check()
 
-    @raises(AssertionError)
     def test_sanity_check_choice_prob_fails(self):
         self.scheme.append([NearestNeighborRepExStrategy(),
                             OneWayShootingStrategy(),
                             OrganizeByMoveGroupStrategy()])
         root = self.scheme.move_decision_tree()
         key0 = list(self.scheme.choice_probability.keys())[0]
         self.scheme.choice_probability[key0] = 0.0
-        self.scheme.sanity_check()
+        with pytest.raises(AssertionError):
+            self.scheme.sanity_check()
 
-    @raises(AssertionError)
     def test_sanity_check_duplicated_movers(self):
         ensemble_subset = self.scheme.network.sampling_transitions[0].ensembles
         self.scheme.append([
             OneWayShootingStrategy(),
             OrganizeByMoveGroupStrategy()
         ])
         root = self.scheme.move_decision_tree()
         self.scheme.movers['foo'] = [self.scheme.movers['shooting'][0]]
-        self.scheme.sanity_check()
+        with pytest.raises(AssertionError):
+            self.scheme.sanity_check()
 
-    @raises(TypeError)
     def test_select_movers_no_choice_probability(self):
         self.scheme.append([OneWayShootingStrategy(),
                             OrganizeByMoveGroupStrategy()])
-        movers = self.scheme._select_movers('shooting')
+        with pytest.raises(TypeError):
+            movers = self.scheme._select_movers('shooting')
 
     def test_select_movers(self):
         self.scheme.append([
             OneWayShootingStrategy(),
             NearestNeighborRepExStrategy(),
             OrganizeByMoveGroupStrategy()
         ])
         root = self.scheme.move_decision_tree()
         some_shooters = self.scheme.movers['shooting'][0:2]
 
         movers = self.scheme._select_movers('shooting')
-        assert_equal(movers, self.scheme.movers['shooting'])
+        assert movers == self.scheme.movers['shooting']
 
         movers = self.scheme._select_movers(some_shooters)
-        assert_equal(movers, some_shooters)
+        assert movers == some_shooters
 
         movers = self.scheme._select_movers(some_shooters[0])
-        assert_equal(movers, [some_shooters[0]])
+        assert movers == [some_shooters[0]]
 
     def test_n_trials_for_steps(self):
         self.scheme.append([
             OneWayShootingStrategy(),
             NearestNeighborRepExStrategy(),
             OrganizeByMoveGroupStrategy()
         ])
@@ -756,102 +753,87 @@
             'ShootingChooser' : paths.OneWayShootingMover,
             'PathreversalChooser' : paths.PathReversalMover,
             'RepexChooser' : paths.ReplicaExchangeMover,
             'MinusChooser' : paths.MinusMover,
             'Ms_outer_shootingChooser' : paths.OneWayShootingMover
         }
         names = list(chooser_type_dict.keys())
-        assert_equal(len(root.movers), len(names))
+        assert len(root.movers) == len(names)
 
         name_dict = {root.movers[i].name : i for i in range(len(root.movers))}
         for name in names:
-            assert_in(name, list(name_dict.keys()))
+            assert name in list(name_dict.keys())
 
         n_normal_repex = 4
         n_msouter_repex = 2
         n_repex = n_normal_repex + n_msouter_repex
 
-        assert_equal(
-            len(root.movers[name_dict['ShootingChooser']].movers), 6
-        )
-        assert_equal(
-            len(root.movers[name_dict['PathreversalChooser']].movers), 7
-        )
-        assert_equal(
-            len(root.movers[name_dict['RepexChooser']].movers), n_repex
-        )
-        assert_equal(
-            len(root.movers[name_dict['MinusChooser']].movers), 2
-        )
-        assert_equal(
-            len(root.movers[name_dict['Ms_outer_shootingChooser']].movers), 1
+        assert len(root.movers[name_dict['ShootingChooser']].movers) == 6
+        assert len(root.movers[name_dict['PathreversalChooser']].movers) == 7
+        assert len(root.movers[name_dict['RepexChooser']].movers) == n_repex
+        assert len(root.movers[name_dict['MinusChooser']].movers) == 2
+        assert (
+            len(root.movers[name_dict['Ms_outer_shootingChooser']].movers)
+            == 1
         )
 
         for choosername in names:
             for mover in root.movers[name_dict[choosername]].movers:
-                assert_equal(type(mover), chooser_type_dict[choosername])
+                assert type(mover) == chooser_type_dict[choosername]
 
     def test_default_scheme_no_ms_outer(self):
         scheme = DefaultScheme(self.no_ms_outer)
         root = scheme.move_decision_tree()
         chooser_type_dict = {
             'ShootingChooser' : paths.OneWayShootingMover,
             'PathreversalChooser' : paths.PathReversalMover,
             'RepexChooser' : paths.ReplicaExchangeMover,
             'MinusChooser' : paths.MinusMover
         }
         names = list(chooser_type_dict.keys())
-        assert_equal(len(root.movers), len(names))
+        assert len(root.movers) == len(names)
 
         name_dict = {root.movers[i].name : i for i in range(len(root.movers))}
         for name in names:
-            assert_in(name, list(name_dict.keys()))
+            assert name in list(name_dict.keys())
 
         n_normal_repex = 4
         n_msouter_repex = 0
         n_repex = n_normal_repex + n_msouter_repex
 
-        assert_equal(
-            len(root.movers[name_dict['ShootingChooser']].movers), 6
-        )
-        assert_equal(
-            len(root.movers[name_dict['PathreversalChooser']].movers), 6
-        )
-        assert_equal(
-            len(root.movers[name_dict['RepexChooser']].movers), n_repex
-        )
-        assert_equal(
-            len(root.movers[name_dict['MinusChooser']].movers), 2
-        )
+        assert len(root.movers[name_dict['ShootingChooser']].movers) == 6
+        assert len(root.movers[name_dict['PathreversalChooser']].movers) == 6
+        assert len(root.movers[name_dict['RepexChooser']].movers) == n_repex
+        assert len(root.movers[name_dict['MinusChooser']].movers) == 2
 
     def test_default_sanity(self):
         scheme = DefaultScheme(self.network)
         root = scheme.move_decision_tree()
         scheme.sanity_check()
 
     def test_default_hidden_ensembles(self):
         scheme = DefaultScheme(self.network)
         root = scheme.move_decision_tree()
         hidden = scheme.find_hidden_ensembles()
-        assert_equal(len(hidden), 2)
+        assert len(hidden) == 2
 
     def test_default_unused_ensembles(self):
         scheme = DefaultScheme(self.network)
         root = scheme.move_decision_tree()
         unused = scheme.find_unused_ensembles()
-        assert_equal(len(unused), 0) # will change when minus/msouter
+        assert len(unused) == 0  # will change when minus/msouter
 
     def test_default_balance_partners(self):
         scheme = DefaultScheme(self.network)
         root = scheme.move_decision_tree()
         scheme.build_balance_partners()
         # by default, every mover is its own balance partner
         for group in list(scheme.movers.values()):
             for mover in group:
-                assert_equal(scheme.balance_partners[mover], [mover])
+                assert scheme.balance_partners[mover] == [mover]
 
     def test_default_choice_probability(self):
         scheme = DefaultScheme(self.network)
         root = scheme.move_decision_tree()
         default_group_weights = {
             'shooting' : 1.0,
             'repex' : 0.5,
@@ -874,15 +856,15 @@
             for mover in scheme.movers[group]:
                 test_prob = scheme.choice_probability[mover]
                 assert_almost_equal(expected_prob, test_prob)
 
     def test_initial_conditions_from_trajectory(self):
         scheme = DefaultScheme(self.network)
         # root = scheme.move_decision_tree()
-        assert_equal(len(scheme.list_initial_ensembles()), 9)
+        assert len(scheme.list_initial_ensembles()) == 9
 
         traj1 = make_1d_traj([-0.6, -0.2, -0.6])
         traj2 = make_1d_traj([-0.6, -0.2, -0.05, -0.4, -0.6])
         traj3 = make_1d_traj([-0.6, -0.2, 0.2, 0.6])
 
         all_trajs = [traj1, traj2, traj3]
 
@@ -893,20 +875,20 @@
         def assert_init_cond(sample_set, ensembles, expected):
             # helper to check the results. Expected is in the form
             # of a list of resulting trajectories
             # ens is the list of ensembles to be tested in order
 
             sample_set.sanity_check()
 
-            assert_equal(len(sample_set), len(expected))
+            assert len(sample_set) == len(expected)
 
             for ensemble, traj in zip(ensembles, expected):
                 # print ensemble.name, sample_set[ensemble].trajectory.xyz[:,0,0], traj.xyz[:, 0,0],
                 # print hex(id(traj)), hex(id(sample_set[ensemble].trajectory.xyz[:,0,0]))
-                assert_equal(sample_set[ensemble].trajectory, traj)
+                assert sample_set[ensemble].trajectory == traj
 
         transAB = transBA = None
         for trans in self.network.sampling_transitions:
             if trans.stateA == self.stateA and trans.stateB == self.stateB:
                 transAB = trans
             elif trans.stateA == self.stateB and trans.stateB == self.stateA:
                 transBA = trans
@@ -970,48 +952,48 @@
             trajectories=all_trajs,
             preconditions=['mirror'],
             reuse_strategy='avoid',
             strategies=['get']
         )
 
         init_cond.sanity_check()
-        assert_equal(len(init_cond), 7)
+        assert len(init_cond) == 7
 
         for ensemble, traj in zip(ensembles[:3], [traj1, traj2, traj3]):
-            assert_equal(init_cond[ensemble].trajectory, traj)
+            assert init_cond[ensemble].trajectory == traj
         for ensemble, traj in zip(ensembles[4:], [traj3r] * 3):
-            assert_equal(init_cond[ensemble].trajectory, traj)
+            assert init_cond[ensemble].trajectory == traj
 
         # because of the way the scheme ensembles are creating involving a
         # set, the order in which the ensemble are created changes.
         # in some cases traj3 is used and hence avoided in the outer
         # in some cases traj3r, but both are fine.
         try:
-            assert_equal(init_cond[ensembles[3]].trajectory, traj3)
+            assert init_cond[ensembles[3]].trajectory == traj3
         except AssertionError:
-            assert_equal(init_cond[ensembles[3]].trajectory, traj3r)
+            assert init_cond[ensembles[3]].trajectory == traj3r
 
         init_cond = scheme.initial_conditions_from_trajectories(
             trajectories=all_trajs,
             preconditions=['mirror', 'sort-shortest'],
             reuse_strategy='avoid',
             strategies=['get']
         )
         init_cond.sanity_check()
-        assert_equal(len(init_cond), 7)
+        assert len(init_cond) == 7
 
         for ensemble, traj in zip(ensembles[:3], [traj1, traj1r, traj3]):
-            assert_equal(init_cond[ensemble].trajectory, traj)
+            assert init_cond[ensemble].trajectory == traj
         for ensemble, traj in zip(ensembles[4:], [traj3r] * 3):
-            assert_equal(init_cond[ensemble].trajectory, traj)
+            assert init_cond[ensemble].trajectory == traj
 
         try:
-            assert_equal(init_cond[ensembles[3]].trajectory, traj3)
+            assert init_cond[ensembles[3]].trajectory == traj3
         except AssertionError:
-            assert_equal(init_cond[ensembles[3]].trajectory, traj3r)
+            assert init_cond[ensembles[3]].trajectory == traj3r
 
         # this one avoids reversed copies
         init_cond = scheme.initial_conditions_from_trajectories(
             trajectories=[traj1],
             preconditions=[],
             strategies=['get']
         )
@@ -1057,41 +1039,41 @@
         )
 
     def test_check_initial_conditions(self):
         scheme = DefaultScheme(self.network)
         traj3 = make_1d_traj([-0.6, -0.2, 0.2, 0.6])
         # cheating a bit, since we know what this gives
         init_cond = scheme.initial_conditions_from_trajectories(traj3)
-        assert_equal(len(init_cond), 7)
-        assert_equal(len(scheme.list_initial_ensembles()), 9)
+        assert len(init_cond) == 7
+        assert len(scheme.list_initial_ensembles()) == 9
         (missing, extra) = scheme.check_initial_conditions(init_cond)
-        assert_equal(len(missing), 2)
-        assert_equal(len(extra), 0)
+        assert len(missing) == 2
+        assert len(extra) == 0
         for ens in list(self.network.special_ensembles['minus'].keys()):
-            assert_in([ens], missing)
+            assert [ens] in missing
         init_cond.append_as_new_replica(
             paths.Sample(trajectory=traj3,
                          ensemble=paths.LengthEnsemble(4),
                          replica=None)
         )
         (missing, extra) = scheme.check_initial_conditions(init_cond)
-        assert_equal(len(missing), 2)
-        assert_equal(len(extra), 1)
+        assert len(missing) == 2
+        assert len(extra) == 1
 
-    @raises(AssertionError)
     def test_assert_initial_conditions(self):
         scheme = DefaultScheme(self.network)
         traj3 = make_1d_traj([-0.6, -0.2, 0.2, 0.6])
         init_cond = scheme.initial_conditions_from_trajectories(traj3)
         init_cond.append_as_new_replica(
             paths.Sample(trajectory=traj3,
                          ensemble=paths.LengthEnsemble(4),
                          replica=None)
         )
-        scheme.assert_initial_conditions(init_cond)
+        with pytest.raises(AssertionError):
+            scheme.assert_initial_conditions(init_cond)
 
     def test_initial_conditions_report(self):
         scheme = DefaultScheme(self.network)
         traj3 = make_1d_traj([-0.6, -0.2, 0.2, 0.6])
         init_cond = scheme.initial_conditions_from_trajectories(traj3)
         init_cond.append_as_new_replica(
             paths.Sample(trajectory=traj3,
@@ -1102,17 +1084,17 @@
         missing_A = "*  [Out A minus]\n"
         missing_B = "*  [Out B minus]\n"
         finish = "Extra ensembles:\n*  [LengthEnsemble]\n"
         expected_AB = start + missing_A + missing_B + finish
         expected_BA = start + missing_B + missing_A + finish
         result = scheme.initial_conditions_report(init_cond)
         try:
-            assert_equal(result, expected_AB)
+            assert result == expected_AB
         except AssertionError:
-            assert_equal(result, expected_BA)
+            assert result == expected_BA
 
 
 class TestLockedMoveScheme(object):
     def setup_method(self):
         paths.InterfaceSet._reset()
         cvA = paths.FunctionCV(name="xA", f=lambda s : s.xyz[0][0])
         cvB = paths.FunctionCV(name="xB", f=lambda s : -s.xyz[0][0])
@@ -1130,47 +1112,47 @@
             )
         )
         self.basic_scheme = DefaultScheme(self.network)
         self.root_mover = self.basic_scheme.move_decision_tree()
 
     def test_initialization(self):
         scheme = LockedMoveScheme(self.root_mover, self.network)
-        assert_equal(scheme.network, self.network)
-        assert_equal(scheme.move_decision_tree(), self.root_mover)
+        assert scheme.network == self.network
+        assert scheme.move_decision_tree() == self.root_mover
 
     def test_build_move_decision_tree(self):
         scheme = LockedMoveScheme(self.root_mover, self.network)
         scheme.move_decision_tree(rebuild=True)
-        assert_equal(scheme.move_decision_tree(), self.root_mover)
+        assert scheme.move_decision_tree() == self.root_mover
 
-    @raises(TypeError)
     def test_append(self):
         scheme = LockedMoveScheme(self.root_mover, self.network)
-        scheme.append(AllSetRepExStrategy())
+        with pytest.raises(TypeError):
+            scheme.append(AllSetRepExStrategy())
 
-    @raises(TypeError)
     def test_apply_strategy(self):
         scheme = LockedMoveScheme(self.root_mover, self.network)
         strategy = AllSetRepExStrategy()
-        scheme.apply_strategy(strategy)
+        with pytest.raises(TypeError):
+            scheme.apply_strategy(strategy)
 
-    @raises(AttributeError)
     def test_choice_probability_fail(self):
         scheme = LockedMoveScheme(self.root_mover, self.network)
-        vals = scheme.choice_probability
+        with pytest.raises(AttributeError):
+            vals = scheme.choice_probability
 
     def test_choice_probability_works(self):
         scheme = LockedMoveScheme(self.root_mover, self.network)
         scheme.choice_probability = self.basic_scheme.choice_probability
         vals = scheme.choice_probability
 
-    @raises(AttributeError)
     def test_movers_fail(self):
         scheme = LockedMoveScheme(self.root_mover, self.network)
-        vals = scheme.movers
+        with pytest.raises(AttributeError):
+            vals = scheme.movers
 
     def test_movers_works(self):
         scheme = LockedMoveScheme(self.root_mover, self.network)
         scheme.movers = self.basic_scheme.movers
         vals = scheme.movers
 
 
@@ -1192,33 +1174,33 @@
                 {interfacesA: 0.0, interfacesB: 0.0}
             )
         )
 
     def test_scheme(self):
         scheme = OneWayShootingMoveScheme(self.network)
         root = scheme.move_decision_tree()
-        assert_equal(len(scheme.movers), 1)
-        assert_equal(len(root.movers), 1)
+        assert len(scheme.movers) == 1
+        assert len(root.movers) == 1
 
     def test_sanity(self):
         scheme = OneWayShootingMoveScheme(self.network)
         root = scheme.move_decision_tree()
         scheme.sanity_check()
 
     def test_unused_ensembles(self):
         scheme = OneWayShootingMoveScheme(self.network)
         root = scheme.move_decision_tree()
         unused = scheme.find_unused_ensembles()
         specials = self.network.special_ensembles
         expected_unused = sum([list(specials[special_type].keys())
                                for special_type in specials], [])
-        assert_equal(set(expected_unused), set(unused))
+        assert set(expected_unused) == set(unused)
 
     def test_check_initial_conditions(self):
         scheme = OneWayShootingMoveScheme(self.network)
         traj3 = make_1d_traj([-0.6, -0.2, 0.2, 0.6])
         init_cond = scheme.initial_conditions_from_trajectories(traj3)
-        assert_equal(len(scheme.list_initial_ensembles()), 6)
-        assert_equal(len(init_cond), 6)
+        assert len(scheme.list_initial_ensembles()) == 6
+        assert len(init_cond) == 6
         scheme.assert_initial_conditions(init_cond)
-        assert_equal(scheme.initial_conditions_report(init_cond),
-                     "No missing ensembles.\nNo extra ensembles.\n")
+        assert (scheme.initial_conditions_report(init_cond)
+                == "No missing ensembles.\nNo extra ensembles.\n")
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_movestrategy.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_movestrategy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from __future__ import division
 from __future__ import print_function
 from __future__ import absolute_import
 from builtins import zip
 from builtins import range
 from past.utils import old_div
 from builtins import object
-from nose.tools import (assert_equal, assert_not_equal, assert_almost_equal,
-                        raises, assert_in, assert_not_in)
-from nose.plugins.skip import Skip, SkipTest
+from numpy.testing import assert_almost_equal
 from .test_helpers import (
     true_func, assert_equal_array_array, make_1d_traj, MoverWithSignature,
     setify_ensemble_signature, reorder_ensemble_signature
 )
 import pytest
 
 import openpathsampling as paths
@@ -42,21 +40,21 @@
         if m.ensemble_signature_set == (set(sig[0]), set(sig[1])):
             mover = m
     return mover
 
 
 class TestStrategyLevels(object):
     def test_level_type(self):
-        assert_equal(levels.level_type(10), levels.SIGNATURE)
-        assert_equal(levels.level_type(1), levels.SIGNATURE)
-        assert_equal(levels.level_type(19), levels.SIGNATURE)
-        assert_equal(levels.level_type(20), None)
-        assert_equal(levels.level_type(21), levels.MOVER)
-        assert_equal(levels.level_type(35), levels.MOVER)
-        assert_equal(levels.level_type(100), levels.GLOBAL)
+        assert levels.level_type(10) == levels.SIGNATURE
+        assert levels.level_type(1) == levels.SIGNATURE
+        assert levels.level_type(19) == levels.SIGNATURE
+        assert levels.level_type(20) is None
+        assert levels.level_type(21) == levels.MOVER
+        assert levels.level_type(35) == levels.MOVER
+        assert levels.level_type(100) == levels.GLOBAL
 
 
 class MoveStrategyTestSetup(object):
     def setup_method(self):
         paths.InterfaceSet._reset()
         cvA = paths.FunctionCV(name="xA", f=lambda s: s.xyz[0][0])
         cvB = paths.FunctionCV(name="xB", f=lambda s: -s.xyz[0][0])
@@ -74,59 +72,59 @@
             )
         )
 
 
 class TestMoveStrategy(MoveStrategyTestSetup):
     def test_levels(self):
         strategy = MockMoveStrategy(ensembles=None, group="test", replace=True)
-        assert_equal(strategy.level, -1)
-        assert_equal(strategy.replace_signatures, False)
-        assert_equal(strategy.replace_movers, False)
+        assert strategy.level == -1
+        assert strategy.replace_signatures is False
+        assert strategy.replace_movers is False
         strategy.level = 10
-        assert_equal(strategy.level, levels.SIGNATURE)
-        assert_equal(strategy.replace_signatures, True)
-        assert_equal(strategy.replace_movers, False)
+        assert strategy.level == levels.SIGNATURE
+        assert strategy.replace_signatures
+        assert not strategy.replace_movers
         strategy.level = 25
-        assert_not_equal(strategy.level, levels.MOVER)
-        assert_equal(levels.level_type(strategy.level), levels.MOVER)
-        assert_equal(strategy.replace_signatures, False)
-        assert_equal(strategy.replace_movers, True)
+        assert strategy.level != levels.MOVER
+        assert levels.level_type(strategy.level) == levels.MOVER
+        assert not strategy.replace_signatures
+        assert strategy.replace_movers
         strategy.level = 99
-        assert_equal(strategy.replace_signatures, False)
-        assert_equal(strategy.replace_movers, False)
+        assert not strategy.replace_signatures
+        assert not strategy.replace_movers
 
     def test_get_ensembles(self):
         self.strategy = MockMoveStrategy(ensembles=None, group="test",
                                          replace=True)
         scheme = MoveScheme(self.network)
         # load up the relevant ensembles to test against
         transition_ensembles = []
         for transition in self.network.sampling_transitions:
             transition_ensembles.append(transition.ensembles)
-        assert_equal(len(transition_ensembles), 2)
+        assert len(transition_ensembles) == 2
         for ens_set in transition_ensembles:
-            assert_equal(len(ens_set), 3)
+            assert len(ens_set) == 3
         ensA = self.network.from_state[self.stateA].ensembles
-        assert_equal(len(ensA), 3)
+        assert len(ensA) == 3
         # if you error before this, something is wrong in setup
         ensembles = self.strategy.get_ensembles(scheme, None)
-        assert_equal(ensembles, transition_ensembles)
+        assert ensembles == transition_ensembles
 
         ensembles = self.strategy.get_ensembles(scheme, ensA)
-        assert_equal(ensembles, [ensA])
+        assert ensembles == [ensA]
 
         extra_ens = transition_ensembles[1][0]
         weird_ens_list = [[ensA[0]], ensA[1], [extra_ens]]
         ensembles = self.strategy.get_ensembles(scheme, weird_ens_list)
-        assert_equal(ensembles, [[ensA[0]], [ensA[1]], [extra_ens]])
+        assert ensembles == [[ensA[0]], [ensA[1]], [extra_ens]]
 
         ensembles = self.strategy.get_ensembles(scheme, extra_ens)
-        assert_equal(len(ensembles), 1)
-        assert_equal(len(ensembles[0]), 1)
-        assert_equal(ensembles[0][0], extra_ens)
+        assert len(ensembles) == 1
+        assert len(ensembles[0]) == 1
+        assert ensembles[0][0] == extra_ens
 
 
 class TestSingleEnsembleMoveStrategy(MoveStrategyTestSetup):
     def setup_method(self):
         super(TestSingleEnsembleMoveStrategy, self).setup_method()
         self.strategy = MockSingleEnsembleMoveStrategy(
             ensembles=None,
@@ -167,95 +165,95 @@
 
 
 class TestForwardShootingStrategy(MoveStrategyTestSetup):
     def test_make_movers(self):
         strategy = ForwardShootingStrategy()
         scheme = MoveScheme(self.network)
         movers = strategy.make_movers(scheme)
-        assert_equal(len(movers), 6)
+        assert len(movers) == 6
         for mover in movers:
-            assert_equal(type(mover), paths.ForwardShootMover)
-            assert_equal(type(mover.selector), paths.UniformSelector)
+            assert type(mover) == paths.ForwardShootMover
+            assert type(mover.selector) == paths.UniformSelector
 
     def test_make_movers_with_list(self):
         list_of_selectors = [
             paths.shooting.InterfaceConstrainedSelector(ens.interface)
             for ens in self.network.sampling_ensembles
         ]
         strategy = ForwardShootingStrategy(
             selector=list_of_selectors,
             ensembles=self.network.sampling_ensembles
         )
         scheme = MoveScheme(self.network)
         movers = strategy.make_movers(scheme)
-        assert_equal(len(movers), 6)
-        assert_equal(len(list_of_selectors), 6)
+        assert len(movers) == 6
+        assert len(list_of_selectors) == 6
         for mover, sel in zip(movers, list_of_selectors):
-            assert_equal(type(mover), paths.ForwardShootMover)
-            assert_equal(type(mover.selector),
-                         paths.shooting.InterfaceConstrainedSelector)
-            assert_equal(mover.selector, sel)
+            assert type(mover) == paths.ForwardShootMover
+            assert (type(mover.selector)
+                    == paths.shooting.InterfaceConstrainedSelector)
+            assert mover.selector == sel
 
 
 class TestOneWayShootingStrategy(MoveStrategyTestSetup):
     def test_make_movers(self):
         strategy = OneWayShootingStrategy()
         scheme = MoveScheme(self.network)
         movers = strategy.make_movers(scheme)
-        assert_equal(len(movers), 6)
+        assert len(movers) == 6
         for mover in movers:
-            assert_equal(type(mover), paths.OneWayShootingMover)
-            assert_equal(type(mover.selector), paths.UniformSelector)
+            assert type(mover) == paths.OneWayShootingMover
+            assert type(mover.selector) == paths.UniformSelector
 
 class TestTwoWayShootingStrategy(MoveStrategyTestSetup):
     def test_make_movers(self):
         strategy = TwoWayShootingStrategy(modifier=paths.NoModification())
         scheme = MoveScheme(self.network)
         movers = strategy.make_movers(scheme)
-        assert_equal(len(movers), 6)
+        assert len(movers) == 6
         for mover in movers:
-            assert_equal(type(mover), paths.TwoWayShootingMover)
-            assert_equal(type(mover.selector), paths.UniformSelector)
-            assert_equal(type(mover.modifier), paths.NoModification)
+            assert type(mover) == paths.TwoWayShootingMover
+            assert type(mover.selector) == paths.UniformSelector
+            assert type(mover.modifier) == paths.NoModification
 
     def test_composition_with_default_scheme(self):
         strategy = TwoWayShootingStrategy(modifier=paths.NoModification())
         scheme = DefaultScheme(self.network, engine=None)
         scheme.append(strategy)
         scheme.build_move_decision_tree()
-        assert_equal(len(scheme.movers['shooting']), 6)
+        assert len(scheme.movers['shooting']) == 6
         for mover in scheme.movers['shooting']:
-            assert_equal(type(mover), paths.TwoWayShootingMover)
-            assert_equal(type(mover.selector), paths.UniformSelector)
-            assert_equal(type(mover.modifier), paths.NoModification)
+            assert type(mover) == paths.TwoWayShootingMover
+            assert type(mover.selector) == paths.UniformSelector
+            assert type(mover.modifier) == paths.NoModification
 
 
 class TestNearestNeighborRepExStrategy(MoveStrategyTestSetup):
     def test_make_movers(self):
         strategy = NearestNeighborRepExStrategy()
         scheme = MoveScheme(self.network)
         movers = strategy.make_movers(scheme)
-        assert_equal(len(movers), 4)
+        assert len(movers) == 4
         ens0 = self.network.sampling_transitions[0].ensembles
         ens1 = self.network.sampling_transitions[1].ensembles
-        assert_equal(movers[0].ensemble_signature_set,
-                     (set([ens0[0], ens0[1]]), set([ens0[0], ens0[1]])))
-        assert_equal(movers[1].ensemble_signature_set,
-                     (set([ens0[1], ens0[2]]), set([ens0[1], ens0[2]])))
-        assert_equal(movers[2].ensemble_signature_set,
-                     (set([ens1[0], ens1[1]]), set([ens1[0], ens1[1]])))
-        assert_equal(movers[3].ensemble_signature_set,
-                     (set([ens1[1], ens1[2]]), set([ens1[1], ens1[2]])))
+        assert (movers[0].ensemble_signature_set
+                == (set([ens0[0], ens0[1]]), set([ens0[0], ens0[1]])))
+        assert (movers[1].ensemble_signature_set
+                == (set([ens0[1], ens0[2]]), set([ens0[1], ens0[2]])))
+        assert (movers[2].ensemble_signature_set
+                == (set([ens1[0], ens1[1]]), set([ens1[0], ens1[1]])))
+        assert (movers[3].ensemble_signature_set
+                == (set([ens1[1], ens1[2]]), set([ens1[1], ens1[2]])))
 
 class TestAllSetRepExStrategy(MoveStrategyTestSetup):
     def test_make_movers(self):
         strategy = AllSetRepExStrategy()
         scheme = MoveScheme(self.network)
         movers = strategy.make_movers(scheme)
-        assert_equal(len(movers), 6)
+        assert len(movers) == 6
         ens0 = self.network.sampling_transitions[0].ensembles
         ens1 = self.network.sampling_transitions[1].ensembles
 
         signatures = [(set(m.ensemble_signature[0]),
                        set(m.ensemble_signature[1])) for m in movers]
         expected_signatures = [
             ((ens0[0], ens0[1]), (ens0[0], ens0[1])),
@@ -263,303 +261,300 @@
             ((ens0[1], ens0[2]), (ens0[1], ens0[2])),
             ((ens1[0], ens1[1]), (ens1[0], ens1[1])),
             ((ens1[0], ens1[2]), (ens1[0], ens1[2])),
             ((ens1[1], ens1[2]), (ens1[1], ens1[2]))
         ]
         for sig in expected_signatures:
             set_sig = (set(sig[0]), set(sig[1]))
-            assert_in(set_sig, signatures)
+            assert set_sig in signatures
 
 class TestSelectedPairsRepExStrategy(MoveStrategyTestSetup):
     def test_make_movers(self):
         ens00 = self.network.sampling_transitions[0].ensembles[0]
         ens02 = self.network.sampling_transitions[0].ensembles[2]
         strategy = SelectedPairsRepExStrategy(ensembles=[ens00, ens02])
         scheme = MoveScheme(self.network)
         movers = strategy.make_movers(scheme)
-        assert_equal(len(movers), 1)
-        assert_equal(movers[0].ensemble_signature_set,
-                     ({ ens00, ens02 }, ({ ens00, ens02 })))
+        assert len(movers) == 1
+        assert (movers[0].ensemble_signature_set
+                == ({ ens00, ens02 }, ({ ens00, ens02 })))
 
-    @raises(RuntimeError)
     def test_init_ensembles_none(self):
-        strategy = SelectedPairsRepExStrategy()
+        with pytest.raises(RuntimeError):
+            strategy = SelectedPairsRepExStrategy()
 
-    @raises(RuntimeError)
     def test_init_ensembles_triplet(self):
         ensembles = self.network.sampling_transitions[0].ensembles
-        strategy = SelectedPairsRepExStrategy(ensembles=ensembles)
+        with pytest.raises(RuntimeError):
+            strategy = SelectedPairsRepExStrategy(ensembles=ensembles)
 
     def test_make_movers_multiple_pairs(self):
         ens00 = self.network.sampling_transitions[0].ensembles[0]
         ens01 = self.network.sampling_transitions[0].ensembles[1]
         ens02 = self.network.sampling_transitions[0].ensembles[2]
         strategy = SelectedPairsRepExStrategy(ensembles=[[ens00, ens01],
                                                          [ens00, ens02],
                                                          [ens01, ens02]])
         scheme = MoveScheme(self.network)
         movers = strategy.make_movers(scheme)
-        assert_equal(len(movers), 3)
-        assert_equal(movers[0].ensemble_signature_set,
-                     ({ens00, ens01}, {ens00, ens01}))
-        assert_equal(movers[1].ensemble_signature_set,
-                     ({ens00, ens02}, {ens00, ens02}))
-        assert_equal(movers[2].ensemble_signature_set,
-                     ({ens01, ens02}, {ens01, ens02}))
+        assert len(movers) == 3
+        assert (movers[0].ensemble_signature_set
+                == ({ens00, ens01}, {ens00, ens01}))
+        assert (movers[1].ensemble_signature_set
+                == ({ens00, ens02}, {ens00, ens02}))
+        assert (movers[2].ensemble_signature_set
+                == ({ens01, ens02}, {ens01, ens02}))
 
 class TestReplicaExchangeStrategy(MoveStrategyTestSetup):
     def test_make_movers(self):
         strategy = ReplicaExchangeStrategy()
         scheme = MoveScheme(self.network)
         scheme.apply_strategy(NearestNeighborRepExStrategy())
         movers = strategy.make_movers(scheme)
-        assert_equal(len(movers), 4)
+        assert len(movers) == 4
 
     def test_swap_to_hop_to_swap(self):
         scheme = DefaultScheme(self.network)
         root = scheme.move_decision_tree()
-        assert_equal(len(scheme.movers['repex']), 6)
+        assert len(scheme.movers['repex']) == 6
         old_movers = scheme.movers['repex']
         scheme.append(EnsembleHopStrategy(), force=True)
         root = scheme.move_decision_tree(rebuild=True)
-        assert_equal(len(scheme.movers['repex']), 12)
+        assert len(scheme.movers['repex']) == 12
         scheme.append(ReplicaExchangeStrategy(), force=True)
         root = scheme.move_decision_tree(rebuild=True)
-        assert_equal(len(scheme.movers['repex']), 6)
+        assert len(scheme.movers['repex']) == 6
         new_movers = scheme.movers['repex']
-        assert_not_equal(old_movers, new_movers)
+        assert old_movers != new_movers
         old_sigs = [m.ensemble_signature_set for m in old_movers]
         new_sigs = [m.ensemble_signature_set for m in new_movers]
         for old in old_sigs:
-            assert_in(old, new_sigs)
+            assert old in new_sigs
 
-    @raises(RuntimeError)
     def test_detailed_balance_partners(self):
         scheme = DefaultScheme(self.network)
         scheme.append(EnsembleHopStrategy(), force=True)
         root = scheme.move_decision_tree()
-        assert_equal(len(scheme.movers['repex']), 12)
+        assert len(scheme.movers['repex']) == 12
         scheme.movers['repex'].pop()
-        assert_equal(len(scheme.movers['repex']), 11)
+        assert len(scheme.movers['repex']) == 11
         strategy = ReplicaExchangeStrategy()
-        strategy.make_movers(scheme)
+        with pytest.raises(RuntimeError):
+            strategy.make_movers(scheme)
 
 
 class TestEnsembleHopStrategy(MoveStrategyTestSetup):
     def test_make_movers(self):
         strategy = EnsembleHopStrategy()
         scheme = MoveScheme(self.network)
         scheme.apply_strategy(NearestNeighborRepExStrategy())
         movers = strategy.make_movers(scheme)
         # defaults to 4 repex movers, so
-        assert_equal(len(movers), 8)
+        assert len(movers) == 8
 
         # set up the swap pairs
         swap_pairs = []
         for trans in self.network.sampling_transitions:
             swap_pairs.extend([[trans.ensembles[i], trans.ensembles[i+1]]
                                for i in range(len(trans.ensembles)-1)])
-        assert_equal(len(swap_pairs), 4)
+        assert len(swap_pairs) == 4
 
         # check that each swap pair has a hop
         mover_sigs = [m.ensemble_signature for m in movers]
         for pair in swap_pairs:
             sig1 = ((pair[0],),(pair[1],))
             sig2 = ((pair[1],),(pair[0],))
-            assert_in(sig1, mover_sigs)
-            assert_in(sig2, mover_sigs)
+            assert sig1 in mover_sigs
+            assert sig2 in mover_sigs
 
         scheme.movers['repex'] = movers
         newmovers = strategy.make_movers(scheme)
-        assert_equal(len(newmovers), 8)
+        assert len(newmovers) == 8
         for mover in newmovers:
-            assert_in(mover.ensemble_signature, mover_sigs)
+            assert mover.ensemble_signature in mover_sigs
 
-    @raises(RuntimeError)
     def test_different_number_input_output_ensembles(self):
         ens0 = self.network.sampling_ensembles[0]
         ens1 = self.network.sampling_ensembles[1]
         ens2 = self.network.sampling_ensembles[2]
         weird_mover = MoverWithSignature(
             input_ensembles=[ens0, ens1, ens2],
             output_ensembles=[ens0, ens1]
         )
-        assert_equal(weird_mover.ensemble_signature,
-                     ((ens0,ens1,ens2),(ens0,ens1)))
+        assert (weird_mover.ensemble_signature
+                == ((ens0,ens1,ens2),(ens0,ens1)))
         scheme = MoveScheme(self.network)
         scheme.movers['weird'] = [weird_mover]
         strategy = EnsembleHopStrategy(group='weird')
-        strategy.make_movers(scheme)
+        with pytest.raises(RuntimeError):
+            strategy.make_movers(scheme)
 
-    @raises(RuntimeError)
     def test_wrong_number_ensembles_in_signature(self):
         ens0 = self.network.sampling_ensembles[0]
         ens1 = self.network.sampling_ensembles[1]
         ens2 = self.network.sampling_ensembles[2]
         weird_mover = MoverWithSignature(
             input_ensembles=[ens0, ens1, ens2],
             output_ensembles=[ens0, ens1, ens2]
         )
-        assert_equal(weird_mover.ensemble_signature,
-                     ((ens0,ens1,ens2),(ens0,ens1,ens2)))
+        assert (weird_mover.ensemble_signature
+                == ((ens0,ens1,ens2),(ens0,ens1,ens2)))
         scheme = MoveScheme(self.network)
         scheme.movers['weird'] = [weird_mover]
         strategy = EnsembleHopStrategy(group='weird')
-        strategy.make_movers(scheme)
+        with pytest.raises(RuntimeError):
+            strategy.make_movers(scheme)
 
-    @raises(RuntimeError)
     def test_not_replica_exchange_signature(self):
         ens0 = self.network.sampling_ensembles[0]
         ens1 = self.network.sampling_ensembles[1]
         ens2 = self.network.sampling_ensembles[2]
         weird_mover = MoverWithSignature(
             input_ensembles=[ens0, ens1],
             output_ensembles=[ens1, ens2]
         )
-        assert_equal(weird_mover.ensemble_signature,
-                     ((ens0,ens1),(ens1,ens2)))
+        assert weird_mover.ensemble_signature == ((ens0,ens1),(ens1,ens2))
         scheme = MoveScheme(self.network)
         scheme.movers['weird'] = [weird_mover]
         strategy = EnsembleHopStrategy(group='weird')
-        strategy.make_movers(scheme)
+        with pytest.raises(RuntimeError):
+            strategy.make_movers(scheme)
 
     def test_replace_nofrom(self):
         # this is the default behavior
         scheme = DefaultScheme(self.network)
         scheme.movers ={}
         scheme.append(EnsembleHopStrategy(replace=True, from_group=None))
         scheme.build_move_decision_tree()
         # 4 normal repex + 2 ms-outer repex = 6 repex * 2 hop/repex = 12
-        assert_equal(len(scheme.movers['repex']), 12)
+        assert len(scheme.movers['repex']) == 12
 
     def test_noreplace_from(self):
         # if replace is False and from_group is given, we end up with two
         # groups: both the new and the old.
         scheme = DefaultScheme(self.network)
         scheme.movers ={}
         scheme.append(EnsembleHopStrategy(replace=False,
                                           group='hop',
                                           from_group='repex'))
         scheme.build_move_decision_tree()
-        assert_equal(len(scheme.movers['repex']), 6)
-        assert_equal(len(scheme.movers['hop']), 12)
+        assert len(scheme.movers['repex']) == 6
+        assert len(scheme.movers['hop']) == 12
 
     def test_replace_from(self):
         # if replace is True and we have a different from_group, we should
         # remove the old from_group from existence
         scheme = DefaultScheme(self.network)
         scheme.movers ={}
         scheme.append(EnsembleHopStrategy(replace=True,
                                           group='hop',
                                           from_group='repex'))
         scheme.build_move_decision_tree()
-        assert_equal(len(scheme.movers['hop']), 12)
-        assert_not_in("repex", list(scheme.movers.keys()))
+        assert len(scheme.movers['hop']) == 12
+        assert "repex" not in list(scheme.movers.keys())
 
     def test_noreplace_nofrom(self):
         # if replace==False and the from_group is not given, we should
         # act as mover replacement (but this is seriously a bad idea)
         scheme = DefaultScheme(self.network)
         scheme.movers ={}
         scheme.append(EnsembleHopStrategy(replace=False, from_group=None))
         scheme.build_move_decision_tree()
-        assert_equal(len(scheme.movers['repex']), 18)
+        assert len(scheme.movers['repex']) == 18
 
 
 class TestPathReversalStrategy(MoveStrategyTestSetup):
     def test_make_movers(self):
         strategy = PathReversalStrategy()
         scheme = MoveScheme(self.network)
         movers = strategy.make_movers(scheme)
-        assert_equal(len(movers), 6)
+        assert len(movers) == 6
         for m in movers:
-            assert_equal(type(m), paths.PathReversalMover)
+            assert type(m) == paths.PathReversalMover
 
 
 class TestMinusMoveStrategy(MoveStrategyTestSetup):
     def test_get_ensembles(self):
         strategy = MinusMoveStrategy()
         scheme = MoveScheme(self.network)
         ensembles = strategy.get_ensembles(scheme, None)
-        assert_equal(len(ensembles), 2)
+        assert len(ensembles) == 2
         for ens_group in ensembles:
-            assert_equal(len(ens_group), 1)
-        assert_not_equal(ensembles[0][0].state_vol, ensembles[1][0].state_vol)
+            assert len(ens_group) == 1
+        assert ensembles[0][0].state_vol != ensembles[1][0].state_vol
 
     def test_get_ensembles_multiple_minus(self):
         strategy = MinusMoveStrategy()
         innerA = self.network.sampling_transitions[0].ensembles[0]
         innerB = self.network.sampling_transitions[1].ensembles[0]
         inner_vol_A = self.network.sampling_transitions[0].interfaces[0]
         inner_vol_B = self.network.sampling_transitions[1].interfaces[0]
         extra_minus = paths.MinusInterfaceEnsemble(
             state_vol=self.network.sampling_transitions[0].stateA,
             innermost_vols=[inner_vol_A, inner_vol_B]
         )
         self.network.special_ensembles['minus'][extra_minus] = [innerA, innerB]
         scheme = MoveScheme(self.network)
         ensembles = strategy.get_ensembles(scheme, None)
-        assert_equal(len(ensembles), 2)
-        assert_equal({ len(ensembles[0]), len(ensembles[1]) }, { 1, 2 })
+        assert len(ensembles) == 2
+        assert { len(ensembles[0]), len(ensembles[1]) } == { 1, 2 }
 
     def test_get_ensembles_fixed_ensembles(self):
         strategy = MinusMoveStrategy()
         minusA = list(self.network.special_ensembles['minus'].keys())[0]
         scheme = MoveScheme(self.network)
         ensembles = strategy.get_ensembles(scheme, minusA)
-        assert_equal(len(ensembles), 1)
-        assert_equal(len(ensembles[0]), 1)
-        assert_equal(ensembles[0][0], minusA)
+        assert len(ensembles) == 1
+        assert len(ensembles[0]) == 1
+        assert ensembles[0][0] == minusA
 
     def test_make_movers(self):
         strategy = MinusMoveStrategy()
         scheme = MoveScheme(self.network)
         movers = strategy.make_movers(scheme)
-        assert_equal(len(movers), 2)
+        assert len(movers) == 2
 
         minuses = self.network.special_ensembles['minus']
         ens_minusA = list(minuses.keys())[0]
         ens_innerA = [t.ensembles[0] for t in minuses[ens_minusA]]
         sig_A = set([ens_minusA] + ens_innerA)
         ens_minusB = list(minuses.keys())[1]
         ens_innerB = [t.ensembles[0] for t in minuses[ens_minusB]]
         sig_B = set([ens_minusB] + ens_innerB)
         all_ens_sigs = [m.ensemble_signature_set for m in movers]
 
         # check the signatures
-        assert_not_equal(sig_A, sig_B)
-        assert_in(tuple([sig_A, sig_A]), all_ens_sigs)
-        assert_in(tuple([sig_B, sig_B]), all_ens_sigs)
+        assert sig_A != sig_B
+        assert tuple([sig_A, sig_A]) in all_ens_sigs
+        assert tuple([sig_B, sig_B]) in all_ens_sigs
 
         # check that these are inner ensembles
         inners = [t.ensembles[0] for t in self.network.sampling_transitions]
         for inner in ens_innerA + ens_innerB:
-            assert_in(inner, inners)
+            assert inner in inners
 
         # check that we've got the right inner for the right state
         stateA_inner = self.network.from_state[ens_minusA.state_vol].ensembles[0]
-        assert_equal([stateA_inner], ens_innerA)
+        assert [stateA_inner] == ens_innerA
         stateB_inner = self.network.from_state[ens_minusB.state_vol].ensembles[0]
-        assert_equal([stateB_inner], ens_innerB)
+        assert [stateB_inner] == ens_innerB
 
         # check that we've got minus ensembles
         for mover in movers:
-            assert_in(mover.minus_ensemble, self.network.minus_ensembles)
-            assert_equal(
-                isinstance(mover.minus_ensemble, paths.MinusInterfaceEnsemble),
-                True
-            )
+            assert mover.minus_ensemble in self.network.minus_ensembles
+            assert isinstance(mover.minus_ensemble,
+                              paths.MinusInterfaceEnsemble)
 
 
 class TestSingleReplicaMinusMoveStrategy(MoveStrategyTestSetup):
     def test_make_movers(self):
         strategy = SingleReplicaMinusMoveStrategy()
         scheme = MoveScheme(self.network)
         movers = strategy.make_movers(scheme)
-        assert_equal(len(movers), 2)
+        assert len(movers) == 2
 
         minuses = self.network.special_ensembles['minus']
         ens_minusA = list(minuses.keys())[0]
         ens_innerA = [t.ensembles[0] for t in minuses[ens_minusA]]
         sig_A = set([ens_minusA] + ens_innerA)
         ens_minusB = list(minuses.keys())[1]
         ens_innerB = [t.ensembles[0] for t in minuses[ens_minusB]]
@@ -599,20 +594,20 @@
         choice_prob = strategy.choice_probability(scheme, group_weights,
                                                   mover_weights)
         # shooting moves: P_a*P_b = 1.0*1.0 (3 times)
         # repex moves: P_a*P_b = 0.5*1.0 (2 times)
         # norm = 3*1.0 + 2*0.5 = 4.0
         # each shooting prob: 0.25
         # each repex prob: 0.125
-        assert_equal(len(choice_prob), len(sum(list(scheme.movers.values()), [])))
+        assert len(choice_prob) == len(sum(list(scheme.movers.values()), []))
         for m in list(choice_prob.keys()):
             if m in scheme.movers['shooting']:
-                assert_equal(choice_prob[m], 0.25)
+                assert choice_prob[m] == 0.25
             elif m in scheme.movers['repex']:
-                assert_equal(choice_prob[m], 0.125)
+                assert choice_prob[m] == 0.125
             else:
                 raise RuntimeError("Unknown mover "+repr(m))
 
         # now change the choice probability for one of them
         ens0_sig = ((ens0,),(ens0,))
         mover_weights[('shooting', ens0_sig)] = 2.0
         choice_prob = strategy.choice_probability(scheme, group_weights,
@@ -621,23 +616,22 @@
         # new norm: 2*1.0 + 1*2.0 + 2*0.5 = 5.0
         # prob shooting0 : 2.0/5.0 = 0.4
         # prob shooting1,2 : 1.0/5.0 = 0.2
         # prob repex: 0.5/5.0 = 0.1
         for m in list(choice_prob.keys()):
             if m in scheme.movers['shooting']:
                    if m.ensemble_signature == ens0_sig:
-                       assert_equal(choice_prob[m], 0.4)
+                       assert choice_prob[m] == 0.4
                    else:
-                       assert_equal(choice_prob[m], 0.2)
+                       assert choice_prob[m] == 0.2
             elif m in scheme.movers['repex']:
-                assert_equal(choice_prob[m], 0.1)
+                assert choice_prob[m] == 0.1
             else:
                 raise RuntimeError("Unknown mover "+repr(m))
 
-    @raises(KeyError)
     def test_choice_probability_bad_group_weights(self):
         scheme = MoveScheme(self.network)
         ens0 = self.network.sampling_transitions[0].ensembles[0]
         ens1 = self.network.sampling_transitions[0].ensembles[1]
         ens2 = self.network.sampling_transitions[0].ensembles[2]
         scheme.movers['shooting'] = [
             paths.OneWayShootingMover(
@@ -652,17 +646,18 @@
         ]
         strategy = OrganizeByMoveGroupStrategy()
         group_weights = {'shooting' : 1.0}
         mover_weights = {}
         for groupname in list(scheme.movers.keys()):
             for mover in scheme.movers[groupname]:
                 mover_weights[(groupname, mover.ensemble_signature)] = 1.0
-        assert_equal(len(mover_weights), 5)
-        choice_prob = strategy.choice_probability(scheme, group_weights,
-                                                  mover_weights)
+        assert len(mover_weights) == 5
+        with pytest.raises(KeyError):
+            choice_prob = strategy.choice_probability(scheme, group_weights,
+                                                      mover_weights)
 
     def test_weights_from_choice_probability(self):
         scheme = self.scheme_setup_shooting_repex()
         ens0 = self.network.sampling_transitions[0].ensembles[0]
         strategy = OrganizeByMoveGroupStrategy()
         group_weights = {'shooting' : 1.0, 'repex' : 0.5}
         mover_weights = {}
@@ -675,16 +670,16 @@
         choice_prob = strategy.choice_probability(scheme, group_weights,
                                                   mover_weights)
 
         (group_w, mover_w) = strategy.weights_from_choice_probability(
             scheme, choice_prob
         )
 
-        assert_equal(group_weights, group_w)
-        assert_equal(mover_weights, mover_w)
+        assert group_weights == group_w
+        assert mover_weights == mover_w
         #TODO: run more thorough tests of this
 
     def test_chooser_root_weights(self):
         scheme = MoveScheme(self.network)
         ens0 = self.network.sampling_transitions[0].ensembles[0]
         ens1 = self.network.sampling_transitions[0].ensembles[1]
         ens2 = self.network.sampling_transitions[0].ensembles[2]
@@ -703,15 +698,15 @@
         group_weights = {'shooting' : 1.0, 'repex' : 0.5}
         mover_weights = {}
         for groupname in list(scheme.movers.keys()):
             for mover in scheme.movers[groupname]:
                 mover_weights[(groupname, mover.ensemble_signature)] = 1.0
 
         w = strategy.chooser_root_weights(scheme, group_weights, mover_weights)
-        assert_equal(w, {'shooting' : 3.0, 'repex' : 1.0})
+        assert w == {'shooting' : 3.0, 'repex' : 1.0}
 
     def test_chooser_mover_weights(self):
         scheme = self.scheme_setup_shooting_repex()
         strategy = OrganizeByMoveGroupStrategy()
         group_weights = {'shooting' : 1.0, 'repex' : 0.5}
         mover_weights = {}
         for groupname in list(scheme.movers.keys()):
@@ -722,15 +717,15 @@
         for g in scheme.movers:
             for m in scheme.movers[g]:
                 m_sig[m] = (g, m.ensemble_signature)
 
         for g in scheme.movers:
             expected_w = {m : mover_weights[m_sig[m]] for m in scheme.movers[g]}
             w = strategy.chooser_mover_weights(scheme, g, mover_weights)
-            assert_equal(w, expected_w)
+            assert w == expected_w
 
 
     def test_make_movers(self):
         scheme = MoveScheme(self.network)
         ens0 = self.network.sampling_transitions[0].ensembles[0]
         ens1 = self.network.sampling_transitions[0].ensembles[1]
         ens2 = self.network.sampling_transitions[0].ensembles[2]
@@ -753,47 +748,47 @@
             minus_ensemble=self.network.minus_ensembles[0],
             innermost_ensembles=[ens0]
         )]
 
         strategy = OrganizeByMoveGroupStrategy()
         root = strategy.make_movers(scheme)
 
-        assert_equal(len(root.movers), 4)
+        assert len(root.movers) == 4
         names = ['ShootingChooser', 'RepexChooser', 'PathreversalChooser',
                  'MinusChooser']
         name_dict = {root.movers[i].name : i for i in range(len(root.movers))}
         for name in names:
-            assert_in(name, list(name_dict.keys()))
+            assert name in list(name_dict.keys())
 
         name = 'ShootingChooser'
         weight = root.weights[name_dict[name]]
         chooser = root.movers[name_dict[name]]
-        assert_equal(type(chooser), paths.RandomChoiceMover)
-        assert_equal(weight, 3.0)
-        assert_equal(len(chooser.movers), 3)
+        assert type(chooser) == paths.RandomChoiceMover
+        assert weight == 3.0
+        assert len(chooser.movers) == 3
         for w in chooser.weights:
-            assert_equal(w, 1.0)
+            assert w == 1.0
 
         name = 'RepexChooser'
         weight = root.weights[name_dict[name]]
         chooser = root.movers[name_dict[name]]
-        assert_equal(type(chooser), paths.RandomChoiceMover)
-        assert_equal(weight, 1.0)
-        assert_equal(len(chooser.movers), 2)
+        assert type(chooser) == paths.RandomChoiceMover
+        assert weight == 1.0
+        assert len(chooser.movers) == 2
         for w in chooser.weights:
-            assert_equal(w, 1.0)
+            assert w == 1.0
 
         name = 'MinusChooser'
         weight = root.weights[name_dict[name]]
         chooser = root.movers[name_dict[name]]
-        assert_equal(type(chooser), paths.RandomChoiceMover)
-        assert_equal(len(chooser.movers), 1)
-        assert_equal(weight, 0.2)
+        assert type(chooser) == paths.RandomChoiceMover
+        assert len(chooser.movers) == 1
+        assert weight == 0.2
         for w in chooser.weights:
-            assert_equal(w, 1.0)
+            assert w == 1.0
 
     def test_make_movers_unknown_group(self):
         scheme = MoveScheme(self.network)
         ens0 = self.network.sampling_transitions[0].ensembles[0]
         ens1 = self.network.sampling_transitions[0].ensembles[1]
         ens2 = self.network.sampling_transitions[0].ensembles[2]
         scheme.movers['blahblah']  = [
@@ -805,19 +800,19 @@
         root = strategy.make_movers(scheme)
 
         name_dict = {root.movers[i].name : i for i in range(len(root.movers))}
 
         name = 'BlahblahChooser'
         weight = root.weights[name_dict[name]]
         chooser = root.movers[name_dict[name]]
-        assert_equal(type(chooser), paths.RandomChoiceMover)
-        assert_equal(weight, 2.0)
-        assert_equal(len(chooser.movers), 2)
+        assert type(chooser) == paths.RandomChoiceMover
+        assert weight == 2.0
+        assert len(chooser.movers) == 2
         for w in chooser.weights:
-            assert_equal(w, 1.0)
+            assert w == 1.0
 
     def test_make_movers_custom_group(self):
         scheme = MoveScheme(self.network)
         ens0 = self.network.sampling_transitions[0].ensembles[0]
         ens1 = self.network.sampling_transitions[0].ensembles[1]
         ens2 = self.network.sampling_transitions[0].ensembles[2]
         scheme.movers['blahblahblah']  = [
@@ -830,70 +825,70 @@
         root = strategy.make_movers(scheme)
 
         name_dict = {root.movers[i].name : i for i in range(len(root.movers))}
 
         name = 'BlahblahblahChooser'
         weight = root.weights[name_dict[name]]
         chooser = root.movers[name_dict[name]]
-        assert_equal(type(chooser), paths.RandomChoiceMover)
-        assert_equal(weight, 4.0)
-        assert_equal(len(chooser.movers), 2)
+        assert type(chooser) == paths.RandomChoiceMover
+        assert weight == 4.0
+        assert len(chooser.movers) == 2
         for w in chooser.weights:
-            assert_equal(w, 1.0)
+            assert w == 1.0
 
     def test_get_weights_scheme_all_unset(self):
         strategy = OrganizeByMoveGroupStrategy()
 
         scheme = MoveScheme(self.network)
         scheme.append(NearestNeighborRepExStrategy())
         scheme.append(OneWayShootingStrategy())
         root = scheme.move_decision_tree()
-        assert_equal(len(scheme.movers), 2)
+        assert len(scheme.movers) == 2
         all_movers = scheme.movers['shooting'] + scheme.movers['repex']
         all_movers_sigs = [m.ensemble_signature for m in all_movers]
-        assert_equal(strategy.group_weights, {})
-        assert_equal(strategy.mover_weights, {})
+        assert strategy.group_weights == {}
+        assert strategy.mover_weights == {}
 
         (group_weights, mover_weights) = strategy.get_weights(
             scheme=scheme,
             sorted_movers=scheme.movers
         )
-        assert_equal(group_weights, {'shooting' : 1.0, 'repex' : 0.5})
+        assert group_weights == {'shooting' : 1.0, 'repex' : 0.5}
 
         # check that the number of sigs in a each group matches the number
         # of movers in that group
         for group in list(group_weights.keys()):
             mover_sigs = [sig for sig in list(mover_weights.keys())
                           if sig[0]==group]
-            assert_equal(len(mover_sigs), len(scheme.movers[group]))
+            assert len(mover_sigs) == len(scheme.movers[group])
 
         for sig in list(mover_weights.keys()):
-            assert_equal(mover_weights[sig], 1.0)
-            assert_in(sig[1], all_movers_sigs)
+            assert mover_weights[sig] == 1.0
+            assert sig[1] in all_movers_sigs
 
         # check that we can reuse these in a different scheme
         scheme2 = MoveScheme(self.network)
         scheme2.append(OneWayShootingStrategy())
         root = scheme2.move_decision_tree()
-        assert_equal(len(scheme2.movers), 1)
+        assert len(scheme2.movers) == 1
 
         (group_weights, mover_weights) = strategy.get_weights(
             scheme=scheme2,
             sorted_movers=scheme2.movers
         )
-        assert_equal(group_weights, {'shooting' : 1.0})
+        assert group_weights == {'shooting' : 1.0}
         for sig in mover_weights:
-            assert_equal(mover_weights[sig], 1.0)
-            assert_in(sig[1], [m.ensemble_signature
-                               for m in scheme2.movers[sig[0]]])
+            assert mover_weights[sig] == 1.0
+            assert sig[1] in [m.ensemble_signature
+                              for m in scheme2.movers[sig[0]]]
 
         for group in list(scheme2.movers.keys()):
             mover_sigs = [sig for sig in list(mover_weights.keys())
                           if sig[0]==group]
-            assert_equal(len(mover_sigs), len(scheme2.movers[group]))
+            assert len(mover_sigs) == len(scheme2.movers[group])
 
     def test_get_weights_both_internal_weights_set(self):
         strategy = OrganizeByMoveGroupStrategy()
         ensA = self.network.sampling_transitions[0].ensembles[0]
         ensA_sig = ((ensA,),(ensA,))
 
         scheme = MoveScheme(self.network)
@@ -913,41 +908,41 @@
             scheme=scheme,
             sorted_movers=scheme.movers,
             sort_weights_override=strategy.group_weights,
             mover_weights_override=strategy.mover_weights
         )
         root = scheme.move_decision_tree(rebuild=True)
 
-        assert_equal(group_weights, {'shooting' : 1.0, 'repex' : 3.0})
+        assert group_weights == {'shooting' : 1.0, 'repex' : 3.0}
         expected_mover_weights = {}
         for group in scheme.movers:
             for mover in scheme.movers[group]:
                 sig = mover.ensemble_signature
                 if group == 'shooting' and sig == ensA_sig:
                     expected_mover_weights[(group,sig)] = 2.0
                 elif group == 'shooting':
                     expected_mover_weights[(group,sig)] = 1.0
                 else:
                     expected_mover_weights[(group,sig)] = 1.0
 
-        assert_equal(mover_weights, expected_mover_weights)
+        assert mover_weights == expected_mover_weights
 
         new_choice_probability = scheme.choice_probability
         new_repex_chooser = [m for m in root if m.name=="RepexChooser"][0]
         repex_chooser_idx = root.movers.index(new_repex_chooser)
-        assert_equal(root.weights[repex_chooser_idx],
-                     3.0*len(new_repex_chooser.movers))
+        assert (root.weights[repex_chooser_idx]
+                == 3.0*len(new_repex_chooser.movers))
 
         new_shoot_chooser = [m for m in root if m.name=="ShootingChooser"][0]
         new_shooter_ensA = [m for m in scheme.movers['shooting']
                             if m.ensemble_signature == ensA_sig][0]
         shooter_ensA_idx = new_shoot_chooser.movers.index(new_shooter_ensA)
-        assert_equal(new_shoot_chooser.weights[shooter_ensA_idx], 2.0)
+        assert new_shoot_chooser.weights[shooter_ensA_idx] == 2.0
 
-        assert_not_equal(new_choice_probability, old_choice_probability)
+        assert new_choice_probability != old_choice_probability
 
     def test_get_weights_group_weights_set(self):
         strategy = OrganizeByMoveGroupStrategy()
         scheme = MoveScheme(self.network)
         scheme.append([NearestNeighborRepExStrategy(),
                        OneWayShootingStrategy(),
                        strategy])
@@ -961,27 +956,27 @@
         for mover in scheme.movers['repex']:
             assert_almost_equal(scheme.choice_probability[mover], old_div(1.0,16.0))
 
 
         strategy.group_weights['shooting'] = 2.0
         root = scheme.move_decision_tree(rebuild=True)
 
-        assert_equal(strategy.group_weights, {'shooting' : 2.0, 'repex' : 0.5})
+        assert strategy.group_weights == {'shooting' : 2.0, 'repex' : 0.5}
 
         (group_weights, mover_weights) = strategy.get_weights(
             scheme=scheme,
             sorted_movers=scheme.movers,
             sort_weights_override=strategy.group_weights
         )
-        assert_equal(group_weights, {'shooting' : 2.0, 'repex' : 0.5})
+        assert group_weights == {'shooting' : 2.0, 'repex' : 0.5}
         # everything within the group should have the same mover_weight
         for group in scheme.movers:
             group_sigs = [s for s in mover_weights if s[0]==group]
             for sig in group_sigs:
-                assert_equal(mover_weights[sig], mover_weights[group_sigs[0]])
+                assert mover_weights[sig] == mover_weights[group_sigs[0]]
 
         choice_prob = strategy.choice_probability(
             scheme, group_weights, mover_weights
         )
         for mover in scheme.movers['shooting']:
             assert_almost_equal(choice_prob[mover], old_div(1.0,7.0))
         for mover in scheme.movers['repex']:
@@ -998,15 +993,15 @@
         strategy.group_weights['repex'] = 3.0
         root = scheme.move_decision_tree()
         (group_weights, mover_weights) = strategy.get_weights(
             scheme=scheme,
             sorted_movers=scheme.movers,
             sort_weights_override=strategy.group_weights
         )
-        assert_equal(group_weights, {'shooting' : 1.0, 'repex' : 3.0})
+        assert group_weights == {'shooting' : 1.0, 'repex' : 3.0}
 
         ensA = self.network.sampling_transitions[0].ensembles[0]
         ensA_sig = ((ensA,),(ensA,))
         strategy.group_weights = {}
         strategy.mover_weights[('shooting',ensA_sig)] = 2.0
 
         (group_weights, mover_weights) = strategy.get_weights(
@@ -1014,17 +1009,17 @@
             sorted_movers=scheme.movers,
             sort_weights_override=strategy.group_weights,
             mover_weights_override=strategy.mover_weights
         )
 
         for sig in mover_weights:
             if sig == ('shooting',ensA_sig):
-                assert_equal(mover_weights[sig], 2.0)
+                assert mover_weights[sig] == 2.0
             elif sig[0] == 'shooting':
-                assert_equal(mover_weights[sig], 1.0)
+                assert mover_weights[sig] == 1.0
 
         assert_almost_equal(group_weights['shooting'], 1.0)
         assert_almost_equal(group_weights['repex'], 3.0)
 
     def test_get_weights_internal_unset_choice_prob_set(self):
         strategy = OrganizeByMoveGroupStrategy()
         scheme = MoveScheme(self.network)
@@ -1071,20 +1066,20 @@
                 ][0]
                 assert_almost_equal(new_choice_prob[mover],
                                     old_choice_prob[old_mover])
 
         #print new_choice_prob
         for (old, new) in zip(list(old_mover_weights.keys()), list(mover_weights.keys())):
             try:
-                assert_equal(old_mover_weights[old], mover_weights[new])
+                assert old_mover_weights[old] == mover_weights[new]
             except AssertionError:
                 print(old_mover_weights[old])
                 print(mover_weights[new])
                 raise
-        assert_equal(old_mover_weights, mover_weights)
+        assert old_mover_weights == mover_weights
 
     def test_get_weights_mover_weights_set_no_shooting(self):
         # follows test_get_weights_mover_weights_set, replacing shooting
         # with path reversal
         strategy = OrganizeByMoveGroupStrategy()
         scheme = MoveScheme(self.network)
         scheme.append([NearestNeighborRepExStrategy(),
@@ -1094,15 +1089,15 @@
         strategy.group_weights['pathreversal'] = 1.0
         root = scheme.move_decision_tree()
         (group_weights, mover_weights) = strategy.get_weights(
             scheme=scheme,
             sorted_movers=scheme.movers,
             sort_weights_override=strategy.group_weights
         )
-        assert_equal(group_weights, {'pathreversal' : 1.0, 'repex' : 3.0})
+        assert group_weights == {'pathreversal' : 1.0, 'repex' : 3.0}
         ensA = self.network.sampling_transitions[0].ensembles[0]
         ensA_sig = ((ensA,),(ensA,))
         strategy.group_weights = {}
         strategy.mover_weights[('pathreversal',ensA_sig)] = 2.0
 
         (group_weights, mover_weights) = strategy.get_weights(
             scheme=scheme,
@@ -1110,17 +1105,17 @@
             sort_weights_override=strategy.group_weights,
             mover_weights_override=strategy.mover_weights
         )
         for sig in [s for s in mover_weights if s[0]=='pathreversal']:
             weight_sigA = mover_weights[('pathreversal',ensA_sig)]
             ratio = old_div(mover_weights[sig], weight_sigA)
             if sig == ('pathreversal',ensA_sig):
-                assert_equal(ratio, 1.0)
+                assert ratio == 1.0
             else:
-                assert_equal(ratio, 0.5)
+                assert ratio == 0.5
 
         assert_almost_equal(group_weights['pathreversal'], 1.0)
         assert_almost_equal(group_weights['repex'], 3.0)
 
 
 class TestOrganizeByEnsembleStrategy(MoveStrategyTestSetup):
     StrategyClass = OrganizeByEnsembleStrategy
@@ -1222,15 +1217,15 @@
             ('repex', sig01) : old_div(13.0,90.0),
             ('repex', sig12) : old_div(7.0,54.0),
             ('minus', sig_minus) : old_div(1.8,9.0),
             ('pathreversal', sig0) : old_div(4.0,45.0),
             ('pathreversal', sig1) : old_div(1.0,18.0),
             ('pathreversal', sig2) : old_div(2.0,27.0)
         }
-        assert_equal(set(expected.keys()), set(found.keys()))
+        assert set(expected.keys()) == set(found.keys())
         for k in list(expected.keys()):
             assert_almost_equal(expected[k], found[k])
 
 
     def test_chooser_mover_weights(self):
         scheme = self.scheme
         ens0 = self.network.sampling_transitions[0].ensembles[0]
@@ -1241,36 +1236,36 @@
 
         (ensemble_weights, mover_weights) = strategy.default_weights(scheme)
 
         for ens in [ens0, ens1, ens2, minus]:
             chooser_mweights = strategy.chooser_mover_weights(scheme, ens,
                                                               mover_weights)
             for mover in chooser_mweights:
-                assert_in(ens, mover.ensemble_signature[0])
+                assert ens in mover.ensemble_signature[0]
 
             if ens in [ens0, ens1]:
-                assert_equal(len(chooser_mweights), 4)
+                assert len(chooser_mweights) == 4
             elif ens is minus:
-                assert_equal(len(chooser_mweights), 1)
+                assert len(chooser_mweights) == 1
             elif ens is ens2:
-                assert_equal(len(chooser_mweights), 3)
+                assert len(chooser_mweights) == 3
         # that test feels a little minimal, but I guess it does the job
 
     def test_default_weights(self):
         scheme = self.scheme
         ens0 = self.network.sampling_transitions[0].ensembles[0]
         ens1 = self.network.sampling_transitions[0].ensembles[1]
         ens2 = self.network.sampling_transitions[0].ensembles[2]
         minus = self.network.minus_ensembles[0]
         strategy = self.StrategyClass()
 
         (ensemble_weights, mover_weights)= strategy.default_weights(scheme)
 
-        assert_equal(ensemble_weights,
-                     {e : 1.0 for e in [ens0, ens1, ens2, minus]})
+        assert ensemble_weights == {e : 1.0
+                                    for e in [ens0, ens1, ens2, minus]}
 
         # get the correct order on repex and minus signatures for testing
         double_sigs = [m.ensemble_signature
                        for m in sum([scheme.movers[g]
                                      for g in ['repex', 'minus']], [])
                       ]
         repex01_sig = reorder_ensemble_signature(((ens0,ens1),(ens0,ens1)),
@@ -1291,19 +1286,19 @@
             ('repex', repex01_sig, ens1),
             ('repex', repex12_sig, ens1),
             ('repex', repex12_sig, ens2),
             ('minus', minus_sig, minus),
             ('minus', minus_sig, ens0),
         ]
 
-        assert_equal(len(mover_ens_sigs), len(list(mover_weights.keys())))
-        assert_equal(set(mover_weights.keys()), set(mover_ens_sigs))
+        assert len(mover_ens_sigs) == len(list(mover_weights.keys()))
+        assert set(mover_weights.keys()) == set(mover_ens_sigs)
 
         expected = {s : 1.0 for s in mover_ens_sigs}
-        assert_equal(expected, mover_weights)
+        assert expected == mover_weights
 
     def test_weights_from_choice_probability(self):
         scheme = self.scheme
         ens0 = self.network.sampling_transitions[0].ensembles[0]
         ens1 = self.network.sampling_transitions[0].ensembles[1]
         ens2 = self.network.sampling_transitions[0].ensembles[2]
         minus = self.network.minus_ensembles[0]
@@ -1339,18 +1334,18 @@
     def test_make_movers(self):
         scheme = self.scheme
         strategy = self.StrategyClass()
         root = strategy.make_movers(scheme)
 
         choosers = root.movers
         chooser_weights = root.weights
-        assert_equal(list(chooser_weights), [1.0]*4)
+        assert list(chooser_weights) == [1.0]*4
         for (mover, w) in zip(choosers, chooser_weights):
             n_moves = len(mover.movers)
-            assert_equal(mover.weights, [1.0]*n_moves)
+            assert mover.weights == [1.0]*n_moves
 
 
     def test_make_mover_rebuild_choice_probability(self):
         scheme = self.scheme
 
         # Organize by move group, switch to ensemble, switch back
         scheme.append(OrganizeByMoveGroupStrategy())
@@ -1408,32 +1403,32 @@
                                               strategy.mover_weights)
         scheme.choice_probability = strategy.choice_probability(scheme,
                                                                 ens_w, mov_w)
         for ens in [ens0, ens1, ens2, minus]:
             chooser_mweights = strategy.chooser_mover_weights(scheme, ens,
                                                               mover_weights)
             if ens in [ens0, ens1]:
-                assert_equal(len(chooser_mweights), 5)
+                assert len(chooser_mweights) == 5
             elif ens is minus:
-                assert_equal(len(chooser_mweights), 2)
+                assert len(chooser_mweights) == 2
             elif ens is ens2:
-                assert_equal(len(chooser_mweights), 4)
+                assert len(chooser_mweights) == 4
 
             real_movers = [m for m in list(chooser_mweights.keys())
                            if m != strategy.null_mover]
             for m in real_movers:
-                assert_equal(scheme.choice_probability[m], chooser_mweights[m])
+                assert scheme.choice_probability[m] == chooser_mweights[m]
             assert_almost_equal(sum(chooser_mweights.values()), 1.0)
 
     def test_make_movers(self):
         scheme = self.scheme
         strategy = self.StrategyClass()
         root = strategy.make_movers(scheme)
 
-        assert_equal(len(root.movers), 4)
+        assert len(root.movers) == 4
 
         for mover in list(scheme.choice_probability.keys()):
             assert_almost_equal(
                 scheme.choice_probability[mover] * 0.25,
                 scheme.real_choice_probability[mover]
             )
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_ms_outer_interface.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_ms_outer_interface.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from __future__ import absolute_import
 from builtins import object
-from nose.tools import (assert_equal, assert_not_equal, assert_almost_equal,
-                        raises)
-from nose.plugins.skip import Skip, SkipTest
 from .test_helpers import (
     true_func, assert_equal_array_array, make_1d_traj, data_filename,
     assert_items_equal
 )
 
 import openpathsampling as paths
 from openpathsampling.high_level.interface_set import GenericVolumeInterfaceSet
@@ -58,73 +55,74 @@
              for t in self.network.sampling_transitions}
         )
 
     def test_initialization(self):
         by_lambda = self.ms_outer
         explicit = self.ms_outer_explicit
         for iface_set in explicit.interface_sets:
-            assert_equal(by_lambda.volume_for_interface_set(iface_set),
-                         explicit.volume_for_interface_set(iface_set))
-            assert_equal(by_lambda.lambda_for_interface_set(iface_set),
-                         explicit.lambda_for_interface_set(iface_set))
+            assert (by_lambda.volume_for_interface_set(iface_set)
+                    == explicit.volume_for_interface_set(iface_set))
+            assert (by_lambda.lambda_for_interface_set(iface_set)
+                    == explicit.lambda_for_interface_set(iface_set))
 
-        assert_equal(len(explicit.volumes), len(by_lambda.volumes))
-        assert_equal(len(explicit.lambdas), len(by_lambda.lambdas))
+        assert len(explicit.volumes) == len(by_lambda.volumes)
+        assert len(explicit.lambdas) == len(by_lambda.lambdas)
         assert_items_equal(set(explicit.interface_sets),
                            set(by_lambda.interface_sets))
 
 
     def test_volume_for_interface_set(self):
-        assert_equal(
-            self.ms_outer.volume_for_interface_set(self.interfaces_inc),
-            self.volumes[0]
-        )
-        assert_equal(
-            self.ms_outer.volume_for_interface_set(self.interfaces_dec),
-            self.volumes[1]
+        assert (
+            self.ms_outer.volume_for_interface_set(self.interfaces_inc)
+            == self.volumes[0]
+        )
+        assert (
+            self.ms_outer.volume_for_interface_set(self.interfaces_dec)
+            == self.volumes[1]
         )
 
     def test_lambda_for_interface_set(self):
-        assert_equal(
-            self.ms_outer.lambda_for_interface_set(self.interfaces_inc),
-            0.5
-        )
-        assert_equal(
-            self.ms_outer.lambda_for_interface_set(self.interfaces_dec),
-            0.4
+        assert (
+            self.ms_outer.lambda_for_interface_set(self.interfaces_inc)
+            == 0.5
+        )
+        assert (
+            self.ms_outer.lambda_for_interface_set(self.interfaces_dec)
+            == 0.4
         )
 
+
     def test_relevant_transitions(self):
         extra_set = paths.VolumeInterfaceSet(self.cv_inc, 0.0, [0.2, 0.3])
         extra = paths.TISTransition(self.stateA, self.stateB, extra_set,
                                     self.cv_inc, "fake")
         transitions = self.network.sampling_transitions + [extra]
         # TODO: switch once network is working
         relevant = self.post_network.relevant_transitions(transitions)
         #relevant = self.ms_outer.relevant_transitions(transitions)
-        assert_equal(len(relevant), 2)
-        assert_equal(set(self.network.sampling_transitions), set(relevant))
+        assert len(relevant) == 2
+        assert set(self.network.sampling_transitions) == set(relevant)
 
     def test_make_ensemble(self):
         transitions = self.network.sampling_transitions
         # TODO: switch once network is working
         ensemble = self.post_network.make_ensemble(transitions)
         #ensemble = self.ms_outer.make_ensemble(transitions)
         test_AA = make_1d_traj([-0.1, 0.2, -0.2])
         test_AXA = make_1d_traj([-0.1, 0.6, -0.2])
         test_BB = make_1d_traj([1.1, 0.9, 1.2])
         test_BXB = make_1d_traj([1.1, 0.5, 1.2])
         test_AXB = make_1d_traj([-0.1, 0.6, 1.1])
         test_BXA = make_1d_traj([1.1, 0.5, -0.1])
-        assert_equal(ensemble(test_AA), False)
-        assert_equal(ensemble(test_AXA), True)
-        assert_equal(ensemble(test_BB), False)
-        assert_equal(ensemble(test_BXB), True)
-        assert_equal(ensemble(test_BXA), True)
-        assert_equal(ensemble(test_AXB), True)
+        assert ensemble(test_AA) is False
+        assert ensemble(test_AXA) is True
+        assert ensemble(test_BB) is False
+        assert ensemble(test_BXB) is True
+        assert ensemble(test_BXA) is True
+        assert ensemble(test_AXB) is True
 
     def test_make_ensemble_with_forbidden(self):
         forbidden = paths.CVDefinedVolume(self.cv_inc, 0.55, 0.65)
         transitions = self.network.sampling_transitions
         # TODO: switch once network is working
         ensemble = self.post_network.make_ensemble(transitions, forbidden)
         #ensemble = self.ms_outer.make_ensemble(transitions, forbidden)
@@ -134,17 +132,17 @@
         test_BB = make_1d_traj([1.1, 0.9, 1.2])
         test_BXB = make_1d_traj([1.1, 0.5, 1.2])
         test_BFB = make_1d_traj([1.1, 0.6, 1.2])
         test_AXB = make_1d_traj([-0.1, 0.7, 1.1])
         test_AFB = make_1d_traj([-0.1, 0.6, 1.1])
         test_BXA = make_1d_traj([1.1, 0.5, -0.1])
         test_BFA = make_1d_traj([1.1, 0.6, -0.1])
-        assert_equal(ensemble(test_AA), False)
-        assert_equal(ensemble(test_AXA), True)
-        assert_equal(ensemble(test_BB), False)
-        assert_equal(ensemble(test_BXB), True)
-        assert_equal(ensemble(test_BXA), True)
-        assert_equal(ensemble(test_AXB), True)
-        assert_equal(ensemble(test_AFA), False)
-        assert_equal(ensemble(test_BFB), False)
-        assert_equal(ensemble(test_AFB), False)
-        assert_equal(ensemble(test_BFA), False)
+        assert ensemble(test_AA) is False
+        assert ensemble(test_AXA) is True
+        assert ensemble(test_BB) is False
+        assert ensemble(test_BXB) is True
+        assert ensemble(test_BXA) is True
+        assert ensemble(test_AXB) is True
+        assert ensemble(test_AFA) is False
+        assert ensemble(test_BFB) is False
+        assert ensemble(test_AFB) is False
+        assert ensemble(test_BFA) is False
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_network.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_network.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from __future__ import absolute_import
 from builtins import zip
 from builtins import object
 import numpy as np
 
-from nose.tools import (assert_equal, assert_not_equal, assert_almost_equal,
-                        raises)
-from nose.plugins.skip import Skip, SkipTest
 from .test_helpers import (
     true_func, assert_equal_array_array, make_1d_traj, data_filename
 )
 
 import openpathsampling as paths
 
 import openpathsampling.engines.toy as peng
@@ -120,103 +117,102 @@
                      (self.stateB, self.ifacesB[0]): 4.0,
                      (self.stateC, self.ifacesC[0]): 5.0}
         self.mstis.set_fluxes(flux_dict)
         for trans in self.mstis.transitions:
             myflux = {self.stateA: 2.0,
                       self.stateB: 4.0,
                       self.stateC: 5.0}[trans[0]]
-            assert_equal(self.mstis.transitions[trans]._flux, myflux)
+            assert self.mstis.transitions[trans]._flux == myflux
 
     def test_all_states(self):
-        assert_equal(set(self.mstis.all_states),
-                     set([self.stateA, self.stateB, self.stateC]))
+        assert (set(self.mstis.all_states)
+                == set([self.stateA, self.stateB, self.stateC]))
 
     def test_trajectories(self):
         # TODO; make this test fully comprehensive? (loop over all
         # possibilities?)
         ensA0 = self.mstis.from_state[self.stateA].ensembles[0]
         ensAm = self.mstis.from_state[self.stateA].ensembles[-1]
-        assert_equal(ensA0(self.traj['AA']), True)
-        assert_equal(ensAm(self.traj['AA']), False)
-        assert_equal(ensAm(self.traj['AB']), True)
+        assert ensA0(self.traj['AA'])
+        assert not ensAm(self.traj['AA'])
+        assert ensAm(self.traj['AB'])
         ensB0 = self.mstis.from_state[self.stateB].ensembles[0]
-        assert_equal(ensB0(self.traj['AB']), False)
-        assert_equal(ensB0(self.traj['BA']), True)
-        assert_equal(ensB0(self.traj['BB']), True)
-        assert_equal(ensB0(self.traj['BC']), True)
-        assert_equal(ensB0(self.traj['AC']), False)
+        assert not ensB0(self.traj['AB'])
+        assert ensB0(self.traj['BA'])
+        assert ensB0(self.traj['BB'])
+        assert ensB0(self.traj['BC'])
+        assert not ensB0(self.traj['AC'])
         ensC0 = self.mstis.from_state[self.stateC].ensembles[0]
-        assert_equal(ensC0(self.traj['CC']), True)
-        assert_equal(ensC0(self.traj['CB']), True)
-        assert_equal(ensC0(self.traj['CA']), True)
-        assert_equal(ensC0(self.traj['BC']), False)
-        assert_equal(ensC0(self.traj['AC']), False)
-        assert_equal(ensC0(self.traj['BB']), False)
+        assert ensC0(self.traj['CC'])
+        assert ensC0(self.traj['CB'])
+        assert ensC0(self.traj['CA'])
+        assert not ensC0(self.traj['BC'])
+        assert not ensC0(self.traj['AC'])
+        assert not ensC0(self.traj['BB'])
 
     def test_ms_outers(self):
         for traj_label in ['AB', 'BA', 'AC', 'CA', 'BC', 'CB']:
-            assert_equal(self.mstis.ms_outers[0](self.traj[traj_label]), True)
+            assert self.mstis.ms_outers[0](self.traj[traj_label])
 
     def test_minus_ensembles(self):
         good_traj_seq = [-0.51, -0.49, -0.40, -0.52, -0.48, -0.51]  # AXXAXA
         bad_traj_seq = [-0.51, -0.49, -0.05, -0.52, -0.48, -0.51]  # AXBAXA
         minus_dict = self.mstis.special_ensembles['minus']
         from_A = self.mstis.from_state[self.stateA]
         trans_to_minus = {trans: minus
                           for (minus, transitions) in minus_dict.items()
                           for trans in transitions}
         minus_A = trans_to_minus[from_A]
 
         good_minus_traj = make_1d_traj(good_traj_seq)
         bad_minus_traj = make_1d_traj(bad_traj_seq)
         # test that the call works
-        assert_equal(minus_A(good_minus_traj), True)
-        assert_equal(minus_A(bad_minus_traj), False)
+        assert minus_A(good_minus_traj)
+        assert not minus_A(bad_minus_traj)
         # test that the can_append works for the good traj
         good_building_traj = paths.Trajectory([])
         for (i, snap) in enumerate(good_minus_traj):
             good_building_traj.append(snap)
             if not minus_A.can_append(good_building_traj, trusted=True):
                 break
-        assert_equal(len(good_building_traj), len(good_minus_traj))
+        assert len(good_building_traj) == len(good_minus_traj)
         # test that the can_append works for the bad traj
         bad_building_traj = paths.Trajectory([])
         for (i, snap) in enumerate(bad_minus_traj):
             bad_building_traj.append(snap)
             if not minus_A.can_append(bad_building_traj, trusted=True):
                 break
-        assert_equal(len(bad_building_traj), 3)
+        assert len(bad_building_traj) == 3
 
     def test_sampling_ensembles(self):
-        assert_equal(len(self.mstis.from_state[self.stateA].ensembles), 2)
-        assert_equal(len(self.mstis.from_state[self.stateB].ensembles), 2)
-        assert_equal(len(self.mstis.from_state[self.stateC].ensembles), 2)
+        assert len(self.mstis.from_state[self.stateA].ensembles) == 2
+        assert len(self.mstis.from_state[self.stateB].ensembles) == 2
+        assert len(self.mstis.from_state[self.stateC].ensembles) == 2
 
         # test that .sampling_ensembles is as expected
-        assert_equal(len(self.mstis.sampling_ensembles), 6)
+        assert len(self.mstis.sampling_ensembles) == 6
         all_sampling_ens = sum(
             [self.mstis.from_state[state].ensembles
              for state in [self.stateA, self.stateB, self.stateC]],
             []
         )
-        assert_equal(set(self.mstis.sampling_ensembles),
-                     set(all_sampling_ens))
+        assert set(self.mstis.sampling_ensembles) == set(all_sampling_ens)
 
         # test that sampling ensembles has cv_max set
-        assert_equal(len(paths.InterfaceSet._cv_max_dict), 1)
+        assert len(paths.InterfaceSet._cv_max_dict) == 1
         cv_max = list(paths.InterfaceSet._cv_max_dict.values())[0]
         for transition in self.mstis.sampling_transitions:
-            assert_equal(transition.interfaces.cv_max, cv_max)
+            assert transition.interfaces.cv_max == cv_max
         for ens in self.mstis.sampling_ensembles:
-            assert_equal(ens.cv_max, cv_max)
+            assert ens.cv_max == cv_max
 
     def test_autonaming(self):
-        assert_equal(self.stateA.name, "A")
-        assert_equal(self.stateB.name, "B")
-        assert_equal(self.stateC.name, "C")
+        assert self.stateA.name == "A"
+        assert self.stateB.name == "B"
+        assert self.stateC.name == "C"
 
         # check that (1) given names stay unchanged; (2) code knows to skip
         # over any default names that have been assigned (i.e., it renames
         # stateC to "C", not to "A"
 
         # force renaming to weirdness
         self.stateA.name = "B"
@@ -231,17 +227,17 @@
         ifacesC = paths.VolumeInterfaceSet(xval, [0.5, 0.4, 0.3],
                                            float("inf"))
         new_network = MSTISNetwork([
             (self.stateA, ifacesA),
             (self.stateB, ifacesB),
             (self.stateC, ifacesC)
         ])
-        assert_equal(self.stateA.name, "B")
-        assert_equal(self.stateB.name, "A")
-        assert_equal(self.stateC.name, "C")
+        assert self.stateA.name == "B"
+        assert self.stateB.name == "A"
+        assert self.stateC.name == "C"
 
 
 class TestMISTISNetwork(TestMultipleStateTIS):
     def setup_method(self):
         super(TestMISTISNetwork, self).setup_method()
 
         ifacesA = self.ifacesA[:-1]
@@ -256,44 +252,43 @@
             [(self.stateA, ifacesA, self.stateB),
              (self.stateB, ifacesB, self.stateA),
              (self.stateA, self.ifacesA, self.stateC)],
             ms_outers=[ms_outer]
         )
 
     def test_initialization(self):
-        assert_equal(len(self.mistis.sampling_transitions), 3)
-        assert_equal(len(self.mistis.input_transitions), 3)
-        assert_equal(len(self.mistis.transitions), 3)
+        assert len(self.mistis.sampling_transitions) == 3
+        assert len(self.mistis.input_transitions) == 3
+        assert len(self.mistis.transitions) == 3
         transitions = self.mistis.transitions
-        assert_equal(len(transitions[self.stateA, self.stateB].ensembles), 2)
-        assert_equal(len(transitions[self.stateB, self.stateA].ensembles), 2)
-        assert_equal(len(transitions[self.stateA, self.stateC].ensembles), 3)
+        assert len(transitions[self.stateA, self.stateB].ensembles) == 2
+        assert len(transitions[self.stateB, self.stateA].ensembles) == 2
+        assert len(transitions[self.stateA, self.stateC].ensembles) == 3
         # TODO: add more checks here
 
     def test_sampling_ensembles(self):
-        assert_equal(len(self.mistis.sampling_ensembles), 7)
+        assert len(self.mistis.sampling_ensembles) == 7
         all_sampling_ens = sum(
             [t.ensembles for t in self.mistis.sampling_transitions], []
         )
-        assert_equal(set(self.mistis.sampling_ensembles),
-                     set(all_sampling_ens))
+        assert set(self.mistis.sampling_ensembles) == set(all_sampling_ens)
         # test that sampling ensembles has cv_max set
-        assert_equal(len(paths.InterfaceSet._cv_max_dict), 1)
+        assert len(paths.InterfaceSet._cv_max_dict) == 1
         cv_max = list(paths.InterfaceSet._cv_max_dict.values())[0]
         for transition in self.mistis.sampling_transitions:
-            assert_equal(transition.interfaces.cv_max, cv_max)
+            assert transition.interfaces.cv_max == cv_max
         for ens in self.mistis.sampling_ensembles:
-            assert_equal(ens.cv_max, cv_max)
+            assert ens.cv_max == cv_max
 
     def test_ms_outers(self):
         ms_outer_ens = self.mistis.ms_outers[0]
         for traj_label in ['AB', 'BA']:
-            assert_equal(ms_outer_ens(self.traj[traj_label]), True)
+            assert ms_outer_ens(self.traj[traj_label])
         for traj_label in ['CB', 'CA']:
-            assert_equal(ms_outer_ens(self.traj[traj_label]), False)
+            assert not ms_outer_ens(self.traj[traj_label])
 
     def test_minus_ensembles(self):
         good_traj_seq = [-0.51, -0.49, -0.40, -0.52, -0.48, -0.51]  # AXXAXA
         bad_traj_seq = [-0.51, -0.49, -0.05, -0.52, -0.48, -0.51]  # AXBAXA
 
         minus_dict = self.mistis.special_ensembles['minus']
         minus_ensembles= [
@@ -310,45 +305,45 @@
 
     def test_set_fluxes(self):
         flux_dict = {(self.stateA, self.ifacesA[0]): 2.0,  # same flux 2x
                      (self.stateB, self.ifacesB[0]): 4.0}
         self.mistis.set_fluxes(flux_dict)
         for (A, B) in self.mistis.transitions:
             if A == self.stateA:
-                assert_equal(self.mistis.transitions[(A, B)]._flux, 2.0)
+                assert self.mistis.transitions[(A, B)]._flux == 2.0
             elif A == self.stateB:
-                assert_equal(self.mistis.transitions[(A, B)]._flux, 4.0)
+                assert self.mistis.transitions[(A, B)]._flux == 4.0
 
     def test_trajectories_nonstrict(self):
         fromA = [trans for trans in self.mistis.sampling_transitions
                  if trans.stateA == self.stateA]
         fromB = [trans for trans in self.mistis.sampling_transitions
                  if trans.stateA == self.stateB]
-        assert_equal(len(fromA), 2)
-        assert_equal(len(fromB), 1)
+        assert len(fromA) == 2
+        assert len(fromB) == 1
         fromA_0 = fromA[0].ensembles[0]
         fromA_1 = fromA[1].ensembles[0]
         fromB_0 = fromB[0].ensembles[0]
-        assert_equal(fromA_0(self.traj['AA']), True)
-        assert_equal(fromA_0(self.traj['AB']), True)
-        assert_equal(fromA_0(self.traj['AC']), True)
-        assert_equal(fromA_0(self.traj['BB']), False)
-        assert_equal(fromA_0(self.traj['CB']), False)
-        assert_equal(fromA_0(self.traj['ABC']), False)
-        assert_equal(fromA_1(self.traj['AA']), True)
-        assert_equal(fromA_1(self.traj['AB']), True)
-        assert_equal(fromA_1(self.traj['AC']), True)
-        assert_equal(fromA_1(self.traj['CB']), False)
-        assert_equal(fromA_1(self.traj['CB']), False)
-        assert_equal(fromA_1(self.traj['ABC']), False)
-        assert_equal(fromB_0(self.traj['BA']), True)
-        assert_equal(fromB_0(self.traj['BB']), True)
-        assert_equal(fromB_0(self.traj['BB']), True)
-        assert_equal(fromB_0(self.traj['AB']), False)
-        assert_equal(fromB_0(self.traj['CB']), False)
+        assert fromA_0(self.traj['AA'])
+        assert fromA_0(self.traj['AB'])
+        assert fromA_0(self.traj['AC'])
+        assert not fromA_0(self.traj['BB'])
+        assert not fromA_0(self.traj['CB'])
+        assert not fromA_0(self.traj['ABC'])
+        assert fromA_1(self.traj['AA'])
+        assert fromA_1(self.traj['AB'])
+        assert fromA_1(self.traj['AC'])
+        assert not fromA_1(self.traj['CB'])
+        assert not fromA_1(self.traj['CB'])
+        assert not fromA_1(self.traj['ABC'])
+        assert fromB_0(self.traj['BA'])
+        assert fromB_0(self.traj['BB'])
+        assert fromB_0(self.traj['BB'])
+        assert not fromB_0(self.traj['AB'])
+        assert not fromB_0(self.traj['CB'])
 
     def test_trajectories_strict(self):
         strict = MISTISNetwork([
             (self.stateA, self.ifacesA, self.stateB),
             (self.stateB, self.ifacesB, self.stateA),
             (self.stateA, self.ifacesA, self.stateC)
         ], strict_sampling=True)
@@ -360,31 +355,31 @@
                        trans.stateB == self.stateC)][0]
         transBA = [trans for trans in strict.sampling_transitions
                    if (trans.stateA == self.stateB and
                        trans.stateB == self.stateA)][0]
         ensAB = transAB.ensembles[0]
         ensAC = transAC.ensembles[0]
         ensBA = transBA.ensembles[0]
-        assert_equal(ensAB(self.traj['AA']), True)
-        assert_equal(ensAB(self.traj['AB']), True)
-        assert_equal(ensAB(self.traj['AC']), False)
-        assert_equal(ensAB(self.traj['BB']), False)
-        assert_equal(ensAB(self.traj['BC']), False)
-        assert_equal(ensAB(self.traj['ABC']), False)
-        assert_equal(ensAC(self.traj['AA']), True)
-        assert_equal(ensAC(self.traj['AC']), True)
-        assert_equal(ensAC(self.traj['AB']), False)
-        assert_equal(ensAC(self.traj['BB']), False)
-        assert_equal(ensAC(self.traj['BC']), False)
-        assert_equal(ensAC(self.traj['ABC']), False)
-        assert_equal(ensBA(self.traj['BB']), True)
-        assert_equal(ensBA(self.traj['BA']), True)
-        assert_equal(ensBA(self.traj['BC']), False)
-        assert_equal(ensBA(self.traj['AB']), False)
-        assert_equal(ensBA(self.traj['AC']), False)
+        assert ensAB(self.traj['AA'])
+        assert ensAB(self.traj['AB'])
+        assert not ensAB(self.traj['AC'])
+        assert not ensAB(self.traj['BB'])
+        assert not ensAB(self.traj['BC'])
+        assert not ensAB(self.traj['ABC'])
+        assert ensAC(self.traj['AA'])
+        assert ensAC(self.traj['AC'])
+        assert not ensAC(self.traj['AB'])
+        assert not ensAC(self.traj['BB'])
+        assert not ensAC(self.traj['BC'])
+        assert not ensAC(self.traj['ABC'])
+        assert ensBA(self.traj['BB'])
+        assert ensBA(self.traj['BA'])
+        assert not ensBA(self.traj['BC'])
+        assert not ensBA(self.traj['AB'])
+        assert not ensBA(self.traj['AC'])
 
     def test_storage(self):
         import os
         fname = data_filename("mistis_storage_test.nc")
         if os.path.isfile(fname):
             os.remove(fname)
         storage_w = paths.Storage(fname, "w")
@@ -393,17 +388,17 @@
         # print(storage_w.simplifier.simplify(self.mistis))
 
         storage_w.save(self.mistis)
         storage_w.sync_all()
 
         storage_r = paths.AnalysisStorage(fname)
         reloaded = storage_r.networks[0]
-        assert_equal(reloaded.strict_sampling, False)
-        assert_equal(reloaded.sampling_transitions[0].ensembles[0],
-                     self.mistis.sampling_transitions[0].ensembles[0])
+        assert not reloaded.strict_sampling
+        assert (reloaded.sampling_transitions[0].ensembles[0]
+                == self.mistis.sampling_transitions[0].ensembles[0])
 
         storage_w.close()
         storage_r.close()
         if os.path.isfile(fname):
             os.remove(fname)
 
 
@@ -467,37 +462,36 @@
              (self.stateB, self.stateA), (self.stateB, self.stateC),
              (self.stateC, self.stateA), (self.stateC, self.stateB)],
             **self.std_kwargs
         )
 
     def test_initialization_2state(self):
         network2a = self.network2a
-        assert_equal(len(network2a.sampling_transitions), 1)
-        assert_equal(len(network2a.transitions), 1)
+        assert len(network2a.sampling_transitions) == 1
+        assert len(network2a.transitions) == 1
         network2b = self.network2b
-        assert_equal(len(network2b.sampling_transitions), 1)
-        assert_equal(len(network2b.transitions), 1)
+        assert len(network2b.sampling_transitions) == 1
+        assert len(network2b.transitions) == 1
         network2c = self.network2c
-        assert_equal(len(network2c.sampling_transitions), 1)
-        assert_equal(len(network2c.transitions), 1)
-        assert_equal(set(network2a.all_states), set(network2b.all_states))
-        assert_equal(set(network2b.all_states), set(network2c.all_states))
-        assert_equal(set(network2a.all_states),
-                     set([self.stateA, self.stateB]))
+        assert len(network2c.sampling_transitions) == 1
+        assert len(network2c.transitions) == 1
+        assert set(network2a.all_states) == set(network2b.all_states)
+        assert set(network2b.all_states) == set(network2c.all_states)
+        assert set(network2a.all_states) == set([self.stateA, self.stateB])
 
     def test_initialization_3state(self):
         network3a = self.network3a
-        assert_equal(len(network3a.sampling_transitions), 1)
-        assert_equal(len(network3a.transitions), 6)
+        assert len(network3a.sampling_transitions) == 1
+        assert len(network3a.transitions) == 6
         network3b = self.network3b
-        assert_equal(len(network3b.sampling_transitions), 1)
-        assert_equal(len(network3b.transitions), 6)
+        assert len(network3b.sampling_transitions) == 1
+        assert len(network3b.transitions) == 6
         network3c = self.network3c
-        assert_equal(len(network3c.sampling_transitions), 1)
-        assert_equal(len(network3c.transitions), 6)
+        assert len(network3c.sampling_transitions) == 1
+        assert len(network3c.transitions) == 6
 
     def test_storage(self):
         import os
         fname = data_filename("tps_network_storage_test.nc")
         if os.path.isfile(fname):
             os.remove(fname)
 
@@ -507,88 +501,88 @@
                                       velocities=np.array([[0.0]]),
                                       engine=engine)
 
         states = [self.stateA, self.stateB, self.stateC]
         network_a = self.NetworkType(initial_states=states,
                                      final_states=states,
                                      **self.std_kwargs)
-        assert_equal(len(network_a.sampling_transitions), 1)
-        assert_equal(len(network_a.transitions), 6)
+        assert len(network_a.sampling_transitions) == 1
+        assert len(network_a.transitions) == 6
         storage_w = paths.storage.Storage(fname, "w")
         storage_w.snapshots.save(self.template)
         storage_w.save(network_a)
         storage_w.sync_all()
 
         storage_r = paths.storage.AnalysisStorage(fname)
         network_b = storage_r.networks[0]
-        assert_equal(len(network_b.sampling_transitions), 1)
-        assert_equal(len(network_b.transitions), 6)
+        assert len(network_b.sampling_transitions) == 1
+        assert len(network_b.transitions) == 6
 
         if os.path.isfile(fname):
             os.remove(fname)
 
     def test_allow_self_transitions_false(self):
         network = self.NetworkType.from_states_all_to_all(
             self.states, allow_self_transitions=False, **self.std_kwargs
         )
-        assert_equal(len(network.sampling_ensembles), 1)
+        assert len(network.sampling_ensembles) == 1
         ensemble = network.sampling_ensembles[0]
-        assert_equal(ensemble(self.traj['AA']), False)
-        assert_equal(ensemble(self.traj['AB']), True)
-        assert_equal(ensemble(self.traj['BA']), True)
-        assert_equal(ensemble(self.traj['BC']), True)
-        assert_equal(ensemble(self.traj['CA']), True)
-        assert_equal(ensemble(self.traj['BB']), False)
-        assert_equal(ensemble(self.traj['CC']), False)
+        assert not ensemble(self.traj['AA'])
+        assert ensemble(self.traj['AB'])
+        assert ensemble(self.traj['BA'])
+        assert ensemble(self.traj['BC'])
+        assert ensemble(self.traj['CA'])
+        assert not ensemble(self.traj['BB'])
+        assert not ensemble(self.traj['CC'])
 
     def test_allow_self_transitions_true(self):
         network = self.NetworkType.from_states_all_to_all(
             self.states, allow_self_transitions=True, **self.std_kwargs
         )
-        assert_equal(len(network.sampling_ensembles), 1)
+        assert len(network.sampling_ensembles) == 1
         ensemble = network.sampling_ensembles[0]
-        assert_equal(ensemble(self.traj['AA']), True)
-        assert_equal(ensemble(self.traj['AB']), True)
-        assert_equal(ensemble(self.traj['BA']), True)
-        assert_equal(ensemble(self.traj['BC']), True)
-        assert_equal(ensemble(self.traj['CA']), True)
-        assert_equal(ensemble(self.traj['BB']), True)
-        assert_equal(ensemble(self.traj['CC']), True)
+        assert ensemble(self.traj['AA'])
+        assert ensemble(self.traj['AB'])
+        assert ensemble(self.traj['BA'])
+        assert ensemble(self.traj['BC'])
+        assert ensemble(self.traj['CA'])
+        assert ensemble(self.traj['BB'])
+        assert ensemble(self.traj['CC'])
 
     def test_allow_self_transitions_false_ABX(self):
         network = self.NetworkType.from_states_all_to_all(
             self.states, allow_self_transitions=False, **self.std_kwargs
         )
-        assert_equal(len(network.sampling_ensembles), 1)
+        assert len(network.sampling_ensembles) == 1
         ensemble = network.sampling_ensembles[0]
-        assert_equal(ensemble(self.traj['AB0']), False)
-        assert_equal(ensemble(self.traj['ABA']), False)
+        assert not ensemble(self.traj['AB0'])
+        assert not ensemble(self.traj['ABA'])
 
     def test_allow_self_transitions_true_ABX(self):
         # special case that differs between fixed and flexible
         network = self.NetworkType.from_states_all_to_all(
             self.states, allow_self_transitions=True, **self.std_kwargs
         )
-        assert_equal(len(network.sampling_ensembles), 1)
+        assert len(network.sampling_ensembles) == 1
         ensemble = network.sampling_ensembles[0]
-        assert_equal(ensemble(self.traj['AB0']), False)
-        assert_equal(ensemble(self.traj['ABA']), False)
+        assert not ensemble(self.traj['AB0'])
+        assert not ensemble(self.traj['ABA'])
 
 
 class TestFixedLengthTPSNetwork(TestTPSNetwork):
     NetworkType = FixedLengthTPSNetwork
     std_kwargs = {'length': 4}
 
     def test_lengths(self):
         for network in [self.network2a, self.network2b, self.network2c,
                         self.network3a, self.network3b, self.network3c]:
-            assert_equal(network.sampling_transitions[0].length, 4)
-            assert_equal(list(network.transitions.values())[0].length, 4)
+            assert network.sampling_transitions[0].length == 4
+            assert list(network.transitions.values())[0].length == 4
 
     def test_allow_self_transitions_true_ABX(self):
         network = self.NetworkType.from_states_all_to_all(
             self.states, allow_self_transitions=True, **self.std_kwargs
         )
-        assert_equal(len(network.sampling_ensembles), 1)
+        assert len(network.sampling_ensembles) == 1
         ensemble = network.sampling_ensembles[0]
-        assert_equal(ensemble(self.traj['AB0']), False)
-        assert_equal(ensemble(self.traj['ABA']), True)
+        assert not ensemble(self.traj['AB0'])
+        assert ensemble(self.traj['ABA'])
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_openmm_engine.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_openmm_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from __future__ import absolute_import
 
 import pytest
 from builtins import range
 from builtins import object
 from past.utils import old_div
 import numpy as np
-from nose.tools import (assert_equal)
-from nose.plugins.skip import SkipTest
 
 from openpathsampling.integration_tools import openmm as mm
 
 if mm is None:
     app = None
 else:
     app = mm.app
@@ -36,15 +34,15 @@
 logging.getLogger('openpathsampling.ensemble').setLevel(logging.CRITICAL)
 logging.getLogger('openpathsampling.storage').setLevel(logging.CRITICAL)
 logging.getLogger('openpathsampling.netcdfplus').setLevel(logging.CRITICAL)
 
 def setup_module():
     global topology, template, system, nan_causing_template
     if not (u and mm and app and md):
-        raise SkipTest
+        pytest.skip("Missing requirements")
     template = peng.snapshot_from_pdb(data_filename("ala_small_traj.pdb"))
     topology = peng.to_openmm_topology(template)
 
     # Generated using OpenMM Script Builder
     # http://builder.openmm.org
 
     forcefield = app.ForceField(
@@ -102,16 +100,16 @@
         context.setPositions(template.coordinates)
         context.setVelocities(u.Quantity(zero_array, old_div(u.nanometers, u.picoseconds)))
 
     def teardown_method(self):
         pass
 
     def test_sanity(self):
-        assert_equal(self.engine.n_steps_per_frame, 2)
-        assert_equal(self.engine.n_frames_max, 5)
+        assert self.engine.n_steps_per_frame == 2
+        assert self.engine.n_frames_max == 5
         # TODO: add more sanity checks
         pass  # not quite a SkipTest, but a reminder to add more
 
     def test_snapshot_get(self):
         snap = self.engine.current_snapshot
         state = self.engine.simulation.context.getState(getVelocities=True,
                                                         getPositions=True)
@@ -157,30 +155,30 @@
         assert(new_snap is not snap0)
         assert(new_snap.statics is not snap0.statics)
         assert(new_snap.kinetics is not snap0.kinetics)
         old_pos = old_div(snap0.coordinates, u.nanometers)
         new_pos = old_div(new_snap.coordinates, u.nanometers)
         old_vel = old_div(snap0.velocities, (old_div(u.nanometers, u.picoseconds)))
         new_vel = old_div(new_snap.velocities, (old_div(u.nanometers, u.picoseconds)))
-        assert_equal(old_pos.shape, new_pos.shape)
-        assert_equal(old_vel.shape, new_vel.shape)
+        assert old_pos.shape == new_pos.shape
+        assert old_vel.shape == new_vel.shape
         assert_not_equal_array_array(old_pos, new_pos)
         assert_not_equal_array_array(old_vel, new_vel)
 
     def test_generate(self):
         try:
             _ = self.engine.generate(self.engine.current_snapshot, [true_func])
         except dyn.EngineMaxLengthError as e:
             traj = e.last_trajectory
-            assert_equal(len(traj), self.engine.n_frames_max)
+            assert len(traj) == self.engine.n_frames_max
         else:
             raise RuntimeError('Did not have correct MaxLengthError')
 
     def test_snapshot_timestep(self):
-        assert_equal(self.engine.snapshot_timestep, 4 * u.femtoseconds)
+        assert self.engine.snapshot_timestep == 4 * u.femtoseconds
 
     @raises_with_message_like(paths.engines.EngineMaxLengthError,
                               "Hit maximal length")
     def test_fail_length(self):
         self.engine.options['on_max_length'] = 'fail'
         self.engine.options['n_max_length'] = 2
         _ = self.engine.generate(self.engine.current_snapshot, [true_func])
@@ -220,23 +218,23 @@
             ensemble=tps,
             selector=paths.UniformSelector(),
             engine=self.engine
         )
         change = mover.move(init_samp)
 
         assert (isinstance(change, paths.RejectedNaNSampleMoveChange))
-        assert_equal(change.details.rejection_reason, 'nan')
+        assert change.details.rejection_reason == 'nan'
         # since we shoot, we start with a shorter trajectory
         assert(len(change.samples[0].trajectory) < len(init_traj))
 
         newsamp = init_samp.apply_samples(change)
-        assert_equal(len(newsamp), 1)
+        assert len(newsamp) == 1
 
         # make sure there is no change!
-        assert_equal(init_samp[0].trajectory, init_traj)
+        assert init_samp[0].trajectory == init_traj
 
     def test_max_length_rejected(self):
         stateA = paths.EmptyVolume()  # will run indefinitely
         stateB = paths.EmptyVolume()
         tps = A2BEnsemble(stateA, stateB)
         self.engine.options['n_frames_max'] = 10
         self.engine.on_max_length = 'fail'
@@ -252,23 +250,22 @@
             ensemble=tps,
             selector=paths.UniformSelector(),
             engine=self.engine
         )
         change = mover.move(init_samp)
 
         assert(isinstance(change, paths.RejectedMaxLengthSampleMoveChange))
-        assert_equal(change.details.rejection_reason, 'max_length')
-        assert_equal(
-            len(change.samples[0].trajectory), self.engine.n_frames_max)
+        assert change.details.rejection_reason == 'max_length'
+        assert len(change.samples[0].trajectory) == self.engine.n_frames_max
 
         newsamp = init_samp.apply_samples(change)
-        assert_equal(len(newsamp), 1)
+        assert len(newsamp) == 1
 
         # make sure there is no change!
-        assert_equal(init_samp[0].trajectory, init_traj)
+        assert init_samp[0].trajectory == init_traj
 
     @pytest.mark.parametrize('has_constraints', [True, False])
     def test_has_constraints(self, has_constraints):
         omt = pytest.importorskip('openmmtools')
         constraints = app.HBonds if has_constraints else None
         system = omt.testsystems.AlanineDipeptideVacuum(
             constraints=constraints
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_openmm_snapshot.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_openmm_snapshot.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from __future__ import division
 from __future__ import absolute_import
 from builtins import object
 import openpathsampling.engines.openmm as omm_engine
 import openpathsampling as paths
-from nose.tools import (assert_equal, assert_almost_equal, assert_not_equal,
-                        assert_is_not, assert_is)
-from nose.plugins.skip import SkipTest
 from .test_helpers import data_filename, assert_close_unit, u
 
 import pytest
 
 try:
     import openmmtools as omt
 except ImportError:
@@ -24,18 +21,18 @@
 logging.getLogger('openpathsampling.ensemble').setLevel(logging.CRITICAL)
 logging.getLogger('openpathsampling.storage').setLevel(logging.CRITICAL)
 logging.getLogger('openpathsampling.netcdfplus').setLevel(logging.CRITICAL)
 
 class TestOpenMMSnapshot(object):
     def setup_method(self):
         if not openmm:
-            raise SkipTest("OpenMM not installed")
+            pytest.skip("OpenMM not installed")
         if not omt:
-            raise SkipTest("OpenMMTools not installed; required for OpenMM "
-                           "tests.")
+            pytest.skip("OpenMMTools not installed; required for OpenMM "
+                        "tests.")
         self.test_system = omt.testsystems.AlanineDipeptideVacuum()
         self.template = omm_engine.snapshot_from_testsystem(self.test_system)
         self.engine = omm_engine.Engine(
             topology=self.template.topology,
             system=self.test_system.system,
             integrator=omt.integrators.VVVRIntegrator()
         )
@@ -45,15 +42,15 @@
             box_vectors=self.template.box_vectors,
             velocities=self.template.velocities,
             engine=self.engine
         )
 
     def test_masses_from_file(self):
         masses = self.template.masses
-        assert_equal(len(masses), self.n_atoms)
+        assert len(masses) == self.n_atoms
 
     def test_masses_from_simulation(self):
         assert len(self.test_snap.masses) == self.n_atoms
 
     def test_masses_for_virtual_sites(self):
         snap = omm_engine.snapshot_from_pdb(data_filename("tip4p_water.pdb"))
         snap_masses = snap.masses
@@ -82,23 +79,23 @@
                           expected_ke / u.BOLTZMANN_CONSTANT_kB / n_dofs)
 
     def test_instantaneous_temperature_changes(self):
         trajectory = self.engine.generate(self.template,
                                           [lambda t, foo: len(t) < 4])
         temp_1 = trajectory[1].instantaneous_temperature
         temp_2 = trajectory[2].instantaneous_temperature
-        assert_not_equal(temp_1, temp_2)
+        assert temp_1 != temp_2
 
     def test_mdtraj_trajectory(self):
         snap_1 = omm_engine.snapshot_from_testsystem(self.test_system,
                                                      periodic=False)
-        assert_is(snap_1.box_vectors, None)
+        assert snap_1.box_vectors is None
         traj_1 = snap_1.md
-        assert_equal(len(traj_1), 1)
-        assert_is_not(traj_1.xyz, None)
-        assert_is(traj_1.unitcell_vectors, None)
+        assert len(traj_1) == 1
+        assert traj_1.xyz is not None
+        assert traj_1.unitcell_vectors is None
 
         snap_2 = self.test_snap
         traj_2 = snap_2.md
-        assert_equal(len(traj_2), 1)
-        assert_is_not(traj_2.xyz, None)
-        assert_is_not(traj_2.unitcell_vectors, None)
+        assert len(traj_2) == 1
+        assert traj_2.xyz is not None
+        assert traj_2.unitcell_vectors is not None
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_openmm_tools.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_openmm_tools.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_part_in_b_tps.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_part_in_b_tps.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from __future__ import absolute_import
-from nose.tools import (assert_equal, assert_not_equal, assert_almost_equal,
-                        raises)
 import logging
 from openpathsampling.high_level.part_in_b_tps import *
 from .test_network import TestFixedLengthTPSNetwork
 
 logging.getLogger('openpathsampling.initialization').setLevel(logging.CRITICAL)
 logging.getLogger('openpathsampling.ensemble').setLevel(logging.CRITICAL)
 logging.getLogger('openpathsampling.storage').setLevel(logging.CRITICAL)
@@ -13,20 +11,20 @@
 class TestPartInBNetwork(TestFixedLengthTPSNetwork):
     NetworkType = PartInBFixedLengthTPSNetwork
 
     def test_allow_self_transitions_false_ABX(self):
         network = self.NetworkType.from_states_all_to_all(
             self.states, allow_self_transitions=False, **self.std_kwargs
         )
-        assert_equal(len(network.sampling_ensembles), 1)
+        assert len(network.sampling_ensembles) == 1
         ensemble = network.sampling_ensembles[0]
-        assert_equal(ensemble(self.traj['AB0']), True)
-        assert_equal(ensemble(self.traj['ABA']), True)
+        assert ensemble(self.traj['AB0'])
+        assert ensemble(self.traj['ABA'])
 
     def test_allow_self_transitions_true_ABX(self):
         network = self.NetworkType.from_states_all_to_all(
             self.states, allow_self_transitions=True, **self.std_kwargs
         )
-        assert_equal(len(network.sampling_ensembles), 1)
+        assert len(network.sampling_ensembles) == 1
         ensemble = network.sampling_ensembles[0]
-        assert_equal(ensemble(self.traj['AB0']), True)
-        assert_equal(ensemble(self.traj['ABA']), True)
+        assert ensemble(self.traj['AB0'])
+        assert ensemble(self.traj['ABA'])
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_path_histogram.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_path_histogram.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,14 @@
 from builtins import object
 import os
 import numpy as np
 import collections
 
 import pytest
 
-from nose.tools import (assert_equal, assert_not_equal, assert_almost_equal,
-                        raises)
-from nose.plugins.skip import Skip, SkipTest
 from .test_helpers import (
     true_func, assert_equal_array_array, make_1d_traj, data_filename,
     assert_items_almost_equal
 )
 
 import openpathsampling as paths
 import logging
@@ -63,17 +60,17 @@
     def test_same_cell(self):
         # check interpolation if successive frames in same cell
         traj = [(0.1, 0.3), (0.2, 0.2), (0.4, 0.6), (0.3, 0.1)]
         hist = PathHistogram(left_bin_edges=(0.0, 0.0),
                              bin_widths=(0.5, 0.5),
                              interpolate=self.Interpolator, per_traj=False)
         hist.add_trajectory(traj)
-        assert_equal(len(list(hist._histogram.keys())), 2)
-        assert_equal(hist._histogram[(0,0)], 3)
-        assert_equal(hist._histogram[(0,1)], 1)
+        assert len(list(hist._histogram.keys())) == 2
+        assert hist._histogram[(0,0)] == 3
+        assert hist._histogram[(0,1)] == 1
 
 
 class TestPathHistogramNoInterpolate(PathHistogramTester):
     Interpolator = NoInterpolation
     def setup_method(self):
         super(TestPathHistogramNoInterpolate, self).setup_method()
         self.expected_bins = [(0, 0), (4, 6), (3, 2),
@@ -150,56 +147,56 @@
                              interpolate=SubdivideInterpolation,
                              per_traj=True)
         hist.add_trajectory(self.trajectory)
         hist.add_trajectory(self.diag, weight=2)
         for val in [(0,1), (0,2), (0,3), (1,2), (1,3), (1,4), (2,1), (2,3),
                     (2,4), (2,5), (3,1), (3,2), (3,4), (3,5), (3,6), (4,5),
                     (4,6)]:
-            assert_equal(hist._histogram[val], 1.0)
+            assert hist._histogram[val] == 1.0
         for val in [(2,2), (4,4)]:
-            assert_equal(hist._histogram[val], 2.0)
+            assert hist._histogram[val] == 2.0
         for val in [(0,0), (1,1), (3,3)]:
-            assert_equal(hist._histogram[val], 3.0)
+            assert hist._histogram[val] == 3.0
         for val in [(0,4), (0,5), (0.6), (0,7), (-1,0)]:
-            assert_equal(hist._histogram[val], 0.0)
+            assert hist._histogram[val] == 0.0
 
     def test_add_data_to_histograms(self):
         hist = PathHistogram(left_bin_edges=(0.0, 0.0),
                              bin_widths=(0.5, 0.5),
                              interpolate=SubdivideInterpolation,
                              per_traj=True)
         counter = hist.add_data_to_histogram([self.trajectory, self.diag],
                                              weights=[1.0, 2.0])
         for val in [(0,1), (0,2), (0,3), (1,2), (1,3), (1,4), (2,1), (2,3),
                     (2,4), (2,5), (3,1), (3,2), (3,4), (3,5), (3,6), (4,5),
                     (4,6)]:
-            assert_equal(counter[val], 1.0)
+            assert counter[val] == 1.0
         for val in [(2,2), (4,4)]:
-            assert_equal(counter[val], 2.0)
+            assert counter[val] == 2.0
         for val in [(0,0), (1,1), (3,3)]:
-            assert_equal(counter[val], 3.0)
+            assert counter[val] == 3.0
         for val in [(0,4), (0,5), (0.6), (0,7), (-1,0)]:
-            assert_equal(counter[val], 0.0)
+            assert counter[val] == 0.0
 
     def test_add_data_to_histograms_no_weight(self):
         hist = PathHistogram(left_bin_edges=(0.0, 0.0),
                              bin_widths=(0.5, 0.5),
                              interpolate=SubdivideInterpolation,
                              per_traj=True)
         counter = hist.add_data_to_histogram([self.trajectory, self.diag])
         for val in [(0,1), (0,2), (0,3), (1,2), (1,3), (1,4), (2,1), (2,3),
                     (2,4), (2,5), (3,1), (3,2), (3,4), (3,5), (3,6), (4,5),
                     (4,6)]:
-            assert_equal(counter[val], 1.0)
+            assert counter[val] == 1.0
         for val in [(2,2), (4,4)]:
-            assert_equal(counter[val], 1.0)
+            assert counter[val] == 1.0
         for val in [(0,0), (1,1), (3,3)]:
-            assert_equal(counter[val], 2.0)
+            assert counter[val] == 2.0
         for val in [(0,4), (0,5), (0.6), (0,7), (-1,0)]:
-            assert_equal(counter[val], 0.0)
+            assert counter[val] == 0.0
 
 
 class TestPathDensityHistogram(object):
     def setup_method(self):
         self.HAS_TQDM = paths.progress.HAS_TQDM
         paths.progress.HAS_TQDM = False
         id_cv = paths.FunctionCV("Id",
@@ -221,43 +218,43 @@
     def teardown_method(self):
         paths.progress.HAS_TQDM = self.HAS_TQDM
 
     def test_histogram_no_weights(self):
         hist = PathDensityHistogram(self.cvs, self.left_bin_edges,
                                     self.bin_widths)
         counter = hist.histogram([self.traj1, self.traj2])
-        assert_equal(len(counter), 5)
+        assert len(counter) == 5
         for bin_label in [(0,0,0), (2,0,0), (1,0,0), (2,1,1)]:
-            assert_equal(counter[bin_label], 1.0)
-        assert_equal(counter[(2,1,0)], 2.0)
+            assert counter[bin_label] == 1.0
+        assert counter[(2,1,0)] == 2.0
         for bin_label in [(1,1,1), (2,2,2), (-1,0,0), (0,-1,0)]:
-            assert_equal(counter[bin_label], 0.0)
+            assert counter[bin_label] == 0.0
 
     def test_histogram_with_weights(self):
         hist = PathDensityHistogram(self.cvs, self.left_bin_edges,
                                     self.bin_widths)
         counter = hist.histogram([self.traj1, self.traj2],
                                  weights=[1.0, 2.0])
-        assert_equal(len(counter), 5)
+        assert len(counter) == 5
         for bin_label in [(0,0,0), (2,0,0), (1,0,0)]:
-            assert_equal(counter[bin_label], 1.0)
-        assert_equal(counter[(2,1,1)], 2.0)
-        assert_equal(counter[(2,1,0)], 3.0)
+            assert counter[bin_label] == 1.0
+        assert counter[(2,1,1)] == 2.0
+        assert counter[(2,1,0)] == 3.0
         for bin_label in [(1,1,1), (2,2,2), (-1,0,0), (0,-1,0)]:
-            assert_equal(counter[bin_label], 0.0)
+            assert counter[bin_label] == 0.0
 
     def test_histogram_single_traj(self):
         hist = PathDensityHistogram(self.cvs, self.left_bin_edges,
                                     self.bin_widths)
         counter = hist.histogram(self.traj1)
-        assert_equal(len(counter), 4)
+        assert len(counter) == 4
         for bin_label in [(0,0,0), (2,0,0), (1,0,0), (2,1,0)]:
-            assert_equal(counter[bin_label], 1.0)
+            assert counter[bin_label] == 1.0
         for bin_label in [(1,1,1), (2,2,2), (-1,0,0), (0,-1,0)]:
-            assert_equal(counter[bin_label], 0.0)
+            assert counter[bin_label] == 0.0
 
     def test_map_to_float_bins_trajectory(self):
         hist = PathDensityHistogram(self.cvs, self.left_bin_edges,
                                     self.bin_widths)
         bin_traj = hist.map_to_float_bins(self.traj2)
         # cv_traj = [[0.6, 0.564642473395035, 0.36],
         #            [0.7, 0.644217687237691, 0.49]]
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_pathmover.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_pathmover.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_pathsimulator.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_pathsimulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import division
 from __future__ import absolute_import
 from builtins import str
 from builtins import range
 from past.utils import old_div
 from builtins import object
+
+import pytest
 from .test_helpers import (raises_with_message_like, data_filename,
                            CalvinistDynamics, make_1d_traj,
                            assert_items_equal)
-from nose.tools import (assert_equal, assert_not_equal, raises,
-                        assert_almost_equal, assert_true, assert_greater)
-# from nose.plugins.skip import SkipTest
+from numpy.testing import assert_almost_equal
 
 from openpathsampling.pathsimulators import *
 import openpathsampling as paths
 import openpathsampling.engines.toy as toys
 import numpy as np
 import os
 
@@ -61,86 +61,86 @@
         self.snapA = make_1d_traj([-0.5])[0]
 
         self.noforbid_noextra_AB = paths.FullBootstrapping(
             transition=self.tisAB,
             snapshot=self.snapA
         )
 
-    @raises(RuntimeError)
     def test_initial_max_length(self):
         engine = CalvinistDynamics([-0.5, -0.4, -0.3, -0.2, -0.1, 0.1, -0.1])
         bootstrap_AB_maxlength = paths.FullBootstrapping(
             transition=self.tisAB,
             snapshot=self.snapA,
             initial_max_length=3,
             engine=engine
         )
         bootstrap_AB_maxlength.output_stream = open(os.devnull, "w")
-        bootstrap_AB_maxlength.run(build_attempts=1)
+        with pytest.raises(RuntimeError):
+            bootstrap_AB_maxlength.run(build_attempts=1)
 
     def test_first_traj_ensemble(self):
         traj_starts_in = make_1d_traj([-0.2, -0.1, 0.1, -0.1])
         traj_starts_out = make_1d_traj([0.1, -0.1, 0.1, -0.1])
         traj_not_good = make_1d_traj([0.1, -0.1, 0.1])
         first_traj_ens = self.noforbid_noextra_AB.first_traj_ensemble
-        assert_equal(first_traj_ens(traj_starts_in), True)
-        assert_equal(first_traj_ens(traj_starts_out), True)
-        assert_equal(first_traj_ens(traj_not_good), False)
+        assert first_traj_ens(traj_starts_in)
+        assert first_traj_ens(traj_starts_out)
+        assert not first_traj_ens(traj_not_good)
 
     def test_sampling_ensembles(self):
         traj1 = make_1d_traj([-0.2, -0.1, 0.1, -0.1])
         traj2 = make_1d_traj([-0.1, 0.1, -0.1])
         traj3 = make_1d_traj([-0.1, 0.1, 0.3, -0.1])
         traj4 = make_1d_traj([0.1, 0.3, 0.1])
         all_ensembles = self.noforbid_noextra_AB.all_ensembles
-        assert_equal(len(all_ensembles), 3)
+        assert len(all_ensembles) == 3
         for ens in all_ensembles:
-            assert_equal(ens(traj1), False)
-            assert_equal(ens(traj4), False)
-        assert_equal(all_ensembles[0](traj2), True)
-        assert_equal(all_ensembles[0](traj3), True)
-        assert_equal(all_ensembles[1](traj2), False)
-        assert_equal(all_ensembles[1](traj3), True)
-        assert_equal(all_ensembles[2](traj2), False)
-        assert_equal(all_ensembles[2](traj3), False)
+            assert not ens(traj1)
+            assert not ens(traj4)
+        assert all_ensembles[0](traj2)
+        assert all_ensembles[0](traj3)
+        assert not all_ensembles[1](traj2)
+        assert all_ensembles[1](traj3)
+        assert not all_ensembles[2](traj2)
+        assert not all_ensembles[2](traj3)
 
     def test_run_already_satisfied(self):
         engine = CalvinistDynamics([-0.5, 0.8, -0.1])
         bootstrap = FullBootstrapping(
             transition=self.tisAB,
             snapshot=self.snapA,
             engine=engine
         )
         bootstrap.output_stream = open(os.devnull, "w")
         gs = bootstrap.run()
-        assert_equal(len(gs), 3)
+        assert len(gs) == 3
 
     def test_run_extra_interfaces(self):
         engine = CalvinistDynamics([-0.5, 0.8, -0.1])
         bootstrap = FullBootstrapping(
             transition=self.tisAB,
             snapshot=self.snapA,
             engine=engine,
             extra_interfaces=[paths.CVDefinedVolume(self.cv, -1.0, 0.6)]
         )
         bootstrap.output_stream = open(os.devnull, "w")
         gs = bootstrap.run()
-        assert_equal(len(gs), 4)
+        assert len(gs) == 4
 
     def test_run_forbidden_states(self):
         engine = CalvinistDynamics([-0.5, 0.3, 3.2, -0.1, 0.8, -0.1])
         # first, without setting forbidden_states
         bootstrap1 = FullBootstrapping(
             transition=self.tisAB,
             snapshot=self.snapA,
             engine=engine
         )
         bootstrap1.output_stream = open(os.devnull, "w")
         gs1 = bootstrap1.run()
-        assert_equal(len(gs1), 3)
+        assert len(gs1) == 3
         assert_items_equal(self.cv(gs1[0]), [-0.5, 0.3, 3.2, -0.1])
         # now with setting forbidden_states
         bootstrap2 = FullBootstrapping(
             transition=self.tisAB,
             snapshot=self.snapA,
             engine=engine,
             forbidden_states=[self.stateC]
@@ -148,24 +148,24 @@
         bootstrap2.output_stream = open(os.devnull, "w")
         # make sure this is where we get the error
         try:
             bootstrap2.run()
         except RuntimeError:
             pass
 
-    @raises(RuntimeError)
     def test_too_much_bootstrapping(self):
         engine = CalvinistDynamics([-0.5, 0.2, -0.1])
         bootstrap = FullBootstrapping(
             transition=self.tisAB,
             snapshot=self.snapA,
             engine=engine,
         )
         bootstrap.output_stream = open(os.devnull, "w")
-        bootstrap.run(max_ensemble_rounds=1)
+        with pytest.raises(RuntimeError):
+            bootstrap.run(max_ensemble_rounds=1)
 
 
 class TestShootFromSnapshotsSimulation(object):
     # note that most of ShootFromSnapshotSimulation is tested in the tests
     # for CommittorSimulation. This is just an additional test to show that
     # using different ensembles from the ones used for the committor will
     # also work.
@@ -211,28 +211,28 @@
 
     def test_run_arbitrary_ensemble(self):
         # integration test of the whole thing, including storage
         self.simulation.run(10)
         self.storage.close()
         analysis = paths.Storage(self.filename, 'r')
         sim = analysis.pathsimulators[0]
-        assert_equal(len(analysis.steps), 10)
+        assert len(analysis.steps) == 10
         length_to_submover = {5: [], 3: []}
         for step in analysis.steps:
             step.active.sanity_check()
-            assert_equal(len(step.active), 1)
+            assert len(step.active) == 1
             active_sample = step.active[0]
             change = step.change
-            assert_equal(change.mover, sim.mover)
+            assert change.mover == sim.mover
             # KeyError here indicates problem with lengths generated
             length_to_submover[len(active_sample)] += change.subchange.mover
 
         for k in length_to_submover:
             # allow 0 or 1  because maybe we made no trials with submover
-            assert_true(len(set(length_to_submover[k])) <= 1)
+            assert len(set(length_to_submover[k])) <= 1
 
 
 class TestCommittorSimulation(object):
     def setup_method(self):
         # As a test system, let's use 1D motion on a flat potential. If the
         # velocity is positive, you right the state on the right. If it is
         # negative, you hit the state on the left.
@@ -272,16 +272,16 @@
         self.storage.close()
         if os.path.isfile(self.filename):
             os.remove(self.filename)
         paths.EngineMover.default_engine = None
 
     def test_initialization(self):
         sim = self.simulation  # convenience
-        assert_equal(len(sim.initial_snapshots), 1)
-        assert_true(isinstance(sim.mover, paths.RandomChoiceMover))
+        assert len(sim.initial_snapshots) == 1
+        assert isinstance(sim.mover, paths.RandomChoiceMover)
 
     def test_storage(self):
         self.storage.tag['simulation'] = self.simulation
         self.storage.close()
         read_store = paths.Storage(self.filename, 'r')
         sim = read_store.tag['simulation']
         new_filename = data_filename("test2.nc")
@@ -291,141 +291,135 @@
         sim.storage.close()
         if os.path.isfile(new_filename):
             os.remove(new_filename)
         self.storage = read_store  # teardown will get rid of this
 
     def test_committor_run(self):
         self.simulation.run(n_per_snapshot=20)
-        assert_equal(len(self.simulation.storage.steps), 20)
+        assert len(self.simulation.storage.steps) == 20
         counts = {'fwd': 0, 'bkwd': 0}
         for step in self.simulation.storage.steps:
             step.active.sanity_check()  # traj is in ensemble
             traj = step.active[0].trajectory
             traj_str = traj.summarize_by_volumes_str(self.state_labels)
             if traj_str == "None-Right":
-                assert_equal(step.change.canonical.mover,
-                             self.simulation.forward_mover)
-                assert_equal(step.active[0].ensemble,
-                             self.simulation.forward_ensemble)
+                assert (step.change.canonical.mover
+                        == self.simulation.forward_mover)
+                assert (step.active[0].ensemble
+                        == self.simulation.forward_ensemble)
                 counts['fwd'] += 1
             elif traj_str == "Left-None":
-                assert_equal(step.change.canonical.mover,
-                             self.simulation.backward_mover)
-                assert_equal(step.active[0].ensemble,
-                             self.simulation.backward_ensemble)
+                assert (step.change.canonical.mover
+                        == self.simulation.backward_mover)
+                assert (step.active[0].ensemble
+                        == self.simulation.backward_ensemble)
                 counts['bkwd'] += 1
             else:
                 raise AssertionError(
                     str(traj_str) + "is neither 'None-Right' nor 'Left-None'"
                 )
-        assert_true(counts['fwd'] > 0)
-        assert_true(counts['bkwd'] > 0)
-        assert_equal(counts['fwd'] + counts['bkwd'], 20)
+        assert counts['fwd'] > 0
+        assert counts['bkwd'] > 0
+        assert counts['fwd'] + counts['bkwd'] == 20
 
     def test_forward_only_committor(self):
         sim = CommittorSimulation(storage=self.storage,
                                   engine=self.engine,
                                   states=[self.left, self.right],
                                   randomizer=paths.NoModification(),
                                   initial_snapshots=self.snap0,
                                   direction=1)
         sim.output_stream = open(os.devnull, 'w')
         sim.run(n_per_snapshot=10)
-        assert_equal(len(sim.storage.steps), 10)
+        assert len(sim.storage.steps) == 10
         for step in self.simulation.storage.steps:
             s = step.active[0]
             step.active.sanity_check()  # traj is in ensemble
-            assert_equal(
-                s.trajectory.summarize_by_volumes_str(self.state_labels),
-                "None-Right"
-            )
-            assert_equal(s.ensemble, sim.forward_ensemble)
-            assert_equal(step.change.canonical.mover,
-                         sim.forward_mover)
+            assert (s.trajectory.summarize_by_volumes_str(self.state_labels)
+                    == "None-Right")
+            assert s.ensemble == sim.forward_ensemble
+            assert step.change.canonical.mover == sim.forward_mover
 
     def test_backward_only_committor(self):
         sim = CommittorSimulation(storage=self.storage,
                                   engine=self.engine,
                                   states=[self.left, self.right],
                                   randomizer=paths.NoModification(),
                                   initial_snapshots=self.snap0,
                                   direction=-1)
         sim.output_stream = open(os.devnull, 'w')
         sim.run(n_per_snapshot=10)
-        assert_equal(len(sim.storage.steps), 10)
+        assert len(sim.storage.steps) == 10
         for step in self.simulation.storage.steps:
             s = step.active[0]
             step.active.sanity_check()  # traj is in ensemble
-            assert_equal(
-                s.trajectory.summarize_by_volumes_str(self.state_labels),
-                "Left-None"
-            )
-            assert_equal(s.ensemble, sim.backward_ensemble)
-            assert_equal(step.change.canonical.mover,
-                         sim.backward_mover)
+            assert (s.trajectory.summarize_by_volumes_str(self.state_labels)
+                    == "Left-None")
+            assert s.ensemble == sim.backward_ensemble
+            assert step.change.canonical.mover == sim.backward_mover
 
     def test_multiple_initial_snapshots(self):
         snap1 = toys.Snapshot(coordinates=np.array([[0.1]]),
                               velocities=np.array([[-1.0]]),
                               engine=self.engine)
         sim = CommittorSimulation(storage=self.storage,
                                   engine=self.engine,
                                   states=[self.left, self.right],
                                   randomizer=paths.NoModification(),
                                   initial_snapshots=[self.snap0, snap1])
         sim.output_stream = open(os.devnull, 'w')
         sim.run(10)
-        assert_equal(len(self.storage.steps), 20)
+        assert len(self.storage.steps) == 20
         snap0_coords = self.snap0.coordinates.tolist()
         snap1_coords = snap1.coordinates.tolist()
         count = {self.snap0: 0, snap1: 0}
         for step in self.storage.steps:
             shooting_snap = step.change.canonical.details.shooting_snapshot
             if shooting_snap.coordinates.tolist() == snap0_coords:
                 mysnap = self.snap0
             elif shooting_snap.coordinates.tolist() == snap1_coords:
                 mysnap = snap1
             else:
                 msg = "Shooting snapshot matches neither test snapshot"
                 raise AssertionError(msg)
             count[mysnap] += 1
-        assert_equal(count, {self.snap0: 10, snap1: 10})
+        assert count == {self.snap0: 10, snap1: 10}
 
     def test_randomized_committor(self):
         # this shows that we get both states even with forward-only
         # shooting, if the randomizer gives the negative velocities
         randomizer = paths.RandomVelocities(beta=1.0)
         sim = CommittorSimulation(storage=self.storage,
                                   engine=self.engine,
                                   states=[self.left, self.right],
                                   randomizer=randomizer,
                                   initial_snapshots=self.snap0,
                                   direction=1)
         sim.output_stream = open(os.devnull, 'w')
         sim.run(50)
-        assert_equal(len(sim.storage.steps), 50)
+        assert len(sim.storage.steps) == 50
         counts = {'None-Right': 0,
                   'Left-None': 0,
                   'None-Left': 0,
                   'Right-None': 0}
         for step in sim.storage.steps:
             step.active.sanity_check()  # traj is in ensemble
             traj = step.active[0].trajectory
             traj_str = traj.summarize_by_volumes_str(self.state_labels)
             try:
                 counts[traj_str] += 1
             except KeyError:
                 msg = "Got trajectory described as '{0}', length {1}"
                 # this might be okay if it is 'None', length 100000
                 raise AssertionError(msg.format(traj_str, len(traj)))
-        assert_equal(counts['Left-None'], 0)
-        assert_equal(counts['Right-None'], 0)
-        assert_true(counts['None-Left'] > 0)
-        assert_true(counts['None-Right'] > 0)
-        assert_equal(sum(counts.values()), 50)
+        assert counts['Left-None'] == 0
+        assert counts['Right-None'] == 0
+        assert counts['None-Left'] > 0
+        assert counts['None-Right'] > 0
+        assert sum(counts.values()) == 50
 
 
 class TestReactiveFluxSimulation(object):
     def setup_method(self):
         # PES is one-dimensional linear slope (y(x) = x)
         pes = toys.LinearSlope(m=[-1.0], c=[0.0])
         # one particle with mass 1.0
@@ -487,66 +481,60 @@
     def teardown_method(self):
         if os.path.isfile(self.filename):
             os.remove(self.filename)
         paths.EngineMover.default_engine = None
 
     def test_initialization(self):
         sim = self.simulation
-        assert_equal(len(sim.initial_snapshots), 3)
-        assert_true(isinstance(sim.mover, paths.ConditionalSequentialMover))
+        assert len(sim.initial_snapshots) == 3
+        assert isinstance(sim.mover, paths.ConditionalSequentialMover)
 
     def test_simulation_run(self):
         self.simulation.run(n_per_snapshot=1)
-        assert_equal(len(self.simulation.storage.steps), 3)
+        assert len(self.simulation.storage.steps) == 3
 
         # snapshot 0, fails at backward shot (falls back to dividing surface)
         step = self.simulation.storage.steps[0]
         # last mover should be backward_mover of simulation
-        assert_equal(step.change.canonical.mover,
-                     self.simulation.backward_mover)
+        assert step.change.canonical.mover == self.simulation.backward_mover
         # active ensemble should be starting ensemble
-        assert_equal(step.active[0].ensemble,
-                     self.simulation.starting_ensemble)
+        assert step.active[0].ensemble == self.simulation.starting_ensemble
         # analyze trajectory, last step should be in 'None', the rest in 'ToA'
         traj = step.change.trials[0].trajectory
         traj_summary = traj.summarize_by_volumes(self.state_labels)
-        assert_equal(traj_summary[0], ('None', 1))
-        assert_equal(traj_summary[1][0], 'ToA')
-        assert_greater(traj_summary[1][1], 1)
+        assert traj_summary[0] == ('None', 1)
+        assert traj_summary[1][0] == 'ToA'
+        assert traj_summary[1][1] > 1
 
         # snapshot 1, fails at backward shot (wrong direction)
         step = self.simulation.storage.steps[1]
         # last mover should be backward_mover of simulation
-        assert_equal(step.change.canonical.mover,
-                     self.simulation.backward_mover)
+        assert step.change.canonical.mover == self.simulation.backward_mover
         # active ensemble should be starting ensemble
-        assert_equal(step.active[0].ensemble,
-                     self.simulation.starting_ensemble)
+        assert step.active[0].ensemble == self.simulation.starting_ensemble
         # analyze trajectory, backwards trajectory reaches immediately 'None'
         traj = step.change.trials[0].trajectory
         traj_summary = traj.summarize_by_volumes(self.state_labels)
-        assert_equal(traj_summary[0], ('None', 2))
+        assert traj_summary[0] == ('None', 2)
 
         # snapshot 2, is accepted
         step = self.simulation.storage.steps[2]
         # last mover should be forward_mover of simulation
-        assert_equal(step.change.canonical.mover,
-                     self.simulation.forward_mover)
+        assert step.change.canonical.mover == self.simulation.forward_mover
         # active ensemble should not be starting ensemble
-        assert_not_equal(step.active[0].ensemble,
-                     self.simulation.starting_ensemble)
+        assert step.active[0].ensemble != self.simulation.starting_ensemble
         # analyze active trajectory, trajectory should start in 'A', end in 'B'
         traj = step.active[0].trajectory
         traj_summary = traj.summarize_by_volumes(self.state_labels)
-        assert_equal(traj_summary[0], ('A', 1))
-        assert_equal(traj_summary[1][0], 'ToA')
-        assert_greater(traj_summary[1][1], 1)
-        assert_equal(traj_summary[2][0], 'None')
-        assert_greater(traj_summary[2][1], 1)
-        assert_equal(traj_summary[3], ('B', 1))
+        assert traj_summary[0] == ('A', 1)
+        assert traj_summary[1][0] == 'ToA'
+        assert traj_summary[1][1] > 1
+        assert traj_summary[2][0] == 'None'
+        assert traj_summary[2][1] > 1
+        assert traj_summary[3] == ('B', 1)
 
 
 class TestDirectSimulation(object):
     def setup_method(self):
         pes = toys.HarmonicOscillator(A=[1.0], omega=[1.0], x0=[0.0])
         topology = toys.Topology(n_spatial=1, masses=[1.0], pes=pes)
         integrator = toys.LeapfrogVerletIntegrator(0.1)
@@ -570,25 +558,24 @@
                                     engine=self.engine,
                                     states=[self.center, self.outside],
                                     flux_pairs=self.flux_pairs,
                                     initial_snapshot=self.snap0)
 
     def test_run(self):
         self.sim.run(200)
-        assert_true(len(self.sim.transition_count) > 1)
-        assert_true(len(self.sim.flux_events[self.flux_pairs[0]]) > 1)
+        assert len(self.sim.transition_count) > 1
+        assert len(self.sim.flux_events[self.flux_pairs[0]]) > 1
 
     def test_results(self):
         self.sim.run(200)
         results = self.sim.results
-        assert_equal(len(results), 2)
-        assert_equal(set(results.keys()),
-                     set(['transition_count', 'flux_events']))
-        assert_equal(results['transition_count'], self.sim.transition_count)
-        assert_equal(results['flux_events'], self.sim.flux_events)
+        assert len(results) == 2
+        assert set(results.keys()) == set(['transition_count', 'flux_events'])
+        assert results['transition_count'] == self.sim.transition_count
+        assert results['flux_events'] == self.sim.flux_events
 
     def test_load_results(self):
         left_interface = paths.CVDefinedVolume(self.cv, -0.3, float("inf"))
         right_interface = paths.CVDefinedVolume(self.cv, float("-inf"), 0.3)
         fake_transition_count = [
             (self.center, 1), (self.outside, 4), (self.center, 7),
             (self.extra, 10), (self.center, 12), (self.outside, 14)
@@ -596,33 +583,31 @@
         fake_flux_events = {(self.center, right_interface):
                             [(15, 3), (23, 15), (48, 23)],
                             (self.center, left_interface):
                             [(97, 34), (160, 97)]}
         results = {'transition_count': fake_transition_count,
                    'flux_events': fake_flux_events}
         self.sim.load_results(results)
-        assert_equal(self.sim.transition_count, fake_transition_count)
-        assert_equal(self.sim.flux_events, fake_flux_events)
+        assert self.sim.transition_count == fake_transition_count
+        assert self.sim.flux_events == fake_flux_events
 
     def test_transitions(self):
         # set fake data
         self.sim.transition_count = [
             (self.center, 1), (self.outside, 4), (self.center, 7),
             (self.extra, 10), (self.center, 12), (self.outside, 14)
         ]
-        assert_equal(self.sim.n_transitions,
-                     {(self.center, self.outside): 2,
-                      (self.outside, self.center): 1,
-                      (self.center, self.extra): 1,
-                      (self.extra, self.center): 1})
-        assert_equal(self.sim.transitions,
-                     {(self.center, self.outside): [3, 2],
-                      (self.outside, self.center): [3],
-                      (self.center, self.extra): [3],
-                      (self.extra, self.center): [2]})
+        assert self.sim.n_transitions == {(self.center, self.outside): 2,
+                                          (self.outside, self.center): 1,
+                                          (self.center, self.extra): 1,
+                                          (self.extra, self.center): 1}
+        assert self.sim.transitions == {(self.center, self.outside): [3, 2],
+                                        (self.outside, self.center): [3],
+                                        (self.center, self.extra): [3],
+                                        (self.extra, self.center): [2]}
 
     def test_rate_matrix(self):
         self.sim.states += [self.extra]
         self.sim.transition_count = [
             (self.center, 1), (self.outside, 4), (self.center, 7),
             (self.extra, 10), (self.center, 12), (self.outside, 14)
         ]
@@ -640,15 +625,15 @@
                                 [1.0/t_outside, nan, nan],
                                 [1.0/t_extra, nan, nan]]) / step_size
         # for some reason, np.testing.assert_allclose(..., equal_nan=True)
         # was raising errors on this input. this hack gets the behavior
         for i in range(len(self.sim.states)):
             for j in range(len(self.sim.states)):
                 if np.isnan(test_matrix[i][j]):
-                    assert_true(np.isnan(rate_matrix[i][j]))
+                    assert np.isnan(rate_matrix[i][j])
                 else:
                     assert_almost_equal(rate_matrix[i][j],
                                         test_matrix[i][j])
 
     def test_fluxes(self):
         left_interface = paths.CVDefinedVolume(self.cv, -0.3, float("inf"))
         right_interface = paths.CVDefinedVolume(self.cv, float("-inf"), 0.3)
@@ -661,15 +646,15 @@
         fake_flux_events = {(self.center, right_interface):
                             [(15, 3), (23, 15), (48, 23)],
                             (self.center, left_interface):
                             [(97, 34), (160, 97)]}
         sim.flux_events = fake_flux_events
         n_flux_events = {(self.center, right_interface): 3,
                          (self.center, left_interface): 2}
-        assert_equal(sim.n_flux_events, n_flux_events)
+        assert sim.n_flux_events == n_flux_events
         time_step = sim.engine.snapshot_timestep
         expected_fluxes = {(self.center, right_interface):
                            1.0 / (((15-3) + (23-15) + (48-23))/3.0) / time_step,
                            (self.center, left_interface):
                            1.0 / (((97-34) + (160-97))/2.0) / time_step}
         for p in expected_fluxes:
             assert_almost_equal(sim.fluxes[p], expected_fluxes[p])
@@ -726,19 +711,19 @@
         sim.run(len(predetermined)-1)
         # subtract 1 from the indices in `predetermined`, b/c 0 index of the
         # traj comes after the found initial step
         expected_flux_events = {
             (state, alpha): [(4, 2), (6, 4), (22, 19)],
             (state, beta): [(9, 6), (12, 9), (22, 17)]
         }
-        assert_equal(len(sim.flux_events), 2)
-        assert_equal(sim.flux_events[(state, alpha)],
-                     expected_flux_events[(state, alpha)])
-        assert_equal(sim.flux_events[(state, beta)],
-                     expected_flux_events[(state, beta)])
+        assert len(sim.flux_events) == 2
+        assert (sim.flux_events[(state, alpha)]
+                == expected_flux_events[(state, alpha)])
+        assert (sim.flux_events[(state, beta)]
+                == expected_flux_events[(state, beta)])
 
     def test_simple_flux(self):
         state = self.center
         interface = self.interface
         A = 0.0
         I = 0.25
         X = 0.35
@@ -750,17 +735,17 @@
         sim = DirectSimulation(storage=None,
                                engine=engine,
                                states=[state],
                                flux_pairs=[(state, interface)],
                                initial_snapshot=init[0])
         sim.run(len(predetermined) - 1)
         expected_flux_events = {(state, interface): [(10, 2)]}
-        assert_equal(len(sim.flux_events), 1)
-        assert_equal(sim.flux_events[(state, interface)],
-                     expected_flux_events[(state, interface)])
+        assert len(sim.flux_events) == 1
+        assert (sim.flux_events[(state, interface)]
+                == expected_flux_events[(state, interface)])
 
     def test_sim_with_storage(self):
         tmpfile = data_filename("direct_sim_test.nc")
         if os.path.isfile(tmpfile):
             os.remove(tmpfile)
 
         storage = paths.Storage(tmpfile, "w", self.snap0)
@@ -768,17 +753,17 @@
                                engine=self.engine,
                                states=[self.center, self.outside],
                                initial_snapshot=self.snap0)
 
         sim.run(200)
         storage.close()
         read_store = paths.AnalysisStorage(tmpfile)
-        assert_equal(len(read_store.trajectories), 1)
+        assert len(read_store.trajectories) == 1
         traj = read_store.trajectories[0]
-        assert_equal(len(traj), 201)
+        assert len(traj) == 201
         read_store.close()
         os.remove(tmpfile)
 
 
 class TestPathSampling(object):
     def setup_method(self):
         paths.InterfaceSet._reset()
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_plumed_wrapper.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_plumed_wrapper.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_progress.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_pyemma_cv.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_pyemma_cv.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_reactive_flux_analysis.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_reactive_flux_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from __future__ import division
 from __future__ import absolute_import
 from builtins import zip
 from builtins import range
 from past.utils import old_div
 from builtins import object
-from nose.tools import (assert_equal, assert_not_equal, raises,
-                        assert_almost_equal, assert_true, assert_in,
-                        assert_raises)
-from nose.plugins.skip import SkipTest
-from numpy.testing import assert_array_almost_equal
+import pytest
+from numpy.testing import assert_array_almost_equal, assert_almost_equal
 from .test_helpers import (make_1d_traj, data_filename, assert_items_equal,
                            assert_same_items)
 
 import openpathsampling as paths
 import openpathsampling.engines as peng
 import numpy as np
 import os
@@ -134,50 +131,50 @@
     def teardown_method(self):
         if os.path.isfile(self.filename):
             self.storage.close()
             os.remove(self.filename)
         paths.EngineMover.default_engine = None
 
     def gradient(self, snapshot):
-        assert_equal(len(snapshot.xyz), 1)
-        assert_equal(len(snapshot.xyz[0]), 1)
+        assert len(snapshot.xyz) == 1
+        assert len(snapshot.xyz[0]) == 1
         return np.array([[1.0]])
 
     def test_analysis(self):
         storage = paths.Storage(self.filename, mode="r")
         self.analysis = paths.ReactiveFluxAnalysis(steps=storage.steps,
                                                    gradient=self.gradient)
 
         # check wrong analyze_single_step() argument
         empty_list = self.analysis.analyze_single_step(3.1415)
-        assert_equal(empty_list, [])
+        assert empty_list == []
 
         # dictionary with three entries returned (mind: trajectories start from
         # x = -0.001, 0.0, 0.001).
-        assert_equal(len(self.analysis), 3)
+        assert len(self.analysis) == 3
 
         # get total and per-snapshot flux.
         flux, flux_dict = self.analysis.flux()
 
         # analyze counters
         for snapshot in flux_dict.keys():
             if snapshot.xyz[0][0] == -0.001:
                 assert_almost_equal(flux_dict[snapshot], 4.0 / 3.0)
-                assert_equal(self.analysis[snapshot]["accepted"], 1)
-                assert_equal(self.analysis[snapshot]["rejected"], 2)
+                assert self.analysis[snapshot]["accepted"] == 1
+                assert self.analysis[snapshot]["rejected"] == 2
                 assert_almost_equal(self.analysis[snapshot]["sumflux"], 4.0)
             elif snapshot.xyz[0][0] == 0.0:
                 assert_almost_equal(flux_dict[snapshot], 7.0 / 4.0)
-                assert_equal(self.analysis[snapshot]["accepted"], 2)
-                assert_equal(self.analysis[snapshot]["rejected"], 2)
+                assert self.analysis[snapshot]["accepted"] == 2
+                assert self.analysis[snapshot]["rejected"] == 2
                 assert_almost_equal(self.analysis[snapshot]["sumflux"], 7.0)
             elif snapshot.xyz[0][0] == 0.001:
                 assert_almost_equal(flux_dict[snapshot], 19.0 / 5.0)
-                assert_equal(self.analysis[snapshot]["accepted"], 3)
-                assert_equal(self.analysis[snapshot]["rejected"], 2)
+                assert self.analysis[snapshot]["accepted"] == 3
+                assert self.analysis[snapshot]["rejected"] == 2
                 assert_almost_equal(self.analysis[snapshot]["sumflux"], 19.0)
 
         # check total flux.
         assert_almost_equal(flux, 30.0 / 12.0)
 
         # check 1D histogram
         # use only two bins, so results of two snapshots are combined.
@@ -199,17 +196,15 @@
             assert_almost_equal(b1, b3)
         assert_almost_equal(hist[0][0], 11.0 / 7.0)
         assert_almost_equal(hist[1][1], 19.0 / 5.0)
 
         # check failure of 3D histogram
         hash3D = lambda snap: (snap.xyz[0][0], snap.xyz[0][0], snap.xyz[0][0])
         bins3D = [-0.0015, 0.0005, 0.0015]
-        assert_raises(RuntimeError,
-                      self.analysis.flux_histogram,
-                      hash3D,
-                      bins3D)
-
-        assert_raises(NotImplementedError, self.analysis.committor)
-        assert_raises(NotImplementedError,
-                      self.analysis.committor_histogram,
-                      hash1D,
-                      bins1D)
+        with pytest.raises(RuntimeError):
+            self.analysis.flux_histogram(hash3D, bins3D)
+
+        with pytest.raises(NotImplementedError):
+            self.analysis.committor()
+
+        with pytest.raises(NotImplementedError):
+            self.analysis.committor_histogram(hash1D, bins1D)
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_resampling_statistics.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_resampling_statistics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import pandas as pd
 from pandas.testing import assert_frame_equal
-from nose.tools import assert_equal
 from .test_helpers import assert_items_equal
 import openpathsampling as paths
 
 import logging
 logging.getLogger('openpathsampling.initialization').setLevel(logging.CRITICAL)
 logging.getLogger('openpathsampling.ensemble').setLevel(logging.CRITICAL)
 logging.getLogger('openpathsampling.storage').setLevel(logging.CRITICAL)
@@ -87,74 +86,74 @@
 
 class TestBlockResampling(object):
     def setup_method(self):
         self.samples = list(range(100))
 
     def test_default_initialization(self):
         resampler = paths.numerics.BlockResampling(self.samples)
-        assert_equal(resampler.n_total_samples, 100)
-        assert_equal(resampler.n_blocks, 20)
-        assert_equal(resampler.n_per_block, 5)
-        assert_equal(len(resampler.blocks), 20)
-        assert_equal(resampler.n_resampled, 100)
-        assert_equal(resampler.unassigned, [])
+        assert resampler.n_total_samples == 100
+        assert resampler.n_blocks == 20
+        assert resampler.n_per_block == 5
+        assert len(resampler.blocks) == 20
+        assert resampler.n_resampled == 100
+        assert resampler.unassigned == []
         assert_items_equal(resampler.blocks[0], list(range(0, 5)))
         assert_items_equal(resampler.blocks[1], list(range(5, 10)))
         assert_items_equal(resampler.blocks[10], list(range(50, 55)))
         assert_items_equal(resampler.blocks[-1], list(range(95, 100)))
 
     def test_n_blocks_initialization(self):
         resampler = paths.numerics.BlockResampling(self.samples, n_blocks=10)
-        assert_equal(resampler.n_total_samples, 100)
-        assert_equal(resampler.n_blocks, 10)
-        assert_equal(resampler.n_per_block, 10)
-        assert_equal(len(resampler.blocks), 10)
-        assert_equal(resampler.n_resampled, 100)
-        assert_equal(resampler.unassigned, [])
+        assert resampler.n_total_samples == 100
+        assert resampler.n_blocks == 10
+        assert resampler.n_per_block == 10
+        assert len(resampler.blocks) == 10
+        assert resampler.n_resampled == 100
+        assert resampler.unassigned == []
         assert_items_equal(resampler.blocks[0], list(range(0, 10)))
         assert_items_equal(resampler.blocks[1], list(range(10, 20)))
         assert_items_equal(resampler.blocks[5], list(range(50, 60)))
         assert_items_equal(resampler.blocks[-1], list(range(90, 100)))
 
         resampler_2 = paths.numerics.BlockResampling(self.samples, n_blocks=8)
-        assert_equal(resampler_2.n_total_samples, 100)
-        assert_equal(resampler_2.n_blocks, 8)
-        assert_equal(resampler_2.n_per_block, 12)
-        assert_equal(resampler_2.n_resampled, 96)
+        assert resampler_2.n_total_samples == 100
+        assert resampler_2.n_blocks == 8
+        assert resampler_2.n_per_block == 12
+        assert resampler_2.n_resampled == 96
         assert_items_equal(resampler_2.blocks[-1], list(range(84, 96)))
         assert_items_equal(resampler_2.unassigned, list(range(96, 100)))
 
     def test_n_per_block_initialization(self):
         resampler = paths.numerics.BlockResampling(self.samples,
                                                    n_per_block=10)
-        assert_equal(resampler.n_total_samples, 100)
-        assert_equal(resampler.n_blocks, 10)
-        assert_equal(resampler.n_per_block, 10)
-        assert_equal(len(resampler.blocks), 10)
-        assert_equal(resampler.n_resampled, 100)
-        assert_equal(resampler.unassigned, [])
+        assert resampler.n_total_samples == 100
+        assert resampler.n_blocks == 10
+        assert resampler.n_per_block == 10
+        assert len(resampler.blocks) == 10
+        assert resampler.n_resampled == 100
+        assert resampler.unassigned == []
         assert_items_equal(resampler.blocks[0], list(range(0, 10)))
         assert_items_equal(resampler.blocks[1], list(range(10, 20)))
         assert_items_equal(resampler.blocks[5], list(range(50, 60)))
         assert_items_equal(resampler.blocks[-1], list(range(90, 100)))
 
         resampler_2 = paths.numerics.BlockResampling(self.samples,
                                                      n_per_block=8)
-        assert_equal(resampler_2.n_total_samples, 100)
-        assert_equal(resampler_2.n_blocks, 12)
-        assert_equal(resampler_2.n_resampled, 96)
+        assert resampler_2.n_total_samples == 100
+        assert resampler_2.n_blocks == 12
+        assert resampler_2.n_resampled == 96
         assert_items_equal(resampler_2.blocks[-1], list(range(88, 96)))
         assert_items_equal(resampler_2.unassigned, list(range(96, 100)))
 
     def test_n_blocks_and_n_per_block_initialization(self):
         resampler = paths.numerics.BlockResampling(self.samples, n_blocks=9,
                                                    n_per_block=10)
-        assert_equal(resampler.n_total_samples, 100)
-        assert_equal(resampler.n_blocks, 9)
-        assert_equal(resampler.n_per_block, 10)
-        assert_equal(len(resampler.blocks), 9)
-        assert_equal(resampler.n_resampled, 90)
+        assert resampler.n_total_samples == 100
+        assert resampler.n_blocks == 9
+        assert resampler.n_per_block == 10
+        assert len(resampler.blocks) == 9
+        assert resampler.n_resampled == 90
         assert_items_equal(resampler.unassigned, list(range(90, 100)))
         assert_items_equal(resampler.blocks[0], list(range(0, 10)))
         assert_items_equal(resampler.blocks[1], list(range(10, 20)))
         assert_items_equal(resampler.blocks[5], list(range(50, 60)))
         assert_items_equal(resampler.blocks[-1], list(range(80, 90)))
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_sample.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_sample.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 '''
 @author: David W.H. Swenson
 '''
 
 from builtins import range
 from builtins import object
-from nose.plugins.skip import SkipTest
-from nose.tools import (assert_equal, raises, assert_true, assert_false)
+import pytest
 from .test_helpers import assert_items_equal, assert_same_items
 
 from openpathsampling.engines.trajectory import Trajectory
 from openpathsampling.ensemble import LengthEnsemble
 from openpathsampling.sample import *
 from openpathsampling.sample import Sample
 
@@ -26,149 +25,148 @@
         self.s1A = Sample(replica=1, trajectory=traj1A, ensemble=self.ensA)
         self.s2B = Sample(replica=2, trajectory=traj2B, ensemble=self.ensB)
         self.s2B_ = Sample(replica=2, trajectory=traj2B_, ensemble=self.ensB)
         self.testset = SampleSet([self.s0A, self.s1A, self.s2B])
 
     def test_equality(self):
         testset2 = SampleSet([self.s0A, self.s1A, self.s2B])
-        assert_true(self.testset == testset2)
-        assert_false(self.testset != testset2)
+        assert self.testset == testset2
 
     def test_initialization(self):
         self.testset.consistency_check()
 
     def test_iter(self):
         samps = [self.s0A, self.s1A, self.s2B]
         for samp in self.testset:
-            assert_equal(samp in samps, True)
+            assert samp in samps
 
     def test_contains(self):
         samps = [self.s0A, self.s1A, self.s2B]
         for samp in samps:
-            assert_equal(samp in self.testset, True)
+            assert samp in self.testset
 
     def test_len(self):
-        assert_equal(len(self.testset), 3)
+        assert len(self.testset) == 3
 
     def test_getitem_ensemble(self):
-        assert_equal(self.testset[self.ensB], self.s2B)
+        assert self.testset[self.ensB] == self.s2B
         # TODO: add test that we pick at random for ensA
 
     def test_getitem_replica(self):
-        assert_equal(self.testset[0], self.s0A)
-        assert_equal(self.testset[1], self.s1A)
-        assert_equal(self.testset[2], self.s2B)
+        assert self.testset[0] == self.s0A
+        assert self.testset[1] == self.s1A
+        assert self.testset[2] == self.s2B
         # TODO: add test that we pick at random
 
     def test_setitem_ensemble(self):
         ensC = LengthEnsemble(3)
         traj3C = Trajectory([-0.5, -0.25, 0.1])
         s3C = Sample(replica=3, trajectory=traj3C, ensemble=ensC)
         self.testset[ensC] = s3C
         self.testset.consistency_check()
-        assert_equal(len(self.testset), 4)
+        assert len(self.testset) == 4
 
     def test_setitem_replace_ensemble(self):
         self.testset[self.ensB] = self.s2B_
-        assert_equal(self.s2B in self.testset, False)
-        assert_equal(self.s2B_ in self.testset, True)
-        assert_equal(self.testset[2], self.s2B_)
-        assert_equal(self.testset[self.ensB], self.s2B_)
+        assert self.s2B not in self.testset
+        assert self.s2B_ in self.testset
+        assert self.testset[2] == self.s2B_
+        assert self.testset[self.ensB] == self.s2B_
         # TODO add test that we replace at random
 
     def test_setitem_replica(self):
         ensC = LengthEnsemble(3)
         traj3C = Trajectory([-0.5, -0.25, 0.1])
         s3C = Sample(replica=3, trajectory=traj3C, ensemble=ensC)
         self.testset[3] = s3C
         self.testset.consistency_check()
-        assert_equal(len(self.testset), 4)
+        assert len(self.testset) == 4
 
     def test_setitem_replace_replica(self):
         self.testset[2] = self.s2B_
-        assert_equal(self.s2B in self.testset, False)
-        assert_equal(self.s2B_ in self.testset, True)
-        assert_equal(self.testset[2], self.s2B_)
+        assert self.s2B not in self.testset
+        assert self.s2B_ in self.testset
+        assert self.testset[2] == self.s2B_
         # TODO add test that we replace at random
 
-    @raises(SampleKeyError)
     def test_illegal_assign_ensemble(self):
-        self.testset[self.ensA] = self.s2B_
+        with pytest.raises(SampleKeyError):
+            self.testset[self.ensA] = self.s2B_
 
-    @raises(SampleKeyError)
     def test_illegal_assign_replica(self):
-        self.testset[0] = self.s2B_
+        with pytest.raises(SampleKeyError):
+            self.testset[0] = self.s2B_
 
     def test_setitem_itemexists_ensemble(self):
         # exact sample is already there
         testset2 = SampleSet([self.s0A, self.s1A, self.s2B])
         # if we accidentally hit the statistical code, repeating 100 times
         # reduces odds of getting the same replacement each time
         for i in range(100):
             self.testset[self.ensA] = self.s0A
             self.testset.consistency_check()
-            assert_equal(len(self.testset), 3)
+            assert len(self.testset) == 3
             assert_items_equal(self.testset, testset2)
 
     def test_setitem_itemexists_replica(self):
         testset = SampleSet([self.s0A, self.s1A, self.s2B, self.s2B_])
         testset2 = SampleSet([self.s0A, self.s1A, self.s2B, self.s2B_])
         testset[2] = self.s2B
         testset.consistency_check()
-        assert_equal(len(testset), 4)
+        assert len(testset) == 4
         assert_items_equal(testset, testset2)
 
     def test_additem(self):
         testset2 = SampleSet([self.s0A, self.s1A, self.s2B, self.s2B_])
         self.testset.append(self.s2B_)
-        assert_equal(self.s2B_ in self.testset, True)
-        assert_equal(len(self.testset), 4)
+        assert self.s2B_ in self.testset
+        assert len(self.testset) == 4
         self.testset.consistency_check()
         assert_items_equal(self.testset, testset2)
 
     def test_additem_itemexists(self):
         # exact sample is already there
         testset2 = SampleSet([self.s0A, self.s1A, self.s2B])
         self.testset.append(self.s2B)
         self.testset.consistency_check()
-        assert_equal(len(self.testset), 3)
+        assert len(self.testset) == 3
         assert_items_equal(self.testset, testset2)
 
     def test_del_sample(self):
         del self.testset[self.s2B]
-        assert_equal(len(self.testset), 2)
-        assert_equal(self.ensB in list(self.testset.ensemble_dict.keys()), False)
-        assert_equal(self.ensA in list(self.testset.ensemble_dict.keys()), True)
-        assert_equal(2 in list(self.testset.replica_dict.keys()), False)
-        assert_equal(0 in list(self.testset.replica_dict.keys()), True)
+        assert len(self.testset) == 2
+        assert self.ensB not in list(self.testset.ensemble_dict.keys())
+        assert self.ensA in list(self.testset.ensemble_dict.keys())
+        assert 2 not in list(self.testset.replica_dict.keys())
+        assert 0 in list(self.testset.replica_dict.keys())
 
     def test_del_ensemble(self):
-        raise SkipTest
+        pytest.skip()
 
     def test_del_replica(self):
-        raise SkipTest
+        pytest.skip()
 
     def test_apply_samples(self):
-        raise SkipTest
+        pytest.skip()
 
     def test_extend(self):
         testset = SampleSet([self.s0A])
         testset.extend([self.s1A])
-        assert_equal(len(testset), 2)
-        assert_equal(self.s1A in testset, True)
+        assert len(testset) == 2
+        assert self.s1A in testset
         testset.consistency_check()
 
         testset.extend(SampleSet([self.s2B]))
-        assert_equal(len(testset), 3)
-        assert_equal(self.s2B in testset, True)
+        assert len(testset) == 3
+        assert self.s2B in testset
         testset.consistency_check()
 
         testset.extend(self.s2B_)
-        assert_equal(len(testset), 4)
-        assert_equal(self.s2B_ in testset, True)
+        assert len(testset) == 4
+        assert self.s2B_ in testset
         testset.consistency_check()
 
     def test_replica_list(self):
         assert_items_equal(self.testset.replica_list(), [0, 1, 2])
         self.testset.append(self.s2B_)
         assert_items_equal(self.testset.replica_list(), [0, 1, 2])
 
@@ -182,37 +180,37 @@
                            [self.s2B])
 
     def test_all_from_replica(self):
         assert_items_equal(self.testset.all_from_replica(2), [self.s2B])
         self.testset.append(self.s2B_)
         assert_items_equal(self.testset.all_from_replica(2), [self.s2B, self.s2B_])
 
-    @raises(AssertionError)
     def test_consistency_fail_size_ensdict(self):
         del self.testset.ensemble_dict[self.ensB]
-        self.testset.consistency_check()
+        with pytest.raises(AssertionError):
+            self.testset.consistency_check()
 
-    @raises(AssertionError)
     def test_consistency_fail_size_repdict(self):
         del self.testset.replica_dict[0]
-        self.testset.consistency_check()
+        with pytest.raises(AssertionError):
+            self.testset.consistency_check()
 
     def test_consistency_fail_sample_in_ensdict(self):
-        raise SkipTest
+        pytest.skip()
 
     def test_consistency_fail_sample_in_repdict(self):
-        raise SkipTest
+        pytest.skip()
 
     def test_consistency_fail_duplicate_samples(self):
-        raise SkipTest
+        pytest.skip()
 
     def test_sanity(self):
         self.testset.sanity_check()
 
-    @raises(AssertionError)
     def test_sanity_insane(self):
         traj0A = self.s0A.trajectory
         ensB = self.s2B.ensemble
         bad_samp = Sample(replica=0, trajectory=traj0A, ensemble=ensB)
         testset = SampleSet([bad_samp])
-        testset.sanity_check()
+        with pytest.raises(AssertionError):
+            testset.sanity_check()
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_shared.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_shooting.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_shooting.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_shooting_point_analysis.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_shooting_point_analysis.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_snapshot.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_snapshot.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """
 @author David W.H. Swenson
 """
 from __future__ import absolute_import
 import pytest
 
 from builtins import object
-from nose.tools import (assert_equal, assert_not_equal, assert_is, raises,
-                        assert_true)
-from nose.plugins.skip import Skip, SkipTest
 from numpy.testing import assert_allclose
 from .test_helpers import CallIdentity, raises_with_message_like, assert_close_unit
 
 import numpy as np
 import openpathsampling.engines.features as features
 
 from openpathsampling.engines.snapshot import SnapshotFactory
@@ -54,13 +51,13 @@
         import openpathsampling.engines.openmm as paths_omm
         # let box_vectors and topology to default to None
         snap = paths_omm.MDSnapshot(coordinates=np.array([[0.0, 0.0, 0.0],
                                                           [0.0, 0.0, 0.0]]),
                                     velocities=np.array([[0.0, 0.0, 0.0],
                                                          [0.0, 0.0, 0.0]]))
         new_snap = snap.copy()
-        assert_true(new_snap is not snap)
-        assert_true(new_snap.coordinates is not snap.coordinates)
+        assert new_snap is not snap
+        assert new_snap.coordinates is not snap.coordinates
         assert_allclose(new_snap.coordinates, snap.coordinates)
-        assert_true(new_snap.box_vectors is snap.box_vectors)
-        assert_true(new_snap.box_vectors is None)
-        assert_true(new_snap.engine is snap.engine)
+        assert new_snap.box_vectors is snap.box_vectors
+        assert new_snap.box_vectors is None
+        assert new_snap.engine is snap.engine
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_snapshot_modifier.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_snapshot_modifier.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_spring_shooting.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_spring_shooting.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,83 +34,73 @@
         self.ges = paths.SampleSet(paths.Sample(
             replica=0, trajectory=self.mytraj, ensemble=self.ens
         ))
 
 
 class TestSpringShootingSelector(SelectorTest):
 
-    @staticmethod
-    def test_neg_delta():
+    def test_neg_delta(self):
         with pytest.raises(ValueError):
             SpringShootingSelector(delta_max=-1,
                                    k_spring=0.1)
 
-    @staticmethod
-    def test_0_delta():
+    def test_0_delta(self):
         with pytest.raises(ValueError):
             SpringShootingSelector(delta_max=0,
                                    k_spring=0.1)
 
-    @staticmethod
-    def test_pos_delta():
+    def test_pos_delta(self):
         delta_max = 1
         sel = SpringShootingSelector(delta_max=delta_max,
                                      k_spring=0.1)
         assert sel.delta_max == delta_max
         assert len(sel._fw_prob_list) == 2*delta_max+1
         assert len(sel._bw_prob_list) == 2*delta_max+1
 
-    @staticmethod
-    def test_neg_k():
+    def test_neg_k(self):
         with pytest.raises(ValueError):
             SpringShootingSelector(delta_max=1,
                                    k_spring=-1)
 
-    @staticmethod
-    def test_0_k():
+    def test_0_k(self):
         sel = SpringShootingSelector(delta_max=1,
                                      k_spring=0)
         ref_list = [1.0, 1.0, 1.0]
         assert sel.k_spring == 0
         assert sel._fw_prob_list == ref_list
         assert sel._bw_prob_list == ref_list
 
-    @staticmethod
-    def test_pos_k():
+    def test_pos_k(self):
         sel = SpringShootingSelector(delta_max=1,
                                      k_spring=1)
         assert sel.k_spring == 1
 
-    @staticmethod
-    def test_sanity_breaking_fw():
+    def test_sanity_breaking_fw(self):
         sel = SpringShootingSelector(delta_max=1,
                                      k_spring=1)
         sel._fw_prob_list = [0, 0, 0]
         with pytest.raises(RuntimeError):
             sel.check_sanity()
 
-    @staticmethod
-    def test_sanity_breaking_bw():
+    def test_sanity_breaking_bw(self):
         sel = SpringShootingSelector(delta_max=1,
                                      k_spring=1)
         sel._bw_prob_list = [0, 0, 0]
 
         with pytest.raises(RuntimeError):
             sel.check_sanity()
 
-    @staticmethod
-    def test_sanity_breaking_total():
+    def test_sanity_breaking_total(self):
         sel = SpringShootingSelector(delta_max=1,
                                      k_spring=1)
         sel._total_bias = sum([0, 0, 0])
         with pytest.raises(RuntimeError):
             sel.check_sanity()
 
-    @staticmethod
-    def test_probability_ratio():
+    def test_probability_ratio(self):
         sel = SpringShootingSelector(delta_max=1,
                                      k_spring=1)
         sel._acceptable_snapshot = True
         # TODO OPS 2.0:  Last value here is not None to silence deprecation
         # warnings, should be set to None after the completion
         ratio = sel.probability_ratio(None, None, None, 1)
         assert ratio == 1.0
@@ -137,16 +127,15 @@
     def test_sanity_breaking_total_pick(self):
         sel = SpringShootingSelector(delta_max=1,
                                      k_spring=1)
         sel._total_bias = sum([0, 0, 0])
         with pytest.raises(RuntimeError):
             sel.pick(trajectory=self.mytraj, direction='forward')
 
-    @staticmethod
-    def test_initial_guess():
+    def test_initial_guess(self):
         sel = SpringShootingSelector(delta_max=1, k_spring=1, initial_guess=12)
         assert sel.trial_snapshot == 12
         assert sel.previous_snapshot == 12
 
     def test_pick_direction(self):
         sel = SpringShootingSelector(delta_max=1, k_spring=1)
         with pytest.raises(RuntimeError):
@@ -268,24 +257,22 @@
         sel = self.default_selector
         pick = sel.pick(trajectory=self.mytraj, direction='backward')
         assert pick == 0
         assert sel.trial_snapshot == -len(self.mytraj)
         assert sel.previous_snapshot == self.initial_guess
         assert sel._acceptable_snapshot is False
 
-    @staticmethod
-    def test_failed_loading():
+    def test_failed_loading(self):
         sel = SpringShootingSelector(delta_max=1, k_spring=0, initial_guess=3)
         details = Details(foo='bar')
         step = FakeStep(details)
         with pytest.raises(RuntimeError):
             sel.restart_from_step(step)
 
-    @staticmethod
-    def test_correct_loading():
+    def test_correct_loading(self):
         sel = SpringShootingSelector(delta_max=1, k_spring=0, initial_guess=3)
         details = Details(initial_trajectory='foo',
                           last_accepted_shooting_index='bar',
                           shooting_index=13,
                           direction='forward')
         step = FakeStep(details)
         sel.restart_from_step(step)
@@ -409,16 +396,15 @@
         assert len(mover.movers) == 2
         assert isinstance(mover.movers[0], SpringMover)
         assert isinstance(mover.movers[1], SpringMover)
         assert mover.movers[0].selector is mover.movers[1].selector
 
 
 class TestSpringShootingStrategy(MoveStrategyTestSetup):
-    @staticmethod
-    def test_init():
+    def test_init(self):
         strategy = SpringShootingStrategy(delta_max=1, k_spring=0.0,
                                           initial_guess=3)
         assert strategy.delta_max == 1
         assert strategy.k_spring == 0.0
         assert strategy.initial_guess == 3
 
     def test_make_movers(self):
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_sshooting_analysis.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_sshooting_analysis.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_sshooting_simulator.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_sshooting_simulator.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_storage.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,33 +6,30 @@
 from builtins import zip
 from builtins import range
 from builtins import object
 import os
 
 import pytest
 
-from nose.tools import (assert_equal)
-
 import openpathsampling as paths
 
 import openpathsampling.engines.openmm as peng
 import openpathsampling.engines.toy as toys
 
 from openpathsampling.netcdfplus import ObjectJSON
 from openpathsampling.storage import Storage
 from .test_helpers import (data_filename, md, compare_snapshot)
 
 import numpy as np
-from nose.plugins.skip import SkipTest
 
 
 class TestStorage(object):
     def setup_method(self):
         if not md:
-            raise SkipTest("mdtraj not installed")
+            pytest.skip("mdtraj not installed")
         self.mdtraj = md.load(data_filename("ala_small_traj.pdb"))
         _ = pytest.importorskip('simtk.unit')
         self.traj = peng.trajectory_from_mdtraj(
             self.mdtraj, simple_topology=True)
 
         self.filename = data_filename("storage_test.nc")
         self.filename_clone = data_filename("storage_test_clone.nc")
@@ -64,30 +61,28 @@
 
     def test_create_storage(self):
         store = Storage(filename=self.filename, mode='w')
         assert(os.path.isfile(data_filename("storage_test.nc")))
         store.close()
 
     def test_stored_topology(self):
-        raise SkipTest
+        pytest.skip()
         store = Storage(
             filename=self.filename,
             mode='w')
         assert(os.path.isfile(self.filename))
         store.close()
 
         store = Storage(filename=self.filename, mode='a')
         loaded_topology = store.template.topology
         # check if path topologies have the same JSON string
         # this also tests the simplifier for topologies
 
-        assert_equal(
-            self.simplifier.to_json(self.template_snapshot.topology),
-            self.simplifier.to_json(loaded_topology)
-        )
+        assert (self.simplifier.to_json(self.template_snapshot.topology)
+                == self.simplifier.to_json(loaded_topology))
 
         store.close()
 
     def test_safemode(self):
         fname = data_filename("cv_storage_safemode_test.nc")
         if os.path.isfile(fname):
             os.remove(fname)
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_tis_analysis.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_tis_analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import itertools
 import random
 import pytest
-from nose.tools import assert_equal, assert_almost_equal, raises
+from numpy.testing import assert_almost_equal
 from .test_helpers import (make_1d_traj, MoverWithSignature, RandomMDEngine,
                            assert_frame_equal, assert_items_equal)
 
 from openpathsampling.analysis.tis import *
 from openpathsampling.analysis.tis.core import steps_to_weighted_trajectories
 from openpathsampling.analysis.tis.flux import default_flux_sort
 import openpathsampling as paths
@@ -32,18 +32,18 @@
     falling = list(reversed(rising))[1:]
     return make_1d_traj(rising + falling)
 
 
 class TestMultiEnsembleSamplingAnalyzer(object):
     # this only has to check the error generation; everything else gets
     # covered by tests of subclasses
-    @raises(RuntimeError)
     def test_no_ensembles(self):
         histogrammer = MultiEnsembleSamplingAnalyzer()
-        histogrammer.calculate([])
+        with pytest.raises(RuntimeError):
+            histogrammer.calculate([])
 
 
 class TISAnalysisTester(object):
     # abstract class to give the same setup to all the test functions
 
     def _make_fake_steps(self, sample_sets, mover):
         steps = []
@@ -177,31 +177,27 @@
 
         # (ensemble_number, trajectory_number): count
         results = {(0, 0): 2, (0, 1): 1, (0, 2): 1, (0, 3): 0,
                    (1, 0): 0, (1, 1): 2, (1, 2): 1, (1, 3): 1,
                    (2, 0): 0, (2, 1): 0, (2, 2): 2, (2, 3): 2}
 
         for ((ens, traj), result) in results.items():
-            assert_equal(
-                weighted_trajs[ensembles_AB[ens]][self.trajs_AB[traj]],
-                result
-            )
-            assert_equal(
-                weighted_trajs[ensembles_BA[ens]][self.trajs_BA[traj]],
-                result
-            )
+            assert (weighted_trajs[ensembles_AB[ens]][self.trajs_AB[traj]]
+                    == result)
+            assert (weighted_trajs[ensembles_BA[ens]][self.trajs_BA[traj]]
+                    == result)
 
     def test_steps_to_weighted_trajectories(self):
-        assert_equal(len(self.mistis_weighted_trajectories),
-                     len(self.mistis.sampling_ensembles))
+        assert (len(self.mistis_weighted_trajectories)
+                == len(self.mistis.sampling_ensembles))
         self._check_network_results(self.mistis,
                                     self.mistis_weighted_trajectories)
 
-        assert_equal(len(self.mstis_weighted_trajectories),
-                     len(self.mstis.sampling_ensembles))
+        assert (len(self.mstis_weighted_trajectories)
+                == len(self.mstis.sampling_ensembles))
         self._check_network_results(self.mstis,
                                     self.mstis_weighted_trajectories)
 
 
 class TestFluxToPandas(TISAnalysisTester):
     # includes tests for default_flux_sort and flux_matrix_pd
     # as a class to simplify setup of flux objects
@@ -245,17 +241,17 @@
         pdt.assert_series_equal(series, self.expected_series)
 
     def test_flux_matrix_pd_None(self):
         series = flux_matrix_pd(self.fluxes, sort_method=None)
         for idx in self.indices:
             assert_almost_equal(series[idx], self.expected_series[idx])
 
-    @raises(KeyError)
     def test_flux_matrix_pd_unknown_str(self):
-        flux_matrix_pd(self.fluxes, sort_method="foo")
+        with pytest.raises(KeyError):
+            flux_matrix_pd(self.fluxes, sort_method="foo")
 
 
 class TestDictFlux(TISAnalysisTester):
     def setup_method(self):
         super(TestDictFlux, self).setup_method()
         self.innermost_interface_A = \
             self.sampling_ensembles_for_transition(self.mistis,
@@ -267,48 +263,41 @@
                                                    self.state_A)[0]
 
         self.flux_dict = {(self.state_A, self.innermost_interface_A): 1.0,
                           (self.state_B, self.innermost_interface_B): 1.0}
         self.flux_method = DictFlux(self.flux_dict)
 
     def test_calculate(self):
-        assert_equal(self.flux_method.calculate(self.mistis_steps),
-                     self.flux_dict)
+        assert self.flux_method.calculate(self.mistis_steps) == self.flux_dict
 
     def test_from_weighted_trajectories(self):
-        assert_equal(
-            self.flux_method.from_weighted_trajectories(self.mistis_steps),
-            self.flux_dict
-        )
+        fd = self.flux_method.from_weighted_trajectories(self.mistis_steps)
+        assert fd == self.flux_dict
 
     def test_intermediates(self):
-        assert_equal(self.flux_method.intermediates(self.mistis_steps), [])
+        assert self.flux_method.intermediates(self.mistis_steps) == []
 
     def test_calculate_from_intermediates(self):
         intermediates = self.flux_method.intermediates(self.mistis_steps)
-        assert_equal(
-            self.flux_method.calculate_from_intermediates(*intermediates),
-            self.flux_dict
-        )
+        fd = self.flux_method.calculate_from_intermediates(*intermediates)
+        assert fd == self.flux_dict
 
     def test_combine_results(self):
         my_result = self.flux_method.calculate(self.mistis_steps)
         same_result = {(self.state_A, self.innermost_interface_A): 1.0,
                        (self.state_B, self.innermost_interface_B): 1.0}
-        assert_equal(
-            self.flux_method.combine_results(my_result, same_result),
-            my_result
-        )
+        res = self.flux_method.combine_results(my_result, same_result)
+        assert res == my_result
 
-    @raises(RuntimeError)
     def test_bad_combine_results(self):
         my_result = self.flux_method.calculate(self.mistis_steps)
         bad_result = {(self.state_A, self.innermost_interface_A): 2.0,
                       (self.state_B, self.innermost_interface_B): 2.0}
-        self.flux_method.combine_results(my_result, bad_result)
+        with pytest.raises(RuntimeError):
+            self.flux_method.combine_results(my_result, bad_result)
 
 
 class TestMinusMoveFlux(TISAnalysisTester):
     def setup_method(self):
         super(TestMinusMoveFlux, self).setup_method()
 
         a = 0.1  # just a number to simplify the trajectory-making
@@ -341,24 +330,24 @@
             self.state_A: lambda x: x,
             self.state_B: lambda x: 1.0 - x
         }
 
         minus_ensemble_to_mover = {m.minus_ensemble: m
                                    for m in scheme.movers['minus']}
 
-        assert_equal(set(minus_ensemble_to_mover.keys()),
-                     set(network.minus_ensembles))
+        assert (set(minus_ensemble_to_mover.keys())
+                == set(network.minus_ensembles))
         steps = []
         mccycle = 0
         for minus_traj in descriptions:
             for i, minus_ensemble in enumerate(network.minus_ensembles):
                 replica = -1 - i
                 adjustment = state_adjustment[minus_ensemble.state_vol]
                 traj = make_1d_traj([adjustment(s) for s in minus_traj])
-                assert_equal(minus_ensemble(traj), True)
+                assert minus_ensemble(traj)
                 samp = paths.Sample(trajectory=traj,
                                     ensemble=minus_ensemble,
                                     replica=replica)
                 sample_set = paths.SampleSet([samp])
                 change = paths.AcceptedSampleMoveChange(
                     samples=[samp],
                     mover=minus_ensemble_to_mover[samp.ensemble],
@@ -369,22 +358,22 @@
                 # how it actually works. However, this is doesn't matter for
                 # the current implementation
                 steps.append(paths.MCStep(mccycle=mccycle,
                                           active=sample_set,
                                           change=change))
 
                 mccycle += 1
-        assert_equal(len(steps), 4)
+        assert len(steps) == 4
         return steps
 
     def test_get_minus_steps(self):
         all_mistis_steps = self.mistis_steps + self.mistis_minus_steps
         mistis_minus_steps = \
             self.mistis_minus_flux._get_minus_steps(all_mistis_steps)
-        assert_equal(len(mistis_minus_steps), len(self.mistis_minus_steps))
+        assert len(mistis_minus_steps) == len(self.mistis_minus_steps)
         assert_items_equal(mistis_minus_steps, self.mistis_minus_steps)
         # this could be repeated for MSTIS, but why?
 
     def test_calculate(self):
         avg_t_in = (5.0 + 3.0) / 2
         avg_t_out = (2.0 + 5.0 + 3.0 + 3.0) / 4
         expected_flux = 1.0 / (avg_t_in + avg_t_out)
@@ -395,15 +384,14 @@
             assert_almost_equal(flux, expected_flux)
 
         mstis_flux = \
             self.mstis_minus_flux.calculate(self.mstis_minus_steps)
         for flux in mstis_flux.values():  # all values are the same
             assert_almost_equal(flux, expected_flux)
 
-    @raises(ValueError)
     def test_bad_network(self):
         # raises error if more than one transition shares a minus ensemble
         # (flux cannot be calculated with multiple interface set minus move)
         state_C = paths.CVDefinedVolume(self.cv_x, 0.5, 0.7)
         trans_AB = self.mistis.transitions[(self.state_A, self.state_B)]
         trans_BA = self.mistis.transitions[(self.state_B, self.state_A)]
         interfaces_AB = trans_AB.interfaces
@@ -412,15 +400,16 @@
         bad_mistis = paths.MISTISNetwork([
             (self.state_A, interfaces_AB, self.state_B),
             (self.state_B, interfaces_BA, self.state_A),
             (self.state_A, interfaces_AC, state_C)
         ])
         scheme = paths.DefaultScheme(bad_mistis)
         scheme.build_move_decision_tree()
-        MinusMoveFlux(scheme)
+        with pytest.raises(ValueError):
+            MinusMoveFlux(scheme)
 
 
 class TestPathLengthHistogrammer(TISAnalysisTester):
     def _check_network_results(self, network, hists):
         results = {0: {(3.0,): 2, (5.0,): 1, (7.0,): 1},
                    1: {(5.0,): 2, (7.0,): 1, (12.0,): 1},
                    2: {(7.0,): 2, (12.0,): 2}}
@@ -429,23 +418,23 @@
                                                               self.state_A,
                                                               self.state_B)
         ensembles_BA = self.sampling_ensembles_for_transition(network,
                                                               self.state_B,
                                                               self.state_A)
         for (key, dct) in results.items():
             hist_dct_AB = hists[ensembles_AB[key]]._histogram
-            assert_equal(dict(hist_dct_AB), dct)
+            assert dict(hist_dct_AB) == dct
             hist_dct_BA = hists[ensembles_BA[key]]._histogram
-            assert_equal(dict(hist_dct_BA), dct)
+            assert dict(hist_dct_BA) == dct
 
     def test_calculate(self):
         default_histogrammer = \
                 PathLengthHistogrammer(self.mistis.sampling_ensembles)
-        assert_equal(default_histogrammer.hist_parameters,
-                     {'bin_width': 5, 'bin_range': (0, 1000)})
+        assert (default_histogrammer.hist_parameters
+                == {'bin_width': 5, 'bin_range': (0, 1000)})
 
         mistis_histogrammer = PathLengthHistogrammer(
             ensembles=self.mistis.sampling_ensembles,
             hist_parameters={'bin_width': 1, 'bin_range': (0, 10)}
         )
         mistis_hists = mistis_histogrammer.calculate(self.mistis_steps)
         self._check_network_results(self.mistis, mistis_hists)
@@ -499,27 +488,27 @@
         mstis_BA_histogrammer = FullHistogramMaxLambdas(
             transition=mstis_BA,
             hist_parameters={'bin_width': 0.1, 'bin_range': (-0.1, 1.1)}
         )
         mstis_BA_hists = mstis_BA_histogrammer.calculate(self.mstis_steps)
         self._check_transition_results(mstis_BA, mstis_BA_hists)
 
-    @raises(RuntimeError)
     def test_calculate_no_max_lambda(self):
         mistis_AB = self.mistis.transitions[(self.state_A, self.state_B)]
         modified_transition = paths.TISTransition(
             stateA=mistis_AB.stateA,
             stateB=mistis_AB.stateB,
             interfaces=mistis_AB.interfaces.volumes,
             orderparameter=mistis_AB.orderparameter
         )
-        FullHistogramMaxLambdas(
-            transition=modified_transition,
-            hist_parameters={'bin_width': 0.1, 'bin_range': (-0.1, 1.1)}
-        )
+        with pytest.raises(RuntimeError):
+            FullHistogramMaxLambdas(
+                transition=modified_transition,
+                hist_parameters={'bin_width': 0.1, 'bin_range': (-0.1, 1.1)}
+            )
 
 
 class TestConditionalTransitionProbability(TISAnalysisTester):
     def _check_network_results(self, network, ctp_results):
         results = {0: 0.0, 1: 0.25, 2: 0.5}
         ensembles_AB = self.sampling_ensembles_for_transition(network,
                                                               self.state_A,
@@ -528,25 +517,25 @@
                                                               self.state_B,
                                                               self.state_A)
 
         for ens_num in range(len(ensembles_AB)):
             dct_AB = ctp_results[ensembles_AB[ens_num]]
             result = results[ens_num]
             if result != 0.0:
-                assert_equal(dct_AB[self.state_B], result)
+                assert dct_AB[self.state_B] == result
             if result != 1.0:
-                assert_equal(dct_AB[self.state_A], 1.0-result)
+                assert dct_AB[self.state_A] == 1.0 - result
 
         for ens_num in range(len(ensembles_BA)):
             dct_BA = ctp_results[ensembles_BA[ens_num]]
             result = results[ens_num]
             if result != 0.0:
-                assert_equal(dct_BA[self.state_A], result)
+                assert dct_BA[self.state_A] == result
             if result != 1.0:
-                assert_equal(dct_BA[self.state_B], 1.0-result)
+                assert dct_BA[self.state_B] == 1.0 - result
 
     def test_calculate(self):
         mistis_ctp_calc = ConditionalTransitionProbability(
             ensembles=self.mistis.sampling_ensembles,
             states=[self.state_A, self.state_B]
         )
         mistis_ctp = mistis_ctp_calc.calculate(self.mistis_steps)
@@ -686,54 +675,46 @@
         self.mstis_transition_dict = TransitionDictResults(
             results_dict=results_dict,
             network=self.mstis,
             allow_sampling=True
         )
 
     def test_iter(self):
-        assert_equal(set(pair for pair in self.mistis_transition_dict),
-                     set(pair for pair in self.mstis_transition_dict))
+        assert (set(pair for pair in self.mistis_transition_dict)
+                == set(pair for pair in self.mstis_transition_dict))
 
     def test_get_by_pair(self):
-        assert_equal(
-            self.mstis_transition_dict[(self.state_A, self.state_B)], 1
-        )
-        assert_equal(
-            self.mstis_transition_dict[(self.state_A, self.state_B)],
-            self.mistis_transition_dict[(self.state_A, self.state_B)]
-        )
-        assert_equal(
-            self.mstis_transition_dict[(self.state_B, self.state_A)], 2
-        )
-        assert_equal(
-            self.mstis_transition_dict[(self.state_B, self.state_A)],
-            self.mistis_transition_dict[(self.state_B, self.state_A)]
-        )
+        assert self.mstis_transition_dict[(self.state_A, self.state_B)] == 1
+        assert (self.mstis_transition_dict[(self.state_A, self.state_B)]
+                == self.mistis_transition_dict[(self.state_A, self.state_B)])
+        assert self.mstis_transition_dict[(self.state_B, self.state_A)] == 2
+        assert (self.mstis_transition_dict[(self.state_B, self.state_A)]
+                == self.mistis_transition_dict[(self.state_B, self.state_A)])
 
-    @raises(KeyError)
     def test_get_bad_pair(self):
-        self.mistis_transition_dict[(self.state_A, self.state_A)]
+        with pytest.raises(KeyError):
+            self.mistis_transition_dict[(self.state_A, self.state_A)]
 
     def test_get_by_transition(self):
         mistis_AB = self.mistis.transitions[(self.state_A, self.state_B)]
         mstis_AB = self.mstis.transitions[(self.state_A, self.state_B)]
-        assert_equal(self.mistis_transition_dict[mistis_AB], 1)
-        assert_equal(self.mistis_transition_dict[mistis_AB],
-                     self.mstis_transition_dict[mstis_AB])
+        assert self.mistis_transition_dict[mistis_AB] == 1
+        assert (self.mistis_transition_dict[mistis_AB]
+                == self.mstis_transition_dict[mstis_AB])
 
     def test_get_by_sampling_transition(self):
         from_A = self.mstis.from_state[self.state_A]
         from_B = self.mstis.from_state[self.state_B]
-        assert_equal(self.mstis_transition_dict[from_A], 1)
-        assert_equal(self.mstis_transition_dict[from_B], 2)
+        assert self.mstis_transition_dict[from_A] == 1
+        assert self.mstis_transition_dict[from_B] == 2
 
-    @raises(KeyError)
     def test_bad_get_sampling_transition(self):
         sampling_trans = self.mistis.sampling_transitions[0]
-        self.mistis_transition_dict[sampling_trans]
+        with pytest.raises(KeyError):
+            self.mistis_transition_dict[sampling_trans]
 
     def test_to_pandas(self):
         result = [[float("nan"), 1], [2, float("nan")]]
         order = [self.state_A, self.state_B]
         ordered_names = ["A", "B"]
         pd_result = pd.DataFrame(data=result, index=ordered_names,
                                  columns=ordered_names)
@@ -781,39 +762,37 @@
         self.mistis_analysis.calculate(self.mistis_steps)
         self.mstis_analysis = self._make_tis_analysis(self.mstis)
         self.mstis_analysis.calculate(self.mstis_steps)
 
     def test_bad_access_cached_results(self):
         no_results = self._make_tis_analysis(self.mistis)
         _ = self.mistis_analysis._access_cached_result('rate')
-        # use a try/except here instead of @raises so that we also test that
-        # the calculated version (previous line) works as expected
-        try:
+        with pytest.raises(AttributeError):
             no_results._access_cached_result('rate')
-        except AttributeError:
-            pass  # this is the expected test result
 
     def test_flux_matrix(self):
-        assert_equal(self.mistis_analysis.flux_matrix,
-                     {(t.stateA, t.interfaces[0]): 0.1
-                      for t in self.mistis.sampling_transitions})
-        assert_equal(self.mstis_analysis.flux_matrix,
-                     {(t.stateA, t.interfaces[0]): 0.1
-                      for t in self.mstis.sampling_transitions})
+        assert self.mistis_analysis.flux_matrix== {
+            (t.stateA, t.interfaces[0]): 0.1
+            for t in self.mistis.sampling_transitions
+        }
+        assert self.mstis_analysis.flux_matrix == {
+            (t.stateA, t.interfaces[0]): 0.1
+            for t in self.mstis.sampling_transitions
+        }
 
     def test_flux(self):
         for transition in self.mistis.sampling_transitions:
             state = transition.stateA
             innermost = transition.interfaces[0]
-            assert_equal(self.mistis_analysis.flux(state, innermost), 0.1)
+            assert self.mistis_analysis.flux(state, innermost) == 0.1
 
         for transition in self.mstis.sampling_transitions:
             state = transition.stateA
             innermost = transition.interfaces[0]
-            assert_equal(self.mstis_analysis.flux(state, innermost), 0.1)
+            assert self.mstis_analysis.flux(state, innermost) == 0.1
 
     def test_flux_through_state(self):
         flux_dict = {(t.stateA, t.interfaces[0]): 0.1
                      for t in self.mistis.sampling_transitions}
         flux_dict.update({(self.state_A, self.state_A): 0.5})
         tis = TISAnalysis(
             network=self.mistis,
@@ -834,29 +813,29 @@
                     )
                 )
                 for transition in self.mistis.transitions.values()
             }
         )
         tis.calculate(self.mistis_steps)
         trans_AB = self.mistis.transitions[(self.state_A, self.state_B)]
-        assert_equal(tis.flux(self.state_A, trans_AB.interfaces[0]), 0.1)
-        assert_equal(tis.flux(self.state_A), 0.5)
+        assert tis.flux(self.state_A, trans_AB.interfaces[0]) == 0.1
+        assert tis.flux(self.state_A) == 0.5
 
     def test_state_fluxes(self):
         for transition in self.mistis.sampling_transitions:
             state = transition.stateA
             innermost = transition.interfaces[0]
-            assert_equal(self.mistis_analysis.state_fluxes(state),
-                         {(state, innermost): 0.1})
+            assert (self.mistis_analysis.state_fluxes(state)
+                    == {(state, innermost): 0.1})
 
         for transition in self.mstis.sampling_transitions:
             state = transition.stateA
             innermost = transition.interfaces[0]
-            assert_equal(self.mstis_analysis.state_fluxes(state),
-                         {(state, innermost): 0.1})
+            assert (self.mstis_analysis.state_fluxes(state)
+                    == {(state, innermost): 0.1})
 
     def test_transition_probability_matrix(self):
         pairs = [(self.state_A, self.state_B), (self.state_B, self.state_A)]
         mistis_tp = self.mistis_analysis.transition_probability_matrix
         mstis_tp = self.mstis_analysis.transition_probability_matrix
         for trans_pair in pairs:
             assert_almost_equal(mistis_tp[trans_pair], 0.125)
@@ -947,31 +926,31 @@
         mistis_interfaces = ['A->B 2', 'B->A 2']
         mstis_interfaces = ['Out A 2', 'Out B 2']
 
         expected_mistis = pd.DataFrame(data=expected_data,
                                        index=mistis_interfaces,
                                        columns=states)
         mistis_ctp = self.mistis_analysis.conditional_transition_probability
-        assert_equal(set(states), set(mistis_ctp.columns))
-        assert_equal(set(mistis_interfaces), set(mistis_ctp.index))
+        assert set(states) == set(mistis_ctp.columns)
+        assert set(mistis_interfaces) == set(mistis_ctp.index)
         for iface in mistis_interfaces:
             for state in states:
-                assert_equal(expected_mistis.loc[(iface, state)],
-                             mistis_ctp.loc[(iface, state)])
+                assert (expected_mistis.loc[(iface, state)]
+                        == mistis_ctp.loc[(iface, state)])
 
         expected_mstis = pd.DataFrame(data=expected_data,
                                       index=mstis_interfaces,
                                       columns=states)
         mstis_ctp = self.mstis_analysis.conditional_transition_probability
-        assert_equal(set(states), set(mstis_ctp.columns))
-        assert_equal(set(mstis_interfaces), set(mstis_ctp.index))
+        assert set(states) == set(mstis_ctp.columns)
+        assert set(mstis_interfaces) == set(mstis_ctp.index)
         for iface in mstis_interfaces:
             for state in states:
-                assert_equal(expected_mstis.loc[(iface, state)],
-                             mstis_ctp.loc[(iface, state)])
+                assert (expected_mstis.loc[(iface, state)]
+                        == mstis_ctp.loc[(iface, state)])
 
     def test_total_crossing_probability(self):
         results = {0.0: 1.0, 0.1: 0.5, 0.2: 0.25, 0.3: 0.125,
                    0.5: 0.125, 1.0: 0.125}
 
         mistis_tcp = self.mistis_analysis.total_crossing_probability
         for transition in self.mistis.transitions.values():
@@ -981,32 +960,32 @@
 
         mstis_tcp = self.mstis_analysis.total_crossing_probability
         for transition in self.mstis.transitions.values():
             tcp = mstis_tcp[transition]
             for x in results:
                 assert_almost_equal(results[x], tcp(x))
 
-    @raises(TypeError)
     def test_bad_no_flux(self):
         network = self.mistis
-        StandardTISAnalysis(
-            network=network,
-            max_lambda_calcs={t: {'bin_width': 0.1,
-                                  'bin_range': (-0.1, 1.1)}
-                              for t in network.sampling_transitions}
-        )
+        with pytest.raises(TypeError):
+            StandardTISAnalysis(
+                network=network,
+                max_lambda_calcs={t: {'bin_width': 0.1,
+                                      'bin_range': (-0.1, 1.1)}
+                                  for t in network.sampling_transitions}
+            )
 
-    @raises(RuntimeError)
     def test_bad_max_lambda_calcs(self):
         network = self.mistis
-        StandardTISAnalysis(
-            network=network,
-            flux_method=DictFlux({(t.stateA, t.interfaces[0]): 0.1
-                                  for t in network.sampling_transitions})
-        )
+        with pytest.raises(RuntimeError):
+            StandardTISAnalysis(
+                network=network,
+                flux_method=DictFlux({(t.stateA, t.interfaces[0]): 0.1
+                                      for t in network.sampling_transitions})
+            )
 
     def test_init_ensemble_histogrammer_max_lambda(self):
         network = self.mistis
         max_lambda_calcs = {
             t: FullHistogramMaxLambdas(
                 transition=t,
                 hist_parameters={'bin_width': 0.1, 'bin_range': (-0.1, 1.1)}
@@ -1048,15 +1027,15 @@
             # note that these trajs are equivalent to minus move
             # descriptions in TestMinusMoveFlux
             seq_1 = [a_in] + [a_out]*2 + [a_in]*5 + [a_out]*5 + [a_in]
             seq_2 = [a_in] + [a_out]*3 + [a_in]*3 + [a_out]*3 + [a_in]
 
             for seq in [seq_1, seq_2]:
                 traj = make_1d_traj(seq)
-                assert_equal(minus_ens(traj), True)
+                assert minus_ens(traj)
                 samp = paths.Sample(trajectory=traj,
                                     ensemble=minus_ens,
                                     replica=replica[state])
                 _ = paths.SampleSet([samp])
                 change = paths.AcceptedSampleMoveChange(
                     samples=[samp],
                     mover=minus_mover,
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_tools.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_tools.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import pytest
-from nose.tools import assert_equal
 from openpathsampling.tools import *
 
 import tempfile
 import hashlib
 import os
 from .test_helpers import data_filename
 
@@ -11,50 +10,43 @@
 logging.getLogger('openpathsampling.initialization').setLevel(logging.CRITICAL)
 logging.getLogger('openpathsampling.ensemble').setLevel(logging.CRITICAL)
 logging.getLogger('openpathsampling.storage').setLevel(logging.CRITICAL)
 logging.getLogger('openpathsampling.netcdfplus').setLevel(logging.CRITICAL)
 
 def test_pretty_print_seconds():
     # test the basics with full reporting
-    assert_equal(pretty_print_seconds(93784),
-                 "1 day 2 hours 3 minutes 4 seconds")
-    assert_equal(pretty_print_seconds(179990),
-                 "2 days 1 hour 59 minutes 50 seconds")
-    assert_equal(pretty_print_seconds(31),
-                 "31 seconds")
+    assert pretty_print_seconds(93784) == "1 day 2 hours 3 minutes 4 seconds"
+    assert (pretty_print_seconds(179990)
+            == "2 days 1 hour 59 minutes 50 seconds")
+    assert pretty_print_seconds(31) == "31 seconds"
 
     # test positive n_labels (including testing rounding)
-    assert_equal(pretty_print_seconds(93784, n_labels=2),
-                 "1 day 2 hours")
-    assert_equal(pretty_print_seconds(179990, n_labels=2),
-                 "2 days 2 hours")
-    assert_equal(pretty_print_seconds(179990, n_labels=3),
-                 "2 days 2 hours 0 minutes")
-    assert_equal(pretty_print_seconds(31, n_labels=2),
-                 "31 seconds")
+    assert pretty_print_seconds(93784, n_labels=2) == "1 day 2 hours"
+    assert pretty_print_seconds(179990, n_labels=2) == "2 days 2 hours"
+    assert (pretty_print_seconds(179990, n_labels=3)
+            == "2 days 2 hours 0 minutes")
+    assert pretty_print_seconds(31, n_labels=2) == "31 seconds"
 
     # test negative n_labels
-    assert_equal(pretty_print_seconds(93784, n_labels=-1),
-                 "1.09 days")
-    assert_equal(pretty_print_seconds(93784, n_labels=-2),
-                 "1 day 2.05 hours")
-    assert_equal(pretty_print_seconds(31, n_labels=-2),
-                 "31 seconds")
+    assert pretty_print_seconds(93784, n_labels=-1) == "1.09 days"
+    assert pretty_print_seconds(93784, n_labels=-2) == "1 day 2.05 hours"
+    assert pretty_print_seconds(31, n_labels=-2) == "31 seconds"
 
     # test separators
-    assert_equal(pretty_print_seconds(93784, separator=", "),
-                 "1 day, 2 hours, 3 minutes, 4 seconds")
+    assert (pretty_print_seconds(93784, separator=", ")
+            == "1 day, 2 hours, 3 minutes, 4 seconds")
 
 def test_progress_string():
-    assert_equal(progress_string(0, 100, 10),
-                 "Starting simulation...\nWorking on first step\n")
-    assert_equal(progress_string(1, 11, 9378.4),
-                 "Running for 2 hours 36 minutes 18 seconds - "
-                 + "9378.40 seconds per step\n"
-                 + "Estimated time remaining: 1 day 2.05 hours\n")
+    assert (progress_string(0, 100, 10)
+            == "Starting simulation...\nWorking on first step\n")
+    assert progress_string(1, 11, 9378.4) == (
+        "Running for 2 hours 36 minutes 18 seconds - "
+        + "9378.40 seconds per step\n"
+        + "Estimated time remaining: 1 day 2.05 hours\n"
+    )
 
 
 def test_ensure_file_dne():
     # when the file doesn't exist and you provide contents, ensure_file
     # should create the missing file
     try:
         tmp_dir = tempfile.TemporaryDirectory()
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_toy_dynamics.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_toy_dynamics.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 from __future__ import absolute_import
 
 from builtins import zip
 from past.utils import old_div
 from builtins import object
 import os
 
-from nose.tools import (assert_equal, assert_not_equal, assert_almost_equal)
-
-from nose.plugins.skip import SkipTest
+import pytest
+from numpy.testing import assert_almost_equal
 
 import openpathsampling as paths
 import openpathsampling.engines.toy as toy
 from .test_helpers import (true_func, assert_equal_array_array,
                            assert_items_equal)
 
 import numpy as np
@@ -104,15 +103,15 @@
         self.velocities = init_vel
         self.mass = sys_mass
 
     def test_V(self):
         assert_almost_equal(linear.V(self), 2.0375)
 
     def test_dVdx(self):
-        assert_equal(linear.dVdx(self), [1.5, 0.75])
+        assert linear.dVdx(self) == [1.5, 0.75]
 
 
 class TestDoubleWell(object):
     def setup_method(self):
         self.positions = init_pos
         self.velocities = init_vel
         self.mass = sys_mass
@@ -157,15 +156,15 @@
         assert_almost_equal(self.simpletest.kinetic_energy(self), 0.4575)
 
 
 # === TESTS FOR TOY ENGINE OBJECT =========================================
 
 class Test_convert_fcn(object):
     def test_convert_to_3Ndim(self):
-        raise SkipTest
+        pytest.skip()
 
         assert_equal_array_array(toy.convert_to_3Ndim([1.0, 2.0]),
                                  np.array([[1.0, 2.0, 0.0]]))
         assert_equal_array_array(toy.convert_to_3Ndim([1.0, 2.0, 3.0]),
                                  np.array([[1.0, 2.0, 3.0]]))
         assert_equal_array_array(toy.convert_to_3Ndim([1.0, 2.0, 3.0, 4.0]),
                                  np.array([[1.0, 2.0, 3.0], [4.0, 0.0, 0.0]]))
@@ -199,18 +198,18 @@
     def teardown_method(self):
         if os.path.isfile('toy_tmp.nc'):
             os.remove('toy_tmp.nc')
 
     def test_sanity(self):
         assert_items_equal(self.sim._mass, sys_mass)
         assert_items_equal(self.sim._minv, [old_div(1.0,m_i) for m_i in sys_mass])
-        assert_equal(self.sim.n_steps_per_frame, 10)
+        assert self.sim.n_steps_per_frame == 10
 
     def test_snapshot_timestep(self):
-        assert_equal(self.sim.snapshot_timestep, 0.02)
+        assert self.sim.snapshot_timestep == 0.02
 
     def test_snapshot_get(self):
         snapshot = self.sim.current_snapshot
         assert_items_equal(snapshot.velocities[0],
                            self.sim.velocities)
         assert_items_equal(snapshot.coordinates[0],
                            self.sim.positions)
@@ -235,32 +234,32 @@
 
     def test_generate(self):
         self.sim.initialized = True
         try:
             traj = self.sim.generate(self.sim.current_snapshot, [true_func])
         except paths.engines.EngineMaxLengthError as e:
             traj = e.last_trajectory
-            assert_equal(len(traj), self.sim.n_frames_max)
+            assert len(traj) == self.sim.n_frames_max
         else:
             raise RuntimeError('Did not raise MaxLength Error')
 
     def test_generate_n_frames(self):
         self.sim.initialized = True
         ens = paths.LengthEnsemble(4)  # first snap plus n_frames
         orig = self.sim.current_snapshot.copy()
         traj1 = self.sim.generate(self.sim.current_snapshot, [ens.can_append])
         self.sim.current_snapshot = orig
         traj2 = [orig] + self.sim.generate_n_frames(3)
-        assert_equal(len(traj1), len(traj2))
+        assert len(traj1) == len(traj2)
         for (s1, s2) in zip(traj1, traj2):
             # snapshots are not the same object
-            assert_not_equal(s1, s2)
+            assert s1 != s2
             # however, they have the same values stored in them
-            assert_equal(len(s1.coordinates), 1)
-            assert_equal(len(s1.coordinates[0]), 2)
+            assert len(s1.coordinates) == 1
+            assert len(s1.coordinates[0]) == 2
             assert_items_equal(s1.coordinates[0], s2.coordinates[0])
             assert_items_equal(s1.velocities[0], s2.velocities[0])
 
     def test_start_with_snapshot(self):
         snap = toy.Snapshot(coordinates=np.array([1, 2]),
                             velocities=np.array([3, 4]))
         self.sim.start(snapshot=snap)
@@ -301,16 +300,16 @@
         self.sim = sim
 
     def test_momentum_update(self):
         self.sim.integ._momentum_update(self.sim, 0.002)
         # velocities = init_vel - pes.dVdx(init_pos)/m*dt
         #            = [0.6, 0.5] - [1.5, 0.75]/[1.5, 1.5] * 0.002
         #            = [0.598, 0.499]
-        assert_equal(self.sim.velocities[0], 0.598)
-        assert_equal(self.sim.velocities[1], 0.499)
+        assert self.sim.velocities[0] == 0.598
+        assert self.sim.velocities[1] == 0.499
 
     def test_position_update(self):
         self.sim.integ._position_update(self.sim, 0.002)
         # positions = init_pos + velocities * dt
         #           = [0.7, 0.65] + [0.6, 0.5]*0.002 = [0.7012, 0.651]
         assert_almost_equal(self.sim.positions[0], 0.7012)
         assert_almost_equal(self.sim.positions[1], 0.651)
@@ -353,22 +352,22 @@
 
         sim.n_steps_per_frame = 10
         self.sim = sim
 
     def test_OU_update(self):
         # we can't actually test for correct values, but we *can* test that
         # some things *don't* happen
-        assert_equal(self.sim.velocities[0], init_vel[0])
-        assert_equal(self.sim.velocities[1], init_vel[1])
+        assert self.sim.velocities[0] == init_vel[0]
+        assert self.sim.velocities[1] == init_vel[1]
         self.sim.integ._OU_update(self.sim, 0.002)
-        assert_not_equal(self.sim.velocities[0], init_vel[0])
-        assert_not_equal(self.sim.velocities[1], init_vel[1])
+        assert self.sim.velocities[0] != init_vel[0]
+        assert self.sim.velocities[1] != init_vel[1]
         # tests that the same random number wasn't used for both:
-        assert_not_equal(self.sim.velocities[0] - init_vel[0],
-                         self.sim.velocities[1] - init_vel[1])
+        assert (self.sim.velocities[0] - init_vel[0]
+                != self.sim.velocities[1] - init_vel[1])
 
     def test_step(self):
         self.sim.generate_next_frame()
 
 
 class TestOverdampedLangevinIntegrator(object):
     '''This is only a test if the integrator runs. Because of its stochastic
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_toy_features.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_toy_features.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from builtins import object
 import openpathsampling.engines.toy as toys
 import numpy as np
 
-from nose.tools import assert_equal, assert_almost_equal
-from nose.plugins.skip import SkipTest
+from numpy.testing import assert_almost_equal
 import logging
 
 logging.getLogger('openpathsampling.initialization').setLevel(logging.CRITICAL)
 logging.getLogger('openpathsampling.ensemble').setLevel(logging.CRITICAL)
 logging.getLogger('openpathsampling.storage').setLevel(logging.CRITICAL)
 logging.getLogger('openpathsampling.netcdfplus').setLevel(logging.CRITICAL)
 
@@ -33,16 +32,16 @@
         self.snap_6D = toys.Snapshot(coordinates=np.array([[0.0, 0.0, 0.0],
                                                            [0.0, 0.0, 0.0]]),
                                      velocities=np.array([[1.0, 0.0, 0.0],
                                                           [1.0, 0.0, 0.0]]),
                                      engine=engine_6D)
 
     def test_n_degrees_of_freedom(self):
-        assert_equal(self.snap_2D.n_degrees_of_freedom, 2)
-        assert_equal(self.snap_6D.n_degrees_of_freedom, 6)
+        assert self.snap_2D.n_degrees_of_freedom == 2
+        assert self.snap_6D.n_degrees_of_freedom == 6
 
     def test_instantaneous_temperature(self):
         # KE = 0.5 * (1.0*2.0**2 + 1.0*4.0**2) = 10.0
         # T = 2 * KE / 2 = KE = 10.0
         assert_almost_equal(self.snap_2D.instantaneous_temperature, 10.0)
         # KE = 0.5 * (1.0*1.0**2 + 2.0*1.0**2) = 1.5
         # T = 2 * KE / 6 = 0.5
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_trajectory.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_trajectory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from __future__ import absolute_import
 from builtins import object
 import logging
 
-from nose.tools import (
-    assert_equal, assert_not_equal, raises
-)
-from nose.plugins.skip import SkipTest
 from .test_helpers import (CallIdentity, prepend_exception_message,
                            make_1d_traj, assert_items_equal)
 
-
 import openpathsampling as paths
 from .test_helpers import make_1d_traj
 
 logging.getLogger('opentis.trajectory').setLevel(logging.DEBUG)
 logging.getLogger('opentis.initialization').setLevel(logging.CRITICAL)
 logging.getLogger('openpathsampling.storage').setLevel(logging.CRITICAL)
 
@@ -115,26 +110,26 @@
             paths.AllInXEnsemble(stateA) & paths.LengthEnsemble(1)
         ])
         subtrajectoriesA = ensemble_A.split(trajectory, overlap=0)
         subtrajectoriesB = ensemble_B.split(trajectory, overlap=0)
         subtrajectoriesABA = ensemble_ABA.split(trajectory)
 
         # make sure we have the trajectories we expect
-        assert_equal(len(subtrajectoriesA), 3)
-        assert_equal(len(subtrajectoriesB), 2)
-        assert_equal(len(subtrajectoriesABA), 1)
+        assert len(subtrajectoriesA) == 3
+        assert len(subtrajectoriesB) == 2
+        assert len(subtrajectoriesABA) == 1
         # the following assertions check that the subtrajectories are the
         # ones that we expect; the numbers here are linked to the indices
         # we'll test next
-        assert_equal(subtrajectoriesA[0], trajectory[0:2])
-        assert_equal(subtrajectoriesA[1], trajectory[3:4])
-        assert_equal(subtrajectoriesA[2], trajectory[11:13])
-        assert_equal(subtrajectoriesB[0], trajectory[5:7])
-        assert_equal(subtrajectoriesB[1], trajectory[8:9])
-        assert_equal(subtrajectoriesABA[0], trajectory[3:12])
+        assert subtrajectoriesA[0] == trajectory[0:2]
+        assert subtrajectoriesA[1] == trajectory[3:4]
+        assert subtrajectoriesA[2] == trajectory[11:13]
+        assert subtrajectoriesB[0] == trajectory[5:7]
+        assert subtrajectoriesB[1] == trajectory[8:9]
+        assert subtrajectoriesABA[0] == trajectory[3:12]
         # now we run the subtrajectory_indices function and test it
         indicesA = trajectory.subtrajectory_indices(subtrajectoriesA)
         indicesB = trajectory.subtrajectory_indices(subtrajectoriesB)
         indicesABA = trajectory.subtrajectory_indices(subtrajectoriesABA)
-        assert_equal(indicesA, [[0, 1], [3], [11, 12]])
-        assert_equal(indicesB, [[5, 6], [8]])
-        assert_equal(indicesABA, [[3, 4, 5, 6, 7, 8, 9, 10, 11]])
+        assert indicesA == [[0, 1], [3], [11, 12]]
+        assert indicesB == [[5, 6], [8]]
+        assert indicesABA == [[3, 4, 5, 6, 7, 8, 9, 10, 11]]
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_trajectory_transition_analysis.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_trajectory_transition_analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import division
 from __future__ import absolute_import
 from builtins import zip
 from past.utils import old_div
 from builtins import object
-from nose.tools import (assert_equal, assert_not_equal, raises,
-                        assert_almost_equal)
-from nose.plugins.skip import SkipTest
+
+import pytest
+from numpy.testing import assert_almost_equal
 from .test_helpers import make_1d_traj
 
 import openpathsampling as paths
 
 import random
 import numpy as np
 
@@ -32,78 +32,78 @@
 
         all_in_1 = paths.AllInXEnsemble(self.vol1)
         self.segments = all_in_1.split(self.trajectory)
         self.container = paths.TrajectorySegmentContainer(self.segments,
                                                           dt=0.5)
 
     def test_list_behavior(self):
-        assert_equal(len(self.container), 3)
-        assert_equal(self.container[0], self.segments[0])
+        assert len(self.container) == 3
+        assert self.container[0] == self.segments[0]
         for (truth, beauty) in zip(self.container, self.segments):
-            assert_equal(truth, beauty)
-        assert_equal(self.segments[0] in self.container, True)
+            assert truth == beauty
+        assert self.segments[0] in self.container
 
-    @raises(TypeError)
     def test_segments_setitem_fails(self):
-        self.container[0] = self.trajectory
+        with pytest.raises(TypeError):
+            self.container[0] = self.trajectory
 
     def test_segments(self):
-        assert_equal(self.container[0], self.trajectory[0:2])
-        assert_equal(self.container[1], self.trajectory[6:8])
-        assert_equal(self.container[2], self.trajectory[9:12])
+        assert self.container[0] == self.trajectory[0:2]
+        assert self.container[1] == self.trajectory[6:8]
+        assert self.container[2] == self.trajectory[9:12]
 
     def test_from_trajectory_and_indices(self):
         container = \
             paths.TrajectorySegmentContainer.from_trajectory_and_indices(
                 trajectory=self.trajectory,
                 indices=[(0, 2), (6, 8), (9, 12)],
                 dt=0.5
             )
-        assert_equal(container[0], self.trajectory[0:2])
-        assert_equal(container[1], self.trajectory[6:8])
-        assert_equal(container[2], self.trajectory[9:12])
+        assert container[0] == self.trajectory[0:2]
+        assert container[1] == self.trajectory[6:8]
+        assert container[2] == self.trajectory[9:12]
 
     def test_n_frames(self):
-        assert_equal(self.container.n_frames.tolist(), [2, 2, 3])
+        assert self.container.n_frames.tolist() == [2, 2, 3]
 
     def test_times(self):
-        assert_equal(self.container.times.tolist(), [1.0, 1.0, 1.5])
+        assert self.container.times.tolist() == [1.0, 1.0, 1.5]
 
-    @raises(RuntimeError)
     def test_times_without_dt(self):
         bad_container = paths.TrajectorySegmentContainer(self.segments)
-        bad_container.times
+        with pytest.raises(RuntimeError):
+            bad_container.times
 
     def test_add(self):
         ens_B = paths.AllInXEnsemble(self.vol3)
         segs_B = ens_B.split(self.trajectory)
         container_B = paths.TrajectorySegmentContainer(segs_B, dt=0.5)
-        assert_equal(len(container_B), 2)
+        assert len(container_B) == 2
         test_container = self.container + container_B
-        assert_equal(len(test_container), 5)
+        assert len(test_container) == 5
         for seg in self.container:
-            assert_equal(seg in test_container, True)
+            assert seg in test_container
         for seg in container_B:
-            assert_equal(seg in test_container, True)
+            assert seg in test_container
 
-    @raises(RuntimeError)
     def test_add_different_dt(self):
         ens_B = paths.AllInXEnsemble(self.vol3)
         segs_B = ens_B.split(self.trajectory)
         container_B = paths.TrajectorySegmentContainer(segs_B)
-        test_container = self.container + container_B
+        with pytest.raises(RuntimeError):
+            test_container = self.container + container_B
 
     def test_iadd(self):
         ens_B = paths.AllInXEnsemble(self.vol3)
         segs_B = ens_B.split(self.trajectory)
         container_B = paths.TrajectorySegmentContainer(segs_B)
         container_B_id = id(container_B)
         container_B += self.container
-        assert_equal(len(container_B), 5)
-        assert_equal(container_B_id, id(container_B))
+        assert len(container_B) == 5
+        assert container_B_id == id(container_B)
 
 
 class TestTrajectoryTransitionAnalysis(object):
     def setup_method(self):
         op = paths.FunctionCV("Id", lambda snap : snap.coordinates[0][0])
         vol1 = paths.CVDefinedVolume(op, 0.1, 0.5)
         vol2 = paths.CVDefinedVolume(op, -0.1, 0.7)
@@ -137,131 +137,128 @@
 
         return make_1d_traj(coordinates=sequence,
                             velocities=[1.0]*len(sequence))
 
     def test_analyze_continuous_time(self):
         resultA = self.analyzer.analyze_continuous_time(self.trajectory,
                                                         self.stateA)
-        assert_equal(resultA.n_frames.tolist(), [3, 1, 1, 1, 1, 1, 1])
+        assert resultA.n_frames.tolist() == [3, 1, 1, 1, 1, 1, 1]
         resultB = self.analyzer.analyze_continuous_time(self.trajectory,
                                                         self.stateB)
-        assert_equal(resultB.n_frames.tolist(), [1, 1, 1, 5])
+        assert resultB.n_frames.tolist() == [1, 1, 1, 5]
         assert_almost_equal(resultA.times.mean(), 9.0/7.0*0.1)
         assert_almost_equal(resultB.times.mean(), 8.0/4.0*0.1)
 
     def test_analyze_lifetime(self):
         resA = self.analyzer.analyze_lifetime(self.trajectory, self.stateA)
         resB = self.analyzer.analyze_lifetime(self.trajectory, self.stateB)
-        assert_equal(resA.n_frames.tolist(), [3, 1, 2])  # A->B
-        assert_equal(resB.n_frames.tolist(), [2, 1, 1, 11])  # B->A
+        assert resA.n_frames.tolist() == [3, 1, 2]  # A->B
+        assert resB.n_frames.tolist() == [2, 1, 1, 11]  # B->A
         assert_almost_equal(resA.times.mean(), 6.0/3.0*0.1)
         assert_almost_equal(resB.times.mean(), 15.0/4.0*0.1)
 
     def test_analyze_transition_duration(self):
         resAB = self.analyzer.analyze_transition_duration(self.trajectory,
                                                           self.stateA,
                                                           self.stateB)
         resBA = self.analyzer.analyze_transition_duration(self.trajectory,
                                                           self.stateB,
                                                           self.stateA)
-        assert_equal(resAB.n_frames.tolist(), [2, 0, 0, 1])
-        assert_equal(resBA.n_frames.tolist(), [1, 0, 0, 6])
-        assert_equal(resAB.times.mean(), 3.0/4.0*0.1)
-        assert_equal(resBA.times.mean(), 7.0/4.0*0.1)
+        assert resAB.n_frames.tolist() == [2, 0, 0, 1]
+        assert resBA.n_frames.tolist() == [1, 0, 0, 6]
+        assert resAB.times.mean() == 3.0/4.0*0.1
+        assert resBA.times.mean() == 7.0/4.0*0.1
 
     def test_analyze_flux(self):
         # A: [{out: 1, in: 1}
         # B: insufficient
         # NOTE: we may want a separate trajectory for this
         flux_core_test_str = "axaxaaaxxaxbxaaxxabaa"
         # frame numbers       0    5    0    5    0
         # in (I) or out (O):   OIOIIIOOI   IIOO
         core_traj = self._make_traj(flux_core_test_str)
         flux_segs_A = self.analyzer.analyze_flux(core_traj, self.stateA)
         # flux_segs_A = self.analyzer.flux_segments[self.stateA]
-        assert_equal(len(flux_segs_A['in']), 4)
-        assert_equal(flux_segs_A['in'][0], core_traj[2:3])
-        assert_equal(flux_segs_A['in'][1], core_traj[4:7])
-        assert_equal(flux_segs_A['in'][2], core_traj[9:10])
-        assert_equal(flux_segs_A['in'][3], core_traj[13:15])
-
-        assert_equal(len(flux_segs_A['out']), 4)
-        assert_equal(flux_segs_A['out'][0], core_traj[1:2])
-        assert_equal(flux_segs_A['out'][1], core_traj[3:4])
-        assert_equal(flux_segs_A['out'][2], core_traj[7:9])
-        assert_equal(flux_segs_A['out'][3], core_traj[15:17])
+        assert len(flux_segs_A['in']) == 4
+        assert flux_segs_A['in'][0] == core_traj[2:3]
+        assert flux_segs_A['in'][1] == core_traj[4:7]
+        assert flux_segs_A['in'][2] == core_traj[9:10]
+        assert flux_segs_A['in'][3] == core_traj[13:15]
+
+        assert len(flux_segs_A['out']) == 4
+        assert flux_segs_A['out'][0] == core_traj[1:2]
+        assert flux_segs_A['out'][1] == core_traj[3:4]
+        assert flux_segs_A['out'][2] == core_traj[7:9]
+        assert flux_segs_A['out'][3] == core_traj[15:17]
 
     def test_analyze_flux_with_interface(self):
         flux_iface_traj_str = "aixixaiaxiixiaxaixbxbixiaaixiai"
         # frame numbers        0    5    0    5    0    5    0
         # in (I) or out (O)      OOOIIIOOOOOIOII       IIIOO
-        assert_equal(len(flux_iface_traj_str), 31) # check I counted correctly
+        assert len(flux_iface_traj_str) == 31 # check I counted correctly
         flux_traj = self._make_traj(flux_iface_traj_str)
         self.analyzer.reset_analysis()
         flux_segs_A = self.analyzer.analyze_flux(flux_traj, self.stateA,
                                                  self.interfaceA0)
         # flux_segs_A = self.analyzer.flux_segments[self.stateA]
-        assert_equal(flux_segs_A['in'][:],
-                     [flux_traj[5:8], flux_traj[13:14], flux_traj[15:17],
-                      flux_traj[24:27]])
-        assert_equal(flux_segs_A['out'][:],
-                     [flux_traj[2:5], flux_traj[8:13], flux_traj[14:15],
-                      flux_traj[27:29]])
+        assert flux_segs_A['in'][:] == [flux_traj[5:8], flux_traj[13:14],
+                                        flux_traj[15:17], flux_traj[24:27]]
+        assert flux_segs_A['out'][:] == [flux_traj[2:5], flux_traj[8:13],
+                                         flux_traj[14:15], flux_traj[27:29]]
 
     def test_minus_flux(self):
         flux_iface_traj_str = "axxxaaaxxxa"
         flux_traj = self._make_traj(flux_iface_traj_str)
         self.analyzer.reset_analysis()
         flux_segs_A = self.analyzer.analyze_flux(flux_traj, self.stateA,
                                                  self.interfaceA0)
-        assert_equal(flux_segs_A['in'][:], [flux_traj[4:7]])
-        assert_equal(flux_segs_A['out'][:],
-                     [flux_traj[1:4], flux_traj[7:10]])
+        assert flux_segs_A['in'][:] == [flux_traj[4:7]]
+        assert flux_segs_A['out'][:] == [flux_traj[1:4], flux_traj[7:10]]
 
     def test_flux(self):
         flux_iface_traj_str = "aixixaiaxiixiaxaixbxbixiaaixiai"
         flux_traj = self._make_traj(flux_iface_traj_str)
         self.analyzer.reset_analysis()
         self.analyzer.dt = 1.0
         flux = self.analyzer.flux(trajectories=[flux_traj],
                                   state=self.stateA,
                                   interface=self.interfaceA0)
         average_out = old_div((3.0 + 5.0 + 1.0 + 2.0), 4.0)
         average_in = old_div((3.0 + 1.0 + 2.0 + 3.0), 4.0)
         assert_almost_equal(flux, old_div(1.0, (average_out + average_in)))
         self.analyzer.dt = None
 
-    @raises(RuntimeError)
     def test_flux_no_dt(self):
         analyzer = paths.TrajectoryTransitionAnalysis(self.transition)
         flux_iface_traj_str = "aixixaiaxiixiaxaixbxbixiaaixiai"
         flux_traj = self._make_traj(flux_iface_traj_str)
-        flux = analyzer.flux(trajectories=[flux_traj],
-                             state=self.stateA,
-                             interface=self.interfaceA0)
+        with pytest.raises(RuntimeError):
+            flux = analyzer.flux(trajectories=[flux_traj],
+                                 state=self.stateA,
+                                 interface=self.interfaceA0)
 
     def test_analyze(self):
         # only test that it runs -- correctness testing in the others
         self.analyzer.analyze(self.trajectory)
         cont_frames = self.analyzer.continuous_frames
         life_frames = self.analyzer.lifetime_frames
         trans_frames = self.analyzer.transition_duration_frames
         cont_times = self.analyzer.continuous_times
         life_times = self.analyzer.lifetimes
         trans_times = self.analyzer.transition_duration
 
         self.analyzer.reset_analysis()
         self.analyzer.analyze([self.trajectory])
-        assert_equal(cont_frames[self.stateA].tolist(),
-                     self.analyzer.continuous_frames[self.stateA].tolist())
-        assert_equal(life_frames[self.stateA].tolist(),
-                     self.analyzer.lifetime_frames[self.stateA].tolist())
+        assert (cont_frames[self.stateA].tolist()
+                == self.analyzer.continuous_frames[self.stateA].tolist())
+        assert (life_frames[self.stateA].tolist()
+                == self.analyzer.lifetime_frames[self.stateA].tolist())
         A2B = (self.stateA, self.stateB)
-        assert_equal(trans_frames[A2B].tolist(),
-                     self.analyzer.transition_duration_frames[A2B].tolist())
-        assert_equal(cont_times[self.stateA].mean(),
-                     self.analyzer.continuous_times[self.stateA].mean())
-        assert_equal(life_times[self.stateA].mean(),
-                     self.analyzer.lifetimes[self.stateA].mean())
-        assert_equal(trans_times[A2B].mean(),
-                     self.analyzer.transition_duration[A2B].mean())
+        assert (trans_frames[A2B].tolist()
+                == self.analyzer.transition_duration_frames[A2B].tolist())
+        assert (cont_times[self.stateA].mean()
+                == self.analyzer.continuous_times[self.stateA].mean())
+        assert (life_times[self.stateA].mean()
+                == self.analyzer.lifetimes[self.stateA].mean())
+        assert (trans_times[A2B].mean()
+                == self.analyzer.transition_duration[A2B].mean())
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_transitions.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_transitions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from __future__ import absolute_import
 from builtins import object
-from nose.tools import assert_equal, assert_not_equal, raises
-from nose.plugins.skip import SkipTest
 from .test_helpers import (
     CallIdentity, prepend_exception_message, make_1d_traj, data_filename,
     assert_items_equal
 )
 
 
 import openpathsampling as paths
@@ -44,36 +42,36 @@
     def _make_traj(self, string):
         pretraj = []
         for l in string:
             pretraj.append({"a" : 0.3, "b" : 2.2, "i" : 0.6, "x" : 1.0}[l])
         return make_1d_traj(coordinates=pretraj, velocities=[1.0]*len(pretraj))
 
     def test_init(self):
-        assert_equal(len(self.transition.ensembles), 1)
-        assert_equal(self.transition.length, 4)
-        assert_equal(self.transition.ensembles[0](self.good_traj), True)
-        assert_equal(self.transition.ensembles[0](self.short_traj), False)
-        assert_equal(self.transition.ensembles[0](self.long_traj), False)
-        assert_equal(self.transition.ensembles[0](self.bad_states_traj), False)
+        assert len(self.transition.ensembles) == 1
+        assert self.transition.length == 4
+        assert self.transition.ensembles[0](self.good_traj)
+        assert not self.transition.ensembles[0](self.short_traj)
+        assert not self.transition.ensembles[0](self.long_traj)
+        assert not self.transition.ensembles[0](self.bad_states_traj)
 
     def test_storage(self):
         import os
         filename = data_filename("transitions.nc")
         if os.path.isfile(filename):
             os.remove(filename)
         storage = paths.Storage(filename, "w")
         storage.snapshots.save(self.good_traj[0])
 
         storage.save(self.transition)
-        assert_equal(len(storage.transitions), 1)
+        assert len(storage.transitions) == 1
         storage.sync_all()
 
         storage_r = paths.storage.AnalysisStorage(filename)
         reloaded = storage_r.transitions[0]
-        assert_equal(self.transition.ensembles[0], reloaded.ensembles[0])
+        assert self.transition.ensembles[0] == reloaded.ensembles[0]
 
         if os.path.isfile(filename):
             os.remove(filename)
 
 class TestMinusSidesSummary(object):
     def setup_method(self):
         op = paths.FunctionCV("Id", lambda snap : snap.coordinates[0][0])
@@ -102,42 +100,42 @@
         pretraj = []
         for l in string:
             pretraj.append({"a" : 0.3, "b" : 2.2, "i" : 0.6, "x" : 1.0}[l])
         return make_1d_traj(coordinates=pretraj, velocities=[1.0]*len(pretraj))
 
     def test_normal_minus(self):
         minus = paths.MinusInterfaceEnsemble(self.stateA, self.stateA)
-        assert_equal(minus_sides_summary(self.traj_axaxa, minus),
-                     {"in" : [5], "out" : [4]})
-        assert_not_equal(minus_sides_summary(self.traj_axaxa, minus),
-                         {"in" : [5], "out" : [3]})
-        assert_equal(minus_sides_summary(self.traj_aixiaixia, minus),
-                     {"in" : [5], "out" : [6] })
-        assert_equal(minus_sides_summary(self.traj_aixixiaxia, minus),
-                     {"in" : [5], "out" : [10] })
+        assert (minus_sides_summary(self.traj_axaxa, minus)
+                == {"in" : [5], "out" : [4]})
+        assert (minus_sides_summary(self.traj_axaxa, minus)
+                != {"in" : [5], "out" : [3]})
+        assert (minus_sides_summary(self.traj_aixiaixia, minus)
+                == {"in" : [5], "out" : [6] })
+        assert (minus_sides_summary(self.traj_aixixiaxia, minus)
+                == {"in" : [5], "out" : [10] })
 
     def test_minus_with_interstitial(self):
         minus = paths.MinusInterfaceEnsemble(self.stateA, self.innermost)
-        assert_equal(minus_sides_summary(self.traj_axaxa, minus),
-                     {"in" : [5], "out" : [4]})
-        assert_equal(minus_sides_summary(self.traj_aixiaixia, minus),
-                     {"in" : [6], "out" : [4] })
-        assert_equal(minus_sides_summary(self.traj_aixixiaxia, minus),
-                     {"in" : [5], "out" : [8] })
+        assert (minus_sides_summary(self.traj_axaxa, minus)
+                == {"in" : [5], "out" : [4]})
+        assert (minus_sides_summary(self.traj_aixiaixia, minus)
+                == {"in" : [6], "out" : [4] })
+        assert (minus_sides_summary(self.traj_aixixiaxia, minus)
+                == {"in" : [5], "out" : [8] })
 
     def test_minus_with_multiple_excursion(self):
         minus = paths.MinusInterfaceEnsemble(self.stateA, self.stateA,
                                              n_l=4)
-        assert_equal(minus_sides_summary(self.traj_axaxaxaxa, minus),
-                     {"in" : [2, 3, 4], "out" : [1, 2, 3]})
-        assert_equal(minus_sides_summary(self.traj_aixixiaixaxiaixia, minus),
-                     {"in" : [2, 1, 3], "out" : [7, 4, 3]})
+        assert (minus_sides_summary(self.traj_axaxaxaxa, minus)
+                == {"in" : [2, 3, 4], "out" : [1, 2, 3]})
+        assert (minus_sides_summary(self.traj_aixixiaixaxiaixia, minus)
+                == {"in" : [2, 1, 3], "out" : [7, 4, 3]})
 
     def test_minus_with_interstitial_and_multiple_excursion(self):
         minus = paths.MinusInterfaceEnsemble(self.stateA, self.innermost, n_l=4)
-        assert_equal(minus_sides_summary(self.traj_axaxaxaxa, minus),
-                     {"in" : [2, 3, 4], "out" : [1, 2, 3]})
-        assert_equal(minus_sides_summary(self.traj_aixixiaixaxiaixia, minus),
-                     {"in" : [4, 1, 5], "out" : [6, 2, 3]})
-        assert_not_equal(minus_sides_summary(self.traj_aixixiaixaxiaixia, minus),
-                     {"in" : [1, 4, 5], "out" : [6, 2, 3]})
+        assert (minus_sides_summary(self.traj_axaxaxaxa, minus)
+                == {"in" : [2, 3, 4], "out" : [1, 2, 3]})
+        assert (minus_sides_summary(self.traj_aixixiaixaxiaixia, minus)
+                == {"in" : [4, 1, 5], "out" : [6, 2, 3]})
+        assert (minus_sides_summary(self.traj_aixixiaixaxiaixia, minus)
+                != {"in" : [1, 4, 5], "out" : [6, 2, 3]})
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_visit_all_states.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_visit_all_states.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_volume.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_volume.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/tests/test_wham.py` & `openpathsampling-1.6.1/openpathsampling/tests/test_wham.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from __future__ import division
 from __future__ import absolute_import
 from builtins import object
+import pytest
 from past.utils import old_div
-from nose.tools import (assert_equal, assert_not_equal, raises,
-                        assert_almost_equal)
-from nose.plugins.skip import SkipTest
 from .test_helpers import assert_items_almost_equal, assert_items_equal
 
 import pandas as pd
 import numpy as np
 import openpathsampling as paths
 
 import logging
@@ -157,44 +155,44 @@
         expected_Z = np.array([1.0, 0.25, 0.25*0.2])
         np.testing.assert_allclose(guess_lnZ.values, np.log(expected_Z))
 
     def test_wham_bam_histogram(self):
         wham_hist = self.wham.wham_bam_histogram(self.input_df)
         np.testing.assert_allclose(wham_hist.values, self.exact)
 
-    @raises(RuntimeError)
     def test_check_overlaps_no_overlap_with_first(self):
         bad_data = np.array([[1.0, 0.0, 0.0],
                              [0.5, 0.0, 0.0],
                              [0.0, 1.0, 0.0],
                              [0.0, 0.5, 1.0],
                              [0.0, 0.1, 0.2]])
         bad_df = pd.DataFrame(data=bad_data,
                               index=self.index[0:5],
                               columns=self.columns)
-        self.wham.check_cleaned_overlaps(bad_df)
+        with pytest.raises(RuntimeError):
+            self.wham.check_cleaned_overlaps(bad_df)
 
-    @raises(RuntimeError)
     def test_check_overlaps_no_overlap_with_final(self):
         bad_data = np.array([[1.0, 0.0, 0.0],
                              [0.5, 0.0, 0.0],
                              [0.2, 1.0, 0.0],
                              [0.1, 0.5, 0.0],
                              [0.0, 0.0, 1.0],
                              [0.0, 0.0, 0.5]])
         bad_df = pd.DataFrame(data=bad_data,
                               index=self.index[0:6],
                               columns=self.columns)
-        self.wham.check_cleaned_overlaps(bad_df)
+        with pytest.raises(RuntimeError):
+            self.wham.check_cleaned_overlaps(bad_df)
 
-    @raises(RuntimeError)
     def test_check_overlaps_no_overlap_in_middle(self):
         bad_data = np.array([[1.0, 0.0, 0.0, 0.0],
                              [0.5, 1.0, 0.0, 0.0],
                              [0.1, 0.2, 0.0, 0.0],
                              [0.0, 0.0, 1.0, 0.0],
                              [0.0, 0.0, 0.5, 1.0],
                              [0.0, 0.0, 0.1, 0.2]])
         bad_df = pd.DataFrame(data=bad_data,
                               index=self.index[0:6],
                               columns=self.columns + ['Interface 4'])
-        self.wham.check_cleaned_overlaps(bad_df)
+        with pytest.raises(RuntimeError):
+            self.wham.check_cleaned_overlaps(bad_df)
```

### Comparing `openpathsampling-1.6.0/openpathsampling/tools.py` & `openpathsampling-1.6.1/openpathsampling/tools.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/treelogic.py` & `openpathsampling-1.6.1/openpathsampling/treelogic.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,15 +284,15 @@
             the function run at each node. The first argrument of the
             callable must be the node, and may take optional (fixed)
             parameters
 
         Returns
         -------
         list :
-            tree (fnc(node, \*\*kwargs))
+            tree (fnc(node, **kwargs))
             nested list of the results of the map
         """
         return [fnc(self)] + [ch.map_tree(fnc) for ch in self._subnodes]
 
     @property
     def identifier(self):
         """
@@ -345,15 +345,15 @@
             the function run at each node. It is given the node and the
             optional (fixed) parameters
         kwargs : named arguments
             optional arguments added to the function
 
         Returns
         -------
-        list (fnc(node, \*\*kwargs))
+        list (fnc(node, **kwargs))
             flattened list of the results of the map
 
         Notes
         -----
         This uses the same order as `reversed()`
 
         See also
@@ -368,15 +368,15 @@
 
         This traverses the underlying tree and applies the given function at
         each node returning a list of the results. Post-order means
         that subnodes are called BEFORE the node itself is evaluated.
 
         Parameters
         ----------
-        fnc : function(node, \*\*kwargs)
+        fnc : function(node, **kwargs)
             the function run at each node. It is given the node and the
             optional (fixed) parameters
         level : int
             the initial level
         kwargs : named arguments
             optional arguments added to the function
 
@@ -404,23 +404,23 @@
 
         This traverses the underlying tree applies the given function at
         each node returning a list of the results. Pre-order means
         that subnodes are called AFTER the node itself is evaluated.
 
         Parameters
         ----------
-        fnc : function(node, \*\*kwargs)
+        fnc : function(node, **kwargs)
             the function run at each node. It is given the node and the
             optional parameters
         kwargs : named arguments
             optional arguments added to the function
 
         Returns
         -------
-        list (fnc(node, \*\*kwargs))
+        list (fnc(node, **kwargs))
             flattened list of the results of the map
 
         Notes
         -----
         This uses the same order as `iter()`
 
         See also
@@ -435,15 +435,15 @@
 
         This traverses the underlying tree applies the given function at
         each node returning a list of the results. Pre-order means
         that subnodes are called AFTER the node itself is evaluated.
 
         Parameters
         ----------
-        fnc : function(node, \*\*kwargs)
+        fnc : function(node, **kwargs)
             the function run at each node. It is given the node and the
             optional parameters
         level : int
             the initial level
         only_canonical : bool, default: False
             if `True` the recursion stops at canonical movers and will hence be
             more compact
```

### Comparing `openpathsampling-1.6.0/openpathsampling/version.py` & `openpathsampling-1.6.1/openpathsampling/version.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/visualize.py` & `openpathsampling-1.6.1/openpathsampling/visualize.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling/volume.py` & `openpathsampling-1.6.1/openpathsampling/volume.py`

 * *Files identical despite different names*

### Comparing `openpathsampling-1.6.0/openpathsampling.egg-info/PKG-INFO` & `openpathsampling-1.6.1/openpathsampling.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpathsampling
-Version: 1.6.0
+Version: 1.6.1
 Summary: A Python package for path sampling simulations
 Home-page: https://github.com/openpathsampling/openpathsampling
 Author: David W.H. Swenson, Jan-Hendrik Prinz, John D. Chodera, and Peter G. Bolhuis
 Author-email: dwhs@hyperblazer.net
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -16,37 +16,36 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: <3.12,>3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: future
 Requires-Dist: psutil
-Requires-Dist: numpy
+Requires-Dist: numpy<2.0
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: netcdf4
 Requires-Dist: svgwrite
 Requires-Dist: networkx
 Requires-Dist: matplotlib
 Requires-Dist: ujson>=4.0.2
 Requires-Dist: dill
+Requires-Dist: sqlalchemy>=1.4.1
 Requires-Dist: mdtraj
 Provides-Extra: test
-Requires-Dist: nose; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: coveralls; extra == "test"
-Requires-Dist: nbval!=0.10.0; extra == "test"
+Requires-Dist: nbval>=0.10.0; extra == "test"
 Provides-Extra: simstore
-Requires-Dist: sqlalchemy>=1.4.1; extra == "simstore"
 
 [![Tests](https://github.com/openpathsampling/openpathsampling/workflows/Tests/badge.svg?branch=master)](https://github.com/openpathsampling/openpathsampling/actions?query=workflow%3ATests)
 [![codecov](https://codecov.io/gh/openpathsampling/openpathsampling/branch/master/graph/badge.svg?token=9W18VHasdb)](https://codecov.io/gh/openpathsampling/openpathsampling)
 
 # OpenPathSampling
 
 An open source Python framework for transition interface and path sampling
```

### Comparing `openpathsampling-1.6.0/openpathsampling.egg-info/SOURCES.txt` & `openpathsampling-1.6.1/openpathsampling.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
+devtools/autorelease_check.py
+devtools/setup_cfg_reqs.py
+devtools/ci/push-docs-to-s3.py
+docs/conf.py
+docs/premake.py
+docs/copyfiles/copyfiles.py
+docs/sphinxext/notebook_sphinxext.py
+docs/sphinxext/pandoc_sphinxext.py
+examples/prep_example_data.py
+examples/alanine_dipeptide_mstis/alatools.py
+examples/resources/toy_plot_helpers.py
 openpathsampling/.gitignore
 openpathsampling/README.md
 openpathsampling/__init__.py
 openpathsampling/_installed_version.py
 openpathsampling/bias_function.py
 openpathsampling/collectivevariable.py
 openpathsampling/deprecations.py
```

### Comparing `openpathsampling-1.6.0/setup.cfg` & `openpathsampling-1.6.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = openpathsampling
-version = 1.6.0
+version = 1.6.1
 description = A Python package for path sampling simulations
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = David W.H. Swenson, Jan-Hendrik Prinz, John D. Chodera, and Peter G. Bolhuis
 author_email = dwhs@hyperblazer.net
 license = MIT
 url = https://github.com/openpathsampling/openpathsampling
@@ -22,40 +22,36 @@
 	Topic :: Scientific/Engineering :: Physics
 	Operating System :: POSIX
 	Operating System :: Unix
 	Operating System :: MacOS
 
 [options]
 include_package_data = True
-python_requires = >3.7,<3.12
+python_requires = >=3.10
 install_requires = 
 	future
 	psutil
-	numpy
+	numpy<2.0
 	scipy
 	pandas
 	netcdf4
 	svgwrite
 	networkx
 	matplotlib
 	ujson>=4.0.2
 	dill
+	sqlalchemy>=1.4.1
 	mdtraj
-packages = find:
+packages = find_namespace:
 
 [options.extras_require]
 test = 
-	nose
 	pytest
 	pytest-cov
 	coveralls
-	nbval!=0.10.0
+	nbval>=0.10.0
 simstore = 
-	sqlalchemy>=1.4.1
-
-[bdist_wheel]
-universal = 1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `openpathsampling-1.6.0/setup.py` & `openpathsampling-1.6.1/setup.py`

 * *Files identical despite different names*

