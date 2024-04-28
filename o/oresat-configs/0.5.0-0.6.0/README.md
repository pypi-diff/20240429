# Comparing `tmp/oresat_configs-0.5.0.tar.gz` & `tmp/oresat_configs-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat_configs-0.5.0.tar", last modified: Sat Apr 27 22:33:19 2024, max compression
+gzip compressed data, was "oresat_configs-0.6.0.tar", last modified: Sun Apr 28 04:36:51 2024, max compression
```

## Comparing `oresat_configs-0.5.0.tar` & `oresat_configs-0.6.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.690468 oresat_configs-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/.github/workflows/pypi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/build_and_install.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/docs/oresat0/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/oresat0/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/docs/oresat0_5/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/oresat0_5/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/docs/oresat1/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/oresat1/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/scripts/gen_beacon_rst.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/docs/static/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.694468 oresat_configs-0.5.0/docs/yamls/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/yamls/beacon_config.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/yamls/card_config.rst
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/docs/yamls/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.698468 oresat_configs-0.5.0/oresat_configs/
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-27 22:33:19.000000 oresat_configs-0.5.0/oresat_configs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    27449 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/_yaml_to_od.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.698468 oresat_configs-0.5.0/oresat_configs/base/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/adcs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/battery.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/c3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/cfc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/diode_test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/dxwifi.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/fw_common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/gps.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/reaction_wheel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/solar.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/star_tracker.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/base/sw_common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/beacon_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/card_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/card_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/cards.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.698468 oresat_configs-0.5.0/oresat_configs/oresat0/
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/oresat0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/oresat0/battery_overlay.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/oresat0/beacon.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/oresat_configs/oresat0_5/
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/oresat0_5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/oresat0_5/beacon.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/oresat_configs/oresat1/
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/oresat1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/oresat1/beacon.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/oresat_configs/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/gen_dbc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/gen_dcf.py
--rw-r--r--   0 runner    (1001) docker     (127)    25953 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/gen_fw_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/gen_xtce.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/list_cards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/pdo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/print_od.py
--rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/scripts/sdo_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/oresat_configs/standard_objects.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/oresat_configs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-27 22:33:19.000000 oresat_configs-0.5.0/oresat_configs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-27 22:33:19.000000 oresat_configs-0.5.0/oresat_configs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 22:33:19.000000 oresat_configs-0.5.0/oresat_configs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-27 22:33:19.000000 oresat_configs-0.5.0/oresat_configs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-27 22:33:19.000000 oresat_configs-0.5.0/oresat_configs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-27 22:33:19.000000 oresat_configs-0.5.0/oresat_configs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 22:33:19.702468 oresat_configs-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/tests/test_config_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/tests/test_oresat0.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/tests/test_oresat0_5.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-27 22:33:12.000000 oresat_configs-0.5.0/tests/test_oresat1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.729952 oresat_configs-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.713952 oresat_configs-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.713952 oresat_configs-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-28 04:36:51.729952 oresat_configs-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/build_and_install.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.717952 oresat_configs-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.717952 oresat_configs-0.6.0/docs/oresat0/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/docs/oresat0/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.717952 oresat_configs-0.6.0/docs/oresat0_5/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/docs/oresat0_5/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.717952 oresat_configs-0.6.0/docs/oresat1/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/docs/oresat1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.717952 oresat_configs-0.6.0/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/docs/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/docs/scripts/gen_beacon_rst.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.717952 oresat_configs-0.6.0/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/docs/static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.717952 oresat_configs-0.6.0/docs/yamls/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/docs/yamls/beacon_config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/docs/yamls/card_config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/docs/yamls/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.721952 oresat_configs-0.6.0/oresat_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 04:36:51.000000 oresat_configs-0.6.0/oresat_configs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27449 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/_yaml_to_od.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.721952 oresat_configs-0.6.0/oresat_configs/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8529 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/base/adcs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/base/battery.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16077 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/base/c3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/base/cfc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/base/diode_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/base/dxwifi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/base/fw_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/base/gps.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/base/reaction_wheel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/base/solar.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/base/star_tracker.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/base/sw_common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/beacon_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/card_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/card_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/cards.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.725952 oresat_configs-0.6.0/oresat_configs/oresat0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/oresat0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/oresat0/battery_overlay.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/oresat0/beacon.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.725952 oresat_configs-0.6.0/oresat_configs/oresat0_5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/oresat0_5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/oresat0_5/beacon.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.725952 oresat_configs-0.6.0/oresat_configs/oresat1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/oresat1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/oresat1/beacon.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.725952 oresat_configs-0.6.0/oresat_configs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15877 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/scripts/gen_dbc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/scripts/gen_dcf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25953 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/scripts/gen_fw_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11487 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/scripts/gen_xtce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/scripts/list_cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/scripts/pdo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/scripts/print_od.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/scripts/sdo_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/oresat_configs/standard_objects.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.725952 oresat_configs-0.6.0/oresat_configs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-04-28 04:36:51.000000 oresat_configs-0.6.0/oresat_configs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-28 04:36:51.000000 oresat_configs-0.6.0/oresat_configs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 04:36:51.000000 oresat_configs-0.6.0/oresat_configs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-28 04:36:51.000000 oresat_configs-0.6.0/oresat_configs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-28 04:36:51.000000 oresat_configs-0.6.0/oresat_configs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-28 04:36:51.000000 oresat_configs-0.6.0/oresat_configs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 04:36:51.729952 oresat_configs-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 04:36:51.725952 oresat_configs-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7840 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/tests/test_config_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/tests/test_oresat0.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/tests/test_oresat0_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-28 04:36:45.000000 oresat_configs-0.6.0/tests/test_oresat1.py
```

### Comparing `oresat_configs-0.5.0/.github/workflows/pypi.yaml` & `oresat_configs-0.6.0/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/.github/workflows/tests.yaml` & `oresat_configs-0.6.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/.gitignore` & `oresat_configs-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/LICENSE` & `oresat_configs-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/PKG-INFO` & `oresat_configs-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-configs
-Version: 0.5.0
+Version: 0.6.0
 Summary: OreSat mission configurations
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oresat_configs-0.5.0/README.md` & `oresat_configs-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/docs/Makefile` & `oresat_configs-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/docs/conf.py` & `oresat_configs-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/docs/make.bat` & `oresat_configs-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/docs/scripts/gen_beacon_rst.py` & `oresat_configs-0.6.0/docs/scripts/gen_beacon_rst.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/docs/yamls/card_config.rst` & `oresat_configs-0.6.0/docs/yamls/card_config.rst`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/__init__.py` & `oresat_configs-0.6.0/oresat_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/__main__.py` & `oresat_configs-0.6.0/oresat_configs/__main__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/_yaml_to_od.py` & `oresat_configs-0.6.0/oresat_configs/_yaml_to_od.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/base/__init__.py` & `oresat_configs-0.6.0/oresat_configs/base/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/base/adcs.yaml` & `oresat_configs-0.6.0/oresat_configs/base/adcs.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/base/battery.yaml` & `oresat_configs-0.6.0/oresat_configs/base/battery.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/base/c3.yaml` & `oresat_configs-0.6.0/oresat_configs/base/c3.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -595,14 +595,57 @@
 
 
 tpdos:
   - num: 1 # time sync TPDO
     fields:
       - [scet]
 
+  - num: 2
+    fields:
+    - [status]
+    - [tx_control, enable]
+    - [mode]
+    event_timer_ms: 5000
+
+  - num: 3
+    fields:
+    - [edl, sequence_count]
+    - [edl, rejected_count]
+    event_timer_ms: 5000
+
+  - num: 4
+    fields:
+      - [opd, status]
+      - [opd, has_fault]
+    event_timer_ms: 5000
+
+  - num: 5
+    fields:
+      - [node_manager, total_nodes]
+      - [node_manager, nodes_off]
+      - [node_manager, nodes_booting]
+      - [node_manager, nodes_on]
+      - [node_manager, nodes_with_errors]
+      - [node_manager, nodes_not_found]
+      - [node_manager, nodes_dead]
+    event_timer_ms: 5000
+
+  - num: 6
+    fields:
+      - [uhf, rx_packets]
+      - [uhf, rssi]
+    event_timer_ms: 5000
+
+  - num: 7
+    fields:
+      - [lband, rx_packets]
+      - [lband, rssi]
+      - [lband, synth_relock_count]
+    event_timer_ms: 5000
+
 fram:
   # DO NOT change this order, only append!
   - [status]
   - [rtc, timestamp]
   - [rtc, alarm_a]
   - [rtc, alarm_b]
   - [rtc, wakeup_interval]
```

### Comparing `oresat_configs-0.5.0/oresat_configs/base/cfc.yaml` & `oresat_configs-0.6.0/oresat_configs/base/cfc.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/base/dxwifi.yaml` & `oresat_configs-0.6.0/oresat_configs/base/dxwifi.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -115,8 +115,11 @@
       
 
 tpdos:
   - num: 3
     fields:
       - [status]
       - [radio, temperature]
+      - [transmission, bit_rate]
+      - [transmission, images_transmitted]
+      - [transmission, enable_pa]
     event_timer_ms: 1000
```

### Comparing `oresat_configs-0.5.0/oresat_configs/base/fw_common.yaml` & `oresat_configs-0.6.0/oresat_configs/base/fw_common.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/base/gps.yaml` & `oresat_configs-0.6.0/oresat_configs/base/gps.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/base/reaction_wheel.yaml` & `oresat_configs-0.6.0/oresat_configs/base/reaction_wheel.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/base/solar.yaml` & `oresat_configs-0.6.0/oresat_configs/base/solar.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/base/star_tracker.yaml` & `oresat_configs-0.6.0/oresat_configs/base/star_tracker.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/base/sw_common.yaml` & `oresat_configs-0.6.0/oresat_configs/base/sw_common.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/beacon_config.py` & `oresat_configs-0.6.0/oresat_configs/beacon_config.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/card_config.py` & `oresat_configs-0.6.0/oresat_configs/card_config.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/card_info.py` & `oresat_configs-0.6.0/oresat_configs/card_info.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/cards.csv` & `oresat_configs-0.6.0/oresat_configs/cards.csv`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/constants.py` & `oresat_configs-0.6.0/oresat_configs/constants.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/oresat0/__init__.py` & `oresat_configs-0.6.0/oresat_configs/oresat0/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/oresat0/battery_overlay.yaml` & `oresat_configs-0.6.0/oresat_configs/oresat0/battery_overlay.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/oresat0/beacon.yaml` & `oresat_configs-0.6.0/oresat_configs/oresat0/beacon.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/oresat0_5/__init__.py` & `oresat_configs-0.6.0/oresat_configs/oresat0_5/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/oresat0_5/beacon.yaml` & `oresat_configs-0.6.0/oresat_configs/oresat0_5/beacon.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/oresat1/__init__.py` & `oresat_configs-0.6.0/oresat_configs/oresat1/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/scripts/gen_dbc.py` & `oresat_configs-0.6.0/oresat_configs/scripts/gen_dbc.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/scripts/gen_dcf.py` & `oresat_configs-0.6.0/oresat_configs/scripts/gen_dcf.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/scripts/gen_fw_files.py` & `oresat_configs-0.6.0/oresat_configs/scripts/gen_fw_files.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/scripts/gen_xtce.py` & `oresat_configs-0.6.0/oresat_configs/scripts/gen_xtce.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/scripts/list_cards.py` & `oresat_configs-0.6.0/oresat_configs/scripts/list_cards.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/scripts/pdo.py` & `oresat_configs-0.6.0/oresat_configs/scripts/pdo.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/scripts/print_od.py` & `oresat_configs-0.6.0/oresat_configs/scripts/print_od.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/scripts/sdo_transfer.py` & `oresat_configs-0.6.0/oresat_configs/scripts/sdo_transfer.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs/standard_objects.yaml` & `oresat_configs-0.6.0/oresat_configs/standard_objects.yaml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/oresat_configs.egg-info/PKG-INFO` & `oresat_configs-0.6.0/oresat_configs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-configs
-Version: 0.5.0
+Version: 0.6.0
 Summary: OreSat mission configurations
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `oresat_configs-0.5.0/oresat_configs.egg-info/SOURCES.txt` & `oresat_configs-0.6.0/oresat_configs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/pyproject.toml` & `oresat_configs-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/tests/__init__.py` & `oresat_configs-0.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat_configs-0.5.0/tests/test_config_types.py` & `oresat_configs-0.6.0/tests/test_config_types.py`

 * *Files identical despite different names*

