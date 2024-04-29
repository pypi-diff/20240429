# Comparing `tmp/scipion-em-cryosparc2-4.0.9.tar.gz` & `tmp/scipion-em-cryosparc2-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-cryosparc2-4.0.9.tar", last modified: Fri Nov 17 09:00:49 2023, max compression
+gzip compressed data, was "scipion-em-cryosparc2-4.1.0.tar", last modified: Mon Apr 29 13:26:26 2024, max compression
```

## Comparing `scipion-em-cryosparc2-4.0.9.tar` & `scipion-em-cryosparc2-4.1.0.tar`

### file list

```diff
@@ -1,60 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:00:49.076780 scipion-em-cryosparc2-4.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2023-11-17 09:00:49.076780 scipion-em-cryosparc2-4.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:00:49.068780 scipion-em-cryosparc2-4.0.9/cryosparc2/
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (127)    32609 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:00:49.068780 scipion-em-cryosparc2-4.0.9/cryosparc2/convert/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/convert/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    28554 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/convert/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    10530 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/convert/cs2Start.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/convert/dataimport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/cryosparc2_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:00:49.072780 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16326 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23486 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    24105 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    21382 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    11456 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py
--rw-r--r--   0 runner    (1001) docker     (127)    14366 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3d_variability.py
--rw-r--r--   0 runner    (1001) docker     (127)    15974 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py
--rw-r--r--   0 runner    (1001) docker     (127)    24600 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_ab.py
--rw-r--r--   0 runner    (1001) docker     (127)    15221 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16530 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)    23668 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (127)    34472 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)    38359 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)    20781 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4615 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py
--rw-r--r--   0 runner    (1001) docker     (127)    14132 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_part_subtract.py
--rw-r--r--   0 runner    (1001) docker     (127)    10025 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_sharppening.py
--rw-r--r--   0 runner    (1001) docker     (127)     9546 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:00:49.072780 scipion-em-cryosparc2-4.0.9/cryosparc2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    47395 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/tests/test_protocols_cryosparc2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6304 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34894 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:00:49.076780 scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_2Dclassify.py
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_initialmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_partsubtract.py
--rw-r--r--   0 runner    (1001) docker     (127)    10873 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_refinement.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/cryosparc2/wizards.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 09:00:49.076780 scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2023-11-17 09:00:49.000000 scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2023-11-17 09:00:49.000000 scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 09:00:49.000000 scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2023-11-17 09:00:49.000000 scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-11-17 09:00:49.000000 scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-17 09:00:49.000000 scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-17 09:00:49.076780 scipion-em-cryosparc2-4.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8736 2023-11-17 09:00:04.000000 scipion-em-cryosparc2-4.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:26.470176 scipion-em-cryosparc2-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-04-29 13:26:26.470176 scipion-em-cryosparc2-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8935 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:26.462176 scipion-em-cryosparc2-4.1.0/cryosparc2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4091 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32627 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:26.466176 scipion-em-cryosparc2-4.1.0/cryosparc2/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/convert/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28554 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/convert/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10530 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/convert/cs2Start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/convert/dataimport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/cryosparc2_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:26.470176 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18229 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23486 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24105 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16841 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_flex_mesh_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11801 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14366 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3d_variability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26982 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24600 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_ab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14940 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_blob_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23246 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34102 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40077 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20362 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4615 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_part_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9606 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_patch_ctf_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10025 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_sharppening.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:26.470176 scipion-em-cryosparc2-4.1.0/cryosparc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47395 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/tests/test_protocols_cryosparc2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6304 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37814 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:26.470176 scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_2Dclassify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_initialmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_partsubtract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14120 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/cryosparc2/wizards.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:26:26.470176 scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-04-29 13:26:26.000000 scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-29 13:26:26.000000 scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:26:26.000000 scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 13:26:26.000000 scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-29 13:26:26.000000 scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-29 13:26:26.000000 scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:26:26.470176 scipion-em-cryosparc2-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-04-29 13:25:48.000000 scipion-em-cryosparc2-4.1.0/setup.py
```

### Comparing `scipion-em-cryosparc2-4.0.9/LICENSE` & `scipion-em-cryosparc2-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/PKG-INFO` & `scipion-em-cryosparc2-4.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryosparc2
-Version: 4.0.9
+Version: 4.1.0
 Summary: Plugin to use cryoSPARC2 programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryosparc2
 Author: Yunior C. Fonseca Reyna, Szu-Chi Chung
 Author-email: cfonseca@cnb.csic.es, phonchi@stat.sinica.edu.tw
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryosparc2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryosparc2/
@@ -30,34 +30,64 @@
         * **Helical 3D Refinement**: Reconstruct and refine a homogeneous helical assembly, with or without imposition and refinement of symmetry parameters.
         * **3D Homogeneous Refinement(new)**: Rapidly refine a single homogeneous structure to high-resolution and validate using the gold-standard FSC. Using new faster GPU code, and support for higher-order aberration (beam tilt, spherical aberration, trefoil, tetrafoil) correction and per-particle defocus refinement on the fly.
         * **3D Non uniform Refinement(new)**: Apply non-uniform refinement to achieve higher resolution and map quality. Specially designed for small proteins and membrane proteins.
         * **3D Local Refinement(new)**  Refine a masked region within a consensus structure by allowing particle alignments to vary only slightly.
         * **Symmetry Expansion**: Duplicate particles around a point-group symmetry.
         * **Homogeneous Reconstruction**: Reconstruct half-maps from input particles with alignments
         * **3D Classification**: Classify particles into multiple 3D classes and optimize 3D class densities (currently, without re-aligning particle pose or shift).
+        * **3D Variability Analysis**: Protocol to compute the principle modes of variability with a dataset of aligned particles
+        * **3D Variability Display**: Protocol to create various versions of a 3D variability result that can be used for display
+        * **Blob Picker**: Automatically picks particles by searching for Gaussian signals.
+        * **Patch CTF Estimation**:  Patch-based CTF estimation automatically estimates defocus variation for tilted, bent, deformed samples and is accurate for all particle sizes and types including flexible and membrane proteins.
+        * **3D Flex Data Prep**: Prepares particles for use in 3DFlex training and reconstruction. At the same  way,  Takes in a consensus (rigid) refinement density map, plus optionally a segmentation and generates a tetrahedral mesh for 3DFlex.
+        * **3D Flex Mesh Prep**: Takes in a consensus (rigid) refinement density map, plus optionally a segmentation and generates a tetrahedral mesh for 3DFlex. See Mesh Generation below.
+        * **3D Flex Training**: Uses a mesh and prepared particles (at a downsampled resolution) to train a 3DFlex model. Parameters control the number of latent dimensions, size of the model, and training hyperparameters. This job outputs checkpoints during training.
+        * **3D Flex Reconstruction**: Takes in a checkpoint from training as well as prepared high-resolution particles and performs high-resolution refinement using L-BFGS under the 3DFlex model. This is the stage at which improvements to density in high-res regions are computed. Outputs two half-maps that can be used for FSC validation, sharpening, and other downstream tasks.
+        
         
         **Latest plugin version**
         ==========================
         
-        **v4.0.9**
+        
+        **v4.1.0**
         -----------
-        * **new**        Compatibility with cryoSPARC v4.4.0
-        * **fixed**      Handling aborted protocols/jobs
+        * **fixed**       Tolerating deletion of projects within CS as well as their folders in the file system
+        
+        * **new**         Add new protocols:
+                            * **3D Flex Data Prep**: Prepares particles for use in 3DFlex training and reconstruction. At the same  way,  Takes in a consensus (rigid) refinement density map, plus optionally a segmentation and generates a tetrahedral mesh for 3DFlex.
+                            * **3D Flex Mesh Prep**: Takes in a consensus (rigid) refinement density map, plus optionally a segmentation and generates a tetrahedral mesh for 3DFlex. See Mesh Generation below.
+                            * **3D Flex Training**: Uses a mesh and prepared particles (at a downsampled resolution) to train a 3DFlex model. Parameters control the number of latent dimensions, size of the model, and training hyperparameters. This job outputs checkpoints during training.
+                            * **3D Flex Reconstruction**: Takes in a checkpoint from training as well as prepared high-resolution particles and performs high-resolution refinement using L-BFGS under the 3DFlex model. This is the stage at which improvements to density in high-res regions are computed. Outputs two half-maps that can be used for FSC validation, sharpening, and other downstream tasks.
+        
+        * **new**         Allowing Scipion to import coordinates
+        
+        
+        **v4.0.11**
+        -----------
+        * **fixed**      Compatibility with cryoSPARC v4.4.1+patch
         
-        **v4.0.8**
+        
+        
+        **v4.0.10**
         -----------
-        * **new**        Compatibility with cryoSPARC v4.3.1
-        * **removed**    Deprecated protocols removed: Legacy Refine, Legacy no uniform refine, Legacy naive local refine.
+        * **new**        Compatibility with cryoSPARC v4.4.1
+        * **new**        Add new protocols:
+        
+                         * **3D Variability Analysis**: Protocol to compute the principle modes of variability with a dataset of aligned particles
+                         * **3D Variability Display**: Protocol to create various versions of a 3D variability result that can be used for display
+                         * **Blob Picker**: Automatically picks particles by searching for Gaussian signals.
+        
+        
         
-        **v4.0.7**
+        
+        **v4.0.9**
         -----------
-        * **new**     :  Compatibility with cryoSPARC v4.2.1
-        * **new**        Plugin operation in a cluster
-        * **fixed**      Fixed an installation error
-        * **fixed**      Fixed an error related with the calculation of the particles shifts
+        * **new**        Compatibility with cryoSPARC v4.4.0
+        * **fixed**      Handling aborted protocols/jobs
+        
         
         **Installing the plugin**
         =========================
         
         In order to install the plugin follow these instructions:
         
         1. **Install the plugin**
```

### Comparing `scipion-em-cryosparc2-4.0.9/README.rst` & `scipion-em-cryosparc2-4.1.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -20,34 +20,64 @@
 * **Helical 3D Refinement**: Reconstruct and refine a homogeneous helical assembly, with or without imposition and refinement of symmetry parameters.
 * **3D Homogeneous Refinement(new)**: Rapidly refine a single homogeneous structure to high-resolution and validate using the gold-standard FSC. Using new faster GPU code, and support for higher-order aberration (beam tilt, spherical aberration, trefoil, tetrafoil) correction and per-particle defocus refinement on the fly.
 * **3D Non uniform Refinement(new)**: Apply non-uniform refinement to achieve higher resolution and map quality. Specially designed for small proteins and membrane proteins.
 * **3D Local Refinement(new)**  Refine a masked region within a consensus structure by allowing particle alignments to vary only slightly.
 * **Symmetry Expansion**: Duplicate particles around a point-group symmetry.
 * **Homogeneous Reconstruction**: Reconstruct half-maps from input particles with alignments
 * **3D Classification**: Classify particles into multiple 3D classes and optimize 3D class densities (currently, without re-aligning particle pose or shift).
+* **3D Variability Analysis**: Protocol to compute the principle modes of variability with a dataset of aligned particles
+* **3D Variability Display**: Protocol to create various versions of a 3D variability result that can be used for display
+* **Blob Picker**: Automatically picks particles by searching for Gaussian signals.
+* **Patch CTF Estimation**:  Patch-based CTF estimation automatically estimates defocus variation for tilted, bent, deformed samples and is accurate for all particle sizes and types including flexible and membrane proteins.
+* **3D Flex Data Prep**: Prepares particles for use in 3DFlex training and reconstruction. At the same  way,  Takes in a consensus (rigid) refinement density map, plus optionally a segmentation and generates a tetrahedral mesh for 3DFlex.
+* **3D Flex Mesh Prep**: Takes in a consensus (rigid) refinement density map, plus optionally a segmentation and generates a tetrahedral mesh for 3DFlex. See Mesh Generation below.
+* **3D Flex Training**: Uses a mesh and prepared particles (at a downsampled resolution) to train a 3DFlex model. Parameters control the number of latent dimensions, size of the model, and training hyperparameters. This job outputs checkpoints during training.
+* **3D Flex Reconstruction**: Takes in a checkpoint from training as well as prepared high-resolution particles and performs high-resolution refinement using L-BFGS under the 3DFlex model. This is the stage at which improvements to density in high-res regions are computed. Outputs two half-maps that can be used for FSC validation, sharpening, and other downstream tasks.
+
 
 **Latest plugin version**
 ==========================
 
-**v4.0.9**
+
+**v4.1.0**
 -----------
-* **new**        Compatibility with cryoSPARC v4.4.0
-* **fixed**      Handling aborted protocols/jobs
+* **fixed**       Tolerating deletion of projects within CS as well as their folders in the file system
+
+* **new**         Add new protocols:
+                    * **3D Flex Data Prep**: Prepares particles for use in 3DFlex training and reconstruction. At the same  way,  Takes in a consensus (rigid) refinement density map, plus optionally a segmentation and generates a tetrahedral mesh for 3DFlex.
+                    * **3D Flex Mesh Prep**: Takes in a consensus (rigid) refinement density map, plus optionally a segmentation and generates a tetrahedral mesh for 3DFlex. See Mesh Generation below.
+                    * **3D Flex Training**: Uses a mesh and prepared particles (at a downsampled resolution) to train a 3DFlex model. Parameters control the number of latent dimensions, size of the model, and training hyperparameters. This job outputs checkpoints during training.
+                    * **3D Flex Reconstruction**: Takes in a checkpoint from training as well as prepared high-resolution particles and performs high-resolution refinement using L-BFGS under the 3DFlex model. This is the stage at which improvements to density in high-res regions are computed. Outputs two half-maps that can be used for FSC validation, sharpening, and other downstream tasks.
+
+* **new**         Allowing Scipion to import coordinates
+
+
+**v4.0.11**
+-----------
+* **fixed**      Compatibility with cryoSPARC v4.4.1+patch
 
-**v4.0.8**
+
+
+**v4.0.10**
 -----------
-* **new**        Compatibility with cryoSPARC v4.3.1
-* **removed**    Deprecated protocols removed: Legacy Refine, Legacy no uniform refine, Legacy naive local refine.
+* **new**        Compatibility with cryoSPARC v4.4.1
+* **new**        Add new protocols:
+
+                 * **3D Variability Analysis**: Protocol to compute the principle modes of variability with a dataset of aligned particles
+                 * **3D Variability Display**: Protocol to create various versions of a 3D variability result that can be used for display
+                 * **Blob Picker**: Automatically picks particles by searching for Gaussian signals.
+
+
 
-**v4.0.7**
+
+**v4.0.9**
 -----------
-* **new**     :  Compatibility with cryoSPARC v4.2.1
-* **new**        Plugin operation in a cluster
-* **fixed**      Fixed an installation error
-* **fixed**      Fixed an error related with the calculation of the particles shifts
+* **new**        Compatibility with cryoSPARC v4.4.0
+* **fixed**      Handling aborted protocols/jobs
+
 
 **Installing the plugin**
 =========================
 
 In order to install the plugin follow these instructions:
 
 1. **Install the plugin**
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/__init__.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 
 import os
 import pwem as em
 import pyworkflow.utils as pwutils
 
 from .constants import *
 
-__version__ = '4.0.9'
+__version__ = '4.1.0'
 _references = ['Punjani2017', 'Brubaker2017', 'daniel_asarnow_2019_3576630']
 _logo = 'cryosparc2_logo.png'
 
 
 class Plugin(em.Plugin):
     _url = "https://github.com/scipion-em/scipion-em-cryosparc2"
     _homeVar = CRYOSPARC_HOME
     _pathVars = [CRYOSPARC_HOME]
     _supportedVersions = [V3_0_0, V3_0_1, V3_1_0, V3_2_0, V3_3_0, V3_3_1,
                           V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3, V4_1_0,
-                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
+                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
 
     @classmethod
     def _defineVariables(cls):
         cls._defineVar(CRYOSPARC_HOME, os.environ.get(CRYOSPARC_DIR, ""))
         cls._defineVar(CRYO_PROJECTS_DIR, "scipion_projects")
 
     @classmethod
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/bibtex.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/constants.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 V4_1_0 = 'V4.1.0'
 V4_1_1 = 'V4.1.1'
 V4_1_2 = 'V4.1.2'
 V4_2_0 = 'V4.2.0'
 V4_2_1 = 'V4.2.1'
 V4_3_1 = 'V4.3.1'
 V4_4_0 = 'V4.4.0'
+V4_4_1 = 'V4.4.1'
 
 # Symmetry dict
 CS_SYM_NAME = dict()
 CS_SYM_NAME[SYM_CYCLIC] = 'Cn'
 CS_SYM_NAME[SYM_DIHEDRAL_Y] = 'Dn'
 CS_SYM_NAME[SYM_TETRAHEDRAL] = 'T'
 CS_SYM_NAME[SYM_OCTAHEDRAL] = 'O'
@@ -121,17 +122,17 @@
 ALL_ITERS = 1
 SELECTED_ITERS = 2
 
 ANGDIST_2DPLOT = 0
 ANGDIST_CHIMERA = 1
 
 # VOLUME_SLICES = 0
-VOLUME_CHIMERA = 1
+VOLUME_CHIMERA = 0
 VOLUME_CRYOSPARC = 0
-DATA_VIEWER = 0
+DATA_VIEWER = 1
 
 fscValues = dict()
 fscValues['fsc_nomask'] = 'No mask'
 fscValues['fsc_loosemask'] = 'Loose'
 fscValues['fsc_tightmask'] = 'Tight'
 fscValues['fsc_noisesub_raw'] = 'Noise sub_raw'
 fscValues['fsc_noisesub_true'] = 'Noise sub_true'
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/convert/__init__.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/convert/convert.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/convert/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/convert/cs2Start.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/convert/cs2Start.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/convert/dataimport.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/convert/dataimport.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 import os
+import logging
 import emtable
 
-from cryosparc2.convert import (defineArgs, convertCs2Star, readSetOfParticles,
+from cryosparc2 import RELIONCOLUMNS
+from cryosparc2.convert import (convertCs2Star, readSetOfParticles,
                                 cryosparcToLocation)
 from pwem import ALIGN_PROJ
+from pwem.objects import Coordinate, SetOfCoordinates
 
+logger = logging.getLogger(__name__)
 
 class cryoSPARCImport:
     """ Class used to import particles from cryoSPARC projects into Scipion.
     """
     def __init__(self, protocol, csFile):
         self.protocol = protocol
         self._csFile = csFile
         self._createFilenameTemplates()
 
     def _createFilenameTemplates(self):
         """ Centralize how files are called. """
         myDict = {
-            'out_particles': self.protocol._getExtraPath('output_particle.star')
+            'output': self.protocol._getExtraPath('output.star')
         }
         self.protocol._updateFilenamesDict(myDict)
 
     def importParticles(self):
         """
         Import particles from a cs 'particles.cs'
         """
         try:
             csPartFile = os.path.abspath(self._csFile)
-            self.outputStarFn = self.protocol._getFileName('out_particles')
+            self.outputStarFn = self.protocol._getFileName('output')
             argsList = [csPartFile, self.outputStarFn]
             convertCs2Star(argsList)
             # Validate the start file generated
             self._validateConvert()
 
             self.partSet = self.protocol._createSetOfParticles()
             self.partSet.setObjComment('Particles imported from cryosPARC .cs file:\n%s' % self._csFile)
@@ -45,17 +49,63 @@
 
             self._fillDataFromIter(self.partSet)
             self.protocol._defineOutputs(outputParticles=self.partSet)
 
         except Exception as e:
             raise Exception("The .cs file has not been imported: %s" % e)
 
+    def importCoordinates(self):
+        """
+        Import coordinates from a cs 'particles.cs'
+        """
+        micSetPtr = self.protocol.inputMicrographs
+        outputCoords = SetOfCoordinates.create(self.protocol.getPath())
+        outputCoords.setMicrographs(micSetPtr)
+
+        micList = {os.path.basename(mic.getFileName()): mic.clone() for mic in micSetPtr.get()}
+
+        for fileName, _ in self.protocol.iterFiles():
+            if fileName.endswith('.cs'):
+                try:
+                    csPartFile = os.path.abspath(fileName)
+                    outputStarFn = self.protocol._getFileName('output')
+                    argsList = [csPartFile, outputStarFn]
+                    convertCs2Star(argsList)
+                    self._fillSetOfCoordinates(outputCoords, outputStarFn, micList)
+
+                except Exception as e:
+                    logger.error("The .cs file has not been imported: %s" % fileName, exc_info=e)
+
+        return outputCoords
+
+    def _fillSetOfCoordinates(self, outputCoords, outputStarFn, micList):
+
+        coord = Coordinate()
+        mdFileName = '%s@%s' % ('particles', outputStarFn)
+        table = emtable.Table(fileName=outputStarFn)
+
+        for row in table.iterRows(mdFileName):
+            coord.setObjId(None)
+            micName = os.path.basename(row.get(RELIONCOLUMNS.rlnMicrographName.value))
+            splitMicName = micName.split('_')
+            if len(splitMicName) > 1:
+                micName = '_'.join(splitMicName[1:])
+            else:
+                micName = splitMicName[-1]
+            coord.setMicrograph(micList[micName])
+            x = row.get(RELIONCOLUMNS.rlnCoordinateX.value)
+            y = row.get(RELIONCOLUMNS.rlnCoordinateY.value)
+            dim = micList[micName].getDimensions()
+            flipY = dim[1] - y
+            coord.setPosition(x, flipY)
+            # Add it to the set
+            outputCoords.append(coord)
 
     def _fillDataFromIter(self, imgSet):
-        outImgsFn = 'particles@' + self.protocol._getFileName('out_particles')
+        outImgsFn = 'particles@' + self.protocol._getFileName('output')
         readSetOfParticles(outImgsFn, imgSet,
                            postprocessImageRow=self._updateItem,
                            alignType=ALIGN_PROJ,
                            samplingRate=imgSet.getSamplingRate())
 
     def _updateItem(self, item, row):
         index, file = item.getLocation()
@@ -102,27 +152,26 @@
         dirProject = separador.join(dirParticlesPath.split(separador)[:-1])
         imageName = os.path.basename(searchFile)
         imageFolder = os.path.dirname(searchFile)
         realdataPath = dirParticlesPath
         folderContent = []
 
         # Case in which the binaries associated to the .cs file are in the same
-        # folder of .cs file
+        # folder of the .cs file
         filesPath = dirParticlesPath
         if os.path.exists(filesPath):
             folderContent += os.listdir(filesPath)
 
         # Case in which the binaries associated to the .cs file are located in
         # the cryoSPARC folders format
         filesPath2 = os.path.join(dirProject, imageFolder)
         if os.path.exists(filesPath2):
             folderContent += os.listdir(filesPath2)
             realdataPath = filesPath2
 
-
         matchFile = [f for f in folderContent if f.endswith(imageName)]
         if matchFile:
             file = os.path.join(realdataPath, matchFile[0])
             return file
         else:
             raise Exception("The images were expected to be found in one of "
                             "these locations: (%s) or (%s)" % (filesPath,
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/cryosparc2_logo.png` & `scipion-em-cryosparc2-4.1.0/cryosparc2/cryosparc2_logo.png`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/__init__.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,22 @@
 from .protocol_cryosparc_3D_classification import ProtCryoSparc3DClassification
 from .protocol_cryosparc_helical_refinement import ProtCryoSparcHelicalRefine3D
 from .protocol_cryosparc_homogeneous_refine import ProtCryoSparc3DHomogeneousRefine
 from .protocol_cryosparc_new_nonuniform_refine import ProtCryoSparcNewNonUniformRefine3D
 from .protocol_cryosparc_symmetry_expansion import ProtCryoSparcSymmetryExpansion
 from .protocol_cryosparc_homogeneous_reconstruction import ProtCryoSparcHomogeneousReconstruct
 from .protocol_cryosparc_new_3D_classification import ProtCryoSparcNew3DClassification
-"""
+
 from .protocol_cryosparc_3d_variability import ProtCryoSparc3DVariability
-from .protocol_cryosparc_3d_variability_display import ProtCryoSparc3DVariabilityAnalisys
+from .protocol_cryosparc_3d_variability_display import ProtCryoSparc3DVariabilityDisplay
+
+from .protocol_cryosparc_blob_picker import ProtCryoSparcBlobPicker
+from .protocol_cryosparc_patch_ctf_estimation import ProtCryoSparcPatchCTFEstimate
+
 
 from .protocol_cryosparc_3D_flex_data_prepare import ProtCryoSparc3DFlexDataPrepare
+from .protocol_cryosparc_3D_flex_mesh_prepare import ProtCryoSparc3DFlexMeshPrepare
 from .protocol_cryosparc_3D_flex_training import ProtCryoSparc3DFlexTraining
 from .protocol_cryosparc_3D_flex_reconstruction import ProtCryoSparc3DFlexReconstruction
-"""
+
+
+
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_base.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,19 +37,20 @@
 import pyworkflow.utils as pwutils
 from pwem.objects import FSC
 
 from ..constants import V3_3_1, excludedFSCValues, fscValues, V4_0_0, V4_1_0
 from ..convert import convertBinaryVol, writeSetOfParticles, ImageHandler
 from ..utils import (getProjectPath, createEmptyProject,
                      createEmptyWorkSpace, getProjectName,
-                     getCryosparcProjectsDir, createProjectDir,
+                     getCryosparcProjectsDir, createProjectContainerDir,
                      doImportParticlesStar, doImportVolumes, killJob, clearJob,
                      get_job_streamlog, getSystemInfo, getJobStatus,
                      STOP_STATUSES, getCryosparcVersion, getProjectInformation,
-                     getCryosparcProjectId, _getLicenceFromFile)
+                     getCryosparcProjectId, _getLicenceFromFile, doImportMicrographs, getCryosparcProjectsList,
+                     getCryosparcWorkSpaces)
 
 
 class ProtCryosparcBase(pw.EMProtocol):
     """
     This class contains the common functions for all Cryosparc protocols.
     """
     _protCompatibility = []
@@ -57,50 +58,53 @@
     _fscColumns = 6
 
     def _initializeCryosparcProject(self):
         """
         Initialize the cryoSPARC project and workspace
         """
         self._initializeUtilsVariables()
-        # create empty project or load an exists one
-        folderPaths = getProjectPath(self.projectPath)
-        if not folderPaths:
+        projectsList = getCryosparcProjectsList()
+        matchProjects = [project for project in projectsList if project.get('title') == self.projectDirName]
+        folderPaths = getProjectPath(self.projectContainerDir)
+        # create an empty project or load an exists one
+        if not matchProjects or not folderPaths:
+            # create an empty project
             self.emptyProject = createEmptyProject(self.projectPath, self.projectDirName)
             self.projectName = pwobj.String(self.emptyProject[-1].split()[-1])
             self.projectDir = pwobj.String(getProjectInformation(self.projectName,
                                            info='project_dir'))
+            # create an empty workspace
+            self.emptyWorkSpace = createEmptyWorkSpace(self.projectName, self.getRunName(),
+                                                       self.getObjComment())
+            self.workSpaceName = pwobj.String(self.emptyWorkSpace[-1].split()[-1])
+            self._store(self)
         else:
-            self.projectDir = pwobj.String(os.path.join(self.projectContainerDir,
-                                                        str(folderPaths[0])))
+            self.projectDir = pwobj.String(matchProjects[-1]['project_dir'])
             cryosparcVersion = getCryosparcVersion()
             if parse_version(cryosparcVersion) < parse_version(V4_0_0):
-                self.projectName = pwobj.String(folderPaths[0])
+                self.projectName = pwobj.String(matchProjects[-1]['title'])
             else:
-                self.projectName = pwobj.String(getCryosparcProjectId(self.projectDir))
+                self.projectName = pwobj.String(matchProjects[-1]['uid'])
 
-        self._store(self)
+            workspacesList = getCryosparcWorkSpaces(str(self.projectName))
+            self.workSpaceName = pwobj.String(workspacesList[-1]['uid'])
 
-        # create empty workspace
-        self.emptyWorkSpace = createEmptyWorkSpace(self.projectName, self.getRunName(),
-                                      self.getObjComment())
-        self.workSpaceName = pwobj.String(self.emptyWorkSpace[-1].split()[-1])
         self._store(self)
-
         self.currenJob = pwobj.String()
         self._store(self)
 
     def _initializeUtilsVariables(self):
         """
         Initialize all utils cryoSPARC variables
         """
         # Create a cryoSPARC project dir
         self.projectDirName = getProjectName(self.getProject().getShortName())
         self.projectPath = pw.pwutils.join(getCryosparcProjectsDir(),
                                         self.projectDirName)
-        self.projectContainerDir = createProjectDir(self.projectPath)[1]
+        self.projectContainerDir = createProjectContainerDir(self.projectPath)[1]
 
     def convertInputStep(self):
         """ Create the input file in STAR format as expected by Relion.
         If the input particles comes from Relion, just link the file.
         """
         imgSet = self._getInputParticles()
         if imgSet is not None:
@@ -114,14 +118,25 @@
             self._importVolume()
 
         mask = self._getInputMask()
         if mask is not None:
             self._importMask()
         else:
             self.mask = pwobj.String()
+
+        focusMask = self._getInputFocusMask()
+        if focusMask is not None:
+            self._importFocusMask()
+        else:
+            self.focusMask = pwobj.String()
+
+        micrographs = self._getInputMicrographs()
+        if micrographs is not None:
+            self._importMicrographs()
+
         self._store(self)
 
     def _getScaledAveragesFile(self, csAveragesFile, force=False):
 
         # For the moment this is the best possible result, scaling from 128 to
         # 300 does not render nice results apart that the factor turns to
         # 299x299. But without this the representative subset is wrong.
@@ -183,37 +198,47 @@
         return None
 
     def _getInputMask(self):
         if self.hasAttribute('refMask'):
             return self.refMask.get()
         return None
 
+    def _getInputFocusMask(self):
+        if self.hasAttribute('refFocusMask'):
+            return self.refFocusMask.get()
+        return None
+
+    def _getInputMicrographs(self):
+        if self.hasAttribute('inputMicrographs'):
+            return self.inputMicrographs.get()
+        return None
+
     def _initializeVolumeSuffix(self):
         """
-        Create a output volume suffix depend of the CS version
+        Create an output volume suffix depend on the CS version
         """
         cryosparcVersion = parse_version(getCryosparcVersion())
         self.outputVolumeSuffix = '.imported_volume.map'
         self.outputMaskSuffix = '.imported_mask.map'
         self.outputVolumeHalf_A = '.imported_volume.map_half_A'
         self.outputVolumeHalf_B = '.imported_volume.map_half_B'
         if cryosparcVersion >= parse_version(V3_3_1):
             self.outputVolumeSuffix = '.imported_volume_1.map'
             self.outputMaskSuffix = '.imported_mask_1.map'
             self.outputVolumeHalf_A = '.imported_volume_1.map_half_A'
             self.outputVolumeHalf_B = '.imported_volume_1.map_half_B'
 
-    def _initializeMaskSuffix(self):
+    def _initializeMaskSuffix(self, sufix='.imported_mask_1.map'):
         """
         Create a output mask suffix depend of the CS version
         """
         cryosparcVersion = parse_version(getCryosparcVersion())
         self.outputMaskSuffix = '.imported_mask.map'
         if cryosparcVersion >= parse_version(V3_3_1):
-            self.outputMaskSuffix = '.imported_mask_1.map'
+            self.outputMaskSuffix = sufix
 
     def _importVolume(self):
         vol = self._getInputVolume()
         self._initializeVolumeSuffix()
         vol_fn = os.path.join(os.getcwd(), convertBinaryVol(vol, self._getTmpPath()))
         importVolumeJob = doImportVolumes(self, vol_fn, vol, 'map', 'Importing volume...')
         self.volume = pwobj.String(str(importVolumeJob.get()) + self.outputVolumeSuffix)
@@ -238,22 +263,38 @@
                                                             self._getTmpPath()))
 
         importMaskJob = doImportVolumes(self, maskFn, self._getInputMask(),
                                         'mask', 'Importing mask... ')
         self.currenJob.set(importMaskJob.get())
         self.mask = pwobj.String(str(importMaskJob.get()) + self.outputMaskSuffix)
 
-    def _importParticles(self):
+    def _importFocusMask(self):
+        self._initializeMaskSuffix()
+        maskFn = os.path.join(os.getcwd(), convertBinaryVol(self._getInputFocusMask(),
+                                                            self._getTmpPath()))
 
+        importFocusMaskJob = doImportVolumes(self, maskFn, self._getInputMask(),
+                                             'mask', 'Importing focus mask... ')
+        self.currenJob.set(importFocusMaskJob.get())
+        self.focusMask = pwobj.String(str(importFocusMaskJob.get()) + self.outputMaskSuffix)
+
+    def _importParticles(self):
         # import_particles_star
         importedParticlesJob = doImportParticlesStar(self)
         self.currenJob = pwobj.String(str(importedParticlesJob.get()))
         self.particles = pwobj.String(str(importedParticlesJob.get()) +
                                       '.imported_particles')
 
+    def _importMicrographs(self):
+        importedMicrographsJob = doImportMicrographs(self)
+        self.currenJob = pwobj.String(str(importedMicrographsJob.get()))
+        self.micrographs = pwobj.String(str(importedMicrographsJob.get()) +
+                                      '.imported_micrographs')
+
+
     def setAborted(self):
         """ Set the status to aborted and updated the endTime. """
         pw.EMProtocol.setAborted(self)
         if hasattr(self, 'projectName') and hasattr(self, 'currenJob') and self.currenJob.get() is not None:
             job = str(self.currenJob.get())
             project = str(self.projectName.get())
             status = getJobStatus(project, job)
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc2d.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc2d.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_classification.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_classification.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_flex_mesh_prepare.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,94 +30,52 @@
                                         BooleanParam, FileParam, StringParam)
 from . import ProtCryosparcBase
 from ..convert import *
 from ..utils import *
 from ..constants import *
 
 
-class ProtCryoSparc3DFlexDataPrepare(ProtCryosparcBase):
+class ProtCryoSparc3DFlexMeshPrepare(ProtCryosparcBase):
     """
     Prepares particles for use in 3DFlex training and reconstruction. At the same
     way,  Takes in a consensus (rigid) refinement density map, plus optionally
      a segmentation and generates a tetrahedral mesh for 3DFlex.
     """
-    _label = '3D flex data/mesh prepare'
+    _label = '3D flex mesh prepare'
     _devStatus = BETA
     _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1,
-                          V4_4_0]
+                          V4_4_0, V4_4_1]
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineFileNames(self):
         """ Centralize how files are called within the protocol. """
         myDict = {
             'input_particles': self._getTmpPath('input_particles.star'),
             'out_particles': self._getPath() + '/output_particle.star',
             'stream_log': self._getPath() + '/stream.log'
         }
         self._updateFilenamesDict(myDict)
 
     def _defineParams(self, form):
         form.addSection(label='Input')
-        form.addParam('inputParticles', PointerParam,
-                      pointerClass='SetOfParticles',
-                      label="Input particles",
+        form.addParam('dataPrepare', PointerParam,
+                      pointerClass='ProtCryoSparc3DFlexDataPrepare',
+                      label="Data prepare protocol",
                       important=True,
-                      help='Particle stacks to use.')
-        form.addParam('refVolume', PointerParam, pointerClass='Volume',
-                      label='Initial volume',
-                      important=True,
-                      help='Initial volume raw data')
+                      help='Prepared particles and consensus volume from the 3D flex data prepare protocol.')
         form.addParam('refMask', PointerParam, pointerClass='VolumeMask',
                       default=None,
                       label='Input Mask',
                       allowsNull=True,
                       help='Mask raw data')
 
-        form.addSection(label='Data Prepare')
-        form.addParam('box_size_pix', IntParam, default=None,
-                      allowsNull=True,
-                      label="Crop box size (pix)",
-                      help="Crop input particles and volume to this box size. "
-                           "This is the box size that will be used for high "
-                           "resolution reconstruction with 3D Flex. Particles "
-                           "are cropped to this box size first, and then "
-                           "downsampled to the Training Box Size for training "
-                           "time. Default (None) means to keep the original "
-                           "box size of the particles.")
-
-        form.addParam('bin_size_pix', IntParam, default=128,
-                      allowsNull=True,
-                      label="Training box size (pix)",
-                      help="Downsample cropped particles (via Fourier cropping)"
-                           " to this box size for training the 3D Flex model. "
-                           "This should be chosen to limit 3D Flex training to "
-                           "a resolution below the gold-standard FSC resolution "
-                           "of the consensus reconstruction, in order to ensure "
-                           "high resolution reconstructions can be validated. "
-                           "Box sizes over 256 may become prohibitively slow")
-
-        form.addParam('alpha_min', IntParam, default=None,
-                      allowsNull=True,
-                      label="Min. scale to keep",
-                      help="Only keep particles with scale factor above this "
-                           "value. Useful for discarding particles that might "
-                           "be junk.")
-
-        form.addParam('keep_num_particles', IntParam, default=None,
-                      allowsNull=True,
-                      label="Num. particles to use",
-                      help="Only keep the first X particles. The final number"
-                           " of particles used during 3D Flex training "
-                           "and reconstruction must be divisible by 1000. "
-                           "If this is None (default) then the number of input "
-                           "particles will be rounded down to the nearest 1000.")
-
         form.addSection(label='Mesh Prepare')
 
-        solventMaskGroup = form.addGroup('Solvent mask preparation')
+        solventMaskGroup = form.addGroup('Solvent mask preparation',
+                                         condition="refMask is None")
         solventMaskGroup.addParam('mask_in_lowpass_A', IntParam, default=10,
                                   condition="refMask is None",
                                   label="Filter input volume res. (A)",
                                   help="Filter the input consensus reconstruction "
                                        "volume to this resolution (A) before thresholding "
                                        "to create the outer solvent mask. Solvent mask is"
                                        " only generated if it is not already input.")
@@ -141,16 +99,14 @@
         solventMaskGroup.addParam('mask_pad_A', IntParam,
                                   default=5,
                                   condition="refMask is None",
                                   label="Mask soft padding (A)",
                                   help="After thresholding and dilation, soft "
                                        "pad by this much (A) to create solvent mask")
 
-
-
         meshPreparationGroup = form.addGroup('Mesh preparation')
         meshPreparationGroup.addParam('tetra_num_cells', IntParam,
                                   default=20,
                                   label="Base num. tetra cells",
                                   help="Number of tetrahedral cells that fit "
                                        "across the extent of the box. Use this "
                                        "to set the size of mesh elements. If "
@@ -232,23 +188,18 @@
 
     def _insertAllSteps(self):
         self._defineFileNames()
         self._defineParamsPrepareName()
         self._defineParamsMeshName()
         self._initializeCryosparcProject()
         self._insertFunctionStep(self.convertInputStep)
-        self._insertFunctionStep(self.dataPrepareStep)
         self._insertFunctionStep(self.mergePrepareStep)
         self._insertFunctionStep(self.createOutputStep)
 
     # --------------------------- STEPS functions ------------------------------
-    def dataPrepareStep(self):
-        self.info(pwutils.yellowStr("3D Flex Data Preparation started..."))
-        self.doRun3DFlexDataPrepare()
-
     def mergePrepareStep(self):
         self.info(pwutils.yellowStr("3D Flex Mesh Preparation started..."))
         self.doRun3DFlexMeshPrepare()
 
     def createOutputStep(self):
         """
         Create the protocol output. Convert cryosparc file to Relion file
@@ -297,26 +248,14 @@
 
     def _createItemMatrix(self, particle, row):
         createItemMatrix(particle, row, align=ALIGN_PROJ)
         setCryosparcAttributes(particle, row, RELIONCOLUMNS.rlnRandomSubset.value)
 
     def _validate(self):
         validateMsgs = cryosparcValidate()
-        if not validateMsgs:
-            particles = self._getInputParticles()
-            if not particles.hasCTF():
-                validateMsgs.append(
-                    "The Particles has not associated a CTF model")
-                if not particles.hasAlignment3D():
-                    validateMsgs.append("The Particles has not aligned")
-                    if self.keep_num_particles.get() % 1000 != 0:
-                        validateMsgs.append("The final number of particles "
-                                            "used during 3D Flex training and "
-                                            "reconstruction must be divisible by 1000")
-
         return validateMsgs
 
     def _defineParamsPrepareName(self):
         """ Define a list with 3D Flex Prepare Data parameters names"""
         self._paramsPrepareName = ['box_size_pix', 'bin_size_pix', 'alpha_min',
                             'keep_num_particles']
         self.lane = str(self.getAttributeValue('compute_lane'))
@@ -327,44 +266,18 @@
                                      'mask_dilate_A', 'mask_pad_A']
         self._paramsMeshName = ['tetra_num_cells', 'tetra_segments_path',
                                 'tetra_segments_fuse_list', 'tetra_rigid_list',
                                 'rigidity_penalty_min',
                                 'rigidity_penalty_stiffen_low_density']
         self.lane = str(self.getAttributeValue('compute_lane'))
 
-    def doRun3DFlexDataPrepare(self):
-        self._className = "flex_prep"
-        input_group_connect = {"particles": self.particles.get(),
-                               "volume": self.volume.get()}
-        params = {}
-
-        for paramName in self._paramsPrepareName:
-            if self.getAttributeValue(paramName) is not None:
-                params[str(paramName)] = str(self.getAttributeValue(paramName))
-
-        run3DFlexDataPrepJob = enqueueJob(self._className, self.projectName.get(),
-                                  self.workSpaceName.get(),
-                                  str(params).replace('\'', '"'),
-                                  str(input_group_connect).replace('\'', '"'),
-                                  self.lane, False)
-
-        self.run3DFlexDataPrepJob = String(run3DFlexDataPrepJob.get())
-        self.currenJob.set(self.run3DFlexDataPrepJob.get())
-        self._store(self)
-
-        waitForCryosparc(self.projectName.get(), self.run3DFlexDataPrepJob.get(),
-                         "An error occurred in the 3D Flex Data Preparation process. "
-                         "Please, go to cryoSPARC software for more "
-                         "details.")
-        clearIntermediateResults(self.projectName.get(), self.run3DFlexDataPrepJob.get())
-
     def doRun3DFlexMeshPrepare(self):
         self._className = 'flex_meshprep'
         params = {}
-        varDataPrepJob = str(self.run3DFlexDataPrepJob.get())
+        varDataPrepJob = str(self.dataPrepare.get().run3DFlexDataPrepJob)
         input_group_connect = {"volume": str('%s.volume' % varDataPrepJob)}
 
         if self.refMask.get() is not None:
             input_group_connect["mask"] = str(self.mask)
         else:
             for paramName in self._maskMeshPrepareName:
                 if self.getAttributeValue(paramName) is not None:
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+from pwem.objects import Volume
 from pyworkflow import BETA
 from pyworkflow.protocol.params import (PointerParam,  IntParam,  BooleanParam)
 from . import ProtCryosparcBase
 from ..convert import *
 from ..utils import *
 from ..constants import *
 
@@ -38,15 +39,15 @@
     particles and performs high-resolution refinement using L-BFGS under
     the 3DFlex model. This is the stage at which improvements to density
     in high-res regions are computed. Outputs two half-maps that can be used
     for FSC validation, sharpening, and other downstream tasks.
     """
     _label = '3D flex reconstruction'
     _devStatus = BETA
-    _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
+    _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineFileNames(self):
         """ Centralize how files are called within the protocol. """
         myDict = {
             'input_particles': self._getTmpPath('input_particles.star'),
             'out_particles': self._getPath() + '/output_particle.star',
@@ -108,15 +109,61 @@
         self._insertFunctionStep(self.createOutputStep)
 
     def reconstructionStep(self):
         self.info(pwutils.yellowStr("3D Flex Reconstruction started..."))
         self.doRun3DFlexReconstruction()
 
     def createOutputStep(self):
-        pass
+        """
+         Create the protocol output.  """
+        self._initializeUtilsVariables()
+        csOutputFolder = os.path.join(self.projectDir.get(),
+                                      self.run3DFlexReconstructionJob.get())
+        csOutputPattern = "%s%s" % (getOutputPreffix(self.projectName.get()),
+                                    self.run3DFlexReconstructionJob.get())
+
+        # Flex volume
+        fnFlexVolName = csOutputPattern + "_flex_map.mrc"
+        flexHalf1Name = csOutputPattern + "_flex_map_half_A.mrc"
+        flexHalf2Name = csOutputPattern + "_flex_map_half_B.mrc"
+
+        # No Flex volume
+        fnNoFlexVolName = csOutputPattern + "_noflex_map.mrc"
+        flexNoHalf1Name = csOutputPattern + "_noflex_map_half_A.mrc"
+        flexNoHalf2Name = csOutputPattern + "_noflex_map_half_B.mrc"
+
+        # Copy the CS output volume and half to extra folder
+        copyFiles(csOutputFolder, self._getExtraPath(), files=[fnFlexVolName, flexHalf1Name, flexHalf2Name,
+                                                               fnNoFlexVolName, flexNoHalf1Name, flexNoHalf2Name])
+
+        fnVol = os.path.join(self._getExtraPath(), fnFlexVolName)
+        half1 = os.path.join(self._getExtraPath(), flexHalf1Name)
+        half2 = os.path.join(self._getExtraPath(), flexHalf2Name)
+
+        flexVol = Volume()
+        fixVolume([fnVol, half1, half2])
+        flexVol.setFileName(fnVol)
+        ccp4header = Ccp4Header(fnVol, readHeader=True)
+        flexVol.setSamplingRate(ccp4header.getSampling()[0])
+        flexVol.setHalfMaps([half1, half2])
+
+        fnVol = os.path.join(self._getExtraPath(), fnNoFlexVolName)
+        half1 = os.path.join(self._getExtraPath(), flexNoHalf1Name)
+        half2 = os.path.join(self._getExtraPath(), flexNoHalf2Name)
+
+        noFlexVol = Volume()
+        fixVolume([fnVol, half1, half2])
+        noFlexVol.setFileName(fnVol)
+        ccp4header = Ccp4Header(fnVol, readHeader=True)
+        noFlexVol.setSamplingRate(ccp4header.getSampling()[0])
+        noFlexVol.setHalfMaps([half1, half2])
+
+        self._defineOutputs(flexVolume=flexVol)
+        self._defineOutputs(noFlexVolume=noFlexVol)
+
 
     def _defineParamsName(self):
         """ Define a list with 3D Flex Reconstruction parameters names"""
         self._paramsName = ['flex_do_noflex_recon', 'flex_bfgs_num_iters',
                             'refine_gs_resplit']
         self.lane = str(self.getAttributeValue('compute_lane'))
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     Uses a mesh and prepared particles (at a downsampled resolution) to train
     a 3DFlex model. Parameters control the number of latent dimensions,
     size of the model, and training hyperparameters. This job outputs
     checkpoints during training.
     """
     _label = '3D flex training'
     _devStatus = BETA
-    _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
+    _protCompatibility = [V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineFileNames(self):
         """ Centralize how files are called within the protocol. """
         myDict = {
             'input_particles': self._getTmpPath('input_particles.star'),
             'out_particles': self._getPath() + '/output_particle.star',
@@ -60,14 +60,20 @@
         form.addSection(label='Input')
         form.addParam('input3DFlexDataPrepareProt', PointerParam,
                       pointerClass='ProtCryoSparc3DFlexDataPrepare',
                       label="3D flex data prepare protocol",
                       important=True,
                       help='Particle stacks to use.')
 
+        form.addParam('input3DMeshFlexPrepareProt', PointerParam,
+                      pointerClass='ProtCryoSparc3DFlexMeshPrepare',
+                      label="3D flex mesh prepare protocol",
+                      important=True,
+                      help='3d Flex mesh.')
+
         form.addParam('flex_K', IntParam, default=2,
                       label="Number of latent dims",
                       help="Number of latent dimensions in the flex refine "
                            "model. See guide for more details. Typically, "
                            "start with 2 and increase if the data appears to "
                            "have more modes of motion present.")
 
@@ -192,16 +198,17 @@
 
         try:
             gpusToUse = self.getGpuList()
         except Exception:
             gpusToUse = False
 
         protocolPrepare = self.input3DFlexDataPrepareProt.get()
+        protocolMesh = self.input3DMeshFlexPrepareProt.get()
         varDataPrepJobParticles = str(protocolPrepare.run3DFlexDataPrepJob)
-        varDataMeshJob = str(protocolPrepare.run3DFlexMeshPrepJob)
+        varDataMeshJob = str(protocolMesh.run3DFlexMeshPrepJob)
         input_group_connect = {"particles": "%s.particles" % varDataPrepJobParticles,
                                "flex_mesh": "%s.flex_mesh" % varDataMeshJob}
         params = {}
 
         for paramName in self._paramsName:
             if self.getAttributeValue(paramName) is not None:
                 params[str(paramName)] = str(self.getAttributeValue(paramName))
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3d_variability.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_3d_variability.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_blob_picker.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,311 +20,305 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-import os.path
-import zipfile
+import os
+import emtable
 
-from pyworkflow import BETA
+from pwem.objects import Coordinate, CTFModel
+import pyworkflow.utils as pwutils
+from pyworkflow import NEW
 from pyworkflow.protocol.params import (PointerParam, FloatParam,
-                                        LEVEL_ADVANCED, EnumParam, IntParam,
-                                        Positive, BooleanParam)
-from pwem.protocols import ProtRefine3D
+                                        BooleanParam, IntParam,
+                                        String)
 
-from . import ProtCryosparcBase
-from ..convert import *
-from ..utils import *
-from ..constants import *
+from .protocol_base import ProtCryosparcBase
+from .. import RELIONCOLUMNS
+from ..convert import convertCs2Star
+from ..utils import (addComputeSectionParams, cryosparcValidate,  enqueueJob, waitForCryosparc, clearIntermediateResults,
+                     copyFiles)
 
 
-class ProtCryoSparc3DVariabilityAnalisys(ProtCryosparcBase, ProtRefine3D):
+class ProtCryoSparcBlobPicker(ProtCryosparcBase):
     """
-    Protocol to create various versions of a 3D variability result that can be
-    used for display
+    Automatically picks particles by searching for Gaussian signals.
     """
-    _label = '3D variability Display'
-    _devStatus = BETA
-
-    def _defineFileNames(self):
-        """ Centralize how files are called. """
-        myDict = {
-            'out_particles': self._getExtraPath('output_particle.star'),
-            'stream_log': self._getPath() + '/stream.log',
-            'out_class': self._getExtraPath() + '/output_class.star'
-        }
-        self._updateFilenamesDict(myDict)
+    _label = 'blob_picker'
+    _className = "blob_picker_gpu"
+    _devStatus = NEW
 
     def _defineParams(self, form):
         form.addSection(label='Input')
-        form.addParam('input3DVariablityAnalisysProt', PointerParam,
-                      label="3D variability analysis protocol",
-                      pointerClass='ProtCryoSparc3DVariability',
-                      help='Particle stacks to use.')
-        form.addParallelSection(threads=1, mpi=1)
-
-        # --------------[3D Variability Display]---------------------------
-        form.addSection(label='3D Variability Output')
-
-        form.addParam('var_output_mode', EnumParam,
-                      choices=['cluster', 'simple', 'intermediates'],
-                      default=0,
-                      label="Output mode",
-                      help='simple mode: output a simple linear "movie" of '
-                           'volumes along each dimension. Number of frames is '
-                           'the next param. '
-                           'cluster mode: fit clusters to reaction coordinates '
-                           'and output volumes and particles from each cluster. '
-                           'Number of clusters is the next param. '
-                           'intermediates mode: - reconstruct multiple '
-                           'intermediate volumes along each variability '
-                           'dimension, useful for better visualizing '
-                           'non-linear changes. Number of intermediate frames '
-                           'is the next param.')
-        form.addParam('var_num_frames', IntParam, default=20,
-                      validators=[Positive],
-                      label="Number of frames/clusters",
-                      help='Number of clusters for cluster mode, or number of '
-                           'frames for simple and intermediates mode.')
-
-        form.addParam('var_range_percentile', FloatParam, default=3,
-                      validators=[Positive],
-                      label="Min/Max Range Percentile (%)",
-                      help='Percentile for computing the min and max for '
-                           'each component.')
+        form.addParam('inputMicrographs', PointerParam, important=True,
+                      label=pwutils.Message.LABEL_INPUT_MIC,
+                      pointerClass='SetOfMicrographs')
+
+        form.addParam('diameter', IntParam, default=None,
+                      label='Minimum particle diameter (px)',
+                      help='Minimum particle diameter (px)')
+
+        form.addParam('diameter_max', IntParam, default=None,
+                      label='Maximum particle diameter (px)',
+                      help='Maximum particle diameter (px)')
+
+        form.addParam('use_circle', BooleanParam, default=True,
+                      label='Use circular blob',
+                      help='Use three circular blobs, at minimum, average, and maximum particle diameters based on parameters above.')
+
+        form.addParam('use_ellipse', BooleanParam, default=False,
+                      label='Use elliptical blob',
+                      help='Use an elliptical blob with minor diameter equal to minimum particle diamater param above, and major diameter equal to maximum particle diameter above. You may want to turn off circular blob with this on.')
+
+        form.addParam('use_ring', BooleanParam, default=False,
+                      label='Use ring blob',
+                      help='Use a ring-shaped blob with inner diameter equal to minimum particle diameter param above, and outer diameter equal to maximum particle diameter above. You may want to turn off circular and elliptical blob with this on.')
+
+        form.addParam('estimate_ctf', BooleanParam, default=False,
+                      label='Estimate CTF before pick?',
+                      help='Estimate CTF using cryoSPARC Patch CTF algorithm')
+
+        # form.addParam('lowpass_res_template', IntParam, default=20,
+        #               label='Lowpass filter to apply to templates (A)',
+        #               help='Lowpass filter to apply to templates, (A)s')
+        #
+        # form.addParam('lowpass_res', IntParam, default=20,
+        #               label='Lowpass filter to apply to micrographs (A)',
+        #               help='Lowpass filter to apply to micrographs, (A)s')
+        #
+        # form.addParam('angular_spacing_deg', IntParam, default=5,
+        #               label='Angular sampling (degrees)',
+        #               help='Angular sampling of templates in degrees. Lower value will mean finer rotations.')
+
+        form.addParam('min_distance', FloatParam, default=1.0,
+                      label='Min. separation dist (diameters)',
+                      help='Minimum distance between particles in units of particle diameter (min diameter for blob picker). The lower this value, the more and closer particles it picks.')
 
-        form.addParam('var_N', IntParam, default=None,
+        form.addParam('num_process', IntParam, default=None,
                       allowsNull=True,
-                      expertLevel=LEVEL_ADVANCED,
-                      label="Downsample to box size",
-                      help='Downsample the output volumes to this size.')
+                      label='Number of mics to process',
+                      help='Number of micrographs to process. None means all.')
 
-        form.addParam('var_M', IntParam, default=None,
-                      expertLevel=LEVEL_ADVANCED,
-                      allowsNull=True,
-                      label="Crop to size (after downsample)",
-                      help='Crop the output volumes to this size after '
-                           'downsampling.')
-
-        # form.addParam('var_num_particles', IntParam, default=None,
-        #               validators=[Positive],
-        #               label="Only use this many particles",
-        #               help='Only use this many particles for reconstructions.')
+        form.addParam('max_num_hits', IntParam, default=4000,
+                      label='Maximum number of local maxima to consider',
+                      help='Maximum number of local maxima (peaks) considered.')
 
-        form.addParam('var_filter_res', FloatParam, default=None,
-                      allowsNull=True,
-                      expertLevel=LEVEL_ADVANCED,
-                      label="Filter resolution (A)",
-                      help='Resolution at which results are filtered')
-
-        form.addParam('var_filter_order', FloatParam, default=1.5,
-                      validators=[Positive],
-                      label="Filter order",
-                      help='Order of filter')
+        """
+            job.param_add('template', "num_plot",             base_value=10,          title="Number of mics to plot",                                               param_type="number",    hidden=False,   advanced=False, desc='Number of micrographs to plot.')
+            job.param_add('template', "recenter_templates",       base_value=True,        title="Recenter templates",                                                param_type="boolean",    hidden=False,   advanced=True, desc='Whether or not to recenter the input templates.')
+        """
 
-        form.addParam('var_highpass_res', FloatParam, default=None,
-                      allowsNull=True,
-                      expertLevel=LEVEL_ADVANCED,
-                      label="Highpass resolution (A)",
-                      help='Resolution at which results are filtered')
-
-        form.addParam('var_highpass_order', FloatParam, default=8,
-                      validators=[Positive],
-                      expertLevel=LEVEL_ADVANCED,
-                      label="Highpass order",
-                      help='Order of filter')
-
-        form.addParam('var_vol_flip', BooleanParam, default=False,
-                      expertLevel=LEVEL_ADVANCED,
-                      label="Flip hand of outputs",
-                      help='Flip the hand out output volumes (including series). '
-                           'Note that this does not flip output '
-                           'alignments - only the output volumes.')
-
-        form.addParam('var_skip_reconstruction', BooleanParam, default=False,
-                      expertLevel=LEVEL_ADVANCED,
-                      label="Skip reconstruction",
-                      help='Skip reconstructions in cluster and '
-                           'intermediate mode - helpful to quickly inspect '
-                           'whether a clustering or division of particles will'
-                           ' be helpful.')
-
-        form.addParam('var_cluster_3D_plots', BooleanParam, default=True,
-                      expertLevel=LEVEL_ADVANCED,
-                      label="Cluster mode: 3D plots",
-                      help='Make 3D instead of 2D plots to show clusters.')
-
-        form.addParam('var_intermediate_width', IntParam, default=2,
-                      validators=[Positive],
-                      expertLevel=LEVEL_ADVANCED,
-                      label="Intermediates: window (frames)",
-                      help='Intermediates: window (frames)')
+        # --------------[Compute settings]---------------------------
         form.addSection(label="Compute settings")
         addComputeSectionParams(form, allowMultipleGPUs=False)
 
     # --------------------------- INSERT steps functions -----------------------
+
     def _insertAllSteps(self):
-        self._defineFileNames()
         self._defineParamsName()
         self._initializeCryosparcProject()
+        self._insertFunctionStep(self.convertInputStep)
         self._insertFunctionStep(self.processStep)
-        self._insertFunctionStep(self.generateStartFiles)
         self._insertFunctionStep(self.createOutputStep)
 
     # --------------------------- STEPS functions ------------------------------
+
     def processStep(self):
-        self.info(pwutils.yellowStr("3D Variability started..."))
-        self.doRun3DVariabilityDisplay()
+        if self.estimate_ctf.get():
+            self.info(pwutils.yellowStr("Patch CTF estimate started..."))
+            self.doPatchCTFEstimate()
+            self.micrographs = String(str(self.runPatchCTF.get()) + '.exposures')
+
+        self.info(pwutils.yellowStr("Blob picker started..."))
+        self.doBlobPicker()
+
+    def createOutputStep(self):
+        """
+        Create the protocol output. Convert cryosparc file to star file
+        """
+        self.info(pwutils.yellowStr("Create output started..."))
+        self._initializeUtilsVariables()
+        micSetPtr = self._getInputMicrographs()
+
+        micList = {os.path.basename(mic.getFileName()): mic.clone() for mic in micSetPtr}
 
-    def generateStartFiles(self):
-        self.info(pwutils.yellowStr("Copying files from CS to Scipion folder..."))
         csOutputFolder = os.path.join(self.projectDir.get(),
-                                      self.run3DVariabilityDisplay.get())
-        import time
-        time.sleep(10)
-        if self.var_output_mode.get() == 0:  # Cluster mode
-
-            # Copy the CS output to extra folder
-            outputFolder = os.path.join(self._getExtraPath(), 'outputs')
-            pwutils.cleanPath(outputFolder)
-            copyFiles(csOutputFolder, outputFolder)
-
-            # Creating the folder where .star files will be create
-            starFilesPath = os.path.join(outputFolder, 'clustersFiles')
-            os.makedirs(starFilesPath)
-
-            # Generating the .star file por all clusters
-            allClusterSeries = '%s%s_series_all_clusters.cs' % (getOutputPreffix(self.projectName.get()),
-                                                             self.run3DVariabilityDisplay.get())
-            allClusterSeriesStar = '%s%s_series_all_clusters.star' % (getOutputPreffix(self.projectName.get()),
-                                                             self.run3DVariabilityDisplay.get())
-
-            filePath = os.path.join(outputFolder, allClusterSeries)
-            outputStarFn = os.path.join(starFilesPath, allClusterSeriesStar)
-            argsList = [filePath, outputStarFn]
+                                      self.runBlobPicker.get())
+        # Copy the CS output coordinates to extra folder
+        outputPath = os.path.join(self._getExtraPath(), self.runBlobPicker.get())
+        copyFiles(csOutputFolder, outputPath)
+        csPickedParticlesName = 'picked_particles.cs'
+
+        csFile = os.path.join(outputPath, csPickedParticlesName)
+        outputStarFn = self._getExtraPath('output_coordinates.star')
+        argsList = [csFile, outputStarFn]
+        convertCs2Star(argsList)
+
+        outputCoords = self._fillSetOfCoordinates(micSetPtr, outputStarFn, micList)
+
+        # Copy the  CTF output to extra folder
+        if self.estimate_ctf.get():
+            csOutputFolder = os.path.join(self.projectDir.get(),
+                                          self.runPatchCTF.get())
+            outputPath = os.path.join(self._getExtraPath(), self.runPatchCTF.get())
+            copyFiles(csOutputFolder, outputPath)
+
+            ctfEstimatedFileName = 'exposures_ctf_estimated.cs'
+            csFile = os.path.join(outputPath, ctfEstimatedFileName)
+            outputStarFn = self._getExtraPath('ctf.star')
+            argsList = [csFile, outputStarFn]
             convertCs2Star(argsList)
 
-            # Creating the .star cluster per cluster
-            numOfClusters = self.var_num_frames.get()
-            self.info(pwutils.yellowStr("Generating .star files for all clusters"))
-            for i in range(numOfClusters):
-                self.info(pwutils.yellowStr("Processing cluster %d ..." % i))
-
-                clusterParticlesPattern = '%s%s_cluster_%03d_particles.cs' % (getOutputPreffix(self.projectName.get()),
-                                                                              self.run3DVariabilityDisplay.get(), i)
-
-                passthroughParticlesPattern = '%s%s_passthrough_particles_cluster_%d.cs' % (getOutputPreffix(self.projectName.get()),
-                                                                                            self.run3DVariabilityDisplay.get(), i)
-                patterns = [clusterParticlesPattern, passthroughParticlesPattern]
-                outputs = ['output_cluster_particle%03d.star' % i,
-                           'output_passthrough_particle%03d.star' % i]
-                # Generating .star files
-                for j in range(len(patterns)):
-                    filePath = os.path.join(outputFolder, patterns[j])
-                    outputStarFn = os.path.join(starFilesPath, outputs[j])
-                    argsList = [filePath, outputStarFn]
-                    convertCs2Star(argsList)
-        else:
-            # Copy the CS output to extra folder
-            outputFolder = self._getExtraPath()
-            pwutils.cleanPath(outputFolder)
-            copyFiles(csOutputFolder, outputFolder)
-            # Creating the .star cluster particles
-            numOfComponets = int(self.input3DVariablityAnalisysProt.get().var_K)
-
-            for i in range(numOfComponets):
-                self.info(pwutils.yellowStr("Extracting component %d ..."))
-                # Creating the folder where clusters will be unzip
-                componetFilesPath = self._getExtraPath('component%03d' % i)
-                os.makedirs(componetFilesPath)
-                componentPattern = "%s%s_component_%03d.zip" % (
-                    getOutputPreffix(self.projectName.get()),
-                    self.run3DVariabilityDisplay.get(),
-                    i)
-                cmd = "unzip %s -d %s" % (
-                self._getExtraPath(componentPattern),
-                componetFilesPath)
-                os.system(cmd)
+            outputCtfSet = self._fillSetOfCTF(outputStarFn, micList)
 
-    def createOutputStep(self):
-        self._initializeUtilsVariables()
-        self.info(pwutils.yellowStr("Creating the output..."))
+            self._defineOutputs(outputCTF=outputCtfSet)
+            self._defineSourceRelation(micSetPtr, outputCtfSet)
 
-        pass
+        self._defineOutputs(outputCoordinates=outputCoords)
+        self._defineSourceRelation(micSetPtr, outputCoords)
 
-    # --------------------------- UTILS functions ------------------------------
+    def _fillSetOfCoordinates(self, micSetPtr, outputStarFn, micList):
+
+        outputCoords = self._createSetOfCoordinates(micSetPtr)
+        boxSixe = (self.diameter.get() + self.diameter_max.get()) / 2
+        outputCoords.setBoxSize(int(boxSixe))
+
+        coord = Coordinate()
+        mdFileName = '%s@%s' % ('particles', outputStarFn)
+        table = emtable.Table(fileName=outputStarFn)
+
+        for row in table.iterRows(mdFileName):
+            coord.setObjId(None)
+            micName = os.path.basename(row.get(RELIONCOLUMNS.rlnMicrographName.value))
+            splitMicName = micName.split('_')
+            if len(splitMicName) > 1:
+                micName = '_'.join(splitMicName[1:])
+            else:
+                micName = splitMicName[-1]
+            coord.setMicrograph(micList[micName])
+            x = row.get(RELIONCOLUMNS.rlnCoordinateX.value)
+            y = row.get(RELIONCOLUMNS.rlnCoordinateY.value)
+            dim = micList[micName].getDimensions()
+            flipY = dim[1] - y
+            coord.setPosition(x, flipY)
+            # Add it to the set
+            outputCoords.append(coord)
+
+        return outputCoords
+
+    def _fillSetOfCTF(self, outputCTFFn, micList):
+
+        inputMics = self._getInputMicrographs()
+        outputCtfSet = self._createSetOfCTF()
+        outputCtfSet.setMicrographs(inputMics)
+        mics = list(micList.values())
+
+        ctf = CTFModel()
+        mdFileName = '%s@%s' % ('micrograph', outputCTFFn)
+        table = emtable.Table(fileName=outputCTFFn)
+
+        for mic, row in enumerate(table.iterRows(mdFileName)):
+            ctf.setDefocusU(row.get(RELIONCOLUMNS.rlnDefocusU.value))
+            ctf.setDefocusV(row.get(RELIONCOLUMNS.rlnDefocusV.value))
+            ctf.setPhaseShift(row.get(RELIONCOLUMNS.rlnPhaseShift.value))
+            ctf.setResolution(row.get(RELIONCOLUMNS.rlnCtfMaxResolution.value))
+            ctf.setDefocusAngle(row.get(RELIONCOLUMNS.rlnDefocusAngle.value))
+            ctf.setMicrograph(mics[mic])
+            outputCtfSet.append(ctf)
+
+        return outputCtfSet
 
     def _defineParamsName(self):
         """ Define a list with all protocol parameters names"""
-        self._paramsName = ['var_output_mode',
-                            'var_num_frames',
-                            'var_range_percentile',
-                            'var_N',
-                            'var_M',
-                            'var_filter_res',
-                            'var_filter_order',
-                            'var_highpass_res',
-                            'var_highpass_order',
-                            'var_vol_flip',
-                            'var_skip_reconstruction',
-                            'var_cluster_3D_plots',
-                            'var_intermediate_width']
+        self._paramsName = ['diameter', 'diameter_max', 'use_circle',
+                            'use_ellipse', 'use_ring', 'min_distance',
+                            'num_process', 'max_num_hits']
+
         self.lane = str(self.getAttributeValue('compute_lane'))
 
+    # --------------------------- INFO functions -------------------------------
     def _validate(self):
+        """ Should be overwritten in subclasses to
+            return summary message for NORMAL EXECUTION.
+        """
         validateMsgs = cryosparcValidate()
-        if not validateMsgs:
-            validateMsgs = gpusValidate(self.getGpuList(), checkSingleGPU=True)
+
+        # if not validateMsgs:
+        #     micrographs = self._getInputMicrographs()
+        #     if micrographs is not None and not micrographs.hasCTF():
+        #         validateMsgs.append("The micrographs has not associated a CTF model")
+
         return validateMsgs
 
-    def doRun3DVariabilityDisplay(self):
-        """
-        :return:
-        """
-        className = "var_3D_disp"
-        varAnalysisJob = str(self.input3DVariablityAnalisysProt.get().run3DVariability)
-        input_group_conect = {"particles": str('%s.particles' %varAnalysisJob) ,
-                              "volume": str('%s.volume'%varAnalysisJob)}
-        params = {}
+    def _summary(self):
+        summary = []
+        return summary
+
+    def doPatchCTFEstimate(self):
+        input_group_connect = {"exposures": self.micrographs.get()}
+        params = {'classic_mode': 'False'}
+        className = 'patch_ctf_estimation_multi'
+        try:
+            gpusToUse = self.getGpuList()
+        except Exception:
+            gpusToUse = False
+
+        runPatchCTFJob = enqueueJob(className,
+                                      self.projectName.get(),
+                                      self.workSpaceName.get(),
+                                      str(params).replace('\'', '"'),
+                                      str(input_group_connect).replace('\'', '"'),
+                                      self.lane, gpusToUse)
 
+        self.runPatchCTF = String(runPatchCTFJob.get())
+        self.currenJob.set(runPatchCTFJob.get())
+        self._store(self)
+
+        waitForCryosparc(self.projectName.get(),
+                         self.runPatchCTF.get(),
+                         "An error occurred in the ctf estimation process. "
+                         "Please, go to cryoSPARC software for more "
+                         "details.")
+
+    def doBlobPicker(self):
+
+        input_group_connect = {"micrographs": self.micrographs.get()}
+        params = {}
+        micSetPtr = self._getInputMicrographs()
+        samplingRate = micSetPtr.getSamplingRate()
         for paramName in self._paramsName:
-            if (paramName != 'var_output_mode' and paramName != 'var_N' and
-                    paramName != 'var_M' and paramName != 'var_filter_res' and
-                    paramName != 'var_highpass_res'):
+            if (paramName != 'diameter' and paramName != 'diameter_max' and
+                    paramName != 'num_process'):
                 params[str(paramName)] = str(self.getAttributeValue(paramName))
-            elif paramName == 'var_output_mode':
-                params[str(paramName)] = str(VAR_OUTPUT_MODE[self.var_output_mode.get()])
-            elif paramName == 'var_N' and self.var_N.get() is not None:
-                params[str(paramName)] = str(self.var_N.get())
-            elif paramName == 'var_M' and self.var_M.get() is not None:
-                params[str(paramName)] = str(self.var_M.get())
-            elif paramName == 'var_filter_res' and self.var_filter_res.get() is not None:
-                params[str(paramName)] = str(self.var_filter_res.get())
-            elif paramName == 'var_highpass_res' and self.var_highpass_res.get() is not None:
-                params[str(paramName)] = str(self.var_highpass_res.get())
+            elif paramName == 'diameter' and self.diameter.get() is not None:
+                params[str(paramName)] = str(int(self.diameter.get()*samplingRate))
+            elif paramName == 'diameter_max' and self.diameter_max.get() is not None:
+                params[str(paramName)] = str(int(self.diameter_max.get()*samplingRate))
+            elif paramName == 'num_process' and self.num_process.get() is not None:
+                params[str(paramName)] = str(self.num_process.get())
 
-        # Determinate the GPUs to use (in dependence of the cryosparc version)
+        # Determinate the GPUs to use (in dependence of
+        # the cryosparc version)
         try:
             gpusToUse = self.getGpuList()
         except Exception:
             gpusToUse = False
 
-        self.run3DVariabilityDisplay = enqueueJob(className,
-                                                  self.projectName.get(),
-                                                  self.workSpaceName.get(),
-                                                  str(params).replace('\'',
-                                                                      '"'),
-                                                  str(input_group_conect).replace(
-                                                      '\'',
-                                                      '"'),
-                                                  self.lane, gpusToUse)
+        runBlobPickerJob = enqueueJob(self._className,
+                                         self.projectName.get(),
+                                         self.workSpaceName.get(),
+                                         str(params).replace('\'', '"'),
+                                         str(input_group_connect).replace('\'', '"'),
+                                         self.lane, gpusToUse)
 
-        self.currenJob.set(self.run3DVariabilityDisplay.get())
+        self.runBlobPicker = String(runBlobPickerJob.get())
+        self.currenJob.set(runBlobPickerJob.get())
         self._store(self)
 
         waitForCryosparc(self.projectName.get(),
-                         self.run3DVariabilityDisplay.get(),
-                         "An error occurred in the 3D Variability process. "
-                         "Please, go to cryosPARC software for more "
+                         self.runBlobPicker.get(),
+                         "An error occurred in the particles picking process. "
+                         "Please, go to cryoSPARC software for more "
                          "details.")
+        clearIntermediateResults(self.projectName.get(), self.runBlobPicker.get())
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_ab.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_ab.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     Wrapper protocol for the Cryosparc's per-particle Global CTF refinement.
     Performs per-exposure-group CTF parameter refinement of higher-order
     aberrations, against a given 3D reference
     """
     _label = 'global ctf refinement'
     _className = "ctf_refine_global"
     _protCompatibility = [V3_3_1, V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3, V4_1_0,
-                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
+                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
     newParamsName = []
 
     def _initialize(self):
         self._createFilenameTemplates()
 
     def _createFilenameTemplates(self):
         """ Centralize how files are called. """
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_helical_refinement.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,18 +48,17 @@
     uses an algorithm that is conceptually similar to Egelman's Iterative
     Helical Real Space Reconstruction (IHRSR) algorithm, while incorporating
     the same maximum likelihood framework, accelerated branch-and-bound
     alignment algorithm, and optional Non-Uniform regularization as used in
     other cryoSPARC refinement jobs.
     """
     _label = '3D helical refinement'
-    _devStatus = BETA
     _fscColumns = 4
     _protCompatibility = [V3_3_1, V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3,
-                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
+                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
     _className = "helix_refine"
 
     def _defineParams(self, form):
         form.addSection(label='Input')
         form.addParam('inputParticles', PointerParam,
                       pointerClass='SetOfParticles',
                       label="Input particles", important=True,
@@ -238,34 +237,28 @@
         self.info(pwutils.yellowStr("Refinement started..."))
         self.doRunRefine()
 
     # --------------------------- INFO functions -------------------------------
     def _validate(self):
         validateMsgs = cryosparcValidate()
         if not validateMsgs:
-            csVersion = getCryosparcVersion()
-            if [version for version in self._protCompatibility
-                if parse_version(version) >= parse_version(csVersion)]:
-                validateMsgs = gpusValidate(self.getGpuList(), checkSingleGPU=True)
-                if not validateMsgs:
-                    if self.referenceVolume.get() is None and not self.use_cylindrical_model.get():
-                        validateMsgs.append("Cannot generate initial model "
-                                            "without in-plane rotation "
-                                            "information. Please input an "
-                                            "initial model from a previous ab-initio or "
-                                            "refinement protocol, or activate the "
-                                            "'Generate a cylindrical initial "
-                                            "model?' parameter")
-
-                    if self.use_cylindrical_model.get() and self.filament_outer_diameter.get() is None:
-                        validateMsgs.append("Must set the filament outer diameter to use a cylindrical model")
-
-            else:
-                validateMsgs.append("The protocol is not compatible with the "
-                                    "cryoSPARC version %s" % csVersion)
+            validateMsgs = gpusValidate(self.getGpuList(), checkSingleGPU=True)
+            if not validateMsgs:
+                if self.referenceVolume.get() is None and not self.use_cylindrical_model.get():
+                    validateMsgs.append("Cannot generate initial model "
+                                        "without in-plane rotation "
+                                        "information. Please input an "
+                                        "initial model from a previous ab-initio or "
+                                        "refinement protocol, or activate the "
+                                        "'Generate a cylindrical initial "
+                                        "model?' parameter")
+
+                if self.use_cylindrical_model.get() and self.filament_outer_diameter.get() is None:
+                    validateMsgs.append("Must set the filament outer diameter to use a cylindrical model")
+
         return validateMsgs
 
     def _defineParamsName(self):
         """ Define a list with all protocol parameters names"""
         self._paramsName = ['refine_init_twist',
                             'refine_init_shift',
                             'refine_hsym_order',
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     """
     _label = 'homogeneous reconstruction'
     _className = "homo_reconstruct"
     _devStatus = NEW
     _fscColumns = 6
     _protCompatibility = [V3_3_0, V3_3_1, V3_3_2, V4_0_0, V4_0_1, V4_0_2,
                           V4_0_3, V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1,
-                          V4_3_1, V4_4_0]
+                          V4_3_1, V4_4_0, V4_4_1]
     ewsParamsName = []
 
     def _initialize(self):
         self._defineFileNames()
 
     def _defineFileNames(self):
         """ Centralize how files are called. """
@@ -350,30 +350,23 @@
     # --------------------------- INFO functions -------------------------------
     def _validate(self):
         """ Should be overwritten in subclasses to
                return summary message for NORMAL EXECUTION.
                """
         validateMsgs = cryosparcValidate()
         if not validateMsgs:
-            csVersion = getCryosparcVersion()
-            if [version for version in self._protCompatibility
-                if parse_version(version) >= parse_version(csVersion)]:
-                validateMsgs = gpusValidate(self.getGpuList(),
-                                            checkSingleGPU=True)
-                if not validateMsgs:
-                    particles = self._getInputParticles()
-                    if not particles.hasCTF():
-                        validateMsgs.append("The Particles has not associated a "
-                                            "CTF model")
-                        if not validateMsgs and not particles.hasAlignment3D():
-                            validateMsgs.append("The Particles has not a 3D "
-                                                "alignment")
-            else:
-                validateMsgs.append("The protocol is not compatible with the "
-                                    "cryoSPARC version %s" % csVersion)
+            validateMsgs = gpusValidate(self.getGpuList(), checkSingleGPU=True)
+            if not validateMsgs:
+                particles = self._getInputParticles()
+                if not particles.hasCTF():
+                    validateMsgs.append("The Particles has not associated a "
+                                        "CTF model")
+                    if not validateMsgs and not particles.hasAlignment3D():
+                        validateMsgs.append("The Particles has not a 3D "
+                                            "alignment")
 
         return validateMsgs
 
     def _summary(self):
         summary = []
         if (not hasattr(self, 'outputVolume') or
                 not hasattr(self, 'outputParticles')):
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         the fly.
     """
     _label = '3D homogeneous refinement'
     _fscColumns = 6
     _className = "homo_refine_new"
     ewsParamsName = []
     _protCompatibility = [V3_3_1, V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3, V4_1_0,
-                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
+                          V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineFileNames(self):
         """ Centralize how files are called within the protocol. """
         myDict = {
             'input_particles': self._getTmpPath('input_particles.star'),
             'out_particles': self._getPath() + '/output_particle.star',
@@ -504,27 +504,21 @@
         self._defineOutputs(outputParticles=outImgSet)
         self._defineTransformRelation(self.inputParticles.get(), outImgSet)
         self.createFSC(idd, imgSet, vol)
 
     def _validate(self):
         validateMsgs = cryosparcValidate()
         if not validateMsgs:
-            csVersion = getCryosparcVersion()
-            if [version for version in self._protCompatibility
-                if parse_version(version) >= parse_version(csVersion)]:
-                validateMsgs = gpusValidate(self.getGpuList())
-                if not validateMsgs:
-                    particles = self._getInputParticles()
-                    if not particles.hasCTF():
-                        validateMsgs.append(
-                            "The Particles has not associated a "
-                            "CTF model")
-            else:
-                validateMsgs.append("The protocol is not compatible with the "
-                                    "cryoSPARC version %s" % csVersion)
+            validateMsgs = gpusValidate(self.getGpuList())
+            if not validateMsgs:
+                particles = self._getInputParticles()
+                if not particles.hasCTF():
+                    validateMsgs.append(
+                        "The Particles has not associated a "
+                        "CTF model")
         return validateMsgs
 
     def _summary(self):
         summary = []
         if (not hasattr(self, 'outputVolume') or
                 not hasattr(self, 'outputParticles')):
             summary.append("Output objects not ready yet.")
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,17 +56,16 @@
     heterogeneity in single particle cryo-EM datasets. This job currently
     implements a version of 3D classification without alignment — a
     classification routine that can complement the existing Heterogeneous
     Refinement job in finding new discrete classes of data.
     """
     _label = '3D Classification'
     _className = "class_3D"
-    _devStatus = BETA
     _protCompatibility = [V3_3_1, V3_3_2, V4_0_0, V4_0_1, V4_0_2, V4_0_3,
-                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
+                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
 
     def _initialize(self):
         self._defineFileNames()
 
     def _defineFileNames(self):
         """ Centralize how files are called. """
         myDict = {
@@ -92,14 +91,19 @@
         form.addParam('refMask', PointerParam, pointerClass='VolumeMask',
                       label='Static mask',
                       allowsNull=True,
                       help="Mask for focussed classification. If none supplied,"
                            " a mask will be created from initial structures "
                            "(bootstrapped or input).")
 
+        form.addParam('refFocusMask', PointerParam, pointerClass='VolumeMask',
+                      label='Focus mask',
+                      allowsNull=True,
+                      help="Optional mask for focussed classification. If not supplied, only the solvent mask will be "
+                           "used.")
         # --------------[3D Classification]---------------------------
         form.addSection(label='3D Classification (without alignment)')
 
         form.addParam('class3D_N_K', IntParam, default=2,
                       label="Number of classes",
                       validators=[Positive],
                       help='Number of classes. This value must be grater than 2')
@@ -163,15 +167,15 @@
         form.addParam('class3D_PCA_num_reconstructions', IntParam, default=100,
                       label="PCA: number of reconstructions",
                       condition="class3D_init_mode==1",
                       validators=[Positive],
                       help='Number of reconstructions which will be used in '
                            'PCA.')
 
-        form.addParam('class3D_PCA_num_components', IntParam, default=5,
+        form.addParam('class3D_PCA_num_components', IntParam, default=2,
                       label="PCA: number of components",
                       condition="class3D_init_mode==1",
                       validators=[Positive],
                       help='PCA: number of components')
 
         form.addParam('class3D_filter_hp_res', IntParam, default=None,
                       allowsNull=True,
@@ -212,24 +216,37 @@
         form.addParam('class3D_mask_use_abs', BooleanParam, default=False,
                       label="Auto mask use absolute value",
                       expertLevel=LEVEL_ADVANCED,
                       help='(If no input mask is provided) Include negative '
                            'regions if they are more negative than the '
                            'threshold')
 
+        form.addParam('class3D_force_resplit', BooleanParam, default=False,
+                      label="Force re-do FSC split",
+                      expertLevel=LEVEL_ADVANCED,
+                      help='Force re-splitting the particles into two random halves. If this is disabled, split is '
+                           'preserved from input alignments. For filaments from helical refinements, it is recommended'
+                           ' to disable this parameter to avoid mis-estimated FSC resolutions.')
+
+        form.addParam('class3D_force_hard_class', BooleanParam, default=False,
+                      label="Force hard classification",
+                      expertLevel=LEVEL_ADVANCED,
+                      help='Force hard classification, so that each particle is only assigned to one class at every '
+                           'iteration, rather than having partial assignment to all classes.')
+
         form.addParam('class3D_class_anneal_beta', FloatParam, default=0.5,
                       label="Class similarity",
                       expertLevel=LEVEL_ADVANCED,
                       validators=[Positive],
                       help='Expected similarity of structures from different '
                            'classes. A number between 0 and 1. 0 means classes '
                            'are independent, 1 means classes are very similar')
 
         form.addParam('class3D_class_anneal_beta_tune', BooleanParam,
-                      default=True,
+                      default=False,
                       label="Auto-tune initial class similarity",
                       expertLevel=LEVEL_ADVANCED,
                       help='Tune initial class similarity based on a target '
                            'class ESS (Effective Sample Size). An ESS close to '
                            'the number of classes at the outset helps to '
                            'ensure the classification does not prematurely '
                            'converge.')
@@ -247,15 +264,15 @@
                       label="Class similarity anneal end iter",
                       expertLevel=LEVEL_ADVANCED,
                       help='Class similarity will be annealed to 0 throughout '
                            'the optimization. This is the end iteration when '
                            'class similarity should equal 0.')
 
         form.addParam('class3D_use_anisomag', BooleanParam,
-                      default=False,
+                      default=True,
                       label="Correct Anisotropic Magnification",
                       expertLevel=LEVEL_ADVANCED,
                       help='Whether or not to correct for anisotropic '
                            'magnification. The anisomag parameters must '
                            'already have been fit but a global CTF refinement '
                            'protocol or within a previous homogeneous '
                            'refinement.')
@@ -364,27 +381,40 @@
             volumes.append(vol)
 
         volumes.setSamplingRate(vol.getSamplingRate())
 
         self._defineOutputs(outputVolumes=volumes)
         self._defineSourceRelation(self.inputParticles.get(), volumes)
 
-        # Create a 3D mask
+        # Create a 3D solvent mask
         volMask = VolumeMask()
         maskFileName = ("%s%s__mask_solvent.mrc" %
                         (getOutputPreffix(self.projectName.get()),
                          self.run3dClassification.get()))
-        # Copy the CS output particles to extra folder
+        # Copy the CS output solvent mask to extra folder
         copyFiles(csOutputFolder, self._getExtraPath(), files=[maskFileName])
         maskFilePath = os.path.join(self._getExtraPath(), maskFileName)
         volMask.setFileName(maskFilePath)
         sr = self._getInputParticles().getSamplingRate()
         volMask.setSamplingRate(sr)
-        self._defineOutputs(outputMask=volMask)
-        self._defineSourceRelation(self.inputParticles.get(), self.outputMask)
+        self._defineOutputs(solventMask=volMask)
+        self._defineSourceRelation(self.inputParticles.get(), volMask)
+
+        # # Create a 3D mask focus
+        # volMaskFocus = VolumeMask()
+        # maskFocusFileName = ("%s%s__mask_focus.mrc" %
+        #                     (getOutputPreffix(self.projectName.get()),
+        #                      self.run3dClassification.get()))
+        # # Copy the CS output focus mask to extra folder
+        # copyFiles(csOutputFolder, self._getExtraPath(), files=[maskFocusFileName])
+        # maskFocusFilePath = os.path.join(self._getExtraPath(), maskFocusFileName)
+        # volMaskFocus.setFileName(maskFocusFilePath)
+        # volMaskFocus.setSamplingRate(sr)
+        # self._defineOutputs(focusMask=volMaskFocus)
+        # self._defineSourceRelation(self.inputParticles.get(), volMaskFocus)
 
     # --------------------------- UTILS functions ---------------------------
     def _loadClassesInfo(self, filename):
         """ Read some information about the produced CryoSparc Classes
         from the star file.
         """
         self._classesInfo = {}  # store classes info, indexed by class id
@@ -482,45 +512,37 @@
         return itera
 
     # --------------------------- INFO functions -------------------------------
 
     def _validate(self):
         validateMsgs = cryosparcValidate()
         if not validateMsgs:
-            csVersion = getCryosparcVersion()
-            if [version for version in self._protCompatibility
-                if parse_version(version) >= parse_version(csVersion)]:
-                validateMsgs = gpusValidate(self.getGpuList(),
-                                            checkSingleGPU=True)
-                if not validateMsgs:
-                    particles = self._getInputParticles()
-                    if not particles.hasCTF():
-                        validateMsgs.append("The Particles has not associated a "
-                                            "CTF model")
-                    if not validateMsgs and not particles.hasAlignmentProj():
-                        validateMsgs.append("The Particles has not "
-                                            "alignment")
+            validateMsgs = gpusValidate(self.getGpuList(),
+                                        checkSingleGPU=True)
+            if not validateMsgs:
+                particles = self._getInputParticles()
+                if not particles.hasCTF():
+                    validateMsgs.append("The Particles has not associated a "
+                                        "CTF model")
+                if not validateMsgs and not particles.hasAlignmentProj():
+                    validateMsgs.append("The Particles has not "
+                                        "alignment")
 
-                    inputVolumes = self._getInputVolume()
+                inputVolumes = self._getInputVolume()
+                if not validateMsgs:
+                    if inputVolumes is not None and inputVolumes:
+                        if self.class3D_init_mode.get() != 2:
+                            validateMsgs.append('Input volumes detected, please set initialization mode to `input` or clear volume inputs.')
+                        if len(inputVolumes) != self.class3D_N_K.get():
+                            validateMsgs.append('No. of input volumes must equal no. of classes')
+                    elif len(particles) < 1000:
+                            validateMsgs.append('Not Enough Images! The set of particles must contain at least 1000 images')
                     if not validateMsgs:
-                        if inputVolumes is not None and inputVolumes:
-                            if self.class3D_init_mode.get() != 2:
-                                validateMsgs.append('Input volumes detected, please set initialization mode to `input` or clear volume inputs.')
-                            if len(inputVolumes) != self.class3D_N_K.get():
-                                validateMsgs.append('No. of input volumes must equal no. of classes')
-                        elif len(particles) < 1000:
-                                validateMsgs.append('Not Enough Images! The set of particles must contain at least 1000 images')
-                        if not validateMsgs:
-                            if self.class3D_N_K.get() < 2:
-                                validateMsgs.append('The number of classes must be grater than 2')
-
-            else:
-                validateMsgs.append("The protocol is not compatible with the "
-                                    "cryoSPARC version %s" % csVersion)
-
+                        if self.class3D_N_K.get() < 2:
+                            validateMsgs.append('The number of classes must be grater than 2')
         return validateMsgs
 
     # --------------------------- UTILS functions ------------------------------
 
     def _getInputVolume(self):
         if self.hasAttribute('refVolumes') and self.refVolumes is not None:
             self.vols = []
@@ -588,14 +610,16 @@
                             'class3D_PCA_num_reconstructions',
                             'class3D_PCA_num_components',
                             'class3D_filter_hp_res', 'class3D_filter_hp_order',
                             'class3D_mask_thresh_factor',
                             'class3D_mask_near_ang',
                             'class3D_mask_far_ang',
                             'class3D_mask_use_abs',
+                            'class3D_force_hard_class',
+                            'class3D_force_resplit',
                             'class3D_class_anneal_beta',
                             'class3D_class_anneal_beta_tune',
                             'class3D_class_anneal_beta_tune_essf',
                             'class3D_class_anneal_end',
                             'class3D_use_anisomag',
                             'class3D_zip_volumes',
                             'class3D_plot_iters',
@@ -631,14 +655,18 @@
         group_connect = {}
         input_group_connect = {"particles": self.particles.get()}
         if self.volumes is not None:
             group_connect["volume"] = self.volumes
 
         if self.mask.get() is not None:
             group_connect["mask"] = [self.mask]
+
+        if self.focusMask.get() is not None:
+            group_connect["mask_focus"] = [self.focusMask]
+
         params = {}
 
         csVersion = getCryosparcVersion()
         isV4_2 = parse_version(csVersion) >= parse_version(V4_1_1)
         if isV4_2:
             params['class3D_reorder_classes'] = str("False")
             params['generate_intermediate_results'] = str("False")
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_new_local_refine.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,16 @@
 
 
 class ProtCryoSparcLocalRefine(ProtCryosparcBase, ProtOperateParticles):
     """ Signal subtraction protocol of cryoSPARC.
         Subtract projections of a masked volume from particles.
         """
     _label = 'local refinement'
-    _devStatus = NEW
     _protCompatibility = [V3_3_1, V3_3_2, V4_0_0,  V4_0_1, V4_0_2, V4_0_3,
-                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0]
+                          V4_1_0, V4_1_1, V4_1_2, V4_2_0, V4_2_1, V4_3_1, V4_4_0, V4_4_1]
     _className = "new_local_refine"
     _fscColumns = 6
 
     def _initialize(self):
         self._defineFileNames()
 
     def _defineFileNames(self):
@@ -274,34 +273,28 @@
     # --------------------------- INFO functions -------------------------------
     def _validate(self):
         """ Should be overwritten in subclasses to
                return summary message for NORMAL EXECUTION.
                """
         validateMsgs = cryosparcValidate()
         if not validateMsgs:
-            csVersion = getCryosparcVersion()
-            if [version for version in self._protCompatibility
-                if parse_version(version) >= parse_version(csVersion)]:
-                validateMsgs = gpusValidate(self.getGpuList(),
-                                            checkSingleGPU=True)
-                if not validateMsgs:
-                    particles = self._getInputParticles()
-                    self._validateDim(particles,
-                                      self.refVolume.get(),
-                                      validateMsgs, 'Input particles',
-                                      'Input volume')
-                    if not particles.hasCTF():
-                        validateMsgs.append("The Particles has not associated a "
-                                            "CTF model")
-                        if not validateMsgs and not particles.hasAlignment3D():
-                            validateMsgs.append("The Particles has not a 3D "
-                                                "alignment")
-            else:
-                validateMsgs.append("The protocol is not compatible with the "
-                                    "cryoSPARC version %s" % csVersion)
+            validateMsgs = gpusValidate(self.getGpuList(),
+                                        checkSingleGPU=True)
+            if not validateMsgs:
+                particles = self._getInputParticles()
+                self._validateDim(particles,
+                                  self.refVolume.get(),
+                                  validateMsgs, 'Input particles',
+                                  'Input volume')
+                if not particles.hasCTF():
+                    validateMsgs.append("The Particles has not associated a "
+                                        "CTF model")
+                    if not validateMsgs and not particles.hasAlignment3D():
+                        validateMsgs.append("The Particles has not a 3D "
+                                            "alignment")
 
         return validateMsgs
 
     def _summary(self):
         summary = []
         if (not hasattr(self, 'outputVolume') or
                 not hasattr(self, 'outputParticles')):
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_part_subtract.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_part_subtract.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_sharppening.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_sharppening.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/protocols.conf` & `scipion-em-cryosparc2-4.1.0/cryosparc2/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/tests/__init__.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/tests/test_protocols_cryosparc2.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/tests/test_protocols_cryosparc2.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/tests/test_utils.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/utils.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+import ast
 import getpass
 import logging
 import os
 import shutil
 import time
 
 from pkg_resources import parse_version
@@ -59,14 +60,35 @@
 # Module variables
 _csVersion = None  # Lazy variable: never use it directly. Use getCryosparcVersion instead
 
 # logging variable
 logger = logging.getLogger(__name__)
 
 
+class NestedDict:
+    def __init__(self, depth=1):
+        self.data = {}
+        self.depth = depth
+
+    def insert(self, keys, value):
+        current = self.data
+        for key in keys[:self.depth - 1]:
+            current = current.setdefault(key, {})
+        current[keys[self.depth - 1]] = value
+
+    def search(self, keys):
+        current = self.data
+        for key in keys[:self.depth]:
+            if key in current:
+                current = current[key]
+            else:
+                return None
+        return current
+
+
 def getCryosparcDir(*paths):
     """
     Get the root directory where cryoSPARC code and dependencies are installed.
     """
     return Plugin.getHome(*paths)
 
 
@@ -220,14 +242,40 @@
     if parse_version(cryosparcVersion) >= parse_version(V4_1_0):
         if userId:
             user = getUserId(user)
 
     return user
 
 
+def getCryosparcProjectsList():
+    """
+    Get list of all projects available
+    :return: all projects available in the database
+    """
+    projects_list_cmd = (getCryosparcProgram() + ' %slist_projects()%s ' % ("'", "'"))
+    cmd = runCmd(projects_list_cmd, printCmd=False)[1]
+    projectList = ast.literal_eval(cmd)
+    return projectList
+
+
+def getCryosparcWorkSpaces(projectId):
+    """ List all workspaces inside a given project (or all projects if not
+    specified)
+
+    :param projectId: target project UID, e.g. "P1", defaults to None
+    :type projectId: str, optional
+    :return: list of workpaces in a project or all projects if not specified
+    :rtype: list
+    """
+    workspace_list_cmd = (getCryosparcProgram() + ' %slist_workspaces("%s")%s ' % ("'", str(projectId), "'"))
+    cmd = runCmd(workspace_list_cmd, printCmd=False)[1]
+    workspacesList = ast.literal_eval(cmd)
+    return workspacesList
+
+
 def isCryosparcStandalone():
     """
     Get the cryoSPARC installation mode. If True, we have a standalone installation
     else a cluster installation is considered. If the environment variable
     CRYOSPARC_STANDALONE_INSTALLATION isn't present, then we assume that we have
     a standalone installation and then, this method returns True
     """
@@ -310,15 +358,15 @@
     return runCmd(create_empty_project_cmd, printCmd=False)
 
 
 def getProjectInformation(project_uid, info='project_dir'):
     """
     Get information about a single project
     :param project_uid: the id of the project
-    :return: the information related to the project thats stored in the database
+    :return: the information related to the project that's stored in the database
     """
     import ast
     getProject_cmd = (getCryosparcProgram() +
                                 ' %sget_project("%s")%s '
                                 % ("'", str(project_uid), "'"))
 
     project_info = runCmd(getProject_cmd, printCmd=False)
@@ -350,15 +398,15 @@
 
 def getOutputPreffix(projectName):
     cryosparcVersion = getCryosparcVersion()
     preffix = "cryosparc_" + projectName+"_" if parse_version(cryosparcVersion) < parse_version(V4_0_0) else ""
     return preffix
 
 
-def createProjectDir(project_container_dir):
+def createProjectContainerDir(project_container_dir):
     """
     Given a "root" directory, create a project (PXXX) dir if it doesn't already
      exist
     :param project_container_dir: the "root" directory in which to create the
                                   project (PXXX) directory
     :returns: str - the final path of the new project dir with shell variables
               still in the returned path (the path should be expanded every
@@ -431,14 +479,49 @@
                      "Please, go to cryoSPARC software for more "
                      "details."
                      )
 
     return importedVolume
 
 
+def doImportMicrographs(protocol):
+    print(pwutils.yellowStr("Importing micrographs..."), flush=True)
+    className = "import_micrographs"
+    micrographs = protocol._getInputMicrographs()
+    acquisition = micrographs.getAcquisition()
+    micList = list(micrographs.getFiles())
+
+    micFolder = os.path.join(protocol._getExtraPath('micrographs'))
+    os.makedirs(micFolder, exist_ok=True)
+
+    for micPath in micList:
+        micName = os.path.basename(micPath)
+        micLink = os.path.join(micFolder, micName)
+        os.symlink(os.path.abspath(micPath), micLink)
+    micExt = '*%s' % os.path.splitext(micList[0])[1]
+
+    params = {"blob_paths": str(os.path.join(os.getcwd(), micFolder, micExt)),
+              "psize_A": str(micrographs.getSamplingRate()),
+              "accel_kv": str(acquisition.getVoltage()),
+              "cs_mm": str(acquisition.getSphericalAberration()),
+              "total_dose_e_per_A2": str(0.1),
+              "output_constant_ctf": "True"
+              }
+
+    import_particles = enqueueJob(className, protocol.projectName, protocol.workSpaceName,
+                                  str(params).replace('\'', '"'), '{}', protocol.lane)
+
+    waitForCryosparc(protocol.projectName.get(), import_particles.get(),
+                     "An error occurred importing particles. "
+                     "Please, go to cryoSPARC software for more "
+                     "details.")
+
+    return import_particles
+
+
 def doJob(jobType, projectName, workSpaceName, params, input_group_connect):
     """
     do_job(job_type, puid='P1', wuid='W1', uuid='devuser', params={},
            input_group_connects={})
     """
     do_job_cmd = (getCryosparcProgram() +
                   ' %sdo_job("%s","%s","%s", "%s", %s, %s)%s' %
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/__init__.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_2Dclassify.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_2Dclassify.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_initialmodel.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_initialmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         group = form.addGroup('3D Classes')
 
         group.addParam('show3DClasses', LabelParam,
                        label='Initial model output classes')
 
         group = form.addGroup('Volume')
 
-        group.addParam('displayVol', EnumParam, choices=['dataViewer', 'cryoSPARC'],
+        group.addParam('displayVol', EnumParam, choices=['cryoSPARC', 'dataViewer'],
                        default=DATA_VIEWER, display=EnumParam.DISPLAY_HLIST,
                        label='Display volume with',
                        help='*dataViewer*: display volumes as surface with Scipion.\n'
                             '*cryoSPARC: display volumes as surface with cryoSPARC')
         # '*slices*: display volumes as 2D slices along z axis.\n'
 
     def _getVisualizeDict(self):
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_partsubtract.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_partsubtract.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/viewers/viewer_refinement.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/viewers/viewer_refinement.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,58 +34,87 @@
 from pyworkflow.protocol.params import (LabelParam, FloatParam, EnumParam)
 from pyworkflow.viewer import DESKTOP_TKINTER, WEB_DJANGO
 from pwem.viewers import (ChimeraView, ObjectView, EmProtocolViewer, FscViewer)
 
 from ..protocols import (ProtCryoSparcLocalRefine, ProtCryoSparcHelicalRefine3D,
                          ProtCryoSparc3DHomogeneousRefine,
                          ProtCryoSparcNewNonUniformRefine3D,
-                         ProtCryoSparcHomogeneousReconstruct)
+                         ProtCryoSparcHomogeneousReconstruct, ProtCryoSparc3DVariability,
+                         ProtCryoSparc3DVariabilityDisplay)
 from ..constants import *
 from ..utils import *
 
 
 class CryosPARCViewer3DRefinement(EmProtocolViewer):
     """ Visualization of e2refine_easy results. """
 
     _targets = [ProtCryoSparcLocalRefine, ProtCryoSparcHelicalRefine3D,
                 ProtCryoSparc3DHomogeneousRefine, ProtCryoSparcNewNonUniformRefine3D,
-                ProtCryoSparcHomogeneousReconstruct]
+                ProtCryoSparcHomogeneousReconstruct, ProtCryoSparc3DVariability,
+                ProtCryoSparc3DVariabilityDisplay]
     _environments = [DESKTOP_TKINTER, WEB_DJANGO]
     _label = 'viewer Refinement'
     cryosparcVersion = getCryosparcVersion()
 
     def _defineParams(self, form):
         self._env = os.environ.copy()
         form.addSection(label='Results')
 
         group = form.addGroup('cryoSPARC')
 
         group.addParam('displayCS', LabelParam,
                        label='Display the processing with cryoSPARC')
 
         if self.protocol.isFinished():
-            group = form.addGroup('Particles')
 
-            group.addParam('showImagesAngularAssignment', LabelParam,
-                           label='Particles angular assignment')
+            if not isinstance(self.protocol, ProtCryoSparc3DVariabilityDisplay):
+                group = form.addGroup('Particles')
 
-            group = form.addGroup('Volume')
+                group.addParam('showImagesAngularAssignment', LabelParam,
+                               label='Particles angular assignment')
+
+            is3dVariavilityProt = isinstance(self.protocol, ProtCryoSparc3DVariabilityDisplay)
+            groupName = 'Volume' if not is3dVariavilityProt else 'Components'
+            if is3dVariavilityProt and self.protocol.var_output_mode.get() == 0:
+                groupName = 'Volume'
+
+            group = form.addGroup(groupName)
+            if not isinstance(self.protocol, ProtCryoSparc3DVariabilityDisplay):
+                displayChoices = ['chimera', 'data viewer']
+            else:
+                if self.protocol.var_output_mode.get() != 0:
+                    self.componetChoices = self.getComponetChoices()
+                    group.addParam('component', EnumParam,
+                                   choices=list(self.componetChoices),
+                                   default=0, display=EnumParam.DISPLAY_COMBO,
+                                   label='Select a component',
+                                   help='Select a component to display the conformation')
+
+                    group.addParam('maxFrameRate', IntParam,
+                                   default=4,
+                                   label='Playback rate',
+                                   help='Specify a maximum playback rate in steps per second. By default, playback is as fast as possible, which can be fairly slow for large data. This option is used to slow playback when it is too fast.'
+                                   )
+
+                displayChoices = ['chimera']
+            label = 'Display volume with' if not isinstance(self.protocol, ProtCryoSparc3DVariabilityDisplay) else 'Display componet with'
+            if is3dVariavilityProt and self.protocol.var_output_mode.get() == 0:
+                label = 'Display volume with'
+                displayChoices = ['data viewer']
 
-            displayChoices = ['data viewer', 'chimera']
-            label = 'Display volume with'
             help = '*data viewer: display volumes as surface with Scipion data viewer. \n ' \
                    '*chimera*: display volumes as surface with Chimera.'
 
             group.addParam('displayVol', EnumParam, choices=displayChoices,
-                           default=DATA_VIEWER, display=EnumParam.DISPLAY_LIST,
+                           default=VOLUME_CHIMERA, display=EnumParam.DISPLAY_LIST,
                            label=label,
                            help=help)
             # '*slices*: display volumes as 2D slices along z axis.\n'
 
-            if self.protocol.isFinished() and parse_version(self.cryosparcVersion) != parse_version(V4_0_0):
+            if self.protocol.isFinished() and parse_version(self.cryosparcVersion) != parse_version(V4_0_0) and not isinstance(self.protocol, ProtCryoSparc3DVariabilityDisplay) and not isinstance(self.protocol, ProtCryoSparc3DVariability):
                 group = form.addGroup('Resolution')
 
                 self.choices = self.getChoices()
 
                 group.addParam('resolutionPlotsFSC', EnumParam,
                                choices=list(self.choices),
                                default=0, display=EnumParam.DISPLAY_COMBO,
@@ -94,15 +123,14 @@
                                     '*masked*: display FSC of masked maps.\n'
                                     '*masked tight*: display FSC of masked tight maps.')
                 group.addParam('resolutionThresholdFSC', FloatParam, default=0.143,
                                expertLevel=LEVEL_ADVANCED,
                                label='Threshold ',
                                help='Threshold in resolution plots')
 
-
     def _getVisualizeDict(self):
         return {'showImagesAngularAssignment': self._showOutputParticles,
                 'displayVol': self._showVolumes,
                 'resolutionPlotsFSC': self._showFSC,
                 'displayCS': self._showCryoSPARVolume
                 }
 
@@ -125,15 +153,15 @@
                                            viewParams=viewParams)
             views.append(v)
         return views
 
     def _showOutputVolume(self, paramName=None):
         views = []
 
-        if getattr(self.protocol, 'outputVolume', None) is not None:
+        if getattr(self.protocol, paramName, None) is not None:
             volume = self.protocol.outputVolume
             fn = volume.getFileName()
             v = self.createScipionPartView(fn, volume)
             views.append(v)
         return views
 
     def createScipionPartView(self, filename, obj, viewParams={}):
@@ -147,15 +175,15 @@
     # =========================================================================
     # ShowVolumes
     # =========================================================================
     def _showVolumes(self, paramName=None):
         if self.displayVol == VOLUME_CHIMERA:
             return self._showVolumesChimera()
         elif self.displayVol == DATA_VIEWER:
-            return self._showOutputVolume()
+            return self._showOutputVolume(paramName='outputVolume')
 
     def _showCryoSPARVolume(self, paramName=None):
         views = []
         system_info = getSystemInfo()
         status_errors = system_info[0]
         print(status_errors)
         if not status_errors:
@@ -185,30 +213,45 @@
     def _showVolumesChimera(self):
         """ Create a chimera script to visualize selected volumes. """
 
         # Check if Chimera is installed
         view = []
         chimera = Domain.importFromPlugin('chimera')
         if chimera is not None:
-            volumes = [self.protocol.outputVolume.getFileName()]
-            if len(volumes) > 1:
+            if not isinstance(self.protocol, ProtCryoSparc3DVariabilityDisplay):
+                volumes = [self.protocol.outputVolume.getFileName()]
+                if len(volumes) > 1:
+                    cmdFile = self.protocol._getExtraPath('chimera_volumes.cxc')
+                    f = open(cmdFile, 'w+')
+                    for vol in volumes:
+                        # We assume that the chimera script will be generated
+                        # at the same folder as eman volumes
+                        if os.path.exists(vol):
+                            localVol = os.path.relpath(vol,
+                                                       self.protocol._getExtraPath())
+                            f.write("open %s\n" % localVol)
+                    f.write('tile\n')
+                    f.close()
+                    view.append(ChimeraView(cmdFile))
+                else:
+                    view.append(ChimeraView(volumes[0]))
+            elif self.protocol.var_output_mode.get() != 0:
+                component = self.componetChoices[self.component.get()]
+                componentsPath = os.path.abspath(self.protocol._getExtraPath(component))
                 cmdFile = self.protocol._getExtraPath('chimera_volumes.cxc')
                 f = open(cmdFile, 'w+')
-                for vol in volumes:
-                    # We assume that the chimera script will be generated
-                    # at the same folder than eman volumes
-                    if os.path.exists(vol):
-                        localVol = os.path.relpath(vol,
-                                                   self.protocol._getExtraPath())
-                        f.write("open %s\n" % localVol)
-                f.write('tile\n')
+                f.write("open %s/*.mrc vseries true\n" % componentsPath)
+                f.write("vseries play #1 loop true maxFrameRate %d\n" % self.maxFrameRate.get())
                 f.close()
                 view.append(ChimeraView(cmdFile))
             else:
-                view.append(ChimeraView(volumes[0]))
+                volume = self.protocol.outputVolumes
+                fn = volume.getFileName()
+                v = self.createScipionPartView(fn, volume)
+                view.append(v)
         else:
             showInfo('Info', "Chimera plugin is not installed. Please, "
                              "install it to display the volume",
                      self.getTkRoot())
 
         return view
 
@@ -229,14 +272,21 @@
             self.protocol._defineOutputs(outputFSC=self.setOfFSCs)
             for fsc in self.setOfFSCs.iterItems():
                 choices.append(fsc.getObjLabel())
         choices.append('All')
 
         return choices
 
+    def getComponetChoices(self):
+        if self.protocol.var_output_mode.get() == 2 and self.protocol.var_intermediate_output_frame_particles.get():
+            return self.protocol._outputs[0:-1]
+        else:
+            return self.protocol._outputs
+
+
     # =========================================================================
     # plotFSC
     # =========================================================================
     def _showFSC(self, paramName=None):
 
         fscViewer = FscViewer(project=self.getProject(),
                               protocol=self.protocol)
```

### Comparing `scipion-em-cryosparc2-4.0.9/cryosparc2/wizards.py` & `scipion-em-cryosparc2-4.1.0/cryosparc2/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/PKG-INFO` & `scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-cryosparc2
-Version: 4.0.9
+Version: 4.1.0
 Summary: Plugin to use cryoSPARC2 programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-cryosparc2
 Author: Yunior C. Fonseca Reyna, Szu-Chi Chung
 Author-email: cfonseca@cnb.csic.es, phonchi@stat.sinica.edu.tw
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-cryosparc2/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-cryosparc2/
@@ -30,34 +30,64 @@
         * **Helical 3D Refinement**: Reconstruct and refine a homogeneous helical assembly, with or without imposition and refinement of symmetry parameters.
         * **3D Homogeneous Refinement(new)**: Rapidly refine a single homogeneous structure to high-resolution and validate using the gold-standard FSC. Using new faster GPU code, and support for higher-order aberration (beam tilt, spherical aberration, trefoil, tetrafoil) correction and per-particle defocus refinement on the fly.
         * **3D Non uniform Refinement(new)**: Apply non-uniform refinement to achieve higher resolution and map quality. Specially designed for small proteins and membrane proteins.
         * **3D Local Refinement(new)**  Refine a masked region within a consensus structure by allowing particle alignments to vary only slightly.
         * **Symmetry Expansion**: Duplicate particles around a point-group symmetry.
         * **Homogeneous Reconstruction**: Reconstruct half-maps from input particles with alignments
         * **3D Classification**: Classify particles into multiple 3D classes and optimize 3D class densities (currently, without re-aligning particle pose or shift).
+        * **3D Variability Analysis**: Protocol to compute the principle modes of variability with a dataset of aligned particles
+        * **3D Variability Display**: Protocol to create various versions of a 3D variability result that can be used for display
+        * **Blob Picker**: Automatically picks particles by searching for Gaussian signals.
+        * **Patch CTF Estimation**:  Patch-based CTF estimation automatically estimates defocus variation for tilted, bent, deformed samples and is accurate for all particle sizes and types including flexible and membrane proteins.
+        * **3D Flex Data Prep**: Prepares particles for use in 3DFlex training and reconstruction. At the same  way,  Takes in a consensus (rigid) refinement density map, plus optionally a segmentation and generates a tetrahedral mesh for 3DFlex.
+        * **3D Flex Mesh Prep**: Takes in a consensus (rigid) refinement density map, plus optionally a segmentation and generates a tetrahedral mesh for 3DFlex. See Mesh Generation below.
+        * **3D Flex Training**: Uses a mesh and prepared particles (at a downsampled resolution) to train a 3DFlex model. Parameters control the number of latent dimensions, size of the model, and training hyperparameters. This job outputs checkpoints during training.
+        * **3D Flex Reconstruction**: Takes in a checkpoint from training as well as prepared high-resolution particles and performs high-resolution refinement using L-BFGS under the 3DFlex model. This is the stage at which improvements to density in high-res regions are computed. Outputs two half-maps that can be used for FSC validation, sharpening, and other downstream tasks.
+        
         
         **Latest plugin version**
         ==========================
         
-        **v4.0.9**
+        
+        **v4.1.0**
         -----------
-        * **new**        Compatibility with cryoSPARC v4.4.0
-        * **fixed**      Handling aborted protocols/jobs
+        * **fixed**       Tolerating deletion of projects within CS as well as their folders in the file system
+        
+        * **new**         Add new protocols:
+                            * **3D Flex Data Prep**: Prepares particles for use in 3DFlex training and reconstruction. At the same  way,  Takes in a consensus (rigid) refinement density map, plus optionally a segmentation and generates a tetrahedral mesh for 3DFlex.
+                            * **3D Flex Mesh Prep**: Takes in a consensus (rigid) refinement density map, plus optionally a segmentation and generates a tetrahedral mesh for 3DFlex. See Mesh Generation below.
+                            * **3D Flex Training**: Uses a mesh and prepared particles (at a downsampled resolution) to train a 3DFlex model. Parameters control the number of latent dimensions, size of the model, and training hyperparameters. This job outputs checkpoints during training.
+                            * **3D Flex Reconstruction**: Takes in a checkpoint from training as well as prepared high-resolution particles and performs high-resolution refinement using L-BFGS under the 3DFlex model. This is the stage at which improvements to density in high-res regions are computed. Outputs two half-maps that can be used for FSC validation, sharpening, and other downstream tasks.
+        
+        * **new**         Allowing Scipion to import coordinates
+        
+        
+        **v4.0.11**
+        -----------
+        * **fixed**      Compatibility with cryoSPARC v4.4.1+patch
         
-        **v4.0.8**
+        
+        
+        **v4.0.10**
         -----------
-        * **new**        Compatibility with cryoSPARC v4.3.1
-        * **removed**    Deprecated protocols removed: Legacy Refine, Legacy no uniform refine, Legacy naive local refine.
+        * **new**        Compatibility with cryoSPARC v4.4.1
+        * **new**        Add new protocols:
+        
+                         * **3D Variability Analysis**: Protocol to compute the principle modes of variability with a dataset of aligned particles
+                         * **3D Variability Display**: Protocol to create various versions of a 3D variability result that can be used for display
+                         * **Blob Picker**: Automatically picks particles by searching for Gaussian signals.
+        
+        
         
-        **v4.0.7**
+        
+        **v4.0.9**
         -----------
-        * **new**     :  Compatibility with cryoSPARC v4.2.1
-        * **new**        Plugin operation in a cluster
-        * **fixed**      Fixed an installation error
-        * **fixed**      Fixed an error related with the calculation of the particles shifts
+        * **new**        Compatibility with cryoSPARC v4.4.0
+        * **fixed**      Handling aborted protocols/jobs
+        
         
         **Installing the plugin**
         =========================
         
         In order to install the plugin follow these instructions:
         
         1. **Install the plugin**
```

### Comparing `scipion-em-cryosparc2-4.0.9/scipion_em_cryosparc2.egg-info/SOURCES.txt` & `scipion-em-cryosparc2-4.1.0/scipion_em_cryosparc2.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,31 @@
 cryosparc2/convert/cs2Start.py
 cryosparc2/convert/dataimport.py
 cryosparc2/protocols/__init__.py
 cryosparc2/protocols/protocol_base.py
 cryosparc2/protocols/protocol_cryosparc2d.py
 cryosparc2/protocols/protocol_cryosparc_3D_classification.py
 cryosparc2/protocols/protocol_cryosparc_3D_flex_data_prepare.py
+cryosparc2/protocols/protocol_cryosparc_3D_flex_mesh_prepare.py
 cryosparc2/protocols/protocol_cryosparc_3D_flex_reconstruction.py
 cryosparc2/protocols/protocol_cryosparc_3D_flex_training.py
 cryosparc2/protocols/protocol_cryosparc_3d_variability.py
 cryosparc2/protocols/protocol_cryosparc_3d_variability_display.py
 cryosparc2/protocols/protocol_cryosparc_ab.py
+cryosparc2/protocols/protocol_cryosparc_blob_picker.py
 cryosparc2/protocols/protocol_cryosparc_global_ctf_refinement.py
 cryosparc2/protocols/protocol_cryosparc_helical_refinement.py
 cryosparc2/protocols/protocol_cryosparc_homogeneous_reconstruction.py
 cryosparc2/protocols/protocol_cryosparc_homogeneous_refine.py
 cryosparc2/protocols/protocol_cryosparc_local_ctf_refinement.py
 cryosparc2/protocols/protocol_cryosparc_new_3D_classification.py
 cryosparc2/protocols/protocol_cryosparc_new_local_refine.py
 cryosparc2/protocols/protocol_cryosparc_new_nonuniform_refine.py
 cryosparc2/protocols/protocol_cryosparc_part_subtract.py
+cryosparc2/protocols/protocol_cryosparc_patch_ctf_estimation.py
 cryosparc2/protocols/protocol_cryosparc_sharppening.py
 cryosparc2/protocols/protocol_cryosparc_symmetry_expansion.py
 cryosparc2/tests/__init__.py
 cryosparc2/tests/test_protocols_cryosparc2.py
 cryosparc2/tests/test_utils.py
 cryosparc2/viewers/__init__.py
 cryosparc2/viewers/viewer_2Dclassify.py
```

### Comparing `scipion-em-cryosparc2-4.0.9/setup.py` & `scipion-em-cryosparc2-4.1.0/setup.py`

 * *Files identical despite different names*

