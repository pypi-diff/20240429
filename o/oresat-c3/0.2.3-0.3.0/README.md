# Comparing `tmp/oresat-c3-0.2.3.tar.gz` & `tmp/oresat_c3-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat-c3-0.2.3.tar", last modified: Wed Jan 10 08:30:44 2024, max compression
+gzip compressed data, was "oresat_c3-0.3.0.tar", last modified: Sun Apr 28 22:21:11 2024, max compression
```

## Comparing `oresat-c3-0.2.3.tar` & `oresat_c3-0.3.0.tar`

### file list

```diff
@@ -1,42 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 08:30:44.507424 oresat-c3-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-01-10 08:30:44.507424 oresat-c3-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 08:30:44.503424 oresat-c3-0.2.3/oresat_c3/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 08:30:44.503424 oresat-c3-0.2.3/oresat_c3/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/drivers/fm24cl64b.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/drivers/max7310.py
--rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/drivers/si41xx.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 08:30:44.503424 oresat-c3-0.2.3/oresat_c3/protocols/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/protocols/ax25.py
--rw-r--r--   0 runner    (1001) docker     (127)    11696 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/protocols/edl_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/protocols/edl_packet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 08:30:44.507424 oresat-c3-0.2.3/oresat_c3/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/services/beacon.py
--rw-r--r--   0 runner    (1001) docker     (127)    19473 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/services/edl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11805 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/services/node_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/services/radios.py
--rw-r--r--   0 runner    (1001) docker     (127)    11455 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/services/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 08:30:44.507424 oresat-c3-0.2.3/oresat_c3/subsystems/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/subsystems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/subsystems/antennas.py
--rw-r--r--   0 runner    (1001) docker     (127)    14093 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/subsystems/opd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 08:30:44.507424 oresat-c3-0.2.3/oresat_c3/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/templates/beacon.html
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/templates/keys.html
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/templates/node_manager.html
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/oresat_c3/templates/state.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 08:30:44.507424 oresat-c3-0.2.3/oresat_c3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4768 2024-01-10 08:30:44.000000 oresat-c3-0.2.3/oresat_c3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-01-10 08:30:44.000000 oresat-c3-0.2.3/oresat_c3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 08:30:44.000000 oresat-c3-0.2.3/oresat_c3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-10 08:30:44.000000 oresat-c3-0.2.3/oresat_c3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-10 08:30:44.000000 oresat-c3-0.2.3/oresat_c3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-10 08:30:44.000000 oresat-c3-0.2.3/oresat_c3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-01-10 08:30:31.000000 oresat-c3-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-10 08:30:44.507424 oresat-c3-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.473003 oresat_c3-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.461003 oresat_c3-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.461003 oresat_c3-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-28 22:21:11.473003 oresat_c3-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.465003 oresat_c3-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/edl.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/opd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/state.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.465003 oresat_c3-0.3.0/docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/static/comms_ipc.drawio
+-rw-r--r--   0 runner    (1001) docker     (127)    33084 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/static/comms_ipc.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    98849 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/docs/static/opd.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.465003 oresat_c3-0.3.0/oresat_c3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-28 22:21:11.000000 oresat_c3-0.3.0/oresat_c3/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.465003 oresat_c3-0.3.0/oresat_c3/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/drivers/fm24cl64b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/drivers/max7310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9300 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/drivers/si41xx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.465003 oresat_c3-0.3.0/oresat_c3/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/protocols/ax25.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11692 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/protocols/edl_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6763 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/protocols/edl_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/oresat_c3/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/services/beacon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29640 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/services/edl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12024 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/services/node_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/services/radios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11807 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/services/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/oresat_c3/subsystems/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/subsystems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/subsystems/antennas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13522 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/subsystems/opd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/subsystems/rtc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/oresat_c3/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/templates/beacon.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/templates/keys.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/templates/node_manager.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/oresat_c3/templates/state.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.473003 oresat_c3-0.3.0/oresat_c3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-04-28 22:21:11.000000 oresat_c3-0.3.0/oresat_c3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-28 22:21:11.000000 oresat_c3-0.3.0/oresat_c3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 22:21:11.000000 oresat_c3-0.3.0/oresat_c3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-28 22:21:11.000000 oresat_c3-0.3.0/oresat_c3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-28 22:21:11.000000 oresat_c3-0.3.0/oresat_c3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-28 22:21:11.000000 oresat_c3-0.3.0/oresat_c3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14200 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/scripts/edl_cmd_shell.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13336 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/scripts/edl_file_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4214 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/scripts/edl_ping_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 22:21:11.473003 oresat_c3-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/tests/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/drivers/test_fm23cl64b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/drivers/test_max7310.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/tests/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/protocols/test_ax25.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/protocols/test_edl_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/protocols/test_edl_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9226 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/services/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:11.469003 oresat_c3-0.3.0/tests/subsystems/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/subsystems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-28 22:21:06.000000 oresat_c3-0.3.0/tests/subsystems/test_opd.py
```

### Comparing `oresat-c3-0.2.3/LICENSE` & `oresat_c3-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat-c3-0.2.3/PKG-INFO` & `oresat_c3-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: oresat-c3
-Version: 0.2.3
+Version: 0.3.0
 Summary: OreSat C3 OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bitstring
+Requires-Dist: cfdp-py
+Requires-Dist: dataclasses-json
 Requires-Dist: oresat-configs
-Requires-Dist: oresat-olaf>=3.3.0
+Requires-Dist: oresat-olaf>=3.5.0
 Requires-Dist: smbus2
 Requires-Dist: spacepackets
 
 # OreSat C3 Software
 
 Main application for Octavo A8 with Debian Linux version of the C3 card.
 
 The C3 card is the "flight" computer of OreSat. C3 stands for command,
-control, and commuication. It handles all commuications and controls
+control, and communication. It handles all communications and controls
 the state of the satellite.
 
 **Note:** For OreSat0, the C3 card used STM32F4 and ChibiOS, for that project
 see the [oresat-firmware] repo and the `src/f4/app_control` directory.
 The C3 card was converted to Octavo A8 card to simplify the code base
 by swapping from heavily embedded system using ChibiOS to a general
 Linux-environment using Python and make to use existing Python libraries.
 
 Like all OreSat software projects it is built using OLAF (OreSat Linux App
-Framework), which it built ontop of [CANopen for Python] project. See the
+Framework), which it built on top of [CANopen for Python] project. See the
 [oresat-olaf] repo for more info about OLAF.
 
-## Quickstart
+## Quick Start
 
-**For development**, install `oresat-configs` from the github repo at 
+**For development**, install `oresat-configs` from the GitHub repo at
 https://github.com/oresat/oresat-configs (not from PyPI). That repo may have
 changes that are not apart of the latest release yet.
 
 Install dependencies
 
 ```bash
 $ pip3 install -r requirements.txt
@@ -58,15 +60,15 @@
 
 Run the C3 app
 
 ```bash
 $ python3 -m oresat_c3
 ```
 
-Can select the CAN bus to use (`vcan0`, `can0`, etc) with the `-b BUS` arg.
+Can select the CAN bus to use (`vcan0`, `can0`, etc) with the `-b BUS` argument.
 
 Can mock hardware by using the `-m HARDWARE` flag.
 
 - The`-m all` argument can be used to mock hardware (CAN bus is always
   required).
 - The `-m opd` argument would only mock the hardware for the OPD subsystem and
   expect all other hardware
@@ -106,15 +108,15 @@
 
 To manually build the documentation:
 
 ```bash
 $ make -C docs html
 ```
 
-Open `docs/build/html/index.html` in a web broswer
+Open `docs/build/html/index.html` in a web browser
 
 ## Unit Tests
 
 This project uses python's build in `unittest` module for unit testing.
 
 To run units:
```

### Comparing `oresat-c3-0.2.3/README.md` & `oresat_c3-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # OreSat C3 Software
 
 Main application for Octavo A8 with Debian Linux version of the C3 card.
 
 The C3 card is the "flight" computer of OreSat. C3 stands for command,
-control, and commuication. It handles all commuications and controls
+control, and communication. It handles all communications and controls
 the state of the satellite.
 
 **Note:** For OreSat0, the C3 card used STM32F4 and ChibiOS, for that project
 see the [oresat-firmware] repo and the `src/f4/app_control` directory.
 The C3 card was converted to Octavo A8 card to simplify the code base
 by swapping from heavily embedded system using ChibiOS to a general
 Linux-environment using Python and make to use existing Python libraries.
 
 Like all OreSat software projects it is built using OLAF (OreSat Linux App
-Framework), which it built ontop of [CANopen for Python] project. See the
+Framework), which it built on top of [CANopen for Python] project. See the
 [oresat-olaf] repo for more info about OLAF.
 
-## Quickstart
+## Quick Start
 
-**For development**, install `oresat-configs` from the github repo at 
+**For development**, install `oresat-configs` from the GitHub repo at
 https://github.com/oresat/oresat-configs (not from PyPI). That repo may have
 changes that are not apart of the latest release yet.
 
 Install dependencies
 
 ```bash
 $ pip3 install -r requirements.txt
@@ -37,15 +37,15 @@
 
 Run the C3 app
 
 ```bash
 $ python3 -m oresat_c3
 ```
 
-Can select the CAN bus to use (`vcan0`, `can0`, etc) with the `-b BUS` arg.
+Can select the CAN bus to use (`vcan0`, `can0`, etc) with the `-b BUS` argument.
 
 Can mock hardware by using the `-m HARDWARE` flag.
 
 - The`-m all` argument can be used to mock hardware (CAN bus is always
   required).
 - The `-m opd` argument would only mock the hardware for the OPD subsystem and
   expect all other hardware
@@ -85,15 +85,15 @@
 
 To manually build the documentation:
 
 ```bash
 $ make -C docs html
 ```
 
-Open `docs/build/html/index.html` in a web broswer
+Open `docs/build/html/index.html` in a web browser
 
 ## Unit Tests
 
 This project uses python's build in `unittest` module for unit testing.
 
 To run units:
```

### Comparing `oresat-c3-0.2.3/oresat_c3/__init__.py` & `oresat_c3-0.3.0/oresat_c3/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 """C3 OLAF App."""
 
 from enum import Enum, IntEnum
 
-__version__ = "0.2.3"
+try:
+    from ._version import version as __version__  # type: ignore
+except ImportError:
+    __version__ = "0.0.0"  # package is not installed
 
 
 class C3State(IntEnum):
     """All valid C3 states"""
 
     OFFLINE = ord("A")
     """This state is never actually reachable by the device. Reset vector is ``PRE_DEPLOY``."""
```

### Comparing `oresat-c3-0.2.3/oresat_c3/__main__.py` & `oresat_c3-0.3.0/oresat_c3/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 from . import C3State, __version__
 from .services.beacon import BeaconService
 from .services.edl import EdlService
 from .services.node_manager import NodeManagerService
 from .services.radios import RadiosService
 from .services.state import StateService
+from .subsystems.rtc import set_system_time_to_rtc_time
 
 
 @rest_api.app.route("/beacon")
 def beacon_template():
     """Render beacon template."""
     return render_olaf_template("beacon.html", name="Beacon")
 
@@ -103,26 +104,29 @@
             set_cpufreq_gov("powersave")
             performance = False
 
 
 def main():
     """OreSat C3 app main."""
 
+    set_system_time_to_rtc_time()
+
     path = os.path.dirname(os.path.abspath(__file__))
 
     args, config = olaf_setup("c3")
     mock_args = [i.lower() for i in args.mock_hw]
     mock_hw = len(mock_args) != 0
 
     # start watchdog thread ASAP
     thread = Thread(target=watchdog, daemon=True)
     thread.start()
 
     app.od["versions"]["sw_version"].value = __version__
-    app.od["hw_id"].value = get_hw_id(mock_hw)
+    if app.od["versions"]["hw_version"].value == "6.0":
+        app.od["hw_id"].value = get_hw_id(mock_hw)
 
     state_service = StateService(config.fram_def, mock_hw)
     radios_service = RadiosService(mock_hw)
     beacon_service = BeaconService(config.beacon_def, radios_service)
     node_mgr_service = NodeManagerService(config.cards, mock_hw)
     edl_service = EdlService(app.node, radios_service, node_mgr_service, beacon_service)
```

### Comparing `oresat-c3-0.2.3/oresat_c3/drivers/fm24cl64b.py` & `oresat_c3-0.3.0/oresat_c3/drivers/fm24cl64b.py`

 * *Files identical despite different names*

### Comparing `oresat-c3-0.2.3/oresat_c3/drivers/max7310.py` & `oresat_c3-0.3.0/oresat_c3/drivers/max7310.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             try:
                 with SMBus(self._bus_num) as bus:
                     bus.i2c_rdwr(write)
             except (TimeoutError, OSError):
                 raise Max7310Error(f"MAX7310 at address 0x{self._addr:02X} does not exist")
 
     def _valid_pin(self, pin_num: int):
-        if pin_num <= 0 or pin_num > 8:
+        if pin_num < 0 or pin_num > 8:
             raise Max7310Error(f"invalid pin_num: {pin_num}, must be between 0 and 7")
 
     def configure(
         self, output_port: int, polarity_inversion: int, configuration: int, timeout: int
     ):
         """
         Configure the MAX7310 registers.
```

### Comparing `oresat-c3-0.2.3/oresat_c3/drivers/si41xx.py` & `oresat_c3-0.3.0/oresat_c3/drivers/si41xx.py`

 * *Files identical despite different names*

### Comparing `oresat-c3-0.2.3/oresat_c3/protocols/ax25.py` & `oresat_c3-0.3.0/oresat_c3/protocols/ax25.py`

 * *Files identical despite different names*

### Comparing `oresat-c3-0.2.3/oresat_c3/protocols/edl_command.py` & `oresat_c3-0.3.0/oresat_c3/protocols/edl_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Anything dealing with packing and unpacking EDL (Engineering Data Link) C3 command packets.
 
-These package are defined as 1 octect for code and X octects for the data.
+These package are defined as 1 octet for code and X octets for the data.
 
 The EDL code is used to identify the message the rest of message is for argument for
-request, and values for responeses.
+request, and values for responses.
 """
 
 import struct
 from collections import namedtuple
 from enum import IntEnum, auto
 
 EdlCommand = namedtuple(
@@ -226,15 +226,15 @@
     RTC_SET_TIME = auto()
     """
     Set the RTC time
 
     Parameters
     ----------
     time: uint32
-        The unix time in seconds.
+        The Unix time in seconds.
 
     Returns
     -------
     bool
         The RTC time was set successfully.
     """
 
@@ -247,15 +247,15 @@
     -------
     bool
         Time sync was sent.
     """
 
     BEACON_PING = auto()
     """
-    C3 will response with a beacon reguardless of tx state.
+    C3 will response with a beacon regardless of tx state.
     """
 
     PING = auto()
     """
     A basic ping to the C3.
 
     Parameters
```

### Comparing `oresat-c3-0.2.3/oresat_c3/protocols/edl_packet.py` & `oresat_c3-0.3.0/oresat_c3/protocols/edl_packet.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     """USLP virtual channel IDs for EDL packets"""
 
     C3_COMMAND = 0
     FILE_TRANSFER = 1
 
 
 def crc16_bytes(data: bytes) -> bytes:
-    """Helper function to generate the crc16 of a message as bytes"""
+    """Helper function to generate the CRC16 of a message as bytes"""
 
     return binascii.crc_hqx(data, 0).to_bytes(2, "little")
 
 
 def gen_hmac(hmac_key: bytes, message: bytes) -> bytes:
     """Helper function to generate HMAC value from HMAC key and the message."""
 
@@ -58,15 +58,15 @@
 class EdlPacket:
     """
     An EDL (Engineering Data Link) packet.
 
     Only packs and unpacks the packet (does not process/run it).
     """
 
-    SPACECRAFT_ID = 0x4F53  # aka "OS" in ascii
+    SPACECRAFT_ID = 0x4F53  # aka "OS" in ASCII
 
     PRIMARY_HEADER_LEN = 7
     SEQ_NUM_LEN = 4
     DFH_LEN = 1
     HMAC_LEN = 32
     FECF_LEN = 2
     TC_MIN_LEN = PRIMARY_HEADER_LEN + SEQ_NUM_LEN + DFH_LEN + HMAC_LEN + FECF_LEN
```

### Comparing `oresat-c3-0.2.3/oresat_c3/services/beacon.py` & `oresat_c3-0.3.0/oresat_c3/services/beacon.py`

 * *Files identical despite different names*

### Comparing `oresat-c3-0.2.3/oresat_c3/services/node_manager.py` & `oresat_c3-0.3.0/oresat_c3/services/node_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """'
 Node manager service.
 """
 
 import json
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass
 from enum import IntEnum
-from time import time
+from time import monotonic
 from typing import Union
 
 import canopen
 from dataclasses_json import dataclass_json
 from olaf import Service, logger
 from oresat_configs import Card
 
@@ -100,15 +100,15 @@
                 continue
 
             self.opd[name] = node
 
         self.opd_addr_to_name = {info.opd_address: name for name, info in cards.items()}
         self.node_id_to_name = {info.node_id: name for name, info in cards.items()}
 
-        self._data = {name: Node(**info.to_dict()) for name, info in cards.items()}
+        self._data = {name: Node(**asdict(info)) for name, info in cards.items()}
         self._data["c3"].status = NodeState.ON
         self._loops = -1
 
         self._flight_mode_obj: canopen.objectdictionary.Variable = None
         self._nodes_off_obj: canopen.objectdictionary.Variable = None
         self._nodes_booting_obj: canopen.objectdictionary.Variable = None
         self._nodes_on_obj: canopen.objectdictionary.Variable = None
@@ -150,36 +150,38 @@
             return next_state
 
         if self._data[name].processor == "stm32":
             timeout = self._STM32_BOOT_TIMEOUT
         else:
             timeout = self._OCTAVO_BOOT_TIMEOUT
 
-        last_hb = self.node.node_status[name][1]
-        if self._data[name].last_enable + timeout > time():
-            if time() > last_hb + self._RESET_TIMEOUT_S:
+        last_hb = self.node.node_status[name][2]
+        if self._data[name].last_enable + timeout > monotonic():
+            if monotonic() > last_hb + self._RESET_TIMEOUT_S:
                 next_state = NodeState.BOOT
             else:
                 next_state = NodeState.ON
-        elif self._flight_mode_obj.value and time() > last_hb + self._RESET_TIMEOUT_S:
+        elif self._data[name].status == NodeState.ERROR:
+            next_state = NodeState.ERROR
+        elif self._flight_mode_obj.value and monotonic() > (last_hb + self._RESET_TIMEOUT_S):
             logger.error(
                 f"CANopen node {name} has had no heartbeats in " f"{self._RESET_TIMEOUT_S} seconds"
             )
             next_state = NodeState.ERROR
         else:
             next_state = NodeState.ON
 
         return next_state
 
     def _get_nodes_state(self, name: str) -> NodeState:
         """Determine a node's state."""
 
         # update status of data not on the OPD
         if self._data[name].opd_address == 0:
-            if time() > self.node.node_status[name][1] + self._HB_TIMEOUT:
+            if monotonic() > (self.node.node_status[name][2] + self._HB_TIMEOUT):
                 next_state = NodeState.OFF
             else:
                 next_state = NodeState.ON
             return next_state
 
         # opd subsystem is off
         if self.opd.status == OpdState.DISABLED:
@@ -247,14 +249,17 @@
         self._nodes_not_found_obj.value = nodes_not_found
         self._nodes_dead_obj.value = nodes_dead
 
         if self.opd.status in [OpdState.DEAD, OpdState.DISABLED]:
             self._loops = -1
             return  # nothing to monitor
 
+        if nodes_not_found == len(self._data):
+            self._loops = 0
+
         # reset data with errors and probe for data not found
         for name, info in self._data.items():
             if info.opd_address == 0:
                 continue
 
             if self._loops % 60 == 0 and self._data[name].status == NodeState.NOT_FOUND:
                 self.opd[name].probe(True)
@@ -284,15 +289,15 @@
         if node.status == NodeState.DEAD:
             logger.error(f"cannot enable node {name} as it is DEAD")
             return
 
         self.opd[name].enable()
         if child_node:
             self.opd[node.child].enable()
-        node.last_enable = time()
+        node.last_enable = monotonic()
 
     def disable(self, name: Union[str, int]):
         """Disable a OreSat node."""
 
         if isinstance(name, int):
             name = self.opd_addr_to_name[name]
 
@@ -336,9 +341,9 @@
 
     def _set_opd_status(self, value: int):
         if value == 0:
             self.opd.disable()
         elif value == 1:
             if self.opd.status == OpdState.DISABLED:
                 for node in self._data.values():
-                    node.last_enable = time()
+                    node.last_enable = monotonic()
             self.opd.enable()
```

### Comparing `oresat-c3-0.2.3/oresat_c3/services/radios.py` & `oresat_c3-0.3.0/oresat_c3/services/radios.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """'
 Radios Service
 
 Handles interfacing with the AX5043 radio driver app.
 """
 
 import socket
-from typing import List
+from queue import SimpleQueue
 
 from olaf import Gpio, Service, logger
 
 from ..drivers.si41xx import Si41xx, Si41xxIfdiv
 
 
 class RadiosService(Service):
@@ -62,15 +62,15 @@
         self._edl_uplink_socket.bind(self.EDL_UPLINK_ADDR)
         self._edl_uplink_socket.settimeout(1)
 
         # EDL downlink: UDP client
         logger.info(f"EDL downlink socket: {self.EDL_DOWNLINK_ADDR}")
         self._edl_downlink_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
 
-        self.recv_queue: List[bytes] = []
+        self.recv_queue: SimpleQueue[bytes] = SimpleQueue()
 
     def on_start(self):
         if not self._mock_hw:
             self.node.add_daemon("lband")
             self.node.add_daemon("uhf")
         self.enable()
 
@@ -83,15 +83,15 @@
             logger.error("si41xx unlocked, resetting lband synth")
             self._relock_count += 1
             self.node.od["lband"]["synth_relock_count"].value = self._relock_count.bit_length()
             self._si41xx.stop()
             self._si41xx.start()
         recv = self._recv_edl_request()
         if recv:
-            self.recv_queue.append(recv)
+            self.recv_queue.put(recv)
 
     def on_stop(self):
         self.disable()
 
     def enable(self):
         """Enable the radios."""
```

### Comparing `oresat-c3-0.2.3/oresat_c3/services/state.py` & `oresat_c3-0.3.0/oresat_c3/services/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 C3 State Service
 
 This handles the main C3 state machine and saving state.
 """
 
+import os
 import subprocess
-from time import time
+from time import monotonic, time
 
 import canopen
 from olaf import NodeStop, Service, UpdaterState, logger
 
 from .. import C3State
 from ..drivers.fm24cl64b import Fm24cl64b
 from ..subsystems.antennas import Antennas
+from ..subsystems.rtc import set_rtc_time
 
 
 class StateService(Service):
     """C3 State Service."""
 
     BAT_LEVEL_LOW = 6500  # in mV
     I2C_BUS_NUM = 2
@@ -28,15 +30,15 @@
         self._fram_objs = fram_objs
         self._fram = Fm24cl64b(self.I2C_BUS_NUM, self.FRAM_I2C_ADDR, mock_hw)
         self._antennas = Antennas(mock_hw)
         self._attempts = 0
         self._loops = 0
         self._last_state = C3State.OFFLINE
         self._last_antennas_deploy = 0
-        self._boot_time = time()
+        self._start_time = monotonic()
 
         self._c3_state_obj: canopen.objectdictionary.Variable = None
         self._reset_timeout_obj: canopen.objectdictionary.Variable = None
         self._attempts_obj: canopen.objectdictionary.Variable = None
         self._deployed_obj: canopen.objectdictionary.Variable = None
         self._pre_deploy_timeout_obj: canopen.objectdictionary.Variable = None
         self._ant_attempt_timeout_obj: canopen.objectdictionary.Variable = None
@@ -69,27 +71,30 @@
         self._last_tx_enable_obj = tx_control_rec["last_enable_timestamp"]
         self._last_edl_obj = edl_rec["last_timestamp"]
         self._edl_timeout_obj = edl_rec["timeout"]
         self._vbatt_bp1_obj = bat_1_rec["pack_1_vbatt"]
         self._vbatt_bp2_obj = bat_1_rec["pack_2_vbatt"]
 
         self.restore_state()
-        self._last_tx_enable_obj.value = 0
+        if not self._tx_enable_obj.value:
+            self._last_tx_enable_obj.value = 0
         if self._c3_state_obj.value == C3State.EDL:
             self._c3_state_obj.value = C3State.STANDBY.value
 
         self.node.add_sdo_callbacks("tx_control", "enable", None, self._on_write_tx_enable)
 
         # make sure the initial state is valid (will be invalid on a cleared F-RAM)
         if self._c3_state_obj.value not in list(C3State):
             self._c3_state_obj.value = C3State.PRE_DEPLOY.value
 
         self._last_state = self._c3_state_obj.value
         logger.info(f"C3 initial state: {C3State(self._last_state).name}")
 
+        self._start_time = monotonic()
+
     def on_stop(self):
         self.store_state()
 
     def _on_write_tx_enable(self, data: bool):
         """On SDO write set tx enable and last enable timestamp objects."""
 
         self._tx_enable_obj.value = data
@@ -103,46 +108,49 @@
     def _reset(self):
         if self.node.od["updater"]["status"].value == UpdaterState.UPDATING:
             return
 
         logger.info("system reset")
 
         result = subprocess.run(
-            ["systemctl", "stop", "oresat-c3-watchdog"], shell=True, check=True, capture_output=True
+            ["systemctl", "stop", "oresat-c3-watchdog"],
+            shell=True,
+            check=False,
+            capture_output=True,
         )
 
-        if result.returncode == 0:
+        if result.returncode != 0:
             logger.error("stopping watchdog app failed, doing a hard reset")
             self.node.stop(NodeStop.HARD_RESET)
 
     def _pre_deploy(self):
         """PRE_DEPLOY state method."""
 
-        if (self._boot_time + self._pre_deploy_timeout_obj.value) > time():
+        if (monotonic() - self._start_time) < self._pre_deploy_timeout_obj.value:
             if not self._tx_enable_obj.value:
                 self._tx_enable_obj.value = True  # start beacons
                 self._last_tx_enable_obj.value = int(time())
         else:
             logger.info("pre-deploy timeout reached")
             self._c3_state_obj.value = C3State.DEPLOY.value
 
     def _deploy(self):
         """DEPLOY state method."""
 
         if not self._deployed_obj.value and self._attempts < self._attempts_obj.value:
             if (
-                time() > self._last_antennas_deploy + self._ant_reattempt_timeout_obj.value
+                monotonic() > (self._last_antennas_deploy + self._ant_reattempt_timeout_obj.value)
                 and self.is_bat_lvl_good
             ):
                 logger.info(f"deploying antennas, attempt {self._attempts + 1}")
                 self._antennas.deploy(
                     self._ant_attempt_timeout_obj.value,
                     self._ant_attempt_between_timeout_obj.value,
                 )
-                self._last_antennas_deploy = time()
+                self._last_antennas_deploy = monotonic()
                 self._attempts += 1
             # wait for battery to be at a good level
         else:
             logger.info("antennas deployed")
             self._c3_state_obj.value = C3State.STANDBY.value
             self._deployed_obj.value = True
             self._attempts = 0
@@ -240,15 +248,18 @@
             and self._vbatt_bp2_obj.value > self.BAT_LEVEL_LOW
         )
 
     @property
     def has_reset_timed_out(self) -> bool:
         """bool: Helper property to check if the reset timeout has been reached."""
 
-        return (time() - self._boot_time) >= self._reset_timeout_obj.value
+        if os.geteuid() != 0 or not self.node.od["flight_mode"].value:
+            return False
+
+        return (monotonic() - self._start_time) > self._reset_timeout_obj.value
 
     def store_state(self):
         """Store the state in F-RAM."""
 
         if self._c3_state_obj.value == C3State.PRE_DEPLOY:
             return  # Do not store state in PRE_DEPLOY state
 
@@ -281,15 +292,15 @@
             else:
                 size = len(obj.encode_raw(obj.default))
                 raw = self._fram.read(offset, size)
                 obj.value = obj.decode_raw(raw)
             offset += size
 
     def clear_state(self):
-        """Clear the state from F-RAM, key will be stored again after clear."""
+        """Clear the rtc time and state from F-RAM; keys will be stored again after clear."""
 
         self._fram.clear()
 
         offset = 0
         for obj in self._fram_objs:
             if obj.data_type == canopen.objectdictionary.DOMAIN:
                 continue
@@ -299,7 +310,9 @@
                 raw_len = len(obj.default)
                 self._fram.write(offset, raw)
             else:
                 raw = obj.encode_raw(obj.value)
                 raw_len = len(raw)
 
             offset += raw_len
+
+        set_rtc_time(0)
```

### Comparing `oresat-c3-0.2.3/oresat_c3/subsystems/antennas.py` & `oresat_c3-0.3.0/oresat_c3/subsystems/antennas.py`

 * *Files identical despite different names*

### Comparing `oresat-c3-0.2.3/oresat_c3/subsystems/opd.py` & `oresat_c3-0.3.0/oresat_c3/subsystems/opd.py`

 * *Files 3% similar despite different names*

```diff
@@ -303,41 +303,21 @@
 
         return self._max7310.output_status(self._UART_PIN)
 
 
 class OpdOctavoNode(OpdNode):
     """A Octavo A8-based OPD Node"""
 
-    _BOOT_PIN = 5  # boot select; eMMC or SD card
+    _SYS_BOOT2 = 0
     _UART_PIN = 7  # connect to C3 UART
 
-    def enable(self, boot_select: bool = True) -> OpdNodeState:
-        """
-        Enable the OPD node.
-
-        Parameters
-        ----------
-        boot_select: bool
-            Boot of of eMMC or SD card. Not implemented yet.
-
-        Returns
-        -------
-        OpdNodeState
-            The node state after disabling the node.
-        """
-
-        try:
-            if boot_select:
-                self._max7310.output_set(self._BOOT_PIN)
-            else:
-                self._max7310.output_clear(self._BOOT_PIN)
-        except Max7310Error:
-            self._status = OpdNodeState.FAULT
-            return self._status
+    def enable(self) -> OpdNodeState:
+        """Enable the node"""
 
+        self._max7310.output_set(self._SYS_BOOT2)
         return super().enable()
 
     def enable_uart(self):
         """Connect the node the C3's UART"""
 
         self._max7310.output_set(self._UART_PIN)
 
@@ -407,16 +387,15 @@
     def __getitem__(self, name: str) -> OpdNode:
         return self._nodes[name]
 
     def __setitem__(self, name: str, node: OpdNode):
         self._nodes[name] = node
 
     def __iter__(self) -> OpdNode:
-        for node in self._nodes.values():
-            yield node
+        yield from self._nodes.values()
 
     def enable(self):
         """Enable the OPD subsystem, will also do a scan."""
 
         if self._status == OpdState.DEAD:
             raise OpdError("OPD subsystem is consider dead")
         if self._status in [OpdState.ENABLED, OpdState.FAULT]:
```

### Comparing `oresat-c3-0.2.3/oresat_c3/templates/keys.html` & `oresat_c3-0.3.0/oresat_c3/templates/keys.html`

 * *Files identical despite different names*

### Comparing `oresat-c3-0.2.3/oresat_c3/templates/node_manager.html` & `oresat_c3-0.3.0/oresat_c3/templates/node_manager.html`

 * *Files 1% similar despite different names*

```diff
@@ -180,10 +180,10 @@
       updateStatus();
     }
 
     buildTable();
     updateStatus();
     const interval = setInterval(function() {
       updateStatus();
-    }, 2500);
+    }, 1000);
   </script>
 {% endblock %}
```

### Comparing `oresat-c3-0.2.3/oresat_c3/templates/state.html` & `oresat_c3-0.3.0/oresat_c3/templates/state.html`

 * *Files identical despite different names*

### Comparing `oresat-c3-0.2.3/oresat_c3.egg-info/PKG-INFO` & `oresat_c3-0.3.0/oresat_c3.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 Metadata-Version: 2.1
 Name: oresat-c3
-Version: 0.2.3
+Version: 0.3.0
 Summary: OreSat C3 OLAF app
 License: GPL-3.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Embedded Systems
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: bitstring
+Requires-Dist: cfdp-py
+Requires-Dist: dataclasses-json
 Requires-Dist: oresat-configs
-Requires-Dist: oresat-olaf>=3.3.0
+Requires-Dist: oresat-olaf>=3.5.0
 Requires-Dist: smbus2
 Requires-Dist: spacepackets
 
 # OreSat C3 Software
 
 Main application for Octavo A8 with Debian Linux version of the C3 card.
 
 The C3 card is the "flight" computer of OreSat. C3 stands for command,
-control, and commuication. It handles all commuications and controls
+control, and communication. It handles all communications and controls
 the state of the satellite.
 
 **Note:** For OreSat0, the C3 card used STM32F4 and ChibiOS, for that project
 see the [oresat-firmware] repo and the `src/f4/app_control` directory.
 The C3 card was converted to Octavo A8 card to simplify the code base
 by swapping from heavily embedded system using ChibiOS to a general
 Linux-environment using Python and make to use existing Python libraries.
 
 Like all OreSat software projects it is built using OLAF (OreSat Linux App
-Framework), which it built ontop of [CANopen for Python] project. See the
+Framework), which it built on top of [CANopen for Python] project. See the
 [oresat-olaf] repo for more info about OLAF.
 
-## Quickstart
+## Quick Start
 
-**For development**, install `oresat-configs` from the github repo at 
+**For development**, install `oresat-configs` from the GitHub repo at
 https://github.com/oresat/oresat-configs (not from PyPI). That repo may have
 changes that are not apart of the latest release yet.
 
 Install dependencies
 
 ```bash
 $ pip3 install -r requirements.txt
@@ -58,15 +60,15 @@
 
 Run the C3 app
 
 ```bash
 $ python3 -m oresat_c3
 ```
 
-Can select the CAN bus to use (`vcan0`, `can0`, etc) with the `-b BUS` arg.
+Can select the CAN bus to use (`vcan0`, `can0`, etc) with the `-b BUS` argument.
 
 Can mock hardware by using the `-m HARDWARE` flag.
 
 - The`-m all` argument can be used to mock hardware (CAN bus is always
   required).
 - The `-m opd` argument would only mock the hardware for the OPD subsystem and
   expect all other hardware
@@ -106,15 +108,15 @@
 
 To manually build the documentation:
 
 ```bash
 $ make -C docs html
 ```
 
-Open `docs/build/html/index.html` in a web broswer
+Open `docs/build/html/index.html` in a web browser
 
 ## Unit Tests
 
 This project uses python's build in `unittest` module for unit testing.
 
 To run units:
```

### Comparing `oresat-c3-0.2.3/oresat_c3.egg-info/SOURCES.txt` & `oresat_c3-0.3.0/oresat_c3.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,29 @@
+.gitignore
+.readthedocs.yaml
 LICENSE
 README.md
 pyproject.toml
+requirements.txt
+.github/workflows/pypi.yaml
+.github/workflows/tests.yaml
+docs/Makefile
+docs/conf.py
+docs/edl.rst
+docs/index.rst
+docs/make.bat
+docs/opd.rst
+docs/state.rst
+docs/static/comms_ipc.drawio
+docs/static/comms_ipc.jpg
+docs/static/custom.css
+docs/static/opd.jpg
 oresat_c3/__init__.py
 oresat_c3/__main__.py
+oresat_c3/_version.py
 oresat_c3.egg-info/PKG-INFO
 oresat_c3.egg-info/SOURCES.txt
 oresat_c3.egg-info/dependency_links.txt
 oresat_c3.egg-info/entry_points.txt
 oresat_c3.egg-info/requires.txt
 oresat_c3.egg-info/top_level.txt
 oresat_c3/drivers/__init__.py
@@ -22,11 +39,27 @@
 oresat_c3/services/edl.py
 oresat_c3/services/node_manager.py
 oresat_c3/services/radios.py
 oresat_c3/services/state.py
 oresat_c3/subsystems/__init__.py
 oresat_c3/subsystems/antennas.py
 oresat_c3/subsystems/opd.py
+oresat_c3/subsystems/rtc.py
 oresat_c3/templates/beacon.html
 oresat_c3/templates/keys.html
 oresat_c3/templates/node_manager.html
-oresat_c3/templates/state.html
+oresat_c3/templates/state.html
+scripts/edl_cmd_shell.py
+scripts/edl_file_upload.py
+scripts/edl_ping_loop.py
+tests/__init__.py
+tests/drivers/__init__.py
+tests/drivers/test_fm23cl64b.py
+tests/drivers/test_max7310.py
+tests/protocols/__init__.py
+tests/protocols/test_ax25.py
+tests/protocols/test_edl_command.py
+tests/protocols/test_edl_packet.py
+tests/services/__init__.py
+tests/services/test_state.py
+tests/subsystems/__init__.py
+tests/subsystems/test_opd.py
```

### Comparing `oresat-c3-0.2.3/pyproject.toml` & `oresat_c3-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "oresat-c3"
 description = "OreSat C3 OLAF app"
 readme = "README.md"
 requires-python = ">=3.9"
@@ -15,16 +15,18 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Embedded Systems",
 ]
 dependencies = [
     "bitstring",
+    "cfdp-py",
+    "dataclasses-json",
     "oresat-configs",
-    "oresat-olaf>=3.3.0",
+    "oresat-olaf>=3.5.0",
     "smbus2",
     "spacepackets",
 ]
 dynamic = ["version"]
 
 [project.scripts]
 oresat-c3 = "oresat_c3.__main__:main"
@@ -34,14 +36,17 @@
 
 [tool.setuptools.packages.find]
 exclude = ["docs*", "tests*", "scripts*"]
 
 [tool.setuptools.package-data]
 "*" = ["*.html"]
 
+[tool.setuptools_scm]
+write_to = "oresat_c3/_version.py"
+
 [tool.black]
 line_length = 100
 
 [tool.pylama]
 format = "pylint"
 skip = "*/.tox/*,*/.env/,*/.git/*,*/.github/*,*/build/*"
 linters = "pycodestyle,pyflakes,pylint,mccabe,mypy,radon"
@@ -57,17 +62,18 @@
 # C0413:    Imports not at top of module
 # C0206:    Consider iterating dictionaries with .items()
 # R1716:    Simplify chained comparison between the operands
 # W1514:    Using open without explicitly specifying an encoding
 # R0902:    Too many instance attributes
 # R0913:    Too many arguments
 # W0707:    Consider explicitly re-raising
-# R1732:    Consider using 'with' for resource-allocating operations 
+# R1732:    Consider using 'with' for resource-allocating operations
 # R0903:    Too few public methods
-ignore = "E402,C901,C0103,E203,R0912,R0915,R901,R901,R0914,C0413,C0206,R1716,W1514,R0902,R0913,W0707,R1732,R0903"
+# R0904:    Too many public methods
+ignore = "E402,C901,C0103,E203,R0912,R0915,R901,R901,R0914,C0413,C0206,R1716,W1514,R0902,R0913,W0707,R1732,R0903,R0904"
 max_line_length = 100
 
 [[tool.pylama.files]]
 path = "*/__init__.py"
 # W0611:    Imported but unused
 # C0114:    Missing module docstring
 ignore = "W0611,C0114"
```

