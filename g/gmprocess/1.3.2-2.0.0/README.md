# Comparing `tmp/gmprocess-1.3.2.tar.gz` & `tmp/gmprocess-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmprocess-1.3.2.tar", last modified: Sat Feb  3 20:54:11 2024, max compression
+gzip compressed data, was "gmprocess-2.0.0.tar", last modified: Mon Apr 29 14:27:44 2024, max compression
```

## Comparing `gmprocess-1.3.2.tar` & `gmprocess-2.0.0.tar`

### file list

```diff
@@ -1,308 +1,262 @@
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.940614 gmprocess-1.3.2/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1660 2024-02-03 20:51:46.000000 gmprocess-1.3.2/LICENSE.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      114 2024-02-03 20:51:46.000000 gmprocess-1.3.2/MANIFEST.in
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     6166 2024-02-03 20:54:11.940614 gmprocess-1.3.2/PKG-INFO
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1582 2024-02-03 20:51:46.000000 gmprocess-1.3.2/README.md
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2584 2024-02-03 20:51:46.000000 gmprocess-1.3.2/pyproject.toml
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-02-03 20:54:11.944614 gmprocess-1.3.2/setup.cfg
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      175 2024-02-03 20:51:46.000000 gmprocess-1.3.2/setup.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.868614 gmprocess-1.3.2/src/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.876614 gmprocess-1.3.2/src/gmprocess/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/__init__.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.876614 gmprocess-1.3.2/src/gmprocess/apps/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/apps/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14597 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/apps/gmrecords.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.880614 gmprocess-1.3.2/src/gmprocess/bin/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/bin/__init__.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6138 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/bin/bundle_datarelease.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8169 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/bin/cwb_gather.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5408 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/bin/fix_inventory.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     5145 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/bin/gmconvert.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8792 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/bin/gminfo.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      152 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/bin/gmrecords.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     5104 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/bin/gmworkspace.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     2002 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/bin/list_metrics.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.880614 gmprocess-1.3.2/src/gmprocess/core/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/core/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    16025 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/core/provenance.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    19090 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/core/stationstream.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    39941 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/core/stationtrace.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5471 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/core/streamarray.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    27744 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/core/streamcollection.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.884614 gmprocess-1.3.2/src/gmprocess/data/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      616 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/CESMD_NGA_ids.csv
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    41885 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/GDMSstations.json
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/data/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25396 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/config_production.yml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25744 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/config_test.yml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    39424 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/cosmos_table10.xls
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    32768 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/cosmos_table4.xls
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.868614 gmprocess-1.3.2/src/gmprocess/data/demo/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.868614 gmprocess-1.3.2/src/gmprocess/data/demo/ci38457511/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.884614 gmprocess-1.3.2/src/gmprocess/data/demo/ci38457511/raw/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   989427 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/demo/ci38457511/raw/CICCC.RAW
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   896593 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/demo/ci38457511/raw/CICLC.v1
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   994737 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/demo/ci38457511/raw/CITOW2.RAW
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    55506 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/fdsn_codes.csv
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.888614 gmprocess-1.3.2/src/gmprocess/data/lme/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999) 11719610 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/lme/SA_rotd50.0_2020.03.31.csv
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      905 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/modules.yml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   737944 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nga_w2_selected.csv
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.896614 gmprocess-1.3.2/src/gmprocess/data/nn_clipping/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      409 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_clipping/bias_1.csv
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       26 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_clipping/bias_output.csv
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       26 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_clipping/masterF.txt
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2032 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_clipping/weight_1.csv
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      408 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_clipping/weight_output.csv
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.872614 gmprocess-1.3.2/src/gmprocess/data/nn_qa/
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.900614 gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8152 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/M.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      304 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/bias_1.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      406 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/bias_2.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       43 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/bias_output.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     5251 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/final_training.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       35 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/masterF.txt
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    11468 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/model_3.txt
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    12981 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/model_5.txt
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      767 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/mu_sigma.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6135 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/weight_1.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6041 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/weight_2.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      791 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/weight_output.csv
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.904614 gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8171 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/M.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      293 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/bias_1.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      316 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/bias_2.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       42 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/bias_output.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     3569 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/final_training.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       35 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/masterF.txt
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    10524 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/model_0.txt
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      770 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/mu_sigma.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6037 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/weight_1.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     4418 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/weight_2.csv
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      596 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/weight_output.csv
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2233 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/picker.yml
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11182 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/station_coordinates.xlsx
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    79189 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/data/usgs_ids_nga_and_srcmod_cross_reference.xlsx
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.904614 gmprocess-1.3.2/src/gmprocess/io/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/io/__init__.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.908614 gmprocess-1.3.2/src/gmprocess/io/asdf/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/io/asdf/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      374 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/asdf/base_metrics_xml.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2271 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/asdf/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    19689 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/asdf/flatfile.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5829 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/asdf/flatfile_constants.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3319 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/asdf/path_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4972 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/asdf/rupture.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3070 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/asdf/station_metrics_xml.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    41928 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/asdf/stream_workspace.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2514 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/asdf/utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4241 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/asdf/waveform_metrics_xml.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      159 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/asdf/workspace_constants.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.908614 gmprocess-1.3.2/src/gmprocess/io/bhrc/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/io/bhrc/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7799 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/bhrc/core.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.908614 gmprocess-1.3.2/src/gmprocess/io/cosmos/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/io/cosmos/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13199 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/cosmos/cesmd_fetcher.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    17913 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/cosmos/cesmd_search.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    28924 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/cosmos/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    31797 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/cosmos/cosmos_writer.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4117 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/cosmos/data_structures.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.908614 gmprocess-1.3.2/src/gmprocess/io/cwb/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/io/cwb/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9344 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/cwb/core.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.908614 gmprocess-1.3.2/src/gmprocess/io/dmg/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/io/dmg/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    32813 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/dmg/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4084 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/dynamic_search_parameters.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.908614 gmprocess-1.3.2/src/gmprocess/io/esm/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/io/esm/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6496 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/esm/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4023 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/fetcher.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.908614 gmprocess-1.3.2/src/gmprocess/io/geonet/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/io/geonet/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13220 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/geonet/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5717 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/global_fetcher.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.908614 gmprocess-1.3.2/src/gmprocess/io/knet/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/io/knet/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6860 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/knet/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    15161 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/knet/knet_fetcher.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1958 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/nga.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.912614 gmprocess-1.3.2/src/gmprocess/io/nsmn/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/io/nsmn/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6220 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/nsmn/core.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.912614 gmprocess-1.3.2/src/gmprocess/io/obspy/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/io/obspy/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9200 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/obspy/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12219 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/obspy/fdsn_fetcher.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5518 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/read.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2548 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/read_directory.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.912614 gmprocess-1.3.2/src/gmprocess/io/renadic/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/io/renadic/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9262 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/renadic/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9991 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/report.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1988 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/seedname.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.912614 gmprocess-1.3.2/src/gmprocess/io/smc/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/io/smc/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    18244 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/smc/core.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.912614 gmprocess-1.3.2/src/gmprocess/io/unam/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/io/unam/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12493 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/unam/core.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.912614 gmprocess-1.3.2/src/gmprocess/io/usc/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/io/usc/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    17340 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/usc/core.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5749 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/io/utils.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.916614 gmprocess-1.3.2/src/gmprocess/metrics/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/metrics/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      986 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/base_metric_collection.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.916614 gmprocess-1.3.2/src/gmprocess/metrics/combination/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/metrics/combination/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1464 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/combination/arithmetic_mean.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2578 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/combination/combination.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1509 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/combination/geometric_mean.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      897 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/combination/greater_of_two_horizontals.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      742 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/combination/null_combination.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1569 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/combination/quadratic_mean.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      129 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/exception.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      691 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/gather.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.916614 gmprocess-1.3.2/src/gmprocess/metrics/imc/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/metrics/imc/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1251 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imc/arithmetic_mean.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1153 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imc/channels.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1246 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imc/geometric_mean.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1103 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imc/gmrotd.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1252 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imc/greater_of_two_horizontals.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1536 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imc/imc.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1402 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imc/quadratic_mean.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1201 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imc/radial_transverse.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1287 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imc/rotd.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.920614 gmprocess-1.3.2/src/gmprocess/metrics/imt/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/metrics/imt/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1116 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imt/arias.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1311 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imt/duration.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1027 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imt/fas.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1366 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imt/imt.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1021 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imt/pga.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1017 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imt/pgv.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      955 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imt/sa.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1337 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/imt/sorted_duration.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    31179 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/metrics_controller.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.920614 gmprocess-1.3.2/src/gmprocess/metrics/reduction/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/metrics/reduction/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2951 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/reduction/arias.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2728 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/reduction/duration.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2933 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/reduction/max.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1749 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/reduction/null_reduction.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3077 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/reduction/percentile.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1231 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/reduction/reduction.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3454 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/reduction/smooth_select.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2888 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/reduction/sorted_duration.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.920614 gmprocess-1.3.2/src/gmprocess/metrics/rotation/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/metrics/rotation/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1192 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/rotation/gmrotd.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      597 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/rotation/null_rotation.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3569 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/rotation/radial_transverse.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7980 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/rotation/rotation.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1451 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/rotation/rotd.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      860 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/station_metric.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9881 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/station_metric_collection.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.924614 gmprocess-1.3.2/src/gmprocess/metrics/transform/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/metrics/transform/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2736 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/transform/differentiate.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3579 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/transform/fft.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2026 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/transform/integrate.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1001 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/transform/null_transform.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6451 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/transform/oscillator.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2474 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/transform/transform.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2842 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11605 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/waveform_metric.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10491 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/waveform_metric_collection.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4552 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/metrics/waveform_metric_list.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.928614 gmprocess-1.3.2/src/gmprocess/subcommands/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/subcommands/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      284 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/arg_dicts.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3904 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/assemble.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4365 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/autoprocess.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3685 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/autoshakemap.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7514 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/base.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4677 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/clean.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4779 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/compute_station_metrics.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5221 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/compute_waveform_metrics.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5200 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/config.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1299 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/download.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4915 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/export_failure_tables.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2272 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/export_gmpacket.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6819 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/export_metric_tables.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2757 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/export_provenance_tables.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2918 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/export_shakemap.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4558 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/generate_regression_plot.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5864 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/generate_report.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2762 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/generate_station_maps.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2356 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/import_data.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1478 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/init.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1406 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/lazy_loader.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5010 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/process_waveforms.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1966 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/processing_steps.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    16157 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/subcommands/projects.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.932614 gmprocess-1.3.2/src/gmprocess/utils/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/utils/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      757 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/args.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3554 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/assemble_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6982 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/base_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12912 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/config.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3923 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/constants.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7036 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/download_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7609 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/event.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13202 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/export_gmpacket_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13147 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/export_shakemap_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      726 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/ground_motion_models.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3291 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/logging.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      380 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/misc.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11858 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/misc_plots.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2335 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/prompt.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12759 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/report_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      577 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/rupture_utils.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2622 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/stderr.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1695 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/strec.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13201 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/summary_plots.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      797 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/tables.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2021 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/utils/test_utils.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.936614 gmprocess-1.3.2/src/gmprocess/waveform_processing/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:51:47.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/__init__.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4499 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/adjust_highpass.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3135 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/adjust_highpass_ridder.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1796 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/baseline_correction.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.936614 gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3258 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/clip_detection.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7371 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/clipping_ann.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2394 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/clipping_check.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14444 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/histogram.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2902 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/jerk.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2626 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/max_amp.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2527 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/ping.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4078 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/std_dev.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10652 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/corner_frequencies.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2319 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/detrend.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3452 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/fft.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4217 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/filtering.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7517 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/instrument_response.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1038 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/integrate.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    30903 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/nn_quality_assurance.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    26303 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/phase.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7131 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/pretesting.py
--rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6775 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/processing.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1187 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/processing_step.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1058 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/resample.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3311 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/sanity_checks.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9980 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/snr.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    20365 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/spectrum.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1555 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/taper.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    19697 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/windows.py
--rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2028 2024-02-03 20:51:46.000000 gmprocess-1.3.2/src/gmprocess/waveform_processing/zero_crossings.py
-drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-02-03 20:54:11.936614 gmprocess-1.3.2/src/gmprocess.egg-info/
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)     6166 2024-02-03 20:54:11.000000 gmprocess-1.3.2/src/gmprocess.egg-info/PKG-INFO
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)    10595 2024-02-03 20:54:11.000000 gmprocess-1.3.2/src/gmprocess.egg-info/SOURCES.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-02-03 20:54:11.000000 gmprocess-1.3.2/src/gmprocess.egg-info/dependency_links.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      319 2024-02-03 20:54:11.000000 gmprocess-1.3.2/src/gmprocess.egg-info/entry_points.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)      871 2024-02-03 20:54:11.000000 gmprocess-1.3.2/src/gmprocess.egg-info/requires.txt
--rw-r--r--   0 usgs-user   (999) usgs-user   (999)       10 2024-02-03 20:54:11.000000 gmprocess-1.3.2/src/gmprocess.egg-info/top_level.txt
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.114842 gmprocess-2.0.0/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1660 2024-04-29 13:59:27.000000 gmprocess-2.0.0/LICENSE.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      116 2024-04-29 14:26:02.000000 gmprocess-2.0.0/MANIFEST.in
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     6557 2024-04-29 14:27:44.110842 gmprocess-2.0.0/PKG-INFO
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1947 2024-04-29 13:59:27.000000 gmprocess-2.0.0/README.md
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2660 2024-04-29 13:59:27.000000 gmprocess-2.0.0/pyproject.toml
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       38 2024-04-29 14:27:44.114842 gmprocess-2.0.0/setup.cfg
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      175 2024-04-29 13:59:27.000000 gmprocess-2.0.0/setup.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.042842 gmprocess-2.0.0/src/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.046842 gmprocess-2.0.0/src/gmprocess/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/__init__.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.050842 gmprocess-2.0.0/src/gmprocess/apps/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/apps/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14633 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/apps/gmrecords.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.050842 gmprocess-2.0.0/src/gmprocess/bin/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/bin/__init__.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6138 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/bin/bundle_datarelease.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8288 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/bin/cwa_gather.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5406 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/bin/fix_inventory.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     5145 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/bin/gmconvert.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8792 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/bin/gminfo.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     2006 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/bin/gmprocess_config.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      152 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/bin/gmrecords.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     5104 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/bin/gmworkspace.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      213 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/bin/update_event_json.sh
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.054842 gmprocess-2.0.0/src/gmprocess/core/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/core/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    16122 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/core/provenance.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11682 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/core/scalar_event.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    19057 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/core/stationstream.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    39567 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/core/stationtrace.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5491 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/core/streamarray.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    28258 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/core/streamcollection.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.058842 gmprocess-2.0.0/src/gmprocess/data/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      616 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/CESMD_NGA_ids.csv
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/data/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    23527 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/config_production.yml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    24932 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/config_production_v1.yml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    24841 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/config_test.yml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    39424 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/cosmos_table10.xls
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    32768 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/cosmos_table4.xls
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.042842 gmprocess-2.0.0/src/gmprocess/data/demo/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.042842 gmprocess-2.0.0/src/gmprocess/data/demo/ci38457511/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.058842 gmprocess-2.0.0/src/gmprocess/data/demo/ci38457511/raw/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   989427 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/demo/ci38457511/raw/CICCC.RAW
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   896593 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/demo/ci38457511/raw/CICLC.v1
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   994737 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/demo/ci38457511/raw/CITOW2.RAW
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.058842 gmprocess-2.0.0/src/gmprocess/data/demo/nc72282711/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)  2053533 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/demo/nc72282711/workspace.h5
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    55506 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/fdsn_codes.csv
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.062842 gmprocess-2.0.0/src/gmprocess/data/lme/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999) 11719610 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/lme/SA_rotd50.0_2020.03.31.csv
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      905 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/modules.yml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)   737944 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nga_w2_selected.csv
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.074842 gmprocess-2.0.0/src/gmprocess/data/nn_clipping/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      409 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_clipping/bias_1.csv
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       26 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_clipping/bias_output.csv
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)       26 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_clipping/masterF.txt
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2032 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_clipping/weight_1.csv
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      408 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_clipping/weight_output.csv
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.042842 gmprocess-2.0.0/src/gmprocess/data/nn_qa/
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.074842 gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8152 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/M.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      304 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/bias_1.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      406 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/bias_2.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       43 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/bias_output.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     5251 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/final_training.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       35 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/masterF.txt
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    11468 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/model_3.txt
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    12981 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/model_5.txt
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      767 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/mu_sigma.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6135 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/weight_1.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6041 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/weight_2.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      791 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/weight_output.csv
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.078842 gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     8171 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/M.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      293 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/bias_1.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      316 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/bias_2.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       42 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/bias_output.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     3569 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/final_training.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)       35 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/masterF.txt
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    10524 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/model_0.txt
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      770 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/mu_sigma.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6037 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/weight_1.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     4418 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/weight_2.csv
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)      596 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/weight_output.csv
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2233 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/picker.yml
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    11182 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/station_coordinates.xlsx
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    79189 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/data/usgs_ids_nga_and_srcmod_cross_reference.xlsx
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.082842 gmprocess-2.0.0/src/gmprocess/io/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/io/__init__.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.082842 gmprocess-2.0.0/src/gmprocess/io/asdf/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/io/asdf/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      374 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/asdf/base_metrics_xml.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2330 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/asdf/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    17731 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/asdf/flatfile.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5882 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/asdf/flatfile_constants.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3319 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/asdf/path_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5005 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/asdf/rupture.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3070 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/asdf/station_metrics_xml.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    40863 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/asdf/stream_workspace.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2514 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/asdf/utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6859 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/asdf/waveform_metrics_xml.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      159 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/asdf/workspace_constants.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.082842 gmprocess-2.0.0/src/gmprocess/io/bhrc/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/io/bhrc/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7799 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/bhrc/core.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.086842 gmprocess-2.0.0/src/gmprocess/io/cosmos/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/io/cosmos/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13199 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/cosmos/cesmd_fetcher.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    17910 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/cosmos/cesmd_search.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    29797 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/cosmos/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    31764 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/cosmos/cosmos_writer.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4117 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/cosmos/data_structures.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.086842 gmprocess-2.0.0/src/gmprocess/io/cwb/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/io/cwb/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9344 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/cwb/core.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.086842 gmprocess-2.0.0/src/gmprocess/io/dmg/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/io/dmg/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    32813 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/dmg/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4084 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/dynamic_search_parameters.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.086842 gmprocess-2.0.0/src/gmprocess/io/esm/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/io/esm/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6496 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/esm/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4023 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/fetcher.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.086842 gmprocess-2.0.0/src/gmprocess/io/geonet/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/io/geonet/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13220 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/geonet/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5717 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/global_fetcher.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.086842 gmprocess-2.0.0/src/gmprocess/io/knet/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/io/knet/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6860 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/knet/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    15161 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/knet/knet_fetcher.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1958 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/nga.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.086842 gmprocess-2.0.0/src/gmprocess/io/nsmn/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/io/nsmn/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6220 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/nsmn/core.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.086842 gmprocess-2.0.0/src/gmprocess/io/obspy/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/io/obspy/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9200 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/obspy/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12629 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/obspy/fdsn_fetcher.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5500 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/read.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2548 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/read_directory.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.086842 gmprocess-2.0.0/src/gmprocess/io/renadic/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/io/renadic/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9262 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/renadic/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10138 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/report.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1988 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/seedname.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.090842 gmprocess-2.0.0/src/gmprocess/io/smc/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/io/smc/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    18244 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/smc/core.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.090842 gmprocess-2.0.0/src/gmprocess/io/unam/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/io/unam/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12493 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/unam/core.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.090842 gmprocess-2.0.0/src/gmprocess/io/usc/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/io/usc/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    17340 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/usc/core.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5749 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/io/utils.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.094842 gmprocess-2.0.0/src/gmprocess/metrics/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/metrics/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2072 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/combine.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4986 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/containers.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      986 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/metric_collection_base.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1661 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/oscillator.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6064 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/reduce.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1253 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/rotate.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      860 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/station_metric.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9895 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/station_metric_collection.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7773 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/transform.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2842 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/utils.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)    11100 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/waveform_metric_calculator.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5132 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/waveform_metric_calculator_component_base.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     9817 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/waveform_metric_collection.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5663 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/waveform_metric_component.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5546 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/waveform_metric_list.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13920 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/metrics/waveform_metric_type.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.098842 gmprocess-2.0.0/src/gmprocess/subcommands/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/subcommands/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      284 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/arg_dicts.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4371 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/assemble.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4607 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/autoprocess.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4288 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/autoshakemap.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5986 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/base.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4788 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/clean.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4223 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/compute_station_metrics.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4794 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/compute_waveform_metrics.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2486 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/download.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4579 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/export_failure_tables.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2133 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/export_gmpacket.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6305 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/export_metric_tables.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2420 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/export_provenance_tables.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2571 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/export_shakemap.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4414 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/generate_regression_plot.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5501 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/generate_report.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2570 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/generate_station_maps.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2215 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/import_data.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1478 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/init.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1406 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/lazy_loader.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     5118 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/process_waveforms.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2884 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/processing_steps.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    16188 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/subcommands/projects.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.102842 gmprocess-2.0.0/src/gmprocess/utils/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/utils/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      757 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/args.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4700 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/assemble_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10714 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/config.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7950 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/config_versioning.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3961 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/constants.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     6102 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/download_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13244 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/export_gmpacket_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13644 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/export_shakemap_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      726 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/ground_motion_models.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3291 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/logging.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      380 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/misc.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12092 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/misc_plots.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2335 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/prompt.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    12759 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/report_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      516 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/rupture_utils.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2622 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/stderr.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1517 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/strec.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    13261 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/summary_plots.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)      797 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/tables.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2482 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/utils/tests_utils.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.106842 gmprocess-2.0.0/src/gmprocess/waveform_processing/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:26:02.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/__init__.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4499 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/adjust_highpass.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3135 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/adjust_highpass_ridder.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1796 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/baseline_correction.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.106842 gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3258 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/clip_detection.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7371 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/clipping_ann.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2401 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/clipping_check.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    14444 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/histogram.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2902 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/jerk.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2626 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/max_amp.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2527 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/ping.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4078 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/std_dev.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10638 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/corner_frequencies.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2319 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/detrend.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3532 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/fft.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     4217 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/filtering.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     8061 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/instrument_response.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1068 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/integrate.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    30903 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/nn_quality_assurance.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    25672 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/phase.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     7131 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/pretesting.py
+-rwxrwxrwx   0 usgs-user   (999) usgs-user   (999)     6775 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/processing.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1187 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/processing_step.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1058 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/resample.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     3311 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/sanity_checks.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    10101 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/snr.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    20372 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/spectrum.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     1555 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/taper.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)    19082 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/windows.py
+-rw-rw-rw-   0 usgs-user   (999) usgs-user   (999)     2028 2024-04-29 13:59:27.000000 gmprocess-2.0.0/src/gmprocess/waveform_processing/zero_crossings.py
+drwxr-xr-x   0 usgs-user   (999) usgs-user   (999)        0 2024-04-29 14:27:44.106842 gmprocess-2.0.0/src/gmprocess.egg-info/
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     6557 2024-04-29 14:27:43.000000 gmprocess-2.0.0/src/gmprocess.egg-info/PKG-INFO
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)     8841 2024-04-29 14:27:44.000000 gmprocess-2.0.0/src/gmprocess.egg-info/SOURCES.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)        1 2024-04-29 14:27:43.000000 gmprocess-2.0.0/src/gmprocess.egg-info/dependency_links.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      374 2024-04-29 14:27:43.000000 gmprocess-2.0.0/src/gmprocess.egg-info/entry_points.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)      889 2024-04-29 14:27:44.000000 gmprocess-2.0.0/src/gmprocess.egg-info/requires.txt
+-rw-r--r--   0 usgs-user   (999) usgs-user   (999)       10 2024-04-29 14:27:44.000000 gmprocess-2.0.0/src/gmprocess.egg-info/top_level.txt
```

### Comparing `gmprocess-1.3.2/LICENSE.md` & `gmprocess-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/PKG-INFO` & `gmprocess-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmprocess
-Version: 1.3.2
+Version: 2.0.0
 Summary: USGS Automated Ground Motion Processing Software
 Author-email: Eric Thompson <emthompsone@usgs.gov>, Mike Hearne <mhearne@usgs.gov>, Brad Aagaard <baagaard@usgs.gov>, Bruce Worden <cbworden@contractor.usgs.gov>, John Rekoske <jrekoske@ucsd.edu>, Heather Hunsinger <hhunsinger@usgs.gov>, Gabe Ferragut <gferragut@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United States
         because it contains materials that originally came from the United States Geological Survey, 
@@ -44,40 +44,41 @@
         to the fullest extent permitted by applicable law. 
         When using or citing the work, you should not imply endorsement by the author or the affirmer.
         
         
         
         [1]: https://creativecommons.org/publicdomain/zero/1.0/legalcode
         
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: beautifulsoup4>=4.11.0
 Requires-Dist: configobj>=5.0.6
 Requires-Dist: esi-core>=1.0.1
 Requires-Dist: esi-utils-colors>1.0
 Requires-Dist: esi-utils-io>1.0
 Requires-Dist: esi-utils-rupture>1.0
 Requires-Dist: folium>=0.12
 Requires-Dist: gmpacket>=0.1.6
 Requires-Dist: h5py>=2.8
 Requires-Dist: lxml>=4.6.1
 Requires-Dist: matplotlib>=3.1.0
+Requires-Dist: numba>=0.58
 Requires-Dist: numpy<2.0,>=1.21
 Requires-Dist: obspy>=1.4.0
 Requires-Dist: openpyxl>=3.0.8
-Requires-Dist: openquake.engine>=3.14
+Requires-Dist: openquake.engine>=3.18
 Requires-Dist: pandas>=1.0
 Requires-Dist: ps2ff>=1.5.2
 Requires-Dist: pyasdf>=0.7
 Requires-Dist: pydantic>=2.0
 Requires-Dist: requests>=2.29
 Requires-Dist: ruamel.yaml>=0.17.16
 Requires-Dist: schema>=0.7
-Requires-Dist: scipy>=1.7
+Requires-Dist: scipy<1.13,>=1.7
 Requires-Dist: setuptools-scm>=6.3.2
 Requires-Dist: statsmodels>=0.12.2
 Requires-Dist: usgs-strec>=2.3.2
 Requires-Dist: xlrd>=2.0
 Provides-Extra: dev
 Requires-Dist: build>=0.7.0; extra == "dev"
 Requires-Dist: black>=21; extra == "dev"
@@ -110,23 +111,28 @@
 # Introduction
 This is a project designed to provide a number of functions related to parsing and processing earthquake ground motion data, building on top of the [ObsPy](https://github.com/obspy/obspy/wiki) library.
 Most of the extensions that we provide are to handle strong motion data and related issues.
 
 
 # Documentation
 - Please note, we are in the process of improving the documentation and that there are some incomplete sections.
-- The full documentation can be viewed locally by running the `doc_source/makedocs.sh` script.
+- The full documentation can be viewed locally by running the `docs/makedocs.sh` script.
 - The documentation is also available [here](https://ghsc.code-pages.usgs.gov/esi/groundmotion-processing/).
+- The MATLAB functions included in the `tools/matlab` directory include a short [tutorial](tools/matlab/readme.md)
 
 # Getting Help
 The developers can be reached at [gmprocess@usgs.gov](mailto:gmprocess@usgs.gov).
 
 If you would like to post an issue to ask a question, request a new feature, or report a bug, you can do so at the [github mirror](https://github.com/DOI-USGS/ghsc-esi-groundmotion-processing) of this repository. 
 
 If you would like to contribute merge requests to this repository, please let us know and we can add you as a collaborator. 
 This will require that you create an account at code.usgs.gov, which is a more involved process than creating a personal account at gitub.com and posting to the issues on the github mirror.
 
-# Reference
-If you wish to cite this software, please use this reference:
+# Suggested Citation
+If you wish to cite this software please cite:
 
-- Hearne, M., E. M. Thompson, H. Schovanec, J. Rekoske, B. T. Aagaard, and C. B. Worden (2019). USGS automated ground motion processing software, USGS Software Release, doi: [10.5066/P9ANQXN3](https://dx.doi.org/10.5066/P9ANQXN3).
+- Thompson, E.M., M. Hearne, B.T. Aagaard, J.M. Rekoske, C.B. Worden, M.P. Moschetti, H.E. Hunsinger, G.C. Ferragut, G.A. Parker, J.A. Smith, K.K. Smith, and A.R. Kottke (2024). USGS Automated Ground Motion Processing Software Version 2, U.S. Geological Survey software release. [https://doi.org/10.5066/P13HMKFJ](https://doi.org/10.5066/P13HMKFJ)
   
+
+# Disclaimer
+
+Any use of trade, firm, or product names is for descriptive purposes only and does not imply endorsement by the U.S. Government.
```

### Comparing `gmprocess-1.3.2/pyproject.toml` & `gmprocess-2.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,41 +9,42 @@
     {name = "Bruce Worden", email="cbworden@contractor.usgs.gov"},
     {name = "John Rekoske", email="jrekoske@ucsd.edu"},
     {name = "Heather Hunsinger", email="hhunsinger@usgs.gov"},
     {name = "Gabe Ferragut", email="gferragut@usgs.gov"},
 ]
 license = {file = "LICENSE.md"}
 readme = "README.md"
-requires-python = ">=3.8,<3.11"
+requires-python = ">=3.9"
 
 # Requirements:
 dependencies = [
     "beautifulsoup4>=4.11.0",
     "configobj>=5.0.6",
     "esi-core>=1.0.1",
     "esi-utils-colors>1.0",
     "esi-utils-io>1.0",
     "esi-utils-rupture>1.0",
     "folium>=0.12",
     "gmpacket>=0.1.6",
     "h5py>=2.8",
     "lxml>=4.6.1",
     "matplotlib>=3.1.0",
+    "numba>=0.58",
     "numpy>=1.21,<2.0",
     "obspy>=1.4.0",
     "openpyxl>=3.0.8",
-    "openquake.engine>=3.14",
+    "openquake.engine>=3.18",
     "pandas>=1.0",
     "ps2ff>=1.5.2",
     "pyasdf>=0.7",
     "pydantic>=2.0",
     "requests>=2.29",
     "ruamel.yaml>=0.17.16",
     "schema>=0.7",
-    "scipy>=1.7",
+    "scipy>=1.7,<1.13",
     "setuptools-scm>=6.3.2",
     "statsmodels>=0.12.2",
     "usgs-strec>=2.3.2",
     "xlrd>=2.0",
 ]
 
 [project.optional-dependencies]
@@ -83,16 +84,17 @@
 
 
 [project.scripts]
 gmconvert = "gmprocess.bin.gmconvert:main"
 gminfo = "gmprocess.bin.gminfo:main"
 gmrecords = "gmprocess.bin.gmrecords:main"
 gmworkspace = "gmprocess.bin.gmworkspace:main"
+gmprocess_config = "gmprocess.bin.gmprocess_config:main"
 list_metrics = "gmprocess.bin.list_metrics:main"
-cwb_gather = "gmprocess.bin.cwb_gather:main"
+cwa_gather = "gmprocess.bin.cwa_gather:main"
 fix_inventory = "gmprocess.bin.fix_inventory:main"
 
 [build-system]
 requires = [
   "setuptools>=42",
   "wheel",
   "setuptools_scm[toml]>=3.4",
```

### Comparing `gmprocess-1.3.2/src/gmprocess/apps/gmrecords.py` & `gmprocess-2.0.0/src/gmprocess/apps/gmrecords.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,24 +275,25 @@
             version="%(prog)s " + VERSION,
             help="Print program version.",
         )
         parser.add_argument(
             "--log",
             type=str,
             default=None,
-            help="Path to log file; if provided, loging is directed to this file.",
+            help="Path to log file; if provided, logging is directed to this file.",
         )
 
         parser.add_argument(
             "-e",
             "--eventid",
             type=str,
+            dest="event_id",
             default=None,
             help=(
-                "Comcat event ID. If None (default) all events in project data "
+                "ComCat event ID. If None (default) all events in project data "
                 "directory will be used. To specify multiple eventids, use a comma "
                 "separated list like "
                 '`gmrecords -e "nc73799091, nc73774300" autoprocess`'
             ),
         )
 
         parser.add_argument(
@@ -300,15 +301,15 @@
             "--textfile",
             type=str,
             default=None,
             help=(
                 "A CSV file without column headers. The columns can be either: "
                 "(1) a single column with ComCat event IDs, or "
                 "(2) six columns in which those columns are: "
-                "id (string, no spaces), time (any ISO standard for date/time), "
+                "event_id (string, no spaces), time (any ISO standard for date/time), "
                 "latitutde (float, decimal degrees), longitude (float, decimal "
                 "degrees), depth (float, km), magnitude (float)."
             ),
         )
 
         parser.add_argument(
             "-l",
```

### Comparing `gmprocess-1.3.2/src/gmprocess/bin/bundle_datarelease.py` & `gmprocess-2.0.0/src/gmprocess/bin/bundle_datarelease.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/bin/fix_inventory.py` & `gmprocess-2.0.0/src/gmprocess/bin/fix_inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                         )
         del ds
 
     def fix_inventories(self):
         ds = pyasdf.ASDFDataSet(self.file)
         for i, waveform in enumerate(ds.waveforms):
             tags = waveform.get_waveform_tags()
-            for tag in tags:
+            for _ in tags:
                 for net in self.inventories[i]:
                     for sta in net.stations:
                         sta.description = ""
         del ds
 
     def delete_stationxml(self):
         h5 = h5py.File(self.file, "r+")
```

### Comparing `gmprocess-1.3.2/src/gmprocess/bin/gmconvert.py` & `gmprocess-2.0.0/src/gmprocess/bin/gmconvert.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/bin/gminfo.py` & `gmprocess-2.0.0/src/gmprocess/bin/gminfo.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/bin/gmworkspace.py` & `gmprocess-2.0.0/src/gmprocess/bin/gmworkspace.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/core/provenance.py` & `gmprocess-2.0.0/src/gmprocess/core/provenance.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     2) Two letter code indicating the type of entity or activity
         (maps to Provenance.ACTIVITIES["code"]) below.
     3) A 7 to 12 letter lowercase alphanumeric hash to ensure uniqueness of ids.
 
 Note that it is important to recognize the difference between the above ID and the
 "prov:id" provenance property, which corresponds to the keys in Provenance.ACTIVITIES.
 """
+
 from abc import ABC, abstractmethod
 import logging
 from datetime import datetime
 import getpass
 import json
 
 import pandas as pd
@@ -114,24 +115,26 @@
         Args:
             prov_dict (dict):
                 Dictionary with keys "prov_id" and "prov_attributes".
         """
         self.provenance_list.append(prov_dict)
 
     @classmethod
-    def from_provenance_document(cls, provdoc, label):
+    def from_provenance_document(cls, provdoc, label, config):
         """Add provenance entires from a provenance document.
 
         Args:
             provdoc (prov.model.ProvDocument):
                 Provenance document.
             label (str):
                 Processing label.
+            config (dict):
+                Dictionary of config options.
         """
-        prov_obj = cls(label)
+        prov_obj = cls(label, config=config)
         prov_obj._from_provenance_document(provdoc)
         return prov_obj
 
     @staticmethod
     def _prov_id_from_property_value(property_value):
         if isinstance(property_value, dict):
             return property_value["$"].split(":")[1]
```

### Comparing `gmprocess-1.3.2/src/gmprocess/core/stationstream.py` & `gmprocess-2.0.0/src/gmprocess/core/stationstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,17 @@
     Comment,
     Response,
     InstrumentSensitivity,
 )
 
 # local imports
 from gmprocess.utils.config import get_config
+from gmprocess.utils import constants
 from .stationtrace import StationTrace
 
-UNITS = {"acc": "cm/s/s", "vel": "cm/s"}
-REVERSE_UNITS = {"cm/s/s": "acc", "cm/s": "vel"}
 
 # Number of samples for Landzos interpolation.
 N_LANCZOS = 20
 
 UNUSED_STANDARD_PARAMS = [
     "instrument_period",
     "instrument_damping",
@@ -433,15 +432,14 @@
         for k in UNUSED_STANDARD_PARAMS:
             if k in self[0].stats.standard:
                 subdict[k] = self[0].stats.standard[k]
 
         format_specific = {}
         if "format_specific" in self[0].stats:
             format_specific = dict(self[0].stats.format_specific)
-
         return {"standard": subdict, "format_specific": format_specific}
 
     def check_stream(self):
         """Check StationStream for being flagged as failed.
 
         The logic of this method is controlled by the "any_trace_failures" config
         parameter in the "check_stream" section:
@@ -468,16 +466,16 @@
             if all(failed_traces):
                 return False
             else:
                 return True
 
 
 def _channel_from_stats(stats):
-    if stats.standard.units_type in UNITS:
-        units = UNITS[stats.standard.units_type]
+    if stats.standard.units_type in constants.UNITS:
+        units = constants.UNITS[stats.standard.units_type]
     else:
         units = ""
     instrument = stats.standard.instrument
     serialnum = stats.standard.sensor_serial_number
     if len(instrument) or len(serialnum):
         equipment = Equipment(type=instrument, serial_number=serialnum)
     else:
```

### Comparing `gmprocess-1.3.2/src/gmprocess/core/stationtrace.py` & `gmprocess-2.0.0/src/gmprocess/core/stationtrace.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,19 @@
 # third party imports
 import numpy as np
 from obspy.core.trace import Trace
 from scipy.integrate import cumtrapz
 
 # local imports
 from gmprocess.utils.config import get_config
+from gmprocess.utils import constants
 from gmprocess.io.cosmos.data_structures import BUILDING_TYPES
 from gmprocess.io.seedname import get_units_type
 from gmprocess.core.provenance import TraceProvenance
 
-UNITS = {"acc": "cm/s^2", "vel": "cm/s"}
-REVERSE_UNITS = {
-    "cm/s^2": "acc",
-    "cm/s**2": "acc",
-    "cm/s/s": "acc",
-    "cm/s": "vel",
-    "cm": "disp",
-}
 
 PROCESS_LEVELS = {
     "V0": "raw counts",
     "V1": "uncorrected physical units",
     "V2": "corrected physical units",
     "V3": "derived time series",
 }
@@ -157,15 +150,15 @@
             # inventory was able to be constructed (e.g., miniseed+StationXML)
             try:
                 seed_id = (
                     f"{header['network']}.{header['station']}.{header['location']}."
                     f"{header['channel']}"
                 )
                 start_time = header["starttime"]
-                (response, standard, coords, format_specific) = _stats_from_inventory(
+                response, standard, coords, format_specific = _stats_from_inventory(
                     data, inventory, seed_id, start_time
                 )
                 header["response"] = response
                 header["coordinates"] = coords
                 header["standard"] = standard
                 header["format_specific"] = format_specific
             except BaseException as err:
@@ -391,42 +384,45 @@
                 "input_units": self.stats.standard.units,
                 "output_units": output_units,
             },
         )
         return self
 
     def integrate(
-        self, frequency=False, initial=0.0, demean=False, taper=False, config=None
+        self,
+        frequency=True,
+        initial=0.0,
+        demean=False,
+        taper=False,
+        taper_width=0.05,
+        taper_type="hann",
+        taper_side="both",
     ):
         """Integrate a StationTrace with respect to either frequency or time.
 
         Args:
             frequency (bool):
                 Determine if we're integrating in frequency domain.
                 If not, integrate in time domain.
             initial (float):
                 Define initial value returned in result.
             demean (bool):
                 Remove mean from array before integrating.
             taper (bool):
-                Taper the ends of entire trace.
-            config (dict):
-                Configuration dictionary (or None). See get_config().
+                Apply a taper.
+            taper_width (float):
+                Taper width.
+            taper_type (float):
+                Taper type.
+            taper_side (float):
+                Taper side.
 
         Returns:
             StationTrace: Input StationTrace is integrated and returned.
         """
-        if config:
-            frequency = config["integration"]["frequency"]
-            initial = config["integration"]["initial"]
-            demean = config["integration"]["demean"]
-            taper = config["integration"]["taper"]["taper"]
-            taper_width = config["integration"]["taper"]["width"]
-            taper_type = config["integration"]["taper"]["type"]
-            taper_side = config["integration"]["taper"]["side"]
 
         if demean:
             self.data -= np.mean(self.data)
             self.set_provenance(
                 "detrend",
                 {
                     "input_units": self.stats.standard.units,
@@ -732,15 +728,15 @@
                 Activity attributes for the given key.
         """
         provdict = {"prov_id": prov_id, "prov_attributes": prov_attributes}
         self.provenance.append(provdict)
         if "output_units" in prov_attributes.keys():
             self.stats.standard.units = prov_attributes["output_units"]
             try:
-                self.stats.standard.units_type = REVERSE_UNITS[
+                self.stats.standard.units_type = constants.REVERSE_UNITS[
                     prov_attributes["output_units"]
                 ]
             except BaseException:
                 self.stats.standard.units_type = "unknown"
 
     def has_parameter(self, param_id):
         """Check to see if Trace contains a given parameter.
@@ -1046,15 +1042,15 @@
         standard["sensor_serial_number"] = ""
         standard["horizontal_orientation"] = float(header["sac"]["cmpaz"])
         # Note: vertical orientatin is defined here as angle from horizontal
         standard["vertical_orientation"] = 90.0 - float(header["sac"]["cmpinc"])
         if "units_type" not in standard or standard["units_type"] == "":
             utype = get_units_type(header["channel"])
             standard["units_type"] = utype
-            standard["units"] = UNITS[utype]
+            standard["units"] = constants.UNIT_TYPES[utype]
         standard["comments"] = ""
         standard["station_name"] = ""
         standard["station_name"] = header["station"]
         format_specific = {
             "conversion_factor": float(config["read"]["sac_conversion_factor"])
         }
         standard["source_format"] = header._format
```

### Comparing `gmprocess-1.3.2/src/gmprocess/core/streamarray.py` & `gmprocess-2.0.0/src/gmprocess/core/streamarray.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,15 +152,15 @@
             if station is not None:
                 if not fnmatch.fnmatch(sta.upper(), station.upper()):
                     continue
             if instrument is not None:
                 if not fnmatch.fnmatch(inst.upper(), instrument.upper()):
                     continue
             sel.append(st)
-        return self.__class__(sel)
+        return self.__class__(sel, config=self.config)
 
     @property
     def n_passed(self):
         n_passed = 0
         for stream in self:
             if stream.passed:
                 n_passed += 1
```

### Comparing `gmprocess-1.3.2/src/gmprocess/core/streamcollection.py` & `gmprocess-2.0.0/src/gmprocess/core/streamcollection.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,17 +123,16 @@
         # If tag exists, it should be consistent across StationStreams
         all_labels = []
         for stream in self:
             if hasattr(stream, "tag"):
                 parts = stream.tag.split("_")
                 if len(parts) > 2:
                     label = parts[-1]
-                    eventid = "_".join(parts[0:-1])
                 else:
-                    eventid, label = stream.tag.split("_")
+                    label = stream.tag.split("_")[-1]
                 all_labels.append(label)
             else:
                 all_labels.append("")
         if len(set(all_labels)) > 1:
             raise ValueError("Only one label allowed within a StreamCollection.")
 
     def select_colocated(
@@ -167,15 +166,15 @@
                     ```
                     dist_thresh = dist[0]
                     for m, d in zip(mag, dist):
                         if eqmag > m:
                             dist_thresh = d
                     ```
 
-            event (gmprocess.utils.event.ScalarEvent):
+            event (gmprocess.core.scalar_event.ScalarEvent):
                 A ScalarEvent object.
         """
         # Do we have different large distnce preference?
         if large_dist is not None and large_dist["enabled"]:
             dist_thresh = large_dist["dist"][0]
             for m, d in zip(large_dist["mag"], large_dist["dist"]):
                 if event.magnitude > m:
@@ -399,29 +398,42 @@
             format_preference (list):
                 A list continaing strings of the file source formats (found
                 in gmprocess.io). Does not need to list all of the formats.
                 Example: ['cosmos', 'dmg'] indicates that cosmos files are
                 preferred over dmg files.
         """
 
-        # If arguments are None, check the config
-        # If not in the config, use the default values at top of the file
+        # Note, that self.config will not exist in some circumstanses, so we need to
+        # provide defaults.
+
         preferences = {
             "max_dist_tolerance": max_dist_tolerance,
             "preference_order": preference_order,
             "process_level_preference": process_level_preference,
             "format_preference": format_preference,
         }
 
-        for key, val in preferences.items():
-            if val is None:
-                if self.config is None:
-                    self.config = get_config()
-                preferences[key] = self.config["duplicate"][key]
-
+        # Set the values from the config if it exists:
+        if hasattr(self, "config") and self.config is not None:
+            for key, val in preferences.items():
+                if val is None:
+                    preferences[key] = self.config["duplicate"][key]
+        else:
+            # Set to defaults:
+            preferences["max_dist_tolerance"] = 500.0
+            preferences["preference_order"] = [
+                "process_level",
+                "source_format",
+                "starttime",
+                "npts",
+                "sampling_rate",
+                "location_code",
+            ]
+            preferences["process_level_preference"] = ["V1", "V0", "V2"]
+            preferences["format_preference"] = ["cosmos", "dmg"]
         stream_params = gather_stream_parameters(self.streams)
 
         traces = []
         for st in self.streams:
             for tr in st:
                 traces.append(tr)
         preferred_traces = []
@@ -715,16 +727,18 @@
         elif pref == "npts":
             tr_prefs = [1 / tr.stats.npts for tr in traces]
         elif pref == "sampling_rate":
             tr_prefs = [1 / tr.stats.sampling_rate for tr in traces]
         elif pref == "location_code":
             sorted_codes = sorted([tr.stats.location for tr in traces])
             tr_prefs = [
-                sorted_codes.index(tr.stats.location)
-                if tr.stats.location != "--"
-                else np.nan
+                (
+                    sorted_codes.index(tr.stats.location)
+                    if tr.stats.location != "--"
+                    else np.nan
+                )
                 for tr in traces
             ]
 
         if len(set(tr_prefs)) != 1:
             return traces[np.nanargmin(tr_prefs)]
     return tr1
```

### Comparing `gmprocess-1.3.2/src/gmprocess/data/CESMD_NGA_ids.csv` & `gmprocess-2.0.0/src/gmprocess/data/CESMD_NGA_ids.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/config_production.yml` & `gmprocess-2.0.0/src/gmprocess/data/config_production_v1.yml`

 * *Files 4% similar despite different names*

```diff
@@ -108,185 +108,185 @@
             # Data from any new station closer to any
             # existing station will not be downloaded.
             minimum_interstation_distance_in_m: 0.0
 
         providers:
             - AUSPASS:
                 bounds:
-                - 103.651901
-                - 151.9907
-                - -44.9425
-                - 1.1267
+                - 103.6
+                - 152.0
+                - -45.0
+                - 1.2
                 url: http://auspass.edu.au
             - BGR:
                 bounds:
-                - -10.3351472
-                - 16.209699999999998
-                - -72.706175
-                - 56.7177
+                - -10.4
+                - 16.2
+                - -72.7
+                - 56.8
                 url: http://eida.bgr.de
             - ETH:
                 bounds:
-                - -88.685139
-                - 93.59834
-                - 9.843528
-                - 52.60745
+                - -88.7
+                - 93.6
+                - 9.8
+                - 52.6
                 url: http://eida.ethz.ch
             - GEONET:
                 bounds:
-                - -180.0
-                - -167.927612069
-                - -46.024042464
-                - -11.80534542
+                - 165.0
+                - -167.9
+                - -46.1
+                - -11.8
                 url: http://service.geonet.org.nz
             - GFZ:
                 bounds:
-                - -176.6116667
-                - 149.1597
-                - -73.6707
-                - 61.9013
+                - -176.6
+                - 149.2
+                - -73.6
+                - 62.0
                 url: http://geofon.gfz-potsdam.de
             - ICGC:
                 bounds:
-                - -17.552500000000002
-                - 5.16244
-                - 26.0718
-                - 44.946905
+                - -17.5
+                - 5.2
+                - 26.0
+                - 45.0
                 url: http://ws.icgc.cat
             - INGV:
                 bounds:
-                - -8.8569
-                - 40.4273
-                - 27.9275
-                - 52.3502
+                - -8.9
+                - 40.5
+                - 27.9
+                - 52.4
                 url: http://webservices.ingv.it
             - IPGP:
                 bounds:
                 - -180.0
-                - 150.996325
-                - -77.1065
-                - 50.216313
+                - 151.0
+                - -77.1
+                - 50.2
                 url: http://ws.ipgp.fr
             - IRIS:
                 bounds:
                 - -180.0
-                - 151.9814
-                - -92.0
-                - 61.9992
+                - 180.0
+                - -90.0
+                - 90.0
                 url: http://service.iris.edu
             - IRISPH5:
                 bounds:
-                - -157.28845
-                - 131.391315
-                - -81.434704
-                - 59.8629
+                - -180.0
+                - 180.0
+                - -90.0
+                - 90.0
                 url: http://service.iris.edu
             - IS:
                 bounds:
                 - 30.0
                 - 43.0
                 - 26.0
                 - 37.5
                 url: https://seis.gsi.gov.il/
             - KNMI:
                 bounds:
-                - -65.24875
-                - 9.119599000000001
-                - 15.4714
-                - 55.5812
+                - -65.2
+                - 9.2
+                - 15.4
+                - 55.6
                 url: http://rdsa.knmi.nl
             - KOERI:
                 bounds:
-                - 23.8987
-                - 46.2384
-                - 33.0157
-                - 44.0195
+                - 23.8
+                - 46.3
+                - 33.0
+                - 44.1
                 url: http://eida.koeri.boun.edu.tr
             - LMU:
                 bounds:
-                - -118.449997
-                - 25.228785
-                - 31.610000999999997
-                - 52.592397
+                - -118.5
+                - 25.3
+                - 31.6
+                - 52.6
                 url: http://erde.geophysik.uni-muenchen.de
             - NCEDC:
                 bounds:
-                - -159.90602
-                - -62.793836
-                - 15.69915
-                - 66.92458
+                - -160.0
+                - -62.7
+                - 15.6
+                - 67.0
             - NIEP:
                 bounds:
-                - -81.0581837
-                - 31.8723
-                - -15.07207207
-                - 52.9305
+                - -81.1
+                - 31.9
+                - -15.1
+                - 53.0
                 url: http://eida-sc3.infp.ro
             - NOA:
                 bounds:
-                - 16.917674
-                - 36.04
-                - 31.0749
-                - 44.8505
+                - 16.9
+                - 36.1
+                - 31.1
+                - 44.9
                 url: http://eida.gein.noa.gr
             - ODC:
                 bounds:
-                - -70.95787
-                - 48.63
-                - -79.875
-                - 61.8576
+                - -71.0
+                - 48.7
+                - -79.9
+                - 61.9
                 url: http://www.orfeus-eu.org
             - ORFEUS:
                 bounds:
-                - -70.95787
-                - 48.63
-                - -79.875
-                - 61.8576
+                - -71.0
+                - 48.7
+                - -79.9
+                - 61.9
                 url: http://www.orfeus-eu.org
             - RESIF:
                 bounds:
                 - -180.0
-                - 150.996325
-                - -77.1065
-                - 54.807
+                - 180.0
+                - -90.0
+                - 90.0
                 url: http://ws.resif.fr
             - RASPISHAKE:
                 bounds:
-                - -178.5268901
-                - 151.8820382
-                - -88.28828829
-                - 61.94594595
+                - -180.0
+                - 180.0
+                - -90.0
+                - 90.0
                 url: https://fdsnws.raspberryshakedata.com
             - SCEDC:
                 bounds:
-                - -159.90602
-                - 74.700264
-                - -35.454085
-                - 60.3877
+                - -160.0
+                - 74.7
+                - -35.5
+                - 60.4
                 url: http://service.scedc.caltech.edu
             - TEXNET:
                 bounds:
-                - -106.985193
-                - -92.17877
-                - 24.57328
-                - 38.44401
+                - -107.0
+                - -92.1
+                - 24.5
+                - 38.5
                 url: http://rtserve.beg.utexas.edu
             - UIB-NORSAR:
                 bounds:
-                - 0.5299999999999998
-                - 19.61
-                - -74.008201
-                - 61.9703
+                - 0.5
+                - 19.7
+                - -74.0
+                - 62.0
                 url: http://eida.geo.uib.no
             - USP:
                 bounds:
-                - -86.11142
-                - 150.996325
-                - -66.7744
-                - 58.4293
+                - -86.2
+                - 151.0
+                - -66.8
+                - 58.5
                 url: http://sismo.iag.usp.br
 
         # authentication:
             # For each of the FDSN providers, a username and password
             # can be provided. This section does not need to contain all of the
             # providers, just the ones you want to give a username and password.
 
@@ -506,16 +506,15 @@
     # Example to always prefer COSMOS files over DMG files
     format_preference: ['cosmos', 'dmg']
 
 
 # -----------------------------------------------------------------------------
 # This is for building a report, with a one-page summary of the data in each
 # StationStream per page. It will write out the latex file, and then look for
-# the `pdflatex` command and attempt to build the pdf. This requires
-# `summary_plots` to have been run.
+# the `pdflatex` command and attempt to build the pdf. 
 build_report:
     enabled: True
     format: latex
 
 # -----------------------------------------------------------------------------
 # This section is for calculating metrics
 metrics:
```

### Comparing `gmprocess-1.3.2/src/gmprocess/data/config_test.yml` & `gmprocess-2.0.0/src/gmprocess/data/config_test.yml`

 * *Files 4% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         #     constant, demean, linear, polynomial, simple, spline
         detrending_method: demean
 
     - compute_snr:
         # Presense of this check says to do the signa-to-noise ratio check. Requires
         # minimum SNR of `threshold` between `min_freq` and `max_freq` using
         # Konno-Omachi smoothed spectra with `bandwidth` parameter.
-        bandwidth: 20.0
+        smoothing_parameter: 20.0
 
     - snr_check:
         # Impose a minimum SNR critera across a frequency band for accepting the record.
         threshold: 3.0
         min_freq: 'f0'  # Either a float or 'f0'. If 'f0', then the Brune
         # corner frequency of the earthquake will be used as the minimum
         # frequency for the SNR check.
@@ -506,85 +506,56 @@
 build_report:
     enabled: True
     format: latex
 
 # -----------------------------------------------------------------------------
 # This section is for calculating metrics
 metrics:
-  # Output IMCs
-  # Valid IMCs: channels, geometric_mean, gmrotd,
-  # greater_of_two_horizontals, rotd
-  output_imcs:
-      - greater_of_two_horizontals
-      - channels
-  # Output IMTs
-  # Valid IMTs: arias, fas, pga, pgv, sa
-  output_imts:
-      - PGA
-      - PGV
-      - SA
-      - duration
-      - sorted_duration
-  # Periods defined for the SA and FAS imts
-  sa:
-      # damping used to calculate the spectral response
-      damping: 0.05
-      # periods for which the spectral response is calculated
-      periods:
-        # Parameters defining an array of periods
-        # syntax is the same as that used for numpy linspace and logspace
-        # start (first value), stop (last value), num (number of values)
-        start: 1.0
-        stop: 3.0
-        num: 3
-        # Valid spacing: linspace, logspace
-        spacing: linspace
-        # Defines whether the above array is used. If False, only the
-        # defined_periods are used
-        use_array: False
-        # Defines a list of user defined periods that are not
-        # predefined by the array of periods
-        defined_periods: [0.3, 1.0, 3.0]
-  fas:
-      smoothing: konno_ohmachi
-      bandwidth: 20.0
-      allow_nans: True
-      periods:
-        # Parameters defining an array of periods
-        # syntax is the same as that used for numpy linspace and logspace
-        # start (first value), stop (last value), num (number of values)
-        start: 1.0
-        stop: 3.0
-        num: 3
-        # Valid spacing: linspace, logspace
-        spacing: linspace
-        # Defines whether the above array is used. If false, only the
-        # defined_periods are used
-        use_array: True
-        # A list of user defined periods that are not
-        # predefined by the array of periods.
-        defined_periods:
-          - 0.3
-  duration:
-      intervals:
-          - 5-75
-          - 5-95
-  # Section for Vs30 calculations. This may contain several keys. Each key
-  # must be unique, and must have the four attributes: file, column_header,
-  # readme_entry, and units.
-  # file: Path to the grid file that can be loaded using MapIO.
-  # column_header: The column header used in the flatfile.
-  # readme_entry: The description used in the README file.
-  # units: Units that will be stored in the StationMetrics XML.
-#   vs30:
-#       example_key:
-#         file: example_file
-#         column_header: example_column_header
-#         readme_entry: example_readme_entry
-#         units: example_units
+  # Specify output IMs (intensity metrics).
+  # Each IM is defined by an IMC (IM component) and a IMT (IM type)
+  # Supported IMCs: channels, geometric_mean, quadratic_mean, rotd
+  # Supported IMT: pga, pgv, sa, duration, sorted_duration, arias, fas
+
+  # The 'components_and_types' section has key-value pairs in which the key is the
+  # metric component and the value is a list of metric types for that component.
+  components_and_types: 
+    channels: [pga, pgv, sa, duration]
+    # rotd: [pga, pgv, sa]
+    # geometric_mean: [duration]
+    # quadratic_mean: [fas]
+
+  component_parameters:
+    rotd:
+       percentiles: [50.0]
+  type_parameters:
+    # Additional parameters required for SA
+    sa:
+        # damping used to calculate the spectral response; if this list includes more than
+        # one value, all periods will be computed for each damping level.
+        damping: [0.05]
+        # periods for which the spectral response is calculated
+        periods: [0.01, 0.1,0.3, 1.0, 3.0, 10.0]
+
+    # Additional parameters required for FAS
+    fas:
+        smoothing_method: konno_ohmachi
+        smoothing_parameter: 20.0
+        allow_nans: True
+        frequencies:
+            # Parameters defining an array of periods
+            # syntax is the same as that used for numpy linspace and logspace
+            # start (first value), stop (last value), num (number of values)
+            start: 0.001
+            stop: 100.0
+            num: 401
+
+    # Additional parameters required for duration
+    duration:
+        intervals: [5-75, 5-95]
+
 # -----------------------------------------------------------------------------
 # This section is for options for integration method
 integration:
     # Frequency or time domain integration?
     frequency: False
     # Assumption for the first value returned in the resulting trace.
     initial: 0.0
@@ -706,7 +677,8 @@
     travel_time:
         # this picker uses travel times using configured velocity model
         # list of models can be found here:
         # https://docs.obspy.org/packages/obspy.taup.html#basic-usage
         model : iasp91
 strec:
     enabled: False
+version: 2
```

### Comparing `gmprocess-1.3.2/src/gmprocess/data/cosmos_table10.xls` & `gmprocess-2.0.0/src/gmprocess/data/cosmos_table10.xls`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/cosmos_table4.xls` & `gmprocess-2.0.0/src/gmprocess/data/cosmos_table4.xls`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/demo/ci38457511/raw/CICCC.RAW` & `gmprocess-2.0.0/src/gmprocess/data/demo/ci38457511/raw/CICCC.RAW`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/demo/ci38457511/raw/CICLC.v1` & `gmprocess-2.0.0/src/gmprocess/data/demo/ci38457511/raw/CICLC.v1`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/demo/ci38457511/raw/CITOW2.RAW` & `gmprocess-2.0.0/src/gmprocess/data/demo/ci38457511/raw/CITOW2.RAW`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/fdsn_codes.csv` & `gmprocess-2.0.0/src/gmprocess/data/fdsn_codes.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/lme/SA_rotd50.0_2020.03.31.csv` & `gmprocess-2.0.0/src/gmprocess/data/lme/SA_rotd50.0_2020.03.31.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/modules.yml` & `gmprocess-2.0.0/src/gmprocess/data/modules.yml`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nga_w2_selected.csv` & `gmprocess-2.0.0/src/gmprocess/data/nga_w2_selected.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_clipping/weight_1.csv` & `gmprocess-2.0.0/src/gmprocess/data/nn_clipping/weight_1.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/M.csv` & `gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/M.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/final_training.csv` & `gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/final_training.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/model_3.txt` & `gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/model_3.txt`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/model_5.txt` & `gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/model_5.txt`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/mu_sigma.csv` & `gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/mu_sigma.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/weight_1.csv` & `gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/weight_1.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/weight_2.csv` & `gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/weight_2.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_qa/Cant/weight_output.csv` & `gmprocess-2.0.0/src/gmprocess/data/nn_qa/Cant/weight_output.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/M.csv` & `gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/M.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/final_training.csv` & `gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/final_training.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/model_0.txt` & `gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/model_0.txt`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/mu_sigma.csv` & `gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/mu_sigma.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/weight_1.csv` & `gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/weight_1.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/weight_2.csv` & `gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/weight_2.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/nn_qa/CantWell/weight_output.csv` & `gmprocess-2.0.0/src/gmprocess/data/nn_qa/CantWell/weight_output.csv`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/picker.yml` & `gmprocess-2.0.0/src/gmprocess/data/picker.yml`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/station_coordinates.xlsx` & `gmprocess-2.0.0/src/gmprocess/data/station_coordinates.xlsx`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/data/usgs_ids_nga_and_srcmod_cross_reference.xlsx` & `gmprocess-2.0.0/src/gmprocess/data/usgs_ids_nga_and_srcmod_cross_reference.xlsx`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/asdf/core.py` & `gmprocess-2.0.0/src/gmprocess/io/asdf/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -67,16 +67,18 @@
     """Write a number of streams (raw or processed) into an ASDF file.
 
     Args:
         filename (str):
             Path to the HDF file that should contain stream data.
         streams (list):
             List of StationStream objects that should be written into the file.
-        event (Obspy Event or dict):
-            Obspy event object or dict (see get_event_dict())
+        event (scalar_event.ScalarEvent):
+            ScalarEvent object
         label (str):
             Label to append to all streams being added to ASDF file.
     """
     workspace = StreamWorkspace(filename)
     workspace.add_config()
+    if not event.id in workspace.get_event_ids():
+        workspace.add_event(event)
     workspace.add_streams(event, streams, label=label, gmprocess_version=VERSION)
     workspace.close()
```

### Comparing `gmprocess-1.3.2/src/gmprocess/io/asdf/flatfile.py` & `gmprocess-2.0.0/src/gmprocess/io/asdf/flatfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 import logging
 
 import pandas as pd
 import numpy as np
 import scipy.interpolate as spint
 from ruamel.yaml import YAML
 
-from gmprocess.utils.config import update_dict, get_config, get_config_imts_imcs
+from gmprocess.utils.config import update_dict, get_config
 from gmprocess.utils import constants
 from gmprocess.io.asdf import flatfile_constants as flat_const
 from gmprocess.metrics.waveform_metric_collection import WaveformMetricCollection
 from gmprocess.metrics.station_metric_collection import StationMetricCollection
+from gmprocess.metrics.utils import component_to_channel
 
 
 class Flatfile(object):
     """Class for creating flatfiles from a StreamWorkspace."""
 
     def __init__(self, workspace, label="default"):
         """Initialize the Flatfile class.
@@ -107,35 +108,35 @@
                     stream_passed = True
                 else:
                     stream_passed = False
             if not stream_passed:
                 continue
 
             wm_df = wml.to_df()
-            imclist = np.unique(wm_df["IMC"]).tolist()
+            self.imclist = list(set(wm_df["IMC"]))
             self.imtlist = np.unique(wm_df["IMT"]).tolist()
             self.imtlist.sort(key=_natural_keys)
 
-            for imc in imclist:
-                if imc not in self.imc_tables:
-                    self.imc_tables[imc] = []
+            for imc in self.imclist:
+                if str(imc) not in self.imc_tables:
+                    self.imc_tables[str(imc)] = []
                 row = self.get_imt_row(passed_traces, wml, imc)
                 if not row:
                     continue
-                self.imc_tables[imc].append(row)
+                self.imc_tables[str(imc)].append(row)
 
     def get_imt_row(self, passed_traces, wml, imc):
         """Get one row of the IMT flatfile fom a stream.
 
         Args:
             passed_traces (list):
                 List dictionaries containing metadata for the passed traces.
             wml (WaveformMetricList):
                 A WaveformMetricList object.
-            imc (str):
+            imc (WaveformMetricComponent):
                 The intensity metric component.
         """
         row = {}
         trace_meta = passed_traces[0]
         event_dict = self.get_event_dict()
         sta_dict = self.get_sta_dict()
         rec_dict = self.get_record_dict(trace_meta)
@@ -144,15 +145,15 @@
         filter_dict = self.get_filter_dict(passed_traces, imc)
         row.update(event_dict)
         row.update(sta_dict)
         row.update(rec_dict)
         row.update(filter_dict)
 
         wm_df = wml.to_df()
-        wm_df = wm_df.loc[wm_df["IMC"] == imc]
+        wm_df = wm_df.loc[wm_df["IMC"] == str(imc)]
         imts = wm_df["IMT"].tolist()
         imt_vals = wm_df["Result"].tolist()
         for imt, val in zip(imts, imt_vals):
             row.update({imt: val})
         return row
 
     def get_record_dict(self, trace_meta):
@@ -205,96 +206,53 @@
             "EarthquakeMagnitude": event_info["magnitude"],
             "EarthquakeMagnitudeType": event_info["magnitude_type"],
         }
 
     def get_filter_dict(self, passed_traces, imc):
         """Get the filter corner frequency dictionary (and also deal with station id).
 
-        This became a very confusion method becuse of the bandaids we had to add to
+        This became a very confusing method becuse of the bandaids we had to add to
         support the "use_array" use-case.
 
         Args:
             passed_traces (list):
-                List dictionaries containing metadata for the passed traces.
-            imc (str):
+                List of dictionaries containing metadata for the passed traces.
+            imc (WaveformMetricComponent):
                 The intensity metric component.
         """
+        # Sort out station id
         tr_met = passed_traces[0]
         base_station_id = ".".join(
             [tr_met["network"], tr_met["station"], tr_met["location"]]
         )
         if tr_met["use_array"]:
             station_id = ".".join([base_station_id, tr_met["channel"]])
         else:
             station_id = ".".join([base_station_id, tr_met["channel"][0:2]])
 
-        if imc.lower() == "channels":
-            if len(passed_traces) > 1:
-                raise ValueError(
-                    "Stream must be length 1 to get row for imc=='channels'."
-                )
-            if not tr_met["passed"]:
-                return {}
-            lpf = tr_met["lowpass_filter"] if "lowpass_filter" in tr_met else np.nan
-            hpf = tr_met["highpass_filter"] if "highpass_filter" in tr_met else np.nan
-            filter_dict = {
-                "Lowpass": lpf,
-                "Highpass": hpf,
-                "StationID": station_id,
-            }
-            station_id = ".".join([base_station_id, tr_met["channel"]])
-        elif imc == "Z":
-            z = [tr_met for tr_met in passed_traces if tr_met["channel"].endswith("Z")]
-            if not z:
-                return {}
-            z = z[0]
-            station_id = ".".join([base_station_id, z["channel"]])
-            if not z["passed"]:
-                return {}
-            lpf = z["lowpass_filter"] if "lowpass_filter" in z else np.nan
-            hpf = z["highpass_filter"] if "highpass_filter" in z else np.nan
-            filter_dict = {
-                "ZLowpass": lpf,
-                "ZHighpass": hpf,
-                "StationID": station_id,
-            }
-        else:
-            h1 = [tr for tr in passed_traces if tr["channel"].endswith("1")]
-            h2 = [tr for tr in passed_traces if tr["channel"].endswith("2")]
-            if not h1:
-                h1 = [tr for tr in passed_traces if tr["channel"].endswith("N")]
-                h2 = [tr for tr in passed_traces if tr["channel"].endswith("E")]
-
-            # Return empty dict if no horizontal channels are found
-            if not h1 or not h2:
-                return {}
-
-            h1 = h1[0]
-            h2 = h2[0]
-
-            # Return empty dict if the stream has not passed for the IMC requested
-            if imc == "H1":
-                if not h1["passed"]:
-                    return {}
-                station_id = ".".join([base_station_id, h1["channel"]])
-            if imc == "H2":
-                if not h2["passed"]:
-                    return {}
-                station_id = ".".join([base_station_id, h1["channel"]])
-            h1lpf = h1["lowpass_filter"] if "lowpass_filter" in h1 else np.nan
-            h1hpf = h1["highpass_filter"] if "highpass_filter" in h1 else np.nan
-            h2lpf = h2["lowpass_filter"] if "lowpass_filter" in h2 else np.nan
-            h2hpf = h2["highpass_filter"] if "highpass_filter" in h2 else np.nan
-            filter_dict = {
-                "H1Lowpass": h1lpf,
-                "H1Highpass": h1hpf,
-                "H2Lowpass": h2lpf,
-                "H2Highpass": h2hpf,
-                "StationID": station_id,
-            }
+        # Deal with channel vs simpler component names
+        channels = [pt["channel"] for pt in passed_traces]
+        _, chan2comp = component_to_channel(channels)
+        components = []
+        for chan in channels:
+            components.append(chan2comp[chan])
+
+        filter_dict = {
+            "StationID": station_id,
+        }
+        for comp, meta in zip(components, passed_traces):
+            lp_key = f"{comp}Lowpass"
+            hp_key = f"{comp}Highpass"
+            filter_dict[lp_key] = (
+                meta["lowpass_filter"] if "lowpass_filter" in meta else np.nan
+            )
+            filter_dict[hp_key] = (
+                meta["highpass_filter"] if "highpass_filter" in meta else np.nan
+            )
+
         return filter_dict
 
     def get_tables(self):
         """Retrieve dataframes containing event information and IMC/IMT metrics.
 
         Returns:
             tuple: Elements are:
@@ -406,17 +364,16 @@
         eventid and label. The second is a README describing each column
         in the first DataFrame.
 
         Returns:
             tuple of pandas DataFrames, which consists of the SNR dataframe and its
             associated readme.
         """
-        imts, _ = get_config_imts_imcs(self.workspace.config)
         periods = np.array(
-            [float(imt.strip("sa")) for imt in imts if imt.startswith("sa")]
+            self.workspace.config["metrics"]["type_parameters"]["sa"]["periods"]
         )
 
         # List that will hold a dictionary for each row of the table
         snr_table = []
 
         event_dict = self.get_event_dict()
```

### Comparing `gmprocess-1.3.2/src/gmprocess/io/asdf/flatfile_constants.py` & `gmprocess-2.0.0/src/gmprocess/io/asdf/flatfile_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,16 @@
     "FAS(X)": (
         f"Fourier amplitude spectrum value ({constants.UNITS['fas']}) at X seconds"
     ),
     "DURATIONp-q": (
         f"p-q percent significant duration ({constants.UNITS['duration']})"
     ),
     "SORTEDDURATION": (f"Sorted significant duration ({constants.UNITS['duration']})"),
-    "ARIASINTENSITY": f"Arias intensity ({constants.UNITS['ariasintensity']})",
+    "ARIAS": f"Arias intensity ({constants.UNITS['arias']})",
+    "CAV": f"Cumulative Absolute Velocity ({constants.UNITS['cav']})",
 }
 
 # List of columns in the fit_spectra_parameters file, along README descriptions
 FIT_SPECTRA_COLUMNS = {
     "EarthquakeId": "Event ID from Comcat",
     "EarthquakeTime": "Earthquake origin time (UTC)",
     "EarthquakeLatitude": "Earthquake latitude (decimal degrees)",
```

### Comparing `gmprocess-1.3.2/src/gmprocess/io/asdf/path_utils.py` & `gmprocess-2.0.0/src/gmprocess/io/asdf/path_utils.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/asdf/rupture.py` & `gmprocess-2.0.0/src/gmprocess/io/asdf/rupture.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,16 @@
                     "depth": 0,
                     "locstring": "",
                     "mag": 0,
                     "time": "",
                 }
             )
 
-        f = open(rupture_file)
-        rupture_json = json.load(f)
+        with open(rupture_file, encoding="utf-8") as fin:
+            rupture_json = json.load(fin)
         reference = rupture_json["metadata"]["reference"]
         description = reference  # for now
 
         rupture = get_rupture(origin_obj, file=rupture_file)
 
         if isinstance(rupture, PointRupture):
             coordinate = rupture_json["features"][0]["geometry"]["coordinates"]
```

### Comparing `gmprocess-1.3.2/src/gmprocess/io/asdf/station_metrics_xml.py` & `gmprocess-2.0.0/src/gmprocess/io/asdf/station_metrics_xml.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/asdf/stream_workspace.py` & `gmprocess-2.0.0/src/gmprocess/io/asdf/stream_workspace.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,41 +16,33 @@
 from obspy.core.utcdatetime import UTCDateTime
 from ruamel.yaml import YAML
 
 from gmprocess.core.stationstream import StationStream
 from gmprocess.core.stationtrace import StationTrace
 from gmprocess.core.streamarray import StreamArray
 from gmprocess.core.streamcollection import StreamCollection
+
 from gmprocess.core import provenance
+from gmprocess.core.scalar_event import ScalarEvent
 from gmprocess.utils import constants
 from gmprocess.utils.config import get_config, update_dict
-from gmprocess.utils.rupture_utils import get_rupture_file
-from gmprocess.utils.event import ScalarEvent
-from gmprocess.utils.strec import STREC
+from gmprocess.utils.config_versioning import get_config_version, config_from_v1
+
 from gmprocess.io.asdf import workspace_constants as wc
-from gmprocess.io.asdf.rupture import Rupture
 from gmprocess.io.asdf.path_utils import (
     get_stream_name,
     get_stream_path,
     get_trace_name,
     get_trace_path,
 )
 
 TIMEFMT_MS = "%Y-%m-%dT%H:%M:%S.%fZ"
 
 VERSION = importlib.metadata.version("gmprocess")
 
-REVERSE_UNITS = {
-    "cm/s^2": "acc",
-    "cm/s**2": "acc",
-    "cm/s/s": "acc",
-    "cm/s": "vel",
-    "cm": "disp",
-}
-
 
 class StreamWorkspace(object):
     """Class for interacting with the ASDF file."""
 
     def __init__(self, filename, compression=None):
         """Create an ASDF file given an Event and list of StationStreams.
 
@@ -62,14 +54,15 @@
         """
         filename = Path(filename)
 
         if filename.is_file():
             self.dataset = pyasdf.ASDFDataSet(filename)
         else:
             self.dataset = pyasdf.ASDFDataSet(filename, compression=compression)
+        self.filename = filename
         self.format_version = wc.FORMAT_VERSION
 
         # Add the config data as workspace attribute if it is present
         group_name = "config/config"
         config_exists = group_name in self.dataset._auxiliary_data_group
         if config_exists:
             self.set_config()
@@ -136,41 +129,125 @@
         return fmt % (nevents, nstations, nstreams)
 
     def add_event(self, event):
         """Add event object to file.
 
         Args:
             event (Event): Obspy event object.
+            strec (dict): STREC results.
         """
-        if self.config["strec"]["enabled"]:
-            self.insert_strec(event)
         self.dataset.add_quakeml(event)
 
-    def insert_strec(self, event):
-        """Insert STREC results into auxiliary data"""
-        workspace_file = self.dataset.filename
-        workspace_path = Path(workspace_file)
-        event_dir = workspace_path.parent.absolute()
-        strec_json = event_dir / "strec_results.json"
-        if strec_json.exists():
-            strec = STREC.from_file(strec_json)
+    def add_rupture(self, rupture, event_id, label):
+        """Inserts information from the rupture model into the workspace.
+
+        Args:
+            event (Event):
+                Obspy event object.
+            label (str):
+                Process label, user can input this from gmrecords assemble subcommand,
+                "default" if no input.
+        """
+        cells = np.array(rupture.cells)
+        vertices = np.array(rupture.vertices)
+        description = rupture.description
+        reference = rupture.reference
+
+        rupture_path = event_id + "_" + label
+
+        self.dataset.add_auxiliary_data(
+            cells,
+            data_type="RuptureModels",
+            path=rupture_path + "/Cells",
+            parameters={},
+        )
+        self.dataset.add_auxiliary_data(
+            vertices,
+            data_type="RuptureModels",
+            path=rupture_path + "/Vertices",
+            parameters={},
+        )
+        self.insert_aux(
+            description,
+            data_name="RuptureModels",
+            path=rupture_path + "/Description",
+        )
+        self.insert_aux(
+            reference, data_name="RuptureModels", path=rupture_path + "/Reference"
+        )
+
+    def get_rupture(self, event_id, label="default"):
+        """Retrieves cells, vertices, description, and reference for a rupture.
+
+        Args:
+            event (Event):
+                Obspy event object.
+            label (str):
+                Process label, "default" if no input.
+        Returns:
+            dict: Keys are cells, vertices, description, and reference.
+
+            Cells and vertices are numpy arrays. The Vertices dataset is
+            a 2D array [#vertices, spaceDim] where spaceDim=3. The Cells
+            dataset is a 2D array [#cells, #corners] where #corners is
+            the number of vertices in a cell. In general, we will have
+            quadrilaterals (#corners=4) or triangles (#corners=3).
+        """
+        aux_data = self.dataset.auxiliary_data
+
+        if "RuptureModels" not in aux_data:
+            return None
+
+        dset_name = f"{event_id}_{label}"
+        if dset_name in aux_data["RuptureModels"]:
+            rupture_model = aux_data["RuptureModels"][dset_name]
         else:
-            strec = STREC.from_event(event)
+            raise ValueError(
+                f"Could not find a rupture model with event id '{event_id}' "
+                f"and label '{label}."
+            )
+
+        cells = rupture_model["Cells"].data
+        cells = np.array(cells)
+
+        vertices = rupture_model["Vertices"].data
+        vertices = np.array(vertices)
+
+        description = array_to_str(rupture_model["Description"].data)
+        reference = array_to_str(rupture_model["Reference"].data)
+
+        rup_dict = {
+            "cells": cells,
+            "vertices": vertices,
+            "description": description,
+            "reference": reference,
+        }
+
+        return rup_dict
+
+    def add_strec(self, strec, event_id):
+        """Add STREC results to auxiliary data.
+
+        Args:
+            strec (dict):
+                STREC results.
+            event_id (str):
+                Event id.
+        """
         strec_params_str = dict_to_str(strec.results)
         dtype = "StrecParameters"
-        strec_path = f"STREC/{event.id}"
+        strec_path = f"STREC/{event_id}"
         self.insert_aux(strec_params_str, dtype, strec_path, True)
 
-    def get_strec(self, event):
+    def get_strec(self, event_id):
         """Get STREC results from auxiliary data"""
-        eventid = event.id.replace("smi:local/", "")
         aux_data = self.dataset.auxiliary_data
         if "StrecParameters" not in aux_data:
             return None
-        jsonstr = array_to_str(aux_data["StrecParameters"]["STREC"][eventid].data[:])
+        jsonstr = array_to_str(aux_data["StrecParameters"]["STREC"][event_id].data[:])
         jdict = json.loads(jsonstr)
         return jdict
 
     def add_config(self, config=None, force=False):
         """Add config to an ASDF dataset and workspace attribute.
 
         Args:
@@ -210,14 +287,17 @@
         if not data_exists:
             logging.error("No config found in auxiliary data.")
         bytelist = self.dataset._auxiliary_data_group[group_name][()].tolist()
 
         # Load config from the workshapce file
         conf_str = "".join([chr(b) for b in bytelist])
         custom_config = json.loads(conf_str)
+        conf_version = get_config_version(custom_config)
+        if conf_version == 1:
+            custom_config = config_from_v1(custom_config)
 
         # Get the default config
         default_config_file = constants.DATA_DIR / constants.CONFIG_FILE_PRODUCTION
         with open(default_config_file, "r", encoding="utf-8") as f:
             yaml = YAML()
             yaml.preserve_quotes = True
             default_config = yaml.load(f)
@@ -289,116 +369,21 @@
                 stats_dict = json.loads(jsonstr)
             else:
                 raise ValueError(f"{stream_path} not in StreamSupplementalStats")
         else:
             raise ValueError(f"{net_sta} not in StreamSupplementalStats")
         return stats_dict
 
-    def add_rupture(self, event, label):
-        """Inserts information from the rupture model into the workspace.
-
-        Args:
-            event (Event):
-                Obspy event object.
-            label (str):
-                Process label, user can input this from gmrecords assemble subcommand,
-                "default" if no input.
-        """
-
-        eventid = self._get_id(event)
-        workspace_file = self.dataset.filename
-        workspace_path = Path(workspace_file)
-        event_dir = workspace_path.parent.absolute()
-        event_dir = str(event_dir)
-
-        rupture_file = get_rupture_file(event_dir)
-
-        if rupture_file is not None:
-            rupture_file = str(rupture_file)
-            rupture_result = Rupture.from_shakemap(rupture_file, event)
-
-            cells = np.array(rupture_result.cells)
-            vertices = np.array(rupture_result.vertices)
-            description = rupture_result.description
-            reference = rupture_result.reference
-
-            rupture_path = eventid + "_" + label
-
-            self.dataset.add_auxiliary_data(
-                cells,
-                data_type="RuptureModels",
-                path=rupture_path + "/Cells",
-                parameters={},
-            )
-            self.dataset.add_auxiliary_data(
-                vertices,
-                data_type="RuptureModels",
-                path=rupture_path + "/Vertices",
-                parameters={},
-            )
-            self.insert_aux(
-                description,
-                data_name="RuptureModels",
-                path=rupture_path + "/Description",
-            )
-            self.insert_aux(
-                reference, data_name="RuptureModels", path=rupture_path + "/Reference"
-            )
-
-    def get_rupture(self, event, label="default"):
-        """Retrieves cells, vertices, description, and reference for a rupture.
-
-        Args:
-            event (Event):
-                Obspy event object.
-            label (str):
-                Process label, "default" if no input.
-        Returns:
-            dict: Keys are cells, vertices, description, and reference.
-
-            Cells and vertices are numpy arrays. The Vertices dataset is
-            a 2D array [#vertices, spaceDim] where spaceDim=3. The Cells
-            dataset is a 2D array [#cells, #corners] where #corners is
-            the number of vertices in a cell. In general, we will have
-            quadrilaterals (#corners=4) or triangles (#corners=3).
-        """
-
-        eventid = self._get_id(event)
-        aux_data = self.dataset.auxiliary_data
-
-        if "RuptureModels" not in aux_data:
-            return None
-
-        try:
-            rupture_model = aux_data["RuptureModels"][eventid + "_" + label]
-        except:
-            raise ValueError(
-                "There does not exist a rupture model with that eventid and label"
-            )
-
-        cells = rupture_model["Cells"].data
-        cells = np.array(cells)
-
-        vertices = rupture_model["Vertices"].data
-        vertices = np.array(vertices)
-
-        description = array_to_str(rupture_model["Description"].data)
-        reference = array_to_str(rupture_model["Reference"].data)
-
-        rup_dict = {
-            "cells": cells,
-            "vertices": vertices,
-            "description": description,
-            "reference": reference,
-        }
-
-        return rup_dict
-
     def add_streams(
-        self, event, streams, label=None, gmprocess_version="unknown", overwrite=False
+        self,
+        event,
+        streams,
+        label=None,
+        gmprocess_version="unknown",
+        overwrite=False,
     ):
         """Add a sequence of StationStream objects to an ASDF file.
 
         Args:
             event (Event):
                 Obspy event object.
             streams (list):
@@ -412,17 +397,15 @@
         """
         if label is not None:
             if "_" in label:
                 raise ValueError("Stream label cannot contain an underscore.")
 
         # To allow for multiple processed versions of the same Stream
         # let's keep a dictionary of stations and sequence number.
-        eventid = self._get_id(event)
-        if not self.has_event(eventid):
-            self.add_event(event)
+        event_id = self._get_id(event)
 
         if hasattr(self, "config"):
             config = self.config
         else:
             config = get_config()
 
         # Level-level provenance entry.
@@ -441,15 +424,15 @@
             # is this a raw file? Check the trace for provenance info.
             is_raw = not stream[0].provenance.ids
 
             if label is None:
                 tfmt = "%Y%m%d%H%M%S"
                 tnow = UTCDateTime.now().strftime(tfmt)
                 label = f"processed{tnow}"
-            tag = f"{eventid}_{label}"
+            tag = f"{event_id}_{label}"
             if is_raw:
                 level = "raw"
             else:
                 level = "processed"
 
             if overwrite:
                 net_sta = stream.get_net_sta()
@@ -529,15 +512,15 @@
             inventory = stream.get_inventory()
             self.dataset.add_stationxml(inventory)
 
     def get_event_ids(self):
         """Return list of event IDs for events in ASDF file.
 
         Returns:
-            list: List of eventid strings.
+            list: List of event_id strings.
         """
         idlist = []
         for event in self.dataset.events:
             eid = event.resource_id.id.replace("smi:local/", "")
             idlist.append(eid)
         return idlist
 
@@ -550,19 +533,19 @@
         all_tags = []
         for w in self.dataset.waveforms:
             all_tags.extend(w.get_waveform_tags())
         all_labels = list(set([at.split("_")[-1] for at in all_tags]))
         labels = list(set(all_labels))
         return labels
 
-    def get_streams(self, eventid, stations=None, labels=None, config=None):
+    def get_streams(self, event_id, stations=None, labels=None, config=None):
         """Get Stream from ASDF file given event id and input tags.
 
         Args:
-            eventid (str):
+            event_id (str):
                 Event ID corresponding to an Event in the workspace.
             stations (list):
                 List of stations (<nework code>.<station code>) to search for.
             labels (list or str):
                 List of processing labels to search for.
             config (dict):
                 Configuration options.
@@ -570,22 +553,14 @@
         Returns:
             StreamCollection: Object containing list of organized
             StationStreams.
         """
         if config is None:
             if hasattr(self, "config"):
                 config = self.config
-                default_config_file = (
-                    constants.DATA_DIR / constants.CONFIG_FILE_PRODUCTION
-                )
-                with open(default_config_file, "r", encoding="utf-8") as f:
-                    yaml = YAML()
-                    yaml.preserve_quotes = True
-                    default_config = yaml.load(f)
-                update_dict(self.config, default_config)
             else:
                 config = get_config()
 
         trace_auxholder = []
         auxdata = self.dataset.auxiliary_data
         streams = []
 
@@ -599,15 +574,15 @@
             all_labels = self.get_labels()
             for label in labels:
                 if label not in all_labels:
                     logging.warning("Label '%s' not found in workspace", label)
 
         net_codes = [st.split(".")[0] for st in stations]
         sta_codes = [st.split(".")[1] for st in stations]
-        tag = [f"{eventid}_{label}" for label in labels]
+        tag = [f"{event_id}_{label}" for label in labels]
 
         for waveform in self.dataset.ifilter(
             self.dataset.q.network == net_codes,
             self.dataset.q.station == sta_codes,
             self.dataset.q.tag == tag,
         ):
             logging.debug(waveform)
@@ -646,17 +621,19 @@
                         )
                         for prov_dict in tmp_doc:
                             trace.provenance.append(prov_dict)
                             prov_attr = prov_dict["prov_attributes"]
                             if "output_units" in prov_attr.keys():
                                 trace.stats.standard.units = prov_attr["output_units"]
                                 try:
-                                    trace.stats.standard.units_type = REVERSE_UNITS[
-                                        prov_attr["output_units"]
-                                    ]
+                                    trace.stats.standard.units_type = (
+                                        constants.REVERSE_UNITS[
+                                            prov_attr["output_units"]
+                                        ]
+                                    )
                                 except BaseException:
                                     trace.stats.standard.units_type = "unknown"
 
                     # get the trace processing parameters
                     if "TraceProcessingParameters" in auxdata:
                         trace_auxholder = auxdata.TraceProcessingParameters
                         if net_sta in trace_auxholder:
@@ -711,17 +688,17 @@
                                     fc_dict = tr_review["corner_frequencies"]
                                     review_dict["corner_frequencies"] = {}
                                     if "highpass" in fc_dict:
                                         review_dict["corner_frequencies"][
                                             "highpass"
                                         ] = fc_dict["highpass"].data[0]
                                     if "lowpass" in fc_dict:
-                                        review_dict["corner_frequencies"][
-                                            "lowpass"
-                                        ] = fc_dict["lowpass"].data[0]
+                                        review_dict["corner_frequencies"]["lowpass"] = (
+                                            fc_dict["lowpass"].data[0]
+                                        )
                                 trace.set_parameter("review", review_dict)
 
                     stream = StationStream(traces=[trace], config=config)
                     stream.tag = tag
 
                     # deal with stream-level data
                     stream_name = get_stream_name(stream, tag, config)
@@ -886,49 +863,49 @@
                     for sta in net2.stations:
                         net1.stations.append(copy.deepcopy(sta))
                 else:
                     inventory.networks.append(copy.deepcopy(net2))
 
         return inventory
 
-    def has_event(self, eventid):
-        """Verify that the workspace file contains an event matching eventid.
+    def has_event(self, event_id):
+        """Verify that the workspace file contains an event matching event_id.
 
         Args:
-            eventid (str):
+            event_id (str):
                 ID of event to search for in ASDF file.
 
         Returns:
             bool: True if event matching ID is found, False if not.
         """
         for event in self.dataset.events:
-            if event.resource_id.id.find(eventid) > -1:
+            if event.resource_id.id.find(event_id) > -1:
                 return True
         return False
 
-    def get_event(self, eventid):
+    def get_event(self, event_id):
         """Get a ScalarEvent object from the ASDF file.
 
         Args:
-            eventid (str):
+            event_id (str):
                 ID of event to search for in ASDF file.
 
         Returns:
             ScalarEvent:
                 Flattened version of Obspy Event object.
         """
-        eventobj = None
+        obspy_event = None
         for event in self.dataset.events:
-            if event.resource_id.id.find(eventid) > -1:
-                eventobj = event
+            if event.resource_id.id.find(event_id) > -1:
+                obspy_event = event
                 break
-        eventobj2 = ScalarEvent.from_event(eventobj) if eventobj else None
-        return eventobj2
+        scalar_event = ScalarEvent.from_obspy(obspy_event) if obspy_event else None
+        return scalar_event
 
-    def get_provenance(self, eventid, stations=None, labels=None):
+    def get_provenance(self, event_id, stations=None, labels=None):
         """Return DataFrame with processing history matching input criteria.
 
                 Output will look like this:
                 Record  Processing Step     Step Attribute              Attribute Value
         0  NZ.HSES.HN1  Remove Response        input_units                       counts
         1  NZ.HSES.HN1  Remove Response       output_units                       cm/s^2
         2  NZ.HSES.HN1          Detrend  detrending_method                       linear
@@ -937,15 +914,15 @@
         5  NZ.HSES.HN1              Cut     new_start_time  2016-11-13T11:02:58.000000Z
         6  NZ.HSES.HN1            Taper               side                         both
         7  NZ.HSES.HN1            Taper        taper_width                         0.05
         8  NZ.HSES.HN1            Taper        window_type                         Hann
         ...
 
                 Args:
-                    eventid (str):
+                    event_id (str):
                         Event ID corresponding to an Event in the workspace.
                     stations (list):
                         List of stations to search for.
                     labels (list):
                         List of processing labels to search for.
 
                 Returns:
```

### Comparing `gmprocess-1.3.2/src/gmprocess/io/asdf/utils.py` & `gmprocess-2.0.0/src/gmprocess/io/asdf/utils.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/asdf/waveform_metrics_xml.py` & `gmprocess-2.0.0/src/gmprocess/metrics/waveform_metric_list.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,123 +1,166 @@
-"""Module for converting waveform metrics dictionaries to XML."""
+"""Module for the WaveormMetricList class."""
 
-from lxml import etree
+import re
 
+import pandas as pd
+
+from gmprocess.metrics.waveform_metric_type import WaveformMetricType
 from gmprocess.utils import constants
-from gmprocess.io.asdf.base_metrics_xml import MetricXML
-from gmprocess.metrics.waveform_metric import WaveformMetric
-from gmprocess.metrics.waveform_metric_list import WaveformMetricList
 
-FLOAT_ATTRIBUTES = ["period", "damping"]
+FLOAT_MATCH = r"[0-9]*\.[0-9]*"
+SA_DEFAULT_DAMPING = 5.0
+FAS_DEFAULT_SMOOTHING = 20.0
+FAS_DEFAULT_METHOD = "Konno-Omachi"
 
 
-class WaveformMetricsXML(MetricXML):
-    """Class for converting a waveform metrics dictionary to/from XML."""
+class WaveformMetricList(object):
+    """A class for holding a list of WaveformMetric instances."""
 
     def __init__(self, metric_list):
-        """Construct a WaveformMetricsXML instance.
-
-        Args:
-            metric_list (list):
-                List of WaveformMetric objects.
-        """
-        if not all(isinstance(wm, WaveformMetric) for wm in metric_list):
+        if not all(isinstance(wm, WaveformMetricType) for wm in metric_list):
             raise TypeError("All elements of metric_list must be a WaveformMetric.")
         self.metric_list = metric_list
 
-    def to_xml(self):
-        """Output the waveform metric in an xml format."""
-        root = etree.Element("waveform_metrics")
-        for wm in self.metric_list:
-            imtstr = wm.type.lower()
-            units = wm.units
-
-            attrs = wm.metric_attributes
-
-            fmt = constants.METRICS_XML_FLOAT_STRING_FORMAT
-
-            attdict = {"units": units}
-
-            for att, atval in attrs.items():
-                if isinstance(atval, str):
-                    attdict[att] = atval
-                else:
-                    attdict[att] = fmt[att] % atval
+    def __iter__(self):
+        return self.metric_list.__iter__()
+
+    def __getitem__(self, i):
+        return self.metric_list[i]
 
-            imt_tag = etree.SubElement(root, imtstr, attrib=attdict)
+    def len(self):
+        return len(self.metric_list)
 
-            for i, imc in enumerate(wm.components):
-                imcstr = imc.lower().replace("(", "").replace(")", "")
-                if wm.component_to_channel and imc in wm.component_to_channel:
-                    attributes = {"original_channel": wm.component_to_channel[imc]}
+    def select(self, mtype=None, **kwargs):
+        """Return a new WaveformMetricList that meets some criteria.
+
+        Args:
+            mtype (str):
+                The metric type to select.
+            **kwargs:
+                Additional critera to be applied to the metric's 'metric_attributes'.
+        """
+        selected = []
+        for metric in self:
+            if mtype is None or metric.type != mtype:
+                continue
+            att_match = []
+            for k, v in kwargs.items():
+                if k not in metric.metric_attributes:
+                    att_match.append(False)
+                    continue
+                if metric.metric_attributes[k] != v:
+                    att_match.append(False)
                 else:
-                    attributes = {}
-                imc_tag = etree.SubElement(imt_tag, imcstr, attrib=attributes)
-                imc_tag.text = fmt[wm.format_type] % wm.value(imc)
-        return etree.tostring(root, encoding="unicode")
+                    att_match.append(True)
+            if all(att_match):
+                selected.append(metric)
+        return WaveformMetricList(selected)
+
+    @property
+    def metric_types(self):
+        mtypes = []
+        for metric in self:
+            mtypes.append(metric.type)
+        return mtypes
+
+    def __repr__(self):
+        wmstring = ""
+        n_metrics = len(self.metric_list)
+        wmstring += f"{n_metrics} metric(s) in list:\n"
+        if n_metrics <= 5:
+            for m in self.metric_list:
+                wmstring += f"  {m}\n"
+        else:
+            for m in self.metric_list[0:2]:
+                wmstring += f"  {m}\n"
+            wmstring += "  ...\n"
+            for m in self.metric_list[-1:]:
+                wmstring += f"  {m}\n"
+        return wmstring
+
+    def to_df(self):
+        """Output the WaveformMetricList in a pandas dataframe format."""
+        values = []
+        imcs = []
+        imts = []
+        for metric in self:
+            mdict = metric.to_dict()
+
+            for comp, val in zip(mdict["components"], mdict["values"]):
+                values.append(val)
+                imcs.append(str(comp))
+                imts.append(metric.identifier)
+
+        dataframe = pd.DataFrame(
+            {
+                "IMC": imcs,
+                "IMT": imts,
+                "Result": values,
+            }
+        )
+        return dataframe
 
     @classmethod
-    def from_xml(cls, xml_str):
-        """Construct a WaveformMetricList object from xml.
+    def from_df(cls, dataframe, component_to_channel=None):
+        """Construct a WaveformMetricList object from a pandas dataframe.
 
         Args:
-            xml_str (str):
-                XML string.
-
-        Returns:
-            WaveformMetricList
+            dataframe (str):
+                The pandas dataframe created by the MetricsController.
+            component_to_channel (dict):
+                Optional dictionary mapping the simplified component names to the
+                as-recorded channel names.
         """
-        root = etree.fromstring(xml_str)
+        imtlist = dataframe["IMT"].unique().tolist()
         metric_list = []
-        for element in root.getchildren():
-            etag = element.tag
-            units = element.attrib["units"]
-            element.attrib.pop("units")
-            comp_to_chan = {}
-            mvalues = []
-            mcomps = []
-            for imc_element in element.getchildren():
-                imc = imc_element.tag.upper()
-                if imc in ["H1", "H2", "Z"]:
-                    if "original_channel" in imc_element.attrib:
-                        comp_to_chan[imc] = imc_element.attrib["original_channel"]
-                mcomps.append(imc)
-                mvalues.append(float(imc_element.text))
-
-            att_dict = dict(element.attrib)
-            for aname, aval in att_dict.items():
-                if aname in FLOAT_ATTRIBUTES:
-                    att_dict[aname] = float(aval)
-
+        for imt in imtlist:
+            temp_df = dataframe.loc[dataframe["IMT"] == imt]
+            imt = imt.lower()
+            if imt.startswith("sa"):
+                metric_attributes = {
+                    "period": float(re.search(FLOAT_MATCH, imt).group()),
+                    "damping": SA_DEFAULT_DAMPING,
+                }
+                fixed_imt = "SA"
+            elif imt.startswith("fas"):
+                metric_attributes = {
+                    "period": float(re.search(FLOAT_MATCH, imt).group()),
+                    "method": FAS_DEFAULT_METHOD,
+                    "smoothing": FAS_DEFAULT_SMOOTHING,
+                }
+                fixed_imt = "FAS"
+            elif imt.startswith("duration"):
+                metric_attributes = {
+                    "interval": imt.replace("duration", ""),
+                }
+                fixed_imt = "Duration"
+            elif imt.startswith("cav"):
+                metric_attributes = {}
+                fixed_imt = "CAV"
+            elif imt.startswith("arias"):
+                metric_attributes = {}
+                fixed_imt = "Arias"
+            elif imt.startswith("sorted"):
+                metric_attributes = {}
+                fixed_imt = "SortedDuration"
+            else:
+                metric_attributes = {}
+                fixed_imt = imt.upper()
+            units = constants.UNITS[fixed_imt.lower()]
+            vals = []
+            comps = []
+            for imc, val in zip(temp_df["IMC"], temp_df["Result"]):
+                comps.append(imc)
+                vals.append(val)
             mdict = {
-                "values": mvalues,
-                "components": mcomps,
-                "type": etag2type(etag),
+                "values": vals,
+                "components": comps,
+                "type": fixed_imt,
                 "format_type": "",
                 "units": units,
-                "metric_attributes": att_dict,
-                "component_to_channel": comp_to_chan,
+                "metric_attributes": metric_attributes,
+                "component_to_channel": component_to_channel,
             }
-            metric_list.append(WaveformMetric.metric_from_dict(mdict))
-        return WaveformMetricList(metric_list)
-
-
-def etag2type(etag):
-    """Convenience method for converting etag to type.
-
-    Probably need a better system for this. Also note that we do something similar
-    in the WaveformMetricList class.
-    """
-    etag = etag.lower()
-    if etag.startswith("sa"):
-        etag_type = "SA"
-    elif etag.startswith("fas"):
-        etag_type = "FAS"
-    elif etag.startswith("duration"):
-        etag_type = "Duration"
-    elif etag.startswith("sorted"):
-        etag_type = "SortedDuration"
-    elif etag.startswith("arias"):
-        etag_type = "AriasIntensity"
-    else:
-        etag_type = etag.upper()
-    return etag_type
+            wm = WaveformMetricType.metric_from_dict(mdict)
+            metric_list.append(wm)
+        return cls(metric_list)
```

### Comparing `gmprocess-1.3.2/src/gmprocess/io/bhrc/core.py` & `gmprocess-2.0.0/src/gmprocess/io/bhrc/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/cosmos/cesmd_fetcher.py` & `gmprocess-2.0.0/src/gmprocess/io/cosmos/cesmd_fetcher.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/cosmos/cesmd_search.py` & `gmprocess-2.0.0/src/gmprocess/io/cosmos/cesmd_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,15 +491,15 @@
                     )
                     print(fmt % (member, str(e)))
                     continue
 
         myzip.close()
 
         datafiles = []
-        for root, fdir, files in os.walk(output):
+        for root, _, files in os.walk(output):
             for tfile in files:
                 if not tfile.endswith(".json"):
                     datafile = os.path.join(root, tfile)
                     datafiles.append(datafile)
 
         return (os.path.abspath(output), datafiles)
     else:
```

### Comparing `gmprocess-1.3.2/src/gmprocess/io/cosmos/core.py` & `gmprocess-2.0.0/src/gmprocess/io/cosmos/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -148,15 +148,14 @@
             Path to possible COSMOS V0/V1 data file.
         config (dict):
             Dictionary containing configuration.
 
     Returns:
         bool: True if COSMOS V0/V1, False otherwise.
     """
-    logging.debug("Checking if format is cosmos.")
     if is_binary(filename):
         return False
     try:
         line = open(filename, "rt", encoding="utf-8").readline()
         for marker in VALID_MARKERS:
             if line.lower().find(marker.lower()) >= 0:
                 if line.lower().find("(format v") >= 0:
@@ -183,15 +182,14 @@
                 station type codes.
             Other arguments will be ignored.
 
     Returns:
         list: List of StationStreams containing three channels of acceleration
         data (cm/s**2).
     """
-    logging.debug("Starting read_cosmos.")
     if not is_cosmos(filename, config):
         raise Exception(f"{filename} is not a valid COSMOS strong motion data file.")
     # get list of valid stations
     valid_station_types = kwargs.get("valid_station_types", None)
     # get list of valid stations
     location = kwargs.get("location", "")
 
@@ -274,15 +272,14 @@
         hdr["duration"] = (hdr["npts"] - 1) * hdr["delta"]
 
     # check units
     unit = hdr["format_specific"]["physical_units"]
     hdr["standard"]["units"] = unit
     if unit in UNIT_CONVERSIONS:
         data *= UNIT_CONVERSIONS[unit]
-        logging.debug(f"Data converted from {unit} to cm/s/s")
     else:
         if unit != "counts":
             raise ValueError(f"COSMOS: {unit} is not a supported unit.")
 
     if hdr["standard"]["units_type"] != "acc":
         raise ValueError("COSMOS: Only acceleration data accepted.")
 
@@ -371,79 +368,89 @@
     Returns:
         dictionary: Dictionary of header/metadata information
     """
     hdr = {}
     coordinates = {}
     standard = {}
     format_specific = {}
+
     # Get unknown parameter number
     try:
-        unknown = int(lines[12][64:71])
+        unknown_int = int(lines[12][64:71])
+    except ValueError:
+        unknown_int = -999
+    try:
+        unknown_flt = float(lines[12][72:80])
     except ValueError:
-        unknown = -999
-    # required metadata
-    network_num = int(int_data[10])
+        unknown_flt = -999.0
+
     # Get network from cosmos table or fdsn code sheet
-    if network_num in COSMOS_NETWORKS:
-        network = COSMOS_NETWORKS[network_num][0]
-        source = COSMOS_NETWORKS[network_num][1]
+    if int_data[10] == unknown_int:
+        network = "--"
+        source = ""
+    elif int_data[10] in COSMOS_NETWORKS:
+        network = COSMOS_NETWORKS[int_data[10]][0]
+        source = COSMOS_NETWORKS[int_data[10]][1]
         if network == "":
-            network = COSMOS_NETWORKS[network_num][2]
+            network = COSMOS_NETWORKS[int_data[10]][2]
     else:
         network_code = lines[4][25:27].upper()
         if network_code in CODES:
             network = network_code
             idx = np.argwhere(CODES == network_code)[0][0]
             source = (
                 SOURCES1[idx].decode("utf-8") + ", " + SOURCES2[idx].decode("utf-8")
             )
         else:
             network = "--"
             source = ""
     hdr["network"] = network
-    logging.debug(f"network: {network}")
     hdr["station"] = lines[4][28:34].strip()
-    logging.debug(f"station: {hdr['station']}")
 
     # the channel orientation can be either relative to true north (idx 53)
     # or relative to sensor orientation (idx 54).
-    horizontal_angle = int(int_data[53])
-    logging.debug(f"horizontal_angle: {horizontal_angle}")
+    if int_data[53] != unknown_int:
+        horizontal_angle = int(int_data[53])
+    else:
+        horizontal_angle = np.nan
+
     if horizontal_angle not in VALID_AZIMUTH_INTS:
-        angles = np.array(int_data[19:21]).astype(np.float32)
-        angles[angles == unknown] = np.nan
-        if np.isnan(angles).all():
-            logging.warning("Horizontal_angle in COSMOS header is not valid.")
-        else:
-            ref = angles[~np.isnan(angles)][0]
+        angles_int = int_data[19:21]
+        angles_float = angles_int.astype(np.float32)
+        angles_float[angles_int == unknown_int] = np.nan
+        if np.any(~np.isnan(angles_float)):
+            ref = angles_float[~np.isnan(angles_float)][0]
             horizontal_angle = int(int_data[54])
             if horizontal_angle not in VALID_AZIMUTH_INTS:
-                logging.warning("Horizontal_angle in COSMOS header is not valid.")
+                raise ValueError("Horizontal_angle in COSMOS header is not valid.")
             else:
                 horizontal_angle += ref
                 if horizontal_angle > 360:
                     horizontal_angle -= 360
 
     horizontal_angle = float(horizontal_angle)
 
     # Store delta and duration. Use them to calculate npts and sampling_rate
 
     # NOTE: flt_data[33] is the delta of the V0 format, and if we are reading
     # a V1 or V2 format then it may have been resampled. We should consider
     # adding flt_data[33] delta to the provenance record at some point.
 
-    delta = float(flt_data[61]) * MSEC_TO_SEC
-    if delta != unknown:
+    if flt_data[61] != unknown_flt:
+        delta = float(flt_data[61]) * MSEC_TO_SEC
         hdr["delta"] = delta
         hdr["sampling_rate"] = 1 / delta
+    else:
+        hdr["delta"] = np.nan
+        hdr["sampling_rate"] = np.nan
 
     # Determine the angle based upon the cosmos table
     # Set horizontal angles other than N,S,E,W to H1 and H2
     # Missing angle results in the channel number
-    if horizontal_angle != unknown:
+    if not np.isnan(horizontal_angle):
         if horizontal_angle in COSMOS_ORIENTATIONS:
             channel = COSMOS_ORIENTATIONS[horizontal_angle][1].upper()
             if channel == "UP" or channel == "DOWN" or channel == "VERT":
                 channel = get_channel_name(
                     hdr["sampling_rate"],
                     is_acceleration=True,
                     is_vertical=True,
@@ -490,88 +497,110 @@
                 )
         horizontal_orientation = horizontal_angle
     else:
         errstr = (
             "Not enough information to distinguish horizontal from "
             "vertical channels."
         )
-        raise BaseException("COSMOS: " + errstr)
+        raise ValueError("COSMOS: " + errstr)
     hdr["channel"] = channel
-    logging.debug(f"channel: {hdr['channel']}")
-    if location == "":
-        location = int(int_data[55])
-        location = str(_check_assign(location, unknown, "--"))
+    if location:
+        hdr["location"] = location
+    else:
+        if int_data[55] != unknown_int:
+            location = str(int(int_data[55]))
+        else:
+            location = "--"
         if len(location) < 2:
             location = location.zfill(2)
         hdr["location"] = location
+
+    if int_data[39] != unknown_int:
+        year = int_data[39]
     else:
-        hdr["location"] = location
-    year = int(int_data[39])
-    month = int(int_data[41])
-    day = int(int_data[42])
-    hour = int(int_data[43])
-    minute = int(int_data[44])
-    second = float(flt_data[29])
-    # If anything more than seconds is excluded
-    # It is considered inadequate time information
-    if second == unknown:
+        year = np.nan
+    if int_data[41] != unknown_int:
+        month = int_data[41]
+    else:
+        month = np.nan
+    if int_data[42] != unknown_int:
+        day = int_data[42]
+    else:
+        day = np.nan
+    if int_data[43] != unknown_int:
+        hour = int_data[43]
+    else:
+        hour = np.nan
+    if int_data[44] != unknown_int:
+        minute = int(int_data[44])
+    else:
+        minute = np.nan
+    if flt_data[29] != unknown_flt:
+        second = float(flt_data[29])
+    else:
+        second = np.nan
+
+    # Inadequate time information if anything more than seconds is excluded
+    if np.isnan(second):
         try:
             hdr["starttime"] = datetime(year, month, day, hour, minute)
         except BaseException:
-            raise BaseException("COSMOS: Inadequate start time information.")
+            raise ValueError("COSMOS: Inadequate start time information.")
     else:
-        second = second
         microsecond = int((second - int(second)) * 1e6)
         try:
             hdr["starttime"] = datetime(
                 year, month, day, hour, minute, int(second), microsecond
             )
         except BaseException:
-            raise BaseException("COSMOS: Inadequate start time information.")
+            raise ValueError("COSMOS: Inadequate start time information.")
 
-    if flt_data[62] != unknown:
+    if flt_data[62] != unknown_flt:
         # COSMOS **defines** "length" as npts*dt (note this is a bit unusual)
         cosmos_length = flt_data[62]
         npts = int(cosmos_length / delta)
         hdr["duration"] = (npts - 1) * delta
         hdr["npts"] = npts
     else:
         raise ValueError("COSMOS file does not specify length.")
 
     # coordinate information
-    coordinates["latitude"] = float(flt_data[0])
-    coordinates["longitude"] = float(flt_data[1])
-    coordinates["elevation"] = float(flt_data[2])
-    for key in coordinates:
-        if coordinates[key] == unknown:
-            if key != "elevation":
-                # logging.warning(f"Missing {key!r}. Setting to np.nan.", Warning)
-                coordinates[key] = np.nan
-            else:
-                # logging.warning(f"Missing {key!r}. Setting to 0.0.", Warning)
-                coordinates[key] = 0.0
+    if flt_data[0] != unknown_flt:
+        coordinates["latitude"] = float(flt_data[0])
+    else:
+        raise ValueError("Latitude is unknown.")
+    if flt_data[1] != unknown_flt:
+        coordinates["longitude"] = float(flt_data[1])
+    else:
+        raise ValueError("Longitude is unknown.")
+    if flt_data[2] != unknown_flt:
+        coordinates["elevation"] = float(flt_data[2])
+    else:
+        coordinates["elevation"] = 0.0
+        logging.warning("Missing elevation. Setting to 0.0.")
 
     hdr["coordinates"] = coordinates
 
     # standard metadata
     standard["units_type"] = get_units_type(channel)
     standard["source"] = source
     standard["horizontal_orientation"] = horizontal_orientation
     standard["vertical_orientation"] = np.nan
-    station_name = lines[4][40:-1].strip()
-    standard["station_name"] = station_name
-    instrument_frequency = float(flt_data[39])
-    if instrument_frequency == 0:
-        standard["instrument_period"] = np.nan
-        logging.warning("Instrument Frequency == 0")
-    else:
-        inst_freq = _check_assign(instrument_frequency, unknown, np.nan)
-        standard["instrument_period"] = 1.0 / inst_freq
-    instrument_damping = float(flt_data[40])
-    standard["instrument_damping"] = _check_assign(instrument_damping, unknown, np.nan)
+    standard["station_name"] = lines[4][40:-1].strip()
+
+    if flt_data[39] != unknown_flt:
+        instrument_frequency = float(flt_data[39])
+    else:
+        instrument_frequency = np.nan
+    standard["instrument_period"] = 1.0 / instrument_frequency
+    if flt_data[40] != unknown_flt:
+        standard["instrument_damping"] = float(flt_data[40])
+    else:
+        standard["instrument_damping"] = np.nan
+
     process_line = lines[10][10:40]
     if process_line.find("-") >= 0 or process_line.find("/") >= 0:
         if process_line.find("-") >= 0:
             delimeter = "-"
         elif process_line.find("/") >= 0:
             delimeter = "/"
         try:
@@ -586,126 +615,182 @@
             microsecond = int((second - int(second)) * 1e6)
             etime = datetime(year, month, day, hour, minute, int(second), microsecond)
             standard["process_time"] = etime.strftime(TIMEFMT)
         except BaseException:
             standard["process_time"] = ""
     else:
         standard["process_time"] = ""
-    process_level = int(int_data[0])
+
+    if int_data[0] != unknown_int:
+        process_level = int(int_data[0])
+    else:
+        raise ValueError("Unknown process level.")
     if process_level == 0:
         standard["process_level"] = PROCESS_LEVELS["V0"]
     elif process_level == 1:
         standard["process_level"] = PROCESS_LEVELS["V1"]
     elif process_level == 2:
         standard["process_level"] = PROCESS_LEVELS["V2"]
     elif process_level == 3:
         standard["process_level"] = PROCESS_LEVELS["V3"]
     else:
         standard["process_level"] = PROCESS_LEVELS["V1"]
-    logging.debug(f"process_level: {process_level}")
-    serial = int(int_data[52])
-    if serial != unknown:
-        standard["sensor_serial_number"] = str(_check_assign(serial, unknown, ""))
+
+    if int_data[52] != unknown_int:
+        standard["sensor_serial_number"] = str(int_data[52])
     else:
         standard["sensor_serial_number"] = ""
-    instrument = int(int_data[51])
-    if instrument != unknown and instrument in SENSOR_TYPES:
-        standard["instrument"] = SENSOR_TYPES[instrument]
+
+    if int_data[51] != unknown_int:
+        instrument = int(int_data[51])
+        if instrument in SENSOR_TYPES:
+            standard["instrument"] = SENSOR_TYPES[instrument]
+        else:
+            standard["instrument"] = lines[6][57:-1].strip()
     else:
         standard["instrument"] = lines[6][57:-1].strip()
-    structure_type = int(int_data[18])
-    if structure_type != unknown and structure_type in BUILDING_TYPES:
-        standard["structure_type"] = BUILDING_TYPES[structure_type]
+
+    if int_data[18] != unknown_int:
+        structure_type_code = int(int_data[18])
+    else:
+        structure_type_code = np.nan
+    if structure_type_code in BUILDING_TYPES:
+        standard["structure_type"] = BUILDING_TYPES[structure_type_code]
     else:
         standard["structure_type"] = ""
-    frequency = float(flt_data[25])
-    standard["corner_frequency"] = _check_assign(frequency, unknown, np.nan)
-    physical_parameter = int(int_data[2])
-    units = int(int_data[1])
-    if units != unknown and units in UNITS:
-        standard["units_type"] = UNITS[units]
+
+    if flt_data[25] != unknown_flt:
+        standard["corner_frequency"] = flt_data[25]
+    else:
+        standard["corner_frequency"] = np.nan
+
+    if int_data[2] != unknown_int:
+        physical_parameter = int_data[2]
+    else:
+        physical_parameter = np.nan
+
+    if int_data[1] != unknown_int:
+        unit_code = int_data[1]
+    else:
+        unit_code = np.nan
+
+    if unit_code in UNITS:
+        standard["units_type"] = UNITS[unit_code]
     else:
         if physical_parameter in [2, 4, 7, 10, 11, 12, 23]:
             standard["units_type"] = "acc"
         elif physical_parameter in [5, 8, 24]:
             standard["units_type"] = "vel"
         elif physical_parameter in [6, 9, 25]:
             standard["units_type"] = "disp"
+
     standard["source_format"] = "cosmos"
+
     standard["comments"] = ", ".join(cmt_data)
+
     # get undocumented SCNL code if it is present because location code doesn't seem to
     # be reported in the header.
     if "<SCNL>" in standard["comments"]:
-        scnl = re.search("<SCNL>(.*?)(?=\s)", standard["comments"]).group(1)
+        scnl = re.search("<SCNL>(.*?)(?=\s)", standard["comments"]).group(1)  # noqa
         # Do not use channel from here because we got it from orientation info
         # previously
         hdr["station"], _, hdr["network"], hdr["location"] = scnl.split(".")
 
     # format specific metadata
     if physical_parameter in PHYSICAL_UNITS:
         physical_parameter = PHYSICAL_UNITS[physical_parameter][0]
     format_specific["physical_units"] = physical_parameter
-    v30 = float(flt_data[3])
-    format_specific["v30"] = _check_assign(v30, unknown, np.nan)
-    least_significant_bit = float(flt_data[21])
-    format_specific["least_significant_bit"] = _check_assign(
-        least_significant_bit, unknown, np.nan
-    )
-    gain = float(flt_data[46])
-    format_specific["gain"] = _check_assign(gain, unknown, np.nan)
-    low_filter_type = int(int_data[60])
-    if low_filter_type in FILTERS:
-        format_specific["low_filter_type"] = FILTERS[low_filter_type]
+
+    if flt_data[3] != unknown_flt:
+        format_specific["v30"] = float(flt_data[3])
+    else:
+        format_specific["v30"] = np.nan
+
+    if flt_data[21] != unknown_flt:
+        format_specific["least_significant_bit"] = float(flt_data[21])
+    else:
+        format_specific["least_significant_bit"] = np.nan
+
+    if flt_data[46] != unknown_flt:
+        format_specific["gain"] = float(flt_data[46])
+    else:
+        format_specific["gain"] = np.nan
+
+    if int_data[60] != unknown_int:
+        low_filter_type = int(int_data[60])
+        if low_filter_type in FILTERS:
+            format_specific["low_filter_type"] = FILTERS[low_filter_type]
+        else:
+            format_specific["low_filter_type"] = ""
     else:
         format_specific["low_filter_type"] = ""
-    low_filter_corner = float(flt_data[53])
-    format_specific["low_filter_corner"] = _check_assign(
-        low_filter_corner, unknown, np.nan
-    )
-    low_filter_decay = float(flt_data[54])
-    format_specific["low_filter_decay"] = _check_assign(
-        low_filter_decay, unknown, np.nan
-    )
-    high_filter_type = int(int_data[61])
-    if high_filter_type in FILTERS:
-        format_specific["high_filter_type"] = FILTERS[high_filter_type]
+
+    if flt_data[53] != unknown_flt:
+        format_specific["low_filter_corner"] = float(flt_data[53])
+    else:
+        format_specific["low_filter_corner"] = np.nan
+
+    if flt_data[54] != unknown_flt:
+        format_specific["low_filter_decay"] = float(flt_data[54])
+    else:
+        format_specific["low_filter_decay"] = np.nan
+
+    if int_data[61] != unknown_int:
+        high_filter_type = int(int_data[61])
+        if high_filter_type in FILTERS:
+            format_specific["high_filter_type"] = FILTERS[high_filter_type]
+        else:
+            format_specific["high_filter_type"] = ""
     else:
         format_specific["high_filter_type"] = ""
-    high_filter_corner = float(flt_data[56])
-    format_specific["high_filter_corner"] = _check_assign(
-        high_filter_corner, unknown, np.nan
-    )
-    high_filter_decay = float(flt_data[57])
-    format_specific["high_filter_decay"] = _check_assign(
-        high_filter_decay, unknown, np.nan
-    )
-    maximum = float(flt_data[63])
-    format_specific["maximum"] = _check_assign(maximum, unknown, np.nan)
-    maximum_time = float(flt_data[64])
-    format_specific["maximum_time"] = _check_assign(maximum_time, unknown, np.nan)
-    format_specific["station_code"] = _check_assign(structure_type, unknown, np.nan)
+
+    if flt_data[56] != unknown_flt:
+        format_specific["high_filter_corner"] = float(flt_data[56])
+    else:
+        format_specific["high_filter_corner"] = np.nan
+
+    if flt_data[57] != unknown_flt:
+        format_specific["high_filter_decay"] = float(flt_data[57])
+    else:
+        format_specific["high_filter_decay"] = np.nan
+
+    if flt_data[63] != unknown_flt:
+        format_specific["maximum"] = float(flt_data[63])
+    else:
+        format_specific["maximum"] = np.nan
+
+    if flt_data[64] != unknown_flt:
+        format_specific["maximum_time"] = float(flt_data[64])
+    else:
+        format_specific["maximum_time"] = np.nan
+
+    format_specific["station_code"] = structure_type_code
+
     record_flag = int(int_data[75])
     if record_flag == 0:
         format_specific["record_flag"] = "No problem"
     elif record_flag == 1:
         format_specific["record_flag"] = "Fixed"
     elif record_flag == 2:
         format_specific["record_flag"] = "Unfixed problem"
     else:
         format_specific["record_flag"] = ""
 
-    scaling_factor = float(flt_data[87])
-    format_specific["scaling_factor"] = _check_assign(scaling_factor, unknown, np.nan)
-    sensor_sensitivity = float(flt_data[41])
-    format_specific["sensor_sensitivity"] = _check_assign(
-        sensor_sensitivity, unknown, np.nan
-    )
+    if flt_data[87] != unknown_flt:
+        format_specific["scaling_factor"] = float(flt_data[87])
+    else:
+        format_specific["scaling_factor"] = np.nan
+
+    if flt_data[41] != unknown_flt:
+        format_specific["sensor_sensitivity"] = float(flt_data[41])
+    else:
+        format_specific["sensor_sensitivity"] = np.nan
 
     # for V0 files, set a standard field called instrument_sensitivity
-    ctov = least_significant_bit / MICRO_TO_VOLT
+    ctov = format_specific["least_significant_bit"] / MICRO_TO_VOLT
     vtog = 1 / format_specific["sensor_sensitivity"]
     if not np.isnan(format_specific["gain"]):
         gain = format_specific["gain"]
     else:
         gain = 1.0
     if gain == 0:
         fmt = "%s.%s.%s.%s"
@@ -719,22 +804,14 @@
     # Set dictionary
     hdr["standard"] = standard
     hdr["coordinates"] = coordinates
     hdr["format_specific"] = format_specific
     return hdr
 
 
-def _check_assign(value, unknown, default):
-    """Check for the unknown flag and return the correct value."""
-    if value != unknown:
-        return value
-    else:
-        return default
-
-
 def _read_lines(skip_rows, filename):
     """Read lines of comments and data exluding headers.
 
     Args:
         skip_rows (int):
             Number of rows to skip.
         filename (str):
```

### Comparing `gmprocess-1.3.2/src/gmprocess/io/cosmos/cosmos_writer.py` & `gmprocess-2.0.0/src/gmprocess/io/cosmos/cosmos_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datetime import datetime
 from enum import Enum
 
 # third party imports
 import numpy as np
 import pandas as pd
 import scipy.constants as sp
-from gmprocess.core.stationtrace import UNITS
+from gmprocess.utils.constants import UNIT_TYPES
 
 # local imports
 from gmprocess.io.asdf.stream_workspace import StreamWorkspace
 from gmprocess.io.cosmos.core import BUILDING_TYPES, MICRO_TO_VOLT, SENSOR_TYPES
 from gmprocess.utils.config import get_config
 from obspy.geodetics.base import gps2dist_azimuth
 
@@ -249,15 +249,14 @@
     header_fmt["missing_data_float"] = ["{value:5.1f}", 72, None]
 
     def __init__(self, trace, scalar_event, stream, volume, gmprocess_version):
         datadir = pathlib.Path(__file__).parent / ".." / ".." / "data"
         excelfile = pathlib.Path(datadir) / "cosmos_table4.xls"
         table4 = Table4(excelfile)
         # fill in data for text header
-        # UNITS = {"acc": "cm/s^2", "vel": "cm/s"}
         quantity = "velocity"
         if trace.stats.standard.units_type == "acc":
             quantity = "acceleration"
         level = "Raw"
         dmax = trace.max()
         maxidx = np.where(trace.data == dmax)[0][0]
 
@@ -349,15 +348,15 @@
 
         # line 10
         dtime = trace.stats.endtime - trace.stats.starttime  # duration secs
         self.set_header_value("record_duration", dtime)
         if volume == Volume.RAW:
             self.set_header_value("raw_maximum", trace.max())
             self.set_header_value(
-                "raw_maximum_units", UNITS[trace.stats.standard.units_type]
+                "raw_maximum_units", UNIT_TYPES[trace.stats.standard.units_type]
             )
             self.set_header_value("raw_maximum_time", maxtime)
         else:
             self.set_header_value("raw_maximum", 0)
             self.set_header_value("raw_maximum_units", "")
             self.set_header_value("raw_maximum_time", 0)
 
@@ -371,15 +370,15 @@
         config = get_config()
         agency = "UNK"
         if "agency" in config:
             agency = config["agency"]
         self.set_header_value("processing_agency", agency)
         self.set_header_value("data_maximum", dmax)
         self.set_header_value(
-            "data_maximum_units", UNITS[trace.stats.standard.units_type]
+            "data_maximum_units", UNIT_TYPES[trace.stats.standard.units_type]
         )
         self.set_header_value("data_maximum_time", maxtime)
 
         # line 12
         lowpass_prov = trace.get_provenance("lowpass_filter")
         highpass_prov = trace.get_provenance("highpass_filter")
         self.set_header_value(
@@ -605,15 +604,15 @@
         self.volume = volume
         self.trace = trace
         quantity = "velocity"
         if trace.stats.standard.units_type == "acc":
             quantity = "acceleration"
         npts = len(trace.data)
         itime = int(trace.stats.endtime - trace.stats.starttime)  # duration secs
-        units = UNITS[trace.stats.standard.units_type]
+        units = UNIT_TYPES[trace.stats.standard.units_type]
         ffmt = cfmt_to_ffmt(DATA_FMT, NUM_DATA_COLS)
 
         # fill in comment fields that we use for overflow information
         self.comment_lines = []
         instrument = trace.stats.standard.instrument.replace("None", "").strip()
         self.write_comment("Sensor", instrument, "standard")
         network = trace.stats.network
```

### Comparing `gmprocess-1.3.2/src/gmprocess/io/cosmos/data_structures.py` & `gmprocess-2.0.0/src/gmprocess/io/cosmos/data_structures.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/cwb/core.py` & `gmprocess-2.0.0/src/gmprocess/io/cwb/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/dmg/core.py` & `gmprocess-2.0.0/src/gmprocess/io/dmg/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/dynamic_search_parameters.py` & `gmprocess-2.0.0/src/gmprocess/io/dynamic_search_parameters.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/esm/core.py` & `gmprocess-2.0.0/src/gmprocess/io/esm/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/fetcher.py` & `gmprocess-2.0.0/src/gmprocess/io/fetcher.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/geonet/core.py` & `gmprocess-2.0.0/src/gmprocess/io/geonet/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/global_fetcher.py` & `gmprocess-2.0.0/src/gmprocess/io/global_fetcher.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/knet/core.py` & `gmprocess-2.0.0/src/gmprocess/io/knet/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/knet/knet_fetcher.py` & `gmprocess-2.0.0/src/gmprocess/io/knet/knet_fetcher.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/nga.py` & `gmprocess-2.0.0/src/gmprocess/io/nga.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/nsmn/core.py` & `gmprocess-2.0.0/src/gmprocess/io/nsmn/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/obspy/core.py` & `gmprocess-2.0.0/src/gmprocess/io/obspy/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/obspy/fdsn_fetcher.py` & `gmprocess-2.0.0/src/gmprocess/io/obspy/fdsn_fetcher.py`

 * *Files 9% similar despite different names*

```diff
@@ -234,14 +234,22 @@
         for provider_dict in selected_providers:
             if provider_dict["name"] == GEO_NET_ARCHIVE_KEY:
                 dt = UTCDateTime.utcnow() - UTCDateTime(self.time)
                 if dt < GEONET_ARCHIVE_DAYS:
                     provider_dict["url"] = GEONET_REALTIME_URL
             if "bounds" in provider_dict:
                 bounds = provider_dict["bounds"]
+                if bounds[0] > bounds[1]:  # crossing meridian
+                    lontest = self.lon
+                    cmpxmax = bounds[1] + 360
+                    if self.lon < 0:
+                        lontest = self.lon + 360
+                    outside_lon = lontest > cmpxmax or lontest < bounds[0]
+                else:
+                    outside_lon = self.lon > bounds[1] or self.lon < bounds[0]
                 outside_lat = self.lat > bounds[3] or self.lat < bounds[2]
                 outside_lon = self.lon > bounds[1] or self.lon < bounds[0]
                 if outside_lat or outside_lon:
                     continue
             try:
                 # Is authetication information configured?
                 fdsn_auth = self.config["fetchers"]["FDSNFetcher"]["authentication"]
```

### Comparing `gmprocess-1.3.2/src/gmprocess/io/read.py` & `gmprocess-2.0.0/src/gmprocess/io/read.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Args:
         filename (str or pathlib.Path):
             Path to file
         read_format (str):
             Format of file
 
     Returns:
-        list: Sequence of obspy.core.stream.Streams read from file
+        list: Sequence of StationStream objects.
     """
     filename = Path(filename)
 
     file_ext = filename.suffix
     if file_ext in EXCLUDED_EXTS:
         raise ValueError(f"Excluded extension: {filename}")
     # Check if file exists
```

### Comparing `gmprocess-1.3.2/src/gmprocess/io/read_directory.py` & `gmprocess-2.0.0/src/gmprocess/io/read_directory.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/renadic/core.py` & `gmprocess-2.0.0/src/gmprocess/io/renadic/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/report.py` & `gmprocess-2.0.0/src/gmprocess/io/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,15 +322,18 @@
         if row == last_row:
             final_dict["Process Step"][i] = ""
             continue
         last_row = row
 
     newdf = pd.DataFrame(final_dict)
     # prov_string = newdf.to_latex(index=False)
-    newdf = newdf.map(str_for_latex)
+    if hasattr(newdf, "map") and callable(newdf.map): # applymap ->map in Pandas 2.1.0
+        newdf = newdf.map(str_for_latex)
+    else:
+        newdf = newdf.applymap(str_for_latex)
     prov_string = newdf.style.to_latex(hrules=True)
     # Annoying hack because pandas removed the functionality to hide the index when
     # writing to latex.
     prov_string = prov_string.replace("{llll", "{lll")
     prov_string = re.sub(r"\n\d* &", "\n", prov_string)
 
     prov_string = "\\tiny\n" + prov_string
```

### Comparing `gmprocess-1.3.2/src/gmprocess/io/seedname.py` & `gmprocess-2.0.0/src/gmprocess/io/seedname.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/smc/core.py` & `gmprocess-2.0.0/src/gmprocess/io/smc/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/unam/core.py` & `gmprocess-2.0.0/src/gmprocess/io/unam/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/usc/core.py` & `gmprocess-2.0.0/src/gmprocess/io/usc/core.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/io/utils.py` & `gmprocess-2.0.0/src/gmprocess/io/utils.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/metrics/base_metric_collection.py` & `gmprocess-2.0.0/src/gmprocess/metrics/metric_collection_base.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/metrics/reduction/smooth_select.py` & `gmprocess-2.0.0/src/gmprocess/metrics/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,106 +1,122 @@
-"""Module for the Smooth_Select class."""
+"""Utilities for the metrics package."""
 
-# Third party imports
-import numpy as np
+import re
 
-# Local imports
-from gmprocess.metrics.exception import PGMException
-from gmprocess.metrics.reduction.reduction import Reduction
-from esi_core.gmprocess.waveform_processing.smoothing.konno_ohmachi import (
-    konno_ohmachi_smooth,
-)
-
-
-class Smooth_Select(Reduction):
-    def __init__(
-        self,
-        reduction_data,
-        bandwidth=None,
-        percentile=None,
-        period=None,
-        smoothing=None,
-        interval=[5, 95],
-        config=None,
-    ):
-        """
-        Args:
-            reduction_data (obspy.core.stream.Stream or numpy.ndarray):
-                Intensity measurement component.
-            bandwidth (float):
-                Bandwidth for the smoothing operation.
-            percentile (float):
-                Percentile for rotation calculations.
-            period (float):
-                Period for smoothing (Fourier amplitude spectra) calculations.
-            smoothing (string):
-                Smoothing type.
-            interval (list):
-                List of length 2 with the quantiles (0-1) for duration interval
-                calculation.
-            config (dict):
-                Config dictionary.
-
-        Raises:
-            PGMException: if the bandwidth, period, or smoothing values
-            are None.
-        """
-        super().__init__(
-            reduction_data,
-            bandwidth=bandwidth,
-            percentile=percentile,
-            period=period,
-            smoothing=smoothing,
-            config=config,
-        )
-        if period is None:
-            raise PGMException(
-                "Smooth_Select: The period value must "
-                "be defined and of type float or int."
-            )
-        if bandwidth is None:
-            raise PGMException(
-                "Smooth_Select: The bandwidth value must "
-                "be defined and of type float or int."
-            )
-        if smoothing is None:
-            raise PGMException(
-                "Smooth_Select: The smoothing value must "
-                "be defined and of type string."
-            )
-        self.period = period
-        self.smoothing = smoothing
-        self.bandwidth = bandwidth
-        self.result = self.get_pick()
-
-    def get_pick(self):
-        """
-        Performs smoothing and picks values for each defined period.
-
-        Returns:
-            picked: Dictionary of values for each period.
-        """
-        if "freqs" in self.reduction_data.keys():
-            # Horizontal channels have been combined
-            picked = {"": self._pick_spectra(self.reduction_data)}
+
+def component_to_channel(channel_names):
+    """Dictionary with mapping from channel name to component.
+
+    Args:
+        channel_names (list):
+            List of strings for channel names, e.g., ["HNZ", "HNN", "HNE"].
+    """
+    channel_names = sorted(channel_names)
+    channel_dict = {}
+    reverse_dict = {}
+    channel_number = 1
+    for channel_name in channel_names:
+        if channel_name.endswith("Z"):
+            channel_dict["Z"] = channel_name
         else:
-            # Channels have not been combined, so we need to return
-            # a dictionary with keys for each channel
-            picked = {}
-            for ch, data in self.reduction_data.items():
-                picked[ch] = self._pick_spectra(data)
-        return picked
-
-    def _pick_spectra(self, data):
-        freqs = data["freqs"]
-        spectra = data["spectra"]
-        fas_frequencies = 1 / np.asarray([self.period])
-        smoothed_values = np.empty_like(fas_frequencies)
-        if self.smoothing.lower() == "konno_ohmachi":
-            konno_ohmachi_smooth(
-                spectra.astype(np.double),
-                freqs,
-                fas_frequencies,
-                smoothed_values,
-                self.bandwidth,
-            )
-        return smoothed_values[0]
+            cname = "H%i" % channel_number
+            channel_number += 1
+            channel_dict[cname] = channel_name
+
+    reverse_dict = {v: k for k, v in channel_dict.items()}
+    return (channel_dict, reverse_dict)
+
+
+def parse_period(imt):
+    """
+    Parses the period from the imt.
+
+    Args:
+        imt (string):
+            Imt that contains a period similar to one of the following
+            examples:
+                - SA(1.0)
+                - SA(1)
+                - SA1.0
+                - SA1
+    Returns:
+        str: Period for the calculation.
+
+    Notes:
+        Can be either a float or integer.
+    """
+    period = re.findall(r"\d+", imt)
+
+    if len(period) > 1:
+        period = ".".join(period)
+    elif len(period) == 1:
+        period = period[0]
+    else:
+        period = None
+    return period
+
+
+def parse_percentile(imc):
+    """
+    Parses the percentile from the imc.
+
+    Args:
+        imc (string):
+            Imc that contains a period similar to one of the following
+            examples:
+                - ROTD(50.0)
+                - ROTD(50)
+                - ROTD50.0
+                - ROTD50
+
+    Returns:
+        str: Period for the calculation.
+
+    Notes:
+        Can be either a float or integer.
+    """
+    percentile = re.findall(r"\d+", imc)
+    if len(percentile) > 1:
+        percentile = ".".join(percentile)
+    elif len(percentile) == 1:
+        percentile = percentile[0]
+    else:
+        percentile = None
+    return percentile
+
+
+def parse_interval(imt):
+    """
+    Parses the interval from the imt string.
+
+    Args:
+        imt (string):
+            Imt that contains a interval.
+            example:
+                - duration5-95
+    Returns:
+        str: Interval for the calculation.
+
+    Notes:
+        Can be either a float or integer.
+    """
+    tmpstr = imt.replace("duration", "")
+    if tmpstr:
+        return [int(p) for p in tmpstr.split("-")]
+    else:
+        return None
+
+
+def find_float(imt):
+    """Find the float in an IMT string.
+
+    Args:
+        imt (str):
+            An IMT string with a float in it (e.g., period for SA).
+
+    Returns:
+        float: the IMT float, if found, otherwise None.
+    """
+    try:
+        return float(re.search(r"[0-9]*\.[0-9]*", imt).group())
+    except AttributeError:
+        return None
```

### Comparing `gmprocess-1.3.2/src/gmprocess/metrics/station_metric.py` & `gmprocess-2.0.0/src/gmprocess/metrics/station_metric.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/metrics/station_metric_collection.py` & `gmprocess-2.0.0/src/gmprocess/metrics/station_metric_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from openquake.hazardlib.geo import geodetic as oqgeo
 
 from esi_utils_rupture.point_rupture import PointRupture
 from esi_utils_rupture.origin import Origin
 from esi_utils_rupture.factory import get_rupture
 
 from gmprocess.utils import constants
-from gmprocess.metrics.base_metric_collection import MetricCollection
+from gmprocess.metrics.metric_collection_base import MetricCollection
 from gmprocess.metrics.station_metric import StationMetric
 from gmprocess.io.asdf.station_metrics_xml import StationMetricsXML
 from gmprocess.io.asdf.path_utils import get_stream_path
 from gmprocess.io.asdf.stream_workspace import array_to_str
 
 
 class StationMetricCollection(MetricCollection):
@@ -49,15 +49,15 @@
     @classmethod
     def from_streams(cls, streams, event, config, rupture_file=None):
         """Construct the StationMetricCollection from a list of StationStreams.
 
         Args:
             streams (list):
                 List of StationStream objects.
-            event (gmprocess.utils.event.ScalarEvent):
+            event (gmprocess.utils.scalar_event.ScalarEvent):
                 A ScalarEvent object.
             config (dict):
                 Dictionary of config options.
             rupture_file (str):
                 Path to rupture file.
         """
 
@@ -102,15 +102,15 @@
         self, streams, event, config, rupture_file=None, label="default"
     ):
         """Calculate station metrics from a list of streams.
 
         Args:
             streams (list):
                 List of StationStream objects.
-            event (gmprocess.utils.event.ScalarEvent):
+            event (gmprocess.utils.scalar_event.ScalarEvent):
                 A ScalarEvent object.
             config (dict):
                 Dictionary of config options.
             rupture_file (str):
                 Path to rupture file.
             label (str):
                 Processing label.
```

### Comparing `gmprocess-1.3.2/src/gmprocess/metrics/transform/oscillator.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/pretesting.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,195 +1,227 @@
-"""Module for oscillator class."""
+"""
+Pretesting methods.
+"""
+
+import logging
+from obspy.signal.trigger import classic_sta_lta
+from gmprocess.utils.config import get_config
+from gmprocess.waveform_processing.processing_step import processing_step
 
-from obspy.core.trace import Trace
 
-# Local import
-from gmprocess.core.stationtrace import StationTrace
-from gmprocess.core.stationstream import StationStream
-from esi_core.gmprocess.metrics.oscillators import calculate_spectrals
-from gmprocess.metrics.transform.transform import Transform
-from gmprocess.utils.constants import GAL_TO_PCTG
-
-
-class oscillator(Transform):
-    """Class for computing the oscillator for a given period."""
-
-    def __init__(
-        self,
-        transform_data,
-        damping,
-        period,
-        times,
-        max_period,
-        allow_nans,
-        bandwidth,
-        config,
-    ):
-        """
-        Args:
-            transform_data (StationStream):
-                Intensity measurement component.
-            damping (float):
-                Damping for spectral amplitude calculations.
-            period (float):
-                Period for spectral amplitude calculations.
-            times (numpy.ndarray):
-                Times for the spectral amplitude calculations.
-            allow_nans (bool):
-                Should nans be allowed in the smoothed spectra. If False, then
-                the number of points in the FFT will be computed to ensure
-                that nans will not result in the smoothed spectra.
-            config (dict):
-                Configuration options.
-
-        """
-        super().__init__(
-            transform_data,
-            damping=damping,
-            period=period,
-            times=times,
-            max_period=max_period,
-            allow_nans=allow_nans,
-            bandwidth=bandwidth,
-            config=config,
-        )
-        self.period = period
-        self.damping = damping
-        self.times = times
-        self.result = self.get_oscillator(config)
-
-    def get_oscillator(self, config=None):
-        """
-        Calculated the oscillator of each trace's data.
-
-        Args:
-            config (dict):
-                Configuration options.
-
-        Returns:
-            spectrals: StationStream or numpy.ndarray with the oscillator data.
-        """
-        spectrals = get_spectral(
-            self.period,
-            self.transform_data,
-            damping=self.damping,
-            times=self.times,
-            config=config,
-        )
-        return spectrals
-
-
-def get_spectral(period, stream, damping=0.05, times=None, config=None):
-    """
-    Returns a stream of spectral response with units of %%g.
-
-    Args:
-        period (float):
-            Period for spectral response.
-        stream (StationStream):
-            Strong motion timeseries for one station.
-        damping (float):
-            Damping of oscillator.
-        times (np.ndarray):
-            Array of times for the horizontal channels. Default is None.
-        config (dict):
-            StationStream.
-
-    Returns:
-        StationStream.
-    """
-
-    # Use as-recorded or upsampled record?
-    use_upsampled = False
-    dt = stream[0].stats.delta
-    ns = (int)(10.0 * dt / period - 0.01) + 1
-    if ns > 1:
-        use_upsampled = True
-        dt = stream[0].get_cached("upsampled")["dt"]
-
-    if "rotated" in stream.get_stream_param_keys():
-        # For ROTD and GMROTD
-        rotated = []
-        if use_upsampled:
-            rotated_data = stream.get_stream_param("upsampled_rotated")
-        else:
-            rotated_data = stream.get_stream_param("rotated")
-
-        for rot_matrix in rotated_data:
-            rotated_spectrals = []
-            # This is the loop over rotation angles
-            for rot_data in rot_matrix:
-                stats = {
-                    "npts": len(rot_data),
-                    "delta": dt,
-                    "sampling_rate": 1.0 / dt,
-                }
-                new_trace = Trace(data=rot_data, header=stats)
-                sa_list = new_and_improved_calculate_spectrals(
-                    new_trace, period, damping
-                )
-                acc_sa = sa_list[0]
-                acc_sa *= GAL_TO_PCTG
-                rotated_spectrals.append(acc_sa)
-            rotated += [rotated_spectrals]
-
-        # Add rotated data to stream parameters
-        stream.set_stream_param("rotated_oscillator", rotated)
-        return stream
-    else:
-        traces = []
-        # For anything but ROTD and GMROTD
-        for trace in stream:
-            if use_upsampled:
-                trace_dict = trace.get_cached("upsampled")
-                stats = {
-                    "npts": trace_dict["np"],
-                    "delta": dt,
-                    "sampling_rate": 1.0 / dt,
-                }
-                temp_trace = Trace(data=trace_dict["data"], header=stats)
+@processing_step
+def min_sample_rate(st, min_sps=20.0, config=None):
+    """Require a minimum sample rate.
+
+    Args:
+        st (gmprocess.core.stationstream.StationStream):
+            Stream of data.
+        min_sps (float):
+            Minimum samples per second.
+        config (dict):
+            Configuration dictionary (or None). See get_config().
+
+    Returns:
+        StationStream: Stream checked for sample rate criteria.
+    """
+    if not st.passed:
+        return st
+
+    for tr in st:
+        if tr.passed:
+            actual_sps = tr.stats.sampling_rate
+            if actual_sps < min_sps:
+                tr.fail(f"Minimum sample rate of {min_sps} not exceeded.")
+
+    return st
+
+
+@processing_step
+def check_instrument(st, n_max=3, n_min=2, require_two_horiz=True, config=None):
+    """Test the channels of the station.
+
+    The purpose of the maximum limit is to skip over stations with muliple
+    strong motion instruments, which can occur with downhole or structural
+    arrays since our code currently is not able to reliably group by location
+    within an array.
+
+    The purpose of the minimum and require_two_horiz checks are to ensure the
+    channels are required for subsequent intensity measures such as ROTD.
+
+    Args:
+        st (gmprocess.core.stationstream.StationStream):
+            Stream of data.
+        n_max (int):
+            Maximum allowed number of streams; default to 3.
+        n_min (int):
+            Minimum allowed number of streams; default to 1.
+        require_two_horiz (bool):
+            Require two horizontal components; default to `False`.
+        config (dict):
+            Configuration dictionary (or None). See get_config().
+
+    Returns:
+        StationStream: With instrument criteria applied.
+    """
+    if not st.passed:
+        return st
+
+    if config is None:
+        config = get_config()
+
+    logging.debug("Starting check_instrument")
+    logging.debug(f"len(st) = {len(st)}")
+
+    for failed_test, message in [
+        (len(st) > n_max, f"More than {n_max} traces in stream."),
+        (len(st) < n_min, f"Less than {n_min} traces in stream."),
+        (
+            require_two_horiz and (st.num_horizontal != 2),
+            "Not two horizontal components",
+        ),
+    ]:
+        if failed_test:
+            for tr in st:
+                tr.fail(message)
+            # Stop at first failed test
+            break
+
+    return st
+
+
+@processing_step
+def check_free_field(st, reject_non_free_field=True, config=None):
+    """Checks free field status of stream.
+
+    Args:
+        st (gmprocess.core.stationstream.StationStream):
+            Stream of data.
+        reject_non_free_field (bool):
+            Should non free-field stations be failed?
+        config (dict):
+            Configuration dictionary (or None). See get_config().
+
+    Returns:
+        StationStream: That has been checked for free field status.
+    """
+    if not st.passed:
+        return st
+
+    for trace in st:
+        if trace.passed and not trace.free_field and reject_non_free_field:
+            trace.fail("Failed free field sensor check.")
+
+    return st
+
+
+@processing_step
+def check_sta_lta(st, sta_length=1.0, lta_length=20.0, threshold=5.0, config=None):
+    """Apply STA/LTA ratio criteria.
+
+    Checks that the maximum STA/LTA ratio of the stream's traces is above a threshold.
+
+    Args:
+        st (gmprocess.core.stationstream.StationStream):
+            Stream of data.
+        sta_length (float):
+            Length of time window for STA (seconds).
+        lta_length (float):
+            Length of time window for LTA (seconds).
+        threshold (float):
+            Required maximum STA/LTA ratio to pass the test.
+        config (dict):
+            Configuration dictionary (or None). See get_config().
+
+    Returns:
+        StationStream: That has been checked for sta/lta requirements.
+    """
+    if not st.passed:
+        return st
+
+    for tr in st:
+        if tr.passed:
+            sr = tr.stats.sampling_rate
+            nlta = lta_length * sr + 1
+            if len(tr) >= nlta:
+                sta_lta = classic_sta_lta(tr.data, sta_length * sr + 1, nlta)
+                if sta_lta.max() < threshold:
+                    tr.fail(
+                        "Failed sta/lta check because threshold sta/lta is not "
+                        "exceeded."
+                    )
             else:
-                temp_trace = trace
-            sa_list = new_and_improved_calculate_spectrals(temp_trace, period, damping)
-            acc_sa = sa_list[0]
-            acc_sa *= GAL_TO_PCTG
-            stats = trace.stats.copy()
-            stats.npts = sa_list[3]
-            stats.delta = sa_list[4]
-            stats.sampling_rate = sa_list[5]
-            stats["units"] = "%%g"
-            spect_trace = StationTrace(data=acc_sa, header=stats, config=config)
-            traces += [spect_trace]
-        spect_stream = StationStream(traces, config=config)
-        return spect_stream
-
-
-def new_and_improved_calculate_spectrals(trace, period, damping):
-    """
-    Pull some stuff out of cython that shouldn't be there.
-    """
-    new_dt = trace.stats.delta
-    new_np = trace.stats.npts
-    new_sample_rate = trace.stats.sampling_rate
-    tlen = (new_np - 1) * new_dt
-    # This is the resample factor for low-sample-rate/high-frequency
-    ns = (int)(10.0 * new_dt / period - 0.01) + 1
-    if ns > 1:
-        # Increase the number of samples as necessary
-        new_np = new_np * ns
-        # Make the new number of samples a power of two
-        # leaving this out for now; it slows things down but doesn't
-        # appear to affect the results. YMMV.
-        # new_np = 1 if new_np == 0 else 2**(new_np - 1).bit_length()
-        # The new sample interval
-        new_dt = tlen / (new_np - 1)
-        # The new sample rate
-        new_sample_rate = 1.0 / new_dt
-        # Make a copy because resampling happens in place
-        trace = trace.copy()
-        # Resample the trace
-        trace.resample(new_sample_rate, window=None)
+                tr.fail(
+                    "Failed sta/lta check because record length is shorter "
+                    "than lta length."
+                )
+
+    return st
+
+
+@processing_step
+def check_max_amplitude(st, min=5, max=2e6, config=None):
+    """Check the maximum amplitude of the traces.
 
-    sa_list = calculate_spectrals(
-        trace.data, new_np, new_dt, new_sample_rate, period, damping
+    Checks that the maximum amplitude of the traces in the stream are within a defined
+    range. Only applied to counts/raw data. This is a simple way to screen for clipped
+    records, but we now recommend/prefer the `check_clipping` method.
+
+    Args:
+        st (gmprocess.core.stationstream.StationStream):
+            Stream of data.
+        min (float):
+            Minimum amplitude for the acceptable range. Default is 5.
+        max (float):
+            Maximum amplitude for the acceptable range. Default is 2e6.
+        config (dict):
+            Configuration dictionary (or None). See get_config().
+
+    Returns:
+        StationStream: That has been checked for maximum amplitude criteria.
+    """
+    if not st.passed:
+        return st
+
+    for tr in st:
+        # Only perform amplitude/clipping check if data has not been converted
+        # to physical units
+        if tr.passed:
+            if "remove_response" not in tr.provenance.ids:
+                if abs(tr.max()) < float(min) or abs(tr.max()) > float(max):
+                    tr.fail("Failed max amplitude check.")
+
+    return st
+
+
+@processing_step
+def max_traces(st, n_max=3, config=None):
+    """Reject a stream if it has more than n_max traces.
+
+    The purpose of this is to skip over stations with muliple strong motion
+    instruments, which can occur with downhole or structural arrays since our
+    code currently is not able to reliably group by location within an array.
+
+    Args:
+        st (gmprocess.core.stationstream.StationStream):
+            Stream of data.
+        n_max (int):
+            Maximum allowed number of streams; default to 3.
+        config (dict):
+            Configuration dictionary (or None). See get_config().
+
+    Returns:
+        StationStream: Stream with max number of traces criteria applied.
+    """
+    logging.warning(
+        "This function is deprecated. Please replace with "
+        "check_instrument, which includes additional "
+        "functionality."
     )
-    return sa_list
+    if not st.passed:
+        return st
+
+    logging.debug("Starting max_traces")
+    logging.debug(f"len(st) = {len(st)}")
+    if len(st) > n_max:
+        for tr in st:
+            tr.fail(f"More than {n_max} traces in stream.")
+    return st
```

### Comparing `gmprocess-1.3.2/src/gmprocess/metrics/waveform_metric.py` & `gmprocess-2.0.0/src/gmprocess/metrics/waveform_metric_type.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-"""Module for the WaveformMetric class."""
+"""Module for WaveformMetricType classes."""
 
 from abc import ABC, abstractmethod
 
 from gmprocess.utils import constants
 
 
-class WaveformMetric(ABC):
+class WaveformMetricType(ABC):
     """Base class for waveform metric classes."""
 
-    def __repr__(self):
-        comps = ", ".join({f"{k}={v:.3f}" for (k, v) in self._values.items()})
-        return f"{self.identifier}: {comps}"
-
     def __init__(self):
         self._values = None
         self._type = None
         self.format_type = None
         self._units = None
         self.metric_attributes = None
         self.component_to_channel = None
 
     def to_dict(self):
-        """Return a dictionary representation of the Metric object."""
+        """Return a dictionary representation of the WaveformMetricType object."""
         return {
             "values": list(self._values.values()),
             "components": self.components,
             "type": self._type,
             "format_type": self.format_type,
             "units": self._units,
             "metric_attributes": self.metric_attributes,
             "component_to_channel": self.component_to_channel,
         }
 
+    def __repr__(self):
+        comps = ", ".join({f"{k}={v:.3f}" for (k, v) in self._values.items()})
+        return f"{self.identifier}: {comps}"
+
     @property
     def type(self):
         """Type is the metric type and does not include metric attributes.
 
         Note that this is the simplest name and we define it to be identical to the
-        name of the Metric subclass.
+        name of the WaveformMetricType subclass.
         """
         return self._type
 
     @property
     @abstractmethod
     def identifier(self):
         """The identifier includes metric attributes, but not values/components."""
@@ -58,48 +58,55 @@
 
     @property
     def components(self):
         """The available components."""
         return list(self._values.keys())
 
     def value(self, component):
-        """Return the value for the specified component"""
-        return self._values[component]
+        """Return the value for the specified component.
+
+        Args:
+            component (str):
+                String representaiton of a WaveformMetricComponent.
+        """
+        for k, v in self._values.items():
+            if str(k) == str(component):
+                return v
 
     @staticmethod
     def metric_from_dict(mdict):
-        """Class factory to create a Metric subclass instance from a dictionary.
+        """Class factory to create a WaveformMetricType from a dictionary.
 
         Args:
             mdict (dict):
                 A dictionary with the structure of the dictionary that is returned by
-                Metric.to_dict().
+                WaveformMetricType.to_dict().
         """
         # List of subclasses
-        metric_subclasses = WaveformMetric.__subclasses__()
+        metric_subclasses = WaveformMetricType.__subclasses__()
 
         # Dictionary for selecting a subclass
-        sub_dict = {m.__name__: m for m in metric_subclasses}
+        sub_dict = {m.__name__.lower(): m for m in metric_subclasses}
 
         # Name of subclass is in the "type" key
-        selected_class = sub_dict[mdict["type"]]
+        selected_class = sub_dict[mdict["type"].lower()]
 
         # Prepare the arguments to construct a class instance
         cargs = mdict.copy()
         rm_keys = ["type", "format_type", "units"]
         for k in rm_keys:
             cargs.pop(k)
         attr = cargs.pop("metric_attributes")
         for k, v in attr.items():
             cargs[k] = v
         return selected_class(**cargs)
 
 
-class PGA(WaveformMetric):
-    """WaveformMetric subclass for PGA."""
+class PGA(WaveformMetricType):
+    """WaveformMetricType subclass for PGA."""
 
     def __init__(self, values, components, component_to_channel=None):
         """Construct a PGA metric object.
 
         Args:
             values (list):
                 List of PGA values.
@@ -121,20 +128,24 @@
         self.component_to_channel = component_to_channel
 
     @property
     def identifier(self):
         return "PGA"
 
 
-class PGV(WaveformMetric):
-    """WaveformMetric subclass for PGV."""
+class PGV(WaveformMetricType):
+    """WaveformMetricType subclass for PGV."""
 
-    def __init__(self, values, components, component_to_channel=None):
+    def __init__(self, values, components, component_to_channel=None, **kwargs):
         """Construct a PGV metric object.
 
+        Note: kwargs is needed because there are parameters that will get automatically
+        passed here due to the integration processing step that we do not actually
+        want to keep as metric parameters.
+
         Args:
             values (list):
                 List of PGV values.
             components (list):
                 List of the components that map to the PGV values.
             component_to_channel (dict):
                 Optional dictionary mapping the simplifued component names to the
@@ -152,16 +163,16 @@
         self.component_to_channel = component_to_channel
 
     @property
     def identifier(self):
         return "PGV"
 
 
-class SA(WaveformMetric):
-    """WaveformMetric subclass for SA, spectral acceleration."""
+class SA(WaveformMetricType):
+    """WaveformMetricType subclass for SA, spectral acceleration."""
 
     def __init__(
         self, values, components, period, damping=5.0, component_to_channel=None
     ):
         """Construct a SA metric object.
 
         Args:
@@ -193,66 +204,78 @@
 
     @property
     def identifier(self):
         attrs = self.metric_attributes
         return f"SA(T={float(attrs['period']):.4f}, D={float(attrs['damping']):.3f})"
 
 
-class FAS(WaveformMetric):
-    """WaveformMetric subclass for FAS, Fourier amplitude spectra."""
+class FAS(WaveformMetricType):
+    """WaveformMetricType subclass for FAS, Fourier amplitude spectra."""
 
     def __init__(
         self,
         values,
         components,
-        period,
-        smoothing=20.0,
-        method="Konno-Omachi",
+        frequencies,  # noqa
+        smoothing_parameter=20.0,
+        smoothing_method="Konno-Omachi",
+        allow_nans=True,
         component_to_channel=None,
     ):
         """Construct a FAS metric object.
 
+        Note that "frequencies" is passed in as a metric parameter, but the resulting
+        array of frequencies is in the "values" container so there's no need to do
+        anything with the "frequencies" array.
+
         Args:
             values (list):
                 List of FAS values.
             components (list):
                 List of the components that map to the FAS values.
-            period (float):
-                Period for this fAS (in seconds).
-            smoothing (float):
+            frequencies (array):
+                Frequencies for this FAS (Hz).
+            smoothing_parameter (float):
                 Smoothing bandwidth parameter; default is 20.
-            method (str):
+            smoothing_method (str):
                 Smoothing method; default is Konno-Omachi.
+            allow_nans (book):
+                Default (True) just uses the number of points in the record, which can
+                result in nans when smoothed using the Konno-Omachi method. False
+                adjusts the number of points in the FFT to ensure no nans.
             component_to_channel (dict):
                 Optional dictionary mapping the simplifued component names to the
                 as-recorded channel names.
         """
         super().__init__()
         if len(values) != len(components):
             raise ValueError("Length of values must equal length of components.")
 
         self._values = dict(zip(components, values))
         self._type = self.__class__.__name__
         self.format_type = "pgm"
         self._units = constants.UNITS[self._type.lower()]
         self.metric_attributes = {
-            "period": period,
-            "smoothing": smoothing,
-            "method": method,
+            "smoothing_parameter": smoothing_parameter,
+            "smoothing_method": smoothing_method,
+            "allow_nans": allow_nans,
         }
         self.component_to_channel = component_to_channel
 
     @property
     def identifier(self):
         attrs = self.metric_attributes
-        return f"FAS(T={float(attrs['period']):.4f}, B={float(attrs['smoothing']):.1f})"
+        return f"FAS(B={float(attrs['smoothing_parameter']):.1f})"
 
+    def __repr__(self):
+        return f"{self.identifier}: {self.components}"
 
-class Duration(WaveformMetric):
-    """WaveformMetric subclass for duration."""
+
+class Duration(WaveformMetricType):
+    """WaveformMetricType subclass for duration."""
 
     def __init__(self, values, components, interval, component_to_channel=None):
         """Construct a Duration metric object.
 
         Args:
             values (list):
                 List of Duration values.
@@ -280,16 +303,16 @@
 
     @property
     def identifier(self):
         attrs = self.metric_attributes
         return f"Duration({attrs['interval']})"
 
 
-class SortedDuration(WaveformMetric):
-    """WaveformMetric subclass for sorted duration."""
+class SortedDuration(WaveformMetricType):
+    """WaveformMetricType subclass for sorted duration."""
 
     def __init__(self, values, components, component_to_channel=None):
         """Construct a SortedDuration metric object.
 
         Args:
             values (list):
                 List of Sorted Duration values.
@@ -311,19 +334,19 @@
         self.component_to_channel = component_to_channel
 
     @property
     def identifier(self):
         return "SortedDuration"
 
 
-class AriasIntensity(WaveformMetric):
-    """WaveformMetric subclass for Arias Intensity."""
+class Arias(WaveformMetricType):
+    """WaveformMetricType subclass for Arias Intensity."""
 
     def __init__(self, values, components, component_to_channel=None):
-        """Construct a AriasIntensity metric object.
+        """Construct a Arias metric object.
 
         Args:
             values (list):
                 List of Arias Intensity values.
             components (list):
                 List of the components that map to the Arias Intensity values.
             component_to_channel (dict):
@@ -339,8 +362,40 @@
         self.format_type = "pgm"
         self._units = constants.UNITS[self._type.lower()]
         self.metric_attributes = {}
         self.component_to_channel = component_to_channel
 
     @property
     def identifier(self):
-        return "AriasIntensity"
+        return "Arias"
+
+
+class CAV(WaveformMetricType):
+    """WaveformMetricType subclass for Cumulative Absolute Velocity."""
+
+    def __init__(self, values, components, component_to_channel=None):
+        """Construct a CAV metric object.
+
+        Args:
+            values (list):
+                List of Cumulative Absolute Velocity values.
+            components (list):
+                List of the components that map to the Cumulative Absolute Velocity
+                values.
+            component_to_channel (dict):
+                Optional dictionary mapping the simplifued component names to the
+                as-recorded channel names.
+        """
+        super().__init__()
+        if len(values) != len(components):
+            raise ValueError("Length of values must equal length of components.")
+
+        self._values = dict(zip(components, values))
+        self._type = self.__class__.__name__
+        self.format_type = "pgm"
+        self._units = constants.UNITS[self._type.lower()]
+        self.metric_attributes = {}
+        self.component_to_channel = component_to_channel
+
+    @property
+    def identifier(self):
+        return "CAV"
```

### Comparing `gmprocess-1.3.2/src/gmprocess/metrics/waveform_metric_collection.py` & `gmprocess-2.0.0/src/gmprocess/metrics/waveform_metric_collection.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 import re
 from io import BytesIO
 import logging
 
 from obspy import read_inventory
 
 from gmprocess.io.asdf.waveform_metrics_xml import WaveformMetricsXML
-from gmprocess.metrics.base_metric_collection import MetricCollection
-from gmprocess.metrics.metrics_controller import MetricsController
-from gmprocess.metrics.waveform_metric_list import WaveformMetricList
-from gmprocess.utils.config import get_config_imts_imcs
+from gmprocess.metrics.metric_collection_base import MetricCollection
+from gmprocess.metrics.waveform_metric_calculator import WaveformMetricCalculator
 from gmprocess.io.asdf.path_utils import get_stream_path
 from gmprocess.io.asdf.stream_workspace import array_to_str
 
 
 class WaveformMetricCollection(MetricCollection):
     """WaveformMetricCollection class
 
@@ -30,15 +28,15 @@
           simpler.
 
     This default initialization method takes in StreamWorkspace object, but does not
     actually populate the "waveform_metrics" list. It can be populated with the
     "from_streams" or "from_workspace" methods.
 
     The "from_streams" class method initializes from a list of StationStreams, and
-    computes the waveform metrics with the MetricsController class, while the
+    computes the waveform metrics with the WaveformMetricCalculator class, while the
     "from_workspace" method loads the pre-computed metrics from the StreamWorkspace
     file.
     """
 
     def __init__(self):
         """Constructor for WaveformMetricCollection object."""
 
@@ -49,15 +47,15 @@
     @classmethod
     def from_streams(cls, streams, event, config, label="default"):
         """Construct the WaveformMetricCollection from a list of StationStreams.
 
         Args:
             streams (list):
                 List of StationStream objects.
-            event (gmprocess.utils.event.ScalarEvent):
+            event (gmprocess.utils.scalar_event.ScalarEvent):
                 A ScalarEvent object.
             config (dict):
                 Dictionary of config options.
             label (str):
                 Procesing labe.
         """
 
@@ -126,42 +124,28 @@
 
     def calculate_metrics(self, streams, event, config, label="default"):
         """Calculate waveform metrics from a list of streams.
 
         Args:
             streams (list):
                 List of StationStream objects.
-            event (gmprocess.utils.event.ScalarEvent):
+            event (gmprocess.utils.scalar_event.ScalarEvent):
                 A ScalarEvent object.
             config (dict):
                 Dictionary of config options.
             label (str):
                 Processing label.
         """
-        imts, imcs = get_config_imts_imcs(config)
-        damping = config["metrics"]["sa"]["damping"]
-        smoothing = config["metrics"]["fas"]["smoothing"]
-        bandwidth = config["metrics"]["fas"]["bandwidth"]
-        allow_nans = config["metrics"]["fas"]["allow_nans"]
         event_id = event.id.replace("smi:local/", "")
         tag = f"{event_id}_{label}"
+        # Need to have something build 'steps'
         for stream in streams:
             if stream.passed:
-                metrics = MetricsController(
-                    imts,
-                    imcs,
-                    stream,
-                    bandwidth=bandwidth,
-                    allow_nans=allow_nans,
-                    damping=damping,
-                    event=event,
-                    smooth_type=smoothing,
-                    config=config,
-                )
-                wml = WaveformMetricList.from_df(metrics.pgms, metrics.channel_dict)
+                wmc = WaveformMetricCalculator(stream, config, event)
+                wml = wmc.calculate()
                 self.waveform_metrics.append(wml)
                 self.stream_paths.append(get_stream_path(stream, tag, config))
 
     def get_stream_metadata_from_workspace(self, workspace):
         """Lightweght summary info of streams.
 
         Args:
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/assemble.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/assemble.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from concurrent.futures import ProcessPoolExecutor
 
 from gmprocess.subcommands.lazy_loader import LazyLoader
 
 arg_dicts = LazyLoader("arg_dicts", globals(), "gmprocess.subcommands.arg_dicts")
 base = LazyLoader("base", globals(), "gmprocess.subcommands.base")
 constants = LazyLoader("constants", globals(), "gmprocess.utils.constants")
+scalar_event = LazyLoader("scalar_event", globals(), "gmprocess.core.scalar_event")
 assemble_utils = LazyLoader(
     "assemble_utils", globals(), "gmprocess.utils.assemble_utils"
 )
 
 
 class AssembleModule(base.SubcommandModule):
     """Assemble raw data and organize it into an ASDF file."""
@@ -28,19 +29,17 @@
             gmrecords:
                 GMrecordsApp instance.
         """
         logging.info(f"Running subcommand '{self.command_name}'")
         self.gmrecords = gmrecords
         self._check_arguments()
 
-        self._get_events()
+        event_ids, events = self._get_event_ids_from_args()
+        logging.info(f"Number of events to assemble: {len(event_ids)}")
 
-        logging.info(f"Number of events to assemble: {len(self.events)}")
-
-        data_path = self.gmrecords.data_path
         overwrite = self.gmrecords.args.overwrite
         label = self.gmrecords.args.label
 
         # label does not get automatically assigned "default" if no input is provided,
         # so it is assigned here
         if label is None:
             label = "default"
@@ -50,67 +49,78 @@
         results = []
 
         if self.gmrecords.args.num_processes:
             futures = []
             executor = ProcessPoolExecutor(
                 max_workers=self.gmrecords.args.num_processes
             )
-            for ievent, event in enumerate(self.events):
+            for ievent, event_id in enumerate(event_ids):
                 logging.info(
-                    f"Assembling event {event.id} ({1+ievent} of {len(self.events)})..."
+                    f"Assembling event {event_id} ({1+ievent} of {len(event_ids)})..."
                 )
+                event = events[ievent] if events else None
                 future = executor.submit(
                     self._assemble_event,
+                    event_id,
                     event,
-                    data_path,
+                    self.gmrecords.data_path,
                     overwrite,
                     conf,
                     version,
                     label,
                 )
                 futures.append(future)
             results = [future.result() for future in futures]
             executor.shutdown()
         else:
-            for ievent, event in enumerate(self.events):
+            for ievent, event_id in enumerate(event_ids):
                 logging.info(
-                    f"Assembling event {event.id} ({1+ievent} of {len(self.events)})..."
+                    f"Assembling event {event_id} ({1+ievent} of {len(event_ids)})..."
                 )
+                event = events[ievent] if events else None
                 results.append(
                     self._assemble_event(
-                        event, data_path, overwrite, conf, version, label
+                        event_id,
+                        event,
+                        self.gmrecords.data_path,
+                        overwrite,
+                        conf,
+                        version,
+                        label,
                     )
                 )
 
         for res in results:
             if res is not None:
                 self.append_file("Workspace", res)
 
         self._summarize_files_created()
 
     # Note: I think that we need to make this a static method in order to be able to
     # call it with ProcessPoolExecutor.
     @staticmethod
-    def _assemble_event(event, data_path, overwrite, conf, version, label):
-        event_dir = data_path / event.id
+    def _assemble_event(event_id, event, data_path, overwrite, conf, version, label):
+        event_dir = data_path / event_id
         event_dir.mkdir(exist_ok=True)
         workname = event_dir / constants.WORKSPACE_NAME
         workspace_exists = workname.is_file()
         if workspace_exists:
             logging.info(f"ASDF exists: {str(workname)}")
             if not overwrite:
                 logging.info("The --overwrite argument not selected.")
-                logging.info(f"No action taken for {event.id}.")
+                logging.info(f"No action taken for {event_id}.")
                 return None
             else:
                 logging.info(f"Removing existing ASDF file: {str(workname)}")
                 workname.unlink()
 
         workspace = assemble_utils.assemble(
+            event_id=event_id,
             event=event,
             config=conf,
             directory=data_path,
             gmprocess_version=version,
             label=label,
         )
-        workspace.close()
+        if workspace:
+            workspace.close()
         return workname
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/autoprocess.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/autoprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module for AutoShakemapModule class."""
 
 import logging
 
 from gmprocess.subcommands.lazy_loader import LazyLoader
 
 base = LazyLoader("base", globals(), "gmprocess.subcommands.base")
+scalar_event = LazyLoader("scalar_event", globals(), "gmprocess.core.scalar_event")
 download = LazyLoader("download", globals(), "gmprocess.subcommands.download")
 assemble = LazyLoader("assemble", globals(), "gmprocess.subcommands.assemble")
 process_waveforms = LazyLoader(
     "process_waveforms", globals(), "gmprocess.subcommands.process_waveforms"
 )
 compute_station_metrics = LazyLoader(
     "compute_station_metrics",
@@ -91,23 +92,28 @@
     ]
 
     def main(self, gmrecords):
         """Chain together the most common processing subcommands."""
         logging.info(f"Running subcommand '{self.command_name}'")
         self.gmrecords = gmrecords
         self._check_arguments()
-        self._get_events()
-        nevents = len(self.events)
 
-        for ievent, event in enumerate(self.events):
+        event_ids, events = self._get_event_ids_from_args()
+        if events:
+            logging.critical(
+                "autoprocess subcommand only works with events given as ComCat ids."
+            )
+
+        for ievent, event_id in enumerate(event_ids):
             logging.info(
-                f"(auto)processing event {event.id} ({1+ievent} of {nevents})..."
+                f"(auto)processing event {event_id} ({1+ievent} of {len(event_ids)})..."
             )
-            # stomp on gmrecords.args.eventid
-            gmrecords.args.eventid = [event.id]
+
+            # stomp on gmrecords.args.event_id
+            gmrecords.args.event_id = [event_id]
 
             # Chain together relevant subcommand modules:
             if not gmrecords.args.no_download:
                 download.DownloadModule().main(gmrecords)
             if not gmrecords.args.no_assemble:
                 assemble.AssembleModule().main(gmrecords)
             if not gmrecords.args.no_process:
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/autoshakemap.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/autoshakemap.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 
 from gmprocess.subcommands.lazy_loader import LazyLoader
 
 arg_dicts = LazyLoader("arg_dicts", globals(), "gmprocess.subcommands.arg_dicts")
 base = LazyLoader("base", globals(), "gmprocess.subcommands.base")
+scalar_event = LazyLoader("scalar_event", globals(), "gmprocess.core.scalar_event")
 download = LazyLoader("download", globals(), "gmprocess.subcommands.download")
 import_data = LazyLoader("import_data", globals(), "gmprocess.subcommands.import_data")
 assemble = LazyLoader("assemble", globals(), "gmprocess.subcommands.assemble")
 process_waveforms = LazyLoader(
     "process_waveforms", globals(), "gmprocess.subcommands.process_waveforms"
 )
 compute_station_metrics = LazyLoader(
@@ -52,15 +53,15 @@
                 "then the download step is also skipped."
             ),
             "type": str,
             "default": None,
         },
         {
             "long_flag": "--skip-download",
-            "help": "Skip data downlaod step.",
+            "help": "Skip data download step.",
             "default": False,
             "action": "store_true",
         },
         {
             "short_flag": "-d",
             "long_flag": "--diagnostics",
             "help": (
@@ -73,30 +74,42 @@
     ]
 
     def main(self, gmrecords):
         """Chain together subcommands to get shakemap ground motion file."""
         logging.info(f"Running subcommand '{self.command_name}'")
         self.gmrecords = gmrecords
         self._check_arguments()
-        self._get_events()
 
         # Hard code overwrite to True since this is all meant to run end-to-end
         # without interruption.
         gmrecords.args.overwrite = True
 
-        # Chain together relevant subcommand modules:
-        if (not gmrecords.args.skip_download) and (gmrecords.args.path is None):
-            download.DownloadModule().main(gmrecords)
-
-        if gmrecords.args.path is not None:
-            import_data.ImportModule().main(gmrecords)
-
-        assemble.AssembleModule().main(gmrecords)
-        process_waveforms.ProcessWaveformsModule().main(gmrecords)
-        compute_station_metrics.ComputeStationMetricsModule().main(gmrecords)
-        compute_waveform_metrics.ComputeWaveformMetricsModule().main(gmrecords)
-        export_shakemap.ExportShakeMapModule().main(gmrecords)
-
-        if gmrecords.args.diagnostics:
-            export_metric_tables.ExportMetricTablesModule().main(gmrecords)
-            generate_regression_plot.GenerateRegressionPlotModule().main(gmrecords)
-            generate_report.GenerateReportModule().main(gmrecords)
+        event_ids, events = self._get_event_ids_from_args()
+        if events:
+            logging.critical(
+                "autoshakemap subcommand only works with events given as ComCat ids."
+            )
+
+        for ievent, event_id in enumerate(event_ids):
+            logging.info(
+                f"(auto)processing event {event_id} ({1+ievent} of {len(event_ids)})..."
+            )
+            # stomp on gmrecords.args.event_id
+            gmrecords.args.event_id = [event_id]
+
+            # Chain together relevant subcommand modules:
+            if (not gmrecords.args.skip_download) and (gmrecords.args.path is None):
+                download.DownloadModule().main(gmrecords)
+
+            if gmrecords.args.path is not None:
+                import_data.ImportModule().main(gmrecords)
+
+            assemble.AssembleModule().main(gmrecords)
+            process_waveforms.ProcessWaveformsModule().main(gmrecords)
+            compute_station_metrics.ComputeStationMetricsModule().main(gmrecords)
+            compute_waveform_metrics.ComputeWaveformMetricsModule().main(gmrecords)
+            export_shakemap.ExportShakeMapModule().main(gmrecords)
+
+            if gmrecords.args.diagnostics:
+                export_metric_tables.ExportMetricTablesModule().main(gmrecords)
+                generate_regression_plot.GenerateRegressionPlotModule().main(gmrecords)
+                generate_report.GenerateReportModule().main(gmrecords)
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/base.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import sys
 from abc import ABC, abstractmethod
 import logging
 from pathlib import Path
 
 from gmprocess.subcommands.lazy_loader import LazyLoader
 
-base_utils = LazyLoader("base_utils", globals(), "gmprocess.utils.base_utils")
 confmod = LazyLoader("confmod", globals(), "gmprocess.utils.config")
 ws = LazyLoader("ws", globals(), "gmprocess.io.asdf.stream_workspace")
-const = LazyLoader("const", globals(), "gmprocess.utils.constants")
+constants = LazyLoader("constants", globals(), "gmprocess.utils.constants")
+scalar_event = LazyLoader("scalar_event", globals(), "gmprocess.core.scalar_event")
 
 
 class SubcommandModule(ABC):
     """gmprocess base module."""
 
     @property
     @abstractmethod
@@ -28,21 +28,21 @@
     """
     aliases = ()
 
     def __init__(self):
         """Dictionary instance variable to track files created by module."""
         self.files_created = {}
 
-    def open_workspace(self, eventid):
+    def open_workspace(self, event_id):
         """Open workspace, add as attribute."""
-        event_dir = Path(self.gmrecords.data_path) / eventid
-        workname = event_dir / const.WORKSPACE_NAME
+        event_dir = Path(self.gmrecords.data_path) / event_id
+        workname = event_dir / constants.WORKSPACE_NAME
         if not workname.is_file():
-            logging.info(
-                f"No workspace file found for event {eventid}. Please run subcommand "
+            logging.warning(
+                f"No workspace file found for event {event_id}. Please run subcommand "
                 "'assemble' to generate workspace file."
             )
             logging.info("Continuing to next event.")
             self.workspace = None
         else:
             self.workspace = ws.StreamWorkspace.open(workname)
 
@@ -92,14 +92,29 @@
         """
         args = self.gmrecords.args
         req_args = self.argugments_default_dict()
         for arg, val in req_args.items():
             if arg not in args:
                 args.__dict__.update({arg: val})
 
+    def _get_event_ids_from_args(self):
+        """Get event ids and events from arguments.
+
+        Returns:
+            Tuple with event ids (list) and events (ScalarEvent).
+        """
+        data_path = self.gmrecords.data_path
+        user_ids = self.gmrecords.args.event_id
+        events_filename = self.gmrecords.args.textfile
+        file_ids, events = scalar_event.get_events_from_file(events_filename)
+        event_ids = scalar_event.get_event_ids(
+            ids=user_ids, file_ids=file_ids, data_dir=data_path
+        )
+        return (event_ids, events)
+
     def append_file(self, tag, filename):
         """Convenience method to add file via tag to self.files_created."""
         if tag in self.files_created:
             self.files_created[tag].append(str(filename.resolve()))
         else:
             self.files_created[tag] = [str(filename.resolve())]
 
@@ -109,75 +124,24 @@
             for file_type, file_list in self.files_created.items():
                 logging.info(f"File type: {file_type}")
                 for fname in file_list:
                     logging.info(f"\t{fname}")
         else:
             logging.info("No new files created.")
 
-    def _get_pstreams(self):
+    def _get_pstreams(self, event_id):
         """Convenience method for recycled code."""
         self._get_labels()
         if self.gmrecords.args.label is None:
             return
 
         config = self._get_config()
 
         self.pstreams = self.workspace.get_streams(
-            self.eventid, labels=[self.gmrecords.args.label], config=config
-        )
-
-    def _get_events(self):
-        # NOTE: as currently written, `get_events` will do the following,
-        #  **stopping** at the first condition that is met:
-        #     1) Use event ids if event id is not None
-        #     2) Use textfile if it is not None
-        #     3) Use event info if it is not None
-        #     4) Use directory if it is not None
-        #     5) Use outdir if it is not None
-        # So in order to ever make use of the 'outdir' argument, we need to
-        # set 'directory' to None, but otherwise set it to proj_data_path.
-        #
-        # This whole thing is really hacky and should probably be completely
-        # rewritten.
-        if hasattr(self.gmrecords.args, "data_source"):
-            if self.gmrecords.args.data_source is None:
-                # Use project directory from config
-                temp_dir = self.gmrecords.data_path
-                if not temp_dir.is_dir():
-                    raise OSError(f"No such directory: {temp_dir}")
-            elif self.gmrecords.args.data_source == "download":
-                temp_dir = None
-            else:
-                temp_dir = self.gmrecords.args.data_source
-                if not temp_dir.is_dir():
-                    raise OSError(f"No such directory: {temp_dir}")
-            self.download_dir = temp_dir
-        else:
-            self.download_dir = None
-
-        info = (
-            self.gmrecords.args.info if hasattr(self.gmrecords.args, "info") else None
-        )
-        tfile = (
-            self.gmrecords.args.textfile
-            if hasattr(self.gmrecords.args, "textfile")
-            else None
-        )
-        if isinstance(self.gmrecords.args.eventid, str):
-            # Need to strip in case there is whitespace
-            self.gmrecords.args.eventid = [
-                eid.strip() for eid in self.gmrecords.args.eventid.split(",")
-            ]
-
-        self.events = base_utils.get_events(
-            eventids=self.gmrecords.args.eventid,
-            textfile=tfile,
-            eventinfo=info,
-            directory=self.download_dir,
-            outdir=self.gmrecords.data_path,
+            event_id, labels=[self.gmrecords.args.label], config=config
         )
 
     def _get_labels(self):
         labels = self.workspace.get_labels()
         if len(labels):
             labels.remove("unprocessed")
         if not len(labels):
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/clean.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/clean.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 import shutil
 
 from gmprocess.subcommands.lazy_loader import LazyLoader
 
 base = LazyLoader("base", globals(), "gmprocess.subcommands.base")
+scalar_event = LazyLoader("scalar_event", globals(), "gmprocess.core.scalar_event")
 
 
 class CleanModule(base.SubcommandModule):
     """Clean (i.e., remove) project data."""
 
     command_name = "clean"
 
@@ -65,15 +66,14 @@
 
         Args:
             gmrecords:
                 GMrecordsApp instance.
         """
         logging.info(f"Running subcommand '{self.command_name}'")
         self.gmrecords = gmrecords
-        self._get_events()
         self._check_arguments()
 
         # ---------------------------------------------------------------------
         # At the project level
         data_path = gmrecords.data_path
 
         # Exported tables
@@ -82,17 +82,18 @@
 
         # Regression
         if gmrecords.args.all or gmrecords.args.plot:
             self.__remove(data_path, ["*.png"])
 
         # ---------------------------------------------------------------------
         # Inside the event directories
-        logging.info(f"Number of events: {len(self.events)}")
-        for event in self.events:
-            event_dir = gmrecords.data_path / event.id
+        event_ids, _ = self._get_event_ids_from_args()
+        logging.info(f"Number of events: {len(event_ids)}")
+        for event_id in event_ids:
+            event_dir = gmrecords.data_path / event_id
             # Exported tables
             if gmrecords.args.all or gmrecords.args.export:
                 patterns = [
                     "*.xlsx",
                     "*.csv",
                     "*_groundmotions_dat.json",
                     "*_metrics.json",
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/compute_station_metrics.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/generate_report.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,140 +1,156 @@
-"""Module for ComputeStationMetricsModule class."""
+"""Module for GenerateReportModule class."""
 
 import logging
-import pathlib
+import shutil
+from concurrent.futures import ProcessPoolExecutor
 
 from gmprocess.subcommands.lazy_loader import LazyLoader
 
-np = LazyLoader("np", globals(), "numpy")
-ob = LazyLoader("ob", globals(), "obspy.geodetics.base")
-oqgeo = LazyLoader("oqgeo", globals(), "openquake.hazardlib.geo.geodetic")
-origin = LazyLoader("rupt", globals(), "esi_utils_rupture.origin")
 
-arg_dicts = LazyLoader("arg_dicts", globals(), "gmprocess.subcommands.arg_dicts")
 base = LazyLoader("base", globals(), "gmprocess.subcommands.base")
-utils = LazyLoader("utils", globals(), "gmprocess.utils")
-rupt_utils = LazyLoader("rupt_utils", globals(), "gmprocess.utils.rupture_utils")
-ws = LazyLoader("ws", globals(), "gmprocess.io.asdf.stream_workspace")
-sta_collection = LazyLoader(
-    "sta_collection", globals(), "gmprocess.metrics.station_metric_collection"
-)
-sta_xml = LazyLoader("sta_xml", globals(), "gmprocess.io.asdf.station_metrics_xml")
-confmod = LazyLoader("confmod", globals(), "gmprocess.utils.config")
+report = LazyLoader("report", globals(), "gmprocess.io.report")
+splot = LazyLoader("plot", globals(), "gmprocess.utils.summary_plots")
+mplot = LazyLoader("plot", globals(), "gmprocess.utils.misc_plots")
+constants = LazyLoader("constants", globals(), "gmprocess.utils.constants")
+scalar_event = LazyLoader("scalar_event", globals(), "gmprocess.core.scalar_event")
 
-M_PER_KM = 1000
 
+class GenerateReportModule(base.SubcommandModule):
+    """Generate summary report (latex required)."""
 
-class ComputeStationMetricsModule(base.SubcommandModule):
-    """Compute station metrics."""
-
-    command_name = "compute_station_metrics"
-    aliases = ("sm",)
+    command_name = "generate_report"
+    aliases = ("report",)
 
     arguments = []
 
     def main(self, gmrecords):
-        """Compute station metrics.
+        """Generate summary report.
+
+        This function generates summary plots and then combines them into a
+        report with latex. If latex (specifically `pdflatex`) is not found on
+        the system then the PDF report will not be generated but the
+        constituent plots will be available.
 
         Args:
             gmrecords:
                 GMrecordsApp instance.
         """
-        logging.info("Running subcommand '%s'", self.command_name)
+        logging.info(f"Running subcommand '{self.command_name}'")
 
         self.gmrecords = gmrecords
         self._check_arguments()
-        self._get_events()
+        event_ids, _ = self._get_event_ids_from_args()
+
+        for ievent, event_id in enumerate(event_ids):
+            event_dir = self.gmrecords.data_path / event_id
+            event = scalar_event.ScalarEvent.from_workspace(
+                event_dir / constants.WORKSPACE_NAME
+            )
+            config = self._get_config()
+            pstreams = self.generate_diagnostic_plots(event, config)
+            if pstreams is None:
+                return
 
-        for ievent, event in enumerate(self.events):
             logging.info(
-                "Computing station metrics for event %s (%s of %s)...",
-                event.id,
-                1 + ievent,
-                len(self.events),
+                f"Generating summary report for event {event_id} "
+                f"({1+ievent} of {len(event_ids)})..."
             )
-            self._event_station_metrics(event)
+
+            build_conf = config["build_report"]
+            if build_conf["enabled"]:
+                report_format = build_conf["format"]
+                if report_format == "latex":
+                    report_file, success = report.build_report_latex(
+                        pstreams,
+                        event_dir,
+                        event,
+                        prefix=f"{gmrecords.project_name}_{gmrecords.args.label}",
+                        config=config,
+                        gmprocess_version=gmrecords.gmprocess_version,
+                    )
+                else:
+                    report_file = ""
+                    success = False
+                if report_file.is_file() and success:
+                    self.append_file("Summary report", report_file)
 
         self._summarize_files_created()
 
-    def _event_station_metrics(self, event):
-        self.eventid = event.id
-        event_dir = self.gmrecords.data_path / self.eventid
-        workname = event_dir / utils.constants.WORKSPACE_NAME
-        if not workname.is_file():
-            logging.info(
-                "No workspace file found for event %s. Please run "
-                "subcommand 'assemble' to generate workspace file.",
-                self.eventid,
-            )
-            logging.info("Continuing to next event.")
-            return event.id
+    def generate_diagnostic_plots(self, event, config):
+        self.open_workspace(event.id)
+        if not self.workspace:
+            return
 
-        self.workspace = ws.StreamWorkspace.open(workname)
         ds = self.workspace.dataset
-        self._get_labels()
-        config = self._get_config()
-
         station_list = ds.waveforms.list()
-        if not len(station_list):
-            self.workspace.close()
-            return event.id
-
-        rupture_file = rupt_utils.get_rupture_file(event_dir)
-        origin_obj = origin.Origin(
-            {
-                "id": self.eventid,
-                "netid": "",
-                "network": "",
-                "lat": event.latitude,
-                "lon": event.longitude,
-                "depth": event.depth_km,
-                "locstring": "",
-                "mag": event.magnitude,
-                "time": event.time,
-            }
-        )
-        self.origin = origin_obj
+        if len(station_list) == 0:
+            logging.info("No processed waveforms available. No report generated.")
+            return []
 
-        if isinstance(rupture_file, pathlib.Path):
-            rupture_file = str(rupture_file)
+        self._get_labels()
+        if self.gmrecords.args.num_processes:
+            futures = []
+            executor = ProcessPoolExecutor(
+                max_workers=self.gmrecords.args.num_processes
+            )
 
+        logging.info(f"Creating diagnostic plots for event {event.id}...")
+        event_dir = self.gmrecords.data_path / event.id
+        plot_dir = event_dir / "plots"
+        if plot_dir.exists():
+            shutil.rmtree(plot_dir, ignore_errors=True)
+        plot_dir.mkdir()
+
+        results = []
+        pstreams = []
         for station_id in station_list:
             streams = self.workspace.get_streams(
                 event.id,
                 stations=[station_id],
                 labels=[self.gmrecords.args.label],
                 config=config,
             )
-            if not streams:
-                logging.error(
-                    "No matching streams found. Aborting computing station "
-                    "metrics for %s for %s.",
-                    station_id,
+            if not len(streams):
+                logging.info("No matching streams found. Cannot generate report.")
+                return
+            streams_raw = (
+                self.workspace.get_streams(
                     event.id,
+                    stations=[station_id],
+                    labels=["unprocessed"],
+                    config=config,
                 )
-                continue
-
-            for stream in streams:
-                if not stream.passed:
-                    continue
-
-                smc = sta_collection.StationMetricCollection.from_streams(
-                    [stream], event, config, rupture_file=rupture_file
-                )
-                # we know there is only one element in the station_metrics list because
-                # we only gave it one stream.
-                station_xml = sta_xml.StationMetricsXML(smc.station_metrics[0])
-                xmlstr = station_xml.to_xml()
-                self.workspace.insert_aux(
-                    xmlstr,
-                    "StationMetrics",
-                    smc.stream_paths[0],
-                    overwrite=self.gmrecords.args.overwrite,
-                )
-        logging.info(
-            "Added station metrics to workspace files with tag '%s'.",
-            self.gmrecords.args.label,
-        )
+                if "unprocessed" in self.workspace.get_labels()
+                else None
+            )
 
-        self.workspace.close()
-        return event.id
+            for stream, stream_raw in zip(streams, streams_raw):
+                pstreams.append(stream)
+                if self.gmrecords.args.num_processes > 0:
+                    future = executor.submit(
+                        _summary_plot,
+                        stream,
+                        stream_raw,
+                        plot_dir,
+                        event,
+                        config,
+                    )
+                    futures.append(future)
+                else:
+                    results.append(
+                        _summary_plot(stream, stream_raw, plot_dir, event, config)
+                    )
+
+        if self.gmrecords.args.num_processes:
+            # Collect the results??
+            results = [future.result() for future in futures]
+            executor.shutdown()
+
+        self.close_workspace()
+
+        return pstreams
+
+
+def _summary_plot(stream, stream_raw, plot_dir, event, config):
+    sp = splot.SummaryPlot(stream, stream_raw, plot_dir, event, config)
+    return sp.plot()
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/compute_waveform_metrics.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/compute_waveform_metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 import logging
 from concurrent.futures import ProcessPoolExecutor
 
 from gmprocess.subcommands.lazy_loader import LazyLoader
 
 arg_dicts = LazyLoader("arg_dicts", globals(), "gmprocess.subcommands.arg_dicts")
 base = LazyLoader("base", globals(), "gmprocess.subcommands.base")
-ws = LazyLoader("ws", globals(), "gmprocess.io.asdf.stream_workspace")
-const = LazyLoader("const", globals(), "gmprocess.utils.constants")
-confmod = LazyLoader("confmod", globals(), "gmprocess.utils.config")
+constants = LazyLoader("constants", globals(), "gmprocess.utils.constants")
+scalar_event = LazyLoader("scalar_event", globals(), "gmprocess.core.scalar_event")
 path_utils = LazyLoader("path_utils", globals(), "gmprocess.io.asdf.path_utils")
 wf_collection = LazyLoader(
     "wf_collection", globals(), "gmprocess.metrics.waveform_metric_collection"
 )
 wf_xml = LazyLoader("wf_xml", globals(), "gmprocess.io.asdf.waveform_metrics_xml")
 
 
@@ -32,69 +31,61 @@
             gmrecords:
                 GMrecordsApp instance.
         """
         logging.info("Running subcommand '%s'", self.command_name)
 
         self.gmrecords = gmrecords
         self._check_arguments()
-        self._get_events()
+        event_ids, _ = self._get_event_ids_from_args()
 
-        for ievent, event in enumerate(self.events):
+        for ievent, event_id in enumerate(event_ids):
             logging.info(
                 "Computing waveform metrics for event %s (%s of %s)...",
-                event.id,
+                event_id,
                 1 + ievent,
-                len(self.events),
+                len(event_ids),
             )
-            self._compute_event_waveform_metrics(event)
+            self._compute_event_waveform_metrics(event_id)
 
         self._summarize_files_created()
 
-    def _compute_event_waveform_metrics(self, event):
-        self.eventid = event.id
-        event_dir = self.gmrecords.data_path / self.eventid
-        workname = event_dir / const.WORKSPACE_NAME
-        if not workname.is_file():
-            logging.info(
-                "No workspace file found for event %s. Please run "
-                "subcommand 'assemble' to generate workspace file.",
-                self.eventid,
-            )
-            logging.info("Continuing to next event.")
-            return event.id
+    def _compute_event_waveform_metrics(self, event_id):
+        self.open_workspace(event_id)
+        if not self.workspace:
+            return
 
-        self.workspace = ws.StreamWorkspace.open(workname)
         ds = self.workspace.dataset
         station_list = ds.waveforms.list()
         self._get_labels()
         config = self._get_config()
+        event = self.workspace.get_event(event_id)
 
         # Start with an empty metric_collection and we will append to it.
         metric_collection = wf_collection.WaveformMetricCollection()
 
         if self.gmrecords.args.num_processes:
             futures = []
             executor = ProcessPoolExecutor(
                 max_workers=self.gmrecords.args.num_processes
             )
 
         for station_id in station_list:
             # Cannot parallelize IO to ASDF file
             streams = self.workspace.get_streams(
-                event.id,
+                event_id,
                 stations=[station_id],
                 labels=[self.gmrecords.args.label],
                 config=config,
             )
             if not streams:
                 logging.warning(
                     "No matching streams found. Aborting computation of station "
                     "metrics for %s for %s.",
                     station_id,
-                    event.id,
+                    event_id,
                 )
                 continue
 
             for stream in streams:
                 if not stream.passed:
                     continue
 
@@ -139,8 +130,7 @@
                 xmlstr,
                 "WaveFormMetrics",
                 metric_path,
                 overwrite=self.gmrecords.args.overwrite,
             )
 
         self.workspace.close()
-        return event.id
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/export_failure_tables.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/export_failure_tables.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from gmprocess.subcommands.lazy_loader import LazyLoader
 
 pd = LazyLoader("pd", globals(), "pandas")
 
 arg_dicts = LazyLoader("arg_dicts", globals(), "gmprocess.subcommands.arg_dicts")
 base = LazyLoader("base", globals(), "gmprocess.subcommands.base")
-ws = LazyLoader("ws", globals(), "gmprocess.io.asdf.stream_workspace")
-const = LazyLoader("const", globals(), "gmprocess.utils.constants")
+constants = LazyLoader("constants", globals(), "gmprocess.utils.constants")
+scalar_event = LazyLoader("scalar_event", globals(), "gmprocess.core.scalar_event")
 
 
 class ExportFailureTablesModule(base.SubcommandModule):
     """Export failure tables."""
 
     command_name = "export_failure_tables"
     aliases = ("ftables",)
@@ -51,51 +51,45 @@
             gmrecords:
                 GMrecordsApp instance.
         """
         logging.info(f"Running subcommand '{self.command_name}'")
 
         self.gmrecords = gmrecords
         self._check_arguments()
-        self._get_events()
+        event_ids, _ = self._get_event_ids_from_args()
 
         failures = {}
-        for ievent, event in enumerate(self.events):
-            self.eventid = event.id
+        for ievent, event_id in enumerate(event_ids):
             logging.info(
-                f"Creating failure tables for event {self.eventid} "
-                f"({1+ievent} of {len(self.events)})..."
+                f"Creating failure tables for event {event_id} "
+                f"({1+ievent} of {len(event_ids)})..."
             )
-            event_dir = self.gmrecords.data_path / self.eventid
-            workname = event_dir / const.WORKSPACE_NAME
-            if not workname.is_file():
-                logging.info(
-                    f"No workspace file found for event {self.eventid}. Please run "
-                    "subcommand 'assemble' to generate workspace file."
-                )
-                logging.info("Continuing to next event.")
+
+            self.open_workspace(event_id)
+            if not self.workspace:
                 continue
 
-            self.workspace = ws.StreamWorkspace.open(workname)
-            self._get_pstreams()
-            self.workspace.close()
+            self._get_pstreams(event_id)
+            self.close_workspace()
 
             if not (hasattr(self, "pstreams") and len(self.pstreams) > 0):
                 logging.info(
                     "No processed waveforms available. No failure tables created."
                 )
                 continue
 
             status_info = self.pstreams.get_status(self.gmrecords.args.type)
-            failures[event.id] = status_info
+            failures[event_id] = status_info
 
             base_file_name = (
                 f"{gmrecords.project_name}_{gmrecords.args.label}_"
                 f"failure_reasons_{self.gmrecords.args.type}"
             )
 
+            event_dir = gmrecords.data_path / event_id
             if self.gmrecords.args.output_format == "csv":
                 csvfile = base_file_name + ".csv"
                 csvpath = event_dir / csvfile
                 self.append_file("Failure table", csvpath)
                 status_info.to_csv(csvpath)
             else:
                 excelfile = base_file_name + ".xlsx"
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/export_metric_tables.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/export_metric_tables.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 
 import logging
 
 from gmprocess.subcommands.lazy_loader import LazyLoader
 
 arg_dicts = LazyLoader("arg_dicts", globals(), "gmprocess.subcommands.arg_dicts")
 base = LazyLoader("base", globals(), "gmprocess.subcommands.base")
-ws = LazyLoader("ws", globals(), "gmprocess.io.asdf.stream_workspace")
-const = LazyLoader("const", globals(), "gmprocess.utils.constants")
+constants = LazyLoader("constants", globals(), "gmprocess.utils.constants")
 tables = LazyLoader("tables", globals(), "gmprocess.utils.tables")
-confmod = LazyLoader("confmod", globals(), "gmprocess.utils.config")
+scalar_event = LazyLoader("scalar_event", globals(), "gmprocess.core.scalar_event")
 flat_mod = LazyLoader("flatmod", globals(), "gmprocess.io.asdf.flatfile")
 
 
 class ExportMetricTablesModule(base.SubcommandModule):
     """Export metric tables."""
 
     command_name = "export_metric_tables"
@@ -30,64 +29,53 @@
             gmrecords:
                 GMrecordsApp instance.
         """
         logging.info("Running subcommand '%s'", self.command_name)
 
         self.gmrecords = gmrecords
         self._check_arguments()
-        self._get_events()
+        event_ids, _ = self._get_event_ids_from_args()
 
-        for ievent, event in enumerate(self.events):
+        for ievent, event_id in enumerate(event_ids):
             logging.info(
                 "Creating tables for event %s (%s of %s)...",
-                event.id,
+                event_id,
                 1 + ievent,
-                len(self.events),
+                len(event_ids),
             )
-            self.eventid = event.id
-            event_dir = gmrecords.data_path / self.eventid
-            workname = event_dir / const.WORKSPACE_NAME
-            if not workname.is_file():
-                logging.warning(
-                    "No workspace file found for event %s. Please run subcommand "
-                    "'assemble' to generate workspace file. Continuing to next event.",
-                    self.eventid,
-                )
-                continue
 
-            self.workspace = ws.StreamWorkspace.open(workname)
+            self.open_workspace(event_id)
+            if not self.workspace:
+                continue
             self._get_labels()
-            config = self._get_config()
 
             if "StationMetrics" not in self.workspace.dataset.auxiliary_data:
                 logging.warning(
                     "Station metrics not found in workspace for event %s."
                     "Continuing to next event.",
-                    self.eventid,
+                    event_id,
                 )
                 continue
             if "WaveFormMetrics" not in self.workspace.dataset.auxiliary_data:
                 logging.warning(
                     "Waveform metrics not found in workspace for event %s."
                     "Continuing to next event.",
-                    self.eventid,
+                    event_id,
                 )
                 continue
 
             flatfile = flat_mod.Flatfile(self.workspace)
             event_table, imc_tables, readmes = flatfile.get_tables()
             ev_fit_spec, fit_readme = flatfile.get_fit_spectra_table()
 
             # We need to have a consistent set of frequencies for reporting the SNR.
             # For now, I'm going to take it from the SA period list, but this could be
             # changed to something else, or even be set via the config file.
             snr_table, snr_readme = flatfile.get_snr_table()
-            self.workspace.close()
-
-            outdir = gmrecords.data_path
+            self.close_workspace()
 
             # Set the precisions for the imc tables, event table, and
             # fit_spectra table before writing
             imc_tables_formatted = {}
             for imc, imc_table in imc_tables.items():
                 imc_tables_formatted[imc] = tables.set_precisions(imc_table)
             event_table_formatted = tables.set_precisions(event_table)
@@ -129,15 +117,15 @@
             output_format = gmrecords.args.output_format
             if output_format != "csv":
                 output_format = "xlsx"
 
             for filename, df in dict(zip(filenames, files)).items():
                 if df is None or df.size == 0:
                     continue
-                filepath = outdir / (filename + f".{output_format}")
+                filepath = gmrecords.data_path / (filename + f".{output_format}")
                 if filepath.exists():
                     if "README" in filename:
                         continue
                     else:
                         if self.gmrecords.args.overwrite:
                             logging.info("Overwriting file: %s", filename)
                             mode = "w"
@@ -149,27 +137,27 @@
                 else:
                     mode = "w"
                     header = True
                 if output_format == "csv":
                     df.to_csv(
                         filepath,
                         index=False,
-                        float_format=const.DEFAULT_FLOAT_FORMAT,
-                        na_rep=const.DEFAULT_NA_REP,
+                        float_format=constants.DEFAULT_FLOAT_FORMAT,
+                        na_rep=constants.DEFAULT_NA_REP,
                         mode=mode,
                         header=header,
                     )
                     if mode == "w":
                         self.append_file("Metric tables", filepath)
                 else:
                     df.to_excel(
                         filepath,
                         index=False,
-                        float_format=const.DEFAULT_FLOAT_FORMAT,
-                        na_rep=const.DEFAULT_NA_REP,
+                        float_format=constants.DEFAULT_FLOAT_FORMAT,
+                        na_rep=constants.DEFAULT_NA_REP,
                         mode=mode,
                         header=header,
                     )
                     if mode == "w":
                         self.append_file("Metric tables", filepath)
 
         self._summarize_files_created()
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/export_provenance_tables.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/export_shakemap.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,78 +1,77 @@
-"""Module for ExportProvenanceTablesModule class."""
+"""Module for ExportShakeMapModule class."""
 
 import logging
 
 from gmprocess.subcommands.lazy_loader import LazyLoader
 
 arg_dicts = LazyLoader("arg_dicts", globals(), "gmprocess.subcommands.arg_dicts")
 base = LazyLoader("base", globals(), "gmprocess.subcommands.base")
-ws = LazyLoader("ws", globals(), "gmprocess.io.asdf.stream_workspace")
-const = LazyLoader("const", globals(), "gmprocess.utils.constants")
+constants = LazyLoader("constants", globals(), "gmprocess.utils.constants")
+sm_utils = LazyLoader("sm_utils", globals(), "gmprocess.utils.export_shakemap_utils")
+scalar_event = LazyLoader("scalar_event", globals(), "gmprocess.core.scalar_event")
 
 
-class ExportProvenanceTablesModule(base.SubcommandModule):
-    """Export provenance tables."""
+class ExportShakeMapModule(base.SubcommandModule):
+    """Export files for ShakeMap input."""
 
-    command_name = "export_provenance_tables"
-    aliases = ("ptables",)
+    command_name = "export_shakemap"
+    aliases = ("shakemap",)
 
     arguments = [
-        arg_dicts.ARG_DICTS["output_format"],
+        {
+            "short_flag": "-x",
+            "long_flag": "--expand-imts",
+            "help": (
+                "Use expanded IMTs. Currently this only means all the "
+                "SA that have been computed, plus PGA and PGV (if "
+                "computed). Could eventually expand for other IMTs also."
+            ),
+            "default": False,
+            "action": "store_true",
+        },
     ]
 
     def main(self, gmrecords):
-        """Export provenance tables.
+        """Export files for ShakeMap input.
 
         Args:
             gmrecords:
                 GMrecordsApp instance.
         """
         logging.info(f"Running subcommand '{self.command_name}'")
 
         self.gmrecords = gmrecords
         self._check_arguments()
-        self._get_events()
+        event_ids, _ = self._get_event_ids_from_args()
 
-        for ievent, event in enumerate(self.events):
-            self.eventid = event.id
+        for ievent, event_id in enumerate(event_ids):
             logging.info(
-                f"Creating provenance tables for event {self.eventid} "
-                f"({1+ievent} of {len(self.events)})..."
+                f"Creating shakemap files for event {event_id} "
+                f"({1+ievent} of {len(event_ids)})..."
             )
-            event_dir = gmrecords.data_path / self.eventid
 
-            workname = event_dir / const.WORKSPACE_NAME
-            if not workname.is_file():
-                logging.info(
-                    f"No workspace file found for event {self.eventid}. Please run "
-                    "subcommand 'assemble' to generate workspace file."
-                )
-                logging.info("Continuing to next event.")
+            self.open_workspace(event_id)
+            if not self.workspace:
                 continue
-
-            self.workspace = ws.StreamWorkspace.open(workname)
-            self._get_pstreams()
-
-            if not (hasattr(self, "pstreams") and len(self.pstreams) > 0):
-                logging.info(
-                    "No processed waveforms available. No provenance tables created."
-                )
-                self.workspace.close()
-                continue
-
-            provdata = self.workspace.get_provenance(
-                self.eventid, labels=self.gmrecords.args.label
+            self._get_labels()
+            config = self._get_config()
+            event_dir = gmrecords.data_path / event_id
+            event = self.workspace.get_event(event_id)
+
+            expanded_imts = self.gmrecords.args.expand_imts
+            jsonfile, stationfile, _ = sm_utils.create_json(
+                self.workspace,
+                event,
+                event_dir,
+                self.gmrecords.args.label,
+                config=config,
+                expanded_imts=expanded_imts,
             )
-            self.workspace.close()
 
-            basename = f"{gmrecords.project_name}_{gmrecords.args.label}_provenance"
-            if gmrecords.args.output_format == "csv":
-                csvfile = event_dir / f"{basename}.csv"
-                self.append_file("Provenance", csvfile)
-                provdata.to_csv(csvfile, index=False)
-            else:
-                excelfile = event_dir / f"{basename}.xlsx"
-                self.append_file("Provenance", excelfile)
-                provdata.to_excel(excelfile, index=False)
+            self.close_workspace()
+            if jsonfile is not None:
+                self.append_file("shakemap", jsonfile)
+            if stationfile is not None:
+                self.append_file("shakemap", stationfile)
 
         self._summarize_files_created()
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/generate_regression_plot.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/generate_regression_plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,53 +70,52 @@
         if not len(imc_tables):
             msg = """No IMC tables found. It is likely that no streams
             passed checks. If you created reports for the events you
             have been processing, check those to see if this is the case,
             then adjust your configuration as necessary to process the data.
             """
             logging.warning(msg)
-        else:
-            pref_imcs = [
-                "rotd50.0",
-                "greater_of_two_horizontals",
-                "h1",
-                "h2",
-            ]
-            pref_imts = ["PGA", "PGV", "SA(1.000)"]
-            found_imc = None
-            found_imt = None
-            tab_key_list = list(imc_tables.keys())
-            tab_key_imcs = [k.split("_")[-1] for k in tab_key_list]
-            tab_key_dict = dict(zip(tab_key_imcs, tab_key_list))
-            for imc in pref_imcs:
-                if imc in tab_key_imcs:
-                    for imt in pref_imts:
-                        if imt in imc_tables[tab_key_dict[imc]].columns:
-                            found_imt = imt
-                            found_imc = imc
-                            break
-                    if found_imc:
+            return
+        pref_imcs = [
+            "rotd(percentile=50.0)",
+            "channels(component=h1)",
+            "channels(component=h2)",
+        ]
+        pref_imts = ["PGA", "PGV", "SA(1.000)"]
+        found_imc = None
+        found_imt = None
+        tab_key_list = list(imc_tables.keys())
+        tab_key_imcs = [k.split("_")[-1] for k in tab_key_list]
+        tab_key_dict = dict(zip(tab_key_imcs, tab_key_list))
+        for imc in pref_imcs:
+            if imc in tab_key_imcs:
+                for imt in pref_imts:
+                    if imt in imc_tables[tab_key_dict[imc]].columns:
+                        found_imt = imt
+                        found_imc = imc
                         break
+                if found_imc:
+                    break
 
-            # now look for whatever IMC/IMTcombination we can find
-            if imc_tables and not found_imc:
-                found_imc = list(imc_tables.keys())[0]
-                table_cols = set(imc_tables[found_imc].columns)
-                imtlist = list(table_cols - const.NON_IMT_COLS)
-                found_imt = imtlist[0]
+        # now look for whatever IMC/IMTcombination we can find
+        if imc_tables and not found_imc:
+            found_imc = list(imc_tables.keys())[0]
+            table_cols = set(imc_tables[found_imc].columns)
+            imtlist = list(table_cols - const.NON_IMT_COLS)
+            found_imt = imtlist[0]
 
-            if found_imc and found_imt:
-                pngfile = f"regression_{found_imc}_{found_imt}.png"
-                regression_file = self.gmrecords.data_path / pngfile
+        if found_imc and found_imt:
+            pngfile = f"regression_{found_imc}_{found_imt}.png"
+            regression_file = self.gmrecords.data_path / pngfile
 
-                plot.plot_regression(
-                    event_table,
-                    found_imc,
-                    imc_tables[tab_key_dict[found_imc]],
-                    found_imt,
-                    regression_file,
-                    distance_metric="EpicentralDistance",
-                    colormap="viridis_r",
-                )
-                self.append_file("Multi-event regression plot", regression_file)
+            plot.plot_regression(
+                event_table,
+                found_imc,
+                imc_tables[tab_key_dict[found_imc]],
+                found_imt,
+                regression_file,
+                distance_metric="EpicentralDistance",
+                colormap="viridis_r",
+            )
+            self.append_file("Multi-event regression plot", regression_file)
 
         self._summarize_files_created()
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/generate_station_maps.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/generate_station_maps.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Module for GenerateHTMLMapModule class."""
 
 import logging
 
 from gmprocess.subcommands.lazy_loader import LazyLoader
 
 base = LazyLoader("base", globals(), "gmprocess.subcommands.base")
-ws = LazyLoader("ws", globals(), "gmprocess.io.asdf.stream_workspace")
-const = LazyLoader("const", globals(), "gmprocess.utils.constants")
+constants = LazyLoader("constants", globals(), "gmprocess.utils.constants")
 report_utils = LazyLoader("report_utils", globals(), "gmprocess.utils.report_utils")
+scalar_event = LazyLoader("scalar_event", globals(), "gmprocess.core.scalar_event")
 
 
 class GenerateHTMLMapModule(base.SubcommandModule):
     """Generate interactive station maps."""
 
     command_name = "generate_station_maps"
     aliases = ("maps",)
@@ -27,55 +27,52 @@
             gmrecords:
                 GMrecordsApp instance.
         """
         logging.info(f"Running subcommand '{self.command_name}'")
 
         self.gmrecords = gmrecords
         self._check_arguments()
-        self._get_events()
+        event_ids, _ = self._get_event_ids_from_args()
 
-        for ievent, event in enumerate(self.events):
-            event_dir = self.gmrecords.data_path / event.id
-            workname = event_dir / const.WORKSPACE_NAME
-            if not workname.is_file():
-                logging.error(
-                    f"No workspace file found for event {event.id}. Please run "
-                    "subcommand 'assemble' to generate workspace file."
-                    "Continuing to next event."
-                )
-                continue
+        for ievent, event_id in enumerate(event_ids):
+            event_dir = self.gmrecords.data_path / event_id
 
-            self.workspace = ws.StreamWorkspace.open(workname)
+            self.open_workspace(event_id)
+            if not self.workspace:
+                continue
             ds = self.workspace.dataset
             station_list = ds.waveforms.list()
             if len(station_list) == 0:
                 logging.info("No processed waveforms available. No report generated.")
                 continue
 
             self._get_labels()
             config = self.workspace.config
             logging.info(
-                f"Generating station maps for event {event.id} "
-                f"({1+ievent} of {len(self.events)})..."
+                f"Generating station maps for event {event_id} "
+                f"({1+ievent} of {len(event_ids)})..."
             )
 
             pstreams = []
             for station_id in station_list:
                 streams = self.workspace.get_streams(
-                    event.id,
+                    event_id,
                     stations=[station_id],
                     labels=[self.gmrecords.args.label],
                     config=config,
                 )
                 if not len(streams):
                     logging.error(
-                        f"No matching streams found for {station_id} for {event.id}."
+                        f"No matching streams found for {station_id} for {event_id}."
                     )
                     continue
 
                 for stream in streams:
                     pstreams.append(stream)
 
+            event = self.workspace.get_event(event_id)
+            self.close_workspace()
+
             mapfile = report_utils.draw_stations_map(pstreams, event, event_dir)
             self.append_file("Station map", mapfile)
 
         self._summarize_files_created()
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/import_data.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/import_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -36,40 +36,38 @@
         """
         logging.info(f"Running subcommand '{self.command_name}'")
         self.gmrecords = gmrecords
         self._check_arguments()
 
         import_path = Path(self.gmrecords.args.path)
 
-        self._get_events()
-
-        if self.events is None:
+        event_ids = [
+            event_id.strip() for event_id in self.gmrecords.args.event_id.split(",")
+        ]
+        if event_ids is None:
             raise ValueError("Please provide a valid event id.")
 
-        if len(self.events) > 1:
+        if len(event_ids) > 1:
             raise ValueError("Can only import data for one event at a time.")
+        event_id = event_ids[0]
 
-        logging.info(f"Number of events to download: {len(self.events)}")
-        for ievent, event in enumerate(self.events):
-            logging.info(
-                f"Importing event {event.id} ({1+ievent} of {len(self.events)})..."
-            )
-            event_dir = gmrecords.data_path / event.id
-            event_dir.mkdir(exist_ok=True)
-
-            raw_dir = event_dir / "raw"
-            raw_dir.mkdir(exist_ok=True)
-
-            if import_path.is_file():
-                import_file = import_path.name
-                src = import_path
-                dst = raw_dir / import_file
-                logging.info(f"Importing {str(src)}")
-                shutil.copy(src, dst)
-            elif import_path.is_dir():
-                src = import_path
-                dst = raw_dir
-                copy_tree(str(src), str(dst))
-            else:
-                raise ValueError("Please provide a valid path to a file or directory")
-            flatten_directory(raw_dir)
-            logging.info(f"Event {event.id} complete.")
+        logging.info(f"Importing event {event_id}...")
+        event_dir = gmrecords.data_path / event_id
+        event_dir.mkdir(exist_ok=True)
+
+        raw_dir = event_dir / "raw"
+        raw_dir.mkdir(exist_ok=True)
+
+        if import_path.is_file():
+            import_file = import_path.name
+            src = import_path
+            dst = raw_dir / import_file
+            logging.info(f"Importing {str(src)}")
+            shutil.copy(src, dst)
+        elif import_path.is_dir():
+            src = import_path
+            dst = raw_dir
+            copy_tree(str(src), str(dst))
+        else:
+            raise ValueError("Please provide a valid path to a file or directory")
+        flatten_directory(raw_dir)
+        logging.info(f"Importing event {event_id} complete.")
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/init.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/init.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/lazy_loader.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/process_waveforms.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/process_waveforms.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,20 +3,19 @@
 import logging
 from concurrent.futures import ProcessPoolExecutor
 
 from gmprocess.subcommands.lazy_loader import LazyLoader
 
 
 base = LazyLoader("base", globals(), "gmprocess.subcommands.base")
-const = LazyLoader("const", globals(), "gmprocess.utils.constants")
-ws = LazyLoader("ws", globals(), "gmprocess.io.asdf.stream_workspace")
+constants = LazyLoader("constants", globals(), "gmprocess.utils.constants")
+scalar_event = LazyLoader("scalar_event", globals(), "gmprocess.core.scalar_event")
 processing = LazyLoader(
     "processing", globals(), "gmprocess.waveform_processing.processing"
 )
-confmod = LazyLoader("confmod", globals(), "gmprocess.utils.config")
 
 
 class ProcessWaveformsModule(base.SubcommandModule):
     """Process waveform data."""
 
     command_name = "process_waveforms"
     aliases = ("process",)
@@ -40,67 +39,70 @@
             gmrecords:
                 GMrecordsApp instance.
         """
         logging.info(f"Running subcommand '{self.command_name}'")
 
         self.gmrecords = gmrecords
         self._check_arguments()
-        self._get_events()
+
+        event_ids, _ = self._get_event_ids_from_args()
+        logging.info(f"Number of events to process: {len(event_ids)}")
 
         # get the process tag from the user or use "default" for tag
         self.process_tag = gmrecords.args.label or "default"
         logging.info(f"Processing tag: {self.process_tag}")
 
-        for ievent, event in enumerate(self.events):
+        for ievent, event_id in enumerate(event_ids):
             logging.info(
-                f"Processing waveforms for event {event.id} "
-                f"({1+ievent} of {len(self.events)})..."
+                f"Processing waveforms for event {event_id} "
+                f"({1+ievent} of {len(event_ids)})..."
             )
-            self._process_event(event)
+            self._process_event(event_id)
 
         self._summarize_files_created()
 
-    def _process_event(self, event):
-        self.open_workspace(event.id)
+    def _process_event(self, event_id):
+        self.open_workspace(event_id)
         if self.workspace is None:
             return
         ds = self.workspace.dataset
         station_list = ds.waveforms.list()
+        event = self.workspace.get_event(event_id)
 
         processed_streams = []
         if self.gmrecords.args.num_processes:
             futures = []
             executor = ProcessPoolExecutor(
                 max_workers=self.gmrecords.args.num_processes
             )
 
         if self.gmrecords.args.reprocess:
             process_type = "Reprocessing"
             plabel = self.process_tag
         else:
             process_type = "Processing"
             plabel = "unprocessed"
-        logging.info(f"{process_type} '{plabel}' streams for event {event.id}...")
+        logging.info(f"{process_type} '{plabel}' streams for event {event_id}...")
 
         for station_id in station_list:
             # Cannot parallelize IO to ASDF file
             config = self._get_config()
             raw_streams = self.workspace.get_streams(
-                event.id,
+                event_id,
                 stations=[station_id],
                 labels=["unprocessed"],
                 config=config,
             )
             if self.gmrecords.args.reprocess:
                 # Don't use "processed_streams" variable name because that is what is
                 # being used for the result of THIS round of processing; thus, I'm
                 # using "old_streams" for the previously processed streams which
                 # contain the manually reviewed information
                 old_streams = self.workspace.get_streams(
-                    event.id,
+                    event_id,
                     stations=[station_id],
                     labels=[self.process_tag],
                     config=config,
                 )
                 logging.debug(old_streams.describe())
             else:
                 old_streams = None
@@ -139,8 +141,8 @@
                 processed_stream,
                 label=self.process_tag,
                 gmprocess_version=self.gmrecords.gmprocess_version,
                 overwrite=overwrite,
             )
 
         self.close_workspace()
-        return event.id
+        return event_id
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/processing_steps.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/processing_steps.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 """Module for the processing_stepsModule class."""
 
 import logging
 import collections
+import inspect
 
 from gmprocess.subcommands.lazy_loader import LazyLoader
 
 base = LazyLoader("base", globals(), "gmprocess.subcommands.base")
 STEPS = LazyLoader("steps", globals(), "gmprocess.waveform_processing.processing_step")
 
 
 class processing_stepsModule(base.SubcommandModule):
     """Print a summary of the currently available processing steps."""
 
     epilog = """
     These are the processing steps that can be included in the `processing` section of
     the config file.
+
+    The "myst" output type is useful for building docs.
     """
 
     command_name = "processing_steps"
     aliases = ()
 
     # Note: do not use the ARG_DICT entry for label because the explanation is
     # different here.
     arguments = [
         {
             "short_flag": "-o",
-            "long_flag": "--output-markdown",
-            "help": ("File path to save output, formated as markdown."),
+            "long_flag": "--output-type",
+            "help": "File path to save output, formated as markdown.",
+            "default": None,
+            "type": str,
+            "choices": ["text", "myst"],
+        },
+        {
+            "short_flag": "-p",
+            "long_flag": "--path",
+            "help": "File path to save output. If unset, then uses standard out.",
             "default": None,
             "type": str,
         },
     ]
 
     def main(self, gmrecords):
         """Summarize available processing steps and their arguments.
@@ -42,21 +53,31 @@
         logging.info(f"Running subcommand '{self.command_name}'")
 
         steps = STEPS.collect_processing_steps()
         osteps = collections.OrderedDict(
             sorted(steps.items(), key=lambda tup: tup[0].lower())
         )
 
-        if gmrecords.args.output_markdown is None:
+        if gmrecords.args.path is None:
             for step, func in osteps.items():
                 print("")
                 print(step)
                 print("=" * len(step))
+                print(f"{func.__name__}{inspect.signature(func)}\n")
                 print(func.__doc__)
         else:
-            with open(gmrecords.args.output_markdown, "w") as out:
-                for step, func in osteps.items():
-                    out.write("\n")
-                    out.write("## " + step + "\n")
-                    out.write("```\n")
-                    out.write(func.__doc__ + "\n")
-                    out.write("```\n")
+            if gmrecords.args.output_type == "myst":
+                with open(gmrecords.args.path, "w") as out:
+                    for step, func in osteps.items():
+                        out.write("```{eval-rst}\n")
+                        func_path = f"{func.__module__}.{func.__name__}"
+                        out.write(f".. autofunction:: {func_path}\n")
+                        out.write("```\n")
+            else:
+                with open(gmrecords.args.path, "w") as out:
+                    for step, func in osteps.items():
+                        out.write("\n")
+                        out.write(f"{step}\n")
+                        out.write(f"{'=' * len(step)}\n")
+                        out.write(f"{func.__name__}{inspect.signature(func)}\n\n")
+                        out.write(f"{func.__doc__}\n")
+                        out.write("\n")
```

### Comparing `gmprocess-1.3.2/src/gmprocess/subcommands/projects.py` & `gmprocess-2.0.0/src/gmprocess/subcommands/projects.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import logging
 import os
 import pathlib
 import platform
 import shutil
 import sys
-from pathlib import Path
 
 from esi_utils_io.cmd import get_command_output
 from gmprocess.subcommands.lazy_loader import LazyLoader
 
 ryaml = LazyLoader("yaml", globals(), "ruamel.yaml")
 base = LazyLoader("base", globals(), "gmprocess.subcommands.base")
 constants = LazyLoader("constants", globals(), "gmprocess.utils.constants")
@@ -229,15 +228,15 @@
         self.config.write()
         print(f"\nCurrent {current_project}")
 
     def create_project(self):
         if not self.config:
             self.config = configobj.ConfigObj(encoding="utf-8")
             self.config.filename = self.config_filepath
-        use_cwd = self.config_filepath.parent.parent == Path.cwd()
+        use_cwd = self.config_filepath.parent.parent == pathlib.Path.cwd()
         create(self.config, use_cwd)
 
     def rename_project(self, source, target):
         self._check_project_name(source)
         self.config["projects"][target] = self.config["projects"].pop(source)
         if self.config["project"] == source:
             self.config["project"] = target
@@ -277,16 +276,16 @@
         self.filename = filename
         self.conf_path = indict["conf_path"]
         self.data_path = indict["data_path"]
         self.current_marker = CURRENT_MARKERS[is_current]
 
     def __repr__(self):
         fmt = "Project: %s %s\n\tConf Path: %s\n\tData Path: %s"
-        cpath = (Path(self.filename).parent / self.conf_path).resolve()
-        dpath = (Path(self.filename).parent / self.data_path).resolve()
+        cpath = (pathlib.Path(self.filename).parent / self.conf_path).resolve()
+        dpath = (pathlib.Path(self.filename).parent / self.data_path).resolve()
         tpl = (self.name, self.current_marker, cpath, dpath)
         return fmt % tpl
 
     @staticmethod
     def from_config(config, name):
         """Create Project from projects configuration.
 
@@ -403,49 +402,49 @@
             f"Project '{project}' already exists.  Run 'gmrecords projects "
             "-l' to see existing projects."
         )
         logging.error(msg)
         return
 
     if use_cwd:
-        cwd = Path.cwd()
+        cwd = pathlib.Path.cwd()
         default_conf_path = cwd / "conf"
         default_data_path = cwd / "data"
     else:
-        project_path = Path("~").expanduser() / "gmprocess_projects" / project
+        project_path = pathlib.Path("~").expanduser() / "gmprocess_projects" / project
         default_conf_path = project_path / "conf"
         default_data_path = project_path / "data"
     conf_path = prompt.get_directory("conf", default_conf_path).resolve()
     data_path = prompt.get_directory("data", default_data_path).resolve()
     conf_path.mkdir(parents=True, exist_ok=True)
     data_path.mkdir(parents=True, exist_ok=True)
 
     user_info = prompt.get_user_info()
     if not user_info:
         sys.exit(1)
 
     # Apparently, relpath doesn't work for Windows, at least with the Azure
     # CI builds
     if platform.system() != "Windows" and use_cwd:
-        rel_path_loc = Path(config.filename).parents[1]
+        rel_path_loc = pathlib.Path(config.filename).parents[1]
         conf_relpath = str(".." / conf_path.relative_to(rel_path_loc))
         data_relpath = str(".." / data_path.relative_to(rel_path_loc))
     else:
         conf_relpath = conf_path
         data_relpath = data_path
 
     if "projects" not in config:
         config["projects"] = {}
     config["projects"][project] = {
         "conf_path": conf_relpath,
         "data_path": data_relpath,
     }
     config["project"] = project
 
-    Path(config.filename).parent.mkdir(exist_ok=True)
+    pathlib.Path(config.filename).parent.mkdir(exist_ok=True)
     config.write()
     proj = Project.from_config(config, project)
     print(f"\nCreated {proj}")
 
     yaml = ryaml.YAML()
     yaml.indent(mapping=4)
     yaml.preserve_quotes = True
```

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/args.py` & `gmprocess-2.0.0/src/gmprocess/utils/args.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/config.py` & `gmprocess-2.0.0/src/gmprocess/utils/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Module for handling configuration options."""
 
 import logging
 import os
 
-import numpy as np
 from ruamel.yaml import YAML
 from ruamel.yaml.error import YAMLError
 from schema import Optional, Or, Schema
 
 from gmprocess.utils import constants
 
 CONF_SCHEMA = Schema(
     {
+        "version": int,
         "user": {"name": str, "email": str},
         "fetchers": {
             "search_parameters": {
                 "enabled": bool,
                 "duration": {
                     "c0": float,
                     "c1": float,
@@ -131,47 +131,42 @@
             "max_dist_tolerance": float,
             "preference_order": list,
             "process_level_preference": list,
             "format_preference": list,
         },
         "build_report": {"enabled": True, "format": "latex"},
         "metrics": {
-            "output_imcs": list,
-            "output_imts": list,
-            "sa": {
-                "damping": float,
-                "periods": {
-                    "start": float,
-                    "stop": float,
-                    "num": int,
-                    "spacing": str,
-                    "use_array": bool,
-                    "defined_periods": list,
+            "components_and_types": dict,
+            "type_parameters": {
+                "sa": {
+                    "damping": list,
+                    "periods": list,
                 },
-            },
-            "fas": {
-                "smoothing": str,
-                "bandwidth": float,
-                "allow_nans": bool,
-                "periods": {
-                    "start": float,
-                    "stop": float,
-                    "num": int,
-                    "spacing": str,
-                    "use_array": bool,
-                    "defined_periods": list,
+                "fas": {
+                    "smoothing_method": str,
+                    "smoothing_parameter": float,
+                    "allow_nans": bool,
+                    "frequencies": {
+                        "start": float,
+                        "stop": float,
+                        "num": int,
+                    },
                 },
+                "duration": {"intervals": list},
             },
-            "duration": {"intervals": list},
+            "component_parameters": {"rotd": {"percentiles": list}},
         },
         "integration": {
             "frequency": bool,
             "initial": float,
             "demean": bool,
-            "taper": {"taper": bool, "type": str, "width": float, "side": str},
+            "taper": bool,
+            "taper_width": float,
+            "taper_type": str,
+            "taper_side": str,
         },
         "gmm_selection": {
             "ActiveShallow": str,
             "ActiveDeep": str,
             "VolcanicShallow": str,
             "SubductionIntraslab": str,
             "SubductionInterface": str,
@@ -345,56 +340,7 @@
 
 
 def __conf_path_to_config(config_path, default_config):
     conf_files = config_path.glob("**/*.yml")
     for cf in conf_files:
         default_config = update_config(cf, default_config)
     return default_config
-
-
-def get_config_imts_imcs(conf):
-    """Method to extract imt and imc lists from config.
-
-    Args:
-        conf (dict):
-            Config options.
-    """
-    metrics = conf["metrics"]
-    config_imts = [imt.lower() for imt in metrics["output_imts"]]
-    imcs = [imc.lower() for imc in metrics["output_imcs"]]
-    # append periods for sa and fas, interval for duration
-    imts = []
-    for imt in config_imts:
-        if imt == "sa":
-            if metrics["sa"]["periods"]["use_array"]:
-                start = metrics["sa"]["periods"]["start"]
-                stop = metrics["sa"]["periods"]["stop"]
-                num = metrics["sa"]["periods"]["num"]
-                if metrics["sa"]["periods"]["spacing"] == "logspace":
-                    periods = np.logspace(np.log10(start), np.log10(stop), num=num)
-                else:
-                    periods = np.linspace(start, stop, num=num)
-                for period in periods:
-                    imts += ["sa" + str(period)]
-            else:
-                for period in metrics["sa"]["periods"]["defined_periods"]:
-                    imts += ["sa" + str(period)]
-        elif imt == "fas":
-            if metrics["fas"]["periods"]["use_array"]:
-                start = metrics["fas"]["periods"]["start"]
-                stop = metrics["fas"]["periods"]["stop"]
-                num = metrics["fas"]["periods"]["num"]
-                if metrics["fas"]["periods"]["spacing"] == "logspace":
-                    periods = np.logspace(np.log10(start), np.log10(stop), num=num)
-                else:
-                    periods = np.linspace(start, stop, num=num)
-                for period in periods:
-                    imts += ["fas" + str(period)]
-            else:
-                for period in metrics["fas"]["periods"]["defined_periods"]:
-                    imts += ["fas" + str(period)]
-        elif imt == "duration":
-            for interval in metrics["duration"]["intervals"]:
-                imts += ["duration" + interval]
-        else:
-            imts += [imt]
-    return imts, imcs
```

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/constants.py` & `gmprocess-2.0.0/src/gmprocess/utils/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,43 +12,56 @@
 PROJECTS_PATH = (pathlib.Path("~").expanduser() / PROJ_CONF_DIR).resolve()
 
 CONFIG_PATH_TEST = (pathlib.Path("~").expanduser() / "gmptest").resolve()
 CONFIG_FILE_PRODUCTION = "config_production.yml"
 CONFIG_FILE_TEST = "config_test.yml"
 PICKER_FILE = "picker.yml"
 MODULE_FILE = "modules.yml"
+EVENT_FILE = "event.json"
 RUPTURE_FILE = "rupture.json"
+STREC_FILE = "strec_results.json"
 
 STREC_CONFIG_PATH = pathlib.Path.home() / ".strec" / "config.ini"
 
 GAL_TO_PCTG = 1.0 / sp.g
 M_PER_KM = 1000
 M_TO_CM = 100.0
 
 WORKSPACE_NAME = "workspace.h5"
 WORKSPACE_NAME_OLD = "workspace.hdf"
 
 
+UNIT_TYPES = {"acc": "cm/s^2", "vel": "cm/s"}
+
 UNITS = {
     "pga": "%g",
     "pgv": "cm/s",
     "sa": "%g",
-    "ariasintensity": "m/s",
+    "arias": "m/s",
+    "cav": "g-s",
     "fas": "cm/s",
     "duration": "s",
     "sortedduration": "s",
 }
 
+REVERSE_UNITS = {
+    "cm/s^2": "acc",
+    "cm/s**2": "acc",
+    "cm/s/s": "acc",
+    "cm/s": "vel",
+    "cm": "disp",
+}
+
 DIMENSION_UNITS = {
     "period": "s",
     "damping": "%",
     "start percentage": "%",
     "end percentage": "%",
-    "smoothing": "",
-    "method": "",
+    "smoothing_method": "",
+    "smoothing_parameter": "",
 }
 
 STATION_METRIC_UNITS = {
     "repi": "km",
     "rhyp": "km",
     "rrup_mean": "km",
     "rrup_var": "km",
@@ -96,18 +109,20 @@
 
 # Formats for storing floating point numbers as strings for the
 # WaveFormMetrics and StationMetrics XMLs.
 METRICS_XML_FLOAT_STRING_FORMAT = {
     "pgm": "%.8g",
     "period": "%.3f",
     "damping": "%.2f",
-    "smoothing": "%.2f",
     "back_azimuth": "%.2f",
     "vs30": "%.2f",
     "distance": "%.2f",
+    "smoothing_method": "%s",
+    "allow_nans": "%s",
+    "smoothing_parameter": "%.2f",
 }
 
 # Default float format when we don't have a preference
 DEFAULT_FLOAT_FORMAT = "%.8E"
 
 # Default NaN representation in outputted flatfiles
 DEFAULT_NA_REP = "nan"
@@ -141,16 +156,7 @@
         "H1Lowpass",
         "H1Highpass",
         "H2Lowpass",
         "H2Highpass",
         "SourceFile",
     ]
 )
-
-COMPONENTS = {
-    "ROTD50.0": ["SA", "PGA", "PGV"],
-    "GREATER_OF_TWO_HORIZONTALS": ["SA", "PGA", "PGV"],
-    "QUADRATIC_MEAN": ["FAS"],
-    "GEOMETRIC_MEAN": ["FAS"],
-    "ARITHMETIC_MEAN": ["FAS"],
-    "CHANNELS": ["SA", "PGA", "PGV", "DURATION", "SORTED_DURATION", "ARIAS"],
-}
```

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/download_utils.py` & `gmprocess-2.0.0/src/gmprocess/utils/download_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,136 +1,98 @@
 """Module for download unility functions."""
 
 # stdlib imports
-import glob
 import json
 import logging
-import os
 import warnings
 
 # third party imports
 import matplotlib.pyplot as plt
 import numpy as np
 import requests
-from obspy.core.utcdatetime import UTCDateTime
 from obspy.geodetics.base import locations2degrees
 from obspy.taup import TauPyModel
 
 # local imports
 from gmprocess.io.global_fetcher import fetch_data
 from gmprocess.utils.misc import get_rawdir
 
+from gmprocess.utils import constants
 from gmprocess.utils.strec import STREC
 
 TIMEFMT2 = "%Y-%m-%dT%H:%M:%S.%f"
 
 
 FLOAT_PATTERN = r"[-+]?[0-9]*\.?[0-9]+"
 
 EVENT_TEMPLATE = (
     "https://earthquake.usgs.gov/earthquakes/feed/v1.0/detail/[EVENT].geojson"
 )
 
 
-def get_event_data(eventid):
-    event_url = EVENT_TEMPLATE.replace("[EVENT]", eventid)
+def download_comcat_event(event_id):
+    """Download event data from ComCat as GeoJSON.
+
+    Args:
+        event_id (str):
+            ComCat event id.
+    Returns:
+        Dictionary with event information.
+    """
+    event_url = EVENT_TEMPLATE.replace("[EVENT]", event_id)
     response = requests.get(event_url)
     return response.json()
 
 
-def download(event, event_dir, config):
-    """Download waveform data.
+def download_event_data(event, event_dir, config, plot_raw=False):
+    """Download event data, including rupture geometry, STREC results (if enabled),
+    and waveforms.
 
     Args:
         event (ScalarEvent):
             Object containing basic event hypocenter, origin time, magnitude.
         event_dir (str):
             Path where raw directory should be created (if downloading).
         config (dict):
             Dictionary with gmprocess configuration information.
-
+        plot_raw (bool):
+            Plot raw waveforms after downloading.
     """
     # Make raw directory
     rawdir = get_rawdir(event_dir)
 
-    # Run STREC if enabled and results are not already downloaded
+    download_rupture_file(event.id, event_dir)
+
     strec = None
     if config["strec"]["enabled"]:
-        strec_file = event_dir / "strec_results.json"
-        if strec_file.exists():
-            strec = STREC.from_file(strec_file)
-        else:
-            strec = STREC.from_event(event)
-            strec.to_file(strec_file)
+        strec = get_strec_results(event, event_dir)
 
     tcollection, _ = fetch_data(
         event.time.datetime,
         event.latitude,
         event.longitude,
         event.depth_km,
         event.magnitude,
         config=config,
         rawdir=rawdir,
         stream_collection=False,
         strec=strec,
     )
-    # download an event.json file in each event directory,
-    # in case user is simply downloading for now
-    create_event_file(event, event_dir)
-    download_rupture_file(event.id, event_dir)
 
     if len(tcollection):
         logging.debug("tcollection.describe_string():")
         logging.debug(tcollection.describe_string())
 
-    # Plot the raw waveforms
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", category=UserWarning)
-        pngfiles = glob.glob(os.path.join(rawdir, "*.png"))
-        if not len(pngfiles):
-            plot_raw(rawdir, tcollection, event)
-
+    if plot_raw:
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore", category=UserWarning)
+            plot_raw_waveforms(rawdir, tcollection, event)
 
-def create_event_file(event, event_dir):
-    """Write event.json file in event_dir.
 
-    Args:
-        event (ScalarEvent):
-            Input event object.
-        event_dir (str):
-            Directory where event.json should be written.
-    """
-
-    # download event.json for event
-    eventid = event.origins[-1].resource_id.id
-    try:
-        data = get_event_data(eventid)
-    except BaseException:
-        # convert time to comcat time
-        ctime = (event.time - UTCDateTime("1970-01-01T00:00:00.000Z")) * 1000.0
-        data = {
-            "type": "Feature",
-            "properties": {
-                "mag": event.magnitude,
-                "time": ctime,
-            },
-            "geometry": {
-                "type": "Point",
-                "coordinates": [event.longitude, event.latitude, event.depth_km],
-            },
-            "id": eventid,
-        }
-
-    # dump the event.json file to the event directory
-    eventfile = os.path.join(event_dir, "event.json")
-    with open(eventfile, "w", encoding="utf-8") as f:
-        json.dump(data, f)
-
-
-def plot_raw(rawdir, tcollection, event):
+def plot_raw_waveforms(rawdir, tcollection, event):
     """Make PNG plots of a collection of raw waveforms.
 
     Args:
         rawdir (str):
             Directory where PNG files should be saved.
         tcollection (StreamCollection):
             Sequence of streams.
@@ -157,24 +119,23 @@
             arrival = arrivals[0]
             arrival_time = arrival.time
         except BaseException as e:
             fmt = 'Exception "%s" generated by get_travel_times() dist=%.3f depth=%.1f'
             logging.warning(fmt, str(e), dist, source_depth)
             arrival_time = 0.0
         ptime = arrival_time + (event.time - stream[0].stats.starttime)
-        outfile = os.path.join(rawdir, f"{stream.get_id()}.png")
+        outfile = rawdir / f"{stream.get_id()}.png"
 
         fig, axeslist = plt.subplots(nrows=3, ncols=1, figsize=(12, 6))
         for ax, trace in zip(axeslist, stream):
             times = np.linspace(
                 0.0, trace.stats.endtime - trace.stats.starttime, trace.stats.npts
             )
             ax.plot(times, trace.data, color="k")
-            ax.set_xlabel("seconds since start of trace")
-            ax.set_title("")
+            ax.set_xlabel("Seconds since start of trace")
             ax.axvline(ptime, color="r")
             ax.set_xlim(left=0, right=times[-1])
             legstr = "%s.%s.%s.%s" % (
                 trace.stats.network,
                 trace.stats.station,
                 trace.stats.location,
                 trace.stats.channel,
@@ -190,29 +151,39 @@
                 yloc = bottom + (top - bottom) / 10
                 ax.text(xloc, yloc, legstr, color="r")
         plt.savefig(outfile, bbox_inches="tight")
         plt.close()
 
 
 def download_rupture_file(event_id, event_dir):
-    """Download rupture file from Comcat.
+    """Download rupture file from ComCat.
 
     Args:
         event_id (str):
             Event id.
-        event_dir (str):
+        event_dir (pathlib.Path):
             Event directory.
     """
     try:
-        data = get_event_data(event_id)
+        data = download_comcat_event(event_id)
     except BaseException:
         logging.info(f"{event_id} not found in ComCat.")
         return
     try:
         shakemap_prod = data["properties"]["products"]["shakemap"][0]
         rupture_url = shakemap_prod["contents"]["download/rupture.json"]["url"]
-        jsonfile = os.path.join(event_dir, "rupture.json")
-        with open(jsonfile, "wt") as f:
-            response = requests.get(rupture_url)
-            json.dump(response.json(), f)
+        rupture_filename = event_dir / constants.RUPTURE_FILE
+        response = requests.get(rupture_url)
+        with open(rupture_filename, "wt", encoding="utf-8") as fout:
+            json.dump(response.json(), fout)
     except BaseException:
         logging.info(f"{event_id} does not have a rupture.json file.")
+
+
+def get_strec_results(event, event_dir):
+    strec_file = event_dir / constants.STREC_FILE
+    if strec_file.exists():
+        strec = STREC.from_file(strec_file)
+    else:
+        strec = STREC.from_event(event)
+        strec.to_file(strec_file)
+    return strec
```

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/export_gmpacket_utils.py` & `gmprocess-2.0.0/src/gmprocess/utils/export_gmpacket_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,28 +20,29 @@
 )
 from gmpacket.packet import Event, GroundMotionPacket
 from gmpacket.provenance import Provenance
 
 # local imports
 from gmprocess.io.asdf.stream_workspace import StreamWorkspace
 from gmprocess.metrics.waveform_metric_collection import WaveformMetricCollection
-from gmprocess.metrics.gather import gather_pgms
+from gmprocess.metrics.waveform_metric_calculator import WaveformMetricCalculator
 from gmprocess.core import provenance
 
 METRIC_INFO = {
     "PGA": ("Peak ground acceleration", "%g"),
     "PGV": ("Peak ground velocity", "cm/s"),
     "SA": ("Spectral acceleration", "%g"),
     "DURATION": ("Earthquake duration", "s"),
     "FAS": ("Fourier Amplitude Spectra", "cm/s"),
     "SORTEDDURATION": (
         "Sorted earthquake duration",
         "s",
     ),
-    "ARIASINTENSITY": ("Earthquake arias intensity", "m/s"),
+    "ARIAS": ("Earthquake arias intensity", "m/s"),
+    "CAV": ("Earthquake cumulative absolute velocity", "g-s"),
 }
 
 VERSION = "0.1dev"
 MIN_PGA = 0.0464
 
 
 class GroundMotionPacketWriter(object):
@@ -81,15 +82,15 @@
                 if "seis_prov:role" not in agent:
                     provdict["agent"][label]["seis_prov:role"] = "data processor"
         gmp_provenance = Provenance(**provdict)
         return gmp_provenance
 
     def get_trace_properties(self, trace, channel, loc, as_recorded):
         gmp_trace_props = TraceProperties(
-            channel_code=channel,
+            channel_code=channel._gmpacket_channel_code,
             location_code=loc,
             as_recorded=as_recorded,
             azimuth=trace.stats.standard.horizontal_orientation,
             dip=trace.stats.standard.vertical_orientation,
             start_time=trace.stats.starttime.datetime,
             end_time=trace.stats.endtime.datetime,
         )
@@ -99,15 +100,14 @@
         array_metrics = {
             "DURATION": DurationMetricHolder(),
             "SA": SAMetricHolder(0.05),
             "FAS": FASMetricHolder(),
         }
         gmp_metrics = []
         for metric in waveform_metric_list.metric_list:
-            logging.info("Outputting metric %s.%s.%s.%s", net, sta, channel, metric)
             data_value = metric.value(channel)
             if data_value is None:
                 continue
             if re.match("Duration", metric.type) is not None:
                 metric_holder = array_metrics["DURATION"]
                 metric_holder.add_value(data_value, metric)
             elif re.match("SA", metric.type) is not None:
@@ -123,15 +123,14 @@
                     name=metric.type,
                     units=units,
                 )
                 gmp_metric = Metric(properties=gmp_metprops, values=data_value)
                 gmp_metrics.append(gmp_metric)
         for metric_type, metric_holder in array_metrics.items():
             if metric_type == "FAS":
-                logging.warning("FAS metric type not fully supported by gmpacket yet.")
                 continue
             dimensions = metric_holder.get_dimensions()
             values = metric_holder.get_values()
             if not values or not values[0]:
                 continue
             description, units = METRIC_INFO[metric_type]
             gmp_metprops = MetricProperties(
@@ -145,22 +144,21 @@
                 dimensions=gmp_metdims,
                 values=values,
             )
             gmp_metrics.append(gmp_metric)
         return gmp_metrics
 
     def write(self):
-        available_imcs = [x for x in gather_pgms()[1]]
+        available_imcs = WaveformMetricCalculator.available_imcs()
         nevents = 0
         nstreams = 0
         ntraces = 0
         files = []
         wmc = WaveformMetricCollection.from_workspace(self._workspace)
         for eventid in self._workspace.get_event_ids():
-            nevents += 1
             gmp_event = self.get_gmp_event(eventid)
             ds = self._workspace.dataset
             gmp_features = []
             gmp_provenance = None
             station_list = ds.waveforms.list()
             for station_id in station_list:
                 streams = self._workspace.get_streams(
@@ -192,34 +190,35 @@
                                 # for older workspace files, we didn't have a prov
                                 # entry for the label.
                                 plist = self._workspace.dataset.provenance.list()
                                 skey = [a for a in plist if a.endswith(self._label)][0]
                                 prov_doc = self._workspace.dataset.provenance[skey]
                             label_provenance = (
                                 provenance.LabelProvenance.from_provenance_document(
-                                    prov_doc, label=self._label
+                                    prov_doc,
+                                    label=self._label,
+                                    config=self._workspace.config,
                                 )
                             )
                             gmp_provenance = self.get_provenance(label_provenance)
                         net = trace.stats.network
                         sta = trace.stats.station
                         loc = trace.stats.location
                         for sp, wm, sm in zip(
                             wmc.stream_paths, wmc.waveform_metrics, wmc.stream_metadata
                         ):
                             if f"{net}.{sta}" in sp:
                                 waveform_metric_list = wm
-                                stream_metadata = sm
                                 break
                         gmp_traces = []
                         for channel in waveform_metric_list.metric_list[0].components:
                             gmp_metrics = None
                             as_recorded = True
                             for imc in available_imcs:
-                                if imc in channel.lower():
+                                if imc in str(channel).lower():
                                     as_recorded = False
                                     break
                             gmp_trace_props = self.get_trace_properties(
                                 trace, channel, loc, as_recorded
                             )
                             gmp_metrics = self.get_metrics(
                                 waveform_metric_list, channel, net, sta
@@ -261,16 +260,17 @@
                 )
                 outfile = pathlib.Path(
                     self._gmpacket_directory, f"{eventid}_groundmotion_packet.json"
                 )
                 gmp_packet.save_to_json(outfile)
                 files.append(outfile)
                 nevents += 1
-
-        return (files, nevents, nstreams, ntraces)
+                return (files, nevents, nstreams, ntraces)
+            else:
+                return ([], 0, 0, 0)
 
     def __del__(self):
         self._workspace.close()
 
 
 class MetricHolder(object):
     float_pat = "[+-]?([0-9]*[.])?[0-9]+"  # class variable
```

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/export_shakemap_utils.py` & `gmprocess-2.0.0/src/gmprocess/utils/export_shakemap_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,21 @@
 import logging
 from datetime import datetime
 from collections import OrderedDict
 
 import numpy as np
 
 from gmprocess.io.cosmos.core import BUILDING_TYPES
-from gmprocess.utils.constants import EVENT_TIMEFMT, COMPONENTS, UNITS
+from gmprocess.utils.constants import EVENT_TIMEFMT, UNITS
 from gmprocess.metrics.waveform_metric_collection import WaveformMetricCollection
 from gmprocess.metrics.station_metric_collection import StationMetricCollection
+from gmprocess.metrics.waveform_metric_component import (
+    Channels,
+    get_supported_metric_types,
+)
 
 # Will need to update this when we support additional damping values.
 DEFAULT_DAMPING = 5.0
 
 
 def create_json(
     workspace,
@@ -88,15 +92,14 @@
         nfeatures += 1
 
         coordinates = [
             wm_meta[0]["longitude"],
             wm_meta[0]["latitude"],
             wm_meta[0]["elevation"],
         ]
-
         station_feature = get_station_feature(
             wm_meta, wml, sm, coordinates, expanded_imts=expanded_imts
         )
         if station_feature is not None:
             station_features.append(station_feature)
 
         sel_stream = streams.select(
@@ -143,15 +146,15 @@
         "event": event_dict,
         "features": features,
     }
 
     station_feature_dict = {"type": "FeatureCollection", "features": station_features}
     stationfile = event_dir / f"{event.id}_groundmotions_dat.json"
     # debugging
-    iterdict(station_feature_dict)
+    # iterdict(station_feature_dict)
     # end debugging
     with open(stationfile, "wt") as f:
         json.dump(station_feature_dict, f, allow_nan=False)
 
     jsonfile = event_dir / f"{event.id}_metrics.json"
     with open(jsonfile, "wt") as f:
         json.dump(feature_dict, f, allow_nan=False)
@@ -186,52 +189,54 @@
 
     station_properties["code"] = wm_meta[0]["station"]
     station_properties["network"] = wm_meta[0]["network"]
     station_properties["distance"] = sm.repi
     station_properties["source"] = wm_meta[0]["source"]
     station_channels = []
     station_channel_names = ["H1", "H2", "Z"]
+    # station_channel_names = [
+    #     comp for comp in wml[0].components if isinstance(comp, Channels)
+    # ]
 
-    imt_df = wml.to_df()
+    # imt_df = wml.to_df()
     if expanded_imts:
-        imts = list(set([i for i in imt_df["IMT"].to_numpy() if i.startswith("SA")]))
+        imts = [wm.identifier for wm in wml if wm.identifier.startswith("SA")]
         imt_lower = [s.lower() for s in imts]
         imt_units = [UNITS["sa"]] * len(imts)
-        if "PGA" in imt_df["IMT"].tolist():
-            imts.append("PGA")
-            imt_lower.append("pga")
-            imt_units.append(UNITS["PGA"])
-        if "PGV" in imt_df["IMT"].tolist():
-            imts.append("PGV")
-            imt_lower.append("pgv")
-            imt_units.append(UNITS["PGV"])
+        imts.append("PGA")
+        imt_lower.append("pga")
+        imt_units.append(UNITS["PGA"])
+        imts.append("PGV")
+        imt_lower.append("pgv")
+        imt_units.append(UNITS["PGV"])
         station_amps = {k: v for k, v in zip(imts, zip(imt_lower, imt_units))}
     else:
         station_amps = {
-            "SA(0.300)": ("sa(0.3)", UNITS["sa"]),
-            "SA(1.000)": ("sa(1.0)", UNITS["sa"]),
-            "SA(3.000)": ("sa(3.0)", UNITS["sa"]),
+            "SA(T=0.3000, D=0.050)": ("sa(T=0.3000, D=0.050)", UNITS["sa"]),
+            "SA(T=1.0000, D=0.050)": ("sa(T=1.0000, D=0.050)", UNITS["sa"]),
+            "SA(T=3.0000, D=0.050)": ("sa(T=3.0000, D=0.050)", UNITS["sa"]),
             "PGA": ("pga", UNITS["pga"]),
             "PGV": ("pgv", UNITS["pgv"]),
         }
 
     comp_to_chan = wml.metric_list[0].component_to_channel
 
     for channel_name in station_channel_names:
+        chan_code = comp_to_chan[channel_name]
         station_channel = OrderedDict()
         if channel_name in comp_to_chan:
             station_channel["name"] = comp_to_chan[channel_name]
             station_amplitudes = []
             for gm_imt, station_tuple in station_amps.items():
-                imt_value = float(
-                    imt_df.loc[
-                        (imt_df["IMT"] == gm_imt) & (imt_df["IMC"] == channel_name),
-                        "Result",
-                    ]
-                )
+                selected_wm = [wm for wm in wml if wm.identifier == gm_imt][0]
+                for ch, val in selected_wm.values.items():
+                    if isinstance(ch, Channels):
+                        if ch.component_attributes["channel"] == chan_code:
+                            imt_value = val
+                            continue
                 station_amplitude = OrderedDict()
                 station_amplitude["name"] = station_tuple[0]
                 station_amplitude["ln_sigma"] = 0
                 station_amplitude["flag"] = 0
                 station_amplitude["value"] = imt_value
                 station_amplitude["units"] = station_tuple[1]
                 station_amplitudes.append(station_amplitude.copy())
@@ -250,35 +255,33 @@
     FLOAT_MATCH = r"[0-9]*\.[0-9]*"
     components = OrderedDict()
     imt_df = wml.to_df()
     all_components = list(set(imt_df["IMC"]))
     imts = list(set(imt_df["IMT"]))
     comp_to_chan = wml.metric_list[0].component_to_channel
     for imc in all_components:
-        if imc in ["H1", "H2", "Z"]:
-            imtlist = COMPONENTS["CHANNELS"]
-        else:
-            imtlist = COMPONENTS[imc]
+        imtlist = get_supported_metric_types(imc)
         measures = OrderedDict()
         spectral_values = []
         spectral_periods = []
         fourier_amplitudes = []
         fourier_periods = []
         for imt in imts:
             if imt.startswith("FAS"):
-                imtstr = "FAS"
+                continue
             elif imt.startswith("SA"):
                 imtstr = "SA"
             else:
                 imtstr = imt
             if imtstr not in imtlist:
                 continue
-            imt_value = float(
-                imt_df.loc[(imt_df["IMT"] == imt) & (imt_df["IMC"] == imc), "Result"]
-            )
+            idx = np.where((imt_df["IMT"] == imt) & (imt_df["IMC"] == imc))[0]
+            if not idx:
+                continue
+            imt_value = float(imt_df["Result"].iloc[idx])
             if np.isnan(imt_value):
                 imt_value = "null"
             if imt.startswith("SA"):
                 period = float(re.search(FLOAT_MATCH, imt).group())
                 spectral_values.append(imt_value)
                 spectral_periods.append(period)
             elif imt.startswith("FAS"):
@@ -289,16 +292,19 @@
                 # TODO - Make interval something retrievable from metrics
                 units = UNITS[imt.lower()]
                 measures[imt] = {"value": imt_value, "units": units, "interval": "5-95"}
             else:
                 units = UNITS[imt.lower()]
                 measures[imt] = {"value": imt_value, "units": units}
 
-        if imc in ["H1", "H2", "Z"]:
-            imcname = comp_to_chan[imc]
+        if isinstance(imc, Channels):
+            for k, v in comp_to_chan.items():
+                if v == imc.component_attributes["channel"]:
+                    imcname = k
+            # imcname = comp_to_chan[imc.component_attributes["channel"]]
             measures["as_recorded"] = True
             for tr in stream:
                 if tr.stats.channel.endswith(imcname[-1]):
                     trace = tr
                     break
             azimuth = np.nan
             dip = np.nan
@@ -306,15 +312,15 @@
             location_code = trace.stats.location
             peak_acc = trace.data.max()
             start = trace.stats.starttime
             delta = trace.stats.delta
             idx = np.where([trace.data >= peak_acc])[1][0]
             peak_pga_time = (start + (delta * idx)).strftime(EVENT_TIMEFMT)
             vel_trace = trace.copy()
-            vel_trace.integrate(config)
+            vel_trace.integrate(**config["integration"])
             peak_vel = vel_trace.data.max()
             start = vel_trace.stats.starttime
             delta = vel_trace.stats.delta
             idx = np.where([vel_trace.data >= peak_vel])[1][0]
             peak_pgv_time = (start + (delta * idx)).strftime(EVENT_TIMEFMT)
             if "horizontal_orientation" in trace.stats.standard:
                 azimuth = trace.stats.standard["horizontal_orientation"]
@@ -323,15 +329,15 @@
             measures["samples_per_second"] = sampling_rate
             measures["location_code"] = location_code
             measures["peak_pga_time"] = peak_pga_time
             measures["peak_pgv_time"] = peak_pgv_time
             measures["azimuth"] = azimuth
             measures["dip"] = dip
         else:
-            imcname = imc
+            imcname = str(imc)
             measures["as_recorded"] = False
         components[imcname] = measures
         if spectral_values:
             units = UNITS["sa"]
             damping = DEFAULT_DAMPING
             sa_dict = {"units": units, "damping": damping, "method": "absolute"}
             sa_dict["values"] = spectral_values
```

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/ground_motion_models.py` & `gmprocess-2.0.0/src/gmprocess/utils/ground_motion_models.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/logging.py` & `gmprocess-2.0.0/src/gmprocess/utils/logging.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/misc_plots.py` & `gmprocess-2.0.0/src/gmprocess/utils/misc_plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from obspy.geodetics.base import gps2dist_azimuth
 from esi_utils_colors.cpalette import ColorPalette
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from matplotlib.dates import num2date
 
-from gmprocess.metrics.transform.oscillator import get_spectral
+from gmprocess.metrics.oscillator import calculate_spectrals
 
 MIN_MAG = 4.0
 MAX_MAG = 7.0
 DELTA_MAG = 0.5
 
 BOTTOM = 0.1
 AX1_LEFT = 0.1
@@ -292,69 +292,73 @@
 
     if file is not None:
         fig.savefig(file, format="png")
     # plt.show()
     return (fig, ax)
 
 
-def plot_oscillators(st, periods=[0.1, 2, 5, 10], file=None, show=False):
+def plot_oscillators(st, periods=[0.1, 2, 5, 10], damping=0.05, file=None, show=False):
     """
     Produces a figure of the oscillator responses for a StationStream. The
     figure will plot the acceleration traces in the first row, and then an
     additional row for each oscillator period. The number of columns is the
     number of channels in the stream.
 
     Args:
         st (gmprocess.core.stationstream.StationStream):
             StaionStream of data.
         periods (list):
             A list of periods (floats, in seconds).
+        damping (float):
+            Critical damping.
         file (str):
             File where the image will be saved. Default is None.
         show (bool):
             Show the figure. Default is False.
     """
 
     fig, axes = plt.subplots(
         nrows=len(periods) + 1, ncols=len(st), figsize=(4 * len(st), 2 * len(periods))
     )
     if len(st) == 1:
         # Ensure that axes is a 2D numpy array
         axes = axes.reshape(-1, 1)
 
+    # i is loop over periods
     for i in range(axes.shape[0]):
-        if i == 0:
-            plot_st = st
-            ylabel = "Acceleration (cm/s$^2$)"
-            textstr = "T: %s s \nPGA: %.2g cm/s$^2$"
-        else:
-            prd = periods[i - 1]
-            plot_st = get_spectral(prd, st)
-            ylabel = "SA %s s (%%g)" % prd
-            textstr = "T: %s s \nSA: %.2g %%g"
+        for j, trace in enumerate(st):
+            if i == 0:
+                result = trace
+                ylabel = "Acceleration (cm/s$^2$)"
+                textstr = "T: %s s \nPGA: %.2g cm/s$^2$"
+            else:
+                tmp = calculate_spectrals(trace, periods[i - 1], damping)[0]
+                result = trace.copy()
+                result.data = tmp
+                ylabel = "SA %s s (%%g)" % periods[i - 1]
+                textstr = "T: %s s \nSA: %.2g %%g"
 
-        for j, tr in enumerate(plot_st):
             ax = axes[i, j]
             dtimes = np.linspace(
-                0, tr.stats.endtime - tr.stats.starttime, tr.stats.npts
+                0, result.stats.endtime - result.stats.starttime, result.stats.npts
             )
-            ax.plot(dtimes, tr.data, "k", linewidth=0.5)
+            ax.plot(dtimes, result.data, "k", linewidth=0.5)
 
             # Get time and amplitude of max SA (using absolute value)
-            tmax = dtimes[np.argmax(abs(tr.data))]
-            sa_max = max(tr.data, key=abs)
+            tmax = dtimes[np.argmax(abs(result.data))]
+            sa_max = max(result.data, key=abs)
 
             ax.axvline(tmax, c="r", ls="--")
             ax.scatter([tmax], [sa_max], c="r", edgecolors="k", zorder=10)
             ax.text(
                 0.01, 0.98, textstr % (tmax, sa_max), transform=ax.transAxes, va="top"
             )
 
             if i == 0:
-                ax.set_title(tr.id)
+                ax.set_title(result.id)
             if i == len(periods):
                 ax.set_xlabel("Time (s)")
             ax.set_ylabel(ylabel)
 
     plt.tight_layout()
 
     if file is not None:
```

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/prompt.py` & `gmprocess-2.0.0/src/gmprocess/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/report_utils.py` & `gmprocess-2.0.0/src/gmprocess/utils/report_utils.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/rupture_utils.py` & `gmprocess-2.0.0/src/gmprocess/utils/rupture_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 """Module for utilities related to the rupture file."""
 
-from pathlib import Path
-
 from gmprocess.utils.constants import RUPTURE_FILE
 
 
-def get_rupture_file(event_dir):
+def get_rupture_filename(event_dir):
     """Get the path to the rupture file, or None if there is not rupture file.
 
     Args:
-        event_dir (str):
+        event_dir (pathlib.Path):
             Event directory.
 
     Returns:
         str: Path to the rupture file. Returns None if no rupture file exists.
     """
-    event_dir = Path(event_dir)
-    rupture_file = event_dir / RUPTURE_FILE
-    if not rupture_file.is_file():
-        rupture_file = None
-    return rupture_file
+    filename = event_dir / RUPTURE_FILE
+    if not filename.is_file():
+        filename = None
+    return filename
```

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/stderr.py` & `gmprocess-2.0.0/src/gmprocess/utils/stderr.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/strec.py` & `gmprocess-2.0.0/src/gmprocess/utils/strec.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,24 +34,20 @@
         """Get STREC results from an event object.
 
         Args:
             event (utils.event.ScalarEvent):
                 A gmprocess ScalarEvent object.
         """
         selector = SubductionSelector()
-        tensor_params = None
-        if hasattr(event, "id"):
-            _, _, _, _, tensor_params = selector.getOnlineTensor(event.id)
         strec_dict = selector.getSubductionType(
             event.latitude,
             event.longitude,
             event.depth_km,
             event.magnitude,
             eventid=event.id,
-            tensor_params=tensor_params,
         ).to_dict()
         return cls(strec_dict)
 
     def to_file(self, filename):
         """Write STREC results to a file.
 
         Args:
```

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/summary_plots.py` & `gmprocess-2.0.0/src/gmprocess/utils/summary_plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import matplotlib.pyplot as plt
 import matplotlib.patches as patches
 import numpy as np
 from obspy.core.utcdatetime import UTCDateTime
 
 from gmprocess.waveform_processing import spectrum
-from gmprocess.utils.constants import UNIT_CONVERSIONS
+from gmprocess.utils import constants
 from gmprocess.utils.config import get_config
 
 MIN_MAG = 4.0
 MAX_MAG = 7.0
 DELTA_MAG = 0.5
 
 BOTTOM = 0.1
@@ -35,15 +35,15 @@
         """Stream summary plot.
 
         Args:
             st (gmprocess.core.stationtrace.StationStream):
                 Stream of data.
             directory (str):
                 Directory for saving plots.
-            event (gmprocess.utils.event.ScalarEvent):
+            event (gmprocess.utils.scalar_event.ScalarEvent):
                 Flattened subclass of Obspy's Event.
             config (dict):
                 Configuration dictionary (or None). See get_config().
 
         """
         self.st = st
         self.st_raw = st_raw
@@ -127,20 +127,22 @@
             plt.close("all")
         return file_name
 
     def get_vel_disp(self):
         "Compute velocity and displaement"
         self.st_vel = self.st.copy()
         for tr in self.st_vel:
-            tr = tr.integrate(config=self.config)
+            tr = tr.integrate(**self.config["integration"])
 
         # Compute displacement
         self.st_dis = self.st.copy()
         for tr in self.st_dis:
-            tr = tr.integrate(config=self.config).integrate(config=self.config)
+            tr = tr.integrate(**self.config["integration"]).integrate(
+                **self.config["integration"]
+            )
 
     def setup_figure(self):
         "Setup figure"
         nrows = 6
         self.ntrace = min(len(self.st), 3)
         fig = plt.figure(figsize=(3.9 * self.ntrace, 11))
         gs = fig.add_gridspec(nrows, self.ntrace, height_ratios=[1, 1, 1, 1, 2, 2])
@@ -201,15 +203,15 @@
             self.ax.set_title(trace_title, color="red")
 
         dtimes = self.tr_raw.times(type="relative")
         self.ax.plot(dtimes, self.tr_raw.data, "k", linewidth=0.5)
         self.ax.tick_params(axis="both", which="major", labelsize=5)
 
     def plot_acceleration(self):
-        pga = np.max(np.abs(self.tr.data)) / UNIT_CONVERSIONS["g"]
+        pga = np.max(np.abs(self.tr.data)) / constants.UNIT_CONVERSIONS["g"]
         dtimes = self.tr.times(type="relative")
         self.ax.plot(dtimes, self.tr.data, "k", linewidth=0.5)
         self.ax.tick_params(axis="both", which="major", labelsize=5)
 
         self.label_peak("PGA", pga, "g")
         self.draw_split_time()
```

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/tables.py` & `gmprocess-2.0.0/src/gmprocess/utils/tables.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/utils/test_utils.py` & `gmprocess-2.0.0/src/gmprocess/utils/tests_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module for utilities related to unit tests."""
 
-import os.path
-import glob
+import os
+import h5py
 import vcr as vcrpy
 
-from gmprocess.utils.base_utils import read_event_json_files
 from gmprocess.utils import constants
+from gmprocess.core import scalar_event
 
 vcr = vcrpy.VCR(
     path_transformer=vcrpy.VCR.ensure_suffix(".yaml"),
     cassette_library_dir=str(constants.TEST_DATA_DIR / "vcr_cassettes"),
     record_mode="once",
     match_on=["uri"],
 )
@@ -40,26 +40,45 @@
     if not eventdir.is_dir():
         return (None, None)
     datafiles = []
     if files is None:
         allfiles = os.listdir(eventdir)
         allfiles.remove("event.json")
         for dfile in allfiles:
-            datafile = os.path.join(eventdir, dfile)
+            datafile = eventdir / dfile
             datafiles.append(datafile)
     elif isinstance(files, str):
-        # regex
-        datafiles = glob.glob(os.path.join(eventdir, files))
+        # files is a regular expression
+        datafiles = list(eventdir.glob(files))
     else:
-        # this is just a list of filenames
+        # files is a list of filenames
         for tfile in files:
-            fullfile = os.path.join(eventdir, tfile)
-            if os.path.isfile(fullfile):
+            fullfile = eventdir / tfile
+            if fullfile.is_file():
                 datafiles.append(fullfile)
 
-    # read the event.json file
     jsonfile = eventdir / "event.json"
-    if not jsonfile.is_dir():
-        event = None
-    event = read_event_json_files([jsonfile])[0]
+    event = None
+    if jsonfile.is_file():
+        event = scalar_event.ScalarEvent.from_json(jsonfile)
 
     return (datafiles, event)
+
+
+def check_workspace(filename, hierarchy):
+    """Check workspace hierarchy to make sure it contains all expected items.
+
+    Args:
+        filename (pathlib.Path):
+            Filename of ASDF workspace.
+        hierarchy (tuple):
+            Tuple of names of items in workspace (matches h5dump -n).
+    """
+
+    def tracker(name):
+        tracker.items.append(name)
+
+    assert filename.is_file()
+    with h5py.File(filename) as h5:
+        tracker.items = []
+        h5.visit(tracker)
+        assert tuple(tracker.items) == hierarchy
```

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/adjust_highpass.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/adjust_highpass.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/adjust_highpass_ridder.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/adjust_highpass_ridder.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/baseline_correction.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/baseline_correction.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/clip_detection.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/clip_detection.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/clipping_ann.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/clipping_ann.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/clipping_check.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/clipping_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     Lower thresholds will pass fewer streams but will give less false negatives
     (i.e., streams in which clipping actually occurred but were missed).
 
     Args:
         st (gmprocess.core.stationstream.StationStream):
            Trace of data.
-        event (gmprocess.utils.event.ScalarEvent):
+        event (gmprocess.utils.scalar_event.ScalarEvent):
             ScalarEvent object.
         threshold (float):
             Threshold probability.
         config (dict):
             Configuration dictionary (or None). See get_config().
 
     Returns:
```

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/histogram.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/histogram.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/jerk.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/jerk.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/max_amp.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/max_amp.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/ping.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/ping.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/clipping/std_dev.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/clipping/std_dev.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/corner_frequencies.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/corner_frequencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 """Module for processing steps related to corner frequencies."""
 
-"""
-Methods for handling/picking corner frequencies.
-"""
-
 import logging
 import numpy as np
 
 from gmprocess.waveform_processing.processing_step import processing_step
 from gmprocess.waveform_processing.snr import compute_snr_trace
 
 # Options for tapering noise/signal windows
@@ -35,15 +31,15 @@
     Note that this step only selects the highpass and lowpass corners. The results can
     be modifed by other steps (such as `lowpass_max_frequency`) and then the filters
     are applied with the `lowpass_filter` and `highpass_filter` steps.
 
     Args:
         st (gmprocess.core.stationstream.StationStream):
             Stream of data.
-        event (gmprocess.utils.event.ScalarEvent):
+        event (gmprocess.utils.scalar_event.ScalarEvent):
             ScalarEvent object.
         method (str):
             Which method to use; currently allowed "snr" or "constant".
         constant(dict):
             Dictionary of `constant` method config options.
         snr (dict):
             Dictionary of `snr` method config options.
@@ -186,15 +182,15 @@
     lowpass=[25.0, 35.0, 40.0],
 ):
     """Use constant corner frequencies across all records.
 
     Args:
         st (gmprocess.core.stationstream.StationStream):
             Stream of data.
-        event (gmprocess.utils.event.ScalarEvent):
+        event (gmprocess.utils.scalar_event.ScalarEvent):
             ScalarEvent object.
         highpass (float):
             Highpass corner frequency (Hz).
         lowpass (float):
             Lowpass corner frequency (Hz).
 
     Returns:
@@ -208,33 +204,33 @@
         tr.set_parameter(
             "corner_frequencies",
             {"type": "magnitude", "highpass": hp_select, "lowpass": lp_select},
         )
     return st
 
 
-def from_snr(st, event, same_horiz=True, bandwidth=20):
+def from_snr(st, event, same_horiz=True, smoothing_parameter=20):
     """Set corner frequencies from SNR.
 
     Args:
         st (StationStream):
             Stream of data.
         same_horiz (bool):
             If True, horizontal traces in the stream must have the same
             corner frequencies.
-        bandwidth (float):
+        smoothing_parameter (float):
             Konno-Omachi smoothing bandwidth parameter.
 
     Returns:
         stream: stream with selected corner frequencies appended to records.
     """
     for tr in st:
         # Check for prior calculation of 'snr'
         if not tr.has_cached("snr"):
-            tr = compute_snr_trace(tr, event.magnitude, bandwidth)
+            tr = compute_snr_trace(tr, event.magnitude, smoothing_parameter)
 
         # If the SNR doesn't exist then it must have failed because it didn't
         # have enough points in the noise or signal windows
         if tr.passed:
             snr_conf = tr.get_parameter("snr_conf")
             threshold = snr_conf["threshold"]
             min_freq = snr_conf["min_freq"]
```

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/detrend.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/detrend.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/fft.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/fft.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 from obspy.signal.util import next_pow_2
 
 from esi_core.gmprocess.waveform_processing.smoothing.konno_ohmachi import (
     konno_ohmachi_smooth,
 )
 
 
-def compute_and_smooth_spectrum(tr, bandwidth, section, window=None, nfft=None):
+def compute_and_smooth_spectrum(
+    tr, smoothing_parameter, section, window=None, nfft=None
+):
     """
     Compute raw and smoothed signal spectrum for a given trace.
 
     Args:
         tr (StationTrace):
            Trace of data. This is the trace where the Cache values will be set.
-        bandwidth (float):
+        smoothing_parameter (float):
            Konno-Omachi smoothing bandwidth parameter.
         section (str):
             Determines the name for the spectrum located in the Cache. This is
             usually either "signal" or "noise".
         window (StationTrace):
             Smaller window of the trace for computing the spectrum (usually
             either the signal or noise window). If not provided, then the
@@ -37,15 +39,17 @@
     if nfft is None:
         nfft = next_pow_2(tr.stats.npts)
     if window is None:
         window = tr
     lowest_usable_freq = 1 / tr.stats.delta / tr.stats.npts
     spec_raw, freqs_raw = compute_fft(window, nfft)
     spec_raw[freqs_raw < lowest_usable_freq] = np.nan
-    spec_smooth, freqs_smooth = smooth_spectrum(spec_raw, freqs_raw, nfft, bandwidth)
+    spec_smooth, freqs_smooth = smooth_spectrum(
+        spec_raw, freqs_raw, nfft, smoothing_parameter
+    )
     spec_smooth[freqs_smooth < lowest_usable_freq] = np.nan
 
     raw_dict = {"spec": spec_raw, "freq": freqs_raw}
     smooth_dict = {"spec": spec_smooth, "freq": freqs_smooth}
 
     tr.set_cached(f"{section}_spectrum", raw_dict)
     tr.set_cached(f"smooth_{section}_spectrum", smooth_dict)
@@ -70,37 +74,37 @@
     """
     dt = trace.stats.delta
     spec = abs(np.fft.rfft(trace.data, n=nfft)) * dt
     freqs = np.fft.rfftfreq(nfft, dt)
     return spec, freqs
 
 
-def smooth_spectrum(spec, freqs, nfft, bandwidth=20):
+def smooth_spectrum(spec, freqs, nfft, smoothing_parameter=20):
     """
     Smooths the amplitude spectrum following the algorithm of
     Konno and Ohmachi.
 
     Args:
         spec (numpy.ndarray):
             Spectral amplitude data.
         freqs (numpy.ndarray):
             Frequencies.
         nfft (int):
             Number of data points for the fourier transform.
-        bandwidth (float):
+        smoothing_parameter (float):
             Konno-Omachi smoothing bandwidth parameter.
 
     Returns:
         numpy.ndarray: Smoothed amplitude data and frequencies.
     """
 
     # Do a maximum of 301 K-O frequencies in the range of the fft freqs
     nkofreqs = min(nfft, 302) - 1
     ko_freqs = np.logspace(np.log10(freqs[1]), np.log10(freqs[-1]), nkofreqs)
     # An array to hold the output
     spec_smooth = np.empty_like(ko_freqs)
 
     # Konno Omachi Smoothing
     konno_ohmachi_smooth(
-        spec.astype(np.double), freqs, ko_freqs, spec_smooth, bandwidth
+        spec.astype(np.double), freqs, ko_freqs, spec_smooth, smoothing_parameter
     )
     return spec_smooth, ko_freqs
```

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/filtering.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/filtering.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/instrument_response.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/instrument_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Methods for handling instrument response."""
 
+import os
 import sys
 import logging
 
 import numpy as np
 
 from gmprocess.core.stationtrace import PROCESS_LEVELS
 from gmprocess.waveform_processing.processing_step import processing_step
@@ -151,28 +152,39 @@
         try:
             # Note: rater than set OUTPUT to 'ACC' for seismometers, we are are setting
             # it to 'VEL" and then differentiating.
             if self.instrument_code == "H":
                 output_units = "VEL"
             else:
                 output_units = "ACC"
-            out = OutputGrabber(sys.stderr)
-            out.start()
-            self.trace.remove_response(
-                inventory=self.inv,
-                output=output_units,
-                water_level=self.water_level,
-                pre_filt=self.pre_filt,
-                zero_mean=True,
-                taper=False,
-            )
-            out.stop()
-            match_str = "computed and reported sensitivities differ"
-            if match_str in out.capturedtext:
-                self.trace.warning("Computed and reported sensitivities differ.")
+            if "JPY_PARENT_PID" in os.environ:
+                # Cannot capture sys.stderr if this is called from a jupyter notebook.
+                self.trace.remove_response(
+                    inventory=self.inv,
+                    output=output_units,
+                    water_level=self.water_level,
+                    pre_filt=self.pre_filt,
+                    zero_mean=True,
+                    taper=False,
+                )
+            else:
+                out = OutputGrabber(sys.stderr)
+                out.start()
+                self.trace.remove_response(
+                    inventory=self.inv,
+                    output=output_units,
+                    water_level=self.water_level,
+                    pre_filt=self.pre_filt,
+                    zero_mean=True,
+                    taper=False,
+                )
+                out.stop()
+                match_str = "computed and reported sensitivities differ"
+                if match_str in out.capturedtext:
+                    self.trace.warning("Computed and reported sensitivities differ.")
 
             self.trace.set_provenance(
                 "remove_response",
                 {
                     "method": "remove_response",
                     "input_units": "counts",
                     "output_units": ABBREV_UNITS[output_units],
@@ -187,14 +199,15 @@
                 self.trace.differentiate(frequency=diff_conf["frequency"])
 
             self.trace.data *= constants.M_TO_CM  # Convert from m to cm
             self.trace.stats.standard.units = ABBREV_UNITS[OUTPUT]
             self.trace.stats.standard.units_type = OUTPUT.lower()
             self.trace.stats.standard.process_level = PROCESS_LEVELS["V1"]
         except BaseException as e:
+            raise e
             reason = (
                 "Encountered an error when attempting to remove instrument response: "
                 f"{str(e)}"
             )
             self.trace.fail(reason)
             return
```

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/integrate.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/integrate.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
     Returns:
         StationTrace.
 
     """
     acc = tr.copy()
     try:
-        disp = acc.integrate(config=config).integrate(config=config)
+        disp = acc.integrate(**config["integration"]).integrate(**config["integration"])
     except Exception as e:
         raise e
     return disp
 
 
 def get_vel(tr, config=None):
     """Integrate acceleration to velocity.
@@ -35,11 +35,11 @@
 
     Returns:
         StationTrace.
 
     """
     acc = tr.copy()
     try:
-        vel = acc.integrate(config=config)
+        vel = acc.integrate(**config["integration"])
     except Exception as e:
         raise e
     return vel
```

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/nn_quality_assurance.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/nn_quality_assurance.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/phase.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/phase.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,21 +12,18 @@
 import scipy.linalg as alg
 from obspy.signal.trigger import ar_pick, pk_baer
 from obspy.core.utcdatetime import UTCDateTime
 from obspy.geodetics.base import locations2degrees
 from obspy.taup import TauPyModel
 
 # local imports
-from gmprocess.utils.config import get_config
-from gmprocess.utils.event import ScalarEvent
+from gmprocess.core import scalar_event
 
 NAN_TIME = UTCDateTime("1970-01-01T00:00:00")
 
-CONFIG = get_config()
-
 
 def butter_bandpass(lowcut, highcut, fs, order=5):
     nyq = 0.5 * fs
     low = lowcut / nyq
     high = highcut / nyq
     b, a = butter(order, [low, high], btype="band")
     return b, a
@@ -211,36 +208,32 @@
 
     if not len(rt):
         return -1
     rt2 = dt.timedelta(seconds=(rt[0] / sps)).total_seconds()
     return rt2
 
 
-def pick_kalkan(stream, picker_config=None, config=None):
+def pick_kalkan(stream, config):
     """Wrapper around the Kalkan P-phase picker.
 
     Args:
         stream (gmprocess.core.stationstream.StationStream):
             Stream containing waveforms that need to be picked.
-        picker_config (dict):
-            Dictionary with parameters for Kalkan P-phase picker.
-            See picker.yml.
         config (dict):
             Configuration dictionary. Key value here is:
                 windows:
                     window_checks:
                         min_noise_duration
     Returns:
         tuple:
             - Best estimate for p-wave arrival time (s since start of trace).
             - Mean signal to noise ratio based on the pick.
     """
-    if picker_config is None:
-        picker_config = CONFIG["pickers"]
-    min_noise_dur = CONFIG["windows"]["window_checks"]["min_noise_duration"]
+    picker_config = config["pickers"]
+    min_noise_dur = config["windows"]["window_checks"]["min_noise_duration"]
     params = picker_config["kalkan"]
     locs = []
     for trace in stream:
         loc = pphase_pick(trace, **params)
         if loc >= 0:
             locs.append(loc)
     locs = np.array(locs)
@@ -253,35 +246,32 @@
         tpl = (minloc, min_noise_dur)
         raise ValueError(fmt % tpl)
     mean_snr = calc_snr(stream, minloc)
 
     return (minloc, mean_snr)
 
 
-def pick_ar(stream, picker_config=None, config=None):
+def pick_ar(stream, config):
     """Wrapper around the AR P-phase picker.
 
     Args:
         stream (gmprocess.core.stationstream.StationStream):
             Stream containing waveforms that need to be picked.
-        picker_config (dict):
-            Dictionary with parameters for AR P-phase picker. See picker.yml.
         config (dict):
             Configuration dictionary. Key value here is:
                 windows:
                     window_checks:
                         min_noise_duration
     Returns:
         tuple:
             - Best estimate for p-wave arrival time (s since start of trace).
             - Mean signal to noise ratio based on the pick.
     """
-    if picker_config is None:
-        picker_config = CONFIG["pickers"]
-    min_noise_dur = CONFIG["windows"]["window_checks"]["min_noise_duration"]
+    picker_config = config["pickers"]
+    min_noise_dur = config["windows"]["window_checks"]["min_noise_duration"]
     params = picker_config["ar"]
     # Get the east, north, and vertical components from the stream
     st_e = stream.select(channel="??[E1]")
     st_n = stream.select(channel="??[N2]")
     st_z = stream.select(channel="??[Z3]")
 
     # Check if we found one of each component
@@ -297,35 +287,32 @@
         tpl = (minloc, min_noise_dur)
         raise ValueError(fmt % tpl)
     mean_snr = calc_snr(stream, minloc)
 
     return (minloc, mean_snr)
 
 
-def pick_baer(stream, picker_config=None, config=None):
+def pick_baer(stream, config):
     """Wrapper around the Baer P-phase picker.
 
     Args:
         stream (gmprocess.core.stationstream.StationStream):
             Stream containing waveforms that need to be picked.
-        picker_config (dict):
-            Dictionary with parameters for Baer P-phase picker. See picker.yml.
         config (dict):
             Configuration dictionary. Key value here is:
                 windows:
                     window_checks:
                         min_noise_duration
     Returns:
         tuple:
             - Best estimate for p-wave arrival time (s since start of trace).
             - Mean signal to noise ratio based on the pick.
     """
-    if picker_config is None:
-        picker_config = CONFIG["pickers"]
-    min_noise_dur = CONFIG["windows"]["window_checks"]["min_noise_duration"]
+    picker_config = config["pickers"]
+    min_noise_dur = config["windows"]["window_checks"]["min_noise_duration"]
     params = picker_config["baer"]
     # fix some param types
     params["tdownmax"] = int(params["tdownmax"])
     params["tupevent"] = int(params["tupevent"])
     params["preset_len"] = int(params["preset_len"])
     params["p_dur"] = int(params["p_dur"])
     locs = []
@@ -343,32 +330,33 @@
         minloc = -1
         mean_snr = 0
     mean_snr = calc_snr(stream, minloc)
 
     return (minloc, mean_snr)
 
 
-def pick_travel(stream, event, model=None, picker_config=None):
+def pick_travel(stream, event, config, model=None):
     """Use TauP travel time model to find P-Phase arrival time.
 
     Args:
         stream (gmprocess.core.stationstream.StationStream):
             StationStream containing 1 or more channels of waveforms.
-        event (ScalarEvent):
+        event (scalar_event.ScalarEvent):
             Event origin/magnitude information.
+        config (dict):
+            Dictionary of config options.
         model (TauPyModel):
             TauPyModel object for computing travel times.
     Returns:
         tuple:
             - Best estimate for p-wave arrival time (s since start of trace).
             - Mean signal to noise ratio based on the pick.
     """
     if model is None:
-        if picker_config is None:
-            picker_config = CONFIG["pickers"]
+        picker_config = config["pickers"]
         model = TauPyModel(picker_config["travel_time"]["model"])
     if stream[0].stats.starttime == NAN_TIME:
         return (-1, 0)
     lat = event.latitude
     lon = event.longitude
     depth = event.depth_km
     if depth < 0:
@@ -395,27 +383,29 @@
     arrival = arrivals[0]
     # we need time since start of the record
     minloc = arrival.time + (etime - stream[0].stats.starttime)
     mean_snr = calc_snr(stream, minloc)
     return (minloc, mean_snr)
 
 
-def pick_yeck(stream):
+def pick_yeck(stream, config):
     """IN DEVELOPMENT! SNR based P-phase picker.
 
     Args:
         stream (StationStream):
             Stream containing waveforms that need to be picked.
+        config (dict):
+            Dictionary of config options.
     Returns:
         tuple:
             - Best estimate for p-wave arrival time (s since start of trace).
             - Mean signal to noise ratio based on the pick.
     """
     min_window = 5.0  # put into config
-    min_noise_dur = CONFIG["windows"]["window_checks"]["min_noise_duration"]
+    min_noise_dur = config["windows"]["window_checks"]["min_noise_duration"]
     locs = []
     for trace in stream:
         data = trace.data
         sr = trace.stats.sampling_rate
         pidx_start = int(min_window * sr)
         snr = np.zeros(len(data))
         for pidx in range(pidx_start, len(data) - pidx_start):
@@ -436,35 +426,32 @@
         tpl = (minloc, min_noise_dur)
         raise ValueError(fmt % tpl)
     mean_snr = calc_snr(stream, minloc)
 
     return (minloc, mean_snr)
 
 
-def pick_power(stream, picker_config=None, config=None):
+def pick_power(stream, config):
     """Wrapper around the power_picker.
 
     Args:
         stream (StationStream):
             Stream containing waveforms that need to be picked.
-        picker_config (dict):
-            Dictionary with parameters for power_picker. See picker.yml.
         config (dict):
             Configuration dictionary. Key value here is:
                 windows:
                     window_checks:
                         min_noise_duration
     Returns:
         tuple:
             - Best estimate for p-wave arrival time (s since start of trace).
             - Mean signal to noise ratio based on the pick.
     """
-    if picker_config is None:
-        picker_config = CONFIG["pickers"]
-    min_noise_dur = CONFIG["windows"]["window_checks"]["min_noise_duration"]
+    picker_config = config["pickers"]
+    min_noise_dur = config["windows"]["window_checks"]["min_noise_duration"]
     params = picker_config["power"]
     locs = []
     for trace in stream:
         loc = power_picker(trace, **params)
         locs.append(loc)
 
     locs = np.array(locs)
@@ -693,15 +680,15 @@
     # uHist_final = (uLow + iMin);
     return levels, histogram, bins
 
 
 def create_travel_time_dataframe(streams, catalog_file, ddepth, ddist, model):
     """
     Creates a travel time dataframe, which contains the phase arrrival times
-    for each station the StreamCollection, for each event in the catalog.
+    for each station in the StreamCollection, for each event in the catalog.
     This uses an interpolation method to save time, and the fineness of the
     interpolation grid can be adjusted using the ddepth and ddist parameters.
     Using the recommended values of ddepth=5 and ddist=0.1 are generally
     sufficient to achieve less than 0.1 seconds of error in the travel times,
     for most cases.
 
     Args:
@@ -721,18 +708,18 @@
         (list of ScalarEvent objects).
     """
 
     # Read the catalog file and create a catalog (list) of ScalarEvent objects
     df_catalog = pd.read_csv(catalog_file)
 
     # Replace any negative depths with 0
-    df_catalog["depth"].clip(lower=0, inplace=True)
+    df_catalog["depth"] = df_catalog["depth"].clip(lower=0)
     catalog = []
     for idx, row in df_catalog.iterrows():
-        event = ScalarEvent.from_params(
+        event = scalar_event.ScalarEvent.from_params(
             row["id"],
             row["time"],
             row["latitude"],
             row["longitude"],
             row["depth"],
             row["mag"],
         )
```

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/processing.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/processing.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/processing_step.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/processing_step.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/resample.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/resample.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/sanity_checks.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/snr.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/snr.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,33 +15,33 @@
 TAPER_WIDTH = 0.05
 TAPER_TYPE = "hann"
 TAPER_SIDE = "both"
 MIN_POINTS_IN_WINDOW = 10
 
 
 @processing_step
-def compute_snr(st, event, bandwidth=20.0, config=None):
+def compute_snr(st, event, smoothing_parameter=20.0, config=None):
     """Compute SNR dictionaries for a stream, looping over all traces.
 
     Args:
         st (StationStream):
            Trace of data.
         event (ScalarEvent):
            ScalarEvent object.
-        bandwidth (float):
+        smoothing_parameter (float):
            Konno-Omachi smoothing bandwidth parameter.
         config (dict):
             Configuration dictionary (or None). See get_config().
 
     Returns:
         StationStream: With SNR dictionaries added as trace parameters.
     """
     for tr in st:
         # Do we have estimates of the signal split time?
-        compute_snr_trace(tr, event.magnitude, bandwidth)
+        compute_snr_trace(tr, event.magnitude, smoothing_parameter)
     return st
 
 
 @processing_step
 def snr_check(
     st,
     mag,
@@ -63,15 +63,15 @@
         threshold (float):
             Threshold SNR value.
         min_freq (float or str):
             Minimum frequency for threshold to be exeeded. If 'f0', then the
             Brune corner frequency will be used.
         max_freq (float):
             Maximum frequency for threshold to be exeeded.
-        bandwidth (float):
+        smoothing_parameter (float):
             Konno-Omachi smoothing bandwidth parameter.
         f0_options (dict):
             Dictionary of f0 options (see config file).
         config (dict):
             Configuration dictionary (or None). See get_config().
 
     Returns:
@@ -108,21 +108,21 @@
                 )
                 tr.fail(f"SNR check: SNR {min_snr:.2f} < {threshold:.2f}")
         snr_conf = {"threshold": threshold, "min_freq": min_freq, "max_freq": max_freq}
         tr.set_parameter("snr_conf", snr_conf)
     return st
 
 
-def compute_snr_trace(tr, event_magnitude, bandwidth=20.0):
+def compute_snr_trace(tr, event_magnitude, smoothing_parameter=20.0):
     """Compute SNR dictionaries for a trace.
 
     Args:
         event_magnitude (float):
             Earthquake magnitude.
-        bandwidth (float):
+        smoothing_parameter (float):
             Konno-Omachi smoothing bandwidth parameter.
 
     """
 
     def _compute_event_spectra(
         preevent_noise_spectrum, event_spectrum, dur_preevent, dur_event
     ):
@@ -172,28 +172,30 @@
         if preevent_noise.stats.npts < MIN_POINTS_IN_WINDOW:
             # Fail the trace, but still compute the event spectra
             # ** only fail here if it hasn't already failed; we do not yet
             # ** support tracking multiple fail reasons and I think it is
             # ** better to know the FIRST reason if I have to pick one.
             if tr.passed:
                 tr.fail("SNR check; Not enough points in noise window")
-            compute_and_smooth_spectrum(tr, bandwidth, "event")
+            compute_and_smooth_spectrum(tr, smoothing_parameter, "event")
             return tr
 
         # Check that there are a minimum number of points in the event window
         if event.stats.npts < MIN_POINTS_IN_WINDOW:
             # Fail the trace, but still compute the event spectra
             if tr.passed:
                 tr.fail("SNR check; Not enough points in event window")
-            compute_and_smooth_spectrum(tr, bandwidth, "event")
+            compute_and_smooth_spectrum(tr, smoothing_parameter, "event")
             return tr
 
         nfft = max(next_pow_2(event.stats.npts), next_pow_2(preevent_noise.stats.npts))
-        compute_and_smooth_spectrum(tr, bandwidth, "noise", preevent_noise, nfft)
-        compute_and_smooth_spectrum(tr, bandwidth, "event", event, nfft)
+        compute_and_smooth_spectrum(
+            tr, smoothing_parameter, "noise", preevent_noise, nfft
+        )
+        compute_and_smooth_spectrum(tr, smoothing_parameter, "event", event, nfft)
 
         # Noise, event, and signal durations.
         #
         # - Pre-event noise duration is the pre-event window duration.
         # - Event noise duration is the event window duration.
         # - Ground motions at these frequencies are approximately white noise, and thus
         #   also scale as sqrt(duration); ground motion is not stationary, so we'll use
@@ -250,20 +252,20 @@
         )
 
         smooth_event_noise_normspectrum = smooth_event_noise_spectrum / np.sqrt(
             dur_event
         )
         smooth_signal_normspectrum = smooth_signal_spectrum / np.sqrt(dur_shaking)
         snr = smooth_signal_normspectrum / smooth_event_noise_normspectrum
-        snr_dict = tr.set_cached(
+        tr.set_cached(
             "snr",
             {
                 "snr": snr,
                 "freq": tr.get_cached("smooth_event_spectrum")["freq"],
             },
         )
 
     else:
         # We do not have an estimate of the event split time for this trace
-        compute_and_smooth_spectrum(tr, bandwidth, "event")
+        compute_and_smooth_spectrum(tr, smoothing_parameter, "event")
 
     return tr
```

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/spectrum.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     config=None,
 ):
     """Fit spectra vaying stress_drop and moment.
 
     Args:
         st (gmprocess.core.stationstream.StationStream):
             Stream of data.
-        event (gmprocess.utils.event.ScalarEvent):
+        event (gmprocess.utils.scalar_event.ScalarEvent):
              ScalarEvent object.
         kappa (float):
             Site diminution factor (sec). Typical value for active cruststal
             regions is about 0.03-0.04, and stable continental regions is about
             0.006.
         RP (float):
             Partition of shear-wave energy into horizontal components.
```

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/taper.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/taper.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/windows.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/windows.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """Helper functions for windowing singal and noise in a trace."""
 
 import logging
 
 import numpy as np
 import pandas as pd
 
-from openquake.hazardlib.gsim.base import RuptureContext
-from openquake.hazardlib import const
-from openquake.hazardlib import imt
+from openquake.hazardlib.contexts import simple_cmaker
 
 from obspy.geodetics.base import gps2dist_azimuth
 
 from gmprocess.waveform_processing.phase import (
     pick_power,
     pick_ar,
     pick_baer,
+    pick_yeck,
     pick_kalkan,
     pick_travel,
 )
 from gmprocess.utils.config import get_config
 from gmprocess.metrics.waveform_metric_collection import WaveformMetricCollection
 from gmprocess.utils.ground_motion_models import load_model
 from gmprocess.waveform_processing.processing_step import processing_step
@@ -49,17 +48,14 @@
     run, in which case the record is trimmed to the end of the signal that
     was estimated by that method.
 
     To trim the beginning of the record, the sec_before_split must be
     specified, which uses the noise/signal split time that was estiamted by the
     windows.signal_split mehtod.
 
-    # Recent changes to reflect major updates to how oq-hazardlib works:
-    # https://github.com/gem/oq-engine/issues/7018
-
     Args:
         st (StationStream):
             Stream of data.
         sec_before_split (float):
             Seconds to trim before split. If None, then the beginning of the
             record will be unchanged.
         config (dict):
@@ -175,41 +171,33 @@
         }
         for tr in st:
             tr.set_parameter("signal_split", split_params)
         return st
 
     picker_config = config["pickers"]
 
-    loc, mean_snr = pick_travel(st, event, model)
+    loc, mean_snr = pick_travel(st, event, config, model)
     if loc > 0:
         tsplit = st[0].stats.starttime + loc
         preferred_picker = "travel_time"
     else:
         pick_methods = ["ar", "baer", "power", "kalkan"]
         rows = []
         for pick_method in pick_methods:
             try:
                 if pick_method == "ar":
-                    loc, mean_snr = pick_ar(
-                        st, picker_config=picker_config, config=config
-                    )
+                    loc, mean_snr = pick_ar(st, config=config)
                 elif pick_method == "baer":
-                    loc, mean_snr = pick_baer(
-                        st, picker_config=picker_config, config=config
-                    )
+                    loc, mean_snr = pick_baer(st, config=config)
                 elif pick_method == "power":
-                    loc, mean_snr = pick_power(
-                        st, picker_config=picker_config, config=config
-                    )
+                    loc, mean_snr = pick_power(st, config=config)
                 elif pick_method == "kalkan":
-                    loc, mean_snr = pick_kalkan(
-                        st, picker_config=picker_config, config=config
-                    )
+                    loc, mean_snr = pick_kalkan(st, config=config)
                 elif pick_method == "yeck":
-                    loc, mean_snr = pick_kalkan(st)
+                    loc, mean_snr = pick_yeck(st, config=config)
             except BaseException:
                 loc = -1
                 mean_snr = np.nan
             rows.append(
                 {
                     "Stream": st.get_id(),
                     "Method": pick_method,
@@ -296,28 +284,14 @@
             for method="model".
 
     Returns:
         trace with stats dict updated to include a
         stats['processing_parameters']['signal_end'] dictionary.
 
     """
-    # Load openquake stuff if method="model"
-    if method == "model":
-        dmodel = load_model(model)
-
-        # Set some "conservative" inputs (in that they will tend to give
-        # larger durations).
-        rctx = RuptureContext()
-        rctx.mag = event_mag
-        rctx.rake = -90.0
-        rctx.vs30 = np.array([180.0])
-        rctx.z1pt0 = np.array([0.51])
-        dur_imt = imt.from_string("RSD595")
-        stddev_types = [const.StdDev.TOTAL]
-
     for tr in st:
         if not tr.has_parameter("signal_split"):
             logging.warning("No signal split in trace, cannot set signal end.")
             continue
         if method == "velocity":
             if vmin is None:
                 raise ValueError('Must specify vmin if method is "velocity".')
@@ -332,31 +306,43 @@
                 )[0]
                 / 1000.0
             )
             end_time = event_time + max(floor, epi_dist / vmin)
         elif method == "model":
             if model is None:
                 raise ValueError('Must specify model if method is "model".')
+            dmodel = load_model(model)
+
+            # Set some "conservative" inputs (in that they will tend to give
+            # larger durations).
+            cmaker = simple_cmaker([dmodel], ["RSD595"], mags="%2.f" % event_mag)
+            ctx = cmaker.new_ctx(1)
+            ctx["mag"] = event_mag
+            ctx["rake"] = -90.0
+            ctx["vs30"] = np.array([180.0])
+            ctx["z1pt0"] = np.array([0.51])
             epi_dist = (
                 gps2dist_azimuth(
                     lat1=event_lat,
                     lon1=event_lon,
                     lat2=tr.stats["coordinates"]["latitude"],
                     lon2=tr.stats["coordinates"]["longitude"],
                 )[0]
                 / 1000.0
             )
             # Repi >= Rrup, so substitution here should be conservative
             # (leading to larger durations).
-            rctx.rrup = np.array([epi_dist])
-            rctx.sids = np.array(range(np.size(rctx.rrup)))
-            lnmu, lnstd = dmodel.get_mean_and_stddevs(
-                rctx, rctx, rctx, dur_imt, stddev_types
-            )
-            duration = np.exp(lnmu + epsilon * lnstd[0])
+            ctx["rrup"] = np.array([epi_dist])
+
+            result = cmaker.get_mean_stds([ctx])
+            lnmu = result[0][0][0]
+            lnstd = result[1][0][0]
+
+            duration = np.exp(lnmu + epsilon * lnstd)
+
             # Get split time
             split_time = tr.get_parameter("signal_split")["split_time"]
             end_time = split_time + float(duration)
         elif method == "magnitude":
             end_time = event_time + duration_from_magnitude(event_mag)
         elif method == "none":
             # need defaults
@@ -481,51 +467,50 @@
     config["metrics"]["output_imcs"] = ["greater_of_two_horizontals"]
     wmc = WaveformMetricCollection.from_streams([st], event, config)
     wm = wmc.waveform_metrics[0].metric_list[0]
     recorded_pga = wm.value("GREATER_OF_TWO_HORIZONTALS")
 
     # Load the GMPE model
     gmpe = load_model(gmpe)
-
-    # Generic context
-    rctx = RuptureContext()
+    cmaker = simple_cmaker([gmpe], ["PGA"], mags="%2.f" % event.magnitude)
+    ctx = cmaker.new_ctx(1)
+    ctx["mag"] = event.magnitude
 
     # Make sure that site parameter values are converted to numpy arrays
     site_parameters_copy = site_parameters.copy()
     for k, v in site_parameters_copy.items():
         site_parameters_copy[k] = np.array([site_parameters_copy[k]])
-    rctx.__dict__.update(site_parameters_copy)
+    ctx.__dict__.update(site_parameters_copy)
 
     # Filter by arrivals that have significant expected PGA using GMPE
     is_significant = []
     for eqid, arrival_time in arrivals.items():
         event = next(event for event in catalog if event.id == eqid)
 
-        # Set rupture parameters
-        rctx.__dict__.update(rupture_parameters)
-        rctx.mag = event.magnitude
+        ctx.__dict__.update(rupture_parameters)
 
         # TODO: distances should be calculated when we refactor to be
         # able to import distance calculations
-        rctx.repi = np.array(
+        ctx.repi = np.array(
             [
                 gps2dist_azimuth(
                     st[0].stats.coordinates.latitude,
                     st[0].stats.coordinates.longitude,
                     event.latitude,
                     event.longitude,
                 )[0]
                 / 1000
             ]
         )
-        rctx.rjb = rctx.repi
-        rctx.rhypo = np.sqrt(rctx.repi**2 + event.depth_km**2)
-        rctx.rrup = rctx.rhypo
-        rctx.sids = np.array(range(np.size(rctx.rrup)))
-        pga, sd = gmpe.get_mean_and_stddevs(rctx, rctx, rctx, imt.PGA(), [])
+        ctx.rjb = ctx.repi
+        ctx.rhypo = np.sqrt(ctx.repi**2 + event.depth_km**2)
+        ctx.rrup = ctx.rhypo
+
+        result = cmaker.get_mean_stds([ctx])
+        pga = result[0][0][0]
 
         # Convert from ln(g) to %g
         predicted_pga = 100 * np.exp(pga[0])
         if predicted_pga > (pga_factor * recorded_pga):
             is_significant.append(True)
         else:
             is_significant.append(False)
```

### Comparing `gmprocess-1.3.2/src/gmprocess/waveform_processing/zero_crossings.py` & `gmprocess-2.0.0/src/gmprocess/waveform_processing/zero_crossings.py`

 * *Files identical despite different names*

### Comparing `gmprocess-1.3.2/src/gmprocess.egg-info/PKG-INFO` & `gmprocess-2.0.0/src/gmprocess.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmprocess
-Version: 1.3.2
+Version: 2.0.0
 Summary: USGS Automated Ground Motion Processing Software
 Author-email: Eric Thompson <emthompsone@usgs.gov>, Mike Hearne <mhearne@usgs.gov>, Brad Aagaard <baagaard@usgs.gov>, Bruce Worden <cbworden@contractor.usgs.gov>, John Rekoske <jrekoske@ucsd.edu>, Heather Hunsinger <hhunsinger@usgs.gov>, Gabe Ferragut <gferragut@usgs.gov>
 License: License
         =======
         
         Unless otherwise noted, This project is in the public domain in the United States
         because it contains materials that originally came from the United States Geological Survey, 
@@ -44,40 +44,41 @@
         to the fullest extent permitted by applicable law. 
         When using or citing the work, you should not imply endorsement by the author or the affirmer.
         
         
         
         [1]: https://creativecommons.org/publicdomain/zero/1.0/legalcode
         
-Requires-Python: <3.11,>=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: beautifulsoup4>=4.11.0
 Requires-Dist: configobj>=5.0.6
 Requires-Dist: esi-core>=1.0.1
 Requires-Dist: esi-utils-colors>1.0
 Requires-Dist: esi-utils-io>1.0
 Requires-Dist: esi-utils-rupture>1.0
 Requires-Dist: folium>=0.12
 Requires-Dist: gmpacket>=0.1.6
 Requires-Dist: h5py>=2.8
 Requires-Dist: lxml>=4.6.1
 Requires-Dist: matplotlib>=3.1.0
+Requires-Dist: numba>=0.58
 Requires-Dist: numpy<2.0,>=1.21
 Requires-Dist: obspy>=1.4.0
 Requires-Dist: openpyxl>=3.0.8
-Requires-Dist: openquake.engine>=3.14
+Requires-Dist: openquake.engine>=3.18
 Requires-Dist: pandas>=1.0
 Requires-Dist: ps2ff>=1.5.2
 Requires-Dist: pyasdf>=0.7
 Requires-Dist: pydantic>=2.0
 Requires-Dist: requests>=2.29
 Requires-Dist: ruamel.yaml>=0.17.16
 Requires-Dist: schema>=0.7
-Requires-Dist: scipy>=1.7
+Requires-Dist: scipy<1.13,>=1.7
 Requires-Dist: setuptools-scm>=6.3.2
 Requires-Dist: statsmodels>=0.12.2
 Requires-Dist: usgs-strec>=2.3.2
 Requires-Dist: xlrd>=2.0
 Provides-Extra: dev
 Requires-Dist: build>=0.7.0; extra == "dev"
 Requires-Dist: black>=21; extra == "dev"
@@ -110,23 +111,28 @@
 # Introduction
 This is a project designed to provide a number of functions related to parsing and processing earthquake ground motion data, building on top of the [ObsPy](https://github.com/obspy/obspy/wiki) library.
 Most of the extensions that we provide are to handle strong motion data and related issues.
 
 
 # Documentation
 - Please note, we are in the process of improving the documentation and that there are some incomplete sections.
-- The full documentation can be viewed locally by running the `doc_source/makedocs.sh` script.
+- The full documentation can be viewed locally by running the `docs/makedocs.sh` script.
 - The documentation is also available [here](https://ghsc.code-pages.usgs.gov/esi/groundmotion-processing/).
+- The MATLAB functions included in the `tools/matlab` directory include a short [tutorial](tools/matlab/readme.md)
 
 # Getting Help
 The developers can be reached at [gmprocess@usgs.gov](mailto:gmprocess@usgs.gov).
 
 If you would like to post an issue to ask a question, request a new feature, or report a bug, you can do so at the [github mirror](https://github.com/DOI-USGS/ghsc-esi-groundmotion-processing) of this repository. 
 
 If you would like to contribute merge requests to this repository, please let us know and we can add you as a collaborator. 
 This will require that you create an account at code.usgs.gov, which is a more involved process than creating a personal account at gitub.com and posting to the issues on the github mirror.
 
-# Reference
-If you wish to cite this software, please use this reference:
+# Suggested Citation
+If you wish to cite this software please cite:
 
-- Hearne, M., E. M. Thompson, H. Schovanec, J. Rekoske, B. T. Aagaard, and C. B. Worden (2019). USGS automated ground motion processing software, USGS Software Release, doi: [10.5066/P9ANQXN3](https://dx.doi.org/10.5066/P9ANQXN3).
+- Thompson, E.M., M. Hearne, B.T. Aagaard, J.M. Rekoske, C.B. Worden, M.P. Moschetti, H.E. Hunsinger, G.C. Ferragut, G.A. Parker, J.A. Smith, K.K. Smith, and A.R. Kottke (2024). USGS Automated Ground Motion Processing Software Version 2, U.S. Geological Survey software release. [https://doi.org/10.5066/P13HMKFJ](https://doi.org/10.5066/P13HMKFJ)
   
+
+# Disclaimer
+
+Any use of trade, firm, or product names is for descriptive purposes only and does not imply endorsement by the U.S. Government.
```

### Comparing `gmprocess-1.3.2/src/gmprocess.egg-info/requires.txt` & `gmprocess-2.0.0/src/gmprocess.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,26 +5,27 @@
 esi-utils-io>1.0
 esi-utils-rupture>1.0
 folium>=0.12
 gmpacket>=0.1.6
 h5py>=2.8
 lxml>=4.6.1
 matplotlib>=3.1.0
+numba>=0.58
 numpy<2.0,>=1.21
 obspy>=1.4.0
 openpyxl>=3.0.8
-openquake.engine>=3.14
+openquake.engine>=3.18
 pandas>=1.0
 ps2ff>=1.5.2
 pyasdf>=0.7
 pydantic>=2.0
 requests>=2.29
 ruamel.yaml>=0.17.16
 schema>=0.7
-scipy>=1.7
+scipy<1.13,>=1.7
 setuptools-scm>=6.3.2
 statsmodels>=0.12.2
 usgs-strec>=2.3.2
 xlrd>=2.0
 
 [build]
 build
```

