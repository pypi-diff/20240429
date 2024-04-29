# Comparing `tmp/icoc-1.8.0.tar.gz` & `tmp/icoc-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icoc-1.8.0.tar", last modified: Tue Dec 19 15:33:01 2023, max compression
+gzip compressed data, was "icoc-1.9.0.tar", last modified: Tue Jan 30 10:04:07 2024, max compression
```

## Comparing `icoc-1.8.0.tar` & `icoc-1.9.0.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.149850 icoc-1.8.0/
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.135868 icoc-1.8.0/.github/
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.137779 icoc-1.8.0/.github/workflows/
--rw-r--r--   0 rene       (501) staff       (20)     1375 2023-11-23 12:44:37.000000 icoc-1.8.0/.github/workflows/documentation.yaml
--rw-r--r--   0 rene       (501) staff       (20)      873 2023-12-13 09:49:50.000000 icoc-1.8.0/.github/workflows/tests.yaml
--rw-r--r--   0 rene       (501) staff       (20)       68 2023-11-23 12:44:37.000000 icoc-1.8.0/MANIFEST.in
--rw-r--r--   0 rene       (501) staff       (20)     3669 2023-12-19 15:33:01.149634 icoc-1.8.0/PKG-INFO
--rw-r--r--   0 rene       (501) staff       (20)     1995 2023-12-13 09:49:50.000000 icoc-1.8.0/ReadMe.md
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.148910 icoc-1.8.0/icoc.egg-info/
--rw-r--r--   0 rene       (501) staff       (20)     3669 2023-12-19 15:33:00.000000 icoc-1.8.0/icoc.egg-info/PKG-INFO
--rw-r--r--   0 rene       (501) staff       (20)     2528 2023-12-19 15:33:01.000000 icoc-1.8.0/icoc.egg-info/SOURCES.txt
--rw-r--r--   0 rene       (501) staff       (20)        1 2023-12-19 15:33:00.000000 icoc-1.8.0/icoc.egg-info/dependency_links.txt
--rw-r--r--   0 rene       (501) staff       (20)      480 2023-12-19 15:33:00.000000 icoc-1.8.0/icoc.egg-info/entry_points.txt
--rw-r--r--   0 rene       (501) staff       (20)      374 2023-12-19 15:33:00.000000 icoc-1.8.0/icoc.egg-info/requires.txt
--rw-r--r--   0 rene       (501) staff       (20)        9 2023-12-19 15:33:00.000000 icoc-1.8.0/icoc.egg-info/top_level.txt
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.138891 icoc-1.8.0/mytoolit/
--rw-r--r--   0 rene       (501) staff       (20)       79 2023-12-19 15:31:11.000000 icoc-1.8.0/mytoolit/__init__.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.140431 icoc-1.8.0/mytoolit/can/
--rw-r--r--   0 rene       (501) staff       (20)      585 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/can/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    11982 2023-12-14 15:43:44.000000 icoc-1.8.0/mytoolit/can/adc.py
--rw-r--r--   0 rene       (501) staff       (20)     5459 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/can/calibration.py
--rw-r--r--   0 rene       (501) staff       (20)    10327 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/can/command.py
--rw-r--r--   0 rene       (501) staff       (20)      233 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/can/error.py
--rw-r--r--   0 rene       (501) staff       (20)    15992 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/can/identifier.py
--rw-r--r--   0 rene       (501) staff       (20)    22170 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/can/message.py
--rw-r--r--   0 rene       (501) staff       (20)   158676 2023-12-14 15:43:44.000000 icoc-1.8.0/mytoolit/can/network.py
--rw-r--r--   0 rene       (501) staff       (20)     4515 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/can/node.py
--rw-r--r--   0 rene       (501) staff       (20)    14700 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/can/status.py
--rw-r--r--   0 rene       (501) staff       (20)    28572 2023-12-14 15:53:31.000000 icoc-1.8.0/mytoolit/can/streaming.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.140980 icoc-1.8.0/mytoolit/cmdline/
--rw-r--r--   0 rene       (501) staff       (20)      260 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/cmdline/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    10437 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/cmdline/commander.py
--rw-r--r--   0 rene       (501) staff       (20)    10449 2023-12-19 13:04:08.000000 icoc-1.8.0/mytoolit/cmdline/icon.py
--rw-r--r--   0 rene       (501) staff       (20)    11649 2023-12-14 15:43:44.000000 icoc-1.8.0/mytoolit/cmdline/parse.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.141478 icoc-1.8.0/mytoolit/config/
--rw-r--r--   0 rene       (501) staff       (20)      204 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/config/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    14437 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/config/config.py
--rwxr-xr-x   0 rene       (501) staff       (20)    13145 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/config/config.yaml
--rw-r--r--   0 rene       (501) staff       (20)     2097 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/config/user.yaml
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.141707 icoc-1.8.0/mytoolit/eeprom/
--rw-r--r--   0 rene       (501) staff       (20)      150 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/eeprom/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     3446 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/eeprom/status.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.141955 icoc-1.8.0/mytoolit/examples/
--rw-r--r--   0 rene       (501) staff       (20)      903 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/examples/read_data.py
--rw-r--r--   0 rene       (501) staff       (20)      805 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/examples/sth_name.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.142357 icoc-1.8.0/mytoolit/experiments/
--rw-r--r--   0 rene       (501) staff       (20)     2513 2023-01-17 10:19:15.000000 icoc-1.8.0/mytoolit/experiments/RF_tests.py
--rw-r--r--   0 rene       (501) staff       (20)     1327 2023-12-12 13:52:31.000000 icoc-1.8.0/mytoolit/experiments/new.py
--rw-r--r--   0 rene       (501) staff       (20)     1570 2023-01-17 10:19:15.000000 icoc-1.8.0/mytoolit/experiments/old.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.143250 icoc-1.8.0/mytoolit/measurement/
--rw-r--r--   0 rene       (501) staff       (20)      329 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/measurement/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     2199 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/measurement/acceleration.py
--rw-r--r--   0 rene       (501) staff       (20)      133 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/measurement/constants.py
--rw-r--r--   0 rene       (501) staff       (20)     5390 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/measurement/sensor.py
--rw-r--r--   0 rene       (501) staff       (20)    13485 2023-12-19 13:04:08.000000 icoc-1.8.0/mytoolit/measurement/storage.py
--rw-r--r--   0 rene       (501) staff       (20)     1685 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/measurement/units.py
--rw-r--r--   0 rene       (501) staff       (20)     1694 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/measurement/voltage.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.144612 icoc-1.8.0/mytoolit/old/
--rw-r--r--   0 rene       (501) staff       (20)    18558 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/old/MyToolItCommands.py
--rw-r--r--   0 rene       (501) staff       (20)     1927 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/old/MyToolItNetworkNumbers.py
--rw-r--r--   0 rene       (501) staff       (20)     1985 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/old/MyToolItSth.py
--rw-r--r--   0 rene       (501) staff       (20)      224 2021-05-12 07:38:00.000000 icoc-1.8.0/mytoolit/old/MyToolItStu.py
--rw-r--r--   0 rene       (501) staff       (20)     9127 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/old/Plotter.py
--rw-r--r--   0 rene       (501) staff       (20)     8642 2023-01-17 10:19:15.000000 icoc-1.8.0/mytoolit/old/SthLimits.py
--rw-r--r--   0 rene       (501) staff       (20)      151 2023-01-17 10:19:15.000000 icoc-1.8.0/mytoolit/old/StuLimits.py
--rw-r--r--   0 rene       (501) staff       (20)        0 2021-03-31 08:39:06.000000 icoc-1.8.0/mytoolit/old/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    39908 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/old/cli.py
--rw-r--r--   0 rene       (501) staff       (20)   102583 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/old/network.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.145686 icoc-1.8.0/mytoolit/old/test/
--rw-r--r--   0 rene       (501) staff       (20)    35677 2023-01-17 10:19:15.000000 icoc-1.8.0/mytoolit/old/test/HardwareSth.py
--rw-r--r--   0 rene       (501) staff       (20)   370906 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/old/test/MyToolItTestSth.py
--rw-r--r--   0 rene       (501) staff       (20)    16040 2023-01-17 10:19:15.000000 icoc-1.8.0/mytoolit/old/test/MyToolItTestSthManually.py
--rw-r--r--   0 rene       (501) staff       (20)    76128 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/old/test/MyToolItTestStu.py
--rw-r--r--   0 rene       (501) staff       (20)     6176 2023-01-17 10:19:15.000000 icoc-1.8.0/mytoolit/old/test/MyToolItTestStuManually.py
--rw-r--r--   0 rene       (501) staff       (20)        0 2021-07-12 14:02:41.000000 icoc-1.8.0/mytoolit/old/test/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      389 2021-09-29 13:59:48.000000 icoc-1.8.0/mytoolit/old/test/testSignal.py
--rw-r--r--   0 rene       (501) staff       (20)    24979 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/old/ui.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.146412 icoc-1.8.0/mytoolit/report/
--rw-r--r--   0 rene       (501) staff       (20)     7454 2021-03-31 08:39:06.000000 icoc-1.8.0/mytoolit/report/MyTooliT.pdf
--rw-r--r--   0 rene       (501) staff       (20)      149 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/report/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     6672 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/report/forms.py
--rw-r--r--   0 rene       (501) staff       (20)     2461 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/report/pdf.py
--rw-r--r--   0 rene       (501) staff       (20)     8269 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/report/report.py
--rw-r--r--   0 rene       (501) staff       (20)     5341 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/report/style.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.146772 icoc-1.8.0/mytoolit/scripts/
--rw-r--r--   0 rene       (501) staff       (20)     4965 2023-01-17 10:19:15.000000 icoc-1.8.0/mytoolit/scripts/eeprom.py
--rw-r--r--   0 rene       (501) staff       (20)      667 2023-01-17 10:19:15.000000 icoc-1.8.0/mytoolit/scripts/mac.py
--rw-r--r--   0 rene       (501) staff       (20)      650 2023-01-17 10:19:15.000000 icoc-1.8.0/mytoolit/scripts/name.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.146882 icoc-1.8.0/mytoolit/test/
--rw-r--r--   0 rene       (501) staff       (20)       13 2021-03-31 08:39:06.000000 icoc-1.8.0/mytoolit/test/__init__.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.147617 icoc-1.8.0/mytoolit/test/production/
--rw-r--r--   0 rene       (501) staff       (20)      429 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/test/production/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)    21317 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/test/production/node.py
--rw-r--r--   0 rene       (501) staff       (20)     4858 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/test/production/sensor_node.py
--rw-r--r--   0 rene       (501) staff       (20)     6387 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/test/production/smh.py
--rw-r--r--   0 rene       (501) staff       (20)    18782 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/test/production/sth.py
--rw-r--r--   0 rene       (501) staff       (20)     3646 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/test/production/stu.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.147960 icoc-1.8.0/mytoolit/test/unit/
--rw-r--r--   0 rene       (501) staff       (20)      246 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/test/unit/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     3918 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/test/unit/extended_test_result.py
--rw-r--r--   0 rene       (501) staff       (20)      722 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/test/unit/extended_test_runner.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-12-19 15:33:01.148748 icoc-1.8.0/mytoolit/utility/
--rw-r--r--   0 rene       (501) staff       (20)      233 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/utility/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1477 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/utility/data.py
--rw-r--r--   0 rene       (501) staff       (20)     1327 2023-12-13 09:49:50.000000 icoc-1.8.0/mytoolit/utility/environment.py
--rw-r--r--   0 rene       (501) staff       (20)     2718 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/utility/log.py
--rw-r--r--   0 rene       (501) staff       (20)     1344 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/utility/naming.py
--rw-r--r--   0 rene       (501) staff       (20)     3531 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/utility/open.py
--rw-r--r--   0 rene       (501) staff       (20)      919 2023-11-23 12:44:37.000000 icoc-1.8.0/mytoolit/utility/types.py
--rw-r--r--   0 rene       (501) staff       (20)     2654 2023-12-13 09:49:50.000000 icoc-1.8.0/pyproject.toml
--rw-r--r--   0 rene       (501) staff       (20)       38 2023-12-19 15:33:01.149895 icoc-1.8.0/setup.cfg
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.061481 icoc-1.9.0/
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.043475 icoc-1.9.0/.github/
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.045795 icoc-1.9.0/.github/workflows/
+-rw-r--r--   0 rene       (501) staff       (20)     1375 2023-11-23 12:44:37.000000 icoc-1.9.0/.github/workflows/documentation.yaml
+-rw-r--r--   0 rene       (501) staff       (20)      873 2023-12-13 09:49:50.000000 icoc-1.9.0/.github/workflows/tests.yaml
+-rw-r--r--   0 rene       (501) staff       (20)       68 2023-11-23 12:44:37.000000 icoc-1.9.0/MANIFEST.in
+-rw-r--r--   0 rene       (501) staff       (20)     3669 2024-01-30 10:04:07.061235 icoc-1.9.0/PKG-INFO
+-rw-r--r--   0 rene       (501) staff       (20)     1995 2023-12-13 09:49:50.000000 icoc-1.9.0/ReadMe.md
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.060512 icoc-1.9.0/icoc.egg-info/
+-rw-r--r--   0 rene       (501) staff       (20)     3669 2024-01-30 10:04:06.000000 icoc-1.9.0/icoc.egg-info/PKG-INFO
+-rw-r--r--   0 rene       (501) staff       (20)     2528 2024-01-30 10:04:07.000000 icoc-1.9.0/icoc.egg-info/SOURCES.txt
+-rw-r--r--   0 rene       (501) staff       (20)        1 2024-01-30 10:04:06.000000 icoc-1.9.0/icoc.egg-info/dependency_links.txt
+-rw-r--r--   0 rene       (501) staff       (20)      480 2024-01-30 10:04:06.000000 icoc-1.9.0/icoc.egg-info/entry_points.txt
+-rw-r--r--   0 rene       (501) staff       (20)      374 2024-01-30 10:04:06.000000 icoc-1.9.0/icoc.egg-info/requires.txt
+-rw-r--r--   0 rene       (501) staff       (20)        9 2024-01-30 10:04:06.000000 icoc-1.9.0/icoc.egg-info/top_level.txt
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.046896 icoc-1.9.0/mytoolit/
+-rw-r--r--   0 rene       (501) staff       (20)       79 2024-01-30 10:00:56.000000 icoc-1.9.0/mytoolit/__init__.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.048774 icoc-1.9.0/mytoolit/can/
+-rw-r--r--   0 rene       (501) staff       (20)      585 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/can/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)    11982 2023-12-14 15:43:44.000000 icoc-1.9.0/mytoolit/can/adc.py
+-rw-r--r--   0 rene       (501) staff       (20)     5459 2023-12-13 09:49:50.000000 icoc-1.9.0/mytoolit/can/calibration.py
+-rw-r--r--   0 rene       (501) staff       (20)    10327 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/can/command.py
+-rw-r--r--   0 rene       (501) staff       (20)      233 2023-12-13 09:49:50.000000 icoc-1.9.0/mytoolit/can/error.py
+-rw-r--r--   0 rene       (501) staff       (20)    15992 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/can/identifier.py
+-rw-r--r--   0 rene       (501) staff       (20)    22170 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/can/message.py
+-rw-r--r--   0 rene       (501) staff       (20)   160300 2024-01-30 08:15:06.000000 icoc-1.9.0/mytoolit/can/network.py
+-rw-r--r--   0 rene       (501) staff       (20)     4514 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/can/node.py
+-rw-r--r--   0 rene       (501) staff       (20)    13103 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/can/status.py
+-rw-r--r--   0 rene       (501) staff       (20)    29601 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/can/streaming.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.049239 icoc-1.9.0/mytoolit/cmdline/
+-rw-r--r--   0 rene       (501) staff       (20)      260 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/cmdline/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)    10437 2023-12-13 09:49:50.000000 icoc-1.9.0/mytoolit/cmdline/commander.py
+-rw-r--r--   0 rene       (501) staff       (20)    11650 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/cmdline/parse.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.049928 icoc-1.9.0/mytoolit/config/
+-rw-r--r--   0 rene       (501) staff       (20)      204 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/config/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)    14395 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/config/config.py
+-rwxr-xr-x   0 rene       (501) staff       (20)    13145 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/config/config.yaml
+-rw-r--r--   0 rene       (501) staff       (20)     2097 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/config/user.yaml
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.050204 icoc-1.9.0/mytoolit/eeprom/
+-rw-r--r--   0 rene       (501) staff       (20)      150 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/eeprom/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     3446 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/eeprom/status.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.050450 icoc-1.9.0/mytoolit/examples/
+-rw-r--r--   0 rene       (501) staff       (20)      903 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/examples/read_data.py
+-rw-r--r--   0 rene       (501) staff       (20)      805 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/examples/sth_name.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.050851 icoc-1.9.0/mytoolit/experiments/
+-rw-r--r--   0 rene       (501) staff       (20)     2513 2023-01-17 10:19:15.000000 icoc-1.9.0/mytoolit/experiments/RF_tests.py
+-rw-r--r--   0 rene       (501) staff       (20)      818 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/experiments/new.py
+-rw-r--r--   0 rene       (501) staff       (20)     1570 2023-01-17 10:19:15.000000 icoc-1.9.0/mytoolit/experiments/old.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.052094 icoc-1.9.0/mytoolit/measurement/
+-rw-r--r--   0 rene       (501) staff       (20)      329 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/measurement/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     2199 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/measurement/acceleration.py
+-rw-r--r--   0 rene       (501) staff       (20)      133 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/measurement/constants.py
+-rw-r--r--   0 rene       (501) staff       (20)     5302 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/measurement/sensor.py
+-rw-r--r--   0 rene       (501) staff       (20)    13570 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/measurement/storage.py
+-rw-r--r--   0 rene       (501) staff       (20)     1685 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/measurement/units.py
+-rw-r--r--   0 rene       (501) staff       (20)     1694 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/measurement/voltage.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.054118 icoc-1.9.0/mytoolit/old/
+-rw-r--r--   0 rene       (501) staff       (20)    18558 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/old/MyToolItCommands.py
+-rw-r--r--   0 rene       (501) staff       (20)     1927 2023-12-13 09:49:50.000000 icoc-1.9.0/mytoolit/old/MyToolItNetworkNumbers.py
+-rw-r--r--   0 rene       (501) staff       (20)     1985 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/old/MyToolItSth.py
+-rw-r--r--   0 rene       (501) staff       (20)      224 2021-05-12 07:38:00.000000 icoc-1.9.0/mytoolit/old/MyToolItStu.py
+-rw-r--r--   0 rene       (501) staff       (20)     9127 2023-12-13 09:49:50.000000 icoc-1.9.0/mytoolit/old/Plotter.py
+-rw-r--r--   0 rene       (501) staff       (20)     8642 2023-01-17 10:19:15.000000 icoc-1.9.0/mytoolit/old/SthLimits.py
+-rw-r--r--   0 rene       (501) staff       (20)      151 2023-01-17 10:19:15.000000 icoc-1.9.0/mytoolit/old/StuLimits.py
+-rw-r--r--   0 rene       (501) staff       (20)        0 2021-03-31 08:39:06.000000 icoc-1.9.0/mytoolit/old/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)    39908 2023-12-13 09:49:50.000000 icoc-1.9.0/mytoolit/old/cli.py
+-rw-r--r--   0 rene       (501) staff       (20)   102507 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/old/network.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.056497 icoc-1.9.0/mytoolit/old/test/
+-rw-r--r--   0 rene       (501) staff       (20)    35677 2023-01-17 10:19:15.000000 icoc-1.9.0/mytoolit/old/test/HardwareSth.py
+-rw-r--r--   0 rene       (501) staff       (20)   370906 2023-12-13 09:49:50.000000 icoc-1.9.0/mytoolit/old/test/MyToolItTestSth.py
+-rw-r--r--   0 rene       (501) staff       (20)    16040 2023-01-17 10:19:15.000000 icoc-1.9.0/mytoolit/old/test/MyToolItTestSthManually.py
+-rw-r--r--   0 rene       (501) staff       (20)    76128 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/old/test/MyToolItTestStu.py
+-rw-r--r--   0 rene       (501) staff       (20)     6176 2023-01-17 10:19:15.000000 icoc-1.9.0/mytoolit/old/test/MyToolItTestStuManually.py
+-rw-r--r--   0 rene       (501) staff       (20)        0 2021-07-12 14:02:41.000000 icoc-1.9.0/mytoolit/old/test/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)      389 2021-09-29 13:59:48.000000 icoc-1.9.0/mytoolit/old/test/testSignal.py
+-rw-r--r--   0 rene       (501) staff       (20)    24979 2023-12-13 09:49:50.000000 icoc-1.9.0/mytoolit/old/ui.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.057361 icoc-1.9.0/mytoolit/report/
+-rw-r--r--   0 rene       (501) staff       (20)     7454 2021-03-31 08:39:06.000000 icoc-1.9.0/mytoolit/report/MyTooliT.pdf
+-rw-r--r--   0 rene       (501) staff       (20)      149 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/report/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     6672 2023-12-13 09:49:50.000000 icoc-1.9.0/mytoolit/report/forms.py
+-rw-r--r--   0 rene       (501) staff       (20)     2558 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/report/pdf.py
+-rw-r--r--   0 rene       (501) staff       (20)     8525 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/report/report.py
+-rw-r--r--   0 rene       (501) staff       (20)     5341 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/report/style.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.057872 icoc-1.9.0/mytoolit/scripts/
+-rw-r--r--   0 rene       (501) staff       (20)     4965 2023-01-17 10:19:15.000000 icoc-1.9.0/mytoolit/scripts/eeprom.py
+-rw-r--r--   0 rene       (501) staff       (20)    10619 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/scripts/icon.py
+-rw-r--r--   0 rene       (501) staff       (20)      667 2023-01-17 10:19:15.000000 icoc-1.9.0/mytoolit/scripts/mac.py
+-rw-r--r--   0 rene       (501) staff       (20)      650 2023-01-17 10:19:15.000000 icoc-1.9.0/mytoolit/scripts/name.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.057985 icoc-1.9.0/mytoolit/test/
+-rw-r--r--   0 rene       (501) staff       (20)       13 2021-03-31 08:39:06.000000 icoc-1.9.0/mytoolit/test/__init__.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.058728 icoc-1.9.0/mytoolit/test/production/
+-rw-r--r--   0 rene       (501) staff       (20)      429 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/test/production/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)    21351 2024-01-30 07:44:37.000000 icoc-1.9.0/mytoolit/test/production/node.py
+-rw-r--r--   0 rene       (501) staff       (20)     5616 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/test/production/sensor_node.py
+-rw-r--r--   0 rene       (501) staff       (20)     6097 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/test/production/smh.py
+-rw-r--r--   0 rene       (501) staff       (20)    18653 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/test/production/sth.py
+-rw-r--r--   0 rene       (501) staff       (20)     3691 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/test/production/stu.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.059073 icoc-1.9.0/mytoolit/test/unit/
+-rw-r--r--   0 rene       (501) staff       (20)      246 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/test/unit/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     3918 2023-12-13 09:49:50.000000 icoc-1.9.0/mytoolit/test/unit/extended_test_result.py
+-rw-r--r--   0 rene       (501) staff       (20)      722 2023-12-13 09:49:50.000000 icoc-1.9.0/mytoolit/test/unit/extended_test_runner.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2024-01-30 10:04:07.060306 icoc-1.9.0/mytoolit/utility/
+-rw-r--r--   0 rene       (501) staff       (20)      233 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/utility/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     1477 2023-12-13 09:49:50.000000 icoc-1.9.0/mytoolit/utility/data.py
+-rw-r--r--   0 rene       (501) staff       (20)     1327 2023-12-13 09:49:50.000000 icoc-1.9.0/mytoolit/utility/environment.py
+-rw-r--r--   0 rene       (501) staff       (20)     2718 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/utility/log.py
+-rw-r--r--   0 rene       (501) staff       (20)     1344 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/utility/naming.py
+-rw-r--r--   0 rene       (501) staff       (20)     3581 2024-01-29 16:12:26.000000 icoc-1.9.0/mytoolit/utility/open.py
+-rw-r--r--   0 rene       (501) staff       (20)      919 2023-11-23 12:44:37.000000 icoc-1.9.0/mytoolit/utility/types.py
+-rw-r--r--   0 rene       (501) staff       (20)     2654 2024-01-29 16:12:26.000000 icoc-1.9.0/pyproject.toml
+-rw-r--r--   0 rene       (501) staff       (20)       38 2024-01-30 10:04:07.061529 icoc-1.9.0/setup.cfg
```

### Comparing `icoc-1.8.0/.github/workflows/documentation.yaml` & `icoc-1.9.0/.github/workflows/documentation.yaml`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/.github/workflows/tests.yaml` & `icoc-1.9.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/PKG-INFO` & `icoc-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icoc
-Version: 1.8.0
+Version: 1.9.0
 Summary: Control and test software for sensory tool holders (STH), sensor milling heads (SMH) and stationary transceiver units (STU)
 Author-email: Clemens Burgstaller <burgstaller@ift.at>, René Schwaiger <rene.schwaiger@ift.at>
 Project-URL: Documentation, https://mytoolit.github.io/ICOc/
 Project-URL: Source, https://github.com/mytoolit/ICOc/
 Keywords: smart-tool,smh,stu,sth,tool-holder
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Other/Proprietary License
```

### Comparing `icoc-1.8.0/ReadMe.md` & `icoc-1.9.0/ReadMe.md`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/icoc.egg-info/PKG-INFO` & `icoc-1.9.0/icoc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icoc
-Version: 1.8.0
+Version: 1.9.0
 Summary: Control and test software for sensory tool holders (STH), sensor milling heads (SMH) and stationary transceiver units (STU)
 Author-email: Clemens Burgstaller <burgstaller@ift.at>, René Schwaiger <rene.schwaiger@ift.at>
 Project-URL: Documentation, https://mytoolit.github.io/ICOc/
 Project-URL: Source, https://github.com/mytoolit/ICOc/
 Keywords: smart-tool,smh,stu,sth,tool-holder
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: Other/Proprietary License
```

### Comparing `icoc-1.8.0/icoc.egg-info/SOURCES.txt` & `icoc-1.9.0/icoc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 mytoolit/can/message.py
 mytoolit/can/network.py
 mytoolit/can/node.py
 mytoolit/can/status.py
 mytoolit/can/streaming.py
 mytoolit/cmdline/__init__.py
 mytoolit/cmdline/commander.py
-mytoolit/cmdline/icon.py
 mytoolit/cmdline/parse.py
 mytoolit/config/__init__.py
 mytoolit/config/config.py
 mytoolit/config/config.yaml
 mytoolit/config/user.yaml
 mytoolit/eeprom/__init__.py
 mytoolit/eeprom/status.py
@@ -64,14 +63,15 @@
 mytoolit/report/MyTooliT.pdf
 mytoolit/report/__init__.py
 mytoolit/report/forms.py
 mytoolit/report/pdf.py
 mytoolit/report/report.py
 mytoolit/report/style.py
 mytoolit/scripts/eeprom.py
+mytoolit/scripts/icon.py
 mytoolit/scripts/mac.py
 mytoolit/scripts/name.py
 mytoolit/test/__init__.py
 mytoolit/test/production/__init__.py
 mytoolit/test/production/node.py
 mytoolit/test/production/sensor_node.py
 mytoolit/test/production/smh.py
```

### Comparing `icoc-1.8.0/mytoolit/can/__init__.py` & `icoc-1.9.0/mytoolit/can/__init__.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/can/adc.py` & `icoc-1.9.0/mytoolit/can/adc.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/can/calibration.py` & `icoc-1.9.0/mytoolit/can/calibration.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/can/command.py` & `icoc-1.9.0/mytoolit/can/command.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/can/identifier.py` & `icoc-1.9.0/mytoolit/can/identifier.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/can/message.py` & `icoc-1.9.0/mytoolit/can/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -516,17 +516,17 @@
 
         explanation = (
             f"{identifier} ({data_explanation})"
             if data_explanation
             else repr(identifier)
         )
 
-        data_representation = " ".join([
-            hex(self.data[byte]) for byte in range(len(self.data))
-        ])
+        data_representation = " ".join(
+            [hex(self.data[byte]) for byte in range(len(self.data))]
+        )
         bit_values = [
             f"0b{identifier.value:029b}",
             str(len(self.data)),
             data_representation,
         ]
         # Filter empty string, since otherwise there might be an additional
         # space at the end of the representation for empty data
```

### Comparing `icoc-1.8.0/mytoolit/can/network.py` & `icoc-1.9.0/mytoolit/can/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Support for working with the ICOtronic system
 
 To communicate with the ICOtronic system, create a new `Network` object and
 use its various coroutines. Unfortunately we do not offer an official API
 documentation yet. For now we recommend you take a look at the
 doctests of the `Network` class or the code for the `icon` command line tool
-(mytoolit.cmdline.icon).
+(mytoolit.scripts.icon).
 """
 
 # pylint: disable=too-many-lines
 
 # -- Imports ------------------------------------------------------------------
 
 from __future__ import annotations
@@ -34,18 +34,19 @@
 from mytoolit.can.adc import ADCConfiguration
 from mytoolit.can.calibration import CalibrationMeasurementFormat
 from mytoolit.can.error import UnsupportedFeatureException
 from mytoolit.can.message import Message
 from mytoolit.can.node import Node
 from mytoolit.can.streaming import (
     AsyncStreamBuffer,
+    StreamingConfiguration,
     StreamingData,
-    TimestampedValue,
     StreamingFormat,
     StreamingFormatVoltage,
+    TimestampedValue,
 )
 from mytoolit.can.status import State
 from mytoolit.measurement import convert_raw_to_supply_voltage
 from mytoolit.measurement.sensor import SensorConfig
 from mytoolit.utility import convert_bytes_to_text
 from mytoolit.utility.log import get_log_file_handler
 
@@ -264,53 +265,58 @@
         getLogger().error("Error while monitoring CAN bus data: %s", exc)
 
 
 class DataStreamContextManager:
     """Open and close a data stream from a sensor device"""
 
     def __init__(
-        self, network: Network, first: bool, second: bool, third: bool
+        self,
+        network: Network,
+        configuration: StreamingConfiguration,
+        timeout: float,
     ) -> None:
         """Create a new stream context manager for the given Network
 
         Parameters
         ----------
 
         network:
             The CAN network class for which this context manager handles
             sensor device stream data
 
-        first:
-            Specifies if the data of the first measurement channel should
-            be streamed or not
-
-        second:
-            Specifies if the data of the second measurement channel should
-            be streamed or not
-
-        third:
-            Specifies if the data of the third measurement channel should
-            be streamed or not
+        configuration:
+            A streaming configuration that specifies which of the three
+            streaming channels should be enabled or not
+
+        timeout
+            The amount of seconds between two consecutive messages, before
+            a TimeoutError will be raised
 
         """
 
         self.network = network
-        self.reader = AsyncStreamBuffer(first, second, third)
+        self.reader = AsyncStreamBuffer(configuration, timeout)
 
     async def __aenter__(self) -> AsyncStreamBuffer:
         """Open the stream of measurement data
 
         Returns
         -------
 
         The stream buffer for the measurement stream
 
         """
 
-        return await self.open()
+        reader = self.reader
+        configuration = reader.configuration
+        await self.network.start_streaming_data(
+            configuration.first, configuration.second, configuration.third
+        )
+        self.network.notifier.add_listener(reader)
+        return reader
 
     async def __aexit__(
         self,
         exception_type: Optional[Type[BaseException]],
         exception_value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None:
@@ -326,39 +332,35 @@
             The value of the exception in case of an exception
 
         traceback:
             The traceback in case of an exception
 
         """
 
-        await self.close()
-
-    async def open(self) -> AsyncStreamBuffer:
-        """Open the stream of measurement data
-
-        Returns
-        -------
-
-        The stream buffer for the measurement stream
-
-        """
-
-        reader = self.reader
-        await self.network.start_streaming_data(
-            reader.first, reader.second, reader.third
-        )
-        self.network.notifier.add_listener(reader)
-        return reader
-
-    async def close(self) -> None:
-        """Clean up the resources used by the stream"""
+        logger = getLogger(__name__)
 
         self.reader.stop()
         self.network.notifier.remove_listener(self.reader)
-        await self.network.stop_streaming_data()
+        if exception_type:
+            # If there was an error while streaming data, then stoping the
+            # stream will usually also fail. Because of this we only try once
+            # and ignore any errors.
+            #
+            # If we did not do that, then the user of the API would be notified
+            # about the error to disable the stream, but not about the original
+            # error. It would also take considerably more time until the
+            # computer would report an error, since the code would usually try
+            # to stop the stream (and fail) multiple times beforehand.
+            logger.info("Stopping stream after error (%s)", exception_type)
+            await self.network.stop_streaming_data(
+                retries=1, ignore_errors=True
+            )
+        else:
+            logger.info("Stopping stream")
+            await self.network.stop_streaming_data()
 
 
 # pylint: disable=too-many-public-methods
 
 
 class Network:
     """Basic class to communicate with STU and STH devices"""
@@ -495,20 +497,23 @@
                 self.bus, listeners=[Logger()], loop=get_running_loop()
             )
 
         assert self._notifier is not None
 
         return self._notifier
 
+    # pylint: disable=too-many-arguments
+
     async def _request(
         self,
         message: Message,
         description: str,
         response_data: Union[bytearray, List[Union[int, None]], None] = None,
         minimum_timeout: float = 0,
+        retries: int = 10,
     ) -> CANMessage:
         """Send a request message and wait for the response
 
         Parameters
         ----------
 
         message:
@@ -520,32 +525,36 @@
         response_data:
            Specifies the expected data in the acknowledgment message
 
         minimum_timeout:
            Minimum time before attempting additional connection attempt
            in seconds
 
+        retries:
+           The number of times the message is sent again, if no response was
+           sent back in a certain amount of time
+
         Returns
         -------
 
         The response message for the given request
 
-        Throws
+        Raises
         ------
 
         NoResponseError:
-            If the receiver did not respond to the message after a certain
-            amount of time (1s)
+            If the receiver did not respond to the message after retries
+            amount of messages sent
 
         ErrorResponseError:
             If the receiver answered with an error message
 
         """
 
-        for attempt in range(10):
+        for attempt in range(retries):
             listener = ResponseListener(message, response_data)
             self.notifier.add_listener(listener)
             getLogger("network.can").debug("%s", message)
             self.bus.send(message.to_python_can())
 
             try:
                 # We increase the timeout after the first and second try.
@@ -577,16 +586,14 @@
                     f"Response Message: {Message(response.message)}"
                 )
 
             return response.message
 
         raise NoResponseError(f"Unable to {description}")
 
-    # pylint: disable=too-many-arguments
-
     async def _request_bluetooth(
         self,
         node: Union[str, Node],
         subcommand: int,
         description: str,
         device_number: Optional[int] = None,
         data: Optional[List[int]] = None,
@@ -1766,17 +1773,17 @@
         timeout_in_s = 20
         end_time = time() + timeout_in_s
 
         sensor_device = None
         sensor_devices: List[STHDeviceInfo] = []
         while sensor_device is None:
             if time() > end_time:
-                sensor_devices_representation = "\n".join([
-                    repr(device) for device in sensor_devices
-                ])
+                sensor_devices_representation = "\n".join(
+                    [repr(device) for device in sensor_devices]
+                )
                 device_info = (
                     "Found the following sensor devices:\n"
                     f"{sensor_devices_representation}"
                     if len(sensor_devices) > 0
                     else "No sensor devices found"
                 )
 
@@ -1919,17 +1926,17 @@
         to filter CAN messages that contain the expected streaming data
 
         """
 
         if not (first or second or third):
             raise ValueError("Please enable at least one measurement channel")
 
-        active_channels = len([
-            channel for channel in (first, second, third) if channel
-        ])
+        active_channels = len(
+            [channel for channel in (first, second, third) if channel]
+        )
 
         streaming_format = StreamingFormat(
             first=first,
             second=second,
             third=third,
             streaming=True,
             sets=3 if active_channels <= 1 else 1,
@@ -1961,34 +1968,59 @@
             message,
             description=(
                 f"enable streaming of {channels_text} measurement "
                 f"channel of “{node}”"
             ),
         )
 
-    async def stop_streaming_data(self) -> None:
-        """Stop streaming data"""
+    async def stop_streaming_data(
+        self, retries: int = 10, ignore_errors=False
+    ) -> None:
+        """Stop streaming data
+
+        Parameters
+        ----------
+
+        retries:
+            The number of times the message is sent again, if no response was
+            sent back in a certain amount of time
+
+        ignore_errors:
+            Specifies, if this coroutine should ignore, if there were any
+            problems while stopping the stream.
+
+        """
 
         streaming_format = StreamingFormat(streaming=True, sets=0)
         node = "STH 1"
         message = Message(
             block="Streaming",
             block_command="Data",
             sender=self.sender,
             receiver=node,
             request=True,
             data=[streaming_format.value],
         )
 
-        await self._request(
-            message, description=f"disable data streaming of “{node}”"
-        )
+        try:
+            await self._request(
+                message,
+                description=f"disable data streaming of “{node}”",
+                retries=retries,
+            )
+        except (NoResponseError, ErrorResponseError) as error:
+            if not ignore_errors:
+                raise error
 
     def open_data_stream(
-        self, first: bool = False, second: bool = False, third: bool = False
+        self,
+        first: bool = False,
+        second: bool = False,
+        third: bool = False,
+        timeout: float = 5,
     ) -> DataStreamContextManager:
         """Open measurement data stream
 
         Parameters
         ----------
 
         first:
@@ -1999,20 +2031,23 @@
             Specifies if the data of the second measurement channel should
             be streamed or not
 
         third:
             Specifies if the data of the third measurement channel should
             be streamed or not
 
+        timeout:
+            The amount of seconds between two consecutive messages, before
+            a TimeoutError will be raised
+
         Returns
         -------
 
         A context manager object for managing stream data
 
-
         Examples
         --------
 
         >>> from asyncio import run
 
         >>> async def read_streaming_data():
         ...     async with Network() as network:
@@ -2033,15 +2068,17 @@
         >>> len(stream_data.second)
         0
         >>> len(stream_data.third)
         3
 
         """
 
-        return DataStreamContextManager(self, first, second, third)
+        return DataStreamContextManager(
+            self, StreamingConfiguration(first, second, third), timeout
+        )
 
     async def read_streaming_data_seconds(
         self,
         seconds: float,
         first: bool = True,
         second: bool = False,
         third: bool = False,
```

### Comparing `icoc-1.8.0/mytoolit/can/node.py` & `icoc-1.9.0/mytoolit/can/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,17 +124,18 @@
         SPU 1
 
         >>> Node(18)
         STU 2
 
         """
 
-        if self.value == 0 or self.value == 31:
-            return "Broadcast With{} Acknowledgment".format(
-                "" if self.value == 0 else "out"
+        if self.value in (0, 31):
+            return (
+                "Broadcast "
+                f"With{'' if self.value == 0 else 'out'} Acknowledgment"
             )
         if self.is_sth():
             return f"STH {self.value}"
 
         if 15 <= self.value <= 16:
             return f"SPU {self.value - 14}"
```

### Comparing `icoc-1.8.0/mytoolit/can/status.py` & `icoc-1.9.0/mytoolit/can/status.py`

 * *Files 16% similar despite different names*

```diff
@@ -248,15 +248,15 @@
         Set State, Location: Bootloader, State: Startup
         >>> State(0b0_1_11_1_001)
         Get State, Location: Reserved, State: Error
 
         """
 
         attributes = [
-            "{} State".format("Set" if self.is_set() else "Get"),
+            f"{'Set' if self.is_set() else 'Get'} State",
             f"Location: {self.location_name()}",
             f"State: {self.state_name()}",
         ]
 
         return ", ".join(attributes)
 
 
@@ -355,61 +355,19 @@
 
         state = (self.value >> 1) & 0b111
         # pylint: disable=unsubscriptable-object
         return State.network_states.inverse[state]
 
 
 class NodeStatusSTH(NodeStatus):
-    def __init__(self, value: Union[List[int], int]) -> None:
-        """Initialize the node status word using the given arguments
-
-        Parameters
-        ----------
-
-        value:
-            A 32 bit integer or list of bytes that specifies the value of the
-            node status word
-
-        """
-
-        super().__init__(value)
-
-    def __repr__(self) -> str:
-        """Retrieve the textual representation of the node status word
-
-        Returns
-        -------
-
-        A string that describes the attributes of the node status word
-
-        Examples
-        --------
-
-        >>> NodeStatusSTH(0b0100)
-        State: Standby, No Error
-
-        """
-
-        return super().__repr__()
+    """Wrapper for the node status word of the STH"""
 
 
 class NodeStatusSTU(NodeStatus):
-    def __init__(self, value: Union[List[int], int]) -> None:
-        """Initialize the node status word using the given arguments
-
-        Parameters
-        ----------
-
-        value:
-            A 32 bit integer or list of bytes that specifies the value of the
-            node status word
-
-        """
-
-        super().__init__(value)
+    """Wrapper for the node status word of the STU"""
 
     def __repr__(self) -> str:
         """Retrieve the textual representation of the node status word
 
         Returns
         -------
 
@@ -426,28 +384,28 @@
 
         radio_port_enabled = self.value >> 4 & 1
         can_port_enabled = self.value >> 5 & 1
         bluetooth_connected = self.value >> 6 & 1
 
         attributes = [
             super().__repr__(),
-            "Radio Port {}".format(
-                "Enabled" if radio_port_enabled else "Disabled"
-            ),
-            "CAN Port {}".format(
-                "Enabled" if can_port_enabled else "Disabled"
-            ),
-            "Bluetooth {}".format(
-                "Connected" if bluetooth_connected else "Disconnected"
+            f"Radio Port {'Enabled' if radio_port_enabled else 'Disabled'}",
+            f"CAN Port {'Enabled' if can_port_enabled else 'Disabled'}",
+            (
+                "Bluetooth "
+                f"{'Connected' if bluetooth_connected else 'Disconnected'}"
             ),
         ]
 
         return ", ".join(attributes)
 
 
+# pylint: disable=too-few-public-methods
+
+
 class ErrorStatus:
     """Wrapper class for the error status word
 
     Please do not use this class directly, but instead use one of the
     two specific error status classes for the STH and STU.
     """
 
@@ -485,29 +443,19 @@
         True
 
         """
 
         return bool(self.value & 1)
 
 
-class ErrorStatusSTH(ErrorStatus):
-    """Wrapper class for error status word 1 of the STH"""
-
-    def __init__(self, value: Union[List[int], int]) -> None:
-        """Initialize the error status word using the given arguments
+# pylint: enable=too-few-public-methods
 
-        Parameters
-        ----------
-
-        value:
-            A 32 bit integer or list of bytes that specifies the value of the
-            error status word
 
-        """
-        super().__init__(value)
+class ErrorStatusSTH(ErrorStatus):
+    """Wrapper class for error status word 1 of the STH"""
 
     def __repr__(self) -> str:
         """Retrieve the textual representation of the error status word
 
         Returns
         -------
 
@@ -564,27 +512,14 @@
 
         return bool((self.value >> 1) & 1)
 
 
 class ErrorStatusSTU(ErrorStatus):
     """Wrapper class for error status word 1 of the STH"""
 
-    def __init__(self, value: Union[List[int], int]) -> None:
-        """Initialize the error status word using the given arguments
-
-        Parameters
-        ----------
-
-        value:
-            A 32 bit integer or list of bytes that specifies the value of the
-            error status word
-
-        """
-        super().__init__(value)
-
     def __repr__(self) -> str:
         """Retrieve the textual representation of the error status word
 
         Returns
         -------
 
         A string that describes the attributes of the error status word
```

### Comparing `icoc-1.8.0/mytoolit/can/streaming.py` & `icoc-1.9.0/mytoolit/can/streaming.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,123 +1,161 @@
 """Support for streaming (measurement) data in the ICOtronic system"""
 
 # -- Imports ------------------------------------------------------------------
 
 from __future__ import annotations
 
-from asyncio import Queue
+from asyncio import Queue, wait_for
 from numbers import Real
 from typing import (
     AsyncIterator,
-    Awaitable,
     Callable,
     Dict,
     List,
+    NamedTuple,
     Optional,
     Tuple,
     Union,
 )
 
 from can import Listener, Message
 from pint import Quantity
 
 from mytoolit.can.identifier import Identifier
 
 # -- Classes ------------------------------------------------------------------
 
 
+class StreamingTimeoutError(Exception):
+    """Raised if no streaming data was received for a certain amount of time"""
+
+
+class StreamingConfiguration(NamedTuple):
+    """Streaming configuration"""
+
+    first: bool = True  # Specifies if the first channel is enabled or not
+    second: bool = False  # Specifies if the second channel is enabled or not
+    third: bool = False  # Specifies if the third channel is enabled or not
+
+    def __repr__(self) -> str:
+        """Return the string representation of the streaming configuration
+
+        Examples
+        --------
+
+        >>> StreamingConfiguration()
+        Channel 1 enabled, Channel 2 disabled, Channel 3 disabled
+
+        >>> StreamingConfiguration(first=False, second=True, third=False)
+        Channel 1 disabled, Channel 2 enabled, Channel 3 disabled
+
+        >>> StreamingConfiguration(first=True, second=True, third=True)
+        Channel 1 enabled, Channel 2 enabled, Channel 3 enabled
+
+        """
+
+        return ", ".join([
+            f"Channel {name} {'en' if status else 'dis'}abled"
+            for name, status in enumerate(
+                (self.first, self.second, self.third), start=1
+            )
+        ])
+
+
 class AsyncStreamBuffer(Listener):
     """Buffer for streaming data"""
 
-    def __init__(self, first: bool, second: bool, third: bool) -> None:
+    def __init__(
+        self, configuration: StreamingConfiguration, timeout: float
+    ) -> None:
         """Initialize object using the given arguments
 
         Parameters
         ----------
 
-        first:
-            Specifies if the data of the first measurement channel will be
-            collected or not
-
-        second:
-            Specifies if the data of the second measurement channel will be
-            collected or not
-
-        third:
-            Specifies if the data of the third measurement channel will be
-            collected or not
+        configuration:
+            A streaming configuration that specifies which of the three
+            streaming channels should be enabled or not
+
+        timeout:
+            The amount of seconds between two consecutive messages, before
+            a TimeoutError will be raised
 
         """
 
         # Expected identifier of received streaming messages
         self.identifier = Identifier(
             block="Streaming",
             block_command="Data",
             sender="STH 1",
             receiver="SPU 1",
             request=False,
         )
-        self.first = first
-        self.second = second
-        self.third = third
+        self.configuration = configuration
         self.queue: Queue[StreamingData] = Queue()
+        self.timeout = timeout
 
     def __aiter__(self) -> AsyncIterator[StreamingData]:
         """Retrieve iterator for collected data
 
         Returns
         -------
 
         An iterator over the received streaming data
 
         """
 
         return self
 
-    def __anext__(self) -> Awaitable[StreamingData]:
+    async def __anext__(self) -> StreamingData:
         """Retrieve next stream data object in collected data
 
         Returns
         -------
 
         Retrieved streaming data
 
         """
 
-        return self.queue.get()
+        try:
+            return await wait_for(self.queue.get(), self.timeout)
+        except TimeoutError as error:
+            raise StreamingTimeoutError(
+                f"No data received for at least {self.timeout} seconds"
+            ) from error
 
-    def on_message_received(self, message: Message) -> None:
+    def on_message_received(self, msg: Message) -> None:
         """Handle received messages
 
         Parameters
         ----------
 
-        message:
+        msg:
             The received CAN message
 
         """
 
-        if message.arbitration_id != self.identifier.value:
+        if msg.arbitration_id != self.identifier.value:
             return
 
-        data = message.data
-        timestamp = message.timestamp
+        data = msg.data
+        timestamp = msg.timestamp
         raw_values = [
             TimestampedValue(
                 value=int.from_bytes(word, byteorder="little"),
                 timestamp=timestamp,
                 counter=data[1],
             )
             for word in (data[2:4], data[4:6], data[6:8])
         ]
 
         streaming_data = StreamingData()
-        first = self.first
-        second = self.second
-        third = self.third
+        first = self.configuration.first
+        second = self.configuration.second
+        third = self.configuration.third
 
         if first and second and third:
             streaming_data.first.append(raw_values[0])
             streaming_data.second.append(raw_values[1])
             streaming_data.third.append(raw_values[2])
         elif first and second:
             streaming_data.first.append(raw_values[0])
@@ -133,24 +171,39 @@
         elif second:
             streaming_data.second.extend(raw_values)
         else:
             streaming_data.third.extend(raw_values)
 
         self.queue.put_nowait(streaming_data)
 
+    def on_error(self, exc: Exception) -> None:
+        """This method is called to handle any exception in the receive thread.
+
+        Parameters
+        ----------
+
+        exc:
+            The exception causing the thread to stop
+
+        """
+
+        raise NotImplementedError()
+
 
 class StreamingFormat:
     """Support for specifying the data streaming format
 
     See also: https://mytoolit.github.io/Documentation/#block-streaming
     """
 
     # Possible number of data sets
     data_set = [0, 1, 3, 6, 10, 15, 20, 30]
 
+    # pylint: disable=too-many-arguments
+
     def __init__(
         self,
         *value,
         streaming: Optional[bool] = None,
         width: Optional[int] = 2,
         first: Optional[bool] = None,
         second: Optional[bool] = None,
@@ -255,14 +308,16 @@
             cls = type(self)
 
             if sets not in cls.data_set:
                 raise ValueError(f"Unsupported number of data sets: {sets}")
 
             set_part(0, 3, cls.data_set.index(sets))
 
+    # pylint: enable=too-many-arguments
+
     def __repr__(self) -> str:
         """Retrieve the textual representation of the streaming format
 
         Returns
         -------
 
         A string that describes the streaming format
@@ -283,17 +338,15 @@
 
         streaming = self.value >> 7
 
         data_sets = self.data_sets()
         data_set_explanation = (
             "Stop Stream"
             if data_sets == 0
-            else "{} Data Set{}".format(
-                data_sets, "" if data_sets == 1 else "s"
-            )
+            else f"{data_sets} Data Set{'' if data_sets == 1 else 's'}"
         )
 
         parts = [
             "Streaming" if streaming else "Single Request",
             f"{self.data_bytes()} Bytes",
             f"{data_set_explanation}",
         ]
@@ -400,37 +453,14 @@
 
         super().__init__(
             *arguments,
             **keyword_arguments,
             value_explanations=("Voltage 1", "Voltage 2", "Voltage 3"),
         )
 
-    def __repr__(self) -> str:
-        """Retrieve the textual representation of the voltage streaming format
-
-        Returns
-        -------
-
-        A string that describes the voltage streaming format
-
-        Examples
-        --------
-
-        >>> StreamingFormatVoltage(streaming=True, width=2, second=True,
-        ...                        sets=10)
-        Streaming, 2 Bytes, 10 Data Sets, Read Voltage 2
-
-        >>> StreamingFormatVoltage(streaming=False, width=3, first=False,
-        ...                        second=True, third=True, sets=3)
-        Single Request, 3 Bytes, 3 Data Sets, Read Voltage 2, Read Voltage 3
-
-        """
-
-        return super().__repr__()
-
 
 class TimestampedValue:
     """Store a single (streaming) value and its timestamp"""
 
     def __init__(
         self,
         timestamp: float,
```

### Comparing `icoc-1.8.0/mytoolit/cmdline/commander.py` & `icoc-1.9.0/mytoolit/cmdline/commander.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/cmdline/icon.py` & `icoc-1.9.0/mytoolit/scripts/icon.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from can.interfaces.pcan import PcanError
 from tqdm import tqdm
 
 from mytoolit.can import Network
 from mytoolit.can.adc import ADCConfiguration
 from mytoolit.can.network import STHDeviceInfo, NetworkError
+from mytoolit.can.streaming import StreamingTimeoutError
 from mytoolit.cmdline.parse import parse_arguments
 from mytoolit.config import ConfigurationUtility, settings
 from mytoolit.measurement import convert_raw_to_g, Storage
 
 
 # -- Functions ----------------------------------------------------------------
 
@@ -229,14 +230,15 @@
                         storage.add_streaming_data(data)
                         progress.update(3)  # 3 values per message
 
                         if time() - start_time >= measurement_time_s:
                             break
             except KeyboardInterrupt:
                 pass
+
             finally:
                 storage.add_acceleration_meta(
                     "Sensor_Range", f"± {sensor_range / 2} g₀"
                 )
 
                 progress.close()
                 print(f"Data Loss: {storage.dataloss()}")
@@ -324,15 +326,17 @@
             "rename": rename,
             "stu": stu,
         }
 
         try:
             run(command_to_coroutine[arguments.subcommand](arguments))
         except NetworkError as error:
-            print(error)
+            print(error, file=stderr)
+        except StreamingTimeoutError as error:
+            print(f"Quitting Measurement: {error}")
         except KeyboardInterrupt:
             pass
 
 
 # -- Main ---------------------------------------------------------------------
 
 if __name__ == "__main__":
```

### Comparing `icoc-1.8.0/mytoolit/cmdline/parse.py` & `icoc-1.9.0/mytoolit/cmdline/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Command Line Parsing support"""
 
 # -- Imports ------------------------------------------------------------------
 
 from argparse import ArgumentParser, ArgumentTypeError, Namespace
 from math import inf
-from re import compile
+from re import compile as re_compile
 
 from netaddr import AddrFormatError, EUI
 
 from mytoolit.can.adc import ADCConfiguration
 
 # -- Functions ----------------------------------------------------------------
 
@@ -37,15 +37,15 @@
     >>> base64_mac_address("CGvXAd")
     Traceback (most recent call last):
        ...
     argparse.ArgumentTypeError: “CGvXAd” is not a Base64 encoded MAC address
 
     """
 
-    base64_regex = compile("[A-Za-z0-9/+]{8}$")
+    base64_regex = re_compile("[A-Za-z0-9/+]{8}$")
     if base64_regex.match(name):
         return name
     raise ArgumentTypeError(f"“{name}” is not a Base64 encoded MAC address")
 
 
 def byte_value(value):
     """Check if the given string represents a byte value
@@ -165,21 +165,21 @@
     Traceback (most recent call last):
        ...
     argparse.ArgumentTypeError: “08:6b:d7:01:de:666” is not a valid MAC address
 
     """
 
     try:
-        mac_address = EUI(address)
+        eui = EUI(address)
     except AddrFormatError as error:
         raise ArgumentTypeError(
             f"“{address}” is not a valid MAC address"
         ) from error
 
-    return mac_address
+    return eui
 
 
 def measurement_time(value: str) -> float:
     """Check if the given number is valid measurement time
 
     0 will be interpreted as infinite measurement runtime
```

### Comparing `icoc-1.8.0/mytoolit/config/config.py` & `icoc-1.9.0/mytoolit/config/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,20 +347,18 @@
             *sth_validators,
             *stu_validators,
         )
 
         try:
             self.validators.validate()
         except ValidationError as error:
-            config_files_text = "\n".join(
-                (
-                    f"  • {ConfigurationUtility.site_config_filepath}",
-                    f"  • {ConfigurationUtility.user_config_filepath}",
-                )
-            )
+            config_files_text = "\n".join((
+                f"  • {ConfigurationUtility.site_config_filepath}",
+                f"  • {ConfigurationUtility.user_config_filepath}",
+            ))
             raise SettingsIncorrectError(
                 f"Incorrect configuration: {error}\n\n"
                 "Please make sure that the configuration files:\n\n"
                 f"{config_files_text}\n\n"
                 "contain the correct configuration values"
             ) from error
```

### Comparing `icoc-1.8.0/mytoolit/config/config.yaml` & `icoc-1.9.0/mytoolit/config/config.yaml`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/config/user.yaml` & `icoc-1.9.0/mytoolit/config/user.yaml`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/eeprom/status.py` & `icoc-1.9.0/mytoolit/eeprom/status.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/examples/read_data.py` & `icoc-1.9.0/mytoolit/examples/read_data.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/examples/sth_name.py` & `icoc-1.9.0/mytoolit/examples/sth_name.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/experiments/RF_tests.py` & `icoc-1.9.0/mytoolit/experiments/RF_tests.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/experiments/old.py` & `icoc-1.9.0/mytoolit/experiments/old.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/measurement/acceleration.py` & `icoc-1.9.0/mytoolit/measurement/acceleration.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/measurement/sensor.py` & `icoc-1.9.0/mytoolit/measurement/sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,23 +51,21 @@
         ''
 
         >>> str(SensorConfig(second=1))
         'M2: S1'
 
         """
 
-        return ", ".join(
-            (
-                f"M{sensor}: S{value}"
-                for sensor, value in enumerate(
-                    (self.first, self.second, self.third), start=1
-                )
-                if value != 0
+        return ", ".join((
+            f"M{sensor}: S{value}"
+            for sensor, value in enumerate(
+                (self.first, self.second, self.third), start=1
             )
-        )
+            if value != 0
+        ))
 
     def __repr__(self) -> str:
         """The textual representation of the sensor configuration
 
         Returns
         -------
 
@@ -80,22 +78,20 @@
         'M1: S1, M2: S3, M3: S2'
 
         >>> repr(SensorConfig())
         'M1: None, M2: None, M3: None'
 
         """
 
-        return ", ".join(
-            (
-                f"M{sensor}: {f'S{value}' if value != 0 else 'None'}"
-                for sensor, value in enumerate(
-                    (self.first, self.second, self.third), start=1
-                )
+        return ", ".join((
+            f"M{sensor}: {f'S{value}' if value != 0 else 'None'}"
+            for sensor, value in enumerate(
+                (self.first, self.second, self.third), start=1
             )
-        )
+        ))
 
     def disable_channel(
         self, first: bool = False, second: bool = False, third: bool = False
     ):
         """Disable certain (measurement) channels
 
         Parameters
```

### Comparing `icoc-1.8.0/mytoolit/measurement/storage.py` & `icoc-1.9.0/mytoolit/measurement/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,21 +60,27 @@
     )
     return description_class
 
 
 # -- Classes ------------------------------------------------------------------
 
 
+# pylint: disable=too-few-public-methods
+
+
 class AccelerationDescription(IsDescription):
     """Description of HDF acceleration table"""
 
     counter = UInt8Col()
     timestamp = UInt64Col()  # Microseconds since measurement start
 
 
+# pylint: enable=too-few-public-methods
+
+
 class StorageException(Exception):
     """Exception for HDF storage errors"""
 
 
 class Storage:
     """Code to store measurement data in HDF5 format"""
```

### Comparing `icoc-1.8.0/mytoolit/measurement/units.py` & `icoc-1.9.0/mytoolit/measurement/units.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/measurement/voltage.py` & `icoc-1.9.0/mytoolit/measurement/voltage.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/old/MyToolItCommands.py` & `icoc-1.9.0/mytoolit/old/MyToolItCommands.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,17 +206,17 @@
     "CalibrationFactorK": 0x60,
     "CalibrationFactorD": 0x61,
     "Calibration Measurement": 0x62,
     "Alarm": 0x80,
     "Hmi": 0xC0,
 })
 
-MyToolItEeprom = bidict({
-    "Read": 0x00, "Write": 0x01, "Read Write Request Counter": 0x20
-})
+MyToolItEeprom = bidict(
+    {"Read": 0x00, "Write": 0x01, "Read Write Request Counter": 0x20}
+)
 
 MyToolItProductData = bidict({
     "GTIN": 0x00,
     "Hardware Version": 0x01,
     "Firmware Version": 0x02,
     "Release Name": 0x03,
     "Serial Number 1": 0x04,
```

### Comparing `icoc-1.8.0/mytoolit/old/MyToolItNetworkNumbers.py` & `icoc-1.9.0/mytoolit/old/MyToolItNetworkNumbers.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/old/MyToolItSth.py` & `icoc-1.9.0/mytoolit/old/MyToolItSth.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/old/Plotter.py` & `icoc-1.9.0/mytoolit/old/Plotter.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/old/SthLimits.py` & `icoc-1.9.0/mytoolit/old/SthLimits.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/old/cli.py` & `icoc-1.9.0/mytoolit/old/cli.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/old/network.py` & `icoc-1.9.0/mytoolit/old/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1374,28 +1374,24 @@
             self.AccConfig.b.bNumber3,
         )
         dataSetsVoltage = self.data_sets(
             self.VoltageConfig.b.bNumber1,
             self.VoltageConfig.b.bNumber2,
             self.VoltageConfig.b.bNumber3,
         )
-        dataPointsAcc = sum(
-            (
-                self.AccConfig.b.bNumber1,
-                self.AccConfig.b.bNumber2,
-                self.AccConfig.b.bNumber3,
-            )
-        )
-        dataPointsVoltage = sum(
-            (
-                self.VoltageConfig.b.bNumber1,
-                self.VoltageConfig.b.bNumber2,
-                self.VoltageConfig.b.bNumber3,
-            )
-        )
+        dataPointsAcc = sum((
+            self.AccConfig.b.bNumber1,
+            self.AccConfig.b.bNumber2,
+            self.AccConfig.b.bNumber3,
+        ))
+        dataPointsVoltage = sum((
+            self.VoltageConfig.b.bNumber1,
+            self.VoltageConfig.b.bNumber2,
+            self.VoltageConfig.b.bNumber3,
+        ))
         totalDataPoints = dataPointsAcc + dataPointsVoltage
         msgAcc = samplingRate / totalDataPoints
         if 0 < dataSetsAcc:
             msgAcc /= dataSetsAcc
         else:
             msgAcc = 0
         msgVoltage = samplingRate / totalDataPoints
```

### Comparing `icoc-1.8.0/mytoolit/old/test/HardwareSth.py` & `icoc-1.9.0/mytoolit/old/test/HardwareSth.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/old/test/MyToolItTestSth.py` & `icoc-1.9.0/mytoolit/old/test/MyToolItTestSth.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/old/test/MyToolItTestSthManually.py` & `icoc-1.9.0/mytoolit/old/test/MyToolItTestSthManually.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/old/test/MyToolItTestStu.py` & `icoc-1.9.0/mytoolit/old/test/MyToolItTestStu.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/old/test/MyToolItTestStuManually.py` & `icoc-1.9.0/mytoolit/old/test/MyToolItTestStuManually.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/old/ui.py` & `icoc-1.9.0/mytoolit/old/ui.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/report/MyTooliT.pdf` & `icoc-1.9.0/mytoolit/report/MyTooliT.pdf`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/report/forms.py` & `icoc-1.9.0/mytoolit/report/forms.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/report/pdf.py` & `icoc-1.9.0/mytoolit/report/pdf.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,32 +35,36 @@
         self.width = width
         self.height = height
 
         with open(filepath, "rb") as pdf_data:
             (page,) = PdfReader(pdf_data).pages
             self.data = pagexobj(page)
 
-    def wrap(self, width, height):
+    # pylint: disable=unused-argument
+
+    def wrap(self, availWidth, availHeight):
         """Wrap the PDF object according to the given dimensions
 
         Parameters
         ----------
 
-        width:
+        availWidth:
             The width of the wrapped PDF object
-        height:
+        availHeight:
             The height of the wrapped PDF object
 
         Returns
         -------
 
         The dimensions of the wrapped object
         """
         return self.width, self.height
 
+    # pylint: enable=unused-argument
+
     def drawOn(self, canvas, x, y, _=0):
         """Draw the PDF object on the given canvas
 
         Parameters
         ----------
 
         canvas:
```

### Comparing `icoc-1.8.0/mytoolit/report/report.py` & `icoc-1.9.0/mytoolit/report/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 from mytoolit.report.pdf import PDFImage
 from mytoolit.report.style import get_style_sheet
 from mytoolit.report.forms import CheckBoxList, KeepTogether, Signature
 
 # -- Functions ----------------------------------------------------------------
 
 
-# noinspection PyUnusedLocal
+# pylint: disable=unused-argument
+
+
 def _first_page(canvas, document, node):
     """Define the style of the first page of the report"""
 
     canvas.saveState()
 
     page_width = defaultPageSize[0]
     page_height = defaultPageSize[1]
@@ -59,16 +61,21 @@
     canvas.drawCentredString(
         center_width, page_height - title_offset, f"{node} Test Report"
     )
 
     canvas.restoreState()
 
 
+# pylint: enable=unused-argument
+
+
 # -- Class --------------------------------------------------------------------
 
+# pylint: disable=too-many-instance-attributes
+
 
 class Report:
     """Generate test reports using ReportLab"""
 
     story: List[Flowable]  # Improve happiness of PyCharm type checker
 
     def __init__(self, node="Device"):
@@ -80,27 +87,25 @@
         node:
             A text that specifies the node (e.g. STH) for which a report
             should be generated
 
         """
 
         self.node = node
+        device_name = {
+            "SMH": "Sensory Milling Head",
+            "STH": "Sensory Tool Holder",
+            "STU": "Stationary Transceiver Unit",
+            "Device": "Device",
+        }
         self.document = SimpleDocTemplate(
             f"{node} Test.pdf",
             author="MyTooliT",
             title="Test Report",
-            subject="{} Test".format(
-                "Sensory Tool Holder"
-                if node == "STH"
-                else (
-                    "Sensory Milling Head"
-                    if node == "SMH"
-                    else "Stationary Transceiver Unit"
-                )
-            ),
+            subject=f"{device_name[node]} Test",
         )
         self.story = [Spacer(1, 3 * cm)]
         self.styles = get_style_sheet()
 
         self.general = []
         self.attributes = []
         self.tests = []
@@ -256,17 +261,25 @@
 
         self.story.append(Signature().to_flowable())
 
         first_page = partial(_first_page, node=self.node)
         self.document.build(self.story, onFirstPage=first_page)
 
 
+# pylint: enable=too-many-instance-attributes
+
+
 # -- Main ---------------------------------------------------------------------
 
-if __name__ == "__main__":
+# pylint: disable=import-outside-toplevel
+
+
+def main():
+    """Manual test code for Report"""
+
     from platform import system
     from subprocess import run
 
     # Create a example test report
     node = "STH"
     pdf_path = f"{node} Test.pdf"
     report = Report(node)
@@ -284,10 +297,18 @@
         # pylint: disable=no-name-in-module
         from os import startfile  # type: ignore
         # pylint: enable=no-name-in-module
         # fmt: on
 
         startfile(pdf_path)
     else:
-        run([
-            "{}open".format("" if system() == "Darwin" else "xdg-"), pdf_path
-        ])
+        run(
+            [f"{'' if system() == 'Darwin' else 'xdg-'}open", pdf_path],
+            check=True,
+        )
+
+
+# pylint: enable=import-outside-toplevel
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `icoc-1.8.0/mytoolit/report/style.py` & `icoc-1.9.0/mytoolit/report/style.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/scripts/eeprom.py` & `icoc-1.9.0/mytoolit/scripts/eeprom.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/scripts/mac.py` & `icoc-1.9.0/mytoolit/scripts/mac.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/scripts/name.py` & `icoc-1.9.0/mytoolit/scripts/name.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/test/production/node.py` & `icoc-1.9.0/mytoolit/test/production/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,26 +133,28 @@
         cls.report.build()
 
     @classmethod
     def __output_general_data(cls):
         """Print general information and add it to PDF report"""
 
         now = datetime.now()
-        date = now.strftime("%Y-%m-%d")
-        time = now.strftime("%H:%M:%S")
-
-        operator = settings.operator.name
 
         attributes = [
             SimpleNamespace(
                 description="ICOc Version", value=__version__, pdf=True
             ),
-            SimpleNamespace(description="Date", value=date, pdf=True),
-            SimpleNamespace(description="Time", value=time, pdf=True),
-            SimpleNamespace(description="Operator", value=operator, pdf=True),
+            SimpleNamespace(
+                description="Date", value=now.strftime("%Y-%m-%d"), pdf=True
+            ),
+            SimpleNamespace(
+                description="Time", value=now.strftime("%H:%M:%S"), pdf=True
+            ),
+            SimpleNamespace(
+                description="Operator", value=settings.operator.name, pdf=True
+            ),
         ]
 
         cls.__output_data(attributes, node_data=False)
 
     @classmethod
     def __output_node_data(cls):
         """Print node information and add it to PDF report"""
@@ -182,20 +184,20 @@
             Specifies if this method outputs node specific or general data
         """
 
         # Only output something, if there is at least one attribute
         if not attributes:
             return
 
-        max_length_description = max([
-            len(attribute.description) for attribute in attributes
-        ])
-        max_length_value = max([
-            len(attribute.value) for attribute in attributes
-        ])
+        max_length_description = max(
+            (len(attribute.description) for attribute in attributes)
+        )
+        max_length_value = max(
+            (len(attribute.value) for attribute in attributes)
+        )
 
         # Print attributes to standard output
         print("\n")
         header = "Attributes" if node_data else "General"
         print(header)
         print("—" * len(header))
 
@@ -273,15 +275,17 @@
 
     def _connect(self):
         """Create a connection to the STU"""
 
         async def connect():
             """Create connection with new network class"""
 
+            # pylint: disable=attribute-defined-outside-init
             self.can = Network()
+            # pylint: enable=attribute-defined-outside-init
             await self.can.reset_node("STU 1")
             # Wait for reset to take place
             await async_sleep(2)
 
         loop = new_event_loop()
         set_event_loop(loop)
         self.loop = loop
@@ -322,27 +326,23 @@
             state,
             f"Expected state “{expected_state}” does not match "
             f"received state “{state}”",
         )
 
     def _test_firmware_flash(
         self,
-        node: str,
         flash_location: Union[str, Path],
         programmmer_serial_number: int,
         chip: str,
     ):
         """Upload bootloader and application into node
 
         Parameters
         ----------
 
-        node:
-            A textual description of the device/node that will be flashed
-
         flash_location:
             The location of the flash image
 
         programmer_serial_number:
             The serial number of the programming board
 
         chip:
```

### Comparing `icoc-1.8.0/mytoolit/test/production/sensor_node.py` & `icoc-1.9.0/mytoolit/test/production/sensor_node.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Shared test code for sensory nodes in the ICOtronic system"""
 
 # -- Imports ------------------------------------------------------------------
 
 from time import sleep
 
 from mytoolit.config import settings
+from mytoolit.can.node import Node
 from mytoolit.test.production.node import TestNode
 
 # -- Classes ------------------------------------------------------------------
 
 
 class TestSensorNode(TestNode):
     """This class contains support code for sensor node (SMH & STH)
@@ -77,14 +78,44 @@
 
         # The sensor devices need a little more time to switch from the
         # “Startup” to the “Operating” state
         sleep(1)
 
         self.loop.run_until_complete(self._test_connection("STH 1"))
 
+    async def _test_name(self, receiver: Node, name: str) -> str:
+        """Check if writing and reading back the name of a sensor device works
+
+        Parameters
+        ----------
+
+        receiver:
+            The node where the name should be updated
+
+        name:
+            The text that should be used as name for the sensor device
+
+        Returns
+        -------
+
+        Read back name
+
+        """
+
+        await self.can.write_eeprom_name(name, receiver)
+        read_name = await self.can.read_eeprom_name(receiver)
+
+        self.assertEqual(
+            name,
+            read_name,
+            f"Written name “{name}” does not match read name “{read_name}”",
+        )
+
+        return read_name
+
     async def _test_eeprom_sleep_advertisement_times(self):
         """Test if reading and writing of sleep/advertisement times works"""
 
         async def read_write_time(
             read_function, write_function, variable, description, milliseconds
         ):
             await write_function(milliseconds)
```

### Comparing `icoc-1.8.0/mytoolit/test/production/smh.py` & `icoc-1.9.0/mytoolit/test/production/smh.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 
         The text `disconnected` in the method name make sure that the test
         framework does not initialize a connection.
 
         """
 
         self._test_firmware_flash(
-            node="SMH",
             flash_location=settings.smh.firmware.location.flash,
             programmmer_serial_number=(
                 settings.smh.programming_board.serial_number
             ),
             chip="BGM121A256V2",
         )
 
@@ -71,34 +70,22 @@
 
     def test_eeprom(self):
         """Test if reading and writing the EEPROM works"""
 
         async def test_eeprom():
             """Test the EERPOM of the SMH"""
 
-            cls = type(self)
             receiver = Node("STH 1")
+            cls = type(self)
 
             # ========
             # = Name =
             # ========
 
-            name = settings.smh.name
-
-            await self.can.write_eeprom_name(name, receiver)
-            read_name = await self.can.read_eeprom_name(receiver)
-
-            self.assertEqual(
-                name,
-                read_name,
-                f"Written name “{name}” does not match read name"
-                f" “{read_name}”",
-            )
-
-            cls.name = read_name
+            cls.name = await self._test_name(receiver, settings.smh.name)
 
             # =========================
             # = Sleep & Advertisement =
             # =========================
 
             await self._test_eeprom_sleep_advertisement_times()
 
@@ -189,14 +176,16 @@
         )
 
 
 # -- Main ---------------------------------------------------------------------
 
 
 def main():
+    """Run production test for Sensory Milling Head (SMH)"""
+
     unittest_main(
         testRunner=ExtendedTestRunner, module="mytoolit.test.production.smh"
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `icoc-1.8.0/mytoolit/test/production/sth.py` & `icoc-1.9.0/mytoolit/test/production/sth.py`

 * *Files 3% similar despite different names*

```diff
@@ -162,26 +162,25 @@
             hardware_version = Version(settings.sth.hardware_version)
         except (TypeError, ValueError) as error:
             raise ValueError(
                 "Incorrect STH hardware version: "
                 f"“{settings.sth.hardware_version}”"
             ) from error
 
-        if not (1 <= hardware_version.major <= 2):
+        if not 1 <= hardware_version.major <= 2:
             raise ValueError(
                 f"STH hardware version “{hardware_version}” "
                 "is currently not supported"
             )
 
         chip = (
             "BGM113A256V2" if hardware_version.major <= 1 else "BGM123A256V2"
         )
 
         self._test_firmware_flash(
-            node="STH",
             flash_location=settings.sth.firmware.location.flash,
             programmmer_serial_number=(
                 settings.sth.programming_board.serial_number
             ),
             chip=chip,
         )
 
@@ -356,14 +355,16 @@
             voltage_diff_abs,
             voltage_diff_maximum,
             f"Measured voltage difference of {voltage_diff_abs:.0f} mV is "
             "greater than expected minimum voltage difference of "
             f"{voltage_diff_maximum:.0f} mV{possible_failure_reason}",
         )
 
+    # pylint: disable=too-many-locals
+
     def test_eeprom(self):
         """Test if reading and writing the EEPROM works"""
 
         async def test_eeprom():
             """Test the EERPOM of the STH"""
 
             cls = type(self)
@@ -376,26 +377,15 @@
             name = (
                 settings.sth.serial_number
                 if settings.sth.status == "Epoxied"
                 else convert_mac_base64(
                     cls.bluetooth_mac  # pylint: disable=no-member
                 )
             )
-
-            await self.can.write_eeprom_name(name, receiver)
-            read_name = await self.can.read_eeprom_name(receiver)
-
-            self.assertEqual(
-                name,
-                read_name,
-                f"Written name “{name}” does not match read name"
-                f" “{read_name}”",
-            )
-
-            cls.name = read_name
+            cls.name = await self._test_name(Node(receiver), name)
 
             # =========================
             # = Sleep & Advertisement =
             # =========================
 
             await self._test_eeprom_sleep_advertisement_times()
 
@@ -421,14 +411,16 @@
 
             sensor = settings.acceleration_sensor()
             acceleration_max = sensor.acceleration.maximum
             adc_max = 0xFFFF
             acceleration_slope = acceleration_max / adc_max
             acceleration_offset = -(acceleration_max / 2)
 
+            # pylint: disable=too-many-arguments
+
             async def write_read_check(
                 class_variable, write_routine, value, read_routine, axis, name
             ):
                 await write_routine(value)
                 setattr(cls, class_variable, await read_routine())
                 read_value = getattr(cls, class_variable)
                 self.assertAlmostEqual(
@@ -438,14 +430,16 @@
                         f"Written {axis} acceleration {name} "
                         f"“{acceleration_slope:.5f}” does not match read "
                         f"{axis} acceleration {name} "
                         f"“{read_value:.5f}”"
                     ),
                 )
 
+            # pylint: enable=too-many-arguments
+
             class_variables = (
                 "acceleration_slope_x",
                 "acceleration_slope_y",
                 "acceleration_slope_z",
                 "acceleration_offset_x",
                 "acceleration_offset_y",
                 "acceleration_offset_z",
@@ -463,20 +457,18 @@
                 self.can.read_eeprom_y_axis_acceleration_slope,
                 self.can.read_eeprom_z_axis_acceleration_slope,
                 self.can.read_eeprom_x_axis_acceleration_offset,
                 self.can.read_eeprom_y_axis_acceleration_offset,
                 self.can.read_eeprom_z_axis_acceleration_offset,
             )
             names = chain(*(repeat("slope", 3), repeat("offset", 3)))
-            values = chain(
-                *(
-                    repeat(acceleration_slope, 3),
-                    repeat(acceleration_offset, 3),
-                )
-            )
+            values = chain(*(
+                repeat(acceleration_slope, 3),
+                repeat(acceleration_offset, 3),
+            ))
             axes = list("xyz") * 2
 
             for (
                 class_variable,
                 write_routine,
                 value,
                 read_routine,
@@ -525,16 +517,20 @@
                 self.fail(
                     "Unable to reconnect to STH using updated name "
                     f"“{cls.name}”"  # pylint: disable=no-member
                 )
 
         self.loop.run_until_complete(test_eeprom())
 
+    # pylint: enable=too-many-locals
+
 
 def main():
+    """Run production test for Sensory Tool Holder (STH)"""
+
     unittest_main(
         testRunner=ExtendedTestRunner, module="mytoolit.test.production.sth"
     )
 
 
 # -- Main ---------------------------------------------------------------------
```

### Comparing `icoc-1.8.0/mytoolit/test/production/stu.py` & `icoc-1.9.0/mytoolit/test/production/stu.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 
         The text `disconnected` in the method name make sure that the test
         framework does not initialize a connection.
 
         """
 
         self._test_firmware_flash(
-            node="STU",
             flash_location=settings.stu.firmware.location.flash,
             programmmer_serial_number=(
                 settings.stu.programming_board.serial_number
             ),
             chip="BGM111A256V2",
         )
 
@@ -112,14 +111,16 @@
         self.loop.run_until_complete(test_eeprom())
 
 
 # -- Main ---------------------------------------------------------------------
 
 
 def main():
+    """Run production test for Stationary Transceiver Unit (STU)"""
+
     unittest_main(
         testRunner=ExtendedTestRunner, module="mytoolit.test.production.stu"
     )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `icoc-1.8.0/mytoolit/test/unit/extended_test_result.py` & `icoc-1.9.0/mytoolit/test/unit/extended_test_result.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/test/unit/extended_test_runner.py` & `icoc-1.9.0/mytoolit/test/unit/extended_test_runner.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/utility/data.py` & `icoc-1.9.0/mytoolit/utility/data.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/utility/environment.py` & `icoc-1.9.0/mytoolit/utility/environment.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/utility/log.py` & `icoc-1.9.0/mytoolit/utility/log.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/utility/naming.py` & `icoc-1.9.0/mytoolit/utility/naming.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/mytoolit/utility/open.py` & `icoc-1.9.0/mytoolit/utility/open.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     ------
 
     An `UnableToOpenError` if opening the file failed
 
     """
 
     # fmt: off
-    # pylint: disable=no-name-in-module
+    # pylint: disable=no-name-in-module, import-outside-toplevel
     from os import startfile  # type: ignore[attr-defined]
-    # pylint: enable=no-name-in-module
+    # pylint: enable=no-name-in-module, import-outside-toplevel
     # fmt: on
 
     try:
         startfile(filepath)
     except FileNotFoundError as error:
         raise UnableToOpenError(f"File “{filepath}” does not exist") from error
```

### Comparing `icoc-1.8.0/mytoolit/utility/types.py` & `icoc-1.9.0/mytoolit/utility/types.py`

 * *Files identical despite different names*

### Comparing `icoc-1.8.0/pyproject.toml` & `icoc-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     "icolyzer>=1.5.0", # Require ICOlyzer for Prysk tests
     "prysk[pytest-plugin]>=0.13.1",
     "pytest",
 ]
 
 [project.scripts]
 icoc = "mytoolit.old.ui:main"
-icon = "mytoolit.cmdline.icon:main"
+icon = "mytoolit.scripts.icon:main"
 check-eeprom = "mytoolit.scripts.eeprom:main"
 test-smh = "mytoolit.test.production.smh:main"
 test-sth = "mytoolit.test.production.sth:main"
 test-sth-verification = "mytoolit.old.test.MyToolItTestSth:main"
 test-stu-verification = "mytoolit.old.test.MyToolItTestStu:main"
 test-stu = "mytoolit.test.production.stu:main"
 convert-base64-mac = "mytoolit.scripts.name:main"
```

