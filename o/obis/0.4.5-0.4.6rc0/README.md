# Comparing `tmp/obis-0.4.5.tar.gz` & `tmp/obis-0.4.6rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obis-0.4.5.tar", last modified: Fri Oct  6 08:23:30 2023, max compression
+gzip compressed data, was "obis-0.4.6rc0.tar", last modified: Mon Apr 29 14:39:16 2024, max compression
```

## Comparing `obis-0.4.5.tar` & `obis-0.4.6rc0.tar`

### file list

```diff
@@ -1,112 +1,109 @@
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-10-06 08:23:30.838002 obis-0.4.5/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1083 2023-10-05 08:20:16.000000 obis-0.4.5/CHANGELOG.md
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    11357 2023-02-20 13:30:53.000000 obis-0.4.5/LICENSE
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      176 2023-02-20 13:30:53.000000 obis-0.4.5/MANIFEST.in
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    32146 2023-10-06 08:23:30.838002 obis-0.4.5/PKG-INFO
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    31587 2023-07-17 10:34:32.000000 obis-0.4.5/README.md
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-10-06 08:23:30.798002 obis-0.4.5/man/
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-10-06 08:23:30.802002 obis-0.4.5/man/man1/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-addref.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      879 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-clone.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      798 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-collection.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      825 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-commit.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-config.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1027 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-data_set.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      893 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-download.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-init.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-init_analysis.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-move.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      762 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-object.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      617 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-removeref.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1221 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-repository.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      742 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-settings.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-status.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      666 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis-sync.1
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1684 2023-02-20 13:30:53.000000 obis-0.4.5/man/man1/obis.1
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-10-06 08:23:30.802002 obis-0.4.5/obis/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      754 2023-10-06 08:23:17.000000 obis-0.4.5/obis/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-10-06 08:23:30.806002 obis-0.4.5/obis/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      317 2023-09-11 20:24:08.000000 obis-0.4.5/obis/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      563 2023-02-27 13:57:44.000000 obis-0.4.5/obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      915 2023-02-21 12:05:41.000000 obis-0.4.5/obis/conftest.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-10-06 08:23:30.810002 obis-0.4.5/obis/dm/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      889 2023-02-21 12:05:41.000000 obis-0.4.5/obis/dm/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-10-06 08:23:30.814002 obis-0.4.5/obis/dm/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      411 2023-02-21 12:13:21.000000 obis-0.4.5/obis/dm/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7402 2023-03-07 09:56:22.000000 obis-0.4.5/obis/dm/__pycache__/checksum.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2407 2023-02-21 12:13:22.000000 obis-0.4.5/obis/dm/__pycache__/command_log.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1839 2023-02-21 12:13:21.000000 obis-0.4.5/obis/dm/__pycache__/command_result.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    15644 2023-02-21 12:13:21.000000 obis-0.4.5/obis/dm/__pycache__/config.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    23132 2023-08-23 18:42:34.000000 obis-0.4.5/obis/dm/__pycache__/data_mgmt.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    17466 2023-07-17 14:48:25.000000 obis-0.4.5/obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7101 2023-03-30 10:33:16.000000 obis-0.4.5/obis/dm/__pycache__/git.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1351 2023-02-21 12:17:13.000000 obis-0.4.5/obis/dm/__pycache__/repository_utils.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3148 2023-03-30 10:51:56.000000 obis-0.4.5/obis/dm/__pycache__/utils.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7820 2023-03-07 08:26:10.000000 obis-0.4.5/obis/dm/checksum.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2674 2023-02-21 12:05:41.000000 obis-0.4.5/obis/dm/command_log.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1981 2023-02-21 12:05:41.000000 obis-0.4.5/obis/dm/command_result.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-10-06 08:23:30.822002 obis-0.4.5/obis/dm/commands/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      634 2023-02-21 12:05:41.000000 obis-0.4.5/obis/dm/commands/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-10-06 08:23:30.830002 obis-0.4.5/obis/dm/commands/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      194 2023-02-21 12:13:21.000000 obis-0.4.5/obis/dm/commands/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1867 2023-03-29 14:28:25.000000 obis-0.4.5/obis/dm/commands/__pycache__/addref.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3935 2023-02-28 09:09:45.000000 obis-0.4.5/obis/dm/commands/__pycache__/clone.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3041 2023-02-28 09:44:21.000000 obis-0.4.5/obis/dm/commands/__pycache__/collection.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3046 2023-02-21 16:35:01.000000 obis-0.4.5/obis/dm/commands/__pycache__/download.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3343 2023-03-03 14:34:14.000000 obis-0.4.5/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2416 2023-02-21 12:17:13.000000 obis-0.4.5/obis/dm/commands/__pycache__/move.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3263 2023-03-01 08:22:27.000000 obis-0.4.5/obis/dm/commands/__pycache__/object.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    10939 2023-08-23 18:48:33.000000 obis-0.4.5/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     6680 2023-02-21 12:17:13.000000 obis-0.4.5/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3273 2023-02-21 12:17:13.000000 obis-0.4.5/obis/dm/commands/__pycache__/removeref.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8949 2023-08-04 10:49:31.000000 obis-0.4.5/obis/dm/commands/__pycache__/search.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1599 2023-09-11 20:24:09.000000 obis-0.4.5/obis/dm/commands/__pycache__/upload.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1897 2023-03-29 14:28:17.000000 obis-0.4.5/obis/dm/commands/addref.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5292 2023-02-28 08:49:14.000000 obis-0.4.5/obis/dm/commands/clone.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3657 2023-02-28 09:16:53.000000 obis-0.4.5/obis/dm/commands/collection.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3920 2023-02-21 13:31:53.000000 obis-0.4.5/obis/dm/commands/download.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4124 2023-03-03 14:31:58.000000 obis-0.4.5/obis/dm/commands/download_physical.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2967 2023-02-21 12:05:41.000000 obis-0.4.5/obis/dm/commands/move.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4373 2023-03-01 08:22:23.000000 obis-0.4.5/obis/dm/commands/object.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    12135 2023-08-23 18:47:42.000000 obis-0.4.5/obis/dm/commands/openbis_command.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1535 2023-02-21 12:05:41.000000 obis-0.4.5/obis/dm/commands/openbis_command_test.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     9774 2023-02-21 12:05:41.000000 obis-0.4.5/obis/dm/commands/openbis_sync.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3565 2023-02-21 12:05:41.000000 obis-0.4.5/obis/dm/commands/removeref.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    13214 2023-08-02 10:52:21.000000 obis-0.4.5/obis/dm/commands/search.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1807 2023-08-25 13:40:17.000000 obis-0.4.5/obis/dm/commands/upload.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    16039 2023-02-21 12:05:42.000000 obis-0.4.5/obis/dm/config.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2934 2023-02-21 12:05:41.000000 obis-0.4.5/obis/dm/config_test.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    27953 2023-08-23 18:41:32.000000 obis-0.4.5/obis/dm/data_mgmt.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    14376 2023-03-29 13:51:23.000000 obis-0.4.5/obis/dm/data_mgmt_test.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      245 2023-02-20 13:30:53.000000 obis-0.4.5/obis/dm/git-annex-attributes
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8502 2023-03-30 10:32:13.000000 obis-0.4.5/obis/dm/git.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1905 2023-02-21 12:05:41.000000 obis-0.4.5/obis/dm/repository_utils.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3789 2023-03-30 10:51:34.000000 obis-0.4.5/obis/dm/utils.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      980 2023-02-21 12:05:41.000000 obis-0.4.5/obis/dm/utils_test.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-10-06 08:23:30.834002 obis-0.4.5/obis/scripts/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      919 2023-02-21 12:05:41.000000 obis-0.4.5/obis/scripts/__init__.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-10-06 08:23:30.834002 obis-0.4.5/obis/scripts/__pycache__/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      431 2023-02-21 12:13:22.000000 obis-0.4.5/obis/scripts/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    30930 2023-07-24 10:38:42.000000 obis-0.4.5/obis/scripts/__pycache__/cli.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2023-09-11 20:24:09.000000 obis-0.4.5/obis/scripts/__pycache__/click_util.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4351 2023-03-30 10:59:33.000000 obis-0.4.5/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    39340 2023-07-24 10:38:39.000000 obis-0.4.5/obis/scripts/cli.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1127 2023-08-25 13:48:21.000000 obis-0.4.5/obis/scripts/click_util.py
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5701 2023-03-30 10:59:06.000000 obis-0.4.5/obis/scripts/data_mgmt_runner.py
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-10-06 08:23:30.838002 obis-0.4.5/obis/test-data/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)   160470 2023-02-20 13:30:53.000000 obis-0.4.5/obis/test-data/snb-data.zip
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       43 2023-02-20 13:30:53.000000 obis-0.4.5/obis/test-data/text-data-2.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       32 2023-02-20 13:30:53.000000 obis-0.4.5/obis/test-data/text-data.txt
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-10-06 08:23:30.798002 obis-0.4.5/obis/test-data/user_config/
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-10-06 08:23:30.838002 obis-0.4.5/obis/test-data/user_config/.obis/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      167 2023-02-20 13:30:53.000000 obis-0.4.5/obis/test-data/user_config/.obis/config.json
-drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2023-10-06 08:23:30.806002 obis-0.4.5/obis.egg-info/
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    32146 2023-10-06 08:23:30.000000 obis-0.4.5/obis.egg-info/PKG-INFO
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3124 2023-10-06 08:23:30.000000 obis-0.4.5/obis.egg-info/SOURCES.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-10-06 08:23:30.000000 obis-0.4.5/obis.egg-info/dependency_links.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       47 2023-10-06 08:23:30.000000 obis-0.4.5/obis.egg-info/entry_points.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2023-02-23 08:39:07.000000 obis-0.4.5/obis.egg-info/not-zip-safe
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       37 2023-10-06 08:23:30.000000 obis-0.4.5/obis.egg-info/requires.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        5 2023-10-06 08:23:30.000000 obis-0.4.5/obis.egg-info/top_level.txt
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       38 2023-10-06 08:23:30.838002 obis-0.4.5/setup.cfg
--rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1982 2023-10-06 08:23:17.000000 obis-0.4.5/setup.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2024-04-29 14:39:16.579644 obis-0.4.6rc0/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1191 2024-04-29 14:39:07.000000 obis-0.4.6rc0/CHANGELOG.md
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    11357 2024-03-25 10:17:57.000000 obis-0.4.6rc0/LICENSE
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      176 2024-03-25 10:17:57.000000 obis-0.4.6rc0/MANIFEST.in
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    32169 2024-04-29 14:39:16.579644 obis-0.4.6rc0/PKG-INFO
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    31587 2024-03-25 10:17:58.000000 obis-0.4.6rc0/README.md
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2024-04-29 14:39:16.575644 obis-0.4.6rc0/man/
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2024-04-29 14:39:16.575644 obis-0.4.6rc0/man/man1/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-addref.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      879 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-clone.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      798 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-collection.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      825 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-commit.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-config.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1027 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-data_set.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      893 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-download.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      757 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-init.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-init_analysis.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      871 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-move.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      762 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-object.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      617 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-removeref.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1221 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-repository.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      742 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-settings.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      593 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-status.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      666 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis-sync.1
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1684 2024-03-25 10:17:57.000000 obis-0.4.6rc0/man/man1/obis.1
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2024-04-29 14:39:16.575644 obis-0.4.6rc0/obis/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      758 2024-04-29 14:34:20.000000 obis-0.4.6rc0/obis/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2024-04-29 14:39:16.575644 obis-0.4.6rc0/obis/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      317 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      915 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/conftest.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2024-04-29 14:39:16.575644 obis-0.4.6rc0/obis/dm/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      889 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2024-04-29 14:39:16.579644 obis-0.4.6rc0/obis/dm/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      411 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7402 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/__pycache__/checksum.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2407 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/__pycache__/command_log.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1839 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/__pycache__/command_result.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    15644 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/__pycache__/config.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    23202 2024-04-29 09:45:27.000000 obis-0.4.6rc0/obis/dm/__pycache__/data_mgmt.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7101 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/__pycache__/git.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1351 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/__pycache__/repository_utils.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3148 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/__pycache__/utils.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     7820 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/checksum.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2674 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/command_log.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1981 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/command_result.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2024-04-29 14:39:16.579644 obis-0.4.6rc0/obis/dm/commands/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      634 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/commands/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2024-04-29 14:39:16.579644 obis-0.4.6rc0/obis/dm/commands/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      194 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/commands/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1867 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/commands/__pycache__/addref.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3935 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/commands/__pycache__/clone.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3041 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/commands/__pycache__/collection.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3343 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2416 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/commands/__pycache__/move.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3263 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/commands/__pycache__/object.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    10939 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     6680 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3273 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/dm/commands/__pycache__/removeref.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8925 2024-04-29 12:11:21.000000 obis-0.4.6rc0/obis/dm/commands/__pycache__/search.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1780 2024-04-29 11:43:24.000000 obis-0.4.6rc0/obis/dm/commands/__pycache__/upload.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1897 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/commands/addref.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5292 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/commands/clone.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3657 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/commands/collection.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3920 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/commands/download.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4124 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/commands/download_physical.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2967 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/commands/move.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4373 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/commands/object.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    12135 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/commands/openbis_command.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1535 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/commands/openbis_command_test.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     9774 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/commands/openbis_sync.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3565 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/commands/removeref.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    13203 2024-04-29 14:31:17.000000 obis-0.4.6rc0/obis/dm/commands/search.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2136 2024-04-29 14:31:17.000000 obis-0.4.6rc0/obis/dm/commands/upload.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    16039 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/config.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2934 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/config_test.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    28052 2024-04-29 14:31:17.000000 obis-0.4.6rc0/obis/dm/data_mgmt.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    14376 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/data_mgmt_test.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      245 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/git-annex-attributes
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     8502 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/git.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1905 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/repository_utils.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     3789 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/utils.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      980 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/dm/utils_test.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2024-04-29 14:39:16.579644 obis-0.4.6rc0/obis/scripts/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      919 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/scripts/__init__.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2024-04-29 14:39:16.579644 obis-0.4.6rc0/obis/scripts/__pycache__/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      431 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/scripts/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    31073 2024-04-29 09:51:32.000000 obis-0.4.6rc0/obis/scripts/__pycache__/cli.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      746 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/scripts/__pycache__/click_util.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     4351 2024-04-26 14:09:19.000000 obis-0.4.6rc0/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    39518 2024-04-29 14:31:17.000000 obis-0.4.6rc0/obis/scripts/cli.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1127 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/scripts/click_util.py
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     5701 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/scripts/data_mgmt_runner.py
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2024-04-29 14:39:16.579644 obis-0.4.6rc0/obis/test-data/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)   160470 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/test-data/snb-data.zip
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       43 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/test-data/text-data-2.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       32 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/test-data/text-data.txt
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2024-04-29 14:39:16.575644 obis-0.4.6rc0/obis/test-data/user_config/
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2024-04-29 14:39:16.579644 obis-0.4.6rc0/obis/test-data/user_config/.obis/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)      167 2024-03-25 10:17:57.000000 obis-0.4.6rc0/obis/test-data/user_config/.obis/config.json
+drwxrwxr-x   0 alaskowski  (1000) alaskowski  (1000)        0 2024-04-29 14:39:16.575644 obis-0.4.6rc0/obis.egg-info/
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)    32169 2024-04-29 14:39:16.000000 obis-0.4.6rc0/obis.egg-info/PKG-INFO
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     2951 2024-04-29 14:39:16.000000 obis-0.4.6rc0/obis.egg-info/SOURCES.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2024-04-29 14:39:16.000000 obis-0.4.6rc0/obis.egg-info/dependency_links.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       48 2024-04-29 14:39:16.000000 obis-0.4.6rc0/obis.egg-info/entry_points.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        1 2024-03-27 12:00:09.000000 obis-0.4.6rc0/obis.egg-info/not-zip-safe
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       37 2024-04-29 14:39:16.000000 obis-0.4.6rc0/obis.egg-info/requires.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)        5 2024-04-29 14:39:16.000000 obis-0.4.6rc0/obis.egg-info/top_level.txt
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)       38 2024-04-29 14:39:16.579644 obis-0.4.6rc0/setup.cfg
+-rw-rw-r--   0 alaskowski  (1000) alaskowski  (1000)     1986 2024-04-29 14:34:20.000000 obis-0.4.6rc0/setup.py
```

### Comparing `obis-0.4.5/CHANGELOG.md` & `obis-0.4.6rc0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+# New in version 0.4.6
+
+* Fixes to data_set search command
+* Added setting of properties in upload command
+
 # New in version 0.4.5
 
 * Changed pybis dependency to version == 1.36.3
 
 # New in version 0.4.4
 
 * Improvements to dataset upload functionality
```

### Comparing `obis-0.4.5/LICENSE` & `obis-0.4.6rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/PKG-INFO` & `obis-0.4.6rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: obis
-Version: 0.4.5
+Version: 0.4.6rc0
 Summary: Local data management with assistance from OpenBIS.
 Home-page: https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line
 Author: ID SIS • ETH Zürich
 Author-email: openbis-support@id.ethz.ch
 License: Apache Software License Version 2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -714,7 +715,9 @@
 
 ## 9. Literature
 
 V. Korolev, A. Joshi, V. Korolev, M.A. Grasso, A. Joshi, M.A. Grasso, et al., "PROB: A tool for
 tracking provenance and reproducibility of big data experiments", Reproduce '14. HPCA 2014, vol. 11,
 pp. 264-286, 2014.
 http://ebiquity.umbc.edu/_file_directory_/papers/693.pdf
+
+
```

### Comparing `obis-0.4.5/README.md` & `obis-0.4.6rc0/README.md`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-addref.1` & `obis-0.4.6rc0/man/man1/obis-addref.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-clone.1` & `obis-0.4.6rc0/man/man1/obis-clone.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-collection.1` & `obis-0.4.6rc0/man/man1/obis-collection.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-commit.1` & `obis-0.4.6rc0/man/man1/obis-commit.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-config.1` & `obis-0.4.6rc0/man/man1/obis-config.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-data_set.1` & `obis-0.4.6rc0/man/man1/obis-data_set.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-download.1` & `obis-0.4.6rc0/man/man1/obis-download.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-init.1` & `obis-0.4.6rc0/man/man1/obis-init.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-init_analysis.1` & `obis-0.4.6rc0/man/man1/obis-init_analysis.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-move.1` & `obis-0.4.6rc0/man/man1/obis-move.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-object.1` & `obis-0.4.6rc0/man/man1/obis-object.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-removeref.1` & `obis-0.4.6rc0/man/man1/obis-removeref.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-repository.1` & `obis-0.4.6rc0/man/man1/obis-repository.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-settings.1` & `obis-0.4.6rc0/man/man1/obis-settings.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-status.1` & `obis-0.4.6rc0/man/man1/obis-status.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis-sync.1` & `obis-0.4.6rc0/man/man1/obis-sync.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/man/man1/obis.1` & `obis-0.4.6rc0/man/man1/obis.1`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/__init__.py` & `obis-0.4.6rc0/obis/dm/commands/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,14 @@
-#   Copyright ETH 2018 - 2023 Zürich, Scientific IT Services
+#   Copyright ETH 2007 - 2023 Zürich, Scientific IT Services
 # 
 #   Licensed under the Apache License, Version 2.0 (the "License");
 #   you may not use this file except in compliance with the License.
 #   You may obtain a copy of the License at
 # 
 #        http://www.apache.org/licenses/LICENSE-2.0
 #   
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
-__author__ = "ID SIS • ETH Zürich"
-__email__ = "openbis-support@id.ethz.ch"
-__version__ = "0.4.5"
-
-from .dm import *
```

### Comparing `obis-0.4.5/obis/conftest.py` & `obis-0.4.6rc0/obis/conftest.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/__init__.py` & `obis-0.4.6rc0/obis/dm/__init__.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/__pycache__/checksum.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/__pycache__/checksum.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Mar  7 08:26:10 2023 UTC, .py size: 7820 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 22f5 0664 8c1e 0000  o......."..d....
+00000000: 6f0d 0d0a 0000 0000 554f 0166 8c1e 0000  o.......UO.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 c200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6402 6403 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 6d07 5a07 0100 6417 6404 6405 8401 5a08  m.Z...d.d.d...Z.
 00000070: 6406 6407 8400 5a09 4700 6408 6409 8400  d.d...Z.G.d.d...
@@ -426,15 +426,15 @@
 00001a90: 0083 0301 006e 1031 0073 4177 0101 0001  .....n.1.sAw....
 00001aa0: 0001 0059 0001 0057 0064 0004 0004 0083  ...Y...W.d......
 00001ab0: 0301 0064 0053 0057 0064 0004 0004 0083  ...d.S.W.d......
 00001ac0: 0301 0064 0053 0031 0073 5977 0101 0001  ...d.S.1.sYw....
 00001ad0: 0001 0059 0001 0064 0053 0029 074e 7a14  ...Y...d.S.).Nz.
 00001ae0: 2e67 6974 2f69 6e66 6f2f 6174 7472 6962  .git/info/attrib
 00001af0: 7574 6573 7a0d 616e 6e65 782e 6261 636b  utesz.annex.back
-00001b00: 656e 64fa 013d 7202 0000 00da 0753 4841  end..=r......SHA
+00001b00: 656e 64da 013d 7202 0000 00da 0753 4841  end..=r......SHA
 00001b10: 3235 3645 7205 0000 0029 0672 0400 0000  256Er....).r....
 00001b20: 720d 0000 0072 4000 0000 da09 7265 6164  r....r@.....read
 00001b30: 6c69 6e65 7372 7900 0000 da05 7374 7269  linesry.....stri
 00001b40: 7029 0472 2a00 0000 da0d 6769 7461 7474  p).r*.....gitatt
 00001b50: 7269 6275 7465 73da 046c 696e 6572 6400  ributes..linerd.
 00001b60: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
 00001b70: 0072 6300 0000 c900 0000 7328 0000 000c  .rc.......s(....
```

### Comparing `obis-0.4.5/obis/dm/__pycache__/command_log.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/__pycache__/command_log.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb 21 12:05:41 2023 UTC, .py size: 2674 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 95b3 f463 720a 0000  o..........cr...
+00000000: 6f0d 0d0a 0000 0000 554f 0166 720a 0000  o.......UO.fr...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2800 0000 6400  .....@...s(...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 5a01 4700 6403 6404 8400 6404 6502 8303  Z.G.d.d...d.e...
 00000050: 5a03 6402 5300 2905 e900 0000 0029 01da  Z.d.S.)......)..
 00000060: 0864 6174 6574 696d 654e 6300 0000 0000  .datetimeNc.....
 00000070: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
```

### Comparing `obis-0.4.5/obis/dm/__pycache__/command_result.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/__pycache__/command_result.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb 21 12:05:41 2023 UTC, .py size: 1981 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 95b3 f463 bd07 0000  o..........c....
+00000000: 6f0d 0d0a 0000 0000 554f 0166 bd07 0000  o.......UO.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2400 0000 4700  .....@...s$...G.
 00000030: 6400 6401 8400 6401 6500 8303 5a01 4700  d.d...d.e...Z.G.
 00000040: 6402 6403 8400 6403 6502 8303 5a03 6404  d.d...d.e...Z.d.
 00000050: 5300 2905 6300 0000 0000 0000 0000 0000  S.).c...........
 00000060: 0000 0000 0003 0000 0040 0000 0073 3a00  .........@...s:.
 00000070: 0000 6500 5a01 6400 5a02 6401 5a03 640e  ..e.Z.d.Z.d.Z.d.
```

### Comparing `obis-0.4.5/obis/dm/__pycache__/config.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/__pycache__/config.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb 21 12:05:42 2023 UTC, .py size: 16039 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 96b3 f463 a73e 0000  o..........c.>..
+00000000: 6f0d 0d0a 0000 0000 554f 0166 a73e 0000  o.......UO.f.>..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 0c01 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6403 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 6d05 5a05 0100 4700 6404 6405 8400 6405  m.Z...G.d.d...d.
 00000060: 6506 8303 5a07 4700 6406 6407 8400 6407  e...Z.G.d.d...d.
 00000070: 6506 8303 5a08 4700 6408 6409 8400 6409  e...Z.G.d.d...d.
```

### Comparing `obis-0.4.5/obis/dm/__pycache__/data_mgmt.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/__pycache__/data_mgmt.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Aug 23 18:41:32 2023 UTC, .py size: 27953 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 dc52 e664 316d 0000  o........R.d1m..
+00000000: 6f0d 0d0a 0000 0000 9f66 2f66 946d 0000  o........f/f.m..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 ae01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6401 6c05 5a05 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6402 6c06 6d07 5a07 0100 6400 6401 6c08  d.l.m.Z...d.d.l.
 00000070: 5a08 6403 6404 6c09 6d0a 5a0b 0100 6403  Z.d.d.l.m.Z...d.
@@ -100,1347 +100,1352 @@
 00000630: 5f6d 676d 742e 7079 da08 4461 7461 4d67  _mgmt.py..DataMg
 00000640: 6d74 3200 0000 7338 0000 0010 0408 0208  mt2...s8........
 00000650: 0108 0108 0208 010a 020c 010a 010c 0108  ................
 00000660: 0108 0206 020a 020a 010e 0104 0104 ff08  ................
 00000670: 030e 0108 010e 0304 0104 ff0a 030e 0108  ................
 00000680: 0104 ff72 3800 0000 6300 0000 0000 0000  ...r8...c.......
 00000690: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
-000006a0: 0073 1a01 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
+000006a0: 0073 1c01 0000 6500 5a01 6400 5a02 6401  .s....e.Z.d.Z.d.
 000006b0: 5a03 0903 642b 6404 6405 8401 5a04 6406  Z...d+d.d...Z.d.
 000006c0: 6407 8400 5a05 6506 6a07 6408 6409 8400  d...Z.e.j.d.d...
 000006d0: 8301 5a08 6506 6a07 640a 640b 8400 8301  ..Z.e.j.d.d.....
 000006e0: 5a09 6506 6a07 642c 640d 640e 8401 8301  Z.e.j.d,d.d.....
 000006f0: 5a0a 6506 6a07 642c 640f 6410 8401 8301  Z.e.j.d,d.d.....
 00000700: 5a0b 6506 6a07 642d 6411 6412 8401 8301  Z.e.j.d-d.d.....
 00000710: 5a0c 6506 6a07 6413 6414 8400 8301 5a0d  Z.e.j.d.d.....Z.
 00000720: 6506 6a07 6415 6416 8400 8301 5a0e 6506  e.j.d.d.....Z.e.
 00000730: 6a07 6417 6418 8400 8301 5a0f 6506 6a07  j.d.d.....Z.e.j.
 00000740: 6419 641a 8400 8301 5a10 6506 6a07 641b  d.d.....Z.e.j.d.
 00000750: 641c 8400 8301 5a11 6506 6a07 642c 641d  d.....Z.e.j.d,d.
 00000760: 641e 8401 8301 5a12 6506 6a07 641f 6420  d.....Z.e.j.d.d 
-00000770: 8400 8301 5a13 6506 6a07 6421 6422 8400  ....Z.e.j.d!d"..
-00000780: 8301 5a14 6506 6a07 6423 6424 8400 8301  ..Z.e.j.d#d$....
-00000790: 5a15 6506 6a07 6425 6426 8400 8301 5a16  Z.e.j.d%d&....Z.
-000007a0: 090c 090c 642e 6427 6428 8401 5a17 6518  ....d.d'd(..Z.e.
-000007b0: 642f 6429 642a 8401 8301 5a19 640c 5300  d/d)d*....Z.d.S.
-000007c0: 2930 da10 4162 7374 7261 6374 4461 7461  )0..AbstractData
-000007d0: 4d67 6d74 7a65 4162 7374 7261 6374 206f  MgmtzeAbstract o
-000007e0: 626a 6563 7420 7468 6174 2069 6d70 6c65  bject that imple
-000007f0: 6d65 6e74 7320 6f70 6572 6174 696f 6e73  ments operations
-00000800: 2e0a 0a20 2020 2041 6c6c 206f 7065 7261  ...    All opera
-00000810: 7469 6f6e 7320 7468 726f 7720 616e 2065  tions throw an e
-00000820: 7865 7063 7469 6f6e 2069 6620 7468 6579  xepction if they
-00000830: 2066 6169 6c2e 0a20 2020 2046 5463 0b00   fail..    FTc..
-00000840: 0000 0000 0000 0000 0000 0b00 0000 0200  ................
-00000850: 0000 4300 0000 734c 0000 007c 017c 005f  ..C...sL...|.|._
-00000860: 007c 027c 005f 017c 037c 005f 027c 047c  .|.|._.|.|._.|.|
-00000870: 005f 037c 057c 005f 047c 067c 005f 057c  ._.|.|._.|.|._.|
-00000880: 077c 005f 067c 087c 005f 077c 097c 005f  .|._.|.|._.|.|._
-00000890: 087c 0a7c 005f 0964 017c 005f 0a64 027c  .|.|._.d.|._.d.|
-000008a0: 005f 0b64 0053 0029 034e 5446 290c 722e  ._.d.S.).NTF).r.
-000008b0: 0000 0072 2f00 0000 7236 0000 0072 3100  ...r/...r6...r1.
-000008c0: 0000 7232 0000 0072 1a00 0000 721b 0000  ..r2...r....r...
-000008d0: 0072 1c00 0000 7233 0000 0072 3400 0000  .r....r3...r4...
-000008e0: da11 7265 7374 6f72 655f 6f6e 5f73 6967  ..restore_on_sig
-000008f0: 696e 74da 1569 676e 6f72 655f 6d69 7373  int..ignore_miss
-00000900: 696e 675f 7061 7265 6e74 290b da04 7365  ing_parent)...se
-00000910: 6c66 722e 0000 0072 2f00 0000 7236 0000  lfr....r/...r6..
-00000920: 0072 3100 0000 7232 0000 0072 1a00 0000  .r1...r2...r....
-00000930: 721b 0000 0072 1c00 0000 7233 0000 0072  r....r....r3...r
-00000940: 3400 0000 721f 0000 0072 1f00 0000 7237  4...r....r....r7
-00000950: 0000 00da 085f 5f69 6e69 745f 5f61 0000  .....__init__a..
-00000960: 0073 1800 0000 0602 0601 0601 0601 0601  .s..............
-00000970: 0601 0601 0601 0601 0601 0603 0a01 7a19  ..............z.
-00000980: 4162 7374 7261 6374 4461 7461 4d67 6d74  AbstractDataMgmt
-00000990: 2e5f 5f69 6e69 745f 5f63 0300 0000 0000  .__init__c......
-000009a0: 0000 0000 0000 0400 0000 0400 0000 4300  ..............C.
-000009b0: 0000 7314 0000 0064 01a0 007c 017c 02a1  ..s....d...|.|..
-000009c0: 027d 0374 017c 0383 0182 0129 027a 1352  .}.t.|.....).z.R
-000009d0: 6169 7365 2061 6e20 6578 6365 7074 696f  aise an exceptio
-000009e0: 6e2e 7a0f 277b 7d27 2066 6169 6c65 642e  n.z.'{}' failed.
-000009f0: 207b 7d29 02da 0666 6f72 6d61 74da 0a56   {})...format..V
-00000a00: 616c 7565 4572 726f 7229 0472 3c00 0000  alueError).r<...
-00000a10: da07 636f 6d6d 616e 64da 0672 6561 736f  ..command..reaso
-00000a20: 6eda 076d 6573 7361 6765 721f 0000 0072  n..messager....r
-00000a30: 1f00 0000 7237 0000 00da 0b65 7272 6f72  ....r7.....error
-00000a40: 5f72 6169 7365 7200 0000 7304 0000 000c  _raiser...s.....
-00000a50: 0208 017a 1c41 6273 7472 6163 7444 6174  ...z.AbstractDat
-00000a60: 614d 676d 742e 6572 726f 725f 7261 6973  aMgmt.error_rais
-00000a70: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
-00000a80: 0000 0100 0000 4300 0000 f304 0000 0064  ......C........d
-00000a90: 0153 0029 027a 1b20 4765 7420 7468 6520  .S.).z. Get the 
-00000aa0: 7365 7474 696e 6773 2072 6573 6f6c 7665  settings resolve
-00000ab0: 7220 4e72 1f00 0000 a901 723c 0000 0072  r Nr......r<...r
-00000ac0: 1f00 0000 721f 0000 0072 3700 0000 da15  ....r....r7.....
-00000ad0: 6765 745f 7365 7474 696e 6773 5f72 6573  get_settings_res
-00000ae0: 6f6c 7665 7277 0000 00f3 0200 0000 0403  olverw..........
-00000af0: 7a26 4162 7374 7261 6374 4461 7461 4d67  z&AbstractDataMg
-00000b00: 6d74 2e67 6574 5f73 6574 7469 6e67 735f  mt.get_settings_
-00000b10: 7265 736f 6c76 6572 6302 0000 0000 0000  resolverc.......
-00000b20: 0000 0000 0002 0000 0001 0000 0043 0000  .............C..
-00000b30: 0072 4400 0000 2902 7a34 2053 6574 7570  .rD...).z4 Setup
-00000b40: 206c 6f63 616c 2073 6574 7469 6e67 7320   local settings 
-00000b50: 2d20 666f 7220 7573 696e 6720 6f62 6973  - for using obis
-00000b60: 2061 7320 6120 6c69 6272 6172 7920 4e72   as a library Nr
-00000b70: 1f00 0000 a902 723c 0000 00da 0c61 6c6c  ......r<.....all
-00000b80: 5f73 6574 7469 6e67 7372 1f00 0000 721f  _settingsr....r.
-00000b90: 0000 0072 3700 0000 da14 7365 7475 705f  ...r7.....setup_
-00000ba0: 6c6f 6361 6c5f 7365 7474 696e 6773 7c00  local_settings|.
-00000bb0: 0000 7247 0000 007a 2541 6273 7472 6163  ..rG...z%Abstrac
-00000bc0: 7444 6174 614d 676d 742e 7365 7475 705f  tDataMgmt.setup_
-00000bd0: 6c6f 6361 6c5f 7365 7474 696e 6773 4e63  local_settingsNc
-00000be0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00000bf0: 0100 0000 4300 0000 7244 0000 0029 0261  ....C...rD...).a
-00000c00: 4b01 0000 496e 6974 6961 6c69 7a65 2061  K...Initialize a
-00000c10: 2064 6174 6120 7265 706f 7369 746f 7279   data repository
-00000c20: 2061 7420 7468 6520 7061 7468 2077 6974   at the path wit
-00000c30: 6820 7468 6520 6465 7363 7269 7074 696f  h the descriptio
-00000c40: 6e2e 0a20 2020 2020 2020 203a 7061 7261  n..        :para
-00000c50: 6d20 7061 7468 3a20 5061 7468 2066 6f72  m path: Path for
-00000c60: 2074 6865 2072 6570 6f73 6974 6f72 792e   the repository.
-00000c70: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00000c80: 6465 7363 3a20 416e 206f 7074 696f 6e61  desc: An optiona
-00000c90: 6c20 7368 6f72 7420 6465 7363 7269 7074  l short descript
-00000ca0: 696f 6e20 6f66 2074 6865 2072 6570 6f73  ion of the repos
-00000cb0: 6974 6f72 7920 2875 7365 6420 6279 2067  itory (used by g
-00000cc0: 6974 2d61 6e6e 6578 290a 2020 2020 2020  it-annex).      
-00000cd0: 2020 3a70 6172 616d 2063 7265 6174 653a    :param create:
-00000ce0: 2049 6620 5472 7565 2061 6e64 2074 6865   If True and the
-00000cf0: 2066 6f6c 6465 7220 646f 6573 206e 6f74   folder does not
-00000d00: 2065 7869 7374 2c20 6372 6561 7465 2069   exist, create i
-00000d10: 742e 2044 6566 6175 6c74 7320 746f 2074  t. Defaults to t
-00000d20: 7275 652e 0a20 2020 2020 2020 203a 7265  rue..        :re
-00000d30: 7475 726e 3a20 4120 436f 6d6d 616e 6452  turn: A CommandR
-00000d40: 6573 756c 742e 0a20 2020 2020 2020 204e  esult..        N
-00000d50: 721f 0000 00a9 0272 3c00 0000 da04 6465  r......r<.....de
-00000d60: 7363 721f 0000 0072 1f00 0000 7237 0000  scr....r....r7..
-00000d70: 00da 0969 6e69 745f 6461 7461 8100 0000  ...init_data....
-00000d80: f302 0000 0004 087a 1a41 6273 7472 6163  .......z.Abstrac
-00000d90: 7444 6174 614d 676d 742e 696e 6974 5f64  tDataMgmt.init_d
-00000da0: 6174 6163 0300 0000 0000 0000 0000 0000  atac............
-00000db0: 0300 0000 0100 0000 4300 0000 7244 0000  ........C...rD..
-00000dc0: 0029 027a f549 6e69 7469 616c 697a 6520  .).z.Initialize 
-00000dd0: 616e 2061 6e61 6c79 7369 7320 7265 706f  an analysis repo
-00000de0: 7369 746f 7279 2061 7420 7468 6520 7061  sitory at the pa
-00000df0: 7468 2e0a 2020 2020 2020 2020 3a70 6172  th..        :par
-00000e00: 616d 2070 6172 656e 745f 666f 6c64 6572  am parent_folder
-00000e10: 3a20 5061 7468 2066 6f72 2074 6865 2072  : Path for the r
-00000e20: 6570 6f73 6974 6f72 792e 0a20 2020 2020  epository..     
-00000e30: 2020 203a 7061 7261 6d20 7061 7265 6e74     :param parent
-00000e40: 3a20 2872 6571 7569 7265 6420 7768 656e  : (required when
-00000e50: 206f 7574 7369 6465 206f 6620 6578 6973   outside of exis
-00000e60: 7469 6e67 2072 6570 6f73 6974 6f72 7929  ting repository)
-00000e70: 2050 6174 6820 666f 7220 7468 6520 7061   Path for the pa
-00000e80: 7265 6e74 2072 6570 6f73 6974 6f72 740a  rent repositort.
-00000e90: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00000ea0: 2041 2043 6f6d 6d61 6e64 5265 7375 6c74   A CommandResult
-00000eb0: 2e0a 2020 2020 2020 2020 4e72 1f00 0000  ..        Nr....
-00000ec0: a903 723c 0000 00da 0d70 6172 656e 745f  ..r<.....parent_
-00000ed0: 666f 6c64 6572 724c 0000 0072 1f00 0000  folderrL...r....
-00000ee0: 721f 0000 0072 3700 0000 da0d 696e 6974  r....r7.....init
-00000ef0: 5f61 6e61 6c79 7369 738b 0000 00f3 0200  _analysis.......
-00000f00: 0000 0407 7a1e 4162 7374 7261 6374 4461  ....z.AbstractDa
-00000f10: 7461 4d67 6d74 2e69 6e69 745f 616e 616c  taMgmt.init_anal
-00000f20: 7973 6973 6304 0000 0000 0000 0000 0000  ysisc...........
-00000f30: 0004 0000 0001 0000 0043 0000 0072 4400  .........C...rD.
-00000f40: 0000 2902 615e 0100 0043 6f6d 6d69 7420  ..).a^...Commit 
-00000f50: 7468 6520 6375 7272 656e 7420 7265 706f  the current repo
-00000f60: 2e0a 0a20 2020 2020 2020 2054 6869 7320  ...        This 
-00000f70: 6973 7375 6573 2061 2067 6974 2063 6f6d  issues a git com
-00000f80: 6d69 7420 616e 6420 636f 6e6e 6563 7473  mit and connects
-00000f90: 2074 6f20 6f70 656e 4249 5320 616e 6420   to openBIS and 
-00000fa0: 6372 6561 7465 7320 6120 6461 7461 2073  creates a data s
-00000fb0: 6574 2069 6e20 6f70 656e 4249 532e 0a20  et in openBIS.. 
-00000fc0: 2020 2020 2020 203a 7061 7261 6d20 6d73         :param ms
-00000fd0: 673a 2043 6f6d 6d69 7420 6d65 7373 6167  g: Commit messag
-00000fe0: 652e 0a20 2020 2020 2020 203a 7061 7261  e..        :para
-00000ff0: 6d20 6175 746f 5f61 6464 3a20 4175 746f  m auto_add: Auto
-00001000: 6d61 7469 6361 6c6c 7920 6164 6420 616c  matically add al
-00001010: 6c20 6669 6c65 7320 696e 2074 6865 2066  l files in the f
-00001020: 6f6c 6465 7220 746f 2074 6865 2072 6570  older to the rep
-00001030: 6f2e 2044 6566 6175 6c74 7320 746f 2054  o. Defaults to T
-00001040: 7275 652e 0a20 2020 2020 2020 203a 7061  rue..        :pa
-00001050: 7261 6d20 7379 6e63 3a20 4966 2074 7275  ram sync: If tru
-00001060: 652c 2073 796e 6320 7769 7468 206f 7065  e, sync with ope
-00001070: 6e42 4953 2073 6572 7665 722e 0a20 2020  nBIS server..   
-00001080: 2020 2020 203a 7265 7475 726e 3a20 4120       :return: A 
-00001090: 436f 6d6d 616e 6452 6573 756c 742e 0a20  CommandResult.. 
-000010a0: 2020 2020 2020 204e 721f 0000 00a9 0472         Nr......r
-000010b0: 3c00 0000 da03 6d73 67da 0861 7574 6f5f  <.....msg..auto_
-000010c0: 6164 64da 0473 796e 6372 1f00 0000 721f  add..syncr....r.
-000010d0: 0000 0072 3700 0000 da06 636f 6d6d 6974  ...r7.....commit
-000010e0: 9400 0000 7302 0000 0004 0a7a 1741 6273  ....s......z.Abs
-000010f0: 7472 6163 7444 6174 614d 676d 742e 636f  tractDataMgmt.co
-00001100: 6d6d 6974 6301 0000 0000 0000 0000 0000  mmitc...........
-00001110: 0001 0000 0001 0000 0043 0000 0072 4400  .........C...rD.
-00001120: 0000 2902 7a86 5379 6e63 2074 6865 2063  ..).z.Sync the c
-00001130: 7572 7265 6e74 2072 6570 6f2e 0a0a 2020  urrent repo...  
-00001140: 2020 2020 2020 5468 6973 2063 6f6e 6e65        This conne
-00001150: 6374 7320 746f 206f 7065 6e42 4953 2061  cts to openBIS a
-00001160: 6e64 2063 7265 6174 6573 2061 2064 6174  nd creates a dat
-00001170: 6120 7365 7420 696e 206f 7065 6e42 4953  a set in openBIS
-00001180: 2e0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00001190: 6e3a 2041 2043 6f6d 6d61 6e64 5265 7375  n: A CommandResu
-000011a0: 6c74 2e0a 2020 2020 2020 2020 4e72 1f00  lt..        Nr..
-000011b0: 0000 7245 0000 0072 1f00 0000 721f 0000  ..rE...r....r...
-000011c0: 0072 3700 0000 7256 0000 00a0 0000 0072  .r7...rV.......r
-000011d0: 5200 0000 7a15 4162 7374 7261 6374 4461  R...z.AbstractDa
-000011e0: 7461 4d67 6d74 2e73 796e 6363 0100 0000  taMgmt.syncc....
-000011f0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00001200: 4300 0000 7244 0000 0029 027a 5752 6574  C...rD...).zWRet
-00001210: 7572 6e20 7468 6520 7374 6174 7573 206f  urn the status o
-00001220: 6620 7468 6520 6375 7272 656e 7420 7265  f the current re
-00001230: 706f 7369 746f 7279 2e0a 2020 2020 2020  pository..      
-00001240: 2020 3a72 6574 7572 6e3a 2041 2043 6f6d    :return: A Com
-00001250: 6d61 6e64 5265 7375 6c74 2e0a 2020 2020  mandResult..    
-00001260: 2020 2020 4e72 1f00 0000 7245 0000 0072      Nr....rE...r
-00001270: 1f00 0000 721f 0000 0072 3700 0000 da06  ....r....r7.....
-00001280: 7374 6174 7573 a900 0000 f302 0000 0004  status..........
-00001290: 057a 1741 6273 7472 6163 7444 6174 614d  .z.AbstractDataM
-000012a0: 676d 742e 7374 6174 7573 6305 0000 0000  gmt.statusc.....
-000012b0: 0000 0000 0000 0005 0000 0001 0000 0043  ...............C
-000012c0: 0000 0072 4400 0000 2902 617d 0100 0043  ...rD...).a}...C
-000012d0: 6c6f 6e65 202f 2063 6f70 7920 6120 7265  lone / copy a re
-000012e0: 706f 7369 746f 7279 2072 656c 6174 6564  pository related
-000012f0: 2074 6f20 7468 6520 6769 7665 6e20 6461   to the given da
-00001300: 7461 2073 6574 2069 642e 0a20 2020 2020  ta set id..     
-00001310: 2020 203a 7061 7261 6d20 6461 7461 5f73     :param data_s
-00001320: 6574 5f69 643a 200a 2020 2020 2020 2020  et_id: .        
-00001330: 3a70 6172 616d 2073 7368 5f75 7365 723a  :param ssh_user:
-00001340: 2073 7368 2075 7365 7220 666f 7220 7265   ssh user for re
-00001350: 6d6f 7465 2073 7973 7465 6d20 286f 7074  mote system (opt
-00001360: 696f 6e61 6c29 0a20 2020 2020 2020 203a  ional).        :
-00001370: 7061 7261 6d20 636f 6e74 656e 745f 636f  param content_co
-00001380: 7079 5f69 6e64 6578 3a20 696e 6465 7820  py_index: index 
-00001390: 6f66 2063 6f6e 7465 6e74 2063 6f70 7920  of content copy 
-000013a0: 696e 2063 6173 6520 7468 6572 6520 6172  in case there ar
-000013b0: 6520 6d75 6c74 6970 6c65 2063 6f70 6965  e multiple copie
-000013c0: 7320 286f 7074 696f 6e61 6c29 0a20 2020  s (optional).   
-000013d0: 2020 2020 203a 7061 7261 6d20 736b 6970       :param skip
-000013e0: 5f69 6e74 6567 7269 7479 5f63 6865 636b  _integrity_check
-000013f0: 3a20 6966 2074 7275 652c 2074 6865 2066  : if true, the f
-00001400: 696c 6520 6368 6563 6b73 756d 7320 7769  ile checksums wi
-00001410: 6c6c 206e 6f74 2062 6520 6368 6563 6b65  ll not be checke
-00001420: 640a 2020 2020 2020 2020 3a72 6574 7572  d.        :retur
-00001430: 6e3a 2041 2043 6f6d 6d61 6e64 5265 7375  n: A CommandResu
-00001440: 6c74 2e0a 2020 2020 2020 2020 4e72 1f00  lt..        Nr..
-00001450: 0000 a905 723c 0000 00da 0b64 6174 615f  ....r<.....data_
-00001460: 7365 745f 6964 da08 7373 685f 7573 6572  set_id..ssh_user
-00001470: da12 636f 6e74 656e 745f 636f 7079 5f69  ..content_copy_i
-00001480: 6e64 6578 da14 736b 6970 5f69 6e74 6567  ndex..skip_integ
-00001490: 7269 7479 5f63 6865 636b 721f 0000 0072  rity_checkr....r
-000014a0: 1f00 0000 7237 0000 00da 0563 6c6f 6e65  ....r7.....clone
-000014b0: b000 0000 f302 0000 0004 097a 1641 6273  ...........z.Abs
-000014c0: 7472 6163 7444 6174 614d 676d 742e 636c  tractDataMgmt.cl
-000014d0: 6f6e 6563 0500 0000 0000 0000 0000 0000  onec............
-000014e0: 0500 0000 0100 0000 4300 0000 7244 0000  ........C...rD..
-000014f0: 0029 0261 7501 0000 4d6f 7665 2061 2072  .).au...Move a r
-00001500: 6570 6f73 6974 6f72 7920 7265 6c61 7465  epository relate
-00001510: 6420 746f 2074 6865 2067 6976 656e 2064  d to the given d
-00001520: 6174 6120 7365 7420 6964 2e0a 2020 2020  ata set id..    
-00001530: 2020 2020 3a70 6172 616d 2064 6174 615f      :param data_
-00001540: 7365 745f 6964 3a20 0a20 2020 2020 2020  set_id: .       
-00001550: 203a 7061 7261 6d20 7373 685f 7573 6572   :param ssh_user
-00001560: 3a20 7373 6820 7573 6572 2066 6f72 2072  : ssh user for r
-00001570: 656d 6f74 6520 7379 7374 656d 2028 6f70  emote system (op
-00001580: 7469 6f6e 616c 290a 2020 2020 2020 2020  tional).        
-00001590: 3a70 6172 616d 2063 6f6e 7465 6e74 5f63  :param content_c
-000015a0: 6f70 795f 696e 6465 783a 2069 6e64 6578  opy_index: index
-000015b0: 206f 6620 636f 6e74 656e 7420 636f 7079   of content copy
-000015c0: 2069 6e20 6361 7365 2074 6865 7265 2061   in case there a
-000015d0: 7265 206d 756c 7469 706c 6520 636f 7069  re multiple copi
-000015e0: 6573 2028 6f70 7469 6f6e 616c 290a 2020  es (optional).  
-000015f0: 2020 2020 2020 3a70 6172 616d 2073 6b69        :param ski
-00001600: 705f 696e 7465 6772 6974 795f 6368 6563  p_integrity_chec
-00001610: 6b3a 2069 6620 7472 7565 2c20 7468 6520  k: if true, the 
-00001620: 6669 6c65 2063 6865 636b 7375 6d73 2077  file checksums w
-00001630: 696c 6c20 6e6f 7420 6265 2063 6865 636b  ill not be check
-00001640: 6564 0a20 2020 2020 2020 203a 7265 7475  ed.        :retu
-00001650: 726e 3a20 4120 436f 6d6d 616e 6452 6573  rn: A CommandRes
-00001660: 756c 742e 0a20 2020 2020 2020 204e 721f  ult..        Nr.
-00001670: 0000 0072 5a00 0000 721f 0000 0072 1f00  ...rZ...r....r..
-00001680: 0000 7237 0000 00da 046d 6f76 65bb 0000  ..r7.....move...
-00001690: 0072 6000 0000 7a15 4162 7374 7261 6374  .r`...z.Abstract
-000016a0: 4461 7461 4d67 6d74 2e6d 6f76 6563 0100  DataMgmt.movec..
-000016b0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
-000016c0: 0000 4300 0000 7244 0000 0029 027a 6341  ..C...rD...).zcA
-000016d0: 6464 2074 6865 2063 7572 7265 6e74 2066  dd the current f
-000016e0: 6f6c 6465 7220 6173 2061 6e20 6f62 6973  older as an obis
-000016f0: 2072 6570 6f73 6974 6f72 7920 746f 206f   repository to o
-00001700: 7065 6e42 4953 2e0a 2020 2020 2020 2020  penBIS..        
-00001710: 3a72 6574 7572 6e3a 2041 2043 6f6d 6d61  :return: A Comma
-00001720: 6e64 5265 7375 6c74 2e0a 2020 2020 2020  ndResult..      
-00001730: 2020 4e72 1f00 0000 7245 0000 0072 1f00    Nr....rE...r..
-00001740: 0000 721f 0000 0072 3700 0000 da06 6164  ..r....r7.....ad
-00001750: 6472 6566 c600 0000 7259 0000 007a 1741  dref....rY...z.A
-00001760: 6273 7472 6163 7444 6174 614d 676d 742e  bstractDataMgmt.
-00001770: 6164 6472 6566 6302 0000 0000 0000 0000  addrefc.........
-00001780: 0000 0002 0000 0001 0000 0043 0000 0072  ...........C...r
-00001790: 4400 0000 2902 7ab4 5265 6d6f 7665 2074  D...).z.Remove t
-000017a0: 6865 2063 7572 7265 6e74 2066 6f6c 6465  he current folde
-000017b0: 7220 2f20 7265 706f 7369 746f 7279 2066  r / repository f
-000017c0: 726f 6d20 6f70 656e 4249 532e 0a20 2020  rom openBIS..   
-000017d0: 2020 2020 203a 7061 7261 6d20 6461 7461       :param data
-000017e0: 5f73 6574 5f69 643a 2049 6420 6f66 2074  _set_id: Id of t
-000017f0: 6865 2064 6174 6120 6672 6f6d 2077 6869  he data from whi
-00001800: 6368 2061 2072 6566 6572 656e 6365 2073  ch a reference s
-00001810: 686f 756c 6420 6265 2072 656d 6f76 6564  hould be removed
-00001820: 2e0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00001830: 6e3a 2041 2043 6f6d 6d61 6e64 5265 7375  n: A CommandResu
-00001840: 6c74 2e0a 2020 2020 2020 2020 4e72 1f00  lt..        Nr..
-00001850: 0000 a902 723c 0000 0072 5b00 0000 721f  ....r<...r[...r.
-00001860: 0000 0072 1f00 0000 7237 0000 00da 0972  ...r....r7.....r
-00001870: 656d 6f76 6572 6566 cd00 0000 7302 0000  emoveref....s...
-00001880: 0004 067a 1a41 6273 7472 6163 7444 6174  ...z.AbstractDat
-00001890: 614d 676d 742e 7265 6d6f 7665 7265 6663  aMgmt.removerefc
-000018a0: 0500 0000 0000 0000 0000 0000 0500 0000  ................
-000018b0: 0100 0000 4300 0000 7244 0000 0029 0261  ....C...rD...).a
-000018c0: 9001 0000 446f 776e 6c6f 6164 2066 696c  ....Download fil
-000018d0: 6573 206f 6620 6120 7265 706f 7369 746f  es of a reposito
-000018e0: 7279 2077 6974 686f 7574 2061 6464 696e  ry without addin
-000018f0: 6720 6120 636f 6e74 656e 7420 636f 7079  g a content copy
-00001900: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-00001910: 2064 6174 615f 7365 745f 6964 3a20 4964   data_set_id: Id
-00001920: 206f 6620 7468 6520 6461 7461 2073 6574   of the data set
-00001930: 2074 6f20 646f 776e 6c6f 6164 2066 726f   to download fro
-00001940: 6d2e 0a20 2020 2020 2020 203a 7061 7261  m..        :para
-00001950: 6d20 6672 6f6d 5f66 696c 653a 2050 6174  m from_file: Pat
-00001960: 6820 6f66 2061 2066 696c 6520 7769 7468  h of a file with
-00001970: 2061 206c 6973 7420 6f66 2064 6174 6173   a list of datas
-00001980: 6574 7320 746f 2064 6f77 6e6c 6f61 642e  ets to download.
-00001990: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000019a0: 6669 6c65 3a20 5061 7468 206f 6620 6120  file: Path of a 
-000019b0: 6669 6c65 2069 6e20 7468 6520 6461 7461  file in the data
-000019c0: 2073 6574 2074 6f20 646f 776e 6c6f 6164   set to download
-000019d0: 2e20 416c 6c20 6669 6c65 7320 6172 6520  . All files are 
-000019e0: 646f 776e 6c6f 6164 6564 2069 6620 6974  downloaded if it
-000019f0: 2069 7320 4e6f 6e65 2e0a 2020 2020 2020   is None..      
-00001a00: 2020 3a70 6172 616d 2073 6b69 705f 696e    :param skip_in
-00001a10: 7465 6772 6974 795f 6368 6563 6b3a 2043  tegrity_check: C
-00001a20: 6865 636b 7375 6d73 206f 6620 6669 6c65  hecksums of file
-00001a30: 7320 6172 6520 6e6f 7420 7665 7269 6669  s are not verifi
-00001a40: 6564 2069 6620 7472 7565 2e0a 2020 2020  ed if true..    
-00001a50: 2020 2020 4e72 1f00 0000 a905 723c 0000      Nr......r<..
-00001a60: 0072 5b00 0000 da09 6672 6f6d 5f66 696c  .r[.....from_fil
-00001a70: 65da 0466 696c 6572 5e00 0000 721f 0000  e..filer^...r...
-00001a80: 0072 1f00 0000 7237 0000 00da 0864 6f77  .r....r7.....dow
-00001a90: 6e6c 6f61 64d5 0000 0072 4e00 0000 7a19  nload....rN...z.
-00001aa0: 4162 7374 7261 6374 4461 7461 4d67 6d74  AbstractDataMgmt
-00001ab0: 2e64 6f77 6e6c 6f61 6463 0400 0000 0000  .downloadc......
-00001ac0: 0000 0000 0000 0400 0000 0100 0000 4300  ..............C.
-00001ad0: 0000 7244 0000 0029 027a ec55 706c 6f61  ..rD...).z.Uploa
-00001ae0: 6420 6669 6c65 732f 6469 7265 6374 6f72  d files/director
-00001af0: 6965 7320 696e 746f 2061 206e 6577 2064  ies into a new d
-00001b00: 6174 6120 7365 742e 0a20 2020 2020 2020  ata set..       
-00001b10: 203a 7061 7261 6d20 7361 6d70 6c65 5f69   :param sample_i
-00001b20: 643a 2070 6572 6d49 6420 6f72 2073 616d  d: permId or sam
-00001b30: 706c 6520 7061 7468 206f 6620 7468 6520  ple path of the 
-00001b40: 7061 7265 6e74 2073 616d 706c 650a 2020  parent sample.  
-00001b50: 2020 2020 2020 3a70 6172 616d 2064 6174        :param dat
-00001b60: 615f 7365 745f 7479 7065 3a20 7479 7065  a_set_type: type
-00001b70: 206f 6620 6372 6561 7465 6420 6461 7461   of created data
-00001b80: 2073 6574 0a20 2020 2020 2020 203a 7061   set.        :pa
-00001b90: 7261 6d20 6669 6c65 733a 206c 6973 7420  ram files: list 
-00001ba0: 6f66 2066 696c 6573 2f64 6972 6563 746f  of files/directo
-00001bb0: 7269 6573 2074 6f20 7570 6c6f 6164 0a20  ries to upload. 
-00001bc0: 2020 2020 2020 204e 721f 0000 0029 0472         Nr....).r
-00001bd0: 3c00 0000 da09 7361 6d70 6c65 5f69 64da  <.....sample_id.
-00001be0: 0d64 6174 615f 7365 745f 7479 7065 da05  .data_set_type..
-00001bf0: 6669 6c65 7372 1f00 0000 721f 0000 0072  filesr....r....r
-00001c00: 3700 0000 da06 7570 6c6f 6164 df00 0000  7.....upload....
-00001c10: 7252 0000 007a 1741 6273 7472 6163 7444  rR...z.AbstractD
-00001c20: 6174 614d 676d 742e 7570 6c6f 6164 6304  ataMgmt.uploadc.
-00001c30: 0000 0000 0000 0000 0000 0004 0000 0001  ................
-00001c40: 0000 0043 0000 0072 4400 0000 2902 612e  ...C...rD...).a.
-00001c50: 0100 0053 6561 7263 6820 666f 7220 6f62  ...Search for ob
-00001c60: 6a65 6374 7320 696e 206f 7065 6e42 4953  jects in openBIS
-00001c70: 2075 7369 6e67 2066 696c 7465 7269 6e67   using filtering
-00001c80: 2063 7269 7465 7269 612e 0a20 2020 2020   criteria..     
-00001c90: 2020 203a 7061 7261 6d20 6669 6c74 6572     :param filter
-00001ca0: 733a 2064 6963 7469 6f6e 6172 7920 6f66  s: dictionary of
-00001cb0: 2066 696c 7465 7220 7061 7261 6d65 7465   filter paramete
-00001cc0: 7273 0a20 2020 2020 2020 203a 7061 7261  rs.        :para
-00001cd0: 6d20 7265 6375 7273 6976 653a 2046 6c61  m recursive: Fla
-00001ce0: 6720 696e 6469 6361 7469 6e67 2069 6620  g indicating if 
-00001cf0: 7365 6172 6368 2073 686f 756c 6420 696e  search should in
-00001d00: 636c 7564 6520 6368 696c 6472 656e 2072  clude children r
-00001d10: 6563 7572 7369 7665 6c79 0a20 2020 2020  ecursively.     
-00001d20: 2020 203a 7061 7261 6d20 7361 7665 3a20     :param save: 
-00001d30: 4669 6c65 2070 6174 6820 746f 2073 6176  File path to sav
-00001d40: 6520 7265 7375 6c74 732e 2049 6620 6d69  e results. If mi
-00001d50: 7373 696e 672c 2073 6561 7263 6820 7265  ssing, search re
-00001d60: 7375 6c74 7320 7769 6c6c 206e 6f74 2062  sults will not b
-00001d70: 6520 7361 7665 642e 0a20 2020 2020 2020  e saved..       
-00001d80: 204e 721f 0000 00a9 0472 3c00 0000 da07   Nr......r<.....
-00001d90: 6669 6c74 6572 73da 0972 6563 7572 7369  filters..recursi
-00001da0: 7665 da04 7361 7665 721f 0000 0072 1f00  ve..saver....r..
-00001db0: 0000 7237 0000 00da 0d73 6561 7263 685f  ..r7.....search_
-00001dc0: 6f62 6a65 6374 e800 0000 7252 0000 007a  object....rR...z
-00001dd0: 1e41 6273 7472 6163 7444 6174 614d 676d  .AbstractDataMgm
-00001de0: 742e 7365 6172 6368 5f6f 626a 6563 7463  t.search_objectc
-00001df0: 0400 0000 0000 0000 0000 0000 0400 0000  ................
-00001e00: 0100 0000 4300 0000 7244 0000 0029 0261  ....C...rD...).a
-00001e10: 2f01 0000 5365 6172 6368 2066 6f72 2064  /...Search for d
-00001e20: 6174 6173 6574 7320 696e 206f 7065 6e42  atasets in openB
-00001e30: 4953 2075 7369 6e67 2066 696c 7465 7269  IS using filteri
-00001e40: 6e67 2063 7269 7465 7269 612e 0a20 2020  ng criteria..   
-00001e50: 2020 2020 203a 7061 7261 6d20 6669 6c74       :param filt
-00001e60: 6572 733a 2064 6963 7469 6f6e 6172 7920  ers: dictionary 
-00001e70: 6f66 2066 696c 7465 7220 7061 7261 6d65  of filter parame
-00001e80: 7465 7273 0a20 2020 2020 2020 203a 7061  ters.        :pa
-00001e90: 7261 6d20 7265 6375 7273 6976 653a 2046  ram recursive: F
-00001ea0: 6c61 6720 696e 6469 6361 7469 6e67 2069  lag indicating i
-00001eb0: 6620 7365 6172 6368 2073 686f 756c 6420  f search should 
-00001ec0: 696e 636c 7564 6520 6368 696c 6472 656e  include children
-00001ed0: 2072 6563 7572 7369 7665 6c79 0a20 2020   recursively.   
-00001ee0: 2020 2020 203a 7061 7261 6d20 7361 7665       :param save
-00001ef0: 3a20 4669 6c65 2070 6174 6820 746f 2073  : File path to s
-00001f00: 6176 6520 7265 7375 6c74 732e 2049 6620  ave results. If 
-00001f10: 6d69 7373 696e 672c 2073 6561 7263 6820  missing, search 
-00001f20: 7265 7375 6c74 7320 7769 6c6c 206e 6f74  results will not
-00001f30: 2062 6520 7361 7665 642e 0a20 2020 2020   be saved..     
-00001f40: 2020 204e 721f 0000 0072 6d00 0000 721f     Nr....rm...r.
-00001f50: 0000 0072 1f00 0000 7237 0000 00da 0f73  ...r....r7.....s
-00001f60: 6561 7263 685f 6461 7461 5f73 6574 f100  earch_data_set..
-00001f70: 0000 7252 0000 007a 2041 6273 7472 6163  ..rR...z Abstrac
-00001f80: 7444 6174 614d 676d 742e 7365 6172 6368  tDataMgmt.search
-00001f90: 5f64 6174 615f 7365 7463 0800 0000 0000  _data_setc......
-00001fa0: 0000 0000 0000 0c00 0000 0c00 0000 4300  ..............C.
-00001fb0: 0000 733e 0100 007c 0372 097c 01a0 0064  ..s>...|.r.|...d
-00001fc0: 0167 01a1 0101 006e 067c 01a0 0064 0267  .g.....n.|...d.g
-00001fd0: 01a1 0101 007c 01a0 01a1 007d 087c 0472  .....|.....}.|.r
-00001fe0: 197c 0864 0319 007d 087c 0574 026a 0375  .|.d...}.|.t.j.u
-00001ff0: 0072 5b7c 0664 0075 0072 3574 046a 057c  .r[|.d.u.r5t.j.|
-00002000: 0864 0464 0564 068d 037d 0974 0664 07a0  .d.d.d...}.t.d..
-00002010: 077c 09a1 0164 0864 098d 0201 0064 0053  .|...d.d.....d.S
-00002020: 007c 067c 0876 0172 4274 0864 0aa0 077c  .|.|.v.rBt.d...|
-00002030: 067c 016a 09a1 0283 0182 017c 067c 087c  .|.j.......|.|.|
-00002040: 0619 0069 017d 0a74 046a 057c 0a64 0464  ...i.}.t.j.|.d.d
-00002050: 0564 068d 037d 0974 0664 07a0 077c 09a1  .d...}.t.d...|..
-00002060: 0164 0864 098d 0201 0064 0053 007c 0574  .d.d.....d.S.|.t
-00002070: 026a 0a75 0072 6d74 0b64 0b7c 00a0 0c7c  .j.u.rmt.d.|...|
-00002080: 027c 017c 067c 077c 037c 04a1 0683 0253  .|.|.|.|.|.....S
-00002090: 007c 0574 026a 0d75 0072 9d7c 0664 0075  .|.t.j.u.r.|.d.u
-000020a0: 0072 9064 0c7d 0b7c 08a0 0ea1 0044 005d  .r.d.}.|.....D.]
-000020b0: 117d 067c 0b74 0b64 0b7c 00a0 0c7c 027c  .}.|.t.d.|...|.|
-000020c0: 017c 0664 007c 037c 04a1 0683 0237 007d  .|.d.|.|.....7.}
-000020d0: 0b71 7c7c 0b53 0074 0b64 0b7c 00a0 0c7c  .q||.S.t.d.|...|
-000020e0: 027c 017c 0664 007c 037c 04a1 0683 0253  .|.|.d.|.|.....S
-000020f0: 0064 0053 0029 0d4e da06 676c 6f62 616c  .d.S.).N..global
-00002100: da05 6c6f 6361 6cda 0a70 726f 7065 7274  ..local..propert
-00002110: 6965 73e9 0400 0000 5429 02da 0669 6e64  ies.....T)...ind
-00002120: 656e 74da 0973 6f72 745f 6b65 7973 7a02  ent..sort_keysz.
-00002130: 7b7d 4629 01da 0e77 6974 685f 7469 6d65  {}F)...with_time
-00002140: 7374 616d 707a 1a55 6e6b 6e6f 776e 2073  stampz.Unknown s
-00002150: 6574 7469 6e67 207b 7d20 666f 7220 7b7d  etting {} for {}
-00002160: 2e72 0400 0000 7201 0000 0029 0fda 1973  .r....r....)...s
-00002170: 6574 5f6c 6f63 6174 696f 6e5f 7365 6172  et_location_sear
-00002180: 6368 5f6f 7264 6572 7226 0000 0072 1200  ch_orderr&...r..
-00002190: 0000 da03 4745 54da 046a 736f 6eda 0564  ....GET..json..d
-000021a0: 756d 7073 7218 0000 0072 3e00 0000 723f  umpsr....r>...r?
-000021b0: 0000 00da 0863 6174 6567 6f74 79da 0353  .....categoty..S
-000021c0: 4554 7219 0000 00da 0c73 6574 5f70 726f  ETr......set_pro
-000021d0: 7065 7274 79da 0543 4c45 4152 da04 6b65  perty..CLEAR..ke
-000021e0: 7973 290c 723c 0000 00da 0872 6573 6f6c  ys).r<.....resol
-000021f0: 7665 7272 3300 0000 da09 6973 5f67 6c6f  verr3.....is_glo
-00002200: 6261 6cda 1469 735f 6461 7461 5f73 6574  bal..is_data_set
-00002210: 5f70 726f 7065 7274 79da 0e6f 7065 7261  _property..opera
-00002220: 7469 6f6e 5f74 7970 65da 0470 726f 70da  tion_type..prop.
-00002230: 0576 616c 7565 7226 0000 00da 0a63 6f6e  .valuer&.....con
-00002240: 6669 675f 7374 72da 0b6c 6974 746c 655f  fig_str..little_
-00002250: 6469 6374 da0b 7265 7475 726e 5f63 6f64  dict..return_cod
-00002260: 6572 1f00 0000 721f 0000 0072 3700 0000  er....r....r7...
-00002270: da0d 7570 6461 7465 5f63 6f6e 6669 67fa  ..update_config.
-00002280: 0000 0073 4e00 0000 0403 0e01 0c02 0802  ...sN...........
-00002290: 0401 0801 0a02 0801 1001 1601 0802 0201  ................
-000022a0: 0c01 04ff 0c02 1001 1601 0a01 0401 0e01  ................
-000022b0: 0201 02ff 04ff 0a03 0801 0401 0c01 0601  ................
-000022c0: 0c01 0401 02ff 08ff 0403 0402 0e01 0201  ................
-000022d0: 02ff 04ff 04f7 7a1e 4162 7374 7261 6374  ......z.Abstract
-000022e0: 4461 7461 4d67 6d74 2e75 7064 6174 655f  DataMgmt.update_
-000022f0: 636f 6e66 6967 6306 0000 0000 0000 0000  configc.........
-00002300: 0000 0008 0000 000a 0000 0043 0000 0073  ...........C...s
-00002310: 8e00 0000 7c04 7204 6401 6e01 6402 7d06  ....|.r.d.n.d.}.
-00002320: 7a18 7c05 7214 7c01 6a00 6403 7c02 7c03  z.|.r.|.j.d.|.|.
-00002330: 7c06 6404 6405 8d05 0100 6e09 7c01 6a01  |.d.d.....n.|.j.
-00002340: 7c02 7c03 7c06 6404 6405 8d04 0100 5700  |.|.|.d.d.....W.
-00002350: 6e22 0400 7402 7940 0100 7d07 0100 7a16  n"..t.y@..}...z.
-00002360: 7c00 6404 7500 722c 7c07 8201 7403 6406  |.d.u.r,|...t.d.
-00002370: 6407 7404 7c07 8301 1700 6408 8d02 5700  d.t.|.....d...W.
-00002380: 0600 5900 6409 7d07 7e07 5300 6409 7d07  ..Y.d.}.~.S.d.}.
-00002390: 7e07 7701 7700 7403 640a 640b 6408 8d02  ~.w.w.t.d.d.d...
-000023a0: 5300 290c 7a3c 4865 6c70 6572 2066 756e  S.).z<Helper fun
-000023b0: 6374 696f 6e20 746f 2069 6d70 6c65 6d65  ction to impleme
-000023c0: 6e74 2074 6865 2070 726f 7065 7274 7920  nt the property 
-000023d0: 7365 7474 696e 6720 7365 6d61 6e74 6963  setting semantic
-000023e0: 732e 7273 0000 0072 7400 0000 7275 0000  s.rs...rt...ru..
-000023f0: 0054 a901 da0b 6170 706c 795f 7275 6c65  .T....apply_rule
-00002400: 73e9 ffff ffff fa07 4572 726f 723a 20a9  s.......Error: .
-00002410: 02da 0a72 6574 7572 6e63 6f64 65da 066f  ...returncode..o
-00002420: 7574 7075 744e 7201 0000 00da 0029 05da  utputNr......)..
-00002430: 1c73 6574 5f76 616c 7565 5f66 6f72 5f6a  .set_value_for_j
-00002440: 736f 6e5f 7061 7261 6d65 7465 72da 1773  son_parameter..s
-00002450: 6574 5f76 616c 7565 5f66 6f72 5f70 6172  et_value_for_par
-00002460: 616d 6574 6572 da09 4578 6365 7074 696f  ameter..Exceptio
-00002470: 6e72 0500 0000 da03 7374 7229 0872 3300  nr......str).r3.
-00002480: 0000 7283 0000 0072 8700 0000 7288 0000  ..r....r....r...
-00002490: 0072 8400 0000 7285 0000 00da 036c 6f63  .r....r......loc
-000024a0: da01 6572 1f00 0000 721f 0000 0072 3700  ..er....r....r7.
-000024b0: 0000 7280 0000 0022 0100 0073 1e00 0000  ..r...."...s....
-000024c0: 0c03 0201 0401 0c01 0201 08ff 1203 0480  ................
-000024d0: 0e01 0801 0401 2001 0880 02fd 0c05 7a1d  ...... .......z.
-000024e0: 4162 7374 7261 6374 4461 7461 4d67 6d74  AbstractDataMgmt
-000024f0: 2e73 6574 5f70 726f 7065 7274 7929 0246  .set_property).F
-00002500: 54a9 014e a902 5454 a902 4e4e 2901 4629  T..N..TT..NN).F)
-00002510: 1ada 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00002520: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00002530: 616d 655f 5fda 075f 5f64 6f63 5f5f 723d  ame__..__doc__r=
-00002540: 0000 0072 4300 0000 da03 6162 63da 0e61  ...rC.....abc..a
-00002550: 6273 7472 6163 746d 6574 686f 6472 4600  bstractmethodrF.
-00002560: 0000 724a 0000 0072 4d00 0000 7251 0000  ..rJ...rM...rQ..
-00002570: 0072 5700 0000 7256 0000 0072 5800 0000  .rW...rV...rX...
-00002580: 725f 0000 0072 6100 0000 7262 0000 0072  r_...ra...rb...r
-00002590: 6400 0000 7268 0000 0072 6c00 0000 7271  d...rh...rl...rq
-000025a0: 0000 0072 7200 0000 728c 0000 00da 0c73  ...rr...r......s
-000025b0: 7461 7469 636d 6574 686f 6472 8000 0000  taticmethodr....
-000025c0: 721f 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
-000025d0: 3700 0000 7239 0000 005b 0000 0073 5000  7...r9...[...sP.
-000025e0: 0000 0800 0401 0206 0aff 0811 0405 0a01  ................
-000025f0: 0404 0a01 0404 0c01 0409 0c01 0408 0c01  ................
-00002600: 040b 0a01 0408 0a01 0406 0a01 040a 0a01  ................
-00002610: 040a 0a01 0406 0c01 0407 0a01 0409 0a01  ................
-00002620: 0408 0a01 0408 0a01 0209 0201 0afe 0228  ...............(
-00002630: 1001 7239 0000 0029 01da 096d 6574 6163  ..r9...)...metac
-00002640: 6c61 7373 6300 0000 0000 0000 0000 0000  lassc...........
-00002650: 0000 0000 0003 0000 0040 0000 0073 9000  .........@...s..
-00002660: 0000 6500 5a01 6400 5a02 6401 5a03 6402  ..e.Z.d.Z.d.Z.d.
-00002670: 6403 8400 5a04 6404 6405 8400 5a05 6422  d...Z.d.d...Z.d"
-00002680: 6407 6408 8401 5a06 6422 6409 640a 8401  d.d...Z.d"d.d...
-00002690: 5a07 6423 640c 640d 8401 5a08 640e 640f  Z.d#d.d...Z.d.d.
-000026a0: 8400 5a09 6410 6411 8400 5a0a 6412 6413  ..Z.d.d...Z.d.d.
-000026b0: 8400 5a0b 6414 6415 8400 5a0c 6416 6417  ..Z.d.d...Z.d.d.
-000026c0: 8400 5a0d 6422 6418 6419 8401 5a0e 641a  ..Z.d"d.d...Z.d.
-000026d0: 641b 8400 5a0f 641c 641d 8400 5a10 641e  d...Z.d.d...Z.d.
-000026e0: 641f 8400 5a11 6420 6421 8400 5a12 6406  d...Z.d d!..Z.d.
-000026f0: 5300 2924 722b 0000 007a 4544 6174 614d  S.)$r+...zEDataM
-00002700: 676d 7420 6f70 6572 6174 696f 6e73 2077  gmt operations w
-00002710: 6865 6e20 6769 7420 6973 206e 6f74 2061  hen git is not a
-00002720: 7661 696c 6162 6c65 202d 2d20 7368 6f77  vailable -- show
-00002730: 2065 7272 6f72 206d 6573 7361 6765 732e   error messages.
-00002740: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00002750: 0004 0000 0043 0000 00f3 1000 0000 7c00  .....C........|.
-00002760: a000 6401 6402 a102 0100 6400 5300 2903  ..d.d.....d.S.).
-00002770: 4e7a 1567 6574 2073 6574 7469 6e67 7320  Nz.get settings 
-00002780: 7265 736f 6c76 6572 fa15 4e6f 2067 6974  resolver..No git
-00002790: 2063 6f6d 6d61 6e64 2066 6f75 6e64 2ea9   command found..
-000027a0: 0172 4300 0000 7245 0000 0072 1f00 0000  .rC...rE...r....
-000027b0: 721f 0000 0072 3700 0000 7246 0000 0037  r....r7...rF...7
-000027c0: 0100 00f3 0200 0000 1001 7a23 4e6f 4769  ..........z#NoGi
-000027d0: 7444 6174 614d 676d 742e 6765 745f 7365  tDataMgmt.get_se
-000027e0: 7474 696e 6773 5f72 6573 6f6c 7665 7263  ttings_resolverc
-000027f0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00002800: 0400 0000 4300 0000 72a6 0000 0029 034e  ....C...r....).N
-00002810: fa14 7365 7475 7020 6c6f 6361 6c20 7365  ..setup local se
-00002820: 7474 696e 6773 72a7 0000 0072 a800 0000  ttingsr....r....
-00002830: 7248 0000 0072 1f00 0000 721f 0000 0072  rH...r....r....r
-00002840: 3700 0000 724a 0000 003a 0100 0072 a900  7...rJ...:...r..
-00002850: 0000 7a22 4e6f 4769 7444 6174 614d 676d  ..z"NoGitDataMgm
-00002860: 742e 7365 7475 705f 6c6f 6361 6c5f 7365  t.setup_local_se
-00002870: 7474 696e 6773 4e63 0200 0000 0000 0000  ttingsNc........
-00002880: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
-00002890: 72a6 0000 0029 034e 7a09 696e 6974 2064  r....).Nz.init d
-000028a0: 6174 6172 a700 0000 72a8 0000 0072 4b00  atar....r....rK.
-000028b0: 0000 721f 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
-000028c0: 0072 4d00 0000 3d01 0000 72a9 0000 007a  .rM...=...r....z
-000028d0: 174e 6f47 6974 4461 7461 4d67 6d74 2e69  .NoGitDataMgmt.i
-000028e0: 6e69 745f 6461 7461 6303 0000 0000 0000  nit_datac.......
-000028f0: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
-00002900: 0072 a600 0000 2903 4efa 0d69 6e69 7420  .r....).N..init 
-00002910: 616e 616c 7973 6973 72a7 0000 0072 a800  analysisr....r..
-00002920: 0000 724f 0000 0072 1f00 0000 721f 0000  ..rO...r....r...
-00002930: 0072 3700 0000 7251 0000 0040 0100 0072  .r7...rQ...@...r
-00002940: a900 0000 7a1b 4e6f 4769 7444 6174 614d  ....z.NoGitDataM
-00002950: 676d 742e 696e 6974 5f61 6e61 6c79 7369  gmt.init_analysi
-00002960: 7354 6304 0000 0000 0000 0000 0000 0004  sTc.............
-00002970: 0000 0004 0000 0043 0000 0072 a600 0000  .......C...r....
-00002980: 2903 4e72 5700 0000 72a7 0000 0072 a800  ).NrW...r....r..
-00002990: 0000 7253 0000 0072 1f00 0000 721f 0000  ..rS...r....r...
-000029a0: 0072 3700 0000 7257 0000 0043 0100 0072  .r7...rW...C...r
-000029b0: a900 0000 7a14 4e6f 4769 7444 6174 614d  ....z.NoGitDataM
-000029c0: 676d 742e 636f 6d6d 6974 6301 0000 0000  gmt.commitc.....
-000029d0: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-000029e0: 0000 0072 a600 0000 2903 4e72 5600 0000  ...r....).NrV...
-000029f0: 72a7 0000 0072 a800 0000 7245 0000 0072  r....r....rE...r
-00002a00: 1f00 0000 721f 0000 0072 3700 0000 7256  ....r....r7...rV
-00002a10: 0000 0046 0100 0072 a900 0000 7a12 4e6f  ...F...r....z.No
-00002a20: 4769 7444 6174 614d 676d 742e 7379 6e63  GitDataMgmt.sync
-00002a30: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00002a40: 0004 0000 0043 0000 0072 a600 0000 2903  .....C...r....).
-00002a50: 4e72 5800 0000 72a7 0000 0072 a800 0000  NrX...r....r....
-00002a60: 7245 0000 0072 1f00 0000 721f 0000 0072  rE...r....r....r
-00002a70: 3700 0000 7258 0000 0049 0100 0072 a900  7...rX...I...r..
-00002a80: 0000 7a14 4e6f 4769 7444 6174 614d 676d  ..z.NoGitDataMgm
-00002a90: 742e 7374 6174 7573 6305 0000 0000 0000  t.statusc.......
-00002aa0: 0000 0000 0005 0000 0004 0000 0043 0000  .............C..
-00002ab0: 0072 a600 0000 2903 4e72 5f00 0000 72a7  .r....).Nr_...r.
-00002ac0: 0000 0072 a800 0000 725a 0000 0072 1f00  ...r....rZ...r..
-00002ad0: 0000 721f 0000 0072 3700 0000 725f 0000  ..r....r7...r_..
-00002ae0: 004c 0100 0072 a900 0000 7a13 4e6f 4769  .L...r....z.NoGi
-00002af0: 7444 6174 614d 676d 742e 636c 6f6e 6563  tDataMgmt.clonec
-00002b00: 0500 0000 0000 0000 0000 0000 0500 0000  ................
-00002b10: 0400 0000 4300 0000 72a6 0000 0029 034e  ....C...r....).N
-00002b20: 7261 0000 0072 a700 0000 72a8 0000 0072  ra...r....r....r
-00002b30: 5a00 0000 721f 0000 0072 1f00 0000 7237  Z...r....r....r7
-00002b40: 0000 0072 6100 0000 4f01 0000 72a9 0000  ...ra...O...r...
-00002b50: 007a 124e 6f47 6974 4461 7461 4d67 6d74  .z.NoGitDataMgmt
-00002b60: 2e6d 6f76 6563 0100 0000 0000 0000 0000  .movec..........
-00002b70: 0000 0100 0000 0400 0000 4300 0000 72a6  ..........C...r.
-00002b80: 0000 0029 034e 7262 0000 0072 a700 0000  ...).Nrb...r....
-00002b90: 72a8 0000 0072 4500 0000 721f 0000 0072  r....rE...r....r
-00002ba0: 1f00 0000 7237 0000 0072 6200 0000 5201  ....r7...rb...R.
-00002bb0: 0000 72a9 0000 007a 144e 6f47 6974 4461  ..r....z.NoGitDa
-00002bc0: 7461 4d67 6d74 2e61 6464 7265 6663 0200  taMgmt.addrefc..
-00002bd0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00002be0: 0000 4300 0000 72a6 0000 0029 034e 7264  ..C...r....).Nrd
-00002bf0: 0000 0072 a700 0000 72a8 0000 0072 6300  ...r....r....rc.
-00002c00: 0000 721f 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
-00002c10: 0072 6400 0000 5501 0000 72a9 0000 007a  .rd...U...r....z
-00002c20: 174e 6f47 6974 4461 7461 4d67 6d74 2e72  .NoGitDataMgmt.r
-00002c30: 656d 6f76 6572 6566 6301 0000 0000 0000  emoverefc.......
-00002c40: 0000 0000 0002 0000 0004 0000 0047 0000  .............G..
-00002c50: 0072 a600 0000 2903 4e72 6800 0000 72a7  .r....).Nrh...r.
-00002c60: 0000 0072 a800 0000 a902 723c 0000 00da  ...r......r<....
-00002c70: 015f 721f 0000 0072 1f00 0000 7237 0000  ._r....r....r7..
-00002c80: 0072 6800 0000 5801 0000 72a9 0000 007a  .rh...X...r....z
-00002c90: 164e 6f47 6974 4461 7461 4d67 6d74 2e64  .NoGitDataMgmt.d
-00002ca0: 6f77 6e6c 6f61 6463 0100 0000 0000 0000  ownloadc........
-00002cb0: 0000 0000 0200 0000 0400 0000 4700 0000  ............G...
-00002cc0: 72a6 0000 00a9 034e da06 7365 6172 6368  r......N..search
-00002cd0: 72a7 0000 0072 a800 0000 72ac 0000 0072  r....r....r....r
-00002ce0: 1f00 0000 721f 0000 0072 3700 0000 7271  ....r....r7...rq
-00002cf0: 0000 005b 0100 0072 a900 0000 7a1b 4e6f  ...[...r....z.No
-00002d00: 4769 7444 6174 614d 676d 742e 7365 6172  GitDataMgmt.sear
-00002d10: 6368 5f6f 626a 6563 7463 0100 0000 0000  ch_objectc......
-00002d20: 0000 0000 0000 0200 0000 0400 0000 4700  ..............G.
-00002d30: 0000 72a6 0000 0072 ae00 0000 72a8 0000  ..r....r....r...
-00002d40: 0072 ac00 0000 721f 0000 0072 1f00 0000  .r....r....r....
-00002d50: 7237 0000 0072 7200 0000 5e01 0000 72a9  r7...rr...^...r.
-00002d60: 0000 007a 1d4e 6f47 6974 4461 7461 4d67  ...z.NoGitDataMg
-00002d70: 6d74 2e73 6561 7263 685f 6461 7461 5f73  mt.search_data_s
-00002d80: 6574 6301 0000 0000 0000 0000 0000 0002  etc.............
-00002d90: 0000 0004 0000 0047 0000 0072 a600 0000  .......G...r....
-00002da0: 2903 4e72 6c00 0000 72a7 0000 0072 a800  ).Nrl...r....r..
-00002db0: 0000 72ac 0000 0072 1f00 0000 721f 0000  ..r....r....r...
-00002dc0: 0072 3700 0000 726c 0000 0061 0100 0072  .r7...rl...a...r
-00002dd0: a900 0000 7a14 4e6f 4769 7444 6174 614d  ....z.NoGitDataM
-00002de0: 676d 742e 7570 6c6f 6164 729b 0000 0072  gmt.uploadr....r
-00002df0: 9c00 0000 2913 729e 0000 0072 9f00 0000  ....).r....r....
-00002e00: 72a0 0000 0072 a100 0000 7246 0000 0072  r....r....rF...r
-00002e10: 4a00 0000 724d 0000 0072 5100 0000 7257  J...rM...rQ...rW
-00002e20: 0000 0072 5600 0000 7258 0000 0072 5f00  ...rV...rX...r_.
-00002e30: 0000 7261 0000 0072 6200 0000 7264 0000  ..ra...rb...rd..
-00002e40: 0072 6800 0000 7271 0000 0072 7200 0000  .rh...rq...rr...
-00002e50: 726c 0000 0072 1f00 0000 721f 0000 0072  rl...r....r....r
-00002e60: 1f00 0000 7237 0000 0072 2b00 0000 3401  ....r7...r+...4.
-00002e70: 0000 7322 0000 0008 0004 0108 0208 030a  ..s"............
-00002e80: 030a 030a 0308 0308 0308 0308 0308 030a  ................
-00002e90: 0308 0308 0308 030c 0372 2b00 0000 6301  .........r+...c.
-00002ea0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00002eb0: 0000 0043 0000 0073 1600 0000 7c00 a000  ...C...s....|...
-00002ec0: a100 0100 7401 a002 6401 a101 0100 6400  ....t...d.....d.
-00002ed0: 5300 2902 4e72 0100 0000 2903 da07 7265  S.).Nr....)...re
-00002ee0: 7374 6f72 65da 0373 7973 da04 6578 6974  store..sys..exit
-00002ef0: 2901 da09 6461 7461 5f6d 676d 7472 1f00  )...data_mgmtr..
-00002f00: 0000 721f 0000 0072 3700 0000 da16 7265  ..r....r7.....re
-00002f10: 7374 6f72 655f 7369 676e 616c 5f68 616e  store_signal_han
-00002f20: 646c 6572 6501 0000 7304 0000 0008 010e  dlere...s.......
-00002f30: 0172 b400 0000 6301 0000 0000 0000 0000  .r....c.........
-00002f40: 0000 0002 0000 0003 0000 0003 0000 00f3  ................
-00002f50: 1000 0000 8700 6601 6401 6402 8408 7d01  ......f.d.d...}.
-00002f60: 7c01 5300 2903 7a33 2054 6f20 6265 2075  |.S.).z3 To be u
-00002f70: 7365 6420 7769 7468 2063 6f6d 6d61 6e64  sed with command
-00002f80: 7320 7468 6174 2075 7365 2074 6865 2043  s that use the C
-00002f90: 6f6d 6d61 6e64 4c6f 672e 2063 0100 0000  ommandLog. c....
-00002fa0: 0000 0000 0000 0000 0400 0000 0a00 0000  ................
-00002fb0: 1700 0000 736e 0000 007a 0a88 007c 0067  ....sn...z...|.g
-00002fc0: 017c 01a2 0152 008e 007d 0257 006e 1604  .|...R...}.W.n..
-00002fd0: 0074 0079 2001 007d 0301 007a 0a7c 006a  .t.y ..}...z.|.j
-00002fe0: 01a0 0274 037c 0383 01a1 0101 007c 0382  ...t.|.......|..
-00002ff0: 0164 007d 037e 0377 0177 007c 02a0 04a1  .d.}.~.w.w.|....
-00003000: 0064 016b 0272 2e7c 006a 01a0 05a1 0001  .d.k.r.|.j......
-00003010: 007c 0253 007c 006a 01a0 027c 026a 06a1  .|.S.|.j...|.j..
-00003020: 0101 007c 0253 0029 024e 4629 0772 9700  ...|.S.).NF).r..
-00003030: 0000 7232 0000 00da 096c 6f67 5f65 7272  ..r2.....log_err
-00003040: 6f72 7298 0000 00da 0766 6169 6c75 7265  orr......failure
-00003050: da07 7375 6363 6573 7372 9300 0000 a904  ..successr......
-00003060: 723c 0000 00da 0461 7267 73da 0672 6573  r<.....args..res
-00003070: 756c 7472 9a00 0000 a901 da01 6672 1f00  ultr........fr..
-00003080: 0000 7237 0000 00da 0a66 5f77 6974 685f  ..r7.....f_with_
-00003090: 6c6f 676d 0100 0073 1800 0000 0201 1401  logm...s........
-000030a0: 0e01 1001 0401 0880 02fe 0c03 0a01 0403  ................
-000030b0: 0eff 0401 7a1c 7769 7468 5f6c 6f67 2e3c  ....z.with_log.<
-000030c0: 6c6f 6361 6c73 3e2e 665f 7769 7468 5f6c  locals>.f_with_l
-000030d0: 6f67 721f 0000 0029 0272 bd00 0000 72be  ogr....).r....r.
-000030e0: 0000 0072 1f00 0000 72bc 0000 0072 3700  ...r....r....r7.
-000030f0: 0000 da08 7769 7468 5f6c 6f67 6a01 0000  ....with_logj...
-00003100: 7304 0000 000c 0304 0c72 bf00 0000 6301  s........r....c.
-00003110: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00003120: 0000 0003 0000 0072 b500 0000 2903 7a2f  .......r....).z/
-00003130: 2053 6574 7320 7468 6520 7265 7374 6f72   Sets the restor
-00003140: 6520 706f 696e 7420 616e 6420 7265 7374  e point and rest
-00003150: 6f72 6573 206f 6e20 6572 726f 722e 2063  ores on error. c
-00003160: 0100 0000 0000 0000 0000 0000 0400 0000  ................
-00003170: 0a00 0000 1700 0000 73aa 0000 0088 00a0  ........s.......
-00003180: 00a1 0001 007a 2588 006a 0172 1374 02a0  .....z%..j.r.t..
-00003190: 0274 026a 0387 0066 0164 0164 0284 08a1  .t.j...f.d.d....
-000031a0: 0201 0088 0188 0067 017c 01a2 0152 008e  .......g.|...R..
-000031b0: 007d 027c 02a0 04a1 0072 2388 00a0 05a1  .}.|.....r#.....
-000031c0: 0001 0088 00a0 06a1 0001 007c 0257 0053  ...........|.W.S
-000031d0: 0004 0074 0779 5401 007d 0301 007a 1f88  ...t.yT..}...z..
-000031e0: 00a0 05a1 0001 0088 006a 0864 036b 0272  .........j.d.k.r
-000031f0: 3c7c 0382 0188 00a0 06a1 0001 0074 0964  <|...........t.d
-00003200: 0464 0574 0a7c 0383 0117 0064 068d 0257  .d.t.|.....d...W
-00003210: 0006 0059 0064 007d 037e 0353 0064 007d  ...Y.d.}.~.S.d.}
-00003220: 037e 0377 0177 0029 074e 6302 0000 0000  .~.w.w.).Nc.....
-00003230: 0000 0000 0000 0002 0000 0002 0000 0013  ................
-00003240: 0000 0073 0800 0000 7400 8800 8301 5300  ...s....t.....S.
-00003250: 729b 0000 0029 0172 b400 0000 2902 da06  r....).r....)...
-00003260: 7369 676e 616c da05 6672 616d 6572 4500  signal..framerE.
-00003270: 0000 721f 0000 0072 3700 0000 da08 3c6c  ..r....r7.....<l
-00003280: 616d 6264 613e 8301 0000 7302 0000 0008  ambda>....s.....
-00003290: 007a 3677 6974 685f 7265 7374 6f72 652e  .z6with_restore.
-000032a0: 3c6c 6f63 616c 733e 2e66 5f77 6974 685f  <locals>.f_with_
-000032b0: 7265 7374 6f72 652e 3c6c 6f63 616c 733e  restore.<locals>
-000032c0: 2e3c 6c61 6d62 6461 3e54 728f 0000 0072  .<lambda>Tr....r
-000032d0: 9000 0000 7291 0000 0029 0bda 1073 6574  ....r....)...set
-000032e0: 5f72 6573 746f 7265 706f 696e 7472 3a00  _restorepointr:.
-000032f0: 0000 72c0 0000 00da 0653 4947 494e 5472  ..r......SIGINTr
-00003300: b700 0000 72b0 0000 00da 1263 6c65 6172  ....r......clear
-00003310: 5f72 6573 746f 7265 706f 696e 7472 9700  _restorepointr..
-00003320: 0000 7233 0000 0072 0500 0000 7298 0000  ..r3...r....r...
-00003330: 0072 b900 0000 72bc 0000 0072 4500 0000  .r....r....rE...
-00003340: 7237 0000 00da 0e66 5f77 6974 685f 7265  r7.....f_with_re
-00003350: 7374 6f72 657f 0100 0073 2200 0000 0801  store....s".....
-00003360: 0201 0601 1601 1001 0801 0801 0801 0601  ................
-00003370: 0e01 0801 0a01 0401 0801 2001 0880 02fb  .......... .....
-00003380: 7a24 7769 7468 5f72 6573 746f 7265 2e3c  z$with_restore.<
-00003390: 6c6f 6361 6c73 3e2e 665f 7769 7468 5f72  locals>.f_with_r
-000033a0: 6573 746f 7265 721f 0000 0029 0272 bd00  estorer....).r..
-000033b0: 0000 72c6 0000 0072 1f00 0000 72bc 0000  ..r....r....r...
-000033c0: 0072 3700 0000 da0c 7769 7468 5f72 6573  .r7.....with_res
-000033d0: 746f 7265 7c01 0000 7304 0000 000c 0304  tore|...s.......
-000033e0: 1172 c700 0000 6300 0000 0000 0000 0000  .r....c.........
-000033f0: 0000 0000 0000 0004 0000 0040 0000 0073  ...........@...s
-00003400: dc00 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
-00003410: 6430 6403 6404 8401 5a04 6405 6406 8400  d0d.d...Z.d.d...
-00003420: 5a05 6407 6408 8400 5a06 6409 640a 8400  Z.d.d...Z.d.d...
-00003430: 5a07 6430 640b 640c 8401 5a08 6430 640d  Z.d0d.d...Z.d0d.
-00003440: 640e 8401 5a09 650a 640f 6410 8400 8301  d...Z.e.d.d.....
-00003450: 5a0b 6411 6412 8400 5a0c 650a 6431 6414  Z.d.d...Z.e.d1d.
-00003460: 6415 8401 8301 5a0d 6416 6417 8400 5a0e  d.....Z.d.d...Z.
-00003470: 6418 6419 8400 5a0f 641a 641b 8400 5a10  d.d...Z.d.d...Z.
-00003480: 641c 641d 8400 5a11 641e 641f 8400 5a12  d.d...Z.d.d...Z.
-00003490: 6513 6420 6421 8400 8301 5a14 6422 6423  e.d d!....Z.d"d#
-000034a0: 8400 5a15 6430 6424 6425 8401 5a16 6426  ..Z.d0d$d%..Z.d&
-000034b0: 6427 8400 5a17 0902 0902 6432 6428 6429  d'..Z.....d2d(d)
-000034c0: 8401 5a18 642a 642b 8400 5a19 642c 642d  ..Z.d*d+..Z.d,d-
-000034d0: 8400 5a1a 642e 642f 8400 5a1b 6402 5300  ..Z.d.d/..Z.d.S.
-000034e0: 2933 722c 0000 007a 2444 6174 614d 676d  )3r,...z$DataMgm
-000034f0: 7420 6f70 6572 6174 696f 6e73 2069 6e20  t operations in 
-00003500: 6e6f 726d 616c 2073 7461 7465 2e4e 6302  normal state.Nc.
-00003510: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00003520: 0000 0043 0000 0073 2600 0000 7c01 6400  ...C...s&...|.d.
-00003530: 7500 7207 7c00 6a00 5300 7401 a002 a100  u.r.|.j.S.t.....
-00003540: 7d02 7c02 a003 6401 7c01 a102 0100 7c02  }.|...d.|.....|.
-00003550: 5300 2902 4eda 0864 6174 615f 7365 7429  S.).N..data_set)
-00003560: 0472 2e00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-00003570: da1b 7365 745f 7265 736f 6c76 6572 5f6c  ..set_resolver_l
-00003580: 6f63 6174 696f 6e5f 726f 6f74 73a9 0372  ocation_roots..r
-00003590: 3c00 0000 da0d 7265 6c61 7469 7665 5f70  <.....relative_p
-000035a0: 6174 6872 2e00 0000 721f 0000 0072 1f00  athr....r....r..
-000035b0: 0000 7237 0000 0072 4600 0000 9601 0000  ..r7...rF.......
-000035c0: 730a 0000 0008 0106 0108 020c 0104 017a  s..............z
-000035d0: 2147 6974 4461 7461 4d67 6d74 2e67 6574  !GitDataMgmt.get
-000035e0: 5f73 6574 7469 6e67 735f 7265 736f 6c76  _settings_resolv
-000035f0: 6572 6302 0000 0000 0000 0000 0000 0007  erc.............
-00003600: 0000 0007 0000 0043 0000 0073 5000 0000  .......C...sP...
-00003610: 7c00 6a00 a001 6401 6402 a102 0100 7c01  |.j...d.d.....|.
-00003620: a002 a100 4400 5d1a 5c02 7d02 7d03 7403  ....D.].\.}.}.t.
-00003630: 7c00 6a00 7c02 8302 7d04 7c03 a002 a100  |.j.|...}.|.....
-00003640: 4400 5d0b 5c02 7d05 7d06 7c04 a004 7c05  D.].\.}.}.|...|.
-00003650: 7c06 6403 a103 0100 7119 710b 6400 5300  |.d.....q.q.d.S.
-00003660: 2904 4e72 c800 0000 da01 2e72 7400 0000  ).Nr.......rt...
-00003670: 2905 722e 0000 0072 c900 0000 da05 6974  ).r....r......it
-00003680: 656d 73da 0767 6574 6174 7472 7296 0000  ems..getattrr...
-00003690: 0029 0772 3c00 0000 7249 0000 00da 0d72  .).r<...rI.....r
-000036a0: 6573 6f6c 7665 725f 7479 7065 da08 7365  esolver_type..se
-000036b0: 7474 696e 6773 7283 0000 00da 036b 6579  ttingsr......key
-000036c0: 7288 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
-000036d0: 3700 0000 724a 0000 009f 0100 0073 0e00  7...rJ.......s..
-000036e0: 0000 0e01 1001 0c01 1001 1001 02ff 04fe  ................
-000036f0: 7a20 4769 7444 6174 614d 676d 742e 7365  z GitDataMgmt.se
-00003700: 7475 705f 6c6f 6361 6c5f 7365 7474 696e  tup_local_settin
-00003710: 6773 6302 0000 0000 0000 0000 0000 0003  gsc.............
-00003720: 0000 0003 0000 0043 0000 00f3 1a00 0000  .......C........
-00003730: 7c00 a000 7c01 a101 7d02 7c02 6a01 a002  |...|...}.|.j...
-00003740: a100 a003 6401 a101 5300 2902 4e72 5b00  ....d...S.).Nr[.
-00003750: 0000 a904 7246 0000 00da 0a72 6570 6f73  ....rF.....repos
-00003760: 6974 6f72 7972 2600 0000 da03 6765 7472  itoryr&.....getr
-00003770: ca00 0000 721f 0000 0072 1f00 0000 7237  ....r....r....r7
-00003780: 0000 00da 0f67 6574 5f64 6174 615f 7365  .....get_data_se
-00003790: 745f 6964 a601 0000 f304 0000 000a 0110  t_id............
-000037a0: 017a 1b47 6974 4461 7461 4d67 6d74 2e67  .z.GitDataMgmt.g
-000037b0: 6574 5f64 6174 615f 7365 745f 6964 6302  et_data_set_idc.
-000037c0: 0000 0000 0000 0000 0000 0003 0000 0003  ................
-000037d0: 0000 0043 0000 0072 d200 0000 2902 4eda  ...C...r....).N.
-000037e0: 0269 6472 d300 0000 72ca 0000 0072 1f00  .idr....r....r..
-000037f0: 0000 721f 0000 0072 3700 0000 da11 6765  ..r....r7.....ge
-00003800: 745f 7265 706f 7369 746f 7279 5f69 64aa  t_repository_id.
-00003810: 0100 0072 d700 0000 7a1d 4769 7444 6174  ...r....z.GitDat
-00003820: 614d 676d 742e 6765 745f 7265 706f 7369  aMgmt.get_reposi
-00003830: 746f 7279 5f69 6463 0200 0000 0000 0000  tory_idc........
-00003840: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
-00003850: 7394 0000 0074 006a 01a0 0264 01a1 0172  s....t.j...d...r
-00003860: 0c74 0364 0264 0364 048d 0253 007c 006a  .t.d.d.d...S.|.j
-00003870: 04a0 05a1 007d 027c 02a0 06a1 0072 177c  .....}.|.....r.|
-00003880: 0253 007c 006a 076a 08a0 09a1 00a0 0a64  .S.|.j.j.......d
-00003890: 05a1 017d 037c 006a 04a0 0b7c 017c 03a1  ...}.|.j...|.|..
-000038a0: 027d 027c 02a0 06a1 0072 2d7c 0253 007c  .}.|.....r-|.S.|
-000038b0: 006a 04a0 0ca1 007d 027c 02a0 06a1 0072  .j.....}.|.....r
-000038c0: 387c 0253 007c 006a 07a0 0d64 0664 07a1  8|.S.|.j...d.d..
-000038d0: 0201 007c 006a 07a0 0ea1 0001 0074 0364  ...|.j.......t.d
-000038e0: 0864 0964 048d 0253 0029 0a4e 721d 0000  .d.d...S.).Nr...
-000038f0: 0072 8f00 0000 fa25 466f 6c64 6572 2069  .r.....%Folder i
-00003900: 7320 616c 7265 6164 7920 616e 206f 6269  s already an obi
-00003910: 7320 7265 706f 7369 746f 7279 2e72 9100  s repository.r..
-00003920: 0000 da11 6769 745f 616e 6e65 785f 6261  ....git_annex_ba
-00003930: 636b 656e 6472 c800 0000 72cc 0000 0072  ckendr....r....r
-00003940: 0100 0000 7294 0000 0029 0f72 2300 0000  ....r....).r#...
-00003950: 7224 0000 0072 2500 0000 7205 0000 0072  r$...r%...r....r
-00003960: 3600 0000 da08 6769 745f 696e 6974 72b7  6.....git_initr.
-00003970: 0000 0072 2e00 0000 7204 0000 0072 2600  ...r....r....r&.
-00003980: 0000 72d5 0000 00da 0e67 6974 5f61 6e6e  ..r......git_ann
-00003990: 6578 5f69 6e69 74da 0e69 6e69 7469 616c  ex_init..initial
-000039a0: 5f63 6f6d 6d69 7472 c900 0000 da14 636f  _commitr......co
-000039b0: 7079 5f67 6c6f 6261 6c5f 746f 5f6c 6f63  py_global_to_loc
-000039c0: 616c 2904 723c 0000 0072 4c00 0000 72bb  al).r<...rL...r.
-000039d0: 0000 0072 db00 0000 721f 0000 0072 1f00  ...r....r....r..
-000039e0: 0000 7237 0000 0072 4d00 0000 ae01 0000  ..r7...rM.......
-000039f0: 731e 0000 000c 020c 010a 0108 0104 0112  s...............
-00003a00: 010e 0108 0104 010a 0108 0104 010e 020a  ................
-00003a10: 010c 017a 1547 6974 4461 7461 4d67 6d74  ...z.GitDataMgmt
-00003a20: 2e69 6e69 745f 6461 7461 6303 0000 0000  .init_datac.....
-00003a30: 0000 0000 0000 0009 0000 000a 0000 0043  ...............C
-00003a40: 0000 0073 1601 0000 7c00 a000 7c01 a101  ...s....|...|...
-00003a50: 7d03 7c00 a001 7c01 a101 6400 7500 7212  }.|...|...d.u.r.
-00003a60: 7402 6401 6402 6403 8d02 5300 7c00 a003  t.d.d.d...S.|...
-00003a70: 7c02 a101 7d04 7c04 a004 a100 721d 7c04  |...}.|.....r.|.
-00003a80: 5300 7405 6a06 a007 7405 a008 a100 7c01  S.t.j...t.....|.
-00003a90: a102 7d05 7405 a008 a100 7d06 7409 7c06  ..}.t.....}.t.|.
-00003aa0: 8301 7409 7c05 8301 6a0a 7600 7254 7405  ..t.|...j.v.rTt.
-00003ab0: 6a06 a00b 7c06 7c05 a102 7d07 740c 7c01  j...|.|...}.t.|.
-00003ac0: 8301 8f0e 0100 7c00 6a0d a00e 7c07 a101  ......|.j...|...
-00003ad0: 0100 5700 6400 0400 0400 8303 0100 6e08  ..W.d.........n.
-00003ae0: 3100 734f 7701 0100 0100 0100 5900 0100  1.sOw.......Y...
-00003af0: 7a0d 7c00 6a0f 6a10 6a11 6404 7c03 6405  z.|.j.j.j.d.|.d.
-00003b00: 6406 6407 8d04 0100 5700 6e23 0400 7412  d.d.....W.n#..t.
-00003b10: 7984 0100 7d08 0100 7a17 7c00 6a13 6406  y...}...z.|.j.d.
-00003b20: 7500 7270 7c08 8201 7402 6401 6408 7414  u.rp|...t.d.d.t.
-00003b30: 7c08 8301 1700 6403 8d02 5700 0600 5900  |.....d...W...Y.
-00003b40: 6400 7d08 7e08 5300 6400 7d08 7e08 7701  d.}.~.S.d.}.~.w.
-00003b50: 7700 7402 6409 640a 6403 8d02 5300 290b  w.t.d.d.d...S.).
-00003b60: 4e72 8f00 0000 7a52 5061 7265 6e74 2064  Nr....zRParent d
-00003b70: 6174 6120 7365 7420 6d75 7374 2062 6520  ata set must be 
-00003b80: 636f 6d6d 6974 7465 6420 746f 206f 7065  committed to ope
-00003b90: 6e42 4953 2062 6566 6f72 6520 6372 6561  nBIS before crea
-00003ba0: 7469 6e67 2061 6e20 616e 616c 7973 6973  ting an analysis
-00003bb0: 2064 6174 6120 7365 742e 7291 0000 0072   data set.r....r
-00003bc0: 5b00 0000 7274 0000 0054 728d 0000 0072  [...rt...Tr....r
-00003bd0: 9000 0000 7201 0000 0072 9400 0000 2915  ....r....r....).
-00003be0: 72d6 0000 0072 d900 0000 7205 0000 0072  r....r....r....r
-00003bf0: 4d00 0000 72b7 0000 0072 2300 0000 7224  M...r....r#...r$
-00003c00: 0000 00da 046a 6f69 6eda 0667 6574 6377  .....join..getcw
-00003c10: 6472 0200 0000 da07 7061 7265 6e74 73da  dr......parents.
-00003c20: 0772 656c 7061 7468 7213 0000 0072 3600  .relpathr....r6.
-00003c30: 0000 da0a 6769 745f 6967 6e6f 7265 722e  ....git_ignorer.
-00003c40: 0000 0072 d400 0000 7296 0000 0072 9700  ...r....r....r..
-00003c50: 0000 7233 0000 0072 9800 0000 2909 723c  ..r3...r....).r<
-00003c60: 0000 0072 5000 0000 724c 0000 00da 1270  ...rP...rL.....p
-00003c70: 6172 656e 745f 6461 7461 5f73 6574 5f69  arent_data_set_i
-00003c80: 6472 bb00 0000 da11 7061 7265 6e74 5f66  dr......parent_f
-00003c90: 6f6c 6465 725f 6162 73da 1361 6e61 6c79  older_abs..analy
-00003ca0: 7369 735f 666f 6c64 6572 5f61 6273 da18  sis_folder_abs..
-00003cb0: 616e 616c 7973 6973 5f66 6f6c 6465 725f  analysis_folder_
-00003cc0: 7265 6c61 7469 7665 729a 0000 0072 1f00  relativer....r..
-00003cd0: 0000 721f 0000 0072 3700 0000 7251 0000  ..r....r7...rQ..
-00003ce0: 00c1 0100 0073 3600 0000 0a02 0e02 0401  .....s6.........
-00003cf0: 0201 06ff 0a03 0801 0401 1203 0801 1201  ................
-00003d00: 0e01 0a01 0e01 1cff 0204 0a01 0401 0201  ................
-00003d10: 0afe 0e03 0a01 0401 2001 0880 02fd 0c05  ........ .......
-00003d20: 7a19 4769 7444 6174 614d 676d 742e 696e  z.GitDataMgmt.in
-00003d30: 6974 5f61 6e61 6c79 7369 7363 0100 0000  it_analysisc....
-00003d40: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00003d50: 4300 0000 7308 0000 007c 00a0 00a1 0053  C...s....|.....S
-00003d60: 0072 9b00 0000 2901 da05 5f73 796e 6372  .r....)..._syncr
-00003d70: 4500 0000 721f 0000 0072 1f00 0000 7237  E...r....r....r7
-00003d80: 0000 0072 5600 0000 e101 0000 7302 0000  ...rV.......s...
-00003d90: 0008 027a 1047 6974 4461 7461 4d67 6d74  ...z.GitDataMgmt
-00003da0: 2e73 796e 6363 0100 0000 0000 0000 0000  .syncc..........
-00003db0: 0000 0200 0000 0300 0000 4300 0000 7314  ..........C...s.
-00003dc0: 0000 0074 007c 007c 006a 0183 027d 017c  ...t.|.|.j...}.|
-00003dd0: 01a0 02a1 0053 0072 9b00 0000 2903 720c  .....S.r....).r.
-00003de0: 0000 0072 3b00 0000 da03 7275 6ea9 0272  ...r;.....run..r
-00003df0: 3c00 0000 da03 636d 6472 1f00 0000 721f  <.....cmdr....r.
-00003e00: 0000 0072 3700 0000 72e9 0000 00e5 0100  ...r7...r.......
-00003e10: 00f3 0400 0000 0c01 0801 7a11 4769 7444  ..........z.GitD
-00003e20: 6174 614d 676d 742e 5f73 796e 6354 6304  ataMgmt._syncTc.
-00003e30: 0000 0000 0000 0000 0000 0005 0000 0003  ................
-00003e40: 0000 0043 0000 0073 5c00 0000 7c02 721a  ...C...s\...|.r.
-00003e50: 7c00 6a00 a001 a100 7d04 7c04 a002 a100  |.j.....}.|.....
-00003e60: 720d 7c04 5300 7c00 6a00 a003 7c04 6a04  r.|.S.|.j...|.j.
-00003e70: a101 7d04 7c04 a002 a100 721a 7c04 5300  ..}.|.....r.|.S.
-00003e80: 7c00 6a00 a005 7c01 a101 7d04 7c04 a002  |.j...|...}.|...
-00003e90: a100 7226 7c04 5300 7c03 722c 7c00 a006  ..r&|.S.|.r,|...
-00003ea0: a100 7d04 7c04 5300 2901 7a28 2047 6974  ..}.|.S.).z( Git
-00003eb0: 2061 6464 2c20 636f 6d6d 6974 2061 6e64   add, commit and
-00003ec0: 2073 796e 6320 7769 7468 206f 7065 6e42   sync with openB
-00003ed0: 4953 2e20 2907 7236 0000 00da 1267 6974  IS. ).r6.....git
-00003ee0: 5f74 6f70 5f6c 6576 656c 5f70 6174 6872  _top_level_pathr
-00003ef0: b700 0000 da07 6769 745f 6164 6472 9300  ......git_addr..
-00003f00: 0000 da0a 6769 745f 636f 6d6d 6974 72e9  ....git_commitr.
-00003f10: 0000 0029 0572 3c00 0000 7254 0000 0072  ...).r<...rT...r
-00003f20: 5500 0000 7256 0000 0072 bb00 0000 721f  U...rV...r....r.
-00003f30: 0000 0072 1f00 0000 7237 0000 0072 5700  ...r....r7...rW.
-00003f40: 0000 e901 0000 731a 0000 0004 030a 0108  ......s.........
-00003f50: 0104 010e 0108 0104 010c 0108 0104 0204  ................
-00003f60: 0108 0104 017a 1247 6974 4461 7461 4d67  .....z.GitDataMg
-00003f70: 6d74 2e63 6f6d 6d69 7463 0100 0000 0000  mt.commitc......
-00003f80: 0000 0000 0000 0400 0000 0800 0000 4300  ..............C.
-00003f90: 0000 737a 0000 007c 006a 00a0 01a1 007d  ..sz...|.j.....}
-00003fa0: 017a 0a74 027c 0083 016a 0364 0164 028d  .z.t.|...j.d.d..
-00003fb0: 017d 0257 006e 1104 0074 046a 056a 0679  .}.W.n...t.j.j.y
-00003fc0: 2001 0001 0001 0074 0764 0364 0464 058d   ......t.d.d.d..
-00003fd0: 027d 0259 006e 0177 007c 016a 087d 037c  .}.Y.n.w.|.j.}.|
-00003fe0: 02a0 09a1 0072 3774 0a7c 0383 0164 066b  .....r7t.|...d.k
-00003ff0: 0472 327c 0364 0737 007d 037c 037c 026a  .r2|.d.7.}.|.|.j
-00004000: 0837 007d 0374 0764 067c 0364 058d 0253  .7.}.t.d.|.d...S
-00004010: 0029 084e 5429 01da 0969 6e66 6f5f 6f6e  .).NT)...info_on
-00004020: 6c79 728f 0000 007a 1d43 6f75 6c64 206e  lyr....z.Could n
-00004030: 6f74 2063 6f6e 6e65 6374 2074 6f20 6f70  ot connect to op
-00004040: 656e 4249 532e 7291 0000 0072 0100 0000  enBIS.r....r....
-00004050: da01 0a29 0b72 3600 0000 da0a 6769 745f  ...).r6.....git_
-00004060: 7374 6174 7573 720c 0000 0072 ea00 0000  statusr....r....
-00004070: da08 7265 7175 6573 7473 da0a 6578 6365  ..requests..exce
-00004080: 7074 696f 6e73 da0f 436f 6e6e 6563 7469  ptions..Connecti
-00004090: 6f6e 4572 726f 7272 0500 0000 7293 0000  onErrorr....r...
-000040a0: 0072 b700 0000 da03 6c65 6e29 0472 3c00  .r......len).r<.
-000040b0: 0000 72f3 0000 00da 0b73 796e 635f 7374  ..r......sync_st
-000040c0: 6174 7573 7293 0000 0072 1f00 0000 721f  atusr....r....r.
-000040d0: 0000 0072 3700 0000 7258 0000 00fb 0100  ...r7...rX......
-000040e0: 0073 1800 0000 0a01 0201 1401 1001 1001  .s..............
-000040f0: 02ff 0602 0801 0c01 0801 0a01 0c01 7a12  ..............z.
-00004100: 4769 7444 6174 614d 676d 742e 7374 6174  GitDataMgmt.stat
-00004110: 7573 6301 0000 0000 0000 0000 0000 0001  usc.............
-00004120: 0000 0004 0000 0043 0000 0073 2600 0000  .......C...s&...
-00004130: 7c00 6a00 a001 a100 6a02 7c00 5f03 7c00  |.j.....j.|._.|.
-00004140: a004 a100 0100 7405 a006 6401 6402 a102  ......t...d.d...
-00004150: 0100 6403 5300 2904 7a3a 2053 746f 7265  ..d.S.).z: Store
-00004160: 7320 7468 6520 6769 7420 636f 6d6d 6974  s the git commit
-00004170: 2068 6173 6820 616e 6420 636f 7069 6573   hash and copies
-00004180: 2074 6865 206f 6269 7320 6d65 7461 6461   the obis metada
-00004190: 7461 2e20 721d 0000 00fa 122e 6f62 6973  ta. r.......obis
-000041a0: 5f72 6573 746f 7265 706f 696e 744e 2907  _restorepointN).
-000041b0: 7236 0000 00da 0f67 6974 5f63 6f6d 6d69  r6.....git_commi
-000041c0: 745f 6861 7368 7293 0000 00da 1870 7265  t_hashr......pre
-000041d0: 7669 6f75 735f 6769 745f 636f 6d6d 6974  vious_git_commit
-000041e0: 5f68 6173 6872 c500 0000 da06 7368 7574  _hashr......shut
-000041f0: 696c da08 636f 7079 7472 6565 7245 0000  il..copytreerE..
-00004200: 0072 1f00 0000 721f 0000 0072 3700 0000  .r....r....r7...
-00004210: 72c3 0000 0008 0200 0073 0600 0000 0e02  r........s......
-00004220: 0801 1001 7a1c 4769 7444 6174 614d 676d  ....z.GitDataMgm
-00004230: 742e 7365 745f 7265 7374 6f72 6570 6f69  t.set_restorepoi
-00004240: 6e74 6301 0000 0000 0000 0000 0000 0001  ntc.............
-00004250: 0000 0004 0000 0043 0000 0073 2800 0000  .......C...s(...
-00004260: 7c00 6a00 a001 7c00 6a02 a101 0100 7403  |.j...|.j.....t.
-00004270: a004 6401 a101 0100 7403 a005 6402 6401  ..d.....t...d.d.
-00004280: a102 0100 6403 5300 2904 7a4d 2052 6573  ....d.S.).zM Res
-00004290: 6574 7320 746f 2074 6865 2073 746f 7265  ets to the store
-000042a0: 6420 6769 7420 636f 6d6d 6974 2068 6173  d git commit has
-000042b0: 6820 616e 6420 7265 7374 6f72 6573 2074  h and restores t
-000042c0: 6865 2063 6f70 6965 6420 6f62 6973 206d  he copied obis m
-000042d0: 6574 6164 6174 612e 2072 1d00 0000 72f9  etadata. r....r.
-000042e0: 0000 004e 2906 7236 0000 00da 0c67 6974  ...N).r6.....git
-000042f0: 5f72 6573 6574 5f74 6f72 fb00 0000 72fc  _reset_tor....r.
-00004300: 0000 00da 0672 6d74 7265 6572 fd00 0000  .....rmtreer....
-00004310: 7245 0000 0072 1f00 0000 721f 0000 0072  rE...r....r....r
-00004320: 3700 0000 72b0 0000 000e 0200 0073 0600  7...r........s..
-00004330: 0000 0e02 0a01 1001 7a13 4769 7444 6174  ........z.GitDat
-00004340: 614d 676d 742e 7265 7374 6f72 6563 0100  aMgmt.restorec..
-00004350: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00004360: 0000 4300 0000 731e 0000 0074 006a 01a0  ..C...s....t.j..
-00004370: 0264 01a1 0172 0d74 03a0 0464 01a1 0101  .d...r.t...d....
-00004380: 0064 0253 0064 0253 0029 037a 3b20 4465  .d.S.d.S.).z; De
-00004390: 6c65 7465 7320 7468 6520 6f62 6973 206d  letes the obis m
-000043a0: 6574 6164 6174 6120 636f 7079 2e20 5468  etadata copy. Th
-000043b0: 6973 206d 7573 7420 616c 7761 7973 2062  is must always b
-000043c0: 6520 646f 6e65 2e20 72f9 0000 004e 2905  e done. r....N).
-000043d0: 7223 0000 0072 2400 0000 7225 0000 0072  r#...r$...r%...r
-000043e0: fc00 0000 72ff 0000 0072 4500 0000 721f  ....r....rE...r.
-000043f0: 0000 0072 1f00 0000 7237 0000 0072 c500  ...r....r7...r..
-00004400: 0000 1402 0000 7306 0000 000c 020e 0104  ......s.........
-00004410: ff7a 1e47 6974 4461 7461 4d67 6d74 2e63  .z.GitDataMgmt.c
-00004420: 6c65 6172 5f72 6573 746f 7265 706f 696e  lear_restorepoin
-00004430: 7463 0500 0000 0000 0000 0000 0000 0600  tc..............
-00004440: 0000 0600 0000 4300 0000 f318 0000 0074  ......C........t
-00004450: 007c 007c 017c 027c 037c 0483 057d 057c  .|.|.|.|.|...}.|
-00004460: 05a0 01a1 0053 0072 9b00 0000 2902 7207  .....S.r....).r.
-00004470: 0000 0072 ea00 0000 a906 723c 0000 0072  ...r......r<...r
-00004480: 5b00 0000 725c 0000 0072 5d00 0000 725e  [...r\...r]...r^
-00004490: 0000 0072 ec00 0000 721f 0000 0072 1f00  ...r....r....r..
-000044a0: 0000 7237 0000 0072 5f00 0000 1902 0000  ..r7...r_.......
-000044b0: f304 0000 0010 0108 017a 1147 6974 4461  .........z.GitDa
-000044c0: 7461 4d67 6d74 2e63 6c6f 6e65 6305 0000  taMgmt.clonec...
-000044d0: 0000 0000 0000 0000 0006 0000 0006 0000  ................
-000044e0: 0043 0000 0072 0001 0000 729b 0000 0029  .C...r....r....)
-000044f0: 0272 0a00 0000 72ea 0000 0072 0101 0000  .r....r....r....
-00004500: 721f 0000 0072 1f00 0000 7237 0000 0072  r....r....r7...r
-00004510: 6100 0000 1d02 0000 7304 0000 0010 0208  a.......s.......
-00004520: 017a 1047 6974 4461 7461 4d67 6d74 2e6d  .z.GitDataMgmt.m
-00004530: 6f76 6563 0100 0000 0000 0000 0000 0000  ovec............
-00004540: 0200 0000 0200 0000 4300 0000 7310 0000  ........C...s...
-00004550: 0074 007c 0083 017d 017c 01a0 01a1 0053  .t.|...}.|.....S
-00004560: 0072 9b00 0000 2902 7206 0000 0072 ea00  .r....).r....r..
-00004570: 0000 72eb 0000 0072 1f00 0000 721f 0000  ..r....r....r...
-00004580: 0072 3700 0000 7262 0000 0022 0200 0073  .r7...rb..."...s
-00004590: 0400 0000 0801 0801 7a12 4769 7444 6174  ........z.GitDat
-000045a0: 614d 676d 742e 6164 6472 6566 6302 0000  aMgmt.addrefc...
-000045b0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-000045c0: 0043 0000 0073 1400 0000 7400 7c00 7c01  .C...s....t.|.|.
-000045d0: 6401 8d02 7d02 7c02 a001 a100 5300 2902  d...}.|.....S.).
-000045e0: 4e29 0172 5b00 0000 2902 720d 0000 0072  N).r[...).r....r
-000045f0: ea00 0000 2903 723c 0000 0072 5b00 0000  ....).r<...r[...
-00004600: 72ec 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
-00004610: 3700 0000 7264 0000 0026 0200 0072 ed00  7...rd...&...r..
-00004620: 0000 7a15 4769 7444 6174 614d 676d 742e  ..z.GitDataMgmt.
-00004630: 7265 6d6f 7665 7265 6663 0500 0000 0000  removerefc......
-00004640: 0000 0000 0000 0500 0000 0400 0000 4300  ..............C.
-00004650: 0000 72a6 0000 0029 034e 7268 0000 00fa  ..r....).Nrh....
-00004660: 3054 6869 7320 636f 6d6d 616e 6420 6973  0This command is
-00004670: 206f 6e6c 7920 6176 6169 6c61 626c 6520   only available 
-00004680: 666f 7220 4d61 6e61 6765 7220 4461 7461  for Manager Data
-00004690: 2e72 a800 0000 7265 0000 0072 1f00 0000  .r....re...r....
-000046a0: 721f 0000 0072 3700 0000 7268 0000 002a  r....r7...rh...*
-000046b0: 0200 0072 a900 0000 7a14 4769 7444 6174  ...r....z.GitDat
-000046c0: 614d 676d 742e 646f 776e 6c6f 6164 6307  aMgmt.downloadc.
-000046d0: 0000 0000 0000 0000 0000 0008 0000 0009  ................
-000046e0: 0000 0043 0000 0073 8a00 0000 7c00 6a00  ...C...s....|.j.
-000046f0: a001 7c01 a101 7d07 7c07 6401 7500 7210  ..|...}.|.d.u.r.
-00004700: 7402 6402 7c01 1700 8301 8201 7c04 7403  t.d.|.......|.t.
-00004710: 6a04 7500 7222 7c05 6401 7501 731b 4a00  j.u.r"|.d.u.s.J.
-00004720: 8201 7c06 6401 7501 7321 4a00 8201 6e17  ..|.d.u.s!J...n.
-00004730: 7c04 7403 6a05 7500 722e 7c06 6401 7500  |.t.j.u.r.|.d.u.
-00004740: 732d 4a00 8201 6e0b 7c04 7403 6a06 7500  s-J...n.|.t.j.u.
-00004750: 7239 7c06 6401 7500 7339 4a00 8201 7c00  r9|.d.u.s9J...|.
-00004760: a007 7c07 7c00 6a08 7c02 7c03 7c04 7c05  ..|.|.j.|.|.|.|.
-00004770: 7c06 a107 5300 2903 e185 0100 000a 2020  |...S.).......  
-00004780: 2020 2020 2020 3a70 6172 616d 2063 6174        :param cat
-00004790: 6567 6f72 793a 2063 6f6e 6669 672c 206f  egory: config, o
-000047a0: 626a 6563 742c 2063 6f6c 6c65 6374 696f  bject, collectio
-000047b0: 6e2c 2064 6174 615f 7365 7420 6f72 2072  n, data_set or r
-000047c0: 6570 6f73 6974 6f72 790a 2020 2020 2020  epository.      
-000047d0: 2020 3a70 6172 616d 2069 735f 676c 6f62    :param is_glob
-000047e0: 616c 3a20 6163 7420 6f6e 2067 6c6f 6261  al: act on globa
-000047f0: 6c20 7365 7474 696e 6773 202d 206c 6f63  l settings - loc
-00004800: 616c 2069 6620 6661 6c73 650a 2020 2020  al if false.    
-00004810: 2020 2020 3a70 6172 616d 2069 735f 6461      :param is_da
-00004820: 7461 5f73 6574 5f70 726f 7065 7274 793a  ta_set_property:
-00004830: 2074 7275 6520 6966 2070 726f 7020 2f20   true if prop / 
-00004840: 7661 6c75 6520 6172 6520 6120 6461 7461  value are a data
-00004850: 2073 6574 2070 726f 7065 7274 790a 2020   set property.  
-00004860: 2020 2020 2020 3a70 6172 616d 206f 7065        :param ope
-00004870: 7261 7469 6f6e 5f74 7970 653a 2074 7970  ration_type: typ
-00004880: 6520 6f66 206f 7065 7261 7469 6f6e 2074  e of operation t
-00004890: 6f20 7065 7266 6f72 6d2e 2049 7420 6361  o perform. It ca
-000048a0: 6e20 6265 2047 4554 2c20 5345 542c 2043  n be GET, SET, C
-000048b0: 4c45 4152 0a20 2020 2020 2020 203a 7061  LEAR.        :pa
-000048c0: 7261 6d20 7072 6f70 3a20 7365 7474 696e  ram prop: settin
-000048d0: 6720 6b65 790a 2020 2020 2020 2020 3a70  g key.        :p
-000048e0: 6172 616d 2076 616c 7565 3a20 7365 7474  aram value: sett
-000048f0: 696e 6720 7661 6c75 650a 2020 2020 2020  ing value.      
-00004900: 2020 4efa 1b49 6e76 616c 6964 2073 6574    N..Invalid set
-00004910: 7469 6e67 7320 6361 7465 676f 7279 3a20  tings category: 
-00004920: 2909 722e 0000 0072 d500 0000 723f 0000  ).r....r....r?..
-00004930: 0072 1200 0000 727f 0000 0072 7b00 0000  .r....r....r{...
-00004940: 7281 0000 0072 8c00 0000 7233 0000 0029  r....r....r3...)
-00004950: 0872 3c00 0000 da08 6361 7465 676f 7279  .r<.....category
-00004960: 7284 0000 0072 8500 0000 7286 0000 0072  r....r....r....r
-00004970: 8700 0000 7288 0000 0072 8300 0000 721f  ....r....r....r.
-00004980: 0000 0072 1f00 0000 7237 0000 0072 0400  ...r....r7...r..
-00004990: 0000 3102 0000 731a 0000 000c 0a08 010c  ..1...s.........
-000049a0: 010a 010c 010e 010a 010e 010a 010c 010e  ................
-000049b0: 0206 0104 ff7a 1247 6974 4461 7461 4d67  .....z.GitDataMg
-000049c0: 6d74 2e63 6f6e 6669 6763 0100 0000 0000  mt.configc......
-000049d0: 0000 0000 0000 0200 0000 0400 0000 4700  ..............G.
-000049e0: 0000 72a6 0000 00a9 034e 72af 0000 0072  ..r......Nr....r
-000049f0: 0301 0000 72a8 0000 0072 ac00 0000 721f  ....r....r....r.
-00004a00: 0000 0072 1f00 0000 7237 0000 0072 7100  ...r....r7...rq.
-00004a10: 0000 4902 0000 72a9 0000 007a 1947 6974  ..I...r....z.Git
-00004a20: 4461 7461 4d67 6d74 2e73 6561 7263 685f  DataMgmt.search_
-00004a30: 6f62 6a65 6374 6301 0000 0000 0000 0000  objectc.........
-00004a40: 0000 0002 0000 0004 0000 0047 0000 0072  ...........G...r
-00004a50: a600 0000 7207 0100 0072 a800 0000 72ac  ....r....r....r.
-00004a60: 0000 0072 1f00 0000 721f 0000 0072 3700  ...r....r....r7.
-00004a70: 0000 7272 0000 004c 0200 0072 a900 0000  ..rr...L...r....
-00004a80: 7a1b 4769 7444 6174 614d 676d 742e 7365  z.GitDataMgmt.se
-00004a90: 6172 6368 5f64 6174 615f 7365 7463 0100  arch_data_setc..
-00004aa0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00004ab0: 0000 4700 0000 72a6 0000 0029 034e 726c  ..G...r....).Nrl
-00004ac0: 0000 0072 0301 0000 72a8 0000 0072 ac00  ...r....r....r..
-00004ad0: 0000 721f 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
-00004ae0: 0072 6c00 0000 4f02 0000 72a9 0000 007a  .rl...O...r....z
-00004af0: 1247 6974 4461 7461 4d67 6d74 2e75 706c  .GitDataMgmt.upl
-00004b00: 6f61 6472 9b00 0000 729c 0000 0072 9d00  oadr....r....r..
-00004b10: 0000 291c 729e 0000 0072 9f00 0000 72a0  ..).r....r....r.
-00004b20: 0000 0072 a100 0000 7246 0000 0072 4a00  ...r....rF...rJ.
-00004b30: 0000 72d6 0000 0072 d900 0000 724d 0000  ..r....r....rM..
-00004b40: 0072 5100 0000 72c7 0000 0072 5600 0000  .rQ...r....rV...
-00004b50: 72e9 0000 0072 5700 0000 7258 0000 0072  r....rW...rX...r
-00004b60: c300 0000 72b0 0000 0072 c500 0000 725f  ....r....r....r_
-00004b70: 0000 0072 bf00 0000 7261 0000 0072 6200  ...r....ra...rb.
-00004b80: 0000 7264 0000 0072 6800 0000 7204 0000  ..rd...rh...r...
-00004b90: 0072 7100 0000 7272 0000 0072 6c00 0000  .rq...rr...rl...
-00004ba0: 721f 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
-00004bb0: 3700 0000 722c 0000 0093 0100 0073 3a00  7...r,.......s:.
-00004bc0: 0000 0800 0401 0a02 0809 0807 0804 0a04  ................
-00004bd0: 0a13 0220 0a01 0803 0204 0c01 0811 080d  ... ............
-00004be0: 0806 0806 0805 0204 0a01 0804 0a04 0804  ................
-00004bf0: 0207 0201 0aff 0818 0803 0c03 722c 0000  ............r,..
-00004c00: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00004c10: 0000 0300 0000 4000 0000 739e 0000 0065  ......@...s....e
-00004c20: 005a 0164 005a 0264 015a 0364 0264 0384  .Z.d.Z.d.Z.d.d..
-00004c30: 005a 0464 0464 0584 005a 0564 2464 0764  .Z.d.d...Z.d$d.d
-00004c40: 0884 015a 0664 2464 0964 0a84 015a 0764  ...Z.d$d.d...Z.d
-00004c50: 2564 0c64 0d84 015a 0864 0e64 0f84 005a  %d.d...Z.d.d...Z
-00004c60: 0964 1064 1184 005a 0a64 1264 1384 005a  .d.d...Z.d.d...Z
-00004c70: 0b64 1464 1584 005a 0c64 1664 1784 005a  .d.d...Z.d.d...Z
-00004c80: 0d64 2464 1864 1984 015a 0e64 1a64 1b84  .d$d.d...Z.d.d..
-00004c90: 005a 0f64 1c64 1d84 005a 1064 1e64 1f84  .Z.d.d...Z.d.d..
-00004ca0: 005a 1164 2064 2184 005a 1209 0609 0664  .Z.d d!..Z.....d
-00004cb0: 2664 2264 2384 015a 1364 0653 0029 2772  &d"d#..Z.d.S.)'r
-00004cc0: 2900 0000 7a28 4461 7461 4d67 6d74 206f  )...z(DataMgmt o
-00004cd0: 7065 7261 7469 6f6e 7320 666f 7220 4453  perations for DS
-00004ce0: 532d 7374 6f72 6564 2064 6174 612e 6301  S-stored data.c.
-00004cf0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00004d00: 0000 0043 0000 0073 0800 0000 7400 a001  ...C...s....t...
-00004d10: a100 5300 729b 0000 0029 0272 2000 0000  ..S.r....).r ...
-00004d20: 7221 0000 0072 4500 0000 721f 0000 0072  r!...rE...r....r
-00004d30: 1f00 0000 7237 0000 0072 4600 0000 5602  ....r7...rF...V.
-00004d40: 0000 7302 0000 0008 017a 2650 6879 7369  ..s......z&Physi
-00004d50: 6361 6c44 6174 614d 676d 742e 6765 745f  calDataMgmt.get_
-00004d60: 7365 7474 696e 6773 5f72 6573 6f6c 7665  settings_resolve
-00004d70: 7263 0200 0000 0000 0000 0000 0000 0200  rc..............
-00004d80: 0000 0400 0000 4300 0000 72a6 0000 0029  ......C...r....)
-00004d90: 034e 72aa 0000 00fa 3854 6869 7320 636f  .Nr.....8This co
-00004da0: 6d6d 616e 6420 6973 206f 6e6c 7920 6176  mmand is only av
-00004db0: 6169 6c61 626c 6520 666f 7220 4578 7465  ailable for Exte
-00004dc0: 726e 616c 204d 616e 6167 6572 2044 6174  rnal Manager Dat
-00004dd0: 6172 a800 0000 7248 0000 0072 1f00 0000  ar....rH...r....
-00004de0: 721f 0000 0072 3700 0000 724a 0000 0059  r....r7...rJ...Y
-00004df0: 0200 00f3 0600 0000 0601 0201 08ff 7a25  ..............z%
-00004e00: 5068 7973 6963 616c 4461 7461 4d67 6d74  PhysicalDataMgmt
-00004e10: 2e73 6574 7570 5f6c 6f63 616c 5f73 6574  .setup_local_set
-00004e20: 7469 6e67 734e 6302 0000 0000 0000 0000  tingsNc.........
-00004e30: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
-00004e40: 6400 0000 7400 6a01 a002 6401 a101 720c  d...t.j...d...r.
-00004e50: 7403 6402 6403 6404 8d02 5300 7c00 6a04  t.d.d.d...S.|.j.
-00004e60: 6a05 a006 a100 0100 7c00 6a04 6a05 a007  j.......|.j.j...
-00004e70: 6405 6406 6407 a103 0100 7c00 6a04 6a05  d.d.d.....|.j.j.
-00004e80: a008 a100 6408 1900 7d02 7c00 6a04 6a05  ....d...}.|.j.j.
-00004e90: a007 6409 7c02 6407 a103 0100 7403 640a  ..d.|.d.....t.d.
-00004ea0: 640b 6404 8d02 5300 290c 4e72 1d00 0000  d.d...S.).Nr....
-00004eb0: 728f 0000 0072 da00 0000 7291 0000 0072  r....r....r....r
-00004ec0: 1e00 0000 5472 7400 0000 da0b 6f70 656e  ....Trt.....open
-00004ed0: 6269 735f 7572 6cda 0f66 696c 6573 6572  bis_url..fileser
-00004ee0: 7669 6365 5f75 726c 7201 0000 007a 294d  vice_urlr....z)M
-00004ef0: 616e 6167 6564 2064 6174 6120 6f62 6973  anaged data obis
-00004f00: 2072 6570 6f73 6974 6f72 7920 696e 6974   repository init
-00004f10: 6961 6c69 7a65 642e 2909 7223 0000 0072  ialized.).r#...r
-00004f20: 2400 0000 7225 0000 0072 0500 0000 722e  $...r%...r....r.
-00004f30: 0000 0072 0400 0000 72df 0000 0072 9600  ...r....r....r..
-00004f40: 0000 7226 0000 0029 0372 3c00 0000 724c  ..r&...).r<...rL
-00004f50: 0000 0072 0a01 0000 721f 0000 0072 1f00  ...r....r....r..
-00004f60: 0000 7237 0000 0072 4d00 0000 5d02 0000  ..r7...rM...]...
-00004f70: 7312 0000 000c 010c 010c 0112 0110 010a  s...............
-00004f80: 0104 0104 ff0c 027a 1a50 6879 7369 6361  .......z.Physica
-00004f90: 6c44 6174 614d 676d 742e 696e 6974 5f64  lDataMgmt.init_d
-00004fa0: 6174 6163 0300 0000 0000 0000 0000 0000  atac............
-00004fb0: 0300 0000 0400 0000 4300 0000 72a6 0000  ........C...r...
-00004fc0: 0029 034e 72ab 0000 0072 0801 0000 72a8  .).Nr....r....r.
-00004fd0: 0000 0072 4f00 0000 721f 0000 0072 1f00  ...rO...r....r..
-00004fe0: 0000 7237 0000 0072 5100 0000 6702 0000  ..r7...rQ...g...
-00004ff0: 7209 0100 007a 1e50 6879 7369 6361 6c44  r....z.PhysicalD
-00005000: 6174 614d 676d 742e 696e 6974 5f61 6e61  ataMgmt.init_ana
-00005010: 6c79 7369 7354 6304 0000 0000 0000 0000  lysisTc.........
-00005020: 0000 0004 0000 0004 0000 0043 0000 0072  ...........C...r
-00005030: a600 0000 2903 4e72 5700 0000 7208 0100  ....).NrW...r...
-00005040: 0072 a800 0000 7253 0000 0072 1f00 0000  .r....rS...r....
-00005050: 721f 0000 0072 3700 0000 7257 0000 006b  r....r7...rW...k
-00005060: 0200 0072 a900 0000 7a17 5068 7973 6963  ...r....z.Physic
-00005070: 616c 4461 7461 4d67 6d74 2e63 6f6d 6d69  alDataMgmt.commi
-00005080: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
-00005090: 0000 0400 0000 4300 0000 72a6 0000 0029  ......C...r....)
-000050a0: 034e 7256 0000 0072 0801 0000 72a8 0000  .NrV...r....r...
-000050b0: 0072 4500 0000 721f 0000 0072 1f00 0000  .rE...r....r....
-000050c0: 7237 0000 0072 5600 0000 6e02 0000 72a9  r7...rV...n...r.
-000050d0: 0000 007a 1550 6879 7369 6361 6c44 6174  ...z.PhysicalDat
-000050e0: 614d 676d 742e 7379 6e63 6301 0000 0000  aMgmt.syncc.....
-000050f0: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-00005100: 0000 0072 a600 0000 2903 4e72 5800 0000  ...r....).NrX...
-00005110: 7208 0100 0072 a800 0000 7245 0000 0072  r....r....rE...r
-00005120: 1f00 0000 721f 0000 0072 3700 0000 7258  ....r....r7...rX
-00005130: 0000 0071 0200 0072 a900 0000 7a17 5068  ...q...r....z.Ph
-00005140: 7973 6963 616c 4461 7461 4d67 6d74 2e73  ysicalDataMgmt.s
-00005150: 7461 7475 7363 0500 0000 0000 0000 0000  tatusc..........
-00005160: 0000 0500 0000 0400 0000 4300 0000 72a6  ..........C...r.
-00005170: 0000 0029 034e 725f 0000 0072 0801 0000  ...).Nr_...r....
-00005180: 72a8 0000 0072 5a00 0000 721f 0000 0072  r....rZ...r....r
-00005190: 1f00 0000 7237 0000 0072 5f00 0000 7402  ....r7...r_...t.
-000051a0: 0000 72a9 0000 007a 1650 6879 7369 6361  ..r....z.Physica
-000051b0: 6c44 6174 614d 676d 742e 636c 6f6e 6563  lDataMgmt.clonec
-000051c0: 0500 0000 0000 0000 0000 0000 0500 0000  ................
-000051d0: 0400 0000 4300 0000 72a6 0000 0029 034e  ....C...r....).N
-000051e0: 7261 0000 0072 0801 0000 72a8 0000 0072  ra...r....r....r
-000051f0: 5a00 0000 721f 0000 0072 1f00 0000 7237  Z...r....r....r7
-00005200: 0000 0072 6100 0000 7702 0000 72a9 0000  ...ra...w...r...
-00005210: 007a 1550 6879 7369 6361 6c44 6174 614d  .z.PhysicalDataM
-00005220: 676d 742e 6d6f 7665 6301 0000 0000 0000  gmt.movec.......
-00005230: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-00005240: 0072 a600 0000 2903 4e72 6200 0000 7208  .r....).Nrb...r.
-00005250: 0100 0072 a800 0000 7245 0000 0072 1f00  ...r....rE...r..
-00005260: 0000 721f 0000 0072 3700 0000 7262 0000  ..r....r7...rb..
-00005270: 007a 0200 0072 a900 0000 7a17 5068 7973  .z...r....z.Phys
-00005280: 6963 616c 4461 7461 4d67 6d74 2e61 6464  icalDataMgmt.add
-00005290: 7265 6663 0200 0000 0000 0000 0000 0000  refc............
-000052a0: 0200 0000 0400 0000 4300 0000 72a6 0000  ........C...r...
-000052b0: 0029 034e 7264 0000 0072 0801 0000 72a8  .).Nrd...r....r.
-000052c0: 0000 0072 6300 0000 721f 0000 0072 1f00  ...rc...r....r..
-000052d0: 0000 7237 0000 0072 6400 0000 7d02 0000  ..r7...rd...}...
-000052e0: 72a9 0000 007a 1a50 6879 7369 6361 6c44  r....z.PhysicalD
-000052f0: 6174 614d 676d 742e 7265 6d6f 7665 7265  ataMgmt.removere
-00005300: 6663 0500 0000 0000 0000 0000 0000 0600  fc..............
-00005310: 0000 0600 0000 4300 0000 7200 0100 0072  ......C...r....r
-00005320: 9b00 0000 2902 7209 0000 0072 ea00 0000  ....).r....r....
-00005330: 2906 723c 0000 0072 5b00 0000 7266 0000  ).r<...r[...rf..
-00005340: 0072 6700 0000 725e 0000 0072 ec00 0000  .rg...r^...r....
-00005350: 721f 0000 0072 1f00 0000 7237 0000 0072  r....r....r7...r
-00005360: 6800 0000 8002 0000 7202 0100 007a 1950  h.......r....z.P
-00005370: 6879 7369 6361 6c44 6174 614d 676d 742e  hysicalDataMgmt.
-00005380: 646f 776e 6c6f 6164 6304 0000 0000 0000  downloadc.......
-00005390: 0000 0000 0005 0000 0005 0000 0043 0000  .............C..
-000053a0: 00f3 1600 0000 7400 7c00 7c01 7c02 7c03  ......t.|.|.|.|.
-000053b0: 8304 7d04 7c04 a001 a100 5300 729b 0000  ..}.|.....S.r...
-000053c0: 0029 0272 0f00 0000 72ea 0000 0029 0572  .).r....r....).r
-000053d0: 3c00 0000 7269 0000 0072 6a00 0000 726b  <...ri...rj...rk
-000053e0: 0000 0072 ec00 0000 721f 0000 0072 1f00  ...r....r....r..
-000053f0: 0000 7237 0000 0072 6c00 0000 8402 0000  ..r7...rl.......
-00005400: f304 0000 000e 0108 017a 1750 6879 7369  .........z.Physi
-00005410: 6361 6c44 6174 614d 676d 742e 7570 6c6f  calDataMgmt.uplo
-00005420: 6164 6304 0000 0000 0000 0000 0000 0005  adc.............
-00005430: 0000 0005 0000 0043 0000 0072 0c01 0000  .......C...r....
-00005440: 729b 0000 0029 0272 0e00 0000 da0e 7365  r....).r......se
-00005450: 6172 6368 5f73 616d 706c 6573 a905 723c  arch_samples..r<
-00005460: 0000 0072 6e00 0000 726f 0000 0072 7000  ...rn...ro...rp.
-00005470: 0000 72ec 0000 0072 1f00 0000 721f 0000  ..r....r....r...
-00005480: 0072 3700 0000 7271 0000 0088 0200 0072  .r7...rq.......r
-00005490: 0d01 0000 7a1e 5068 7973 6963 616c 4461  ....z.PhysicalDa
-000054a0: 7461 4d67 6d74 2e73 6561 7263 685f 6f62  taMgmt.search_ob
-000054b0: 6a65 6374 6304 0000 0000 0000 0000 0000  jectc...........
-000054c0: 0005 0000 0005 0000 0043 0000 0072 0c01  .........C...r..
-000054d0: 0000 729b 0000 0029 0272 0e00 0000 da10  ..r....).r......
-000054e0: 7365 6172 6368 5f64 6174 615f 7365 7473  search_data_sets
-000054f0: 720f 0100 0072 1f00 0000 721f 0000 0072  r....r....r....r
-00005500: 3700 0000 7272 0000 008c 0200 0072 0d01  7...rr.......r..
-00005510: 0000 7a20 5068 7973 6963 616c 4461 7461  ..z PhysicalData
-00005520: 4d67 6d74 2e73 6561 7263 685f 6461 7461  Mgmt.search_data
-00005530: 5f73 6574 6307 0000 0000 0000 0000 0000  _setc...........
-00005540: 0009 0000 0009 0000 0043 0000 0073 f600  .........C...s..
-00005550: 0000 7c00 6a00 a001 7c01 a101 7d07 7c07  ..|.j...|...}.|.
-00005560: 6401 7500 7210 7402 6402 7c01 1700 8301  d.u.r.t.d.|.....
-00005570: 8201 7c04 7403 6a04 7500 7222 7c05 6401  ..|.t.j.u.r"|.d.
-00005580: 7501 731b 4a00 8201 7c06 6401 7501 7321  u.s.J...|.d.u.s!
-00005590: 4a00 8201 6e1e 7c04 7403 6a05 7500 722e  J...n.|.t.j.u.r.
-000055a0: 7c06 6401 7500 732d 4a00 8201 6e12 7c04  |.d.u.s-J...n.|.
-000055b0: 7403 6a06 7500 7240 7c01 6403 6b03 7240  t.j.u.r@|.d.k.r@
-000055c0: 7c00 a007 7c01 9b00 6404 9d02 6405 a102  |...|...d...d...
-000055d0: 0100 7c01 6406 6b02 724f 7408 7c00 7c04  ..|.d.k.rOt.|.|.
-000055e0: 7c05 7c06 8304 7d08 7c08 a009 a100 5300  |.|...}.|.....S.
-000055f0: 7c01 6407 6b02 725e 740a 7c00 7c04 7c05  |.d.k.r^t.|.|.|.
-00005600: 7c06 8304 7d08 7c08 a009 a100 5300 7c01  |...}.|.....S.|.
-00005610: 6403 6b02 726e 7c00 a00b 7c07 7c00 6a0c  d.k.rn|...|.|.j.
-00005620: 7c02 7c03 7c04 7c05 7c06 a107 5300 7c00  |.|.|.|.|...S.|.
-00005630: a007 7c01 9b00 6408 7c04 9b00 9d03 6405  ..|...d.|.....d.
-00005640: a102 0100 6401 5300 2909 7204 0100 004e  ....d.S.).r....N
-00005650: 7205 0100 0072 0400 0000 7a06 2063 6c65  r....r....z. cle
-00005660: 6172 7208 0100 00da 066f 626a 6563 74da  arr......object.
-00005670: 0a63 6f6c 6c65 6374 696f 6efa 0120 290d  .collection.. ).
-00005680: 722e 0000 0072 d500 0000 723f 0000 0072  r....r....r?...r
-00005690: 1200 0000 727f 0000 0072 7b00 0000 7281  ....r....r{...r.
-000056a0: 0000 0072 4300 0000 720b 0000 0072 ea00  ...rC...r....r..
-000056b0: 0000 7208 0000 0072 8c00 0000 7233 0000  ..r....r....r3..
-000056c0: 0029 0972 3c00 0000 7206 0100 0072 8400  .).r<...r....r..
-000056d0: 0000 7285 0000 0072 8600 0000 7287 0000  ..r....r....r...
-000056e0: 0072 8800 0000 7283 0000 0072 ec00 0000  .r....r....r....
-000056f0: 721f 0000 0072 1f00 0000 7237 0000 0072  r....r....r7...r
-00005700: 0400 0000 9002 0000 7332 0000 000c 0a08  ........s2......
-00005710: 010c 010a 010c 010e 010a 010e 0112 010c  ................
-00005720: 0102 0104 ff08 030e 0108 0108 010e 0108  ................
-00005730: 0108 010e 0106 0104 ff10 0302 0108 ff7a  ...............z
-00005740: 1750 6879 7369 6361 6c44 6174 614d 676d  .PhysicalDataMgm
-00005750: 742e 636f 6e66 6967 729b 0000 0072 9c00  t.configr....r..
-00005760: 0000 729d 0000 0029 1472 9e00 0000 729f  ..r....).r....r.
-00005770: 0000 0072 a000 0000 72a1 0000 0072 4600  ...r....r....rF.
-00005780: 0000 724a 0000 0072 4d00 0000 7251 0000  ..rJ...rM...rQ..
-00005790: 0072 5700 0000 7256 0000 0072 5800 0000  .rW...rV...rX...
-000057a0: 725f 0000 0072 6100 0000 7262 0000 0072  r_...ra...rb...r
-000057b0: 6400 0000 7268 0000 0072 6c00 0000 7271  d...rh...rl...rq
-000057c0: 0000 0072 7200 0000 7204 0000 0072 1f00  ...rr...r....r..
-000057d0: 0000 721f 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
-000057e0: 0072 2900 0000 5302 0000 7328 0000 0008  .r)...S...s(....
-000057f0: 0004 0108 0208 030a 040a 0a0a 0408 0308  ................
-00005800: 0308 0308 0308 030a 0308 0308 0408 0408  ................
-00005810: 0402 0402 010e ff72 2900 0000 2938 72a2  .......r)...)8r.
-00005820: 0000 0072 7c00 0000 7223 0000 0072 fc00  ...r|...r#...r..
-00005830: 0000 72c0 0000 0072 b100 0000 da07 7061  ..r....r......pa
-00005840: 7468 6c69 6272 0200 0000 72f4 0000 0072  thlibr....r....r
-00005850: 9400 0000 7204 0000 0072 2000 0000 da0e  ....r....r .....
-00005860: 636f 6d6d 616e 645f 7265 7375 6c74 7205  command_resultr.
-00005870: 0000 00da 0f63 6f6d 6d61 6e64 732e 6164  .....commands.ad
-00005880: 6472 6566 7206 0000 00da 0e63 6f6d 6d61  drefr......comma
-00005890: 6e64 732e 636c 6f6e 6572 0700 0000 da13  nds.cloner......
-000058a0: 636f 6d6d 616e 6473 2e63 6f6c 6c65 6374  commands.collect
-000058b0: 696f 6e72 0800 0000 da1a 636f 6d6d 616e  ionr......comman
-000058c0: 6473 2e64 6f77 6e6c 6f61 645f 7068 7973  ds.download_phys
-000058d0: 6963 616c 7209 0000 00da 0d63 6f6d 6d61  icalr......comma
-000058e0: 6e64 732e 6d6f 7665 720a 0000 00da 0f63  nds.mover......c
-000058f0: 6f6d 6d61 6e64 732e 6f62 6a65 6374 720b  ommands.objectr.
-00005900: 0000 00da 1563 6f6d 6d61 6e64 732e 6f70  .....commands.op
-00005910: 656e 6269 735f 7379 6e63 720c 0000 00da  enbis_syncr.....
-00005920: 1263 6f6d 6d61 6e64 732e 7265 6d6f 7665  .commands.remove
-00005930: 7265 6672 0d00 0000 da0f 636f 6d6d 616e  refr......comman
-00005940: 6473 2e73 6561 7263 6872 0e00 0000 da0f  ds.searchr......
-00005950: 636f 6d6d 616e 6473 2e75 706c 6f61 6472  commands.uploadr
-00005960: 0f00 0000 da03 6769 7472 1000 0000 da05  ......gitr......
-00005970: 7574 696c 7372 1100 0000 7212 0000 0072  utilsr....r....r
-00005980: 1300 0000 7214 0000 0072 1500 0000 7216  ....r....r....r.
-00005990: 0000 00da 1273 6372 6970 7473 2e63 6c69  .....scripts.cli
-000059a0: 636b 5f75 7469 6c72 1800 0000 7219 0000  ck_utilr....r...
-000059b0: 0072 2200 0000 7238 0000 00da 0741 4243  .r"...r8.....ABC
-000059c0: 4d65 7461 7239 0000 0072 2b00 0000 72b4  Metar9...r+...r.
-000059d0: 0000 0072 bf00 0000 72c7 0000 0072 2c00  ...r....r....r,.
-000059e0: 0000 7229 0000 0072 1f00 0000 721f 0000  ..r)...r....r...
-000059f0: 0072 1f00 0000 7237 0000 00da 083c 6d6f  .r....r7.....<mo
-00005a00: 6475 6c65 3e01 0000 0073 4e00 0000 0811  dule>....sN.....
-00005a10: 0801 0801 0801 0801 0801 0c01 0802 0c02  ................
-00005a20: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 0c01  ................
-00005a30: 0c01 0c01 0c01 0c01 1001 0c01 0c01 0c01  ................
-00005a40: 0c01 1001 0804 0c01 0aff 1429 007f 105a  ...........)...Z
-00005a50: 0831 0805 0812 1017 007f 1441            .1.........A
+00000770: 8400 8301 5a13 6506 6a07 642c 6421 6422  ....Z.e.j.d,d!d"
+00000780: 8401 8301 5a14 6506 6a07 6423 6424 8400  ....Z.e.j.d#d$..
+00000790: 8301 5a15 6506 6a07 6425 6426 8400 8301  ..Z.e.j.d%d&....
+000007a0: 5a16 090c 090c 642e 6427 6428 8401 5a17  Z.....d.d'd(..Z.
+000007b0: 6518 642f 6429 642a 8401 8301 5a19 640c  e.d/d)d*....Z.d.
+000007c0: 5300 2930 da10 4162 7374 7261 6374 4461  S.)0..AbstractDa
+000007d0: 7461 4d67 6d74 7a65 4162 7374 7261 6374  taMgmtzeAbstract
+000007e0: 206f 626a 6563 7420 7468 6174 2069 6d70   object that imp
+000007f0: 6c65 6d65 6e74 7320 6f70 6572 6174 696f  lements operatio
+00000800: 6e73 2e0a 0a20 2020 2041 6c6c 206f 7065  ns...    All ope
+00000810: 7261 7469 6f6e 7320 7468 726f 7720 616e  rations throw an
+00000820: 2065 7865 7063 7469 6f6e 2069 6620 7468   exepction if th
+00000830: 6579 2066 6169 6c2e 0a20 2020 2046 5463  ey fail..    FTc
+00000840: 0b00 0000 0000 0000 0000 0000 0b00 0000  ................
+00000850: 0200 0000 4300 0000 734c 0000 007c 017c  ....C...sL...|.|
+00000860: 005f 007c 027c 005f 017c 037c 005f 027c  ._.|.|._.|.|._.|
+00000870: 047c 005f 037c 057c 005f 047c 067c 005f  .|._.|.|._.|.|._
+00000880: 057c 077c 005f 067c 087c 005f 077c 097c  .|.|._.|.|._.|.|
+00000890: 005f 087c 0a7c 005f 0964 017c 005f 0a64  ._.|.|._.d.|._.d
+000008a0: 027c 005f 0b64 0053 0029 034e 5446 290c  .|._.d.S.).NTF).
+000008b0: 722e 0000 0072 2f00 0000 7236 0000 0072  r....r/...r6...r
+000008c0: 3100 0000 7232 0000 0072 1a00 0000 721b  1...r2...r....r.
+000008d0: 0000 0072 1c00 0000 7233 0000 0072 3400  ...r....r3...r4.
+000008e0: 0000 da11 7265 7374 6f72 655f 6f6e 5f73  ....restore_on_s
+000008f0: 6967 696e 74da 1569 676e 6f72 655f 6d69  igint..ignore_mi
+00000900: 7373 696e 675f 7061 7265 6e74 290b da04  ssing_parent)...
+00000910: 7365 6c66 722e 0000 0072 2f00 0000 7236  selfr....r/...r6
+00000920: 0000 0072 3100 0000 7232 0000 0072 1a00  ...r1...r2...r..
+00000930: 0000 721b 0000 0072 1c00 0000 7233 0000  ..r....r....r3..
+00000940: 0072 3400 0000 721f 0000 0072 1f00 0000  .r4...r....r....
+00000950: 7237 0000 00da 085f 5f69 6e69 745f 5f61  r7.....__init__a
+00000960: 0000 0073 1800 0000 0602 0601 0601 0601  ...s............
+00000970: 0601 0601 0601 0601 0601 0601 0603 0a01  ................
+00000980: 7a19 4162 7374 7261 6374 4461 7461 4d67  z.AbstractDataMg
+00000990: 6d74 2e5f 5f69 6e69 745f 5f63 0300 0000  mt.__init__c....
+000009a0: 0000 0000 0000 0000 0400 0000 0400 0000  ................
+000009b0: 4300 0000 7314 0000 0064 01a0 007c 017c  C...s....d...|.|
+000009c0: 02a1 027d 0374 017c 0383 0182 0129 027a  ...}.t.|.....).z
+000009d0: 1352 6169 7365 2061 6e20 6578 6365 7074  .Raise an except
+000009e0: 696f 6e2e 7a0f 277b 7d27 2066 6169 6c65  ion.z.'{}' faile
+000009f0: 642e 207b 7d29 02da 0666 6f72 6d61 74da  d. {})...format.
+00000a00: 0a56 616c 7565 4572 726f 7229 0472 3c00  .ValueError).r<.
+00000a10: 0000 da07 636f 6d6d 616e 64da 0672 6561  ....command..rea
+00000a20: 736f 6eda 076d 6573 7361 6765 721f 0000  son..messager...
+00000a30: 0072 1f00 0000 7237 0000 00da 0b65 7272  .r....r7.....err
+00000a40: 6f72 5f72 6169 7365 7200 0000 7304 0000  or_raiser...s...
+00000a50: 000c 0208 017a 1c41 6273 7472 6163 7444  .....z.AbstractD
+00000a60: 6174 614d 676d 742e 6572 726f 725f 7261  ataMgmt.error_ra
+00000a70: 6973 6563 0100 0000 0000 0000 0000 0000  isec............
+00000a80: 0100 0000 0100 0000 4300 0000 f304 0000  ........C.......
+00000a90: 0064 0153 0029 027a 1b20 4765 7420 7468  .d.S.).z. Get th
+00000aa0: 6520 7365 7474 696e 6773 2072 6573 6f6c  e settings resol
+00000ab0: 7665 7220 4e72 1f00 0000 a901 723c 0000  ver Nr......r<..
+00000ac0: 0072 1f00 0000 721f 0000 0072 3700 0000  .r....r....r7...
+00000ad0: da15 6765 745f 7365 7474 696e 6773 5f72  ..get_settings_r
+00000ae0: 6573 6f6c 7665 7277 0000 00f3 0200 0000  esolverw........
+00000af0: 0403 7a26 4162 7374 7261 6374 4461 7461  ..z&AbstractData
+00000b00: 4d67 6d74 2e67 6574 5f73 6574 7469 6e67  Mgmt.get_setting
+00000b10: 735f 7265 736f 6c76 6572 6302 0000 0000  s_resolverc.....
+00000b20: 0000 0000 0000 0002 0000 0001 0000 0043  ...............C
+00000b30: 0000 0072 4400 0000 2902 7a34 2053 6574  ...rD...).z4 Set
+00000b40: 7570 206c 6f63 616c 2073 6574 7469 6e67  up local setting
+00000b50: 7320 2d20 666f 7220 7573 696e 6720 6f62  s - for using ob
+00000b60: 6973 2061 7320 6120 6c69 6272 6172 7920  is as a library 
+00000b70: 4e72 1f00 0000 a902 723c 0000 00da 0c61  Nr......r<.....a
+00000b80: 6c6c 5f73 6574 7469 6e67 7372 1f00 0000  ll_settingsr....
+00000b90: 721f 0000 0072 3700 0000 da14 7365 7475  r....r7.....setu
+00000ba0: 705f 6c6f 6361 6c5f 7365 7474 696e 6773  p_local_settings
+00000bb0: 7c00 0000 7247 0000 007a 2541 6273 7472  |...rG...z%Abstr
+00000bc0: 6163 7444 6174 614d 676d 742e 7365 7475  actDataMgmt.setu
+00000bd0: 705f 6c6f 6361 6c5f 7365 7474 696e 6773  p_local_settings
+00000be0: 4e63 0200 0000 0000 0000 0000 0000 0200  Nc..............
+00000bf0: 0000 0100 0000 4300 0000 7244 0000 0029  ......C...rD...)
+00000c00: 0261 4b01 0000 496e 6974 6961 6c69 7a65  .aK...Initialize
+00000c10: 2061 2064 6174 6120 7265 706f 7369 746f   a data reposito
+00000c20: 7279 2061 7420 7468 6520 7061 7468 2077  ry at the path w
+00000c30: 6974 6820 7468 6520 6465 7363 7269 7074  ith the descript
+00000c40: 696f 6e2e 0a20 2020 2020 2020 203a 7061  ion..        :pa
+00000c50: 7261 6d20 7061 7468 3a20 5061 7468 2066  ram path: Path f
+00000c60: 6f72 2074 6865 2072 6570 6f73 6974 6f72  or the repositor
+00000c70: 792e 0a20 2020 2020 2020 203a 7061 7261  y..        :para
+00000c80: 6d20 6465 7363 3a20 416e 206f 7074 696f  m desc: An optio
+00000c90: 6e61 6c20 7368 6f72 7420 6465 7363 7269  nal short descri
+00000ca0: 7074 696f 6e20 6f66 2074 6865 2072 6570  ption of the rep
+00000cb0: 6f73 6974 6f72 7920 2875 7365 6420 6279  ository (used by
+00000cc0: 2067 6974 2d61 6e6e 6578 290a 2020 2020   git-annex).    
+00000cd0: 2020 2020 3a70 6172 616d 2063 7265 6174      :param creat
+00000ce0: 653a 2049 6620 5472 7565 2061 6e64 2074  e: If True and t
+00000cf0: 6865 2066 6f6c 6465 7220 646f 6573 206e  he folder does n
+00000d00: 6f74 2065 7869 7374 2c20 6372 6561 7465  ot exist, create
+00000d10: 2069 742e 2044 6566 6175 6c74 7320 746f   it. Defaults to
+00000d20: 2074 7275 652e 0a20 2020 2020 2020 203a   true..        :
+00000d30: 7265 7475 726e 3a20 4120 436f 6d6d 616e  return: A Comman
+00000d40: 6452 6573 756c 742e 0a20 2020 2020 2020  dResult..       
+00000d50: 204e 721f 0000 00a9 0272 3c00 0000 da04   Nr......r<.....
+00000d60: 6465 7363 721f 0000 0072 1f00 0000 7237  descr....r....r7
+00000d70: 0000 00da 0969 6e69 745f 6461 7461 8100  .....init_data..
+00000d80: 0000 f302 0000 0004 087a 1a41 6273 7472  .........z.Abstr
+00000d90: 6163 7444 6174 614d 676d 742e 696e 6974  actDataMgmt.init
+00000da0: 5f64 6174 6163 0300 0000 0000 0000 0000  _datac..........
+00000db0: 0000 0300 0000 0100 0000 4300 0000 7244  ..........C...rD
+00000dc0: 0000 0029 027a f549 6e69 7469 616c 697a  ...).z.Initializ
+00000dd0: 6520 616e 2061 6e61 6c79 7369 7320 7265  e an analysis re
+00000de0: 706f 7369 746f 7279 2061 7420 7468 6520  pository at the 
+00000df0: 7061 7468 2e0a 2020 2020 2020 2020 3a70  path..        :p
+00000e00: 6172 616d 2070 6172 656e 745f 666f 6c64  aram parent_fold
+00000e10: 6572 3a20 5061 7468 2066 6f72 2074 6865  er: Path for the
+00000e20: 2072 6570 6f73 6974 6f72 792e 0a20 2020   repository..   
+00000e30: 2020 2020 203a 7061 7261 6d20 7061 7265       :param pare
+00000e40: 6e74 3a20 2872 6571 7569 7265 6420 7768  nt: (required wh
+00000e50: 656e 206f 7574 7369 6465 206f 6620 6578  en outside of ex
+00000e60: 6973 7469 6e67 2072 6570 6f73 6974 6f72  isting repositor
+00000e70: 7929 2050 6174 6820 666f 7220 7468 6520  y) Path for the 
+00000e80: 7061 7265 6e74 2072 6570 6f73 6974 6f72  parent repositor
+00000e90: 740a 2020 2020 2020 2020 3a72 6574 7572  t.        :retur
+00000ea0: 6e3a 2041 2043 6f6d 6d61 6e64 5265 7375  n: A CommandResu
+00000eb0: 6c74 2e0a 2020 2020 2020 2020 4e72 1f00  lt..        Nr..
+00000ec0: 0000 a903 723c 0000 00da 0d70 6172 656e  ....r<.....paren
+00000ed0: 745f 666f 6c64 6572 724c 0000 0072 1f00  t_folderrL...r..
+00000ee0: 0000 721f 0000 0072 3700 0000 da0d 696e  ..r....r7.....in
+00000ef0: 6974 5f61 6e61 6c79 7369 738b 0000 00f3  it_analysis.....
+00000f00: 0200 0000 0407 7a1e 4162 7374 7261 6374  ......z.Abstract
+00000f10: 4461 7461 4d67 6d74 2e69 6e69 745f 616e  DataMgmt.init_an
+00000f20: 616c 7973 6973 6304 0000 0000 0000 0000  alysisc.........
+00000f30: 0000 0004 0000 0001 0000 0043 0000 0072  ...........C...r
+00000f40: 4400 0000 2902 615e 0100 0043 6f6d 6d69  D...).a^...Commi
+00000f50: 7420 7468 6520 6375 7272 656e 7420 7265  t the current re
+00000f60: 706f 2e0a 0a20 2020 2020 2020 2054 6869  po...        Thi
+00000f70: 7320 6973 7375 6573 2061 2067 6974 2063  s issues a git c
+00000f80: 6f6d 6d69 7420 616e 6420 636f 6e6e 6563  ommit and connec
+00000f90: 7473 2074 6f20 6f70 656e 4249 5320 616e  ts to openBIS an
+00000fa0: 6420 6372 6561 7465 7320 6120 6461 7461  d creates a data
+00000fb0: 2073 6574 2069 6e20 6f70 656e 4249 532e   set in openBIS.
+00000fc0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00000fd0: 6d73 673a 2043 6f6d 6d69 7420 6d65 7373  msg: Commit mess
+00000fe0: 6167 652e 0a20 2020 2020 2020 203a 7061  age..        :pa
+00000ff0: 7261 6d20 6175 746f 5f61 6464 3a20 4175  ram auto_add: Au
+00001000: 746f 6d61 7469 6361 6c6c 7920 6164 6420  tomatically add 
+00001010: 616c 6c20 6669 6c65 7320 696e 2074 6865  all files in the
+00001020: 2066 6f6c 6465 7220 746f 2074 6865 2072   folder to the r
+00001030: 6570 6f2e 2044 6566 6175 6c74 7320 746f  epo. Defaults to
+00001040: 2054 7275 652e 0a20 2020 2020 2020 203a   True..        :
+00001050: 7061 7261 6d20 7379 6e63 3a20 4966 2074  param sync: If t
+00001060: 7275 652c 2073 796e 6320 7769 7468 206f  rue, sync with o
+00001070: 7065 6e42 4953 2073 6572 7665 722e 0a20  penBIS server.. 
+00001080: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00001090: 4120 436f 6d6d 616e 6452 6573 756c 742e  A CommandResult.
+000010a0: 0a20 2020 2020 2020 204e 721f 0000 00a9  .        Nr.....
+000010b0: 0472 3c00 0000 da03 6d73 67da 0861 7574  .r<.....msg..aut
+000010c0: 6f5f 6164 64da 0473 796e 6372 1f00 0000  o_add..syncr....
+000010d0: 721f 0000 0072 3700 0000 da06 636f 6d6d  r....r7.....comm
+000010e0: 6974 9400 0000 7302 0000 0004 0a7a 1741  it....s......z.A
+000010f0: 6273 7472 6163 7444 6174 614d 676d 742e  bstractDataMgmt.
+00001100: 636f 6d6d 6974 6301 0000 0000 0000 0000  commitc.........
+00001110: 0000 0001 0000 0001 0000 0043 0000 0072  ...........C...r
+00001120: 4400 0000 2902 7a86 5379 6e63 2074 6865  D...).z.Sync the
+00001130: 2063 7572 7265 6e74 2072 6570 6f2e 0a0a   current repo...
+00001140: 2020 2020 2020 2020 5468 6973 2063 6f6e          This con
+00001150: 6e65 6374 7320 746f 206f 7065 6e42 4953  nects to openBIS
+00001160: 2061 6e64 2063 7265 6174 6573 2061 2064   and creates a d
+00001170: 6174 6120 7365 7420 696e 206f 7065 6e42  ata set in openB
+00001180: 4953 2e0a 2020 2020 2020 2020 3a72 6574  IS..        :ret
+00001190: 7572 6e3a 2041 2043 6f6d 6d61 6e64 5265  urn: A CommandRe
+000011a0: 7375 6c74 2e0a 2020 2020 2020 2020 4e72  sult..        Nr
+000011b0: 1f00 0000 7245 0000 0072 1f00 0000 721f  ....rE...r....r.
+000011c0: 0000 0072 3700 0000 7256 0000 00a0 0000  ...r7...rV......
+000011d0: 0072 5200 0000 7a15 4162 7374 7261 6374  .rR...z.Abstract
+000011e0: 4461 7461 4d67 6d74 2e73 796e 6363 0100  DataMgmt.syncc..
+000011f0: 0000 0000 0000 0000 0000 0100 0000 0100  ................
+00001200: 0000 4300 0000 7244 0000 0029 027a 5752  ..C...rD...).zWR
+00001210: 6574 7572 6e20 7468 6520 7374 6174 7573  eturn the status
+00001220: 206f 6620 7468 6520 6375 7272 656e 7420   of the current 
+00001230: 7265 706f 7369 746f 7279 2e0a 2020 2020  repository..    
+00001240: 2020 2020 3a72 6574 7572 6e3a 2041 2043      :return: A C
+00001250: 6f6d 6d61 6e64 5265 7375 6c74 2e0a 2020  ommandResult..  
+00001260: 2020 2020 2020 4e72 1f00 0000 7245 0000        Nr....rE..
+00001270: 0072 1f00 0000 721f 0000 0072 3700 0000  .r....r....r7...
+00001280: da06 7374 6174 7573 a900 0000 f302 0000  ..status........
+00001290: 0004 057a 1741 6273 7472 6163 7444 6174  ...z.AbstractDat
+000012a0: 614d 676d 742e 7374 6174 7573 6305 0000  aMgmt.statusc...
+000012b0: 0000 0000 0000 0000 0005 0000 0001 0000  ................
+000012c0: 0043 0000 0072 4400 0000 2902 617d 0100  .C...rD...).a}..
+000012d0: 0043 6c6f 6e65 202f 2063 6f70 7920 6120  .Clone / copy a 
+000012e0: 7265 706f 7369 746f 7279 2072 656c 6174  repository relat
+000012f0: 6564 2074 6f20 7468 6520 6769 7665 6e20  ed to the given 
+00001300: 6461 7461 2073 6574 2069 642e 0a20 2020  data set id..   
+00001310: 2020 2020 203a 7061 7261 6d20 6461 7461       :param data
+00001320: 5f73 6574 5f69 643a 200a 2020 2020 2020  _set_id: .      
+00001330: 2020 3a70 6172 616d 2073 7368 5f75 7365    :param ssh_use
+00001340: 723a 2073 7368 2075 7365 7220 666f 7220  r: ssh user for 
+00001350: 7265 6d6f 7465 2073 7973 7465 6d20 286f  remote system (o
+00001360: 7074 696f 6e61 6c29 0a20 2020 2020 2020  ptional).       
+00001370: 203a 7061 7261 6d20 636f 6e74 656e 745f   :param content_
+00001380: 636f 7079 5f69 6e64 6578 3a20 696e 6465  copy_index: inde
+00001390: 7820 6f66 2063 6f6e 7465 6e74 2063 6f70  x of content cop
+000013a0: 7920 696e 2063 6173 6520 7468 6572 6520  y in case there 
+000013b0: 6172 6520 6d75 6c74 6970 6c65 2063 6f70  are multiple cop
+000013c0: 6965 7320 286f 7074 696f 6e61 6c29 0a20  ies (optional). 
+000013d0: 2020 2020 2020 203a 7061 7261 6d20 736b         :param sk
+000013e0: 6970 5f69 6e74 6567 7269 7479 5f63 6865  ip_integrity_che
+000013f0: 636b 3a20 6966 2074 7275 652c 2074 6865  ck: if true, the
+00001400: 2066 696c 6520 6368 6563 6b73 756d 7320   file checksums 
+00001410: 7769 6c6c 206e 6f74 2062 6520 6368 6563  will not be chec
+00001420: 6b65 640a 2020 2020 2020 2020 3a72 6574  ked.        :ret
+00001430: 7572 6e3a 2041 2043 6f6d 6d61 6e64 5265  urn: A CommandRe
+00001440: 7375 6c74 2e0a 2020 2020 2020 2020 4e72  sult..        Nr
+00001450: 1f00 0000 a905 723c 0000 00da 0b64 6174  ......r<.....dat
+00001460: 615f 7365 745f 6964 da08 7373 685f 7573  a_set_id..ssh_us
+00001470: 6572 da12 636f 6e74 656e 745f 636f 7079  er..content_copy
+00001480: 5f69 6e64 6578 da14 736b 6970 5f69 6e74  _index..skip_int
+00001490: 6567 7269 7479 5f63 6865 636b 721f 0000  egrity_checkr...
+000014a0: 0072 1f00 0000 7237 0000 00da 0563 6c6f  .r....r7.....clo
+000014b0: 6e65 b000 0000 f302 0000 0004 097a 1641  ne...........z.A
+000014c0: 6273 7472 6163 7444 6174 614d 676d 742e  bstractDataMgmt.
+000014d0: 636c 6f6e 6563 0500 0000 0000 0000 0000  clonec..........
+000014e0: 0000 0500 0000 0100 0000 4300 0000 7244  ..........C...rD
+000014f0: 0000 0029 0261 7501 0000 4d6f 7665 2061  ...).au...Move a
+00001500: 2072 6570 6f73 6974 6f72 7920 7265 6c61   repository rela
+00001510: 7465 6420 746f 2074 6865 2067 6976 656e  ted to the given
+00001520: 2064 6174 6120 7365 7420 6964 2e0a 2020   data set id..  
+00001530: 2020 2020 2020 3a70 6172 616d 2064 6174        :param dat
+00001540: 615f 7365 745f 6964 3a20 0a20 2020 2020  a_set_id: .     
+00001550: 2020 203a 7061 7261 6d20 7373 685f 7573     :param ssh_us
+00001560: 6572 3a20 7373 6820 7573 6572 2066 6f72  er: ssh user for
+00001570: 2072 656d 6f74 6520 7379 7374 656d 2028   remote system (
+00001580: 6f70 7469 6f6e 616c 290a 2020 2020 2020  optional).      
+00001590: 2020 3a70 6172 616d 2063 6f6e 7465 6e74    :param content
+000015a0: 5f63 6f70 795f 696e 6465 783a 2069 6e64  _copy_index: ind
+000015b0: 6578 206f 6620 636f 6e74 656e 7420 636f  ex of content co
+000015c0: 7079 2069 6e20 6361 7365 2074 6865 7265  py in case there
+000015d0: 2061 7265 206d 756c 7469 706c 6520 636f   are multiple co
+000015e0: 7069 6573 2028 6f70 7469 6f6e 616c 290a  pies (optional).
+000015f0: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
+00001600: 6b69 705f 696e 7465 6772 6974 795f 6368  kip_integrity_ch
+00001610: 6563 6b3a 2069 6620 7472 7565 2c20 7468  eck: if true, th
+00001620: 6520 6669 6c65 2063 6865 636b 7375 6d73  e file checksums
+00001630: 2077 696c 6c20 6e6f 7420 6265 2063 6865   will not be che
+00001640: 636b 6564 0a20 2020 2020 2020 203a 7265  cked.        :re
+00001650: 7475 726e 3a20 4120 436f 6d6d 616e 6452  turn: A CommandR
+00001660: 6573 756c 742e 0a20 2020 2020 2020 204e  esult..        N
+00001670: 721f 0000 0072 5a00 0000 721f 0000 0072  r....rZ...r....r
+00001680: 1f00 0000 7237 0000 00da 046d 6f76 65bb  ....r7.....move.
+00001690: 0000 0072 6000 0000 7a15 4162 7374 7261  ...r`...z.Abstra
+000016a0: 6374 4461 7461 4d67 6d74 2e6d 6f76 6563  ctDataMgmt.movec
+000016b0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000016c0: 0100 0000 4300 0000 7244 0000 0029 027a  ....C...rD...).z
+000016d0: 6341 6464 2074 6865 2063 7572 7265 6e74  cAdd the current
+000016e0: 2066 6f6c 6465 7220 6173 2061 6e20 6f62   folder as an ob
+000016f0: 6973 2072 6570 6f73 6974 6f72 7920 746f  is repository to
+00001700: 206f 7065 6e42 4953 2e0a 2020 2020 2020   openBIS..      
+00001710: 2020 3a72 6574 7572 6e3a 2041 2043 6f6d    :return: A Com
+00001720: 6d61 6e64 5265 7375 6c74 2e0a 2020 2020  mandResult..    
+00001730: 2020 2020 4e72 1f00 0000 7245 0000 0072      Nr....rE...r
+00001740: 1f00 0000 721f 0000 0072 3700 0000 da06  ....r....r7.....
+00001750: 6164 6472 6566 c600 0000 7259 0000 007a  addref....rY...z
+00001760: 1741 6273 7472 6163 7444 6174 614d 676d  .AbstractDataMgm
+00001770: 742e 6164 6472 6566 6302 0000 0000 0000  t.addrefc.......
+00001780: 0000 0000 0002 0000 0001 0000 0043 0000  .............C..
+00001790: 0072 4400 0000 2902 7ab4 5265 6d6f 7665  .rD...).z.Remove
+000017a0: 2074 6865 2063 7572 7265 6e74 2066 6f6c   the current fol
+000017b0: 6465 7220 2f20 7265 706f 7369 746f 7279  der / repository
+000017c0: 2066 726f 6d20 6f70 656e 4249 532e 0a20   from openBIS.. 
+000017d0: 2020 2020 2020 203a 7061 7261 6d20 6461         :param da
+000017e0: 7461 5f73 6574 5f69 643a 2049 6420 6f66  ta_set_id: Id of
+000017f0: 2074 6865 2064 6174 6120 6672 6f6d 2077   the data from w
+00001800: 6869 6368 2061 2072 6566 6572 656e 6365  hich a reference
+00001810: 2073 686f 756c 6420 6265 2072 656d 6f76   should be remov
+00001820: 6564 2e0a 2020 2020 2020 2020 3a72 6574  ed..        :ret
+00001830: 7572 6e3a 2041 2043 6f6d 6d61 6e64 5265  urn: A CommandRe
+00001840: 7375 6c74 2e0a 2020 2020 2020 2020 4e72  sult..        Nr
+00001850: 1f00 0000 a902 723c 0000 0072 5b00 0000  ......r<...r[...
+00001860: 721f 0000 0072 1f00 0000 7237 0000 00da  r....r....r7....
+00001870: 0972 656d 6f76 6572 6566 cd00 0000 7302  .removeref....s.
+00001880: 0000 0004 067a 1a41 6273 7472 6163 7444  .....z.AbstractD
+00001890: 6174 614d 676d 742e 7265 6d6f 7665 7265  ataMgmt.removere
+000018a0: 6663 0500 0000 0000 0000 0000 0000 0500  fc..............
+000018b0: 0000 0100 0000 4300 0000 7244 0000 0029  ......C...rD...)
+000018c0: 0261 9001 0000 446f 776e 6c6f 6164 2066  .a....Download f
+000018d0: 696c 6573 206f 6620 6120 7265 706f 7369  iles of a reposi
+000018e0: 746f 7279 2077 6974 686f 7574 2061 6464  tory without add
+000018f0: 696e 6720 6120 636f 6e74 656e 7420 636f  ing a content co
+00001900: 7079 2e0a 2020 2020 2020 2020 3a70 6172  py..        :par
+00001910: 616d 2064 6174 615f 7365 745f 6964 3a20  am data_set_id: 
+00001920: 4964 206f 6620 7468 6520 6461 7461 2073  Id of the data s
+00001930: 6574 2074 6f20 646f 776e 6c6f 6164 2066  et to download f
+00001940: 726f 6d2e 0a20 2020 2020 2020 203a 7061  rom..        :pa
+00001950: 7261 6d20 6672 6f6d 5f66 696c 653a 2050  ram from_file: P
+00001960: 6174 6820 6f66 2061 2066 696c 6520 7769  ath of a file wi
+00001970: 7468 2061 206c 6973 7420 6f66 2064 6174  th a list of dat
+00001980: 6173 6574 7320 746f 2064 6f77 6e6c 6f61  asets to downloa
+00001990: 642e 0a20 2020 2020 2020 203a 7061 7261  d..        :para
+000019a0: 6d20 6669 6c65 3a20 5061 7468 206f 6620  m file: Path of 
+000019b0: 6120 6669 6c65 2069 6e20 7468 6520 6461  a file in the da
+000019c0: 7461 2073 6574 2074 6f20 646f 776e 6c6f  ta set to downlo
+000019d0: 6164 2e20 416c 6c20 6669 6c65 7320 6172  ad. All files ar
+000019e0: 6520 646f 776e 6c6f 6164 6564 2069 6620  e downloaded if 
+000019f0: 6974 2069 7320 4e6f 6e65 2e0a 2020 2020  it is None..    
+00001a00: 2020 2020 3a70 6172 616d 2073 6b69 705f      :param skip_
+00001a10: 696e 7465 6772 6974 795f 6368 6563 6b3a  integrity_check:
+00001a20: 2043 6865 636b 7375 6d73 206f 6620 6669   Checksums of fi
+00001a30: 6c65 7320 6172 6520 6e6f 7420 7665 7269  les are not veri
+00001a40: 6669 6564 2069 6620 7472 7565 2e0a 2020  fied if true..  
+00001a50: 2020 2020 2020 4e72 1f00 0000 a905 723c        Nr......r<
+00001a60: 0000 0072 5b00 0000 da09 6672 6f6d 5f66  ...r[.....from_f
+00001a70: 696c 65da 0466 696c 6572 5e00 0000 721f  ile..filer^...r.
+00001a80: 0000 0072 1f00 0000 7237 0000 00da 0864  ...r....r7.....d
+00001a90: 6f77 6e6c 6f61 64d5 0000 0072 4e00 0000  ownload....rN...
+00001aa0: 7a19 4162 7374 7261 6374 4461 7461 4d67  z.AbstractDataMg
+00001ab0: 6d74 2e64 6f77 6e6c 6f61 6463 0500 0000  mt.downloadc....
+00001ac0: 0000 0000 0000 0000 0500 0000 0100 0000  ................
+00001ad0: 4300 0000 7244 0000 0029 0261 2101 0000  C...rD...).a!...
+00001ae0: 5570 6c6f 6164 2066 696c 6573 2f64 6972  Upload files/dir
+00001af0: 6563 746f 7269 6573 2069 6e74 6f20 6120  ectories into a 
+00001b00: 6e65 7720 6461 7461 2073 6574 2e0a 2020  new data set..  
+00001b10: 2020 2020 2020 3a70 6172 616d 2073 616d        :param sam
+00001b20: 706c 655f 6964 3a20 7065 726d 4964 206f  ple_id: permId o
+00001b30: 7220 7361 6d70 6c65 2070 6174 6820 6f66  r sample path of
+00001b40: 2074 6865 2070 6172 656e 7420 7361 6d70   the parent samp
+00001b50: 6c65 0a20 2020 2020 2020 203a 7061 7261  le.        :para
+00001b60: 6d20 6461 7461 5f73 6574 5f74 7970 653a  m data_set_type:
+00001b70: 2074 7970 6520 6f66 2063 7265 6174 6564   type of created
+00001b80: 2064 6174 6120 7365 740a 2020 2020 2020   data set.      
+00001b90: 2020 3a70 6172 616d 2066 696c 6573 3a20    :param files: 
+00001ba0: 6c69 7374 206f 6620 6669 6c65 732f 6469  list of files/di
+00001bb0: 7265 6374 6f72 6965 7320 746f 2075 706c  rectories to upl
+00001bc0: 6f61 640a 2020 2020 2020 2020 3a70 6172  oad.        :par
+00001bd0: 616d 2070 726f 7065 7274 6965 733a 206c  am properties: l
+00001be0: 6973 7420 6f66 2070 726f 7065 7274 6965  ist of propertie
+00001bf0: 7320 746f 2073 6574 0a20 2020 2020 2020  s to set.       
+00001c00: 204e 721f 0000 0029 0572 3c00 0000 da09   Nr....).r<.....
+00001c10: 7361 6d70 6c65 5f69 64da 0d64 6174 615f  sample_id..data_
+00001c20: 7365 745f 7479 7065 da05 6669 6c65 73da  set_type..files.
+00001c30: 0a70 726f 7065 7274 6965 7372 1f00 0000  .propertiesr....
+00001c40: 721f 0000 0072 3700 0000 da06 7570 6c6f  r....r7.....uplo
+00001c50: 6164 df00 0000 724e 0000 007a 1741 6273  ad....rN...z.Abs
+00001c60: 7472 6163 7444 6174 614d 676d 742e 7570  tractDataMgmt.up
+00001c70: 6c6f 6164 6304 0000 0000 0000 0000 0000  loadc...........
+00001c80: 0004 0000 0001 0000 0043 0000 0072 4400  .........C...rD.
+00001c90: 0000 2902 612e 0100 0053 6561 7263 6820  ..).a....Search 
+00001ca0: 666f 7220 6f62 6a65 6374 7320 696e 206f  for objects in o
+00001cb0: 7065 6e42 4953 2075 7369 6e67 2066 696c  penBIS using fil
+00001cc0: 7465 7269 6e67 2063 7269 7465 7269 612e  tering criteria.
+00001cd0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001ce0: 6669 6c74 6572 733a 2064 6963 7469 6f6e  filters: diction
+00001cf0: 6172 7920 6f66 2066 696c 7465 7220 7061  ary of filter pa
+00001d00: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00001d10: 203a 7061 7261 6d20 7265 6375 7273 6976   :param recursiv
+00001d20: 653a 2046 6c61 6720 696e 6469 6361 7469  e: Flag indicati
+00001d30: 6e67 2069 6620 7365 6172 6368 2073 686f  ng if search sho
+00001d40: 756c 6420 696e 636c 7564 6520 6368 696c  uld include chil
+00001d50: 6472 656e 2072 6563 7572 7369 7665 6c79  dren recursively
+00001d60: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00001d70: 7361 7665 3a20 4669 6c65 2070 6174 6820  save: File path 
+00001d80: 746f 2073 6176 6520 7265 7375 6c74 732e  to save results.
+00001d90: 2049 6620 6d69 7373 696e 672c 2073 6561   If missing, sea
+00001da0: 7263 6820 7265 7375 6c74 7320 7769 6c6c  rch results will
+00001db0: 206e 6f74 2062 6520 7361 7665 642e 0a20   not be saved.. 
+00001dc0: 2020 2020 2020 204e 721f 0000 00a9 0472         Nr......r
+00001dd0: 3c00 0000 da07 6669 6c74 6572 73da 0972  <.....filters..r
+00001de0: 6563 7572 7369 7665 da04 7361 7665 721f  ecursive..saver.
+00001df0: 0000 0072 1f00 0000 7237 0000 00da 0d73  ...r....r7.....s
+00001e00: 6561 7263 685f 6f62 6a65 6374 e900 0000  earch_object....
+00001e10: 7252 0000 007a 1e41 6273 7472 6163 7444  rR...z.AbstractD
+00001e20: 6174 614d 676d 742e 7365 6172 6368 5f6f  ataMgmt.search_o
+00001e30: 626a 6563 7463 0400 0000 0000 0000 0000  bjectc..........
+00001e40: 0000 0400 0000 0100 0000 4300 0000 7244  ..........C...rD
+00001e50: 0000 0029 0261 2f01 0000 5365 6172 6368  ...).a/...Search
+00001e60: 2066 6f72 2064 6174 6173 6574 7320 696e   for datasets in
+00001e70: 206f 7065 6e42 4953 2075 7369 6e67 2066   openBIS using f
+00001e80: 696c 7465 7269 6e67 2063 7269 7465 7269  iltering criteri
+00001e90: 612e 0a20 2020 2020 2020 203a 7061 7261  a..        :para
+00001ea0: 6d20 6669 6c74 6572 733a 2064 6963 7469  m filters: dicti
+00001eb0: 6f6e 6172 7920 6f66 2066 696c 7465 7220  onary of filter 
+00001ec0: 7061 7261 6d65 7465 7273 0a20 2020 2020  parameters.     
+00001ed0: 2020 203a 7061 7261 6d20 7265 6375 7273     :param recurs
+00001ee0: 6976 653a 2046 6c61 6720 696e 6469 6361  ive: Flag indica
+00001ef0: 7469 6e67 2069 6620 7365 6172 6368 2073  ting if search s
+00001f00: 686f 756c 6420 696e 636c 7564 6520 6368  hould include ch
+00001f10: 696c 6472 656e 2072 6563 7572 7369 7665  ildren recursive
+00001f20: 6c79 0a20 2020 2020 2020 203a 7061 7261  ly.        :para
+00001f30: 6d20 7361 7665 3a20 4669 6c65 2070 6174  m save: File pat
+00001f40: 6820 746f 2073 6176 6520 7265 7375 6c74  h to save result
+00001f50: 732e 2049 6620 6d69 7373 696e 672c 2073  s. If missing, s
+00001f60: 6561 7263 6820 7265 7375 6c74 7320 7769  earch results wi
+00001f70: 6c6c 206e 6f74 2062 6520 7361 7665 642e  ll not be saved.
+00001f80: 0a20 2020 2020 2020 204e 721f 0000 0072  .        Nr....r
+00001f90: 6e00 0000 721f 0000 0072 1f00 0000 7237  n...r....r....r7
+00001fa0: 0000 00da 0f73 6561 7263 685f 6461 7461  .....search_data
+00001fb0: 5f73 6574 f200 0000 7252 0000 007a 2041  _set....rR...z A
+00001fc0: 6273 7472 6163 7444 6174 614d 676d 742e  bstractDataMgmt.
+00001fd0: 7365 6172 6368 5f64 6174 615f 7365 7463  search_data_setc
+00001fe0: 0800 0000 0000 0000 0000 0000 0c00 0000  ................
+00001ff0: 0c00 0000 4300 0000 733e 0100 007c 0372  ....C...s>...|.r
+00002000: 097c 01a0 0064 0167 01a1 0101 006e 067c  .|...d.g.....n.|
+00002010: 01a0 0064 0267 01a1 0101 007c 01a0 01a1  ...d.g.....|....
+00002020: 007d 087c 0472 197c 0864 0319 007d 087c  .}.|.r.|.d...}.|
+00002030: 0574 026a 0375 0072 5b7c 0664 0075 0072  .t.j.u.r[|.d.u.r
+00002040: 3574 046a 057c 0864 0464 0564 068d 037d  5t.j.|.d.d.d...}
+00002050: 0974 0664 07a0 077c 09a1 0164 0864 098d  .t.d...|...d.d..
+00002060: 0201 0064 0053 007c 067c 0876 0172 4274  ...d.S.|.|.v.rBt
+00002070: 0864 0aa0 077c 067c 016a 09a1 0283 0182  .d...|.|.j......
+00002080: 017c 067c 087c 0619 0069 017d 0a74 046a  .|.|.|...i.}.t.j
+00002090: 057c 0a64 0464 0564 068d 037d 0974 0664  .|.d.d.d...}.t.d
+000020a0: 07a0 077c 09a1 0164 0864 098d 0201 0064  ...|...d.d.....d
+000020b0: 0053 007c 0574 026a 0a75 0072 6d74 0b64  .S.|.t.j.u.rmt.d
+000020c0: 0b7c 00a0 0c7c 027c 017c 067c 077c 037c  .|...|.|.|.|.|.|
+000020d0: 04a1 0683 0253 007c 0574 026a 0d75 0072  .....S.|.t.j.u.r
+000020e0: 9d7c 0664 0075 0072 9064 0c7d 0b7c 08a0  .|.d.u.r.d.}.|..
+000020f0: 0ea1 0044 005d 117d 067c 0b74 0b64 0b7c  ...D.].}.|.t.d.|
+00002100: 00a0 0c7c 027c 017c 0664 007c 037c 04a1  ...|.|.|.d.|.|..
+00002110: 0683 0237 007d 0b71 7c7c 0b53 0074 0b64  ...7.}.q||.S.t.d
+00002120: 0b7c 00a0 0c7c 027c 017c 0664 007c 037c  .|...|.|.|.d.|.|
+00002130: 04a1 0683 0253 0064 0053 0029 0d4e da06  .....S.d.S.).N..
+00002140: 676c 6f62 616c da05 6c6f 6361 6c72 6c00  global..localrl.
+00002150: 0000 e904 0000 0054 2902 da06 696e 6465  .......T)...inde
+00002160: 6e74 da09 736f 7274 5f6b 6579 737a 027b  nt..sort_keysz.{
+00002170: 7d46 2901 da0e 7769 7468 5f74 696d 6573  }F)...with_times
+00002180: 7461 6d70 7a1a 556e 6b6e 6f77 6e20 7365  tampz.Unknown se
+00002190: 7474 696e 6720 7b7d 2066 6f72 207b 7d2e  tting {} for {}.
+000021a0: 7204 0000 0072 0100 0000 290f da19 7365  r....r....)...se
+000021b0: 745f 6c6f 6361 7469 6f6e 5f73 6561 7263  t_location_searc
+000021c0: 685f 6f72 6465 7272 2600 0000 7212 0000  h_orderr&...r...
+000021d0: 00da 0347 4554 da04 6a73 6f6e da05 6475  ...GET..json..du
+000021e0: 6d70 7372 1800 0000 723e 0000 0072 3f00  mpsr....r>...r?.
+000021f0: 0000 da08 6361 7465 676f 7479 da03 5345  ....categoty..SE
+00002200: 5472 1900 0000 da0c 7365 745f 7072 6f70  Tr......set_prop
+00002210: 6572 7479 da05 434c 4541 52da 046b 6579  erty..CLEAR..key
+00002220: 7329 0c72 3c00 0000 da08 7265 736f 6c76  s).r<.....resolv
+00002230: 6572 7233 0000 00da 0969 735f 676c 6f62  err3.....is_glob
+00002240: 616c da14 6973 5f64 6174 615f 7365 745f  al..is_data_set_
+00002250: 7072 6f70 6572 7479 da0e 6f70 6572 6174  property..operat
+00002260: 696f 6e5f 7479 7065 da04 7072 6f70 da05  ion_type..prop..
+00002270: 7661 6c75 6572 2600 0000 da0a 636f 6e66  valuer&.....conf
+00002280: 6967 5f73 7472 da0b 6c69 7474 6c65 5f64  ig_str..little_d
+00002290: 6963 74da 0b72 6574 7572 6e5f 636f 6465  ict..return_code
+000022a0: 721f 0000 0072 1f00 0000 7237 0000 00da  r....r....r7....
+000022b0: 0d75 7064 6174 655f 636f 6e66 6967 fb00  .update_config..
+000022c0: 0000 734e 0000 0004 030e 010c 0208 0204  ..sN............
+000022d0: 0108 010a 0208 0110 0116 0108 0202 010c  ................
+000022e0: 0104 ff0c 0210 0116 010a 0104 010e 0102  ................
+000022f0: 0102 ff04 ff0a 0308 0104 010c 0106 010c  ................
+00002300: 0104 0102 ff08 ff04 0304 020e 0102 0102  ................
+00002310: ff04 ff04 f77a 1e41 6273 7472 6163 7444  .....z.AbstractD
+00002320: 6174 614d 676d 742e 7570 6461 7465 5f63  ataMgmt.update_c
+00002330: 6f6e 6669 6763 0600 0000 0000 0000 0000  onfigc..........
+00002340: 0000 0800 0000 0a00 0000 4300 0000 738e  ..........C...s.
+00002350: 0000 007c 0472 0464 016e 0164 027d 067a  ...|.r.d.n.d.}.z
+00002360: 187c 0572 147c 016a 0064 037c 027c 037c  .|.r.|.j.d.|.|.|
+00002370: 0664 0464 058d 0501 006e 097c 016a 017c  .d.d.....n.|.j.|
+00002380: 027c 037c 0664 0464 058d 0401 0057 006e  .|.|.d.d.....W.n
+00002390: 2204 0074 0279 4001 007d 0701 007a 167c  "..t.y@..}...z.|
+000023a0: 0064 0475 0072 2c7c 0782 0174 0364 0664  .d.u.r,|...t.d.d
+000023b0: 0774 047c 0783 0117 0064 088d 0257 0006  .t.|.....d...W..
+000023c0: 0059 0064 097d 077e 0753 0064 097d 077e  .Y.d.}.~.S.d.}.~
+000023d0: 0777 0177 0074 0364 0a64 0b64 088d 0253  .w.w.t.d.d.d...S
+000023e0: 0029 0c7a 3c48 656c 7065 7220 6675 6e63  .).z<Helper func
+000023f0: 7469 6f6e 2074 6f20 696d 706c 656d 656e  tion to implemen
+00002400: 7420 7468 6520 7072 6f70 6572 7479 2073  t the property s
+00002410: 6574 7469 6e67 2073 656d 616e 7469 6373  etting semantics
+00002420: 2e72 7400 0000 7275 0000 0072 6c00 0000  .rt...ru...rl...
+00002430: 54a9 01da 0b61 7070 6c79 5f72 756c 6573  T....apply_rules
+00002440: e9ff ffff fffa 0745 7272 6f72 3a20 a902  .......Error: ..
+00002450: da0a 7265 7475 726e 636f 6465 da06 6f75  ..returncode..ou
+00002460: 7470 7574 4e72 0100 0000 da00 2905 da1c  tputNr......)...
+00002470: 7365 745f 7661 6c75 655f 666f 725f 6a73  set_value_for_js
+00002480: 6f6e 5f70 6172 616d 6574 6572 da17 7365  on_parameter..se
+00002490: 745f 7661 6c75 655f 666f 725f 7061 7261  t_value_for_para
+000024a0: 6d65 7465 72da 0945 7863 6570 7469 6f6e  meter..Exception
+000024b0: 7205 0000 00da 0373 7472 2908 7233 0000  r......str).r3..
+000024c0: 0072 8300 0000 7287 0000 0072 8800 0000  .r....r....r....
+000024d0: 7284 0000 0072 8500 0000 da03 6c6f 63da  r....r......loc.
+000024e0: 0165 721f 0000 0072 1f00 0000 7237 0000  .er....r....r7..
+000024f0: 0072 8000 0000 2301 0000 731e 0000 000c  .r....#...s.....
+00002500: 0302 0104 010c 0102 0108 ff12 0304 800e  ................
+00002510: 0108 0104 0120 0108 8002 fd0c 057a 1d41  ..... .......z.A
+00002520: 6273 7472 6163 7444 6174 614d 676d 742e  bstractDataMgmt.
+00002530: 7365 745f 7072 6f70 6572 7479 2902 4654  set_property).FT
+00002540: a901 4ea9 0254 54a9 024e 4e29 0146 291a  ..N..TT..NN).F).
+00002550: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00002560: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00002570: 6d65 5f5f da07 5f5f 646f 635f 5f72 3d00  me__..__doc__r=.
+00002580: 0000 7243 0000 00da 0361 6263 da0e 6162  ..rC.....abc..ab
+00002590: 7374 7261 6374 6d65 7468 6f64 7246 0000  stractmethodrF..
+000025a0: 0072 4a00 0000 724d 0000 0072 5100 0000  .rJ...rM...rQ...
+000025b0: 7257 0000 0072 5600 0000 7258 0000 0072  rW...rV...rX...r
+000025c0: 5f00 0000 7261 0000 0072 6200 0000 7264  _...ra...rb...rd
+000025d0: 0000 0072 6800 0000 726d 0000 0072 7200  ...rh...rm...rr.
+000025e0: 0000 7273 0000 0072 8c00 0000 da0c 7374  ..rs...r......st
+000025f0: 6174 6963 6d65 7468 6f64 7280 0000 0072  aticmethodr....r
+00002600: 1f00 0000 721f 0000 0072 1f00 0000 7237  ....r....r....r7
+00002610: 0000 0072 3900 0000 5b00 0000 7350 0000  ...r9...[...sP..
+00002620: 0008 0004 0102 060a ff08 1104 050a 0104  ................
+00002630: 040a 0104 040c 0104 090c 0104 080c 0104  ................
+00002640: 0b0a 0104 080a 0104 060a 0104 0a0a 0104  ................
+00002650: 0a0a 0104 060c 0104 070a 0104 090c 0104  ................
+00002660: 090a 0104 080a 0102 0902 010a fe02 2810  ..............(.
+00002670: 0172 3900 0000 2901 da09 6d65 7461 636c  .r9...)...metacl
+00002680: 6173 7363 0000 0000 0000 0000 0000 0000  assc............
+00002690: 0000 0000 0300 0000 4000 0000 7390 0000  ........@...s...
+000026a0: 0065 005a 0164 005a 0264 015a 0364 0264  .e.Z.d.Z.d.Z.d.d
+000026b0: 0384 005a 0464 0464 0584 005a 0564 2264  ...Z.d.d...Z.d"d
+000026c0: 0764 0884 015a 0664 2264 0964 0a84 015a  .d...Z.d"d.d...Z
+000026d0: 0764 2364 0c64 0d84 015a 0864 0e64 0f84  .d#d.d...Z.d.d..
+000026e0: 005a 0964 1064 1184 005a 0a64 1264 1384  .Z.d.d...Z.d.d..
+000026f0: 005a 0b64 1464 1584 005a 0c64 1664 1784  .Z.d.d...Z.d.d..
+00002700: 005a 0d64 2264 1864 1984 015a 0e64 1a64  .Z.d"d.d...Z.d.d
+00002710: 1b84 005a 0f64 1c64 1d84 005a 1064 1e64  ...Z.d.d...Z.d.d
+00002720: 1f84 005a 1164 2064 2184 005a 1264 0653  ...Z.d d!..Z.d.S
+00002730: 0029 2472 2b00 0000 7a45 4461 7461 4d67  .)$r+...zEDataMg
+00002740: 6d74 206f 7065 7261 7469 6f6e 7320 7768  mt operations wh
+00002750: 656e 2067 6974 2069 7320 6e6f 7420 6176  en git is not av
+00002760: 6169 6c61 626c 6520 2d2d 2073 686f 7720  ailable -- show 
+00002770: 6572 726f 7220 6d65 7373 6167 6573 2e63  error messages.c
+00002780: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00002790: 0400 0000 4300 0000 f310 0000 007c 00a0  ....C........|..
+000027a0: 0064 0164 02a1 0201 0064 0053 0029 034e  .d.d.....d.S.).N
+000027b0: 7a15 6765 7420 7365 7474 696e 6773 2072  z.get settings r
+000027c0: 6573 6f6c 7665 72fa 154e 6f20 6769 7420  esolver..No git 
+000027d0: 636f 6d6d 616e 6420 666f 756e 642e a901  command found...
+000027e0: 7243 0000 0072 4500 0000 721f 0000 0072  rC...rE...r....r
+000027f0: 1f00 0000 7237 0000 0072 4600 0000 3801  ....r7...rF...8.
+00002800: 0000 f302 0000 0010 017a 234e 6f47 6974  .........z#NoGit
+00002810: 4461 7461 4d67 6d74 2e67 6574 5f73 6574  DataMgmt.get_set
+00002820: 7469 6e67 735f 7265 736f 6c76 6572 6302  tings_resolverc.
+00002830: 0000 0000 0000 0000 0000 0002 0000 0004  ................
+00002840: 0000 0043 0000 0072 a600 0000 2903 4efa  ...C...r....).N.
+00002850: 1473 6574 7570 206c 6f63 616c 2073 6574  .setup local set
+00002860: 7469 6e67 7372 a700 0000 72a8 0000 0072  tingsr....r....r
+00002870: 4800 0000 721f 0000 0072 1f00 0000 7237  H...r....r....r7
+00002880: 0000 0072 4a00 0000 3b01 0000 72a9 0000  ...rJ...;...r...
+00002890: 007a 224e 6f47 6974 4461 7461 4d67 6d74  .z"NoGitDataMgmt
+000028a0: 2e73 6574 7570 5f6c 6f63 616c 5f73 6574  .setup_local_set
+000028b0: 7469 6e67 734e 6302 0000 0000 0000 0000  tingsNc.........
+000028c0: 0000 0002 0000 0004 0000 0043 0000 0072  ...........C...r
+000028d0: a600 0000 2903 4e7a 0969 6e69 7420 6461  ....).Nz.init da
+000028e0: 7461 72a7 0000 0072 a800 0000 724b 0000  tar....r....rK..
+000028f0: 0072 1f00 0000 721f 0000 0072 3700 0000  .r....r....r7...
+00002900: 724d 0000 003e 0100 0072 a900 0000 7a17  rM...>...r....z.
+00002910: 4e6f 4769 7444 6174 614d 676d 742e 696e  NoGitDataMgmt.in
+00002920: 6974 5f64 6174 6163 0300 0000 0000 0000  it_datac........
+00002930: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
+00002940: 72a6 0000 0029 034e fa0d 696e 6974 2061  r....).N..init a
+00002950: 6e61 6c79 7369 7372 a700 0000 72a8 0000  nalysisr....r...
+00002960: 0072 4f00 0000 721f 0000 0072 1f00 0000  .rO...r....r....
+00002970: 7237 0000 0072 5100 0000 4101 0000 72a9  r7...rQ...A...r.
+00002980: 0000 007a 1b4e 6f47 6974 4461 7461 4d67  ...z.NoGitDataMg
+00002990: 6d74 2e69 6e69 745f 616e 616c 7973 6973  mt.init_analysis
+000029a0: 5463 0400 0000 0000 0000 0000 0000 0400  Tc..............
+000029b0: 0000 0400 0000 4300 0000 72a6 0000 0029  ......C...r....)
+000029c0: 034e 7257 0000 0072 a700 0000 72a8 0000  .NrW...r....r...
+000029d0: 0072 5300 0000 721f 0000 0072 1f00 0000  .rS...r....r....
+000029e0: 7237 0000 0072 5700 0000 4401 0000 72a9  r7...rW...D...r.
+000029f0: 0000 007a 144e 6f47 6974 4461 7461 4d67  ...z.NoGitDataMg
+00002a00: 6d74 2e63 6f6d 6d69 7463 0100 0000 0000  mt.commitc......
+00002a10: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+00002a20: 0000 72a6 0000 0029 034e 7256 0000 0072  ..r....).NrV...r
+00002a30: a700 0000 72a8 0000 0072 4500 0000 721f  ....r....rE...r.
+00002a40: 0000 0072 1f00 0000 7237 0000 0072 5600  ...r....r7...rV.
+00002a50: 0000 4701 0000 72a9 0000 007a 124e 6f47  ..G...r....z.NoG
+00002a60: 6974 4461 7461 4d67 6d74 2e73 796e 6363  itDataMgmt.syncc
+00002a70: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00002a80: 0400 0000 4300 0000 72a6 0000 0029 034e  ....C...r....).N
+00002a90: 7258 0000 0072 a700 0000 72a8 0000 0072  rX...r....r....r
+00002aa0: 4500 0000 721f 0000 0072 1f00 0000 7237  E...r....r....r7
+00002ab0: 0000 0072 5800 0000 4a01 0000 72a9 0000  ...rX...J...r...
+00002ac0: 007a 144e 6f47 6974 4461 7461 4d67 6d74  .z.NoGitDataMgmt
+00002ad0: 2e73 7461 7475 7363 0500 0000 0000 0000  .statusc........
+00002ae0: 0000 0000 0500 0000 0400 0000 4300 0000  ............C...
+00002af0: 72a6 0000 0029 034e 725f 0000 0072 a700  r....).Nr_...r..
+00002b00: 0000 72a8 0000 0072 5a00 0000 721f 0000  ..r....rZ...r...
+00002b10: 0072 1f00 0000 7237 0000 0072 5f00 0000  .r....r7...r_...
+00002b20: 4d01 0000 72a9 0000 007a 134e 6f47 6974  M...r....z.NoGit
+00002b30: 4461 7461 4d67 6d74 2e63 6c6f 6e65 6305  DataMgmt.clonec.
+00002b40: 0000 0000 0000 0000 0000 0005 0000 0004  ................
+00002b50: 0000 0043 0000 0072 a600 0000 2903 4e72  ...C...r....).Nr
+00002b60: 6100 0000 72a7 0000 0072 a800 0000 725a  a...r....r....rZ
+00002b70: 0000 0072 1f00 0000 721f 0000 0072 3700  ...r....r....r7.
+00002b80: 0000 7261 0000 0050 0100 0072 a900 0000  ..ra...P...r....
+00002b90: 7a12 4e6f 4769 7444 6174 614d 676d 742e  z.NoGitDataMgmt.
+00002ba0: 6d6f 7665 6301 0000 0000 0000 0000 0000  movec...........
+00002bb0: 0001 0000 0004 0000 0043 0000 0072 a600  .........C...r..
+00002bc0: 0000 2903 4e72 6200 0000 72a7 0000 0072  ..).Nrb...r....r
+00002bd0: a800 0000 7245 0000 0072 1f00 0000 721f  ....rE...r....r.
+00002be0: 0000 0072 3700 0000 7262 0000 0053 0100  ...r7...rb...S..
+00002bf0: 0072 a900 0000 7a14 4e6f 4769 7444 6174  .r....z.NoGitDat
+00002c00: 614d 676d 742e 6164 6472 6566 6302 0000  aMgmt.addrefc...
+00002c10: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00002c20: 0043 0000 0072 a600 0000 2903 4e72 6400  .C...r....).Nrd.
+00002c30: 0000 72a7 0000 0072 a800 0000 7263 0000  ..r....r....rc..
+00002c40: 0072 1f00 0000 721f 0000 0072 3700 0000  .r....r....r7...
+00002c50: 7264 0000 0056 0100 0072 a900 0000 7a17  rd...V...r....z.
+00002c60: 4e6f 4769 7444 6174 614d 676d 742e 7265  NoGitDataMgmt.re
+00002c70: 6d6f 7665 7265 6663 0100 0000 0000 0000  moverefc........
+00002c80: 0000 0000 0200 0000 0400 0000 4700 0000  ............G...
+00002c90: 72a6 0000 0029 034e 7268 0000 0072 a700  r....).Nrh...r..
+00002ca0: 0000 72a8 0000 00a9 0272 3c00 0000 da01  ..r......r<.....
+00002cb0: 5f72 1f00 0000 721f 0000 0072 3700 0000  _r....r....r7...
+00002cc0: 7268 0000 0059 0100 0072 a900 0000 7a16  rh...Y...r....z.
+00002cd0: 4e6f 4769 7444 6174 614d 676d 742e 646f  NoGitDataMgmt.do
+00002ce0: 776e 6c6f 6164 6301 0000 0000 0000 0000  wnloadc.........
+00002cf0: 0000 0002 0000 0004 0000 0047 0000 0072  ...........G...r
+00002d00: a600 0000 a903 4eda 0673 6561 7263 6872  ......N..searchr
+00002d10: a700 0000 72a8 0000 0072 ac00 0000 721f  ....r....r....r.
+00002d20: 0000 0072 1f00 0000 7237 0000 0072 7200  ...r....r7...rr.
+00002d30: 0000 5c01 0000 72a9 0000 007a 1b4e 6f47  ..\...r....z.NoG
+00002d40: 6974 4461 7461 4d67 6d74 2e73 6561 7263  itDataMgmt.searc
+00002d50: 685f 6f62 6a65 6374 6301 0000 0000 0000  h_objectc.......
+00002d60: 0000 0000 0002 0000 0004 0000 0047 0000  .............G..
+00002d70: 0072 a600 0000 72ae 0000 0072 a800 0000  .r....r....r....
+00002d80: 72ac 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
+00002d90: 3700 0000 7273 0000 005f 0100 0072 a900  7...rs..._...r..
+00002da0: 0000 7a1d 4e6f 4769 7444 6174 614d 676d  ..z.NoGitDataMgm
+00002db0: 742e 7365 6172 6368 5f64 6174 615f 7365  t.search_data_se
+00002dc0: 7463 0100 0000 0000 0000 0000 0000 0200  tc..............
+00002dd0: 0000 0400 0000 4700 0000 72a6 0000 0029  ......G...r....)
+00002de0: 034e 726d 0000 0072 a700 0000 72a8 0000  .Nrm...r....r...
+00002df0: 0072 ac00 0000 721f 0000 0072 1f00 0000  .r....r....r....
+00002e00: 7237 0000 0072 6d00 0000 6201 0000 72a9  r7...rm...b...r.
+00002e10: 0000 007a 144e 6f47 6974 4461 7461 4d67  ...z.NoGitDataMg
+00002e20: 6d74 2e75 706c 6f61 6472 9b00 0000 729c  mt.uploadr....r.
+00002e30: 0000 0029 1372 9e00 0000 729f 0000 0072  ...).r....r....r
+00002e40: a000 0000 72a1 0000 0072 4600 0000 724a  ....r....rF...rJ
+00002e50: 0000 0072 4d00 0000 7251 0000 0072 5700  ...rM...rQ...rW.
+00002e60: 0000 7256 0000 0072 5800 0000 725f 0000  ..rV...rX...r_..
+00002e70: 0072 6100 0000 7262 0000 0072 6400 0000  .ra...rb...rd...
+00002e80: 7268 0000 0072 7200 0000 7273 0000 0072  rh...rr...rs...r
+00002e90: 6d00 0000 721f 0000 0072 1f00 0000 721f  m...r....r....r.
+00002ea0: 0000 0072 3700 0000 722b 0000 0035 0100  ...r7...r+...5..
+00002eb0: 0073 2200 0000 0800 0401 0802 0803 0a03  .s".............
+00002ec0: 0a03 0a03 0803 0803 0803 0803 0803 0a03  ................
+00002ed0: 0803 0803 0803 0c03 722b 0000 0063 0100  ........r+...c..
+00002ee0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00002ef0: 0000 4300 0000 7316 0000 007c 00a0 00a1  ..C...s....|....
+00002f00: 0001 0074 01a0 0264 01a1 0101 0064 0053  ...t...d.....d.S
+00002f10: 0029 024e 7201 0000 0029 03da 0772 6573  .).Nr....)...res
+00002f20: 746f 7265 da03 7379 73da 0465 7869 7429  tore..sys..exit)
+00002f30: 01da 0964 6174 615f 6d67 6d74 721f 0000  ...data_mgmtr...
+00002f40: 0072 1f00 0000 7237 0000 00da 1672 6573  .r....r7.....res
+00002f50: 746f 7265 5f73 6967 6e61 6c5f 6861 6e64  tore_signal_hand
+00002f60: 6c65 7266 0100 0073 0400 0000 0801 0e01  lerf...s........
+00002f70: 72b4 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00002f80: 0000 0200 0000 0300 0000 0300 0000 f310  ................
+00002f90: 0000 0087 0066 0164 0164 0284 087d 017c  .....f.d.d...}.|
+00002fa0: 0153 0029 037a 3320 546f 2062 6520 7573  .S.).z3 To be us
+00002fb0: 6564 2077 6974 6820 636f 6d6d 616e 6473  ed with commands
+00002fc0: 2074 6861 7420 7573 6520 7468 6520 436f   that use the Co
+00002fd0: 6d6d 616e 644c 6f67 2e20 6301 0000 0000  mmandLog. c.....
+00002fe0: 0000 0000 0000 0004 0000 000a 0000 0017  ................
+00002ff0: 0000 0073 6e00 0000 7a0a 8800 7c00 6701  ...sn...z...|.g.
+00003000: 7c01 a201 5200 8e00 7d02 5700 6e16 0400  |...R...}.W.n...
+00003010: 7400 7920 0100 7d03 0100 7a0a 7c00 6a01  t.y ..}...z.|.j.
+00003020: a002 7403 7c03 8301 a101 0100 7c03 8201  ..t.|.......|...
+00003030: 6400 7d03 7e03 7701 7700 7c02 a004 a100  d.}.~.w.w.|.....
+00003040: 6401 6b02 722e 7c00 6a01 a005 a100 0100  d.k.r.|.j.......
+00003050: 7c02 5300 7c00 6a01 a002 7c02 6a06 a101  |.S.|.j...|.j...
+00003060: 0100 7c02 5300 2902 4e46 2907 7297 0000  ..|.S.).NF).r...
+00003070: 0072 3200 0000 da09 6c6f 675f 6572 726f  .r2.....log_erro
+00003080: 7272 9800 0000 da07 6661 696c 7572 65da  rr......failure.
+00003090: 0773 7563 6365 7373 7293 0000 00a9 0472  .successr......r
+000030a0: 3c00 0000 da04 6172 6773 da06 7265 7375  <.....args..resu
+000030b0: 6c74 729a 0000 00a9 01da 0166 721f 0000  ltr........fr...
+000030c0: 0072 3700 0000 da0a 665f 7769 7468 5f6c  .r7.....f_with_l
+000030d0: 6f67 6e01 0000 7318 0000 0002 0114 010e  ogn...s.........
+000030e0: 0110 0104 0108 8002 fe0c 030a 0104 030e  ................
+000030f0: ff04 017a 1c77 6974 685f 6c6f 672e 3c6c  ...z.with_log.<l
+00003100: 6f63 616c 733e 2e66 5f77 6974 685f 6c6f  ocals>.f_with_lo
+00003110: 6772 1f00 0000 2902 72bd 0000 0072 be00  gr....).r....r..
+00003120: 0000 721f 0000 0072 bc00 0000 7237 0000  ..r....r....r7..
+00003130: 00da 0877 6974 685f 6c6f 676b 0100 0073  ...with_logk...s
+00003140: 0400 0000 0c03 040c 72bf 0000 0063 0100  ........r....c..
+00003150: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00003160: 0000 0300 0000 72b5 0000 0029 037a 2f20  ......r....).z/ 
+00003170: 5365 7473 2074 6865 2072 6573 746f 7265  Sets the restore
+00003180: 2070 6f69 6e74 2061 6e64 2072 6573 746f   point and resto
+00003190: 7265 7320 6f6e 2065 7272 6f72 2e20 6301  res on error. c.
+000031a0: 0000 0000 0000 0000 0000 0004 0000 000a  ................
+000031b0: 0000 0017 0000 0073 aa00 0000 8800 a000  .......s........
+000031c0: a100 0100 7a25 8800 6a01 7213 7402 a002  ....z%..j.r.t...
+000031d0: 7402 6a03 8700 6601 6401 6402 8408 a102  t.j...f.d.d.....
+000031e0: 0100 8801 8800 6701 7c01 a201 5200 8e00  ......g.|...R...
+000031f0: 7d02 7c02 a004 a100 7223 8800 a005 a100  }.|.....r#......
+00003200: 0100 8800 a006 a100 0100 7c02 5700 5300  ..........|.W.S.
+00003210: 0400 7407 7954 0100 7d03 0100 7a1f 8800  ..t.yT..}...z...
+00003220: a005 a100 0100 8800 6a08 6403 6b02 723c  ........j.d.k.r<
+00003230: 7c03 8201 8800 a006 a100 0100 7409 6404  |...........t.d.
+00003240: 6405 740a 7c03 8301 1700 6406 8d02 5700  d.t.|.....d...W.
+00003250: 0600 5900 6400 7d03 7e03 5300 6400 7d03  ..Y.d.}.~.S.d.}.
+00003260: 7e03 7701 7700 2907 4e63 0200 0000 0000  ~.w.w.).Nc......
+00003270: 0000 0000 0000 0200 0000 0200 0000 1300  ................
+00003280: 0000 7308 0000 0074 0088 0083 0153 0072  ..s....t.....S.r
+00003290: 9b00 0000 2901 72b4 0000 0029 02da 0673  ....).r....)...s
+000032a0: 6967 6e61 6cda 0566 7261 6d65 7245 0000  ignal..framerE..
+000032b0: 0072 1f00 0000 7237 0000 00da 083c 6c61  .r....r7.....<la
+000032c0: 6d62 6461 3e84 0100 0073 0200 0000 0800  mbda>....s......
+000032d0: 7a36 7769 7468 5f72 6573 746f 7265 2e3c  z6with_restore.<
+000032e0: 6c6f 6361 6c73 3e2e 665f 7769 7468 5f72  locals>.f_with_r
+000032f0: 6573 746f 7265 2e3c 6c6f 6361 6c73 3e2e  estore.<locals>.
+00003300: 3c6c 616d 6264 613e 5472 8f00 0000 7290  <lambda>Tr....r.
+00003310: 0000 0072 9100 0000 290b da10 7365 745f  ...r....)...set_
+00003320: 7265 7374 6f72 6570 6f69 6e74 723a 0000  restorepointr:..
+00003330: 0072 c000 0000 da06 5349 4749 4e54 72b7  .r......SIGINTr.
+00003340: 0000 0072 b000 0000 da12 636c 6561 725f  ...r......clear_
+00003350: 7265 7374 6f72 6570 6f69 6e74 7297 0000  restorepointr...
+00003360: 0072 3300 0000 7205 0000 0072 9800 0000  .r3...r....r....
+00003370: 72b9 0000 0072 bc00 0000 7245 0000 0072  r....r....rE...r
+00003380: 3700 0000 da0e 665f 7769 7468 5f72 6573  7.....f_with_res
+00003390: 746f 7265 8001 0000 7322 0000 0008 0102  tore....s"......
+000033a0: 0106 0116 0110 0108 0108 0108 0106 010e  ................
+000033b0: 0108 010a 0104 0108 0120 0108 8002 fb7a  ......... .....z
+000033c0: 2477 6974 685f 7265 7374 6f72 652e 3c6c  $with_restore.<l
+000033d0: 6f63 616c 733e 2e66 5f77 6974 685f 7265  ocals>.f_with_re
+000033e0: 7374 6f72 6572 1f00 0000 2902 72bd 0000  storer....).r...
+000033f0: 0072 c600 0000 721f 0000 0072 bc00 0000  .r....r....r....
+00003400: 7237 0000 00da 0c77 6974 685f 7265 7374  r7.....with_rest
+00003410: 6f72 657d 0100 0073 0400 0000 0c03 0411  ore}...s........
+00003420: 72c7 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00003430: 0000 0000 0000 0400 0000 4000 0000 73dc  ..........@...s.
+00003440: 0000 0065 005a 0164 005a 0264 015a 0364  ...e.Z.d.Z.d.Z.d
+00003450: 3064 0364 0484 015a 0464 0564 0684 005a  0d.d...Z.d.d...Z
+00003460: 0564 0764 0884 005a 0664 0964 0a84 005a  .d.d...Z.d.d...Z
+00003470: 0764 3064 0b64 0c84 015a 0864 3064 0d64  .d0d.d...Z.d0d.d
+00003480: 0e84 015a 0965 0a64 0f64 1084 0083 015a  ...Z.e.d.d.....Z
+00003490: 0b64 1164 1284 005a 0c65 0a64 3164 1464  .d.d...Z.e.d1d.d
+000034a0: 1584 0183 015a 0d64 1664 1784 005a 0e64  .....Z.d.d...Z.d
+000034b0: 1864 1984 005a 0f64 1a64 1b84 005a 1064  .d...Z.d.d...Z.d
+000034c0: 1c64 1d84 005a 1164 1e64 1f84 005a 1265  .d...Z.d.d...Z.e
+000034d0: 1364 2064 2184 0083 015a 1464 2264 2384  .d d!....Z.d"d#.
+000034e0: 005a 1564 3064 2464 2584 015a 1664 2664  .Z.d0d$d%..Z.d&d
+000034f0: 2784 005a 1709 0209 0264 3264 2864 2984  '..Z.....d2d(d).
+00003500: 015a 1864 2a64 2b84 005a 1964 2c64 2d84  .Z.d*d+..Z.d,d-.
+00003510: 005a 1a64 2e64 2f84 005a 1b64 0253 0029  .Z.d.d/..Z.d.S.)
+00003520: 3372 2c00 0000 7a24 4461 7461 4d67 6d74  3r,...z$DataMgmt
+00003530: 206f 7065 7261 7469 6f6e 7320 696e 206e   operations in n
+00003540: 6f72 6d61 6c20 7374 6174 652e 4e63 0200  ormal state.Nc..
+00003550: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+00003560: 0000 4300 0000 7326 0000 007c 0164 0075  ..C...s&...|.d.u
+00003570: 0072 077c 006a 0053 0074 01a0 02a1 007d  .r.|.j.S.t.....}
+00003580: 027c 02a0 0364 017c 01a1 0201 007c 0253  .|...d.|.....|.S
+00003590: 0029 024e da08 6461 7461 5f73 6574 2904  .).N..data_set).
+000035a0: 722e 0000 0072 2000 0000 7221 0000 00da  r....r ...r!....
+000035b0: 1b73 6574 5f72 6573 6f6c 7665 725f 6c6f  .set_resolver_lo
+000035c0: 6361 7469 6f6e 5f72 6f6f 7473 a903 723c  cation_roots..r<
+000035d0: 0000 00da 0d72 656c 6174 6976 655f 7061  .....relative_pa
+000035e0: 7468 722e 0000 0072 1f00 0000 721f 0000  thr....r....r...
+000035f0: 0072 3700 0000 7246 0000 0097 0100 0073  .r7...rF.......s
+00003600: 0a00 0000 0801 0601 0802 0c01 0401 7a21  ..............z!
+00003610: 4769 7444 6174 614d 676d 742e 6765 745f  GitDataMgmt.get_
+00003620: 7365 7474 696e 6773 5f72 6573 6f6c 7665  settings_resolve
+00003630: 7263 0200 0000 0000 0000 0000 0000 0700  rc..............
+00003640: 0000 0700 0000 4300 0000 7350 0000 007c  ......C...sP...|
+00003650: 006a 00a0 0164 0164 02a1 0201 007c 01a0  .j...d.d.....|..
+00003660: 02a1 0044 005d 1a5c 027d 027d 0374 037c  ...D.].\.}.}.t.|
+00003670: 006a 007c 0283 027d 047c 03a0 02a1 0044  .j.|...}.|.....D
+00003680: 005d 0b5c 027d 057d 067c 04a0 047c 057c  .].\.}.}.|...|.|
+00003690: 0664 03a1 0301 0071 1971 0b64 0053 0029  .d.....q.q.d.S.)
+000036a0: 044e 72c8 0000 00da 012e 7275 0000 0029  .Nr.......ru...)
+000036b0: 0572 2e00 0000 72c9 0000 00da 0569 7465  .r....r......ite
+000036c0: 6d73 da07 6765 7461 7474 7272 9600 0000  ms..getattrr....
+000036d0: 2907 723c 0000 0072 4900 0000 da0d 7265  ).r<...rI.....re
+000036e0: 736f 6c76 6572 5f74 7970 65da 0873 6574  solver_type..set
+000036f0: 7469 6e67 7372 8300 0000 da03 6b65 7972  tingsr......keyr
+00003700: 8800 0000 721f 0000 0072 1f00 0000 7237  ....r....r....r7
+00003710: 0000 0072 4a00 0000 a001 0000 730e 0000  ...rJ.......s...
+00003720: 000e 0110 010c 0110 0110 0102 ff04 fe7a  ...............z
+00003730: 2047 6974 4461 7461 4d67 6d74 2e73 6574   GitDataMgmt.set
+00003740: 7570 5f6c 6f63 616c 5f73 6574 7469 6e67  up_local_setting
+00003750: 7363 0200 0000 0000 0000 0000 0000 0300  sc..............
+00003760: 0000 0300 0000 4300 0000 f31a 0000 007c  ......C........|
+00003770: 00a0 007c 01a1 017d 027c 026a 01a0 02a1  ...|...}.|.j....
+00003780: 00a0 0364 01a1 0153 0029 024e 725b 0000  ...d...S.).Nr[..
+00003790: 00a9 0472 4600 0000 da0a 7265 706f 7369  ...rF.....reposi
+000037a0: 746f 7279 7226 0000 00da 0367 6574 72ca  toryr&.....getr.
+000037b0: 0000 0072 1f00 0000 721f 0000 0072 3700  ...r....r....r7.
+000037c0: 0000 da0f 6765 745f 6461 7461 5f73 6574  ....get_data_set
+000037d0: 5f69 64a7 0100 00f3 0400 0000 0a01 1001  _id.............
+000037e0: 7a1b 4769 7444 6174 614d 676d 742e 6765  z.GitDataMgmt.ge
+000037f0: 745f 6461 7461 5f73 6574 5f69 6463 0200  t_data_set_idc..
+00003800: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+00003810: 0000 4300 0000 72d2 0000 0029 024e da02  ..C...r....).N..
+00003820: 6964 72d3 0000 0072 ca00 0000 721f 0000  idr....r....r...
+00003830: 0072 1f00 0000 7237 0000 00da 1167 6574  .r....r7.....get
+00003840: 5f72 6570 6f73 6974 6f72 795f 6964 ab01  _repository_id..
+00003850: 0000 72d7 0000 007a 1d47 6974 4461 7461  ..r....z.GitData
+00003860: 4d67 6d74 2e67 6574 5f72 6570 6f73 6974  Mgmt.get_reposit
+00003870: 6f72 795f 6964 6302 0000 0000 0000 0000  ory_idc.........
+00003880: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
+00003890: 9400 0000 7400 6a01 a002 6401 a101 720c  ....t.j...d...r.
+000038a0: 7403 6402 6403 6404 8d02 5300 7c00 6a04  t.d.d.d...S.|.j.
+000038b0: a005 a100 7d02 7c02 a006 a100 7217 7c02  ....}.|.....r.|.
+000038c0: 5300 7c00 6a07 6a08 a009 a100 a00a 6405  S.|.j.j.......d.
+000038d0: a101 7d03 7c00 6a04 a00b 7c01 7c03 a102  ..}.|.j...|.|...
+000038e0: 7d02 7c02 a006 a100 722d 7c02 5300 7c00  }.|.....r-|.S.|.
+000038f0: 6a04 a00c a100 7d02 7c02 a006 a100 7238  j.....}.|.....r8
+00003900: 7c02 5300 7c00 6a07 a00d 6406 6407 a102  |.S.|.j...d.d...
+00003910: 0100 7c00 6a07 a00e a100 0100 7403 6408  ..|.j.......t.d.
+00003920: 6409 6404 8d02 5300 290a 4e72 1d00 0000  d.d...S.).Nr....
+00003930: 728f 0000 00fa 2546 6f6c 6465 7220 6973  r.....%Folder is
+00003940: 2061 6c72 6561 6479 2061 6e20 6f62 6973   already an obis
+00003950: 2072 6570 6f73 6974 6f72 792e 7291 0000   repository.r...
+00003960: 00da 1167 6974 5f61 6e6e 6578 5f62 6163  ...git_annex_bac
+00003970: 6b65 6e64 72c8 0000 0072 cc00 0000 7201  kendr....r....r.
+00003980: 0000 0072 9400 0000 290f 7223 0000 0072  ...r....).r#...r
+00003990: 2400 0000 7225 0000 0072 0500 0000 7236  $...r%...r....r6
+000039a0: 0000 00da 0867 6974 5f69 6e69 7472 b700  .....git_initr..
+000039b0: 0000 722e 0000 0072 0400 0000 7226 0000  ..r....r....r&..
+000039c0: 0072 d500 0000 da0e 6769 745f 616e 6e65  .r......git_anne
+000039d0: 785f 696e 6974 da0e 696e 6974 6961 6c5f  x_init..initial_
+000039e0: 636f 6d6d 6974 72c9 0000 00da 1463 6f70  commitr......cop
+000039f0: 795f 676c 6f62 616c 5f74 6f5f 6c6f 6361  y_global_to_loca
+00003a00: 6c29 0472 3c00 0000 724c 0000 0072 bb00  l).r<...rL...r..
+00003a10: 0000 72db 0000 0072 1f00 0000 721f 0000  ..r....r....r...
+00003a20: 0072 3700 0000 724d 0000 00af 0100 0073  .r7...rM.......s
+00003a30: 1e00 0000 0c02 0c01 0a01 0801 0401 1201  ................
+00003a40: 0e01 0801 0401 0a01 0801 0401 0e02 0a01  ................
+00003a50: 0c01 7a15 4769 7444 6174 614d 676d 742e  ..z.GitDataMgmt.
+00003a60: 696e 6974 5f64 6174 6163 0300 0000 0000  init_datac......
+00003a70: 0000 0000 0000 0900 0000 0a00 0000 4300  ..............C.
+00003a80: 0000 7316 0100 007c 00a0 007c 01a1 017d  ..s....|...|...}
+00003a90: 037c 00a0 017c 01a1 0164 0075 0072 1274  .|...|...d.u.r.t
+00003aa0: 0264 0164 0264 038d 0253 007c 00a0 037c  .d.d.d...S.|...|
+00003ab0: 02a1 017d 047c 04a0 04a1 0072 1d7c 0453  ...}.|.....r.|.S
+00003ac0: 0074 056a 06a0 0774 05a0 08a1 007c 01a1  .t.j...t.....|..
+00003ad0: 027d 0574 05a0 08a1 007d 0674 097c 0683  .}.t.....}.t.|..
+00003ae0: 0174 097c 0583 016a 0a76 0072 5474 056a  .t.|...j.v.rTt.j
+00003af0: 06a0 0b7c 067c 05a1 027d 0774 0c7c 0183  ...|.|...}.t.|..
+00003b00: 018f 0e01 007c 006a 0da0 0e7c 07a1 0101  .....|.j...|....
+00003b10: 0057 0064 0004 0004 0083 0301 006e 0831  .W.d.........n.1
+00003b20: 0073 4f77 0101 0001 0001 0059 0001 007a  .sOw.......Y...z
+00003b30: 0d7c 006a 0f6a 106a 1164 047c 0364 0564  .|.j.j.j.d.|.d.d
+00003b40: 0664 078d 0401 0057 006e 2304 0074 1279  .d.....W.n#..t.y
+00003b50: 8401 007d 0801 007a 177c 006a 1364 0675  ...}...z.|.j.d.u
+00003b60: 0072 707c 0882 0174 0264 0164 0874 147c  .rp|...t.d.d.t.|
+00003b70: 0883 0117 0064 038d 0257 0006 0059 0064  .....d...W...Y.d
+00003b80: 007d 087e 0853 0064 007d 087e 0877 0177  .}.~.S.d.}.~.w.w
+00003b90: 0074 0264 0964 0a64 038d 0253 0029 0b4e  .t.d.d.d...S.).N
+00003ba0: 728f 0000 007a 5250 6172 656e 7420 6461  r....zRParent da
+00003bb0: 7461 2073 6574 206d 7573 7420 6265 2063  ta set must be c
+00003bc0: 6f6d 6d69 7474 6564 2074 6f20 6f70 656e  ommitted to open
+00003bd0: 4249 5320 6265 666f 7265 2063 7265 6174  BIS before creat
+00003be0: 696e 6720 616e 2061 6e61 6c79 7369 7320  ing an analysis 
+00003bf0: 6461 7461 2073 6574 2e72 9100 0000 725b  data set.r....r[
+00003c00: 0000 0072 7500 0000 5472 8d00 0000 7290  ...ru...Tr....r.
+00003c10: 0000 0072 0100 0000 7294 0000 0029 1572  ...r....r....).r
+00003c20: d600 0000 72d9 0000 0072 0500 0000 724d  ....r....r....rM
+00003c30: 0000 0072 b700 0000 7223 0000 0072 2400  ...r....r#...r$.
+00003c40: 0000 da04 6a6f 696e da06 6765 7463 7764  ....join..getcwd
+00003c50: 7202 0000 00da 0770 6172 656e 7473 da07  r......parents..
+00003c60: 7265 6c70 6174 6872 1300 0000 7236 0000  relpathr....r6..
+00003c70: 00da 0a67 6974 5f69 676e 6f72 6572 2e00  ...git_ignorer..
+00003c80: 0000 72d4 0000 0072 9600 0000 7297 0000  ..r....r....r...
+00003c90: 0072 3300 0000 7298 0000 0029 0972 3c00  .r3...r....).r<.
+00003ca0: 0000 7250 0000 0072 4c00 0000 da12 7061  ..rP...rL.....pa
+00003cb0: 7265 6e74 5f64 6174 615f 7365 745f 6964  rent_data_set_id
+00003cc0: 72bb 0000 00da 1170 6172 656e 745f 666f  r......parent_fo
+00003cd0: 6c64 6572 5f61 6273 da13 616e 616c 7973  lder_abs..analys
+00003ce0: 6973 5f66 6f6c 6465 725f 6162 73da 1861  is_folder_abs..a
+00003cf0: 6e61 6c79 7369 735f 666f 6c64 6572 5f72  nalysis_folder_r
+00003d00: 656c 6174 6976 6572 9a00 0000 721f 0000  elativer....r...
+00003d10: 0072 1f00 0000 7237 0000 0072 5100 0000  .r....r7...rQ...
+00003d20: c201 0000 7336 0000 000a 020e 0204 0102  ....s6..........
+00003d30: 0106 ff0a 0308 0104 0112 0308 0112 010e  ................
+00003d40: 010a 010e 011c ff02 040a 0104 0102 010a  ................
+00003d50: fe0e 030a 0104 0120 0108 8002 fd0c 057a  ....... .......z
+00003d60: 1947 6974 4461 7461 4d67 6d74 2e69 6e69  .GitDataMgmt.ini
+00003d70: 745f 616e 616c 7973 6973 6301 0000 0000  t_analysisc.....
+00003d80: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00003d90: 0000 0073 0800 0000 7c00 a000 a100 5300  ...s....|.....S.
+00003da0: 729b 0000 0029 01da 055f 7379 6e63 7245  r....)..._syncrE
+00003db0: 0000 0072 1f00 0000 721f 0000 0072 3700  ...r....r....r7.
+00003dc0: 0000 7256 0000 00e2 0100 0073 0200 0000  ..rV.......s....
+00003dd0: 0802 7a10 4769 7444 6174 614d 676d 742e  ..z.GitDataMgmt.
+00003de0: 7379 6e63 6301 0000 0000 0000 0000 0000  syncc...........
+00003df0: 0002 0000 0003 0000 0043 0000 0073 1400  .........C...s..
+00003e00: 0000 7400 7c00 7c00 6a01 8302 7d01 7c01  ..t.|.|.j...}.|.
+00003e10: a002 a100 5300 729b 0000 0029 0372 0c00  ....S.r....).r..
+00003e20: 0000 723b 0000 00da 0372 756e a902 723c  ..r;.....run..r<
+00003e30: 0000 00da 0363 6d64 721f 0000 0072 1f00  .....cmdr....r..
+00003e40: 0000 7237 0000 0072 e900 0000 e601 0000  ..r7...r........
+00003e50: f304 0000 000c 0108 017a 1147 6974 4461  .........z.GitDa
+00003e60: 7461 4d67 6d74 2e5f 7379 6e63 5463 0400  taMgmt._syncTc..
+00003e70: 0000 0000 0000 0000 0000 0500 0000 0300  ................
+00003e80: 0000 4300 0000 735c 0000 007c 0272 1a7c  ..C...s\...|.r.|
+00003e90: 006a 00a0 01a1 007d 047c 04a0 02a1 0072  .j.....}.|.....r
+00003ea0: 0d7c 0453 007c 006a 00a0 037c 046a 04a1  .|.S.|.j...|.j..
+00003eb0: 017d 047c 04a0 02a1 0072 1a7c 0453 007c  .}.|.....r.|.S.|
+00003ec0: 006a 00a0 057c 01a1 017d 047c 04a0 02a1  .j...|...}.|....
+00003ed0: 0072 267c 0453 007c 0372 2c7c 00a0 06a1  .r&|.S.|.r,|....
+00003ee0: 007d 047c 0453 0029 017a 2820 4769 7420  .}.|.S.).z( Git 
+00003ef0: 6164 642c 2063 6f6d 6d69 7420 616e 6420  add, commit and 
+00003f00: 7379 6e63 2077 6974 6820 6f70 656e 4249  sync with openBI
+00003f10: 532e 2029 0772 3600 0000 da12 6769 745f  S. ).r6.....git_
+00003f20: 746f 705f 6c65 7665 6c5f 7061 7468 72b7  top_level_pathr.
+00003f30: 0000 00da 0767 6974 5f61 6464 7293 0000  .....git_addr...
+00003f40: 00da 0a67 6974 5f63 6f6d 6d69 7472 e900  ...git_commitr..
+00003f50: 0000 2905 723c 0000 0072 5400 0000 7255  ..).r<...rT...rU
+00003f60: 0000 0072 5600 0000 72bb 0000 0072 1f00  ...rV...r....r..
+00003f70: 0000 721f 0000 0072 3700 0000 7257 0000  ..r....r7...rW..
+00003f80: 00ea 0100 0073 1a00 0000 0403 0a01 0801  .....s..........
+00003f90: 0401 0e01 0801 0401 0c01 0801 0402 0401  ................
+00003fa0: 0801 0401 7a12 4769 7444 6174 614d 676d  ....z.GitDataMgm
+00003fb0: 742e 636f 6d6d 6974 6301 0000 0000 0000  t.commitc.......
+00003fc0: 0000 0000 0004 0000 0008 0000 0043 0000  .............C..
+00003fd0: 0073 7a00 0000 7c00 6a00 a001 a100 7d01  .sz...|.j.....}.
+00003fe0: 7a0a 7402 7c00 8301 6a03 6401 6402 8d01  z.t.|...j.d.d...
+00003ff0: 7d02 5700 6e11 0400 7404 6a05 6a06 7920  }.W.n...t.j.j.y 
+00004000: 0100 0100 0100 7407 6403 6404 6405 8d02  ......t.d.d.d...
+00004010: 7d02 5900 6e01 7700 7c01 6a08 7d03 7c02  }.Y.n.w.|.j.}.|.
+00004020: a009 a100 7237 740a 7c03 8301 6406 6b04  ....r7t.|...d.k.
+00004030: 7232 7c03 6407 3700 7d03 7c03 7c02 6a08  r2|.d.7.}.|.|.j.
+00004040: 3700 7d03 7407 6406 7c03 6405 8d02 5300  7.}.t.d.|.d...S.
+00004050: 2908 4e54 2901 da09 696e 666f 5f6f 6e6c  ).NT)...info_onl
+00004060: 7972 8f00 0000 7a1d 436f 756c 6420 6e6f  yr....z.Could no
+00004070: 7420 636f 6e6e 6563 7420 746f 206f 7065  t connect to ope
+00004080: 6e42 4953 2e72 9100 0000 7201 0000 00da  nBIS.r....r.....
+00004090: 010a 290b 7236 0000 00da 0a67 6974 5f73  ..).r6.....git_s
+000040a0: 7461 7475 7372 0c00 0000 72ea 0000 00da  tatusr....r.....
+000040b0: 0872 6571 7565 7374 73da 0a65 7863 6570  .requests..excep
+000040c0: 7469 6f6e 73da 0f43 6f6e 6e65 6374 696f  tions..Connectio
+000040d0: 6e45 7272 6f72 7205 0000 0072 9300 0000  nErrorr....r....
+000040e0: 72b7 0000 00da 036c 656e 2904 723c 0000  r......len).r<..
+000040f0: 0072 f300 0000 da0b 7379 6e63 5f73 7461  .r......sync_sta
+00004100: 7475 7372 9300 0000 721f 0000 0072 1f00  tusr....r....r..
+00004110: 0000 7237 0000 0072 5800 0000 fc01 0000  ..r7...rX.......
+00004120: 7318 0000 000a 0102 0114 0110 0110 0102  s...............
+00004130: ff06 0208 010c 0108 010a 010c 017a 1247  .............z.G
+00004140: 6974 4461 7461 4d67 6d74 2e73 7461 7475  itDataMgmt.statu
+00004150: 7363 0100 0000 0000 0000 0000 0000 0100  sc..............
+00004160: 0000 0400 0000 4300 0000 7326 0000 007c  ......C...s&...|
+00004170: 006a 00a0 01a1 006a 027c 005f 037c 00a0  .j.....j.|._.|..
+00004180: 04a1 0001 0074 05a0 0664 0164 02a1 0201  .....t...d.d....
+00004190: 0064 0353 0029 047a 3a20 5374 6f72 6573  .d.S.).z: Stores
+000041a0: 2074 6865 2067 6974 2063 6f6d 6d69 7420   the git commit 
+000041b0: 6861 7368 2061 6e64 2063 6f70 6965 7320  hash and copies 
+000041c0: 7468 6520 6f62 6973 206d 6574 6164 6174  the obis metadat
+000041d0: 612e 2072 1d00 0000 fa12 2e6f 6269 735f  a. r.......obis_
+000041e0: 7265 7374 6f72 6570 6f69 6e74 4e29 0772  restorepointN).r
+000041f0: 3600 0000 da0f 6769 745f 636f 6d6d 6974  6.....git_commit
+00004200: 5f68 6173 6872 9300 0000 da18 7072 6576  _hashr......prev
+00004210: 696f 7573 5f67 6974 5f63 6f6d 6d69 745f  ious_git_commit_
+00004220: 6861 7368 72c5 0000 00da 0673 6875 7469  hashr......shuti
+00004230: 6cda 0863 6f70 7974 7265 6572 4500 0000  l..copytreerE...
+00004240: 721f 0000 0072 1f00 0000 7237 0000 0072  r....r....r7...r
+00004250: c300 0000 0902 0000 7306 0000 000e 0208  ........s.......
+00004260: 0110 017a 1c47 6974 4461 7461 4d67 6d74  ...z.GitDataMgmt
+00004270: 2e73 6574 5f72 6573 746f 7265 706f 696e  .set_restorepoin
+00004280: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
+00004290: 0000 0400 0000 4300 0000 7328 0000 007c  ......C...s(...|
+000042a0: 006a 00a0 017c 006a 02a1 0101 0074 03a0  .j...|.j.....t..
+000042b0: 0464 01a1 0101 0074 03a0 0564 0264 01a1  .d.....t...d.d..
+000042c0: 0201 0064 0353 0029 047a 4d20 5265 7365  ...d.S.).zM Rese
+000042d0: 7473 2074 6f20 7468 6520 7374 6f72 6564  ts to the stored
+000042e0: 2067 6974 2063 6f6d 6d69 7420 6861 7368   git commit hash
+000042f0: 2061 6e64 2072 6573 746f 7265 7320 7468   and restores th
+00004300: 6520 636f 7069 6564 206f 6269 7320 6d65  e copied obis me
+00004310: 7461 6461 7461 2e20 721d 0000 0072 f900  tadata. r....r..
+00004320: 0000 4e29 0672 3600 0000 da0c 6769 745f  ..N).r6.....git_
+00004330: 7265 7365 745f 746f 72fb 0000 0072 fc00  reset_tor....r..
+00004340: 0000 da06 726d 7472 6565 72fd 0000 0072  ....rmtreer....r
+00004350: 4500 0000 721f 0000 0072 1f00 0000 7237  E...r....r....r7
+00004360: 0000 0072 b000 0000 0f02 0000 7306 0000  ...r........s...
+00004370: 000e 020a 0110 017a 1347 6974 4461 7461  .......z.GitData
+00004380: 4d67 6d74 2e72 6573 746f 7265 6301 0000  Mgmt.restorec...
+00004390: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+000043a0: 0043 0000 0073 1e00 0000 7400 6a01 a002  .C...s....t.j...
+000043b0: 6401 a101 720d 7403 a004 6401 a101 0100  d...r.t...d.....
+000043c0: 6402 5300 6402 5300 2903 7a3b 2044 656c  d.S.d.S.).z; Del
+000043d0: 6574 6573 2074 6865 206f 6269 7320 6d65  etes the obis me
+000043e0: 7461 6461 7461 2063 6f70 792e 2054 6869  tadata copy. Thi
+000043f0: 7320 6d75 7374 2061 6c77 6179 7320 6265  s must always be
+00004400: 2064 6f6e 652e 2072 f900 0000 4e29 0572   done. r....N).r
+00004410: 2300 0000 7224 0000 0072 2500 0000 72fc  #...r$...r%...r.
+00004420: 0000 0072 ff00 0000 7245 0000 0072 1f00  ...r....rE...r..
+00004430: 0000 721f 0000 0072 3700 0000 72c5 0000  ..r....r7...r...
+00004440: 0015 0200 0073 0600 0000 0c02 0e01 04ff  .....s..........
+00004450: 7a1e 4769 7444 6174 614d 676d 742e 636c  z.GitDataMgmt.cl
+00004460: 6561 725f 7265 7374 6f72 6570 6f69 6e74  ear_restorepoint
+00004470: 6305 0000 0000 0000 0000 0000 0006 0000  c...............
+00004480: 0006 0000 0043 0000 00f3 1800 0000 7400  .....C........t.
+00004490: 7c00 7c01 7c02 7c03 7c04 8305 7d05 7c05  |.|.|.|.|...}.|.
+000044a0: a001 a100 5300 729b 0000 0029 0272 0700  ....S.r....).r..
+000044b0: 0000 72ea 0000 00a9 0672 3c00 0000 725b  ..r......r<...r[
+000044c0: 0000 0072 5c00 0000 725d 0000 0072 5e00  ...r\...r]...r^.
+000044d0: 0000 72ec 0000 0072 1f00 0000 721f 0000  ..r....r....r...
+000044e0: 0072 3700 0000 725f 0000 001a 0200 00f3  .r7...r_........
+000044f0: 0400 0000 1001 0801 7a11 4769 7444 6174  ........z.GitDat
+00004500: 614d 676d 742e 636c 6f6e 6563 0500 0000  aMgmt.clonec....
+00004510: 0000 0000 0000 0000 0600 0000 0600 0000  ................
+00004520: 4300 0000 7200 0100 0072 9b00 0000 2902  C...r....r....).
+00004530: 720a 0000 0072 ea00 0000 7201 0100 0072  r....r....r....r
+00004540: 1f00 0000 721f 0000 0072 3700 0000 7261  ....r....r7...ra
+00004550: 0000 001e 0200 0073 0400 0000 1002 0801  .......s........
+00004560: 7a10 4769 7444 6174 614d 676d 742e 6d6f  z.GitDataMgmt.mo
+00004570: 7665 6301 0000 0000 0000 0000 0000 0002  vec.............
+00004580: 0000 0002 0000 0043 0000 0073 1000 0000  .......C...s....
+00004590: 7400 7c00 8301 7d01 7c01 a001 a100 5300  t.|...}.|.....S.
+000045a0: 729b 0000 0029 0272 0600 0000 72ea 0000  r....).r....r...
+000045b0: 0072 eb00 0000 721f 0000 0072 1f00 0000  .r....r....r....
+000045c0: 7237 0000 0072 6200 0000 2302 0000 7304  r7...rb...#...s.
+000045d0: 0000 0008 0108 017a 1247 6974 4461 7461  .......z.GitData
+000045e0: 4d67 6d74 2e61 6464 7265 6663 0200 0000  Mgmt.addrefc....
+000045f0: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00004600: 4300 0000 7314 0000 0074 007c 007c 0164  C...s....t.|.|.d
+00004610: 018d 027d 027c 02a0 01a1 0053 0029 024e  ...}.|.....S.).N
+00004620: 2901 725b 0000 0029 0272 0d00 0000 72ea  ).r[...).r....r.
+00004630: 0000 0029 0372 3c00 0000 725b 0000 0072  ...).r<...r[...r
+00004640: ec00 0000 721f 0000 0072 1f00 0000 7237  ....r....r....r7
+00004650: 0000 0072 6400 0000 2702 0000 72ed 0000  ...rd...'...r...
+00004660: 007a 1547 6974 4461 7461 4d67 6d74 2e72  .z.GitDataMgmt.r
+00004670: 656d 6f76 6572 6566 6305 0000 0000 0000  emoverefc.......
+00004680: 0000 0000 0005 0000 0004 0000 0043 0000  .............C..
+00004690: 0072 a600 0000 2903 4e72 6800 0000 fa30  .r....).Nrh....0
+000046a0: 5468 6973 2063 6f6d 6d61 6e64 2069 7320  This command is 
+000046b0: 6f6e 6c79 2061 7661 696c 6162 6c65 2066  only available f
+000046c0: 6f72 204d 616e 6167 6572 2044 6174 612e  or Manager Data.
+000046d0: 72a8 0000 0072 6500 0000 721f 0000 0072  r....re...r....r
+000046e0: 1f00 0000 7237 0000 0072 6800 0000 2b02  ....r7...rh...+.
+000046f0: 0000 72a9 0000 007a 1447 6974 4461 7461  ..r....z.GitData
+00004700: 4d67 6d74 2e64 6f77 6e6c 6f61 6463 0700  Mgmt.downloadc..
+00004710: 0000 0000 0000 0000 0000 0800 0000 0900  ................
+00004720: 0000 4300 0000 738a 0000 007c 006a 00a0  ..C...s....|.j..
+00004730: 017c 01a1 017d 077c 0764 0175 0072 1074  .|...}.|.d.u.r.t
+00004740: 0264 027c 0117 0083 0182 017c 0474 036a  .d.|.......|.t.j
+00004750: 0475 0072 227c 0564 0175 0173 1b4a 0082  .u.r"|.d.u.s.J..
+00004760: 017c 0664 0175 0173 214a 0082 016e 177c  .|.d.u.s!J...n.|
+00004770: 0474 036a 0575 0072 2e7c 0664 0175 0073  .t.j.u.r.|.d.u.s
+00004780: 2d4a 0082 016e 0b7c 0474 036a 0675 0072  -J...n.|.t.j.u.r
+00004790: 397c 0664 0175 0073 394a 0082 017c 00a0  9|.d.u.s9J...|..
+000047a0: 077c 077c 006a 087c 027c 037c 047c 057c  .|.|.j.|.|.|.|.|
+000047b0: 06a1 0753 0029 03e1 8501 0000 0a20 2020  ...S.).......   
+000047c0: 2020 2020 203a 7061 7261 6d20 6361 7465       :param cate
+000047d0: 676f 7279 3a20 636f 6e66 6967 2c20 6f62  gory: config, ob
+000047e0: 6a65 6374 2c20 636f 6c6c 6563 7469 6f6e  ject, collection
+000047f0: 2c20 6461 7461 5f73 6574 206f 7220 7265  , data_set or re
+00004800: 706f 7369 746f 7279 0a20 2020 2020 2020  pository.       
+00004810: 203a 7061 7261 6d20 6973 5f67 6c6f 6261   :param is_globa
+00004820: 6c3a 2061 6374 206f 6e20 676c 6f62 616c  l: act on global
+00004830: 2073 6574 7469 6e67 7320 2d20 6c6f 6361   settings - loca
+00004840: 6c20 6966 2066 616c 7365 0a20 2020 2020  l if false.     
+00004850: 2020 203a 7061 7261 6d20 6973 5f64 6174     :param is_dat
+00004860: 615f 7365 745f 7072 6f70 6572 7479 3a20  a_set_property: 
+00004870: 7472 7565 2069 6620 7072 6f70 202f 2076  true if prop / v
+00004880: 616c 7565 2061 7265 2061 2064 6174 6120  alue are a data 
+00004890: 7365 7420 7072 6f70 6572 7479 0a20 2020  set property.   
+000048a0: 2020 2020 203a 7061 7261 6d20 6f70 6572       :param oper
+000048b0: 6174 696f 6e5f 7479 7065 3a20 7479 7065  ation_type: type
+000048c0: 206f 6620 6f70 6572 6174 696f 6e20 746f   of operation to
+000048d0: 2070 6572 666f 726d 2e20 4974 2063 616e   perform. It can
+000048e0: 2062 6520 4745 542c 2053 4554 2c20 434c   be GET, SET, CL
+000048f0: 4541 520a 2020 2020 2020 2020 3a70 6172  EAR.        :par
+00004900: 616d 2070 726f 703a 2073 6574 7469 6e67  am prop: setting
+00004910: 206b 6579 0a20 2020 2020 2020 203a 7061   key.        :pa
+00004920: 7261 6d20 7661 6c75 653a 2073 6574 7469  ram value: setti
+00004930: 6e67 2076 616c 7565 0a20 2020 2020 2020  ng value.       
+00004940: 204e fa1b 496e 7661 6c69 6420 7365 7474   N..Invalid sett
+00004950: 696e 6773 2063 6174 6567 6f72 793a 2029  ings category: )
+00004960: 0972 2e00 0000 72d5 0000 0072 3f00 0000  .r....r....r?...
+00004970: 7212 0000 0072 7f00 0000 727b 0000 0072  r....r....r{...r
+00004980: 8100 0000 728c 0000 0072 3300 0000 2908  ....r....r3...).
+00004990: 723c 0000 00da 0863 6174 6567 6f72 7972  r<.....categoryr
+000049a0: 8400 0000 7285 0000 0072 8600 0000 7287  ....r....r....r.
+000049b0: 0000 0072 8800 0000 7283 0000 0072 1f00  ...r....r....r..
+000049c0: 0000 721f 0000 0072 3700 0000 7204 0000  ..r....r7...r...
+000049d0: 0032 0200 0073 1a00 0000 0c0a 0801 0c01  .2...s..........
+000049e0: 0a01 0c01 0e01 0a01 0e01 0a01 0c01 0e02  ................
+000049f0: 0601 04ff 7a12 4769 7444 6174 614d 676d  ....z.GitDataMgm
+00004a00: 742e 636f 6e66 6967 6301 0000 0000 0000  t.configc.......
+00004a10: 0000 0000 0002 0000 0004 0000 0047 0000  .............G..
+00004a20: 0072 a600 0000 a903 4e72 af00 0000 7203  .r......Nr....r.
+00004a30: 0100 0072 a800 0000 72ac 0000 0072 1f00  ...r....r....r..
+00004a40: 0000 721f 0000 0072 3700 0000 7272 0000  ..r....r7...rr..
+00004a50: 004a 0200 0072 a900 0000 7a19 4769 7444  .J...r....z.GitD
+00004a60: 6174 614d 676d 742e 7365 6172 6368 5f6f  ataMgmt.search_o
+00004a70: 626a 6563 7463 0100 0000 0000 0000 0000  bjectc..........
+00004a80: 0000 0200 0000 0400 0000 4700 0000 72a6  ..........G...r.
+00004a90: 0000 0072 0701 0000 72a8 0000 0072 ac00  ...r....r....r..
+00004aa0: 0000 721f 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
+00004ab0: 0072 7300 0000 4d02 0000 72a9 0000 007a  .rs...M...r....z
+00004ac0: 1b47 6974 4461 7461 4d67 6d74 2e73 6561  .GitDataMgmt.sea
+00004ad0: 7263 685f 6461 7461 5f73 6574 6301 0000  rch_data_setc...
+00004ae0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00004af0: 0047 0000 0072 a600 0000 2903 4e72 6d00  .G...r....).Nrm.
+00004b00: 0000 7203 0100 0072 a800 0000 72ac 0000  ..r....r....r...
+00004b10: 0072 1f00 0000 721f 0000 0072 3700 0000  .r....r....r7...
+00004b20: 726d 0000 0050 0200 0072 a900 0000 7a12  rm...P...r....z.
+00004b30: 4769 7444 6174 614d 676d 742e 7570 6c6f  GitDataMgmt.uplo
+00004b40: 6164 729b 0000 0072 9c00 0000 729d 0000  adr....r....r...
+00004b50: 0029 1c72 9e00 0000 729f 0000 0072 a000  .).r....r....r..
+00004b60: 0000 72a1 0000 0072 4600 0000 724a 0000  ..r....rF...rJ..
+00004b70: 0072 d600 0000 72d9 0000 0072 4d00 0000  .r....r....rM...
+00004b80: 7251 0000 0072 c700 0000 7256 0000 0072  rQ...r....rV...r
+00004b90: e900 0000 7257 0000 0072 5800 0000 72c3  ....rW...rX...r.
+00004ba0: 0000 0072 b000 0000 72c5 0000 0072 5f00  ...r....r....r_.
+00004bb0: 0000 72bf 0000 0072 6100 0000 7262 0000  ..r....ra...rb..
+00004bc0: 0072 6400 0000 7268 0000 0072 0400 0000  .rd...rh...r....
+00004bd0: 7272 0000 0072 7300 0000 726d 0000 0072  rr...rs...rm...r
+00004be0: 1f00 0000 721f 0000 0072 1f00 0000 7237  ....r....r....r7
+00004bf0: 0000 0072 2c00 0000 9401 0000 733a 0000  ...r,.......s:..
+00004c00: 0008 0004 010a 0208 0908 0708 040a 040a  ................
+00004c10: 1302 200a 0108 0302 040c 0108 1108 0d08  .. .............
+00004c20: 0608 0608 0502 040a 0108 040a 0408 0402  ................
+00004c30: 0702 010a ff08 1808 030c 0372 2c00 0000  ...........r,...
+00004c40: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00004c50: 0003 0000 0040 0000 0073 a000 0000 6500  .....@...s....e.
+00004c60: 5a01 6400 5a02 6401 5a03 6402 6403 8400  Z.d.Z.d.Z.d.d...
+00004c70: 5a04 6404 6405 8400 5a05 6424 6407 6408  Z.d.d...Z.d$d.d.
+00004c80: 8401 5a06 6424 6409 640a 8401 5a07 6425  ..Z.d$d.d...Z.d%
+00004c90: 640c 640d 8401 5a08 640e 640f 8400 5a09  d.d...Z.d.d...Z.
+00004ca0: 6410 6411 8400 5a0a 6412 6413 8400 5a0b  d.d...Z.d.d...Z.
+00004cb0: 6414 6415 8400 5a0c 6416 6417 8400 5a0d  d.d...Z.d.d...Z.
+00004cc0: 6424 6418 6419 8401 5a0e 641a 641b 8400  d$d.d...Z.d.d...
+00004cd0: 5a0f 6424 641c 641d 8401 5a10 641e 641f  Z.d$d.d...Z.d.d.
+00004ce0: 8400 5a11 6420 6421 8400 5a12 0906 0906  ..Z.d d!..Z.....
+00004cf0: 6426 6422 6423 8401 5a13 6406 5300 2927  d&d"d#..Z.d.S.)'
+00004d00: 7229 0000 007a 2844 6174 614d 676d 7420  r)...z(DataMgmt 
+00004d10: 6f70 6572 6174 696f 6e73 2066 6f72 2044  operations for D
+00004d20: 5353 2d73 746f 7265 6420 6461 7461 2e63  SS-stored data.c
+00004d30: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00004d40: 0200 0000 4300 0000 7308 0000 0074 00a0  ....C...s....t..
+00004d50: 01a1 0053 0072 9b00 0000 2902 7220 0000  ...S.r....).r ..
+00004d60: 0072 2100 0000 7245 0000 0072 1f00 0000  .r!...rE...r....
+00004d70: 721f 0000 0072 3700 0000 7246 0000 0057  r....r7...rF...W
+00004d80: 0200 0073 0200 0000 0801 7a26 5068 7973  ...s......z&Phys
+00004d90: 6963 616c 4461 7461 4d67 6d74 2e67 6574  icalDataMgmt.get
+00004da0: 5f73 6574 7469 6e67 735f 7265 736f 6c76  _settings_resolv
+00004db0: 6572 6302 0000 0000 0000 0000 0000 0002  erc.............
+00004dc0: 0000 0004 0000 0043 0000 0072 a600 0000  .......C...r....
+00004dd0: 2903 4e72 aa00 0000 fa38 5468 6973 2063  ).Nr.....8This c
+00004de0: 6f6d 6d61 6e64 2069 7320 6f6e 6c79 2061  ommand is only a
+00004df0: 7661 696c 6162 6c65 2066 6f72 2045 7874  vailable for Ext
+00004e00: 6572 6e61 6c20 4d61 6e61 6765 7220 4461  ernal Manager Da
+00004e10: 7461 72a8 0000 0072 4800 0000 721f 0000  tar....rH...r...
+00004e20: 0072 1f00 0000 7237 0000 0072 4a00 0000  .r....r7...rJ...
+00004e30: 5a02 0000 f306 0000 0006 0102 0108 ff7a  Z..............z
+00004e40: 2550 6879 7369 6361 6c44 6174 614d 676d  %PhysicalDataMgm
+00004e50: 742e 7365 7475 705f 6c6f 6361 6c5f 7365  t.setup_local_se
+00004e60: 7474 696e 6773 4e63 0200 0000 0000 0000  ttingsNc........
+00004e70: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
+00004e80: 7364 0000 0074 006a 01a0 0264 01a1 0172  sd...t.j...d...r
+00004e90: 0c74 0364 0264 0364 048d 0253 007c 006a  .t.d.d.d...S.|.j
+00004ea0: 046a 05a0 06a1 0001 007c 006a 046a 05a0  .j.......|.j.j..
+00004eb0: 0764 0564 0664 07a1 0301 007c 006a 046a  .d.d.d.....|.j.j
+00004ec0: 05a0 08a1 0064 0819 007d 027c 006a 046a  .....d...}.|.j.j
+00004ed0: 05a0 0764 097c 0264 07a1 0301 0074 0364  ...d.|.d.....t.d
+00004ee0: 0a64 0b64 048d 0253 0029 0c4e 721d 0000  .d.d...S.).Nr...
+00004ef0: 0072 8f00 0000 72da 0000 0072 9100 0000  .r....r....r....
+00004f00: 721e 0000 0054 7275 0000 00da 0b6f 7065  r....Tru.....ope
+00004f10: 6e62 6973 5f75 726c da0f 6669 6c65 7365  nbis_url..filese
+00004f20: 7276 6963 655f 7572 6c72 0100 0000 7a29  rvice_urlr....z)
+00004f30: 4d61 6e61 6765 6420 6461 7461 206f 6269  Managed data obi
+00004f40: 7320 7265 706f 7369 746f 7279 2069 6e69  s repository ini
+00004f50: 7469 616c 697a 6564 2e29 0972 2300 0000  tialized.).r#...
+00004f60: 7224 0000 0072 2500 0000 7205 0000 0072  r$...r%...r....r
+00004f70: 2e00 0000 7204 0000 0072 df00 0000 7296  ....r....r....r.
+00004f80: 0000 0072 2600 0000 2903 723c 0000 0072  ...r&...).r<...r
+00004f90: 4c00 0000 720a 0100 0072 1f00 0000 721f  L...r....r....r.
+00004fa0: 0000 0072 3700 0000 724d 0000 005e 0200  ...r7...rM...^..
+00004fb0: 0073 1200 0000 0c01 0c01 0c01 1201 1001  .s..............
+00004fc0: 0a01 0401 04ff 0c02 7a1a 5068 7973 6963  ........z.Physic
+00004fd0: 616c 4461 7461 4d67 6d74 2e69 6e69 745f  alDataMgmt.init_
+00004fe0: 6461 7461 6303 0000 0000 0000 0000 0000  datac...........
+00004ff0: 0003 0000 0004 0000 0043 0000 0072 a600  .........C...r..
+00005000: 0000 2903 4e72 ab00 0000 7208 0100 0072  ..).Nr....r....r
+00005010: a800 0000 724f 0000 0072 1f00 0000 721f  ....rO...r....r.
+00005020: 0000 0072 3700 0000 7251 0000 0068 0200  ...r7...rQ...h..
+00005030: 0072 0901 0000 7a1e 5068 7973 6963 616c  .r....z.Physical
+00005040: 4461 7461 4d67 6d74 2e69 6e69 745f 616e  DataMgmt.init_an
+00005050: 616c 7973 6973 5463 0400 0000 0000 0000  alysisTc........
+00005060: 0000 0000 0400 0000 0400 0000 4300 0000  ............C...
+00005070: 72a6 0000 0029 034e 7257 0000 0072 0801  r....).NrW...r..
+00005080: 0000 72a8 0000 0072 5300 0000 721f 0000  ..r....rS...r...
+00005090: 0072 1f00 0000 7237 0000 0072 5700 0000  .r....r7...rW...
+000050a0: 6c02 0000 72a9 0000 007a 1750 6879 7369  l...r....z.Physi
+000050b0: 6361 6c44 6174 614d 676d 742e 636f 6d6d  calDataMgmt.comm
+000050c0: 6974 6301 0000 0000 0000 0000 0000 0001  itc.............
+000050d0: 0000 0004 0000 0043 0000 0072 a600 0000  .......C...r....
+000050e0: 2903 4e72 5600 0000 7208 0100 0072 a800  ).NrV...r....r..
+000050f0: 0000 7245 0000 0072 1f00 0000 721f 0000  ..rE...r....r...
+00005100: 0072 3700 0000 7256 0000 006f 0200 0072  .r7...rV...o...r
+00005110: a900 0000 7a15 5068 7973 6963 616c 4461  ....z.PhysicalDa
+00005120: 7461 4d67 6d74 2e73 796e 6363 0100 0000  taMgmt.syncc....
+00005130: 0000 0000 0000 0000 0100 0000 0400 0000  ................
+00005140: 4300 0000 72a6 0000 0029 034e 7258 0000  C...r....).NrX..
+00005150: 0072 0801 0000 72a8 0000 0072 4500 0000  .r....r....rE...
+00005160: 721f 0000 0072 1f00 0000 7237 0000 0072  r....r....r7...r
+00005170: 5800 0000 7202 0000 72a9 0000 007a 1750  X...r...r....z.P
+00005180: 6879 7369 6361 6c44 6174 614d 676d 742e  hysicalDataMgmt.
+00005190: 7374 6174 7573 6305 0000 0000 0000 0000  statusc.........
+000051a0: 0000 0005 0000 0004 0000 0043 0000 0072  ...........C...r
+000051b0: a600 0000 2903 4e72 5f00 0000 7208 0100  ....).Nr_...r...
+000051c0: 0072 a800 0000 725a 0000 0072 1f00 0000  .r....rZ...r....
+000051d0: 721f 0000 0072 3700 0000 725f 0000 0075  r....r7...r_...u
+000051e0: 0200 0072 a900 0000 7a16 5068 7973 6963  ...r....z.Physic
+000051f0: 616c 4461 7461 4d67 6d74 2e63 6c6f 6e65  alDataMgmt.clone
+00005200: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
+00005210: 0004 0000 0043 0000 0072 a600 0000 2903  .....C...r....).
+00005220: 4e72 6100 0000 7208 0100 0072 a800 0000  Nra...r....r....
+00005230: 725a 0000 0072 1f00 0000 721f 0000 0072  rZ...r....r....r
+00005240: 3700 0000 7261 0000 0078 0200 0072 a900  7...ra...x...r..
+00005250: 0000 7a15 5068 7973 6963 616c 4461 7461  ..z.PhysicalData
+00005260: 4d67 6d74 2e6d 6f76 6563 0100 0000 0000  Mgmt.movec......
+00005270: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+00005280: 0000 72a6 0000 0029 034e 7262 0000 0072  ..r....).Nrb...r
+00005290: 0801 0000 72a8 0000 0072 4500 0000 721f  ....r....rE...r.
+000052a0: 0000 0072 1f00 0000 7237 0000 0072 6200  ...r....r7...rb.
+000052b0: 0000 7b02 0000 72a9 0000 007a 1750 6879  ..{...r....z.Phy
+000052c0: 7369 6361 6c44 6174 614d 676d 742e 6164  sicalDataMgmt.ad
+000052d0: 6472 6566 6302 0000 0000 0000 0000 0000  drefc...........
+000052e0: 0002 0000 0004 0000 0043 0000 0072 a600  .........C...r..
+000052f0: 0000 2903 4e72 6400 0000 7208 0100 0072  ..).Nrd...r....r
+00005300: a800 0000 7263 0000 0072 1f00 0000 721f  ....rc...r....r.
+00005310: 0000 0072 3700 0000 7264 0000 007e 0200  ...r7...rd...~..
+00005320: 0072 a900 0000 7a1a 5068 7973 6963 616c  .r....z.Physical
+00005330: 4461 7461 4d67 6d74 2e72 656d 6f76 6572  DataMgmt.remover
+00005340: 6566 6305 0000 0000 0000 0000 0000 0006  efc.............
+00005350: 0000 0006 0000 0043 0000 0072 0001 0000  .......C...r....
+00005360: 729b 0000 0029 0272 0900 0000 72ea 0000  r....).r....r...
+00005370: 0029 0672 3c00 0000 725b 0000 0072 6600  .).r<...r[...rf.
+00005380: 0000 7267 0000 0072 5e00 0000 72ec 0000  ..rg...r^...r...
+00005390: 0072 1f00 0000 721f 0000 0072 3700 0000  .r....r....r7...
+000053a0: 7268 0000 0081 0200 0072 0201 0000 7a19  rh.......r....z.
+000053b0: 5068 7973 6963 616c 4461 7461 4d67 6d74  PhysicalDataMgmt
+000053c0: 2e64 6f77 6e6c 6f61 6463 0500 0000 0000  .downloadc......
+000053d0: 0000 0000 0000 0600 0000 0600 0000 4300  ..............C.
+000053e0: 0000 7200 0100 0072 9b00 0000 2902 720f  ..r....r....).r.
+000053f0: 0000 0072 ea00 0000 2906 723c 0000 0072  ...r....).r<...r
+00005400: 6900 0000 726a 0000 0072 6b00 0000 726c  i...rj...rk...rl
+00005410: 0000 0072 ec00 0000 721f 0000 0072 1f00  ...r....r....r..
+00005420: 0000 7237 0000 0072 6d00 0000 8502 0000  ..r7...rm.......
+00005430: 7202 0100 007a 1750 6879 7369 6361 6c44  r....z.PhysicalD
+00005440: 6174 614d 676d 742e 7570 6c6f 6164 6304  ataMgmt.uploadc.
+00005450: 0000 0000 0000 0000 0000 0005 0000 0005  ................
+00005460: 0000 0043 0000 00f3 1600 0000 7400 7c00  ...C........t.|.
+00005470: 7c01 7c02 7c03 8304 7d04 7c04 a001 a100  |.|.|...}.|.....
+00005480: 5300 729b 0000 0029 0272 0e00 0000 da0e  S.r....).r......
+00005490: 7365 6172 6368 5f73 616d 706c 6573 a905  search_samples..
+000054a0: 723c 0000 0072 6f00 0000 7270 0000 0072  r<...ro...rp...r
+000054b0: 7100 0000 72ec 0000 0072 1f00 0000 721f  q...r....r....r.
+000054c0: 0000 0072 3700 0000 7272 0000 0089 0200  ...r7...rr......
+000054d0: 00f3 0400 0000 0e01 0801 7a1e 5068 7973  ..........z.Phys
+000054e0: 6963 616c 4461 7461 4d67 6d74 2e73 6561  icalDataMgmt.sea
+000054f0: 7263 685f 6f62 6a65 6374 6304 0000 0000  rch_objectc.....
+00005500: 0000 0000 0000 0005 0000 0005 0000 0043  ...............C
+00005510: 0000 0072 0c01 0000 729b 0000 0029 0272  ...r....r....).r
+00005520: 0e00 0000 da10 7365 6172 6368 5f64 6174  ......search_dat
+00005530: 615f 7365 7473 720e 0100 0072 1f00 0000  a_setsr....r....
+00005540: 721f 0000 0072 3700 0000 7273 0000 008d  r....r7...rs....
+00005550: 0200 0072 0f01 0000 7a20 5068 7973 6963  ...r....z Physic
+00005560: 616c 4461 7461 4d67 6d74 2e73 6561 7263  alDataMgmt.searc
+00005570: 685f 6461 7461 5f73 6574 6307 0000 0000  h_data_setc.....
+00005580: 0000 0000 0000 0009 0000 0009 0000 0043  ...............C
+00005590: 0000 0073 f600 0000 7c00 6a00 a001 7c01  ...s....|.j...|.
+000055a0: a101 7d07 7c07 6401 7500 7210 7402 6402  ..}.|.d.u.r.t.d.
+000055b0: 7c01 1700 8301 8201 7c04 7403 6a04 7500  |.......|.t.j.u.
+000055c0: 7222 7c05 6401 7501 731b 4a00 8201 7c06  r"|.d.u.s.J...|.
+000055d0: 6401 7501 7321 4a00 8201 6e1e 7c04 7403  d.u.s!J...n.|.t.
+000055e0: 6a05 7500 722e 7c06 6401 7500 732d 4a00  j.u.r.|.d.u.s-J.
+000055f0: 8201 6e12 7c04 7403 6a06 7500 7240 7c01  ..n.|.t.j.u.r@|.
+00005600: 6403 6b03 7240 7c00 a007 7c01 9b00 6404  d.k.r@|...|...d.
+00005610: 9d02 6405 a102 0100 7c01 6406 6b02 724f  ..d.....|.d.k.rO
+00005620: 7408 7c00 7c04 7c05 7c06 8304 7d08 7c08  t.|.|.|.|...}.|.
+00005630: a009 a100 5300 7c01 6407 6b02 725e 740a  ....S.|.d.k.r^t.
+00005640: 7c00 7c04 7c05 7c06 8304 7d08 7c08 a009  |.|.|.|...}.|...
+00005650: a100 5300 7c01 6403 6b02 726e 7c00 a00b  ..S.|.d.k.rn|...
+00005660: 7c07 7c00 6a0c 7c02 7c03 7c04 7c05 7c06  |.|.j.|.|.|.|.|.
+00005670: a107 5300 7c00 a007 7c01 9b00 6408 7c04  ..S.|...|...d.|.
+00005680: 9b00 9d03 6405 a102 0100 6401 5300 2909  ....d.....d.S.).
+00005690: 7204 0100 004e 7205 0100 0072 0400 0000  r....Nr....r....
+000056a0: 7a06 2063 6c65 6172 7208 0100 00da 066f  z. clearr......o
+000056b0: 626a 6563 74da 0a63 6f6c 6c65 6374 696f  bject..collectio
+000056c0: 6efa 0120 290d 722e 0000 0072 d500 0000  n.. ).r....r....
+000056d0: 723f 0000 0072 1200 0000 727f 0000 0072  r?...r....r....r
+000056e0: 7b00 0000 7281 0000 0072 4300 0000 720b  {...r....rC...r.
+000056f0: 0000 0072 ea00 0000 7208 0000 0072 8c00  ...r....r....r..
+00005700: 0000 7233 0000 0029 0972 3c00 0000 7206  ..r3...).r<...r.
+00005710: 0100 0072 8400 0000 7285 0000 0072 8600  ...r....r....r..
+00005720: 0000 7287 0000 0072 8800 0000 7283 0000  ..r....r....r...
+00005730: 0072 ec00 0000 721f 0000 0072 1f00 0000  .r....r....r....
+00005740: 7237 0000 0072 0400 0000 9102 0000 7332  r7...r........s2
+00005750: 0000 000c 0a08 010c 010a 010c 010e 010a  ................
+00005760: 010e 0112 010c 0102 0104 ff08 030e 0108  ................
+00005770: 0108 010e 0108 0108 010e 0106 0104 ff10  ................
+00005780: 0302 0108 ff7a 1750 6879 7369 6361 6c44  .....z.PhysicalD
+00005790: 6174 614d 676d 742e 636f 6e66 6967 729b  ataMgmt.configr.
+000057a0: 0000 0072 9c00 0000 729d 0000 0029 1472  ...r....r....).r
+000057b0: 9e00 0000 729f 0000 0072 a000 0000 72a1  ....r....r....r.
+000057c0: 0000 0072 4600 0000 724a 0000 0072 4d00  ...rF...rJ...rM.
+000057d0: 0000 7251 0000 0072 5700 0000 7256 0000  ..rQ...rW...rV..
+000057e0: 0072 5800 0000 725f 0000 0072 6100 0000  .rX...r_...ra...
+000057f0: 7262 0000 0072 6400 0000 7268 0000 0072  rb...rd...rh...r
+00005800: 6d00 0000 7272 0000 0072 7300 0000 7204  m...rr...rs...r.
+00005810: 0000 0072 1f00 0000 721f 0000 0072 1f00  ...r....r....r..
+00005820: 0000 7237 0000 0072 2900 0000 5402 0000  ..r7...r)...T...
+00005830: 7328 0000 0008 0004 0108 0208 030a 040a  s(..............
+00005840: 0a0a 0408 0308 0308 0308 0308 030a 0308  ................
+00005850: 030a 0408 0408 0402 0402 010e ff72 2900  .............r).
+00005860: 0000 2938 72a2 0000 0072 7c00 0000 7223  ..)8r....r|...r#
+00005870: 0000 0072 fc00 0000 72c0 0000 0072 b100  ...r....r....r..
+00005880: 0000 da07 7061 7468 6c69 6272 0200 0000  ....pathlibr....
+00005890: 72f4 0000 0072 9400 0000 7204 0000 0072  r....r....r....r
+000058a0: 2000 0000 da0e 636f 6d6d 616e 645f 7265   .....command_re
+000058b0: 7375 6c74 7205 0000 00da 0f63 6f6d 6d61  sultr......comma
+000058c0: 6e64 732e 6164 6472 6566 7206 0000 00da  nds.addrefr.....
+000058d0: 0e63 6f6d 6d61 6e64 732e 636c 6f6e 6572  .commands.cloner
+000058e0: 0700 0000 da13 636f 6d6d 616e 6473 2e63  ......commands.c
+000058f0: 6f6c 6c65 6374 696f 6e72 0800 0000 da1a  ollectionr......
+00005900: 636f 6d6d 616e 6473 2e64 6f77 6e6c 6f61  commands.downloa
+00005910: 645f 7068 7973 6963 616c 7209 0000 00da  d_physicalr.....
+00005920: 0d63 6f6d 6d61 6e64 732e 6d6f 7665 720a  .commands.mover.
+00005930: 0000 00da 0f63 6f6d 6d61 6e64 732e 6f62  .....commands.ob
+00005940: 6a65 6374 720b 0000 00da 1563 6f6d 6d61  jectr......comma
+00005950: 6e64 732e 6f70 656e 6269 735f 7379 6e63  nds.openbis_sync
+00005960: 720c 0000 00da 1263 6f6d 6d61 6e64 732e  r......commands.
+00005970: 7265 6d6f 7665 7265 6672 0d00 0000 da0f  removerefr......
+00005980: 636f 6d6d 616e 6473 2e73 6561 7263 6872  commands.searchr
+00005990: 0e00 0000 da0f 636f 6d6d 616e 6473 2e75  ......commands.u
+000059a0: 706c 6f61 6472 0f00 0000 da03 6769 7472  ploadr......gitr
+000059b0: 1000 0000 da05 7574 696c 7372 1100 0000  ......utilsr....
+000059c0: 7212 0000 0072 1300 0000 7214 0000 0072  r....r....r....r
+000059d0: 1500 0000 7216 0000 00da 1273 6372 6970  ....r......scrip
+000059e0: 7473 2e63 6c69 636b 5f75 7469 6c72 1800  ts.click_utilr..
+000059f0: 0000 7219 0000 0072 2200 0000 7238 0000  ..r....r"...r8..
+00005a00: 00da 0741 4243 4d65 7461 7239 0000 0072  ...ABCMetar9...r
+00005a10: 2b00 0000 72b4 0000 0072 bf00 0000 72c7  +...r....r....r.
+00005a20: 0000 0072 2c00 0000 7229 0000 0072 1f00  ...r,...r)...r..
+00005a30: 0000 721f 0000 0072 1f00 0000 7237 0000  ..r....r....r7..
+00005a40: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00005a50: 4e00 0000 0811 0801 0801 0801 0801 0801  N...............
+00005a60: 0c01 0802 0c02 0c01 0c01 0c01 0c01 0c01  ................
+00005a70: 0c01 0c01 0c01 0c01 0c01 0c01 0c01 1001  ................
+00005a80: 0c01 0c01 0c01 0c01 1001 0804 0c01 0aff  ................
+00005a90: 1429 007f 105b 0831 0805 0812 1017 007f  .)...[.1........
+00005aa0: 1441                                     .A
```

### Comparing `obis-0.4.5/obis/dm/__pycache__/git.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/__pycache__/git.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 30 10:32:13 2023 UTC, .py size: 8502 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2d65 2564 3621 0000  o.......-e%d6!..
+00000000: 6f0d 0d0a 0000 0000 554f 0166 3621 0000  o.......UO.f6!..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5c00 0000 6400  .....@...s\...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 0100 6402  d.l.m.Z.m.Z...d.
 00000050: 6404 6c05 6d06 5a06 0100 6405 6406 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 4700 6407 6408 8400 6408  m.Z...G.d.d...d.
 00000070: 6509 8303 5a0a 4700 6409 640a 8400 640a  e...Z.G.d.d...d.
```

### Comparing `obis-0.4.5/obis/dm/__pycache__/repository_utils.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/__pycache__/repository_utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb 21 12:05:41 2023 UTC, .py size: 1905 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 95b3 f463 7107 0000  o..........cq...
+00000000: 6f0d 0d0a 0000 0000 554f 0166 7107 0000  o.......UO.fq...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 4c00 0000 6400  .....@...sL...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 0100 6402 6404 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6405 6406 8400 5a06 6407  m.Z...d.d...Z.d.
 00000060: 6408 8400 5a07 6409 640a 8400 5a08 640b  d...Z.d.d...Z.d.
 00000070: 640c 8400 5a09 6401 5300 290d e900 0000  d...Z.d.S.).....
```

### Comparing `obis-0.4.5/obis/dm/__pycache__/utils.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 30 10:51:34 2023 UTC, .py size: 3789 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b669 2564 cd0e 0000  o........i%d....
+00000000: 6f0d 0d0a 0000 0000 554f 0166 cd0e 0000  o.......UO.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d04 5a04 0100 6400 6404 6c05 6d06 5a06  m.Z...d.d.l.m.Z.
 00000060: 0100 6405 6406 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 0100 4700 6407 6408 8400 6408 6506 8303  ..G.d.d...d.e...
@@ -138,15 +138,15 @@
 00000890: 0000 0073 3200 0000 7400 6401 a001 7c00  ...s2...t.d...|.
 000008a0: a101 6701 6402 6403 8d02 7d01 7c01 a002  ..g.d.d...}.|...
 000008b0: a100 7217 7c01 6a03 a004 6404 a101 6405  ..r.|.j...d...d.
 000008c0: 1900 7c01 5f03 7c01 5300 2906 7a27 5265  ..|._.|.S.).z'Re
 000008d0: 7475 726e 2061 2074 7570 6c65 206f 6620  turn a tuple of 
 000008e0: 2872 6574 7572 6e63 6f64 652c 2073 7464  (returncode, std
 000008f0: 6f75 7429 2e7a 0774 7970 6520 7b7d 5429  out).z.type {}T)
-00000900: 0172 3c00 0000 fa01 20e9 ffff ffff 2905  .r<..... .....).
+00000900: 0172 3c00 0000 da01 20e9 ffff ffff 2905  .r<..... .....).
 00000910: 7245 0000 00da 0666 6f72 6d61 7472 2f00  rE.....formatr/.
 00000920: 0000 7230 0000 00da 0573 706c 6974 2902  ..r0.....split).
 00000930: da07 636f 6d6d 616e 6472 4400 0000 7215  ..commandrD...r.
 00000940: 0000 0072 1500 0000 7216 0000 0072 2e00  ...r....r....r..
 00000950: 0000 5300 0000 7308 0000 0014 0308 0212  ..S...s.........
 00000960: 0104 0172 2e00 0000 6301 0000 0000 0000  ...r....c.......
 00000970: 0000 0000 0002 0000 0009 0000 0063 0000  .............c..
@@ -169,15 +169,15 @@
 00000a80: 5200 0000 6301 0000 0000 0000 0000 0000  R...c...........
 00000a90: 0002 0000 0008 0000 0043 0000 0073 4e00  .........C...sN.
 00000aa0: 0000 6401 7c00 7601 7206 6402 5300 7c00  ..d.|.v.r.d.S.|.
 00000ab0: a000 6401 a101 7d01 7a11 7401 a002 7c01  ..d...}.z.t...|.
 00000ac0: 6403 1900 6404 a102 0100 7403 7c01 6405  d...d.....t.|.d.
 00000ad0: 1900 8301 0100 5700 6406 5300 0400 7404  ......W.d.S...t.
 00000ae0: 7926 0100 0100 0100 5900 6402 5300 7700  y&......Y.d.S.w.
-00000af0: 2907 4efa 012d 4672 0100 0000 7a0e 2559  ).N..-Fr....z.%Y
+00000af0: 2907 4eda 012d 4672 0100 0000 7a0e 2559  ).N..-Fr....z.%Y
 00000b00: 256d 2564 2548 254d 2553 2566 7205 0000  %m%d%H%M%S%fr...
 00000b10: 0054 2905 7249 0000 0072 0300 0000 da08  .T).rI...r......
 00000b20: 7374 7270 7469 6d65 da03 696e 74da 0a56  strptime..int..V
 00000b30: 616c 7565 4572 726f 7229 02da 046e 616d  alueError)...nam
 00000b40: 6572 4900 0000 7215 0000 0072 1500 0000  erI...r....r....
 00000b50: 7216 0000 00da 1069 735f 7661 6c69 645f  r......is_valid_
 00000b60: 7065 726d 5f69 6468 0000 0073 1400 0000  perm_idh...s....
```

### Comparing `obis-0.4.5/obis/dm/checksum.py` & `obis-0.4.6rc0/obis/dm/checksum.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/command_log.py` & `obis-0.4.6rc0/obis/dm/command_log.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/command_result.py` & `obis-0.4.6rc0/obis/dm/command_result.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/commands/__pycache__/addref.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/commands/__pycache__/addref.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Mar 29 14:28:17 2023 UTC, .py size: 1897 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 014b 2464 6907 0000  o........K$di...
+00000000: 6f0d 0d0a 0000 0000 554f 0166 6907 0000  o.......UO.fi...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6404 6405 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6404 6406 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6407 6408 8400 6408 6502 8303 5a08 6401  d.d...d.e...Z.d.
 00000070: 5300 2909 e900 0000 004e e901 0000 0029  S.)......N.....)
```

### Comparing `obis-0.4.5/obis/dm/commands/__pycache__/clone.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/commands/__pycache__/clone.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb 28 08:49:14 2023 UTC, .py size: 5292 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 0ac0 fd63 ac14 0000  o..........c....
+00000000: 6f0d 0d0a 0000 0000 554f 0166 ac14 0000  o.......UO.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 6d03 5a03 0100 6404 6405 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6404 6406 6c06 6d07 5a07 6d08 5a08  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6404 6407 6c09 6d0a 5a0a 0100 6404  ..d.d.l.m.Z...d.
 00000070: 6408 6c0b 6d0c 5a0c 0100 6409 640a 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `obis-0.4.5/obis/dm/commands/__pycache__/collection.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/commands/__pycache__/collection.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb 28 09:16:53 2023 UTC, .py size: 3657 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 85c6 fd63 490e 0000  o..........cI...
+00000000: 6f0d 0d0a 0000 0000 554f 0166 490e 0000  o.......UO.fI...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6404 6405 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6406 6407 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6408 6409 8400 6409 6502 8303 5a08 6401  d.d...d.e...Z.d.
 00000070: 5300 290a e900 0000 004e e901 0000 0029  S.)......N.....)
```

### Comparing `obis-0.4.5/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/commands/__pycache__/download_physical.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Mar  3 14:31:58 2023 UTC, .py size: 4124 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 de04 0264 1c10 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 554f 0166 1c10 0000  o.......UO.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6000 0000 6400  .....@...s`...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 0100 6404 6405 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6404 6406 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6404 6407 6c08 6d09 5a09 0100 6408  ..d.d.l.m.Z...d.
 00000070: 6409 6c0a 6d0b 5a0b 0100 4700 640a 640b  d.l.m.Z...G.d.d.
```

### Comparing `obis-0.4.5/obis/dm/commands/__pycache__/move.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/commands/__pycache__/move.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb 21 12:05:41 2023 UTC, .py size: 2967 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 95b3 f463 970b 0000  o..........c....
+00000000: 6f0d 0d0a 0000 0000 554f 0166 970b 0000  o.......UO.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6402 6403 6c03 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6402 6404 6c05 6d06 5a06 6d07 5a07  ..d.d.l.m.Z.m.Z.
 00000060: 0100 6405 6406 6c08 6d09 5a09 0100 6405  ..d.d.l.m.Z...d.
 00000070: 6407 6c0a 6d0b 5a0b 0100 6405 6408 6c0a  d.l.m.Z...d.d.l.
```

### Comparing `obis-0.4.5/obis/dm/commands/__pycache__/object.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/commands/__pycache__/object.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Mar  1 08:22:23 2023 UTC, .py size: 4373 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3f0b ff63 1511 0000  o.......?..c....
+00000000: 6f0d 0d0a 0000 0000 554f 0166 1511 0000  o.......UO.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6404 6405 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 0100 6406 6407 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6408 6409 8400 6409 6502 8303 5a08 6401  d.d...d.e...Z.d.
 00000070: 5300 290a e900 0000 004e e901 0000 0029  S.)......N.....)
```

### Comparing `obis-0.4.5/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Aug 23 18:47:42 2023 UTC, .py size: 12135 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 4e54 e664 672f 0000  o.......NT.dg/..
+00000000: 6f0d 0d0a 0000 0000 554f 0166 672f 0000  o.......UO.fg/..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6402 6403 6c05 6d06 5a07  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6402 6404 6c08 6d09 5a09 0100 6402  ..d.d.l.m.Z...d.
 00000070: 6405 6c08 6d0a 5a0a 0100 6402 6406 6c0b  d.l.m.Z...d.d.l.
```

### Comparing `obis-0.4.5/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb 21 12:05:41 2023 UTC, .py size: 9774 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 95b3 f463 2e26 0000  o..........c.&..
+00000000: 6f0d 0d0a 0000 0000 554f 0166 2e26 0000  o.......UO.f.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a00 6402 6403 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6401 6c03 5a03 6400 6401 6c04  ..d.d.l.Z.d.d.l.
 00000050: 5a04 6402 6404 6c05 6d06 5a06 0100 6405  Z.d.d.l.m.Z...d.
 00000060: 6406 6c07 6d08 5a08 0100 4700 6407 6408  d.l.m.Z...G.d.d.
 00000070: 8400 6408 6508 8303 5a09 6401 5300 2909  ..d.e...Z.d.S.).
```

### Comparing `obis-0.4.5/obis/dm/commands/__pycache__/removeref.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/commands/__pycache__/removeref.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Feb 21 12:05:41 2023 UTC, .py size: 3565 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 95b3 f463 ed0d 0000  o..........c....
+00000000: 6f0d 0d0a 0000 0000 554f 0166 ed0d 0000  o.......UO.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 0100 6404  d.l.m.Z.m.Z...d.
 00000050: 6405 6c05 6d06 5a06 6d07 5a07 0100 6404  d.l.m.Z.m.Z...d.
 00000060: 6406 6c08 6d09 5a09 0100 4700 6407 6408  d.l.m.Z...G.d.d.
 00000070: 8400 6408 6503 8303 5a0a 6401 5300 2909  ..d.e...Z.d.S.).
```

### Comparing `obis-0.4.5/obis/dm/commands/__pycache__/search.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/commands/__pycache__/search.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Aug  2 10:52:21 2023 UTC, .py size: 13214 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6535 ca64 9e33 0000  o.......e5.d.3..
+00000000: 6f0d 0d0a 0000 0000 408e 2f66 9333 0000  o.......@./f.3..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c04 6d05 5a05 0100 6403 6404 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6405 6406 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6405 6407 6c0a 6d0b 5a0b 0100 6408  ..d.d.l.m.Z...d.
 00000070: 6409 6c0c 6d0d 5a0d 0100 640a 640b 8400  d.l.m.Z...d.d...
@@ -144,16 +144,16 @@
 000008f0: 0000 0300 0000 4300 0000 736a 0000 0074  ......C...sj...t
 00000900: 007c 0183 0172 3174 007c 0283 0172 3174  .|...r1t.|...r1t
 00000910: 01a0 027c 01a1 017d 0374 01a0 027c 02a1  ...|...}.t...|..
 00000920: 017d 047c 0064 016b 0272 1a7c 047c 036b  .}.|.d.k.r.|.|.k
 00000930: 0253 007c 0064 026b 0272 227c 047c 036b  .S.|.d.k.r"|.|.k
 00000940: 0453 007c 0064 036b 0272 2a7c 047c 036b  .S.|.d.k.r*|.|.k
 00000950: 0053 0074 0364 047c 009b 009d 0283 0182  .S.t.d.|........
-00000960: 0174 0364 0583 0182 0129 064e fa01 3dfa  .t.d.....).N..=.
-00000970: 013e fa01 3c7a 0d55 6e6b 6e6f 776e 2073  .>..<z.Unknown s
+00000960: 0174 0364 0583 0182 0129 064e da01 3dda  .t.d.....).N..=.
+00000970: 013e da01 3c7a 0d55 6e6b 6e6f 776e 2073  .>..<z.Unknown s
 00000980: 6967 6e20 7a25 4461 7465 7320 6172 6520  ign z%Dates are 
 00000990: 6e6f 7420 696e 2061 2073 7570 706f 7274  not in a support
 000009a0: 6564 2066 6f72 6d61 7473 2129 0472 0200  ed formats!).r..
 000009b0: 0000 da02 7064 da0b 746f 5f64 6174 6574  ....pd..to_datet
 000009c0: 696d 65da 0a56 616c 7565 4572 726f 7229  ime..ValueError)
 000009d0: 05da 0473 6967 6eda 0564 6174 6531 da05  ...sign..date1..
 000009e0: 6461 7465 32da 0a74 696d 6573 7461 6d70  date2..timestamp
@@ -326,235 +326,233 @@
 00001450: 0000 0072 8100 0000 720e 0000 0072 0e00  ...r....r....r..
 00001460: 0000 7213 0000 00da 195f 6765 745f 7361  ..r......_get_sa
 00001470: 6d70 6c65 5f77 6974 685f 6461 7461 7365  mple_with_datase
 00001480: 7473 b700 0000 7306 0000 000c 0104 0106  ts....s.........
 00001490: ff7a 2053 6561 7263 682e 5f67 6574 5f73  .z Search._get_s
 000014a0: 616d 706c 655f 7769 7468 5f64 6174 6173  ample_with_datas
 000014b0: 6574 7346 6302 0000 0000 0000 0000 0000  etsFc...........
-000014c0: 0006 0000 0006 0000 0043 0000 0073 a200  .........C...s..
+000014c0: 0005 0000 0006 0000 0043 0000 0073 9e00  .........C...s..
 000014d0: 0000 7c00 6a00 7205 6401 7d01 6402 7c00  ..|.j.r.d.}.d.|.
 000014e0: 6a01 7600 721b 7c00 6a02 6a03 7c00 6a01  j.v.r.|.j.j.|.j.
 000014f0: 6402 1900 6700 6403 a201 7c01 7c00 6a04  d...g.d...|.|.j.
 00001500: 6404 8d04 7d02 6e16 7c00 a005 7c00 6a04  d...}.n.|...|.j.
 00001510: 6700 6403 a201 a102 7d03 7c01 7c03 6405  g.d.....}.|.|.d.
 00001520: 3c00 7c00 6a02 6a03 640a 6900 7c03 a401  <.|.j.j.d.i.|...
-00001530: 8e01 7d02 7c00 6a00 7245 7406 6406 8301  ..}.|.j.rEt.d...
+00001530: 8e01 7d02 7c00 6a00 7243 7406 6406 8301  ..}.|.j.rCt.d...
 00001540: 0100 7407 7c02 6407 1900 6408 7c00 6a08  ..t.|.d...d.|.j.
-00001550: 8303 7d04 7c04 7d05 7c05 5300 7c01 724d  ..}.|.}.|.S.|.rM
-00001560: 7c02 6407 1900 7d05 7c05 5300 7c02 7d05  |.d...}.|.S.|.}.
-00001570: 7c05 5300 290b 7a1f 4865 6c70 6572 206d  |.S.).z.Helper m
-00001580: 6574 686f 6420 746f 2073 6561 7263 6820  ethod to search 
-00001590: 7361 6d70 6c65 7354 da0b 6f62 6a65 6374  samplesT..object
-000015a0: 5f63 6f64 6572 6900 0000 2904 7282 0000  _coderi...).r...
-000015b0: 0072 6d00 0000 7268 0000 0072 5300 0000  .rm...rh...rS...
-000015c0: 7268 0000 007a 3e52 6563 7572 7369 7665  rh...z>Recursive
-000015d0: 2073 6561 7263 6820 656e 6162 6c65 642e   search enabled.
-000015e0: 2049 7420 6d61 7920 7461 6b65 2074 696d   It may take tim
-000015f0: 6520 746f 2070 726f 6475 6365 2072 6573  e to produce res
-00001600: 756c 7473 2e72 2000 0000 7282 0000 004e  ults.r ...r....N
-00001610: 720e 0000 0029 0972 5e00 0000 7258 0000  r....).r^...rX..
-00001620: 0072 7700 0000 7280 0000 0072 5300 0000  .rw...r....rS...
-00001630: da13 5f67 6574 5f66 696c 7465 7269 6e67  .._get_filtering
-00001640: 5f61 7267 7372 0900 0000 7237 0000 0072  _argsr....r7...r
-00001650: 8600 0000 2906 7263 0000 0072 6800 0000  ....).rc...rh...
-00001660: da07 7265 7375 6c74 73da 0461 7267 73da  ..results..args.
-00001670: 076f 7574 7075 7432 727d 0000 0072 0e00  .output2r}...r..
-00001680: 0000 720e 0000 0072 1300 0000 7276 0000  ..r....r....rv..
-00001690: 00bb 0000 0073 2a00 0000 0603 0401 0a02  .....s*.........
-000016a0: 0e01 0601 0201 0401 08fd 1205 0801 1201  ................
-000016b0: 0602 0801 1201 0402 0406 04fc 0801 0403  ................
-000016c0: 04ff 0401 7a16 5365 6172 6368 2e5f 7365  ....z.Search._se
-000016d0: 6172 6368 5f73 616d 706c 6573 6302 0000  arch_samplesc...
-000016e0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-000016f0: 0043 0000 0073 1200 0000 7c00 6a00 6a01  .C...s....|.j.j.
-00001700: 7c01 6401 6701 6402 8d02 5300 2903 4e72  |.d.g.d...S.).Nr
-00001710: 1600 0000 727f 0000 0029 0272 7700 0000  ....r....).rw...
-00001720: da0c 6765 745f 6461 7461 7365 7473 2902  ..get_datasets).
-00001730: 7263 0000 00da 0670 6572 6d49 6472 0e00  rc.....permIdr..
-00001740: 0000 720e 0000 0072 1300 0000 da16 5f67  ..r....r......_g
-00001750: 6574 5f64 6174 6173 6574 735f 6368 696c  et_datasets_chil
-00001760: 6472 656e d700 0000 7302 0000 0012 017a  dren....s......z
-00001770: 1d53 6561 7263 682e 5f67 6574 5f64 6174  .Search._get_dat
-00001780: 6173 6574 735f 6368 696c 6472 656e 6301  asets_childrenc.
-00001790: 0000 0000 0000 0000 0000 000d 0000 0008  ................
-000017a0: 0000 0043 0000 0073 6002 0000 7c00 6a00  ...C...s`...|.j.
-000017b0: 6400 7501 7211 7c00 a001 a100 6400 7500  d.u.r.|.....d.u.
-000017c0: 7211 7402 6401 6402 6403 8d02 5300 7c00  r.t.d.d.d...S.|.
-000017d0: 6a03 a004 a100 7d01 6404 6405 8400 7c01  j.....}.d.d...|.
-000017e0: a005 a100 4400 8301 7d02 6406 6405 8400  ....D...}.d.d...
-000017f0: 7c01 a005 a100 4400 8301 7d03 7c02 728b  |.....D...}.|.r.
-00001800: 6407 7c02 7600 723d 7c02 6407 1900 6400  d.|.v.r=|.d...d.
-00001810: 7501 723a 7c02 6407 1900 7c02 6408 3c00  u.r:|.d...|.d.<.
-00001820: 7c02 6407 3d00 7c02 7c00 5f03 7c00 6a06  |.d.=.|.|._.|.j.
-00001830: 6409 640a 8d01 7d04 7407 640b 7408 7c04  d.d...}.t.d.t.|.
-00001840: 8301 9b00 9d02 8301 0100 640c 640d 8400  ..........d.d...
-00001850: 7c04 4400 8301 7d05 7409 7c05 8301 7d05  |.D...}.t.|...}.
-00001860: 640e 640d 8400 7c05 4400 8301 7d05 7c00  d.d...|.D...}.|.
-00001870: 6a0a 6a0b 7c05 7c00 6a0c 640f 8d02 7d05  j.j.|.|.j.d...}.
-00001880: 6700 7d06 7c05 4400 5d0c 7d07 740d 7c07  g.}.|.D.].}.t.|.
-00001890: 7c03 8302 727a 7c06 7c07 6701 3700 7d06  |...rz|.|.g.7.}.
-000018a0: 716e 7c00 6a0a 6a0e 7c00 6a0c 6410 640d  qn|.j.j.|.j.d.d.
-000018b0: 8400 7c06 4400 8301 6409 6411 8d03 7d05  ..|.D...d.d...}.
-000018c0: 6e60 7c00 6a0f 72c0 7c00 a006 a100 7d04  n`|.j.r.|.....}.
-000018d0: 6700 7d08 7c04 6a10 4400 5d0e 7d09 7c08  g.}.|.j.D.].}.|.
-000018e0: 7c09 6a11 6412 6413 6702 7c00 6a0c 6414  |.j.d.d.g.|.j.d.
-000018f0: 8d02 3700 7d08 7197 7412 7c08 6415 7c00  ..7.}.q.t.|.d.|.
-00001900: 6a13 7c00 6a0a 6a0b 8304 7d0a 7c00 6a0a  j.|.j.j...}.|.j.
-00001910: 6a0e 7c00 6a0c 6416 640d 8400 7c0a 4400  j.|.j.d.d...|.D.
-00001920: 8301 6409 6411 8d03 7d05 6e2b 6417 7c00  ..d.d...}.n+d.|.
-00001930: 6a03 7600 72d7 7c00 6a0a a014 7c00 6a03  j.v.r.|.j...|.j.
-00001940: 6417 1900 a101 6a11 6412 6413 6702 7c00  d.....j.d.d.g.|.
-00001950: 6a0c 6414 8d02 7d0b 6e12 7c00 a015 7c00  j.d...}.n.|...|.
-00001960: 6a0c 6412 6413 6702 a102 7d0c 7c00 6a0a  j.d.d.g...}.|.j.
-00001970: 6a11 641f 6900 7c0c a401 8e01 7d0b 7c0b  j.d.i.|.....}.|.
-00001980: 7d05 7407 6418 7408 7c05 8301 9b00 9d02  }.t.d.t.|.......
-00001990: 8301 0100 7c00 6a00 6400 7501 9001 7223  ....|.j.d.u...r#
-000019a0: 7407 6419 7c00 6a00 9b00 9d02 8301 0100  t.d.|.j.........
-000019b0: 7416 7c00 6a17 6a18 8301 8f11 0100 7c05  t.|.j.j.......|.
-000019c0: 6a19 6a1a 7c00 6a00 641a 641b 8d02 0100  j.j.|.j.d.d.....
-000019d0: 5700 6400 0400 0400 8303 0100 6e09 3100  W.d.........n.1.
-000019e0: 9001 731d 7701 0100 0100 0100 5900 0100  ..s.w.......Y...
-000019f0: 6e07 7407 641c 7c05 9b00 9d02 8301 0100  n.t.d.|.........
-00001a00: 7402 641d 641e 6403 8d02 5300 2920 4ee9  t.d.d.d...S.) N.
-00001a10: ffff ffff 7a3b 436f 6e66 6967 7572 6174  ....z;Configurat
-00001a20: 696f 6e20 6669 6c65 7365 7276 6963 655f  ion fileservice_
-00001a30: 7572 6c20 6e65 6564 7320 746f 2062 6520  url needs to be 
-00001a40: 7365 7420 666f 7220 646f 776e 6c6f 6164  set for download
-00001a50: 2e72 7400 0000 6301 0000 0000 0000 0000  .rt...c.........
-00001a60: 0000 0003 0000 0005 0000 0053 0000 0073  ...........S...s
-00001a70: 2800 0000 6900 7c00 5d10 5c02 7d01 7d02  (...i.|.].\.}.}.
-00001a80: 7c01 a000 6400 a101 7202 7c01 6401 6402  |...d...r.|.d.d.
-00001a90: 8502 1900 7c02 9302 7102 5300 2903 da07  ....|...q.S.)...
-00001aa0: 6f62 6a65 6374 5fe9 0700 0000 4ea9 01da  object_.....N...
-00001ab0: 0a73 7461 7274 7377 6974 68a9 0372 0f00  .startswith..r..
-00001ac0: 0000 da01 6bda 0176 720e 0000 0072 0e00  ....k..vr....r..
-00001ad0: 0000 7213 0000 00da 0a3c 6469 6374 636f  ..r......<dictco
-00001ae0: 6d70 3ee1 0000 0073 0200 0000 2800 7a2b  mp>....s....(.z+
-00001af0: 5365 6172 6368 2e73 6561 7263 685f 6461  Search.search_da
-00001b00: 7461 5f73 6574 732e 3c6c 6f63 616c 733e  ta_sets.<locals>
-00001b10: 2e3c 6469 6374 636f 6d70 3e63 0100 0000  .<dictcomp>c....
-00001b20: 0000 0000 0000 0000 0300 0000 0500 0000  ................
-00001b30: 5300 0000 7320 0000 0069 007c 005d 0c5c  S...s ...i.|.].\
-00001b40: 027d 017d 027c 01a0 0064 00a1 0173 027c  .}.}.|...d...s.|
-00001b50: 017c 0293 0271 0253 0029 0172 9000 0000  .|...q.S.).r....
-00001b60: 7292 0000 0072 9400 0000 720e 0000 0072  r....r....r....r
-00001b70: 0e00 0000 7213 0000 0072 9700 0000 e200  ....r....r......
-00001b80: 0000 7302 0000 0020 00da 0269 6472 8700  ..s.... ...idr..
-00001b90: 0000 5472 6700 0000 7a0f 5361 6d70 6c65  ..Trg...z.Sample
-00001ba0: 7320 666f 756e 643a 2063 0100 0000 0000  s found: c......
-00001bb0: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
-00001bc0: 0000 7314 0000 0067 007c 005d 067d 017c  ..s....g.|.].}.|
-00001bd0: 0164 0019 0091 0271 0253 0029 0172 6b00  .d.....q.S.).rk.
-00001be0: 0000 720e 0000 0072 2e00 0000 720e 0000  ..r....r....r...
-00001bf0: 0072 0e00 0000 7213 0000 0072 1400 0000  .r....r....r....
-00001c00: ec00 0000 7215 0000 007a 2b53 6561 7263  ....r....z+Searc
-00001c10: 682e 7365 6172 6368 5f64 6174 615f 7365  h.search_data_se
-00001c20: 7473 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ts.<locals>.<lis
-00001c30: 7463 6f6d 703e 6301 0000 0000 0000 0000  tcomp>c.........
-00001c40: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
-00001c50: 1800 0000 6700 7c00 5d08 7d01 7c01 6400  ....g.|.].}.|.d.
-00001c60: 1900 6400 1900 9102 7102 5300 2901 728d  ..d.....q.S.).r.
-00001c70: 0000 0072 0e00 0000 722e 0000 0072 0e00  ...r....r....r..
-00001c80: 0000 720e 0000 0072 1300 0000 7214 0000  ..r....r....r...
-00001c90: 00ee 0000 0072 3100 0000 2902 da07 7065  .....r1...)...pe
-00001ca0: 726d 4964 7372 5300 0000 6301 0000 0000  rmIdsrS...c.....
-00001cb0: 0000 0000 0000 0002 0000 0003 0000 0053  ...............S
-00001cc0: 0000 00f3 1200 0000 6700 7c00 5d05 7d01  ........g.|.].}.
-00001cd0: 7c01 6a00 9102 7102 5300 720e 0000 00a9  |.j...q.S.r.....
-00001ce0: 0172 3600 0000 722e 0000 0072 0e00 0000  .r6...r....r....
-00001cf0: 720e 0000 0072 1300 0000 7214 0000 00f7  r....r....r.....
-00001d00: 0000 0073 0200 0000 1200 2903 7253 0000  ...s......).rS..
-00001d10: 0072 6c00 0000 726e 0000 0072 6a00 0000  .rl...rn...rj...
-00001d20: 7216 0000 0029 0272 6d00 0000 7253 0000  r....).rm...rS..
-00001d30: 0072 8d00 0000 6301 0000 0000 0000 0000  .r....c.........
-00001d40: 0000 0002 0000 0003 0000 0053 0000 0072  ...........S...r
-00001d50: 9a00 0000 720e 0000 0072 9b00 0000 2902  ....r....r....).
-00001d60: 720f 0000 0072 5700 0000 720e 0000 0072  r....rW...r....r
-00001d70: 0e00 0000 7213 0000 0072 1400 0000 0501  ....r....r......
-00001d80: 0000 7306 0000 0006 0002 010a ffda 0a64  ..s............d
-00001d90: 6174 6173 6574 5f69 647a 1144 6174 6120  ataset_idz.Data 
-00001da0: 7365 7473 2066 6f75 6e64 3a20 726f 0000  sets found: ro..
-00001db0: 0046 7270 0000 0072 7200 0000 7201 0000  .Frp...rr...r...
-00001dc0: 0072 7300 0000 720e 0000 0029 1b72 5f00  .rs...r....).r_.
-00001dd0: 0000 da0f 6669 6c65 7365 7276 6963 655f  ....fileservice_
-00001de0: 7572 6c72 0600 0000 7258 0000 00da 0463  urlr....rX.....c
-00001df0: 6f70 79da 0569 7465 6d73 7276 0000 0072  opy..itemsrv...r
-00001e00: 0900 0000 7279 0000 0072 3200 0000 7277  ....ry...r2...rw
-00001e10: 0000 00da 0b67 6574 5f64 6174 6173 6574  .....get_dataset
-00001e20: 7253 0000 0072 5b00 0000 da1a 5f64 6174  rS...r[....._dat
-00001e30: 6173 6574 5f6c 6973 745f 666f 725f 7265  aset_list_for_re
-00001e40: 7370 6f6e 7365 725e 0000 0072 2000 0000  sponser^...r ...
-00001e50: 728c 0000 0072 2d00 0000 728e 0000 0072  r....r-...r....r
-00001e60: 8500 0000 7288 0000 0072 0700 0000 727a  ....r....r....rz
-00001e70: 0000 0072 7b00 0000 721d 0000 0072 7c00  ...r{...r....r|.
-00001e80: 0000 290d 7263 0000 00da 0c6d 6169 6e5f  ..).rc.....main_
-00001e90: 6669 6c74 6572 73da 0e6f 626a 6563 745f  filters..object_
-00001ea0: 6669 6c74 6572 73da 0f64 6174 6173 6574  filters..dataset
-00001eb0: 5f66 696c 7465 7273 727d 0000 00da 0864  _filtersr}.....d
-00001ec0: 6174 6173 6574 73da 1166 696c 7465 7265  atasets..filtere
-00001ed0: 645f 6461 7461 7365 7473 7257 0000 00da  d_datasetsrW....
-00001ee0: 016f 7250 0000 0072 2700 0000 7289 0000  .orP...r'...r...
-00001ef0: 0072 8a00 0000 720e 0000 0072 0e00 0000  .r....r....r....
-00001f00: 7213 0000 00da 1073 6561 7263 685f 6461  r......search_da
-00001f10: 7461 5f73 6574 73da 0000 0073 7e00 0000  ta_sets....s~...
-00001f20: 1601 0401 0201 06ff 0a03 1202 1201 0401  ................
-00001f30: 0801 0c01 0c01 0601 0601 0c01 1201 0e02  ................
-00001f40: 0801 0e01 1201 0402 0801 0a01 0a01 0280  ................
-00001f50: 0a02 0601 0201 04ff 0202 08fd 0605 0801  ................
-00001f60: 0401 0a01 0601 0a01 0aff 0602 0401 0601  ................
-00001f70: 04fe 0a03 0601 0202 04fe 0203 08fc 0a06  ................
-00001f80: 1201 0a01 08ff 1203 1201 0401 1202 0c01  ................
-00001f90: 1001 0e01 1401 1eff 0280 0e03 0c02 7a17  ..............z.
-00001fa0: 5365 6172 6368 2e73 6561 7263 685f 6461  Search.search_da
-00001fb0: 7461 5f73 6574 7363 0300 0000 0000 0000  ta_setsc........
-00001fc0: 0000 0000 0500 0000 0900 0000 4300 0000  ............C...
-00001fd0: 739e 0000 0064 007d 037c 006a 0064 0119  s....d.}.|.j.d..
-00001fe0: 0064 0075 0172 1a7c 006a 0064 0219 0064  .d.u.r.|.j.d...d
-00001ff0: 0075 0172 1a7c 006a 0064 0119 007c 006a  .u.r.|.j.d...|.j
-00002000: 0064 0219 0069 017d 0374 017c 006a 0064  .d...i.}.t.|.j.d
-00002010: 0319 007c 006a 0064 0419 007c 006a 0064  ...|.j.d...|.j.d
-00002020: 0519 007c 006a 0064 0619 007c 037c 027c  ...|.j.d...|.|.|
-00002030: 0164 078d 077d 047c 006a 0064 0819 0064  .d...}.|.j.d...d
-00002040: 0075 0172 3f7c 006a 0064 0819 007c 0464  .u.r?|.j.d...|.d
-00002050: 093c 007c 006a 0064 0a19 0064 0075 0172  .<.|.j.d...d.u.r
-00002060: 4d7c 006a 0064 0a19 007c 0464 0b3c 007c  M|.j.d...|.d.<.|
-00002070: 0453 0029 0c4e 724b 0000 0072 4c00 0000  .S.).NrK...rL...
-00002080: 7247 0000 0072 4900 0000 da0a 636f 6c6c  rG...rI.....coll
-00002090: 6563 7469 6f6e 7248 0000 0029 0772 4700  ectionrH...).rG.
-000020a0: 0000 7249 0000 0072 4a00 0000 7252 0000  ..rI...rJ...rR..
-000020b0: 00da 0577 6865 7265 726d 0000 0072 5300  ...whererm...rS.
-000020c0: 0000 724d 0000 0072 5500 0000 724e 0000  ..rM...rU...rN..
-000020d0: 0072 5600 0000 2902 7258 0000 00da 0464  .rV...).rX.....d
-000020e0: 6963 7429 0572 6300 0000 7253 0000 0072  ict).rc...rS...r
-000020f0: 6d00 0000 72aa 0000 0072 8a00 0000 720e  m...r....r....r.
-00002100: 0000 0072 0e00 0000 7213 0000 0072 8800  ...r....r....r..
-00002110: 0000 1c01 0000 7322 0000 0004 011c 0110  ......s"........
-00002120: 0204 ff0a 0408 0108 0208 0102 0102 0102  ................
-00002130: 0106 f90e 090e 010e 010e 0104 017a 1a53  .............z.S
-00002140: 6561 7263 682e 5f67 6574 5f66 696c 7465  earch._get_filte
-00002150: 7269 6e67 5f61 7267 7329 0146 290d da08  ring_args).F)...
-00002160: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00002170: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00002180: 5f5f da07 5f5f 646f 635f 5f72 6200 0000  __..__doc__rb...
-00002190: 727e 0000 0072 8300 0000 7286 0000 0072  r~...r....r....r
-000021a0: 7600 0000 728e 0000 0072 a800 0000 7288  v...r....r....r.
-000021b0: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-000021c0: 5f5f 720e 0000 0072 0e00 0000 7265 0000  __r....r....re..
-000021d0: 0072 1300 0000 725c 0000 008e 0000 0073  .r....r\.......s
-000021e0: 1400 0000 0800 0401 0c04 080e 0813 0803  ................
-000021f0: 0a04 081c 0803 1042 725c 0000 0029 14da  .......Br\...)..
-00002200: 1263 6f6e 6375 7272 656e 742e 6675 7475  .concurrent.futu
-00002210: 7265 7372 1700 0000 da06 7061 6e64 6173  resr......pandas
-00002220: 723e 0000 00da 1a70 7962 6973 2e70 726f  r>.....pybis.pro
-00002230: 7065 7274 795f 7265 666f 726d 6174 7465  perty_reformatte
-00002240: 7272 0200 0000 da0f 6f70 656e 6269 735f  rr......openbis_
-00002250: 636f 6d6d 616e 6472 0400 0000 da0e 636f  commandr......co
-00002260: 6d6d 616e 645f 7265 7375 6c74 7206 0000  mmand_resultr...
-00002270: 00da 0575 7469 6c73 7207 0000 00da 1273  ...utilsr......s
-00002280: 6372 6970 7473 2e63 6c69 636b 5f75 7469  cripts.click_uti
-00002290: 6c72 0900 0000 722d 0000 0072 3700 0000  lr....r-...r7...
-000022a0: 7232 0000 0072 4600 0000 725b 0000 0072  r2...rF...r[...r
-000022b0: 5c00 0000 720e 0000 0072 0e00 0000 720e  \...r....r....r.
-000022c0: 0000 0072 1300 0000 da08 3c6d 6f64 756c  ...r......<modul
-000022d0: 653e 0100 0000 731a 0000 0008 0f08 020c  e>....s.........
-000022e0: 020c 010c 010c 010c 0108 0308 1f08 1708  ................
-000022f0: 0708 0f14 27                             ....'
+00001550: 8303 7d04 7c04 5300 7c01 724b 7c02 6407  ..}.|.S.|.rK|.d.
+00001560: 1900 7d04 7c04 5300 7c02 7d04 7c04 5300  ..}.|.S.|.}.|.S.
+00001570: 290b 7a1f 4865 6c70 6572 206d 6574 686f  ).z.Helper metho
+00001580: 6420 746f 2073 6561 7263 6820 7361 6d70  d to search samp
+00001590: 6c65 7354 da0b 6f62 6a65 6374 5f63 6f64  lesT..object_cod
+000015a0: 6572 6900 0000 2904 7282 0000 0072 6d00  eri...).r....rm.
+000015b0: 0000 7268 0000 0072 5300 0000 7268 0000  ..rh...rS...rh..
+000015c0: 007a 3e52 6563 7572 7369 7665 2073 6561  .z>Recursive sea
+000015d0: 7263 6820 656e 6162 6c65 642e 2049 7420  rch enabled. It 
+000015e0: 6d61 7920 7461 6b65 2074 696d 6520 746f  may take time to
+000015f0: 2070 726f 6475 6365 2072 6573 756c 7473   produce results
+00001600: 2e72 2000 0000 7282 0000 004e 720e 0000  .r ...r....Nr...
+00001610: 0029 0972 5e00 0000 7258 0000 0072 7700  .).r^...rX...rw.
+00001620: 0000 7280 0000 0072 5300 0000 da13 5f67  ..r....rS....._g
+00001630: 6574 5f66 696c 7465 7269 6e67 5f61 7267  et_filtering_arg
+00001640: 7372 0900 0000 7237 0000 0072 8600 0000  sr....r7...r....
+00001650: 2905 7263 0000 0072 6800 0000 da07 7265  ).rc...rh.....re
+00001660: 7375 6c74 73da 0461 7267 7372 7d00 0000  sults..argsr}...
+00001670: 720e 0000 0072 0e00 0000 7213 0000 0072  r....r....r....r
+00001680: 7600 0000 bb00 0000 7328 0000 0006 0304  v.......s(......
+00001690: 010a 020e 0106 0102 0104 0108 fd12 0508  ................
+000016a0: 0112 0106 0208 0112 0104 0604 fc08 0104  ................
+000016b0: 0304 ff04 017a 1653 6561 7263 682e 5f73  .....z.Search._s
+000016c0: 6561 7263 685f 7361 6d70 6c65 7363 0200  earch_samplesc..
+000016d0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+000016e0: 0000 4300 0000 7312 0000 007c 006a 006a  ..C...s....|.j.j
+000016f0: 017c 0164 0167 0164 028d 0253 0029 034e  .|.d.g.d...S.).N
+00001700: 7216 0000 0072 7f00 0000 2902 7277 0000  r....r....).rw..
+00001710: 00da 0c67 6574 5f64 6174 6173 6574 7329  ...get_datasets)
+00001720: 0272 6300 0000 da06 7065 726d 4964 720e  .rc.....permIdr.
+00001730: 0000 0072 0e00 0000 7213 0000 00da 165f  ...r....r......_
+00001740: 6765 745f 6461 7461 7365 7473 5f63 6869  get_datasets_chi
+00001750: 6c64 7265 6ed5 0000 0073 0200 0000 1201  ldren....s......
+00001760: 7a1d 5365 6172 6368 2e5f 6765 745f 6461  z.Search._get_da
+00001770: 7461 7365 7473 5f63 6869 6c64 7265 6e63  tasets_childrenc
+00001780: 0100 0000 0000 0000 0000 0000 0d00 0000  ................
+00001790: 0800 0000 4300 0000 735c 0200 007c 006a  ....C...s\...|.j
+000017a0: 0064 0075 0172 117c 00a0 01a1 0064 0075  .d.u.r.|.....d.u
+000017b0: 0072 1174 0264 0164 0264 038d 0253 007c  .r.t.d.d.d...S.|
+000017c0: 006a 03a0 04a1 007d 0164 0464 0584 007c  .j.....}.d.d...|
+000017d0: 01a0 05a1 0044 0083 017d 0264 0664 0584  .....D...}.d.d..
+000017e0: 007c 01a0 05a1 0044 0083 017d 037c 0272  .|.....D...}.|.r
+000017f0: 8b64 077c 0276 0072 3d7c 0264 0719 0064  .d.|.v.r=|.d...d
+00001800: 0075 0172 3a7c 0264 0719 007c 0264 083c  .u.r:|.d...|.d.<
+00001810: 007c 0264 073d 007c 027c 005f 037c 006a  .|.d.=.|.|._.|.j
+00001820: 0664 0964 0a8d 017d 0474 0764 0b74 087c  .d.d...}.t.d.t.|
+00001830: 0483 019b 009d 0283 0101 0064 0c64 0d84  ...........d.d..
+00001840: 007c 0444 0083 017d 0574 097c 0583 017d  .|.D...}.t.|...}
+00001850: 0564 0e64 0d84 007c 0544 0083 017d 057c  .d.d...|.D...}.|
+00001860: 006a 0a6a 0b7c 057c 006a 0c64 0f8d 027d  .j.j.|.|.j.d...}
+00001870: 0567 007d 067c 0544 005d 0c7d 0774 0d7c  .g.}.|.D.].}.t.|
+00001880: 077c 0383 0272 7a7c 067c 0767 0137 007d  .|...rz|.|.g.7.}
+00001890: 0671 6e7c 006a 0a6a 0e7c 006a 0c64 1064  .qn|.j.j.|.j.d.d
+000018a0: 0d84 007c 0644 0083 0164 0964 118d 037d  ...|.D...d.d...}
+000018b0: 056e 5e7c 006a 0f72 c07c 00a0 06a1 007d  .n^|.j.r.|.....}
+000018c0: 0467 007d 087c 046a 1044 005d 0e7d 097c  .g.}.|.j.D.].}.|
+000018d0: 087c 096a 1164 1264 1367 027c 006a 0c64  .|.j.d.d.g.|.j.d
+000018e0: 148d 0237 007d 0871 9774 127c 0864 157c  ...7.}.q.t.|.d.|
+000018f0: 006a 137c 006a 0a6a 0b83 047d 0a7c 006a  .j.|.j.j...}.|.j
+00001900: 0a6a 0e7c 006a 0c64 1664 0d84 007c 0a44  .j.|.j.d.d...|.D
+00001910: 0083 0164 0964 118d 037d 056e 2964 177c  ...d.d...}.n)d.|
+00001920: 006a 0376 0072 d57c 006a 0a6a 117c 006a  .j.v.r.|.j.j.|.j
+00001930: 0364 1719 0064 1264 1367 027c 006a 0c64  .d...d.d.g.|.j.d
+00001940: 148d 037d 0b6e 127c 00a0 147c 006a 0c64  ...}.n.|...|.j.d
+00001950: 1264 1367 02a1 027d 0c7c 006a 0a6a 1164  .d.g...}.|.j.j.d
+00001960: 1f69 007c 0ca4 018e 017d 0b7c 0b7d 0574  .i.|.....}.|.}.t
+00001970: 0764 1874 087c 0583 019b 009d 0283 0101  .d.t.|..........
+00001980: 007c 006a 0064 0075 0190 0172 2174 0764  .|.j.d.u...r!t.d
+00001990: 197c 006a 009b 009d 0283 0101 0074 157c  .|.j.........t.|
+000019a0: 006a 166a 1783 018f 1101 007c 056a 186a  .j.j.......|.j.j
+000019b0: 197c 006a 0064 1a64 1b8d 0201 0057 0064  .|.j.d.d.....W.d
+000019c0: 0004 0004 0083 0301 006e 0931 0090 0173  .........n.1...s
+000019d0: 1b77 0101 0001 0001 0059 0001 006e 0774  .w.......Y...n.t
+000019e0: 0764 1c7c 059b 009d 0283 0101 0074 0264  .d.|.........t.d
+000019f0: 1d64 1e64 038d 0253 0029 204e e9ff ffff  .d.d...S.) N....
+00001a00: ff7a 3b43 6f6e 6669 6775 7261 7469 6f6e  .z;Configuration
+00001a10: 2066 696c 6573 6572 7669 6365 5f75 726c   fileservice_url
+00001a20: 206e 6565 6473 2074 6f20 6265 2073 6574   needs to be set
+00001a30: 2066 6f72 2064 6f77 6e6c 6f61 642e 7274   for download.rt
+00001a40: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001a50: 0300 0000 0500 0000 5300 0000 7328 0000  ........S...s(..
+00001a60: 0069 007c 005d 105c 027d 017d 027c 01a0  .i.|.].\.}.}.|..
+00001a70: 0064 00a1 0172 027c 0164 0164 0285 0219  .d...r.|.d.d....
+00001a80: 007c 0293 0271 0253 0029 03da 076f 626a  .|...q.S.)...obj
+00001a90: 6563 745f e907 0000 004e a901 da0a 7374  ect_.....N....st
+00001aa0: 6172 7473 7769 7468 a903 720f 0000 00da  artswith..r.....
+00001ab0: 016b da01 7672 0e00 0000 720e 0000 0072  .k..vr....r....r
+00001ac0: 1300 0000 da0a 3c64 6963 7463 6f6d 703e  ......<dictcomp>
+00001ad0: df00 0000 7302 0000 0028 007a 2b53 6561  ....s....(.z+Sea
+00001ae0: 7263 682e 7365 6172 6368 5f64 6174 615f  rch.search_data_
+00001af0: 7365 7473 2e3c 6c6f 6361 6c73 3e2e 3c64  sets.<locals>.<d
+00001b00: 6963 7463 6f6d 703e 6301 0000 0000 0000  ictcomp>c.......
+00001b10: 0000 0000 0003 0000 0005 0000 0053 0000  .............S..
+00001b20: 0073 2000 0000 6900 7c00 5d0c 5c02 7d01  .s ...i.|.].\.}.
+00001b30: 7d02 7c01 a000 6400 a101 7302 7c01 7c02  }.|...d...s.|.|.
+00001b40: 9302 7102 5300 2901 728f 0000 0072 9100  ..q.S.).r....r..
+00001b50: 0000 7293 0000 0072 0e00 0000 720e 0000  ..r....r....r...
+00001b60: 0072 1300 0000 7296 0000 00e0 0000 0073  .r....r........s
+00001b70: 0200 0000 2000 da02 6964 7287 0000 0054  .... ...idr....T
+00001b80: 7267 0000 007a 0f53 616d 706c 6573 2066  rg...z.Samples f
+00001b90: 6f75 6e64 3a20 6301 0000 0000 0000 0000  ound: c.........
+00001ba0: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+00001bb0: 1400 0000 6700 7c00 5d06 7d01 7c01 6400  ....g.|.].}.|.d.
+00001bc0: 1900 9102 7102 5300 2901 726b 0000 0072  ....q.S.).rk...r
+00001bd0: 0e00 0000 722e 0000 0072 0e00 0000 720e  ....r....r....r.
+00001be0: 0000 0072 1300 0000 7214 0000 00ea 0000  ...r....r.......
+00001bf0: 0072 1500 0000 7a2b 5365 6172 6368 2e73  .r....z+Search.s
+00001c00: 6561 7263 685f 6461 7461 5f73 6574 732e  earch_data_sets.
+00001c10: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00001c20: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
+00001c30: 0200 0000 0400 0000 5300 0000 7318 0000  ........S...s...
+00001c40: 0067 007c 005d 087d 017c 0164 0019 0064  .g.|.].}.|.d...d
+00001c50: 0019 0091 0271 0253 0029 0172 8c00 0000  .....q.S.).r....
+00001c60: 720e 0000 0072 2e00 0000 720e 0000 0072  r....r....r....r
+00001c70: 0e00 0000 7213 0000 0072 1400 0000 ec00  ....r....r......
+00001c80: 0000 7231 0000 0029 02da 0770 6572 6d49  ..r1...)...permI
+00001c90: 6473 7253 0000 0063 0100 0000 0000 0000  dsrS...c........
+00001ca0: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
+00001cb0: f312 0000 0067 007c 005d 057d 017c 016a  .....g.|.].}.|.j
+00001cc0: 0091 0271 0253 0072 0e00 0000 a901 7236  ...q.S.r......r6
+00001cd0: 0000 0072 2e00 0000 720e 0000 0072 0e00  ...r....r....r..
+00001ce0: 0000 7213 0000 0072 1400 0000 f500 0000  ..r....r........
+00001cf0: 7302 0000 0012 0029 0372 5300 0000 726c  s......).rS...rl
+00001d00: 0000 0072 6e00 0000 726a 0000 0072 1600  ...rn...rj...r..
+00001d10: 0000 2902 726d 0000 0072 5300 0000 728c  ..).rm...rS...r.
+00001d20: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00001d30: 0200 0000 0300 0000 5300 0000 7299 0000  ........S...r...
+00001d40: 0072 0e00 0000 729a 0000 0029 0272 0f00  .r....r....).r..
+00001d50: 0000 7257 0000 0072 0e00 0000 720e 0000  ..rW...r....r...
+00001d60: 0072 1300 0000 7214 0000 0003 0100 0073  .r....r........s
+00001d70: 0600 0000 0600 0201 0aff da0a 6461 7461  ............data
+00001d80: 7365 745f 6964 7a11 4461 7461 2073 6574  set_idz.Data set
+00001d90: 7320 666f 756e 643a 2072 6f00 0000 4672  s found: ro...Fr
+00001da0: 7000 0000 7272 0000 0072 0100 0000 7273  p...rr...r....rs
+00001db0: 0000 0072 0e00 0000 291a 725f 0000 00da  ...r....).r_....
+00001dc0: 0f66 696c 6573 6572 7669 6365 5f75 726c  .fileservice_url
+00001dd0: 7206 0000 0072 5800 0000 da04 636f 7079  r....rX.....copy
+00001de0: da05 6974 656d 7372 7600 0000 7209 0000  ..itemsrv...r...
+00001df0: 0072 7900 0000 7232 0000 0072 7700 0000  .ry...r2...rw...
+00001e00: da0b 6765 745f 6461 7461 7365 7472 5300  ..get_datasetrS.
+00001e10: 0000 725b 0000 00da 1a5f 6461 7461 7365  ..r[....._datase
+00001e20: 745f 6c69 7374 5f66 6f72 5f72 6573 706f  t_list_for_respo
+00001e30: 6e73 6572 5e00 0000 7220 0000 0072 8b00  nser^...r ...r..
+00001e40: 0000 722d 0000 0072 8d00 0000 7288 0000  ..r-...r....r...
+00001e50: 0072 0700 0000 727a 0000 0072 7b00 0000  .r....rz...r{...
+00001e60: 721d 0000 0072 7c00 0000 290d 7263 0000  r....r|...).rc..
+00001e70: 00da 0c6d 6169 6e5f 6669 6c74 6572 73da  ...main_filters.
+00001e80: 0e6f 626a 6563 745f 6669 6c74 6572 73da  .object_filters.
+00001e90: 0f64 6174 6173 6574 5f66 696c 7465 7273  .dataset_filters
+00001ea0: 727d 0000 00da 0864 6174 6173 6574 73da  r}.....datasets.
+00001eb0: 1166 696c 7465 7265 645f 6461 7461 7365  .filtered_datase
+00001ec0: 7473 7257 0000 00da 016f 7250 0000 0072  tsrW.....orP...r
+00001ed0: 2700 0000 7289 0000 0072 8a00 0000 720e  '...r....r....r.
+00001ee0: 0000 0072 0e00 0000 7213 0000 00da 1073  ...r....r......s
+00001ef0: 6561 7263 685f 6461 7461 5f73 6574 73d8  earch_data_sets.
+00001f00: 0000 0073 7e00 0000 1601 0401 0201 06ff  ...s~...........
+00001f10: 0a03 1202 1201 0401 0801 0c01 0c01 0601  ................
+00001f20: 0601 0c01 1201 0e02 0801 0e01 1201 0402  ................
+00001f30: 0801 0a01 0a01 0280 0a02 0601 0201 04ff  ................
+00001f40: 0202 08fd 0605 0801 0401 0a01 0601 0a01  ................
+00001f50: 0aff 0602 0401 0601 04fe 0a03 0601 0202  ................
+00001f60: 04fe 0203 08fc 0a06 0e01 0a01 08ff 1203  ................
+00001f70: 1201 0401 1202 0c01 1001 0e01 1401 1eff  ................
+00001f80: 0280 0e03 0c02 7a17 5365 6172 6368 2e73  ......z.Search.s
+00001f90: 6561 7263 685f 6461 7461 5f73 6574 7363  earch_data_setsc
+00001fa0: 0300 0000 0000 0000 0000 0000 0500 0000  ................
+00001fb0: 0900 0000 4300 0000 739e 0000 0064 007d  ....C...s....d.}
+00001fc0: 037c 006a 0064 0119 0064 0075 0172 1a7c  .|.j.d...d.u.r.|
+00001fd0: 006a 0064 0219 0064 0075 0172 1a7c 006a  .j.d...d.u.r.|.j
+00001fe0: 0064 0119 007c 006a 0064 0219 0069 017d  .d...|.j.d...i.}
+00001ff0: 0374 017c 006a 0064 0319 007c 006a 0064  .t.|.j.d...|.j.d
+00002000: 0419 007c 006a 0064 0519 007c 006a 0064  ...|.j.d...|.j.d
+00002010: 0619 007c 037c 027c 0164 078d 077d 047c  ...|.|.|.d...}.|
+00002020: 006a 0064 0819 0064 0075 0172 3f7c 006a  .j.d...d.u.r?|.j
+00002030: 0064 0819 007c 0464 093c 007c 006a 0064  .d...|.d.<.|.j.d
+00002040: 0a19 0064 0075 0172 4d7c 006a 0064 0a19  ...d.u.rM|.j.d..
+00002050: 007c 0464 0b3c 007c 0453 0029 0c4e 724b  .|.d.<.|.S.).NrK
+00002060: 0000 0072 4c00 0000 7247 0000 0072 4900  ...rL...rG...rI.
+00002070: 0000 da0a 636f 6c6c 6563 7469 6f6e 7248  ....collectionrH
+00002080: 0000 0029 0772 4700 0000 7249 0000 0072  ...).rG...rI...r
+00002090: 4a00 0000 7252 0000 00da 0577 6865 7265  J...rR.....where
+000020a0: 726d 0000 0072 5300 0000 724d 0000 0072  rm...rS...rM...r
+000020b0: 5500 0000 724e 0000 0072 5600 0000 2902  U...rN...rV...).
+000020c0: 7258 0000 00da 0464 6963 7429 0572 6300  rX.....dict).rc.
+000020d0: 0000 7253 0000 0072 6d00 0000 72a9 0000  ..rS...rm...r...
+000020e0: 0072 8a00 0000 720e 0000 0072 0e00 0000  .r....r....r....
+000020f0: 7213 0000 0072 8800 0000 1a01 0000 7322  r....r........s"
+00002100: 0000 0004 011c 0110 0204 ff0a 0408 0108  ................
+00002110: 0208 0102 0102 0102 0106 f90e 090e 010e  ................
+00002120: 010e 0104 017a 1a53 6561 7263 682e 5f67  .....z.Search._g
+00002130: 6574 5f66 696c 7465 7269 6e67 5f61 7267  et_filtering_arg
+00002140: 7329 0146 290d da08 5f5f 6e61 6d65 5f5f  s).F)...__name__
+00002150: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00002160: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+00002170: 635f 5f72 6200 0000 727e 0000 0072 8300  c__rb...r~...r..
+00002180: 0000 7286 0000 0072 7600 0000 728d 0000  ..r....rv...r...
+00002190: 0072 a700 0000 7288 0000 00da 0d5f 5f63  .r....r......__c
+000021a0: 6c61 7373 6365 6c6c 5f5f 720e 0000 0072  lasscell__r....r
+000021b0: 0e00 0000 7265 0000 0072 1300 0000 725c  ....re...r....r\
+000021c0: 0000 008e 0000 0073 1400 0000 0800 0401  .......s........
+000021d0: 0c04 080e 0813 0803 0a04 081a 0803 1042  ...............B
+000021e0: 725c 0000 0029 14da 1263 6f6e 6375 7272  r\...)...concurr
+000021f0: 656e 742e 6675 7475 7265 7372 1700 0000  ent.futuresr....
+00002200: da06 7061 6e64 6173 723e 0000 00da 1a70  ..pandasr>.....p
+00002210: 7962 6973 2e70 726f 7065 7274 795f 7265  ybis.property_re
+00002220: 666f 726d 6174 7465 7272 0200 0000 da0f  formatterr......
+00002230: 6f70 656e 6269 735f 636f 6d6d 616e 6472  openbis_commandr
+00002240: 0400 0000 da0e 636f 6d6d 616e 645f 7265  ......command_re
+00002250: 7375 6c74 7206 0000 00da 0575 7469 6c73  sultr......utils
+00002260: 7207 0000 00da 1273 6372 6970 7473 2e63  r......scripts.c
+00002270: 6c69 636b 5f75 7469 6c72 0900 0000 722d  lick_utilr....r-
+00002280: 0000 0072 3700 0000 7232 0000 0072 4600  ...r7...r2...rF.
+00002290: 0000 725b 0000 0072 5c00 0000 720e 0000  ..r[...r\...r...
+000022a0: 0072 0e00 0000 720e 0000 0072 1300 0000  .r....r....r....
+000022b0: da08 3c6d 6f64 756c 653e 0100 0000 731a  ..<module>....s.
+000022c0: 0000 0008 0f08 020c 020c 010c 010c 010c  ................
+000022d0: 0108 0308 1f08 1708 0708 0f14 27         ............'
```

### Comparing `obis-0.4.5/obis/dm/commands/__pycache__/upload.cpython-310.pyc` & `obis-0.4.6rc0/obis/dm/commands/__pycache__/upload.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Aug 25 13:40:17 2023 UTC, .py size: 1807 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,100 +1,112 @@
-00000000: 6f0d 0d0a 0000 0000 41af e864 0f07 0000  o.......A..d....
+00000000: 6f0d 0d0a 0000 0000 c787 2f66 5808 0000  o........./fX...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 0100 6402 6403 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6402 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6405 6406 6c06 6d07 5a07 0100 4700  ..d.d.l.m.Z...G.
 00000060: 6407 6408 8400 6408 6501 8303 5a08 6409  d.d...d.e...Z.d.
 00000070: 5300 290a e901 0000 0029 01da 0e4f 7065  S.)......)...Ope
 00000080: 6e62 6973 436f 6d6d 616e 64e9 0200 0000  nbisCommand.....
 00000090: 2901 da0d 436f 6d6d 616e 6452 6573 756c  )...CommandResul
 000000a0: 7429 01da 0263 64e9 0300 0000 2901 da0a  t)...cd.....)...
 000000b0: 636c 6963 6b5f 6563 686f 6300 0000 0000  click_echoc.....
-000000c0: 0000 0000 0000 0000 0000 0003 0000 0000  ................
-000000d0: 0000 0073 2800 0000 6500 5a01 6400 5a02  ...s(...e.Z.d.Z.
-000000e0: 6401 5a03 8700 6601 6402 6403 8408 5a04  d.Z...f.d.d...Z.
-000000f0: 6404 6405 8400 5a05 8700 0400 5a06 5300  d.d...Z.....Z.S.
-00000100: 2906 da06 5570 6c6f 6164 7a3e 0a20 2020  )...Uploadz>.   
-00000110: 2043 6f6d 6d61 6e64 2074 6f20 7570 6c6f   Command to uplo
-00000120: 6164 2070 6879 7369 6361 6c20 6669 6c65  ad physical file
-00000130: 7320 746f 2066 6f72 6d20 6120 6461 7461  s to form a data
-00000140: 2073 6574 2e0a 2020 2020 6305 0000 0000   set..    c.....
-00000150: 0000 0000 0000 0005 0000 0003 0000 0003  ................
-00000160: 0000 0073 3000 0000 7c03 7c00 5f00 7c04  ...s0...|.|._.|.
-00000170: 7c00 5f01 7c02 7c00 5f02 7c00 a003 7c01  |._.|.|._.|...|.
-00000180: a101 0100 7404 7405 7c00 8302 a006 7c01  ....t.t.|.....|.
-00000190: a101 0100 6401 5300 2902 7ae9 0a20 2020  ....d.S.).z..   
-000001a0: 2020 2020 203a 7061 7261 6d20 646d 3a20       :param dm: 
-000001b0: 6461 7461 206d 616e 6167 656d 656e 740a  data management.
-000001c0: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-000001d0: 616d 706c 655f 6964 3a20 7065 726d 4964  ample_id: permId
-000001e0: 206f 7220 7361 6d70 6c65 2070 6174 6820   or sample path 
-000001f0: 6f66 2074 6865 2070 6172 656e 7420 7361  of the parent sa
-00000200: 6d70 6c65 0a20 2020 2020 2020 203a 7061  mple.        :pa
-00000210: 7261 6d20 6461 7461 5f73 6574 5f74 7970  ram data_set_typ
-00000220: 653a 2074 7970 6520 6f66 206e 6577 6c79  e: type of newly
-00000230: 2063 7265 6174 6564 2064 6174 6120 7365   created data se
-00000240: 742e 0a20 2020 2020 2020 203a 7061 7261  t..        :para
-00000250: 6d20 6669 6c65 733a 206c 6973 7420 6f66  m files: list of
-00000260: 2066 696c 6573 2f64 6972 6563 746f 7269   files/directori
-00000270: 6573 2074 6f20 7570 6c6f 6164 0a20 2020  es to upload.   
-00000280: 2020 2020 204e 2907 da0d 6461 7461 5f73       N)...data_s
-00000290: 6574 5f74 7970 65da 0566 696c 6573 da09  et_type..files..
-000002a0: 7361 6d70 6c65 5f69 64da 126c 6f61 645f  sample_id..load_
-000002b0: 676c 6f62 616c 5f63 6f6e 6669 67da 0573  global_config..s
-000002c0: 7570 6572 7208 0000 00da 085f 5f69 6e69  uperr......__ini
-000002d0: 745f 5f29 05da 0473 656c 66da 0264 6d72  t__)...self..dmr
-000002e0: 0b00 0000 7209 0000 0072 0a00 0000 a901  ....r....r......
-000002f0: da09 5f5f 636c 6173 735f 5fa9 00fa 632f  ..__class__...c/
-00000300: 686f 6d65 2f61 6c61 736b 6f77 736b 692f  home/alaskowski/
-00000310: 7265 706f 2f6f 7065 6e62 6973 5f70 7974  repo/openbis_pyt
-00000320: 686f 6e2f 6170 702d 6f70 656e 6269 732d  hon/app-openbis-
-00000330: 636f 6d6d 616e 642d 6c69 6e65 2f73 7263  command-line/src
-00000340: 2f70 7974 686f 6e2f 6f62 6973 2f64 6d2f  /python/obis/dm/
-00000350: 636f 6d6d 616e 6473 2f75 706c 6f61 642e  commands/upload.
-00000360: 7079 720e 0000 001b 0000 0073 0a00 0000  pyr........s....
-00000370: 0607 0601 0601 0a01 1401 7a0f 5570 6c6f  ..........z.Uplo
-00000380: 6164 2e5f 5f69 6e69 745f 5f63 0100 0000  ad.__init__c....
-00000390: 0000 0000 0000 0000 0300 0000 0800 0000  ................
-000003a0: 4300 0000 737e 0000 0074 007c 006a 016a  C...s~...t.|.j.j
-000003b0: 0283 018f 2f01 0074 0364 0174 047c 006a  ..../..t.d.t.|.j
-000003c0: 0583 019b 0064 027c 006a 069b 009d 0483  .....d.|.j......
-000003d0: 0101 007c 006a 076a 087c 006a 097c 006a  ...|.j.j.|.j.|.j
-000003e0: 067c 006a 0564 038d 037d 017c 01a0 0aa1  .|.j.d...}.|....
-000003f0: 007d 0274 0b64 0464 057c 029b 009d 0264  .}.t.d.d.|.....d
-00000400: 068d 0257 0002 0064 0004 0004 0083 0301  ...W...d........
-00000410: 0053 0031 0073 3877 0101 0001 0001 0059  .S.1.s8w.......Y
-00000420: 0001 0064 0053 0029 074e 7a10 5570 6c6f  ...d.S.).Nz.Uplo
-00000430: 6164 696e 6720 6669 6c65 7320 7a07 2075  ading files z. u
-00000440: 6e64 6572 2029 03da 0474 7970 65da 0673  nder )...type..s
-00000450: 616d 706c 6572 0a00 0000 e900 0000 007a  ampler.........z
-00000460: 1e55 706c 6f61 6420 6669 6e69 7368 6564  .Upload finished
-00000470: 2e20 4e65 7720 6461 7461 7365 743a 2029  . New dataset: )
-00000480: 02da 0a72 6574 7572 6e63 6f64 65da 066f  ...returncode..o
-00000490: 7574 7075 7429 0c72 0500 0000 da09 6461  utput).r......da
-000004a0: 7461 5f6d 676d 74da 0f69 6e76 6f63 6174  ta_mgmt..invocat
-000004b0: 696f 6e5f 7061 7468 7207 0000 00da 046c  ion_pathr......l
-000004c0: 6973 7472 0a00 0000 720b 0000 00da 076f  istr....r......o
-000004d0: 7065 6e62 6973 da0b 6e65 775f 6461 7461  penbis..new_data
-000004e0: 7365 7472 0900 0000 da04 7361 7665 7204  setr......saver.
-000004f0: 0000 0029 0372 0f00 0000 da02 6473 da06  ...).r......ds..
-00000500: 7265 7375 6c74 7213 0000 0072 1300 0000  resultr....r....
-00000510: 7214 0000 00da 0372 756e 2800 0000 7310  r......run(...s.
-00000520: 0000 000e 011c 010e 0104 0106 ff08 0210  ................
-00000530: 0124 fb7a 0a55 706c 6f61 642e 7275 6e29  .$.z.Upload.run)
-00000540: 07da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00000550: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00000560: 616d 655f 5fda 075f 5f64 6f63 5f5f 720e  ame__..__doc__r.
-00000570: 0000 0072 2200 0000 da0d 5f5f 636c 6173  ...r".....__clas
-00000580: 7363 656c 6c5f 5f72 1300 0000 7213 0000  scell__r....r...
-00000590: 0072 1100 0000 7214 0000 0072 0800 0000  .r....r....r....
-000005a0: 1600 0000 7308 0000 0008 0004 010c 0410  ....s...........
-000005b0: 0d72 0800 0000 4e29 09da 0f6f 7065 6e62  .r....N)...openb
-000005c0: 6973 5f63 6f6d 6d61 6e64 7202 0000 00da  is_commandr.....
-000005d0: 0e63 6f6d 6d61 6e64 5f72 6573 756c 7472  .command_resultr
-000005e0: 0400 0000 da05 7574 696c 7372 0500 0000  ......utilsr....
-000005f0: da12 7363 7269 7074 732e 636c 6963 6b5f  ..scripts.click_
-00000600: 7574 696c 7207 0000 0072 0800 0000 7213  utilr....r....r.
-00000610: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-00000620: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000630: 730a 0000 000c 0f0c 010c 010c 0114 03    s..............
+000000c0: 0000 0000 0000 0000 0000 0004 0000 0000  ................
+000000d0: 0000 0073 2a00 0000 6500 5a01 6400 5a02  ...s*...e.Z.d.Z.
+000000e0: 6401 5a03 6407 8700 6601 6403 6404 8409  d.Z.d...f.d.d...
+000000f0: 5a04 6405 6406 8400 5a05 8700 0400 5a06  Z.d.d...Z.....Z.
+00000100: 5300 2908 da06 5570 6c6f 6164 7a3e 0a20  S.)...Uploadz>. 
+00000110: 2020 2043 6f6d 6d61 6e64 2074 6f20 7570     Command to up
+00000120: 6c6f 6164 2070 6879 7369 6361 6c20 6669  load physical fi
+00000130: 6c65 7320 746f 2066 6f72 6d20 6120 6461  les to form a da
+00000140: 7461 2073 6574 2e0a 2020 2020 4e63 0600  ta set..    Nc..
+00000150: 0000 0000 0000 0000 0000 0900 0000 0500  ................
+00000160: 0000 0300 0000 737c 0000 007c 037c 005f  ......s|...|.|._
+00000170: 007c 047c 005f 017c 027c 005f 0269 007c  .|.|._.|.|._.i.|
+00000180: 005f 037c 0564 0175 0172 2f69 007d 067c  ._.|.d.u.r/i.}.|
+00000190: 0544 005d 127d 077c 07a0 0464 0264 03a1  .D.].}.|...d.d..
+000001a0: 027d 087c 0864 0319 007c 067c 0864 0419  .}.|.d...|.|.d..
+000001b0: 00a0 05a1 003c 0071 147c 067c 005f 0374  .....<.q.|.|._.t
+000001c0: 067c 006a 0383 0101 007c 00a0 077c 01a1  .|.j.....|...|..
+000001d0: 0101 0074 0874 097c 0083 02a0 0a7c 01a1  ...t.t.|.....|..
+000001e0: 0101 0064 0153 0029 057a e90a 2020 2020  ...d.S.).z..    
+000001f0: 2020 2020 3a70 6172 616d 2064 6d3a 2064      :param dm: d
+00000200: 6174 6120 6d61 6e61 6765 6d65 6e74 0a20  ata management. 
+00000210: 2020 2020 2020 203a 7061 7261 6d20 7361         :param sa
+00000220: 6d70 6c65 5f69 643a 2070 6572 6d49 6420  mple_id: permId 
+00000230: 6f72 2073 616d 706c 6520 7061 7468 206f  or sample path o
+00000240: 6620 7468 6520 7061 7265 6e74 2073 616d  f the parent sam
+00000250: 706c 650a 2020 2020 2020 2020 3a70 6172  ple.        :par
+00000260: 616d 2064 6174 615f 7365 745f 7479 7065  am data_set_type
+00000270: 3a20 7479 7065 206f 6620 6e65 776c 7920  : type of newly 
+00000280: 6372 6561 7465 6420 6461 7461 2073 6574  created data set
+00000290: 2e0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000002a0: 2066 696c 6573 3a20 6c69 7374 206f 6620   files: list of 
+000002b0: 6669 6c65 732f 6469 7265 6374 6f72 6965  files/directorie
+000002c0: 7320 746f 2075 706c 6f61 640a 2020 2020  s to upload.    
+000002d0: 2020 2020 4eda 013d 7201 0000 00e9 0000      N..=r.......
+000002e0: 0000 290b da0d 6461 7461 5f73 6574 5f74  ..)...data_set_t
+000002f0: 7970 65da 0566 696c 6573 da09 7361 6d70  ype..files..samp
+00000300: 6c65 5f69 64da 0a70 726f 7065 7274 6965  le_id..propertie
+00000310: 73da 0573 706c 6974 da05 6c6f 7765 72da  s..split..lower.
+00000320: 0570 7269 6e74 da12 6c6f 6164 5f67 6c6f  .print..load_glo
+00000330: 6261 6c5f 636f 6e66 6967 da05 7375 7065  bal_config..supe
+00000340: 7272 0800 0000 da08 5f5f 696e 6974 5f5f  rr......__init__
+00000350: 2909 da04 7365 6c66 da02 646d 720d 0000  )...self..dmr...
+00000360: 0072 0b00 0000 720c 0000 0072 0e00 0000  .r....r....r....
+00000370: da05 7072 6f70 73da 0470 726f 7072 0f00  ..props..propr..
+00000380: 0000 a901 da09 5f5f 636c 6173 735f 5fa9  ......__class__.
+00000390: 00fa 632f 686f 6d65 2f61 6c61 736b 6f77  ..c/home/alaskow
+000003a0: 736b 692f 7265 706f 2f6f 7065 6e62 6973  ski/repo/openbis
+000003b0: 5f70 7974 686f 6e2f 6170 702d 6f70 656e  _python/app-open
+000003c0: 6269 732d 636f 6d6d 616e 642d 6c69 6e65  bis-command-line
+000003d0: 2f73 7263 2f70 7974 686f 6e2f 6f62 6973  /src/python/obis
+000003e0: 2f64 6d2f 636f 6d6d 616e 6473 2f75 706c  /dm/commands/upl
+000003f0: 6f61 642e 7079 7214 0000 001b 0000 0073  oad.pyr........s
+00000400: 1a00 0000 0607 0601 0601 0601 0801 0401  ................
+00000410: 0801 0c01 1601 0601 0a01 0a01 1401 7a0f  ..............z.
+00000420: 5570 6c6f 6164 2e5f 5f69 6e69 745f 5f63  Upload.__init__c
+00000430: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00000440: 0800 0000 4300 0000 7382 0000 0074 007c  ....C...s....t.|
+00000450: 006a 016a 0283 018f 3101 0074 0364 0174  .j.j....1..t.d.t
+00000460: 047c 006a 0583 019b 0064 027c 006a 069b  .|.j.....d.|.j..
+00000470: 009d 0483 0101 007c 006a 076a 087c 006a  .......|.j.j.|.j
+00000480: 097c 006a 067c 006a 057c 006a 0a64 038d  .|.j.|.j.|.j.d..
+00000490: 047d 017c 01a0 0ba1 007d 0274 0c64 0464  .}.|.....}.t.d.d
+000004a0: 057c 029b 009d 0264 068d 0257 0002 0064  .|.....d...W...d
+000004b0: 0004 0004 0083 0301 0053 0031 0073 3a77  .........S.1.s:w
+000004c0: 0101 0001 0001 0059 0001 0064 0053 0029  .......Y...d.S.)
+000004d0: 074e 7a10 5570 6c6f 6164 696e 6720 6669  .Nz.Uploading fi
+000004e0: 6c65 7320 7a07 2075 6e64 6572 2029 04da  les z. under )..
+000004f0: 0474 7970 65da 0673 616d 706c 6572 0c00  .type..sampler..
+00000500: 0000 7217 0000 0072 0a00 0000 7a1e 5570  ..r....r....z.Up
+00000510: 6c6f 6164 2066 696e 6973 6865 642e 204e  load finished. N
+00000520: 6577 2064 6174 6173 6574 3a20 2902 da0a  ew dataset: )...
+00000530: 7265 7475 726e 636f 6465 da06 6f75 7470  returncode..outp
+00000540: 7574 290d 7205 0000 00da 0964 6174 615f  ut).r......data_
+00000550: 6d67 6d74 da0f 696e 766f 6361 7469 6f6e  mgmt..invocation
+00000560: 5f70 6174 6872 0700 0000 da04 6c69 7374  _pathr......list
+00000570: 720c 0000 0072 0d00 0000 da07 6f70 656e  r....r......open
+00000580: 6269 73da 0b6e 6577 5f64 6174 6173 6574  bis..new_dataset
+00000590: 720b 0000 0072 0e00 0000 da04 7361 7665  r....r......save
+000005a0: 7204 0000 0029 0372 1500 0000 da02 6473  r....).r......ds
+000005b0: da06 7265 7375 6c74 721b 0000 0072 1b00  ..resultr....r..
+000005c0: 0000 721c 0000 00da 0372 756e 3000 0000  ..r......run0...
+000005d0: 7310 0000 000e 011c 010e 0208 0106 ff08  s...............
+000005e0: 0210 0124 fa7a 0a55 706c 6f61 642e 7275  ...$.z.Upload.ru
+000005f0: 6e29 014e 2907 da08 5f5f 6e61 6d65 5f5f  n).N)...__name__
+00000600: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000610: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+00000620: 635f 5f72 1400 0000 7229 0000 00da 0d5f  c__r....r)....._
+00000630: 5f63 6c61 7373 6365 6c6c 5f5f 721b 0000  _classcell__r...
+00000640: 0072 1b00 0000 7219 0000 0072 1c00 0000  .r....r....r....
+00000650: 7208 0000 0016 0000 0073 0800 0000 0800  r........s......
+00000660: 0401 0e04 1015 7208 0000 004e 2909 da0f  ......r....N)...
+00000670: 6f70 656e 6269 735f 636f 6d6d 616e 6472  openbis_commandr
+00000680: 0200 0000 da0e 636f 6d6d 616e 645f 7265  ......command_re
+00000690: 7375 6c74 7204 0000 00da 0575 7469 6c73  sultr......utils
+000006a0: 7205 0000 00da 1273 6372 6970 7473 2e63  r......scripts.c
+000006b0: 6c69 636b 5f75 7469 6c72 0700 0000 7208  lick_utilr....r.
+000006c0: 0000 0072 1b00 0000 721b 0000 0072 1b00  ...r....r....r..
+000006d0: 0000 721c 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+000006e0: 3e01 0000 0073 0a00 0000 0c0f 0c01 0c01  >....s..........
+000006f0: 0c01 1403                                ....
```

### Comparing `obis-0.4.5/obis/dm/commands/addref.py` & `obis-0.4.6rc0/obis/dm/commands/addref.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/commands/clone.py` & `obis-0.4.6rc0/obis/dm/commands/clone.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/commands/collection.py` & `obis-0.4.6rc0/obis/dm/commands/collection.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/commands/download.py` & `obis-0.4.6rc0/obis/dm/commands/download.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/commands/download_physical.py` & `obis-0.4.6rc0/obis/dm/commands/download_physical.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/commands/move.py` & `obis-0.4.6rc0/obis/dm/commands/move.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/commands/object.py` & `obis-0.4.6rc0/obis/dm/commands/object.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/commands/openbis_command.py` & `obis-0.4.6rc0/obis/dm/commands/openbis_command.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/commands/openbis_command_test.py` & `obis-0.4.6rc0/obis/dm/commands/openbis_command_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/commands/openbis_sync.py` & `obis-0.4.6rc0/obis/dm/commands/openbis_sync.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/commands/removeref.py` & `obis-0.4.6rc0/obis/dm/commands/removeref.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/commands/search.py` & `obis-0.4.6rc0/obis/dm/commands/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,17 +198,15 @@
         else:
             args = self._get_filtering_args(self.props, ["parents", "children", "dataSets"])
             args["raw_response"] = raw_response
             results = self.openbis.get_samples(**args)
 
         if self.recursive:
             click_echo("Recursive search enabled. It may take time to produce results.")
-            output2 = _dfs_samples(results['objects'], 'identifier', self._get_sample_with_datasets)
-
-            search_results = output2
+            search_results = _dfs_samples(results['objects'], 'identifier', self._get_sample_with_datasets)
         else:
             if raw_response:
                 search_results = results['objects']
             else:
                 search_results = results
         return search_results
 
@@ -260,16 +258,16 @@
                 datasets = self.openbis._dataset_list_for_response(props=self.props,
                                                                    response=[dataset.data for
                                                                              dataset
                                                                              in output],
                                                                    parsed=True)
             else:
                 if "dataset_id" in self.filters:
-                    results = self.openbis.get_sample(self.filters['dataset_id']).get_datasets(
-                        attrs=["parents", "children"], props=self.props)
+                    results = self.openbis.get_datasets(self.filters['dataset_id'],
+                                                        attrs=["parents", "children"], props=self.props)
                 else:
                     args = self._get_filtering_args(self.props, ["parents", "children"])
                     results = self.openbis.get_datasets(**args)
                 datasets = results
 
         click_echo(f"Data sets found: {len(datasets)}")
         if self.save_path is not None:
```

### Comparing `obis-0.4.5/obis/dm/commands/upload.py` & `obis-0.4.6rc0/obis/dm/commands/upload.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,27 +20,36 @@
 
 
 class Upload(OpenbisCommand):
     """
     Command to upload physical files to form a data set.
     """
 
-    def __init__(self, dm, sample_id, data_set_type, files):
+    def __init__(self, dm, sample_id, data_set_type, files, properties=None):
         """
         :param dm: data management
         :param sample_id: permId or sample path of the parent sample
         :param data_set_type: type of newly created data set.
         :param files: list of files/directories to upload
         """
         self.data_set_type = data_set_type
         self.files = files
         self.sample_id = sample_id
+        self.properties = {}
+        if properties is not None:
+            props = {}
+            for prop in properties:
+                split = prop.split('=', 1)
+                props[split[0].lower()] = split[1]
+            self.properties = props
+            print(self.properties)
         self.load_global_config(dm)
         super(Upload, self).__init__(dm)
 
     def run(self):
         with cd(self.data_mgmt.invocation_path):
             click_echo(f"Uploading files {list(self.files)} under {self.sample_id}")
+
             ds = self.openbis.new_dataset(type=self.data_set_type, sample=self.sample_id,
-                                          files=self.files)
+                                          files=self.files, props=self.properties)
             result = ds.save()
             return CommandResult(returncode=0, output=f"Upload finished. New dataset: {result}")
```

### Comparing `obis-0.4.5/obis/dm/config.py` & `obis-0.4.6rc0/obis/dm/config.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/config_test.py` & `obis-0.4.6rc0/obis/dm/config_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/data_mgmt.py` & `obis-0.4.6rc0/obis/dm/data_mgmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,19 +217,20 @@
         :param from_file: Path of a file with a list of datasets to download.
         :param file: Path of a file in the data set to download. All files are downloaded if it is None.
         :param skip_integrity_check: Checksums of files are not verified if true.
         """
         return
 
     @abc.abstractmethod
-    def upload(self, sample_id, data_set_type, files):
+    def upload(self, sample_id, data_set_type, files, properties=None):
         """Upload files/directories into a new data set.
         :param sample_id: permId or sample path of the parent sample
         :param data_set_type: type of created data set
         :param files: list of files/directories to upload
+        :param properties: list of properties to set
         """
         return
 
     @abc.abstractmethod
     def search_object(self, filters, recursive, save):
         """Search for objects in openBIS using filtering criteria.
         :param filters: dictionary of filter parameters
@@ -637,16 +638,16 @@
     def removeref(self, data_set_id=None):
         self.error_raise("removeref", "This command is only available for External Manager Data")
 
     def download(self, data_set_id, from_file, file, skip_integrity_check):
         cmd = DownloadPhysical(self, data_set_id, from_file, file, skip_integrity_check)
         return cmd.run()
 
-    def upload(self, sample_id, data_set_type, files):
-        cmd = Upload(self, sample_id, data_set_type, files)
+    def upload(self, sample_id, data_set_type, files, properties=None):
+        cmd = Upload(self, sample_id, data_set_type, files, properties)
         return cmd.run()
 
     def search_object(self, filters, recursive, save):
         cmd = Search(self, filters, recursive, save)
         return cmd.search_samples()
 
     def search_data_set(self, filters, recursive, save):
```

### Comparing `obis-0.4.5/obis/dm/data_mgmt_test.py` & `obis-0.4.6rc0/obis/dm/data_mgmt_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/git.py` & `obis-0.4.6rc0/obis/dm/git.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/repository_utils.py` & `obis-0.4.6rc0/obis/dm/repository_utils.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/utils.py` & `obis-0.4.6rc0/obis/dm/utils.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/dm/utils_test.py` & `obis-0.4.6rc0/obis/dm/utils_test.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/scripts/__init__.py` & `obis-0.4.6rc0/obis/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/scripts/__pycache__/cli.cpython-310.pyc` & `obis-0.4.6rc0/obis/scripts/__pycache__/cli.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jul 24 10:38:39 2023 UTC, .py size: 39340 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 af54 be64 ac99 0000  o........T.d....
+00000000: 6f0d 0d0a 0000 0000 a16d 2f66 5e9a 0000  o........m/f^...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0012 0000 0040 0000 0073 720d 0000 6400  .....@...sr...d.
+00000020: 0012 0000 0040 0000 0073 900d 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6403 6c03 6d03 5a03 0100 6401  Z.d.d.l.m.Z...d.
 00000050: 6402 6c04 5a04 6401 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6401 6405 6c07 6d08 5a08 0100 6401  ..d.d.l.m.Z...d.
 00000070: 6406 6c09 6d0a 5a0a 0100 6407 6408 6c0b  d.l.m.Z...d.d.l.
 00000080: 6d0c 5a0c 0100 6407 6409 6c0d 6d0e 5a0e  m.Z...d.d.l.m.Z.
 00000090: 0100 640a 640b 6c0f 6d10 5a10 0100 640a  ..d.d.l.m.Z...d.
@@ -17,15 +17,15 @@
 00000100: 6417 641f 6419 8d05 6504 6a19 6420 6421  d.d.d...e.j.d d!
 00000110: 8400 8301 8301 8301 8301 8301 8301 5a1a  ..............Z.
 00000120: 6422 6423 8400 5a1b 6424 6425 8400 5a1c  d"d#..Z.d$d%..Z.
 00000130: 4700 6426 6427 8400 6427 6504 6a1d 8303  G.d&d'..d'e.j...
 00000140: 5a1e 4700 6428 6429 8400 6429 651e 8303  Z.G.d(d)..d)e...
 00000150: 5a1f 4700 642a 642b 8400 642b 6504 6a1d  Z.G.d*d+..d+e.j.
 00000160: 8303 5a20 642c 642d 8400 5a21 642e 642f  ..Z d,d-..Z!d.d/
-00000170: 8400 5a22 9001 6440 6430 6431 8401 5a23  ..Z"..d@d0d1..Z#
+00000170: 8400 5a22 9001 6444 6430 6431 8401 5a23  ..Z"..dDd0d1..Z#
 00000180: 6432 6433 8400 5a24 6434 6435 8400 5a25  d2d3..Z$d4d5..Z%
 00000190: 6436 6437 8400 5a26 651a a016 a100 6504  d6d7..Z&e.....e.
 000001a0: 6a18 6438 6439 6416 6417 643a 6419 8d05  j.d8d9d.d.d:d...
 000001b0: 6504 6a19 643b 643c 8400 8301 8301 8301  e.j.d;d<........
 000001c0: 5a27 6527 a028 643d a101 6504 6a19 643e  Z'e'.(d=..e.j.d>
 000001d0: 643f 8400 8301 8301 5a29 651a a016 a100  d?......Z)e.....
 000001e0: 6504 6a18 6438 6439 6416 6417 6440 6419  e.j.d8d9d.d.d@d.
@@ -162,15 +162,15 @@
 00000a10: 8301 8301 8301 5a56 651a 6a16 64fa 64a5  ......ZVe.j.d.d.
 00000a20: 8d01 6504 6a19 64fb 64fc 8400 8301 8301  ..e.j.d.d.......
 00000a30: 5a57 6557 6a28 643d 64fd 64a5 8d02 6504  ZWeWj(d=d.d...e.
 00000a40: 6a2b 64fe 6416 64ff 8d02 6504 6a18 9001  j+d.d.d...e.j...
 00000a50: 6400 9001 6401 9001 6402 8d02 6504 6a18  d...d...d...e.j.
 00000a60: 9001 6403 9001 6404 9001 6402 8d02 6504  ..d...d...d...e.
 00000a70: 6a18 9001 6405 9001 6406 9001 6402 8d02  j...d...d...d...
-00000a80: 6504 6a19 9001 6441 9001 6407 9001 6408  e.j...dA..d...d.
+00000a80: 6504 6a19 9001 6445 9001 6407 9001 6408  e.j...dE..d...d.
 00000a90: 8401 8301 8301 8301 8301 8301 8301 5a58  ..............ZX
 00000aa0: 6504 6a2b 6442 6504 6a45 6417 6416 64d3  e.j+dBe.jEd.d.d.
 00000ab0: 8d02 6416 64d4 8d03 6701 5a59 652a 6a28  ..d.d...g.ZYe*j(
 00000ac0: 9001 6409 9001 640a 64a5 8d02 6504 6a19  ..d...d.d...e.j.
 00000ad0: 6515 6559 8301 9001 640b 9001 640c 8400  e.eY....d...d...
 00000ae0: 8301 8301 8301 5a5a 651a 6a28 9001 640a  ......ZZe.j(..d.
 00000af0: 64a5 8d01 6504 6a19 6515 6559 8301 9001  d...e.j.e.eY....
@@ -189,1746 +189,1755 @@
 00000bc0: 9001 641a 9001 641b 9001 641c 9001 641d  ..d...d...d...d.
 00000bd0: 9001 6402 8d04 6504 6a18 641a 9001 641e  ..d...e.j.d...d.
 00000be0: 6416 6417 9001 641f 6419 8d05 6704 5a5f  d.d...d.d...g.Z_
 00000bf0: 651a 6a28 9001 6420 9001 6421 64a5 8d02  e.j(..d ..d!d...
 00000c00: 6515 655f 8301 6504 6a19 9001 6422 9001  e.e_..e.j...d"..
 00000c10: 6420 8400 8301 8301 8301 5a60 6504 6a18  d ........Z`e.j.
 00000c20: 9001 641a 9001 641b 9001 6423 9001 6424  ..d...d...d#..d$
-00000c30: 6417 6417 9001 6425 8d06 6504 a02b 9001  d.d...d%..e..+..
-00000c40: 6426 a101 6504 a02b 9001 6427 a101 6703  d&..e..+..d'..g.
-00000c50: 5a61 651a 6a28 9001 6428 9001 6429 64a5  Zae.j(..d(..d)d.
-00000c60: 8d02 6515 6561 8301 6504 6a19 9001 642a  ..e.ea..e.j...d*
-00000c70: 9001 6428 8400 8301 8301 8301 5a62 6504  ..d(........Zbe.
-00000c80: 6a18 9001 642b 9001 642c 6402 9001 642d  j...d+..d,d...d-
-00000c90: 6450 8d04 6504 6a18 9001 642e 9001 642f  dP..e.j...d...d/
-00000ca0: 6563 6402 9001 6430 9001 6431 8d05 6504  ecd...d0..d1..e.
-00000cb0: 6a18 641a 9001 641e 6416 6417 9001 6432  j.d...d.d.d...d2
-00000cc0: 6419 8d05 6504 a02b 9001 6415 a101 6704  d...e..+..d...g.
-00000cd0: 5a64 6531 6a28 9001 6433 9001 6434 64a5  Zde1j(..d3..d4d.
-00000ce0: 8d02 6504 6a19 6515 6564 8301 9001 6435  ..e.j.e.ed....d5
-00000cf0: 9001 6436 8400 8301 8301 8301 5a65 651a  ..d6........Zee.
-00000d00: 6a28 9001 6434 64a5 8d01 6504 6a19 6515  j(..d4d...e.j.e.
-00000d10: 6564 8301 9001 6437 9001 6433 8400 8301  ed....d7..d3....
-00000d20: 8301 8301 5a66 6531 6a28 9001 6438 9001  ....Zfe1j(..d8..
-00000d30: 6439 64a5 8d02 6504 6a19 6515 6564 8301  d9d...e.j.e.ed..
-00000d40: 9001 643a 9001 643b 8400 8301 8301 8301  ..d:..d;........
-00000d50: 5a67 651a 6a28 9001 6439 64a5 8d01 6504  Zge.j(..d9d...e.
-00000d60: 6a19 6515 6564 8301 9001 643c 9001 6438  j.e.ed....d<..d8
-00000d70: 8400 8301 8301 8301 5a68 9001 643d 9001  ........Zh..d=..
-00000d80: 643e 8400 5a69 656a 9001 643f 6b02 9006  d>..Ziej..d?k...
-00000d90: 72b7 6569 8300 0100 6402 5300 6402 5300  r.ei....d.S.d.S.
-00000da0: 2842 0100 007a 360a 636c 692e 7079 0a0a  (B...z6.cli.py..
-00000db0: 5468 6520 6d6f 6475 6c65 2074 6861 7420  The module that 
-00000dc0: 696d 706c 656d 656e 7473 2074 6865 2043  implements the C
-00000dd0: 4c49 2066 6f72 206f 6269 732e 0ae9 0000  LI for obis.....
-00000de0: 0000 4e29 01da 0864 6174 6574 696d 6529  ..N)...datetime)
-00000df0: 01da 0d72 656c 6174 6976 6564 656c 7461  ...relativedelta
-00000e00: 2901 da0f 436f 6e6e 6563 7469 6f6e 4572  )...ConnectionEr
-00000e10: 726f 7229 01da 074f 7065 6e62 6973 e901  ror)...Openbis..
-00000e20: 0000 00a9 01da 0a63 6c69 636b 5f65 6368  .......click_ech
-00000e30: 6f29 01da 0e44 6174 614d 676d 7452 756e  o)...DataMgmtRun
-00000e40: 6e65 72e9 0200 0000 2901 da0d 436f 6d6d  ner.....)...Comm
-00000e50: 616e 6452 6573 756c 7429 01da 0d4f 7065  andResult)...Ope
-00000e60: 7261 7469 6f6e 5479 7065 6301 0000 0000  rationTypec.....
-00000e70: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00000e80: 0000 0073 2000 0000 7c00 6401 1900 6402  ...s ...|.d...d.
-00000e90: 6b02 720e 7400 7c00 6403 1900 8301 0100  k.r.t.|.d.......
-00000ea0: 6400 5300 6400 5300 2904 4eda 0474 7970  d.S.d.S.).N..typ
-00000eb0: 65da 0870 726f 6772 6573 73da 076d 6573  e..progress..mes
-00000ec0: 7361 6765 7207 0000 00a9 01da 0d70 726f  sager........pro
-00000ed0: 6772 6573 735f 6461 7461 a900 7212 0000  gress_data..r...
-00000ee0: 00fa 5c2f 686f 6d65 2f61 6c61 736b 6f77  ..\/home/alaskow
-00000ef0: 736b 692f 7265 706f 2f6f 7065 6e62 6973  ski/repo/openbis
-00000f00: 5f70 7974 686f 6e2f 6170 702d 6f70 656e  _python/app-open
-00000f10: 6269 732d 636f 6d6d 616e 642d 6c69 6e65  bis-command-line
-00000f20: 2f73 7263 2f70 7974 686f 6e2f 6f62 6973  /src/python/obis
-00000f30: 2f73 6372 6970 7473 2f63 6c69 2e70 79da  /scripts/cli.py.
-00000f40: 0e63 6c69 636b 5f70 726f 6772 6573 7327  .click_progress'
-00000f50: 0000 0073 0600 0000 0c01 1001 04ff 7214  ...s..........r.
-00000f60: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-00000f70: 0100 0000 0600 0000 4300 0000 7328 0000  ........C...s(..
-00000f80: 007c 0064 0119 0064 026b 0272 1274 00a0  .|.d...d.k.r.t..
-00000f90: 0164 03a0 027c 0064 0419 00a1 01a1 0101  .d...|.d........
-00000fa0: 0064 0053 0064 0053 0029 054e 720d 0000  .d.S.d.S.).Nr...
-00000fb0: 0072 0e00 0000 fa02 7b7d 720f 0000 0029  .r......{}r....)
-00000fc0: 03da 0563 6c69 636b da04 6563 686f da06  ...click..echo..
-00000fd0: 666f 726d 6174 7210 0000 0072 1200 0000  formatr....r....
-00000fe0: 7212 0000 0072 1300 0000 da14 636c 6963  r....r......clic
-00000ff0: 6b5f 7072 6f67 7265 7373 5f6e 6f5f 7473  k_progress_no_ts
-00001000: 2c00 0000 7306 0000 000c 0118 0104 ff72  ,...s..........r
-00001010: 1900 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00001020: 0002 0000 0003 0000 0003 0000 0073 1000  .............s..
-00001030: 0000 8700 6601 6401 6402 8408 7d01 7c01  ....f.d.d...}.|.
-00001040: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
-00001050: 0000 0200 0000 0300 0000 1300 0000 731a  ..............s.
-00001060: 0000 0074 0088 0083 0144 005d 067d 017c  ...t.....D.].}.|
-00001070: 017c 0083 017d 0071 047c 0053 00a9 014e  .|...}.q.|.S...N
-00001080: 2901 da08 7265 7665 7273 6564 2902 da04  )...reversed)...
-00001090: 6675 6e63 da05 7061 7261 6da9 01da 0670  func..param....p
-000010a0: 6172 616d 7372 1200 0000 7213 0000 00da  aramsr....r.....
-000010b0: 0b5f 6164 645f 7061 7261 6d73 3200 0000  ._add_params2...
-000010c0: 7306 0000 000c 010a 0104 017a 1f61 6464  s..........z.add
-000010d0: 5f70 6172 616d 732e 3c6c 6f63 616c 733e  _params.<locals>
-000010e0: 2e5f 6164 645f 7061 7261 6d73 7212 0000  ._add_paramsr...
-000010f0: 0029 0272 1f00 0000 7220 0000 0072 1200  .).r....r ...r..
-00001100: 0000 721e 0000 0072 1300 0000 da0a 6164  ..r....r......ad
-00001110: 645f 7061 7261 6d73 3100 0000 7304 0000  d_params1...s...
-00001120: 000c 0104 0572 2100 0000 2901 da07 7665  .....r!...)...ve
-00001130: 7273 696f 6e7a 022d 717a 072d 2d71 7569  rsionz.-qz.--qui
-00001140: 6574 4654 7a1a 5375 7070 7265 7373 2073  etFTz.Suppress s
-00001150: 7461 7475 7320 7265 706f 7274 696e 672e  tatus reporting.
-00001160: 2903 da07 6465 6661 756c 74da 0769 735f  )...default..is_
-00001170: 666c 6167 da04 6865 6c70 7a02 2d73 7a13  flag..helpz.-sz.
-00001180: 2d2d 736b 6970 5f76 6572 6966 6963 6174  --skip_verificat
-00001190: 696f 6e7a 1944 6f20 6e6f 7420 7665 7269  ionz.Do not veri
-000011a0: 6679 2063 6572 6669 6369 6174 6573 7a02  fy cerficiatesz.
-000011b0: 2d64 7a07 2d2d 6465 6275 677a 1a53 686f  -dz.--debugz.Sho
-000011c0: 7720 7374 6163 6b20 7472 6163 6520 6f6e  w stack trace on
-000011d0: 2065 7272 6f72 2e63 0400 0000 0000 0000   error.c........
-000011e0: 0000 0000 0400 0000 0300 0000 4300 0000  ............C...
-000011f0: 7326 0000 007c 017c 006a 0064 013c 007c  s&...|.|.j.d.<.|
-00001200: 0272 0c64 027c 006a 0064 033c 007c 037c  .r.d.|.j.d.<.|.|
-00001210: 006a 0064 043c 0064 0053 0029 054e da05  .j.d.<.d.S.).N..
-00001220: 7175 6965 7446 da13 7665 7269 6679 5f63  quietF..verify_c
-00001230: 6572 7469 6669 6361 7465 73da 0564 6562  ertificates..deb
-00001240: 7567 a901 da03 6f62 6a29 04da 0363 7478  ug....obj)...ctx
-00001250: 7226 0000 00da 1173 6b69 705f 7665 7269  r&.....skip_veri
-00001260: 6669 6361 7469 6f6e 7228 0000 0072 1200  ficationr(...r..
-00001270: 0000 7212 0000 0072 1300 0000 da03 636c  ..r....r......cl
-00001280: 693a 0000 0073 0800 0000 0a08 0401 0a01  i:...s..........
-00001290: 0e01 722d 0000 0063 0300 0000 0000 0000  ..r-...c........
-000012a0: 0000 0000 0300 0000 0600 0000 0300 0000  ................
-000012b0: 7346 0000 007c 0164 0175 0072 0664 027d  sF...|.d.u.r.d.}
-000012c0: 0174 0064 03a0 017c 01a1 0183 0101 0088  .t.d...|........
-000012d0: 0064 046b 0372 1388 006e 0164 0189 007c  .d.k.r...n.d...|
-000012e0: 006a 0264 0519 00a0 0364 0687 0066 0164  .j.d.....d...f.d
-000012f0: 0764 0884 087c 01a1 0353 0029 097a 3053  .d...|...S.).z0S
-00001300: 6861 7265 6420 696d 706c 656d 656e 7461  hared implementa
-00001310: 7469 6f6e 2066 6f72 2074 6865 2069 6e69  tion for the ini
-00001320: 745f 6461 7461 2063 6f6d 6d61 6e64 2e4e  t_data command.N
-00001330: da01 2e7a 0c69 6e69 745f 6461 7461 207b  ...z.init_data {
-00001340: 7dda 00da 0672 756e 6e65 72da 0969 6e69  }....runner..ini
-00001350: 745f 6461 7461 6301 0000 0000 0000 0000  t_datac.........
-00001360: 0000 0001 0000 0003 0000 0013 0000 0073  ...............s
-00001370: 0a00 0000 7c00 a000 8800 a101 5300 721a  ....|.......S.r.
-00001380: 0000 0029 0172 3100 0000 a901 da02 646d  ...).r1.......dm
-00001390: a901 da04 6465 7363 7212 0000 0072 1300  ....descr....r..
-000013a0: 0000 da08 3c6c 616d 6264 613e 4e00 0000  ....<lambda>N...
-000013b0: f302 0000 000a 007a 2069 6e69 745f 6461  .......z init_da
-000013c0: 7461 5f69 6d70 6c2e 3c6c 6f63 616c 733e  ta_impl.<locals>
-000013d0: 2e3c 6c61 6d62 6461 3e29 0472 0800 0000  .<lambda>).r....
-000013e0: 7218 0000 0072 2a00 0000 da03 7275 6e29  r....r*.....run)
-000013f0: 0372 2b00 0000 da0a 7265 706f 7369 746f  .r+.....reposito
-00001400: 7279 7235 0000 0072 1200 0000 7234 0000  ryr5...r....r4..
-00001410: 0072 1300 0000 da0e 696e 6974 5f64 6174  .r......init_dat
-00001420: 615f 696d 706c 4800 0000 730a 0000 0008  a_implH...s.....
-00001430: 0204 010e 0110 011c 0172 3a00 0000 6304  .........r:...c.
-00001440: 0000 0000 0000 0000 0000 0006 0000 0006  ................
-00001450: 0000 0003 0000 0073 ce00 0000 7400 6401  .......s....t.d.
-00001460: a001 7c02 a101 8301 0100 8801 6400 7501  ..|.........d.u.
-00001470: 7217 7402 6a03 a004 8801 a101 7217 7400  r.t.j.......r.t.
-00001480: 6402 8301 0100 6403 5300 7c02 6400 7501  d.....d.S.|.d.u.
-00001490: 7227 7402 6a03 a004 7c02 a101 7227 7400  r't.j...|...r't.
-000014a0: 6404 8301 0100 6403 5300 8800 6405 6b03  d.....d.S...d.k.
-000014b0: 722d 8800 6e01 6400 8900 8801 6400 7500  r-..n.d.....d.u.
-000014c0: 7237 7402 a005 a100 6e08 7402 6a03 a006  r7t.....n.t.j...
-000014d0: 7402 a005 a100 8801 a102 7d04 7402 6a03  t.........}.t.j.
-000014e0: a006 7402 a005 a100 7c02 a102 7d05 7402  ..t.....|...}.t.
-000014f0: 6a03 a007 7c04 7c05 a102 8901 8801 6400  j...|.|.......d.
-00001500: 7500 7256 6406 6e01 8801 8901 7c00 6a08  u.rVd.n.....|.j.
-00001510: 6407 1900 a009 6408 8700 8701 6602 6409  d.....d.....f.d.
-00001520: 640a 8408 7c02 a103 5300 290b 4e7a 1069  d...|...S.).Nz.i
-00001530: 6e69 745f 616e 616c 7973 6973 207b 7d7a  nit_analysis {}z
-00001540: 3345 7272 6f72 3a20 5468 6520 7061 7265  3Error: The pare
-00001550: 6e74 206d 7573 7420 6265 2067 6976 656e  nt must be given
-00001560: 2061 7320 6120 7265 6c61 7469 7665 2070   as a relative p
-00001570: 6174 682e e9ff ffff ff7a 3745 7272 6f72  ath......z7Error
-00001580: 3a20 5468 6520 7265 706f 7369 746f 7279  : The repository
-00001590: 206d 7573 7420 6265 2067 6976 656e 2061   must be given a
-000015a0: 7320 6120 7265 6c61 7469 7665 2070 6174  s a relative pat
-000015b0: 682e 722f 0000 007a 022e 2e72 3000 0000  h.r/...z...r0...
-000015c0: da0d 696e 6974 5f61 6e61 6c79 7369 7363  ..init_analysisc
-000015d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000015e0: 0400 0000 1300 0000 730c 0000 007c 00a0  ........s....|..
-000015f0: 0088 0188 00a1 0253 0072 1a00 0000 2901  .......S.r....).
-00001600: 723c 0000 0072 3200 0000 a902 da0b 6465  r<...r2.......de
-00001610: 7363 7269 7074 696f 6eda 0670 6172 656e  scription..paren
-00001620: 7472 1200 0000 7213 0000 0072 3600 0000  tr....r....r6...
-00001630: 5e00 0000 f302 0000 000c 007a 2469 6e69  ^..........z$ini
-00001640: 745f 616e 616c 7973 6973 5f69 6d70 6c2e  t_analysis_impl.
-00001650: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-00001660: 3e29 0a72 0800 0000 7218 0000 00da 026f  >).r....r......o
-00001670: 73da 0470 6174 68da 0569 7361 6273 da06  s..path..isabs..
-00001680: 6765 7463 7764 da04 6a6f 696e da07 7265  getcwd..join..re
-00001690: 6c70 6174 6872 2a00 0000 7238 0000 0029  lpathr*...r8...)
-000016a0: 0672 2b00 0000 723f 0000 0072 3900 0000  .r+...r?...r9...
-000016b0: 723e 0000 00da 0a70 6172 656e 745f 6469  r>.....parent_di
-000016c0: 72da 0c61 6e61 6c79 7369 735f 6469 7272  r..analysis_dirr
-000016d0: 1200 0000 723d 0000 0072 1300 0000 da12  ....r=...r......
-000016e0: 696e 6974 5f61 6e61 6c79 7369 735f 696d  init_analysis_im
-000016f0: 706c 5100 0000 731e 0000 000e 0114 0108  plQ...s.........
-00001700: 0104 0114 0108 0104 0110 0122 0112 010e  ..........."....
-00001710: 0110 0118 0102 0104 ff72 4900 0000 6300  .........rI...c.
-00001720: 0000 0000 0000 0000 0000 0000 0000 0002  ................
-00001730: 0000 0040 0000 0073 2000 0000 6500 5a01  ...@...s ...e.Z.
-00001740: 6400 5a02 6401 5a03 6402 6403 8400 5a04  d.Z.d.Z.d.d...Z.
-00001750: 6404 6405 8400 5a05 6406 5300 2907 da0b  d.d...Z.d.S.)...
-00001760: 5365 7474 696e 6773 4765 74da 0c73 6574  SettingsGet..set
-00001770: 7469 6e67 735f 6765 7463 0400 0000 0000  tings_getc......
-00001780: 0000 0000 0000 0500 0000 0600 0000 4300  ..............C.
-00001790: 0000 7336 0000 007a 0f74 0074 0164 0164  ..s6...z.t.t.d.d
-000017a0: 0284 007c 01a0 0264 03a1 0183 0283 017d  ...|...d.......}
-000017b0: 047c 0457 0053 0001 0001 0001 007c 00a0  .|.W.S.......|..
-000017c0: 037c 02a1 0101 0059 0064 0053 0029 044e  .|.....Y.d.S.).N
-000017d0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000017e0: 0002 0000 0053 0000 00f3 0c00 0000 7400  .....S........t.
-000017f0: 7c00 8301 6401 6b04 5300 a902 4e72 0100  |...d.k.S...Nr..
-00001800: 0000 a901 da03 6c65 6ea9 01da 0474 6572  ......len....ter
-00001810: 6d72 1200 0000 7212 0000 0072 1300 0000  mr....r....r....
-00001820: 7236 0000 006a 0000 0072 4000 0000 7a25  r6...j...r@...z%
-00001830: 5365 7474 696e 6773 4765 742e 636f 6e76  SettingsGet.conv
-00001840: 6572 742e 3c6c 6f63 616c 733e 2e3c 6c61  ert.<locals>.<la
-00001850: 6d62 6461 3efa 012c 2904 da04 6c69 7374  mbda>..,)...list
-00001860: da06 6669 6c74 6572 da05 7370 6c69 74da  ..filter..split.
-00001870: 055f 6661 696c 2905 da04 7365 6c66 da05  ._fail)...self..
-00001880: 7661 6c75 6572 1d00 0000 722b 0000 0072  valuer....r+...r
-00001890: 5500 0000 7212 0000 0072 1200 0000 7213  U...r....r....r.
-000018a0: 0000 00da 0763 6f6e 7665 7274 6800 0000  .....converth...
-000018b0: 730a 0000 0002 0118 0106 0106 0110 017a  s..............z
-000018c0: 1353 6574 7469 6e67 7347 6574 2e63 6f6e  .SettingsGet.con
-000018d0: 7665 7274 6302 0000 0000 0000 0000 0000  vertc...........
-000018e0: 0002 0000 0004 0000 0043 0000 00f3 1200  .........C......
-000018f0: 0000 7c00 6a00 7c01 6401 6402 8d02 0100  ..|.j.|.d.d.....
-00001900: 6400 5300 2903 4e7a 2f53 6574 7469 6e67  d.S.).Nz/Setting
-00001910: 7320 6d75 7374 2062 6520 696e 2074 6865  s must be in the
-00001920: 2066 6f72 6d61 743a 206b 6579 312c 206b   format: key1, k
-00001930: 6579 322c 202e 2e2e a902 721d 0000 0072  ey2, .....r....r
-00001940: 0f00 0000 a901 da04 6661 696c a902 7257  ........fail..rW
-00001950: 0000 0072 1d00 0000 7212 0000 0072 1200  ...r....r....r..
-00001960: 0000 7213 0000 0072 5600 0000 6f00 0000  ..r....rV...o...
-00001970: f306 0000 0004 0104 010a ff7a 1153 6574  ...........z.Set
-00001980: 7469 6e67 7347 6574 2e5f 6661 696c 4e29  tingsGet._failN)
-00001990: 06da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-000019a0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-000019b0: 616d 655f 5fda 046e 616d 6572 5900 0000  ame__..namerY...
-000019c0: 7256 0000 0072 1200 0000 7212 0000 0072  rV...r....r....r
-000019d0: 1200 0000 7213 0000 0072 4a00 0000 6500  ....r....rJ...e.
-000019e0: 0000 7308 0000 0008 0004 0108 020c 0772  ..s............r
-000019f0: 4a00 0000 6300 0000 0000 0000 0000 0000  J...c...........
-00001a00: 0000 0000 0001 0000 0040 0000 0073 0c00  .........@...s..
-00001a10: 0000 6500 5a01 6400 5a02 6401 5300 2902  ..e.Z.d.Z.d.S.).
-00001a20: da0d 5365 7474 696e 6773 436c 6561 724e  ..SettingsClearN
-00001a30: 2903 7260 0000 0072 6100 0000 7262 0000  ).r`...ra...rb..
-00001a40: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
-00001a50: 7213 0000 0072 6400 0000 7400 0000 7304  r....rd...t...s.
-00001a60: 0000 0008 0004 0172 6400 0000 6300 0000  .......rd...c...
-00001a70: 0000 0000 0000 0000 0000 0000 0002 0000  ................
-00001a80: 0040 0000 0073 3000 0000 6500 5a01 6400  .@...s0...e.Z.d.
-00001a90: 5a02 6401 5a03 6402 6403 8400 5a04 6404  Z.d.Z.d.d...Z.d.
-00001aa0: 6405 8400 5a05 6406 6407 8400 5a06 6408  d...Z.d.d...Z.d.
-00001ab0: 6409 8400 5a07 640a 5300 290b da0b 5365  d...Z.d.S.)...Se
-00001ac0: 7474 696e 6773 5365 74da 0c73 6574 7469  ttingsSet..setti
-00001ad0: 6e67 735f 7365 7463 0400 0000 0000 0000  ngs_setc........
-00001ae0: 0000 0000 0900 0000 0600 0000 4300 0000  ............C...
-00001af0: 738c 0000 007a 3a7c 00a0 007c 01a1 017d  s....z:|...|...}
-00001b00: 0169 007d 0474 0174 0264 0164 0284 007c  .i.}.t.t.d.d...|
-00001b10: 01a0 0364 03a1 0183 0283 017d 057c 0544  ...d.......}.|.D
-00001b20: 005d 217d 067c 06a0 0364 04a1 017d 0774  .]!}.|...d...}.t
-00001b30: 047c 0783 0164 056b 0372 287c 00a0 057c  .|...d.k.r(|...|
-00001b40: 02a1 0101 007c 0764 0619 007d 087c 0764  .....|.d...}.|.d
-00001b50: 0719 007d 017c 00a0 067c 01a1 017c 047c  ...}.|...|...|.|
-00001b60: 083c 0071 167c 0457 0053 0001 0001 0001  .<.q.|.W.S......
-00001b70: 007c 00a0 057c 02a1 0101 0059 0064 0053  .|...|.....Y.d.S
-00001b80: 0029 084e 6301 0000 0000 0000 0000 0000  .).Nc...........
-00001b90: 0001 0000 0002 0000 0053 0000 0072 4c00  .........S...rL.
-00001ba0: 0000 724d 0000 0072 4e00 0000 7250 0000  ..rM...rN...rP..
-00001bb0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-00001bc0: 7236 0000 007f 0000 0072 4000 0000 7a25  r6.......r@...z%
-00001bd0: 5365 7474 696e 6773 5365 742e 636f 6e76  SettingsSet.conv
-00001be0: 6572 742e 3c6c 6f63 616c 733e 2e3c 6c61  ert.<locals>.<la
-00001bf0: 6d62 6461 3e72 5200 0000 fa01 3d72 0a00  mbda>rR.....=r..
-00001c00: 0000 7201 0000 0072 0600 0000 2907 da0c  ..r....r....)...
-00001c10: 5f65 6e63 6f64 655f 6a73 6f6e 7253 0000  _encode_jsonrS..
-00001c20: 0072 5400 0000 7255 0000 0072 4f00 0000  .rT...rU...rO...
-00001c30: 7256 0000 00da 0c5f 6465 636f 6465 5f6a  rV....._decode_j
-00001c40: 736f 6e29 0972 5700 0000 7258 0000 0072  son).rW...rX...r
-00001c50: 1d00 0000 722b 0000 00da 0873 6574 7469  ....r+.....setti
-00001c60: 6e67 7372 5500 0000 da07 7365 7474 696e  ngsrU.....settin
-00001c70: 67da 0d73 6574 7469 6e67 5f73 706c 6974  g..setting_split
-00001c80: da03 6b65 7972 1200 0000 7212 0000 0072  ..keyr....r....r
-00001c90: 1300 0000 7259 0000 007b 0000 0073 1c00  ....rY...{...s..
-00001ca0: 0000 0201 0a01 0401 1801 0801 0a01 0c01  ................
-00001cb0: 0a01 0801 0801 1001 0601 0601 1001 7a13  ..............z.
-00001cc0: 5365 7474 696e 6773 5365 742e 636f 6e76  SettingsSet.conv
-00001cd0: 6572 7463 0200 0000 0000 0000 0000 0000  ertc............
-00001ce0: 0700 0000 0600 0000 4300 0000 7362 0000  ........C...sb..
-00001cf0: 0064 017d 0264 027d 0364 037d 047c 037d  .d.}.d.}.d.}.|.}
-00001d00: 057c 0144 005d 247d 067c 0664 046b 0272  .|.D.]$}.|.d.k.r
-00001d10: 137c 047d 056e 067c 0664 056b 0272 197c  .|.}.n.|.d.k.r.|
-00001d20: 037d 057c 057c 036b 0272 227c 027c 0637  .}.|.|.k.r"|.|.7
-00001d30: 007d 0271 0a7c 057c 046b 0272 2e7c 027c  .}.q.|.|.k.r.|.|
-00001d40: 06a0 0064 0664 07a1 0237 007d 0271 0a7c  ...d.d...7.}.q.|
-00001d50: 0253 0029 084e 722f 0000 0072 0100 0000  .S.).Nr/...r....
-00001d60: 7206 0000 00da 017b da01 7d72 5200 0000  r......{..}rR...
-00001d70: fa01 7ca9 01da 0772 6570 6c61 6365 2907  ..|....replace).
-00001d80: 7257 0000 0072 5800 0000 da07 656e 636f  rW...rX.....enco
-00001d90: 6465 64da 0453 4545 4bda 0645 4e43 4f44  ded..SEEK..ENCOD
-00001da0: 45da 046d 6f64 65da 0463 6861 7272 1200  E..mode..charr..
-00001db0: 0000 7212 0000 0072 1300 0000 7268 0000  ..r....r....rh..
-00001dc0: 008b 0000 0073 1e00 0000 0401 0401 0401  .....s..........
-00001dd0: 0401 0801 0801 0601 0801 0401 0801 0a01  ................
-00001de0: 0801 1001 0280 0401 7a18 5365 7474 696e  ........z.Settin
-00001df0: 6773 5365 742e 5f65 6e63 6f64 655f 6a73  gsSet._encode_js
-00001e00: 6f6e 6302 0000 0000 0000 0000 0000 0002  onc.............
-00001e10: 0000 0004 0000 0043 0000 0073 0c00 0000  .......C...s....
-00001e20: 7c01 a000 6401 6402 a102 5300 2903 4e72  |...d.d...S.).Nr
-00001e30: 7000 0000 7252 0000 0072 7100 0000 2902  p...rR...rq...).
-00001e40: 7257 0000 0072 5800 0000 7212 0000 0072  rW...rX...r....r
-00001e50: 1200 0000 7213 0000 0072 6900 0000 9b00  ....r....ri.....
-00001e60: 0000 7302 0000 000c 017a 1853 6574 7469  ..s......z.Setti
-00001e70: 6e67 7353 6574 2e5f 6465 636f 6465 5f6a  ngsSet._decode_j
-00001e80: 736f 6e63 0200 0000 0000 0000 0000 0000  sonc............
-00001e90: 0200 0000 0400 0000 4300 0000 725a 0000  ........C...rZ..
-00001ea0: 0029 034e 7a3d 5365 7474 696e 6773 206d  .).Nz=Settings m
-00001eb0: 7573 7420 6265 2069 6e20 7468 6520 666f  ust be in the fo
-00001ec0: 726d 6174 3a20 6b65 7931 3d76 616c 7565  rmat: key1=value
-00001ed0: 312c 206b 6579 323d 7661 6c75 6532 2c20  1, key2=value2, 
-00001ee0: 2e2e 2e72 5b00 0000 725c 0000 0072 5e00  ...r[...r\...r^.
-00001ef0: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00001f00: 0072 5600 0000 9e00 0000 725f 0000 007a  .rV.......r_...z
-00001f10: 1153 6574 7469 6e67 7353 6574 2e5f 6661  .SettingsSet._fa
-00001f20: 696c 4e29 0872 6000 0000 7261 0000 0072  ilN).r`...ra...r
-00001f30: 6200 0000 7263 0000 0072 5900 0000 7268  b...rc...rY...rh
-00001f40: 0000 0072 6900 0000 7256 0000 0072 1200  ...ri...rV...r..
-00001f50: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00001f60: 0072 6500 0000 7800 0000 730c 0000 0008  .re...x...s.....
-00001f70: 0004 0108 0208 1008 100c 0372 6500 0000  ...........re...
-00001f80: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
-00001f90: 0005 0000 0043 0000 0073 2c00 0000 6900  .....C...s,...i.
-00001fa0: 7d01 7c00 4400 5d0f 7d02 7c02 a000 a100  }.|.D.].}.|.....
-00001fb0: 4400 5d08 5c02 7d03 7d04 7c04 7c01 7c03  D.].\.}.}.|.|.|.
-00001fc0: 3c00 710a 7104 7c01 5300 721a 0000 0029  <.q.q.|.S.r....)
-00001fd0: 01da 0569 7465 6d73 2905 da0d 7365 7474  ...items)...sett
-00001fe0: 696e 675f 6469 6374 73da 066a 6f69 6e65  ing_dicts..joine
-00001ff0: 64da 0c73 6574 7469 6e67 5f64 6963 7472  d..setting_dictr
-00002000: 6d00 0000 7258 0000 0072 1200 0000 7212  m...rX...r....r.
-00002010: 0000 0072 1300 0000 da12 5f6a 6f69 6e5f  ...r......_join_
-00002020: 7365 7474 696e 6773 5f73 6574 a300 0000  settings_set....
-00002030: 730c 0000 0004 0108 0110 010a 0102 ff04  s...............
-00002040: 0272 7c00 0000 6301 0000 0000 0000 0000  .r|...c.........
-00002050: 0000 0003 0000 0003 0000 0043 0000 0073  ...........C...s
-00002060: 1a00 0000 6700 7d01 7c00 4400 5d06 7d02  ....g.}.|.D.].}.
-00002070: 7c01 7c02 3700 7d01 7104 7c01 5300 721a  |.|.7.}.q.|.S.r.
-00002080: 0000 0072 1200 0000 2903 da0d 7365 7474  ...r....)...sett
-00002090: 696e 675f 6c69 7374 7372 7a00 0000 da0c  ing_listsrz.....
-000020a0: 7365 7474 696e 675f 6c69 7374 7212 0000  setting_listr...
-000020b0: 0072 1200 0000 7213 0000 00da 125f 6a6f  .r....r......_jo
-000020c0: 696e 5f73 6574 7469 6e67 735f 6765 74ab  in_settings_get.
-000020d0: 0000 0073 0800 0000 0401 0801 0a01 0401  ...s............
-000020e0: 727f 0000 0063 0400 0000 0000 0000 0000  r....c..........
-000020f0: 0000 0800 0000 0800 0000 4300 0000 7350  ..........C...sP
-00002100: 0000 007c 006a 0064 0119 007d 047c 006a  ...|.j.d...}.|.j
-00002110: 0064 0219 007d 057c 006a 0064 0319 007d  .d...}.|.j.d...}
-00002120: 0664 047d 0764 057c 006a 0076 0072 1b7c  .d.}.d.|.j.v.r.|
-00002130: 006a 0064 0519 007d 077c 056a 017c 067c  .j.d...}.|.j.|.|
-00002140: 047c 077c 017c 027c 0364 068d 0601 0064  .|.|.|.|.d.....d
-00002150: 0053 0029 074e da09 6973 5f67 6c6f 6261  .S.).N..is_globa
-00002160: 6c72 3000 0000 da08 7265 736f 6c76 6572  lr0.....resolver
-00002170: 46da 1469 735f 6461 7461 5f73 6574 5f70  F..is_data_set_p
-00002180: 726f 7065 7274 79a9 02da 0470 726f 7072  roperty....propr
-00002190: 5800 0000 2902 722a 0000 00da 0663 6f6e  X...).r*.....con
-000021a0: 6669 6729 0872 2b00 0000 da0e 6f70 6572  fig).r+.....oper
-000021b0: 6174 696f 6e5f 7479 7065 7284 0000 0072  ation_typer....r
-000021c0: 5800 0000 7280 0000 0072 3000 0000 7281  X...r....r0...r.
-000021d0: 0000 0072 8200 0000 7212 0000 0072 1200  ...r....r....r..
-000021e0: 0000 7213 0000 00da 105f 6163 6365 7373  ..r......_access
-000021f0: 5f73 6574 7469 6e67 73b2 0000 0073 1200  _settings....s..
-00002200: 0000 0a01 0a01 0a01 0401 0a01 0a01 0c01  ................
-00002210: 0401 0aff 7287 0000 0063 0200 0000 0000  ....r....c......
-00002220: 0000 0000 0000 0500 0000 0700 0000 4300  ..............C.
-00002230: 0000 7338 0000 0074 007c 0183 017d 027c  ..s8...t.|...}.|
-00002240: 02a0 01a1 0044 005d 0d5c 027d 037d 0474  .....D.].\.}.}.t
-00002250: 027c 0074 036a 047c 037c 0464 018d 0401  .|.t.j.|.|.d....
-00002260: 0071 0874 0564 0264 0364 048d 0253 0029  .q.t.d.d.d...S.)
-00002270: 054e 7283 0000 0072 0100 0000 722f 0000  .Nr....r....r/..
-00002280: 00a9 02da 0a72 6574 7572 6e63 6f64 65da  .....returncode.
-00002290: 066f 7574 7075 7429 0672 7c00 0000 7278  .output).r|...rx
-000022a0: 0000 0072 8700 0000 720c 0000 00da 0353  ...r....r......S
-000022b0: 4554 720b 0000 0029 0572 2b00 0000 726a  ETr....).r+...rj
-000022c0: 0000 00da 0d73 6574 7469 6e67 735f 6469  .....settings_di
-000022d0: 6374 7284 0000 0072 5800 0000 7212 0000  ctr....rX...r...
-000022e0: 0072 1200 0000 7213 0000 00da 045f 7365  .r....r......_se
-000022f0: 74bd 0000 0073 0800 0000 0801 1001 1401  t....s..........
-00002300: 0c01 728d 0000 0063 0200 0000 0000 0000  ..r....c........
-00002310: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
-00002320: f340 0000 0074 007c 0183 017d 0274 017c  .@...t.|...}.t.|
-00002330: 0283 0164 016b 0272 0d64 0067 017d 027c  ...d.k.r.d.g.}.|
-00002340: 0244 005d 0a7d 0374 027c 0074 036a 047c  .D.].}.t.|.t.j.|
-00002350: 0364 028d 0301 0071 0f74 0564 0164 0364  .d.....q.t.d.d.d
-00002360: 048d 0253 00a9 054e 7201 0000 0029 0172  ...S...Nr....).r
-00002370: 8400 0000 722f 0000 0072 8800 0000 2906  ....r/...r....).
-00002380: 727f 0000 0072 4f00 0000 7287 0000 0072  r....rO...r....r
-00002390: 0c00 0000 da03 4745 5472 0b00 0000 a904  ......GETr......
-000023a0: 722b 0000 0072 6a00 0000 da0d 7365 7474  r+...rj.....sett
-000023b0: 696e 6773 5f6c 6973 7472 8400 0000 7212  ings_listr....r.
-000023c0: 0000 0072 1200 0000 7213 0000 00da 045f  ...r....r......_
-000023d0: 6765 74c4 0000 00f3 0c00 0000 0801 0c01  get.............
-000023e0: 0601 0801 1201 0c01 7293 0000 0063 0200  ........r....c..
-000023f0: 0000 0000 0000 0000 0000 0400 0000 0600  ................
-00002400: 0000 4300 0000 728e 0000 0072 8f00 0000  ..C...r....r....
-00002410: 2906 727f 0000 0072 4f00 0000 7287 0000  ).r....rO...r...
-00002420: 0072 0c00 0000 da05 434c 4541 5272 0b00  .r......CLEARr..
-00002430: 0000 7291 0000 0072 1200 0000 7212 0000  ..r....r....r...
-00002440: 0072 1300 0000 da06 5f63 6c65 6172 cd00  .r......_clear..
-00002450: 0000 7294 0000 0072 9600 0000 7a02 2d67  ..r....r....z.-g
-00002460: 7a0b 2d2d 6973 5f67 6c6f 6261 6c7a 1447  z.--is_globalz.G
-00002470: 6574 2067 6c6f 6261 6c20 6f72 206c 6f63  et global or loc
-00002480: 616c 2e63 0200 0000 0000 0000 0000 0000  al.c............
-00002490: 0200 0000 0300 0000 4300 0000 730e 0000  ........C...s...
-000024a0: 007c 017c 006a 0064 013c 0064 0253 0029  .|.|.j.d.<.d.S.)
-000024b0: 037a 2820 4578 7465 726e 616c 2044 6174  .z( External Dat
-000024c0: 6120 5374 6f72 653a 2047 6574 2061 6c6c  a Store: Get all
-000024d0: 2073 6574 7469 6e67 732e 2072 8000 0000   settings. r....
-000024e0: 4e72 2900 0000 2902 722b 0000 0072 8000  Nr)...).r+...r..
-000024f0: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00002500: 0072 6a00 0000 d800 0000 f302 0000 000e  .rj.............
-00002510: 0572 6a00 0000 da03 6765 7463 0100 0000  .rj.....getc....
-00002520: 0000 0000 0000 0000 0400 0000 0500 0000  ................
-00002530: 4300 0000 733a 0000 0074 007c 006a 0164  C...s:...t.|.j.d
-00002540: 0164 028d 027d 017c 01a0 02a1 007d 0274  .d...}.|.....}.t
-00002550: 036a 047c 0264 0364 0464 058d 037d 0374  .j.|.d.d.d...}.t
-00002560: 05a0 0664 06a0 077c 03a1 01a1 0101 0064  ...d...|.......d
-00002570: 0753 0029 087a 2320 4578 7465 726e 616c  .S.).z# External
-00002580: 2044 6174 6120 5374 6f72 653a 2047 6574   Data Store: Get
-00002590: 2073 6574 7469 6e67 2e20 46a9 01da 1168   setting. F....h
-000025a0: 616c 745f 6f6e 5f65 7272 6f72 5f6c 6f67  alt_on_error_log
-000025b0: e904 0000 0054 2902 da06 696e 6465 6e74  .....T)...indent
-000025c0: da09 736f 7274 5f6b 6579 7372 1500 0000  ..sort_keysr....
-000025d0: 4e29 0872 0900 0000 722a 0000 00da 0c67  N).r....r*.....g
-000025e0: 6574 5f73 6574 7469 6e67 73da 046a 736f  et_settings..jso
-000025f0: 6eda 0564 756d 7073 7216 0000 0072 1700  n..dumpsr....r..
-00002600: 0000 7218 0000 0029 0472 2b00 0000 7230  ..r....).r+...r0
-00002610: 0000 0072 6a00 0000 da0c 7365 7474 696e  ...rj.....settin
-00002620: 6773 5f73 7472 7212 0000 0072 1200 0000  gs_strr....r....
-00002630: 7213 0000 0072 4b00 0000 e000 0000 7308  r....rK.......s.
-00002640: 0000 000e 0408 0110 0114 0172 4b00 0000  ...........rK...
-00002650: 7a18 5365 742f 6765 7420 676c 6f62 616c  z.Set/get global
-00002660: 206f 7220 6c6f 6361 6c2e 6302 0000 0000   or local.c.....
-00002670: 0000 0000 0000 0003 0000 0004 0000 0043  ...............C
-00002680: 0000 00f3 3000 0000 7400 7c00 6a01 6401  ....0...t.|.j.d.
-00002690: 6402 8d02 7d02 7c01 7c00 6a01 6403 3c00  d...}.|.|.j.d.<.
-000026a0: 7c02 7c00 6a01 6404 3c00 6405 7c00 6a01  |.|.j.d.<.d.|.j.
-000026b0: 6406 3c00 6407 5300 2908 7a42 2045 7874  d.<.d.S.).zB Ext
-000026c0: 6572 6e61 6c20 4461 7461 2053 746f 7265  ernal Data Store
-000026d0: 3a20 4765 742f 7365 7420 7365 7474 696e  : Get/set settin
-000026e0: 6773 2072 656c 6174 6564 2074 6f20 7468  gs related to th
-000026f0: 6520 7265 706f 7369 746f 7279 2e20 4672  e repository. Fr
-00002700: 9900 0000 7280 0000 0072 3000 0000 7239  ....r....r0...r9
-00002710: 0000 0072 8100 0000 4ea9 0272 0900 0000  ...r....N..r....
-00002720: 722a 0000 00a9 0372 2b00 0000 7280 0000  r*.....r+...r...
-00002730: 0072 3000 0000 7212 0000 0072 1200 0000  .r0...r....r....
-00002740: 7213 0000 0072 3900 0000 ec00 0000 7308  r....r9.......s.
-00002750: 0000 000e 050a 010a 010e 0172 3900 0000  ...........r9...
-00002760: da03 7365 7472 3b00 0000 2902 720d 0000  ..setr;...).r...
-00002770: 00da 056e 6172 6773 6302 0000 0000 0000  ...nargsc.......
-00002780: 0000 0000 0002 0000 0006 0000 0003 0000  ................
-00002790: 00f3 1c00 0000 8800 6a00 6401 1900 a001  ........j.d.....
-000027a0: 6402 8700 8701 6602 6403 6404 8408 a102  d.....f.d.d.....
-000027b0: 5300 2905 7a3e 2045 7874 6572 6e61 6c20  S.).z> External 
-000027c0: 4461 7461 2053 746f 7265 3a20 5365 7420  Data Store: Set 
-000027d0: 7365 7474 696e 6773 2072 656c 6174 6564  settings related
-000027e0: 2074 6f20 7468 6520 7265 706f 7369 746f   to the reposito
-000027f0: 7279 2e20 7230 0000 00da 0e72 6570 6f73  ry. r0.....repos
-00002800: 6974 6f72 795f 7365 7463 0100 0000 0000  itory_setc......
-00002810: 0000 0000 0000 0100 0000 0300 0000 1300  ................
-00002820: 0000 f30a 0000 0074 0088 0088 0183 0253  .......t.......S
-00002830: 0072 1a00 0000 a901 728d 0000 0072 3200  .r......r....r2.
-00002840: 0000 a902 722b 0000 0072 6a00 0000 7212  ....r+...rj...r.
-00002850: 0000 0072 1300 0000 7236 0000 00fc 0000  ...r....r6......
-00002860: 0072 3700 0000 7a20 7265 706f 7369 746f  .r7...z reposito
-00002870: 7279 5f73 6574 2e3c 6c6f 6361 6c73 3e2e  ry_set.<locals>.
-00002880: 3c6c 616d 6264 613e a902 722a 0000 0072  <lambda>..r*...r
-00002890: 3800 0000 72ab 0000 0072 1200 0000 72ab  8...r....r....r.
-000028a0: 0000 0072 1300 0000 72a8 0000 00f7 0000  ...r....r.......
-000028b0: 00f3 0200 0000 1c05 72a8 0000 0063 0200  ........r....c..
-000028c0: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-000028d0: 0000 0300 0000 72a7 0000 0029 057a 3e20  ......r....).z> 
-000028e0: 4578 7465 726e 616c 2044 6174 6120 5374  External Data St
-000028f0: 6f72 653a 2047 6574 2073 6574 7469 6e67  ore: Get setting
-00002900: 7320 7265 6c61 7465 6420 746f 2074 6865  s related to the
-00002910: 2072 6570 6f73 6974 6f72 792e 2072 3000   repository. r0.
-00002920: 0000 da0e 7265 706f 7369 746f 7279 5f67  ....repository_g
-00002930: 6574 6301 0000 0000 0000 0000 0000 0001  etc.............
-00002940: 0000 0003 0000 0013 0000 0072 a900 0000  ...........r....
-00002950: 721a 0000 00a9 0172 9300 0000 7232 0000  r......r....r2..
-00002960: 0072 ab00 0000 7212 0000 0072 1300 0000  .r....r....r....
-00002970: 7236 0000 0004 0100 0072 3700 0000 7a20  r6.......r7...z 
-00002980: 7265 706f 7369 746f 7279 5f67 6574 2e3c  repository_get.<
-00002990: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
-000029a0: 72ac 0000 0072 ab00 0000 7212 0000 0072  r....r....r....r
-000029b0: ab00 0000 7213 0000 0072 ae00 0000 ff00  ....r....r......
-000029c0: 0000 72ad 0000 0072 ae00 0000 da05 636c  ..r....r......cl
-000029d0: 6561 7263 0200 0000 0000 0000 0000 0000  earc............
-000029e0: 0200 0000 0600 0000 0300 0000 72a7 0000  ............r...
-000029f0: 0029 057a 4020 4578 7465 726e 616c 2044  .).z@ External D
-00002a00: 6174 6120 5374 6f72 653a 2043 6c65 6172  ata Store: Clear
-00002a10: 2073 6574 7469 6e67 7320 7265 6c61 7465   settings relate
-00002a20: 6420 746f 2074 6865 2072 6570 6f73 6974  d to the reposit
-00002a30: 6f72 792e 2072 3000 0000 da10 7265 706f  ory. r0.....repo
-00002a40: 7369 746f 7279 5f63 6c65 6172 6301 0000  sitory_clearc...
-00002a50: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00002a60: 0013 0000 0072 a900 0000 721a 0000 00a9  .....r....r.....
-00002a70: 0172 9600 0000 7232 0000 0072 ab00 0000  .r....r2...r....
-00002a80: 7212 0000 0072 1300 0000 7236 0000 000c  r....r....r6....
-00002a90: 0100 0072 3700 0000 7a22 7265 706f 7369  ...r7...z"reposi
-00002aa0: 746f 7279 5f63 6c65 6172 2e3c 6c6f 6361  tory_clear.<loca
-00002ab0: 6c73 3e2e 3c6c 616d 6264 613e 72ac 0000  ls>.<lambda>r...
-00002ac0: 0072 ab00 0000 7212 0000 0072 ab00 0000  .r....r....r....
-00002ad0: 7213 0000 0072 b100 0000 0701 0000 72ad  r....r........r.
-00002ae0: 0000 0072 b100 0000 7a06 2d73 7061 6365  ...r....z.-space
-00002af0: 7a07 2d2d 7370 6163 657a 0a53 7061 6365  z.--spacez.Space
-00002b00: 2063 6f64 6529 0272 2300 0000 7225 0000   code).r#...r%..
-00002b10: 007a 082d 7072 6f6a 6563 747a 092d 2d70  .z.-projectz.--p
-00002b20: 726f 6a65 6374 7a1b 5072 6f6a 6563 7420  rojectz.Project 
-00002b30: 6964 656e 7469 6669 6361 7469 6f6e 2063  identification c
-00002b40: 6f64 657a 0b2d 636f 6c6c 6563 7469 6f6e  odez.-collection
-00002b50: 7a0c 2d2d 636f 6c6c 6563 7469 6f6e 7a0f  z.--collectionz.
-00002b60: 436f 6c6c 6563 7469 6f6e 2063 6f64 657a  Collection codez
-00002b70: 032d 6964 7a04 2d2d 6964 da0a 6461 7461  .-idz.--id..data
-00002b80: 7365 745f 6964 7a42 4461 7461 7365 7420  set_idzBDataset 
-00002b90: 6964 656e 7469 6669 6361 7469 6f6e 2069  identification i
-00002ba0: 6e66 6f72 6d61 7469 6f6e 2c20 6974 2063  nformation, it c
-00002bb0: 616e 2062 6520 7065 726d 4964 206f 7220  an be permId or 
-00002bc0: 6964 656e 7469 6669 6572 7a05 2d74 7970  identifierz.-typ
-00002bd0: 657a 062d 2d74 7970 65da 0974 7970 655f  ez.--type..type_
-00002be0: 636f 6465 7a11 4461 7461 7365 7420 7479  codez.Dataset ty
-00002bf0: 7065 2063 6f64 657a 092d 7072 6f70 6572  pe codez.-proper
-00002c00: 7479 da0d 7072 6f70 6572 7479 5f63 6f64  ty..property_cod
-00002c10: 657a 0d50 726f 7065 7274 7920 636f 6465  ez.Property code
-00002c20: 7a0f 2d70 726f 7065 7274 792d 7661 6c75  z.-property-valu
-00002c30: 65da 0e70 726f 7065 7274 795f 7661 6c75  e..property_valu
-00002c40: 657a 0e50 726f 7065 7274 7920 7661 6c75  ez.Property valu
-00002c50: 657a 122d 7265 6769 7374 7261 7469 6f6e  ez.-registration
-00002c60: 2d64 6174 657a 132d 2d72 6567 6973 7472  -datez.--registr
-00002c70: 6174 696f 6e2d 6461 7465 da11 7265 6769  ation-date..regi
-00002c80: 7374 7261 7469 6f6e 5f64 6174 657a 4d52  stration_datezMR
-00002c90: 6567 6973 7472 6174 696f 6e20 6461 7465  egistration date
-00002ca0: 2c20 6974 2063 616e 2062 6520 696e 2074  , it can be in t
-00002cb0: 6865 2066 6f72 6d61 7420 226f 5959 5959  he format "oYYYY
-00002cc0: 2d4d 4d2d 4444 2220 2865 2e67 2e20 223e  -MM-DD" (e.g. ">
-00002cd0: 3230 3233 2d30 312d 3031 2229 7a12 2d6d  2023-01-01")z.-m
-00002ce0: 6f64 6966 6963 6174 696f 6e2d 6461 7465  odification-date
-00002cf0: 7a13 2d2d 6d6f 6469 6669 6361 7469 6f6e  z.--modification
-00002d00: 2d64 6174 65da 116d 6f64 6966 6963 6174  -date..modificat
-00002d10: 696f 6e5f 6461 7465 7a4d 4d6f 6469 6669  ion_datezMModifi
-00002d20: 6361 7469 6f6e 2064 6174 652c 2069 7420  cation date, it 
-00002d30: 6361 6e20 6265 2069 6e20 7468 6520 666f  can be in the fo
-00002d40: 726d 6174 2022 6f59 5959 592d 4d4d 2d44  rmat "oYYYY-MM-D
-00002d50: 4422 2028 652e 672e 2022 3e32 3032 332d  D" (e.g. ">2023-
-00002d60: 3031 2d30 3122 297a 052d 7361 7665 7a06  01-01")z.-savez.
-00002d70: 2d2d 7361 7665 7a18 4669 6c65 6e61 6d65  --savez.Filename
-00002d80: 2074 6f20 7361 7665 2072 6573 756c 7473   to save results
-00002d90: 7a02 2d72 7a0b 2d2d 7265 6375 7273 6976  z.-rz.--recursiv
-00002da0: 65da 0972 6563 7572 7369 7665 7a17 5365  e..recursivez.Se
-00002db0: 6172 6368 2064 6174 6120 7265 6375 7273  arch data recurs
-00002dc0: 6976 656c 7929 0372 2400 0000 7223 0000  ively).r$...r#..
-00002dd0: 0072 2500 0000 7a0c 2d6f 626a 6563 742d  .r%...z.-object-
-00002de0: 7479 7065 7a0d 2d2d 6f62 6a65 6374 2d74  typez.--object-t
-00002df0: 7970 65da 106f 626a 6563 745f 7479 7065  ype..object_type
-00002e00: 5f63 6f64 657a 1d4f 626a 6563 7420 7479  _codez.Object ty
-00002e10: 7065 2063 6f64 6520 746f 2066 696c 7465  pe code to filte
-00002e20: 7220 6279 7a0d 2d6f 626a 6563 742d 7370  r byz.-object-sp
-00002e30: 6163 657a 0e2d 2d6f 626a 6563 742d 7370  acez.--object-sp
-00002e40: 6163 65da 0c6f 626a 6563 745f 7370 6163  ace..object_spac
-00002e50: 657a 114f 626a 6563 7420 7370 6163 6520  ez.Object space 
-00002e60: 636f 6465 7a0f 2d6f 626a 6563 742d 7072  codez.-object-pr
-00002e70: 6f6a 6563 747a 102d 2d6f 626a 6563 742d  ojectz.--object-
-00002e80: 7072 6f6a 6563 74da 0e6f 626a 6563 745f  project..object_
-00002e90: 7072 6f6a 6563 747a 2746 756c 6c20 6f62  projectz'Full ob
-00002ea0: 6a65 6374 2070 726f 6a65 6374 2069 6465  ject project ide
-00002eb0: 6e74 6966 6963 6174 696f 6e20 636f 6465  ntification code
-00002ec0: 7a12 2d6f 626a 6563 742d 636f 6c6c 6563  z.-object-collec
-00002ed0: 7469 6f6e 7a13 2d2d 6f62 6a65 6374 2d63  tionz.--object-c
-00002ee0: 6f6c 6c65 6374 696f 6eda 116f 626a 6563  ollection..objec
-00002ef0: 745f 636f 6c6c 6563 7469 6f6e 7a1b 4675  t_collectionz.Fu
-00002f00: 6c6c 206f 626a 6563 7420 636f 6c6c 6563  ll object collec
-00002f10: 7469 6f6e 2063 6f64 657a 0a2d 6f62 6a65  tion codez.-obje
-00002f20: 6374 2d69 647a 0b2d 2d6f 626a 6563 742d  ct-idz.--object-
-00002f30: 6964 da09 6f62 6a65 6374 5f69 647a 414f  id..object_idzAO
-00002f40: 626a 6563 7420 6964 656e 7469 6669 6361  bject identifica
-00002f50: 7469 6f6e 2069 6e66 6f72 6d61 7469 6f6e  tion information
-00002f60: 2c20 6974 2063 616e 2062 6520 7065 726d  , it can be perm
-00002f70: 4964 206f 7220 6964 656e 7469 6669 6572  Id or identifier
-00002f80: 7a10 2d6f 626a 6563 742d 7072 6f70 6572  z.-object-proper
-00002f90: 7479 da14 6f62 6a65 6374 5f70 726f 7065  ty..object_prope
-00002fa0: 7274 795f 636f 6465 7a14 4f62 6a65 6374  rty_codez.Object
-00002fb0: 2070 726f 7065 7274 7920 636f 6465 7a16   property codez.
-00002fc0: 2d6f 626a 6563 742d 7072 6f70 6572 7479  -object-property
-00002fd0: 2d76 616c 7565 da15 6f62 6a65 6374 5f70  -value..object_p
-00002fe0: 726f 7065 7274 795f 7661 6c75 657a 154f  roperty_valuez.O
-00002ff0: 626a 6563 7420 7072 6f70 6572 7479 2076  bject property v
-00003000: 616c 7565 7a19 2d6f 626a 6563 742d 7265  aluez.-object-re
-00003010: 6769 7374 7261 7469 6f6e 2d64 6174 657a  gistration-datez
-00003020: 1a2d 2d6f 626a 6563 742d 7265 6769 7374  .--object-regist
-00003030: 7261 7469 6f6e 2d64 6174 65da 186f 626a  ration-date..obj
-00003040: 6563 745f 7265 6769 7374 7261 7469 6f6e  ect_registration
-00003050: 5f64 6174 657a 192d 6f62 6a65 6374 2d6d  _datez.-object-m
-00003060: 6f64 6966 6963 6174 696f 6e2d 6461 7465  odification-date
-00003070: 7a1a 2d2d 6f62 6a65 6374 2d6d 6f64 6966  z.--object-modif
-00003080: 6963 6174 696f 6e2d 6461 7465 da18 6f62  ication-date..ob
-00003090: 6a65 6374 5f6d 6f64 6966 6963 6174 696f  ject_modificatio
-000030a0: 6e5f 6461 7465 da08 6461 7461 5f73 6574  n_date..data_set
-000030b0: 7a02 2d70 7a16 2d2d 6973 5f64 6174 615f  z.-pz.--is_data_
-000030c0: 7365 745f 7072 6f70 6572 7479 7a1c 436f  set_propertyz.Co
-000030d0: 6e66 6967 7572 6520 6461 7461 2073 6574  nfigure data set
-000030e0: 2070 726f 7065 7274 792e 6303 0000 0000   property.c.....
-000030f0: 0000 0000 0000 0004 0000 0004 0000 0043  ...............C
-00003100: 0000 0073 3a00 0000 7400 7c00 6a01 6401  ...s:...t.|.j.d.
-00003110: 6402 8d02 7d03 7c01 7c00 6a01 6403 3c00  d...}.|.|.j.d.<.
-00003120: 7c02 7c00 6a01 6404 3c00 7c03 7c00 6a01  |.|.j.d.<.|.|.j.
-00003130: 6405 3c00 6406 7c00 6a01 6407 3c00 6408  d.<.d.|.j.d.<.d.
-00003140: 5300 2909 7a40 2045 7874 6572 6e61 6c20  S.).z@ External 
-00003150: 4461 7461 2053 746f 7265 3a20 4765 742f  Data Store: Get/
-00003160: 7365 7420 7365 7474 696e 6773 2072 656c  set settings rel
-00003170: 6174 6564 2074 6f20 7468 6520 6461 7461  ated to the data
-00003180: 2073 6574 2e20 4672 9900 0000 7280 0000   set. Fr....r...
-00003190: 0072 8200 0000 7230 0000 0072 c300 0000  .r....r0...r....
-000031a0: 7281 0000 004e 72a3 0000 0029 0472 2b00  r....Nr....).r+.
-000031b0: 0000 7280 0000 0072 8200 0000 7230 0000  ..r....r....r0..
-000031c0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-000031d0: 72c3 0000 003b 0100 0073 0a00 0000 0e07  r....;...s......
-000031e0: 0a01 0a01 0a01 0e01 da11 6461 7461 5f73  ..........data_s
-000031f0: 6574 5f73 6574 7469 6e67 7363 0200 0000  et_settingsc....
-00003200: 0000 0000 0000 0000 0200 0000 0600 0000  ................
-00003210: 0300 0000 72a7 0000 0029 057a 3c20 4578  ....r....).z< Ex
-00003220: 7465 726e 616c 2044 6174 6120 5374 6f72  ternal Data Stor
-00003230: 653a 2053 6574 2073 6574 7469 6e67 7320  e: Set settings 
-00003240: 7265 6c61 7465 6420 746f 2074 6865 2064  related to the d
-00003250: 6174 6120 7365 742e 2072 3000 0000 da0c  ata set. r0.....
-00003260: 6461 7461 5f73 6574 5f73 6574 6301 0000  data_set_setc...
-00003270: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-00003280: 0013 0000 0072 a900 0000 721a 0000 0072  .....r....r....r
-00003290: aa00 0000 7232 0000 00a9 0272 2b00 0000  ....r2.....r+...
-000032a0: 72c4 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-000032b0: 3600 0000 4e01 0000 7237 0000 007a 1e64  6...N...r7...z.d
-000032c0: 6174 615f 7365 745f 7365 742e 3c6c 6f63  ata_set_set.<loc
-000032d0: 616c 733e 2e3c 6c61 6d62 6461 3e72 ac00  als>.<lambda>r..
-000032e0: 0000 72c6 0000 0072 1200 0000 72c6 0000  ..r....r....r...
-000032f0: 0072 1300 0000 72c5 0000 0049 0100 0072  .r....r....I...r
-00003300: ad00 0000 72c5 0000 0063 0200 0000 0000  ....r....c......
-00003310: 0000 0000 0000 0200 0000 0600 0000 0300  ................
-00003320: 0000 72a7 0000 0029 057a 3c20 4578 7465  ..r....).z< Exte
-00003330: 726e 616c 2044 6174 6120 5374 6f72 653a  rnal Data Store:
-00003340: 2047 6574 2073 6574 7469 6e67 7320 7265   Get settings re
-00003350: 6c61 7465 6420 746f 2074 6865 2064 6174  lated to the dat
-00003360: 6120 7365 742e 2072 3000 0000 da0c 6461  a set. r0.....da
-00003370: 7461 5f73 6574 5f67 6574 6301 0000 0000  ta_set_getc.....
-00003380: 0000 0000 0000 0001 0000 0003 0000 0013  ................
-00003390: 0000 0072 a900 0000 721a 0000 0072 af00  ...r....r....r..
-000033a0: 0000 7232 0000 0072 c600 0000 7212 0000  ..r2...r....r...
-000033b0: 0072 1300 0000 7236 0000 0056 0100 0072  .r....r6...V...r
-000033c0: 3700 0000 7a1e 6461 7461 5f73 6574 5f67  7...z.data_set_g
-000033d0: 6574 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  et.<locals>.<lam
-000033e0: 6264 613e 72ac 0000 0072 c600 0000 7212  bda>r....r....r.
-000033f0: 0000 0072 c600 0000 7213 0000 0072 c700  ...r....r....r..
-00003400: 0000 5101 0000 72ad 0000 0072 c700 0000  ..Q...r....r....
-00003410: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00003420: 0006 0000 0003 0000 0072 a700 0000 2905  .........r....).
-00003430: 7a3e 2045 7874 6572 6e61 6c20 4461 7461  z> External Data
-00003440: 2053 746f 7265 3a20 436c 6561 7220 7365   Store: Clear se
-00003450: 7474 696e 6773 2072 656c 6174 6564 2074  ttings related t
-00003460: 6f20 7468 6520 6461 7461 2073 6574 2e20  o the data set. 
-00003470: 7230 0000 00da 0e64 6174 615f 7365 745f  r0.....data_set_
-00003480: 636c 6561 7263 0100 0000 0000 0000 0000  clearc..........
-00003490: 0000 0100 0000 0300 0000 1300 0000 72a9  ..............r.
-000034a0: 0000 0072 1a00 0000 72b2 0000 0072 3200  ...r....r....r2.
-000034b0: 0000 72c6 0000 0072 1200 0000 7213 0000  ..r....r....r...
-000034c0: 0072 3600 0000 5e01 0000 7237 0000 007a  .r6...^...r7...z
-000034d0: 2064 6174 615f 7365 745f 636c 6561 722e   data_set_clear.
-000034e0: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-000034f0: 3e72 ac00 0000 72c6 0000 0072 1200 0000  >r....r....r....
-00003500: 72c6 0000 0072 1300 0000 72c8 0000 0059  r....r....r....Y
-00003510: 0100 0072 ad00 0000 72c8 0000 0063 0200  ...r....r....c..
-00003520: 0000 0000 0000 0000 0000 0200 0000 0200  ................
-00003530: 0000 4300 0000 7320 0000 007c 0064 0075  ..C...s ...|.d.u
-00003540: 0072 087c 0164 0075 0170 0f7c 0064 0075  .r.|.d.u.p.|.d.u
-00003550: 016f 0f7c 0164 0075 0053 0072 1a00 0000  .o.|.d.u.S.r....
-00003560: 7212 0000 0029 02da 0670 6172 616d 31da  r....)...param1.
-00003570: 0670 6172 616d 3272 1200 0000 7212 0000  .param2r....r...
-00003580: 0072 1300 0000 da10 5f70 6169 725f 6973  .r......_pair_is
-00003590: 5f6e 6f74 5f73 6574 6101 0000 7302 0000  _not_seta...s...
-000035a0: 0020 0172 cb00 0000 da06 7365 6172 6368  . .r......search
-000035b0: 7a2f 5365 6172 6368 2066 6f72 2064 6174  z/Search for dat
-000035c0: 6173 6574 7320 7573 696e 6720 6120 6669  asets using a fi
-000035d0: 6c74 6572 696e 6720 6372 6974 6572 6961  ltering criteria
-000035e0: 2e29 01da 0a73 686f 7274 5f68 656c 7063  .)...short_helpc
-000035f0: 1500 0000 0000 0000 0000 0000 1600 0000  ................
-00003600: 1100 0000 0300 0000 733c 0100 007c 017c  ........s<...|.|
-00003610: 027c 037c 047c 057c 067c 087c 097c 0c7c  .|.|.|.|.|.|.|.|
-00003620: 0d7c 0e7c 0f7c 107c 117c 127c 137c 1467  .|.|.|.|.|.|.|.g
-00003630: 117d 1574 0064 0164 0284 007c 157c 0767  .}.t.d.d...|.|.g
-00003640: 0117 0044 0083 0183 0172 2574 0164 0383  ...D.....r%t.d..
-00003650: 0101 0064 0453 0074 027c 087c 0983 0273  ...d.S.t.|.|...s
-00003660: 2f74 027c 117c 1283 0272 3574 0164 0583  /t.|.|...r5t.d..
-00003670: 0101 0064 0453 0074 037c 006a 0464 0664  ...d.S.t.|.j.d.d
-00003680: 078d 027c 006a 0464 083c 007c 0764 0975  ...|.j.d.<.|.d.u
-00003690: 0172 5674 0564 0a64 0284 007c 1544 0083  .rVt.d.d...|.D..
-000036a0: 0183 0172 5074 0164 0b83 0101 0074 067c  ...rPt.d.....t.|
-000036b0: 0764 0c8d 0189 006e 3874 0664 2169 0064  .d.....n8t.d!i.d
-000036c0: 0d7c 0193 0164 0e7c 0293 0164 0f7c 0393  .|...d.|...d.|..
-000036d0: 0164 107c 0493 0164 117c 0893 0164 127c  .d.|...d.|...d.|
-000036e0: 0593 0164 137c 0693 0164 147c 0993 0164  ...d.|...d.|...d
-000036f0: 157c 0c93 0164 167c 0d93 0164 177c 0e93  .|...d.|...d.|..
-00003700: 0164 187c 0f93 0164 197c 1093 0164 1a7c  .d.|...d.|...d.|
-00003710: 1193 0164 1b7c 1293 0164 1c7c 1393 0164  ...d.|...d.|...d
-00003720: 1d7c 1493 018e 0189 007c 006a 0464 0819  .|.......|.j.d..
-00003730: 00a0 0764 1e87 0087 0187 0266 0364 1f64  ...d.......f.d.d
-00003740: 2084 08a1 0266 0153 0029 227a 9453 7461   ....f.S.)"z.Sta
-00003750: 6e64 6172 6420 4461 7461 2053 746f 7265  ndard Data Store
-00003760: 3a20 5365 6172 6368 2064 6174 6120 7365  : Search data se
-00003770: 7473 2067 6976 656e 2074 6865 2066 696c  ts given the fil
-00003780: 7465 7269 6e67 2063 7269 7465 7269 6120  tering criteria 
-00003790: 6f72 206f 626a 6563 7420 6964 656e 7469  or object identi
-000037a0: 6669 6572 2e0a 2020 2020 5265 7375 6c74  fier..    Result
-000037b0: 7320 6f66 2074 6869 7320 636f 6d6d 616e  s of this comman
-000037c0: 6420 6361 6e20 6265 2075 7365 6420 696e  d can be used in
-000037d0: 2060 6f62 6973 2064 6f77 6e6c 6f61 6460   `obis download`
-000037e0: 2e63 0100 0000 0000 0000 0000 0000 0200  .c..............
-000037f0: 0000 0300 0000 7300 0000 f318 0000 0081  ......s.........
-00003800: 007c 005d 077d 017c 0164 0075 0056 0001  .|.].}.|.d.u.V..
-00003810: 0071 0264 0053 0072 1a00 0000 7212 0000  .q.d.S.r....r...
-00003820: 00a9 02da 022e 30da 0176 7212 0000 0072  ......0..vr....r
-00003830: 1200 0000 7213 0000 00da 093c 6765 6e65  ....r......<gene
-00003840: 7870 723e 7401 0000 f304 0000 0002 8016  xpr>t...........
-00003850: 007a 2264 6174 615f 7365 745f 7365 6172  .z"data_set_sear
-00003860: 6368 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  ch.<locals>.<gen
-00003870: 6578 7072 3efa 3159 6f75 206d 7573 7420  expr>.1You must 
-00003880: 7072 6f76 6964 6520 6174 206c 6561 7374  provide at least
-00003890: 206f 6e65 2066 696c 7465 7269 6e67 2063   one filtering c
-000038a0: 7269 7465 7269 6121 723b 0000 007a 3c50  riteria!r;...z<P
-000038b0: 726f 7065 7274 7920 636f 6465 2061 6e64  roperty code and
-000038c0: 2070 726f 7065 7274 7920 7661 6c75 6520   property value 
-000038d0: 7061 6972 206e 6565 6473 2074 6f20 6265  pair needs to be
-000038e0: 2073 7065 6369 6669 6564 2146 7299 0000   specified!Fr...
-000038f0: 0072 3000 0000 4e63 0100 0000 0000 0000  .r0...Nc........
-00003900: 0000 0000 0200 0000 0300 0000 7300 0000  ............s...
-00003910: f318 0000 0081 007c 005d 077d 017c 0164  .......|.].}.|.d
-00003920: 0075 0156 0001 0071 0264 0053 0072 1a00  .u.V...q.d.S.r..
-00003930: 0000 7212 0000 0072 cf00 0000 7212 0000  ..r....r....r...
-00003940: 0072 1200 0000 7213 0000 0072 d200 0000  .r....r....r....
-00003950: 7d01 0000 72d3 0000 007a 4944 6174 6173  }...r....zIDatas
-00003960: 6574 2069 6420 7061 7261 6d65 7465 7220  et id parameter 
-00003970: 6465 7465 6374 6564 2120 4f74 6865 7220  detected! Other 
-00003980: 6669 6c74 6572 696e 6720 6172 6775 6d65  filtering argume
-00003990: 6e74 7320 7769 6c6c 2062 6520 6f6d 6974  nts will be omit
-000039a0: 7465 6421 2901 72b3 0000 0072 b400 0000  ted!).r....r....
-000039b0: da05 7370 6163 65da 0770 726f 6a65 6374  ..space..project
-000039c0: da0a 6578 7065 7269 6d65 6e74 72b5 0000  ..experimentr...
-000039d0: 0072 b700 0000 72b8 0000 0072 b600 0000  .r....r....r....
-000039e0: 72ba 0000 0072 bb00 0000 72bc 0000 0072  r....r....r....r
-000039f0: bd00 0000 72be 0000 0072 bf00 0000 72c0  ....r....r....r.
-00003a00: 0000 0072 c100 0000 72c2 0000 00da 0f64  ...r....r......d
-00003a10: 6174 615f 7365 745f 7365 6172 6368 6301  ata_set_searchc.
-00003a20: 0000 0000 0000 0000 0000 0001 0000 0005  ................
-00003a30: 0000 0013 0000 00f3 0e00 0000 7c00 a000  ............|...
-00003a40: 8800 8801 8802 a103 5300 721a 0000 0029  ........S.r....)
-00003a50: 01da 0f73 6561 7263 685f 6461 7461 5f73  ...search_data_s
-00003a60: 6574 7232 0000 00a9 03da 0766 696c 7465  etr2.......filte
-00003a70: 7273 72b9 0000 00da 0473 6176 6572 1200  rsr......saver..
-00003a80: 0000 7213 0000 0072 3600 0000 8c01 0000  ..r....r6.......
-00003a90: f302 0000 000e 007a 2164 6174 615f 7365  .......z!data_se
-00003aa0: 745f 7365 6172 6368 2e3c 6c6f 6361 6c73  t_search.<locals
-00003ab0: 3e2e 3c6c 616d 6264 613e 7212 0000 0029  >.<lambda>r....)
-00003ac0: 08da 0361 6c6c 7208 0000 0072 cb00 0000  ...allr....r....
-00003ad0: 7209 0000 0072 2a00 0000 da03 616e 79da  r....r*.....any.
-00003ae0: 0464 6963 7472 3800 0000 2916 722b 0000  .dictr8...).r+..
-00003af0: 0072 b400 0000 72d6 0000 0072 d700 0000  .r....r....r....
-00003b00: da0a 636f 6c6c 6563 7469 6f6e 72b7 0000  ..collectionr...
-00003b10: 0072 b800 0000 72b3 0000 0072 b500 0000  .r....r....r....
-00003b20: 72b6 0000 0072 de00 0000 72b9 0000 0072  r....r....r....r
-00003b30: ba00 0000 72bb 0000 0072 bc00 0000 72bd  ....r....r....r.
-00003b40: 0000 0072 be00 0000 72bf 0000 0072 c000  ...r....r....r..
-00003b50: 0000 72c1 0000 0072 c200 0000 da13 6669  ..r....r......fi
-00003b60: 6c74 6572 696e 675f 6172 6775 6d65 6e74  ltering_argument
-00003b70: 7372 1200 0000 72dc 0000 0072 1300 0000  sr....r....r....
-00003b80: 72d9 0000 0065 0100 0073 6a00 0000 0a0a  r....e...sj.....
-00003b90: 0601 0801 0601 0401 04fc 1805 0801 0401  ................
-00003ba0: 0e01 0201 04ff 0802 0401 1401 0801 1201  ................
-00003bb0: 0801 0c01 1402 0401 02ff 0401 02ff 0401  ................
-00003bc0: 02ff 0402 02fe 0402 02fe 0403 02fd 0403  ................
-00003bd0: 02fd 0404 02fc 0404 02fc 0405 02fb 0405  ................
-00003be0: 02fb 0406 02fa 0407 02f9 0408 02f8 0409  ................
-00003bf0: 04f7 0c0a 0e01 06ff 72d9 0000 0063 0200  ........r....c..
-00003c00: 0000 0000 0000 0000 0000 0300 0000 0400  ................
-00003c10: 0000 4300 0000 72a2 0000 0029 087a 9e20  ..C...r....).z. 
-00003c20: 4578 7465 726e 616c 2044 6174 6120 5374  External Data St
-00003c30: 6f72 653a 2047 6574 2f73 6574 2070 726f  ore: Get/set pro
-00003c40: 7065 7274 6965 7320 7265 6c61 7465 6420  perties related 
-00003c50: 746f 2074 6865 206f 626a 6563 742e 0a0a  to the object...
-00003c60: 2020 2020 5374 616e 6461 7264 2044 6174      Standard Dat
-00003c70: 6120 5374 6f72 653a 2047 6574 2f73 6574  a Store: Get/set
-00003c80: 2070 726f 7065 7274 6965 7320 6f66 206f   properties of o
-00003c90: 626a 6563 7473 2063 6f6e 6e65 6374 6564  bjects connected
-00003ca0: 2074 6f20 646f 776e 6c6f 6164 6564 2064   to downloaded d
-00003cb0: 6174 6173 6574 732e 0a20 2020 2046 7299  atasets..    Fr.
-00003cc0: 0000 0072 8000 0000 7230 0000 00da 066f  ...r....r0.....o
-00003cd0: 626a 6563 7472 8100 0000 4e72 a300 0000  bjectr....Nr....
-00003ce0: 72a4 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
-00003cf0: 1300 0000 72e5 0000 0092 0100 00f3 0800  ....r...........
-00003d00: 0000 0e08 0a01 0a01 0e01 72e5 0000 00da  ..........r.....
-00003d10: 0f6f 626a 6563 745f 7365 7474 696e 6773  .object_settings
-00003d20: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00003d30: 0006 0000 0003 0000 0072 a700 0000 2905  .........r....).
-00003d40: 7a98 2045 7874 6572 6e61 6c20 4461 7461  z. External Data
-00003d50: 2053 746f 7265 3a20 5365 7420 7072 6f70   Store: Set prop
-00003d60: 6572 7469 6573 2072 656c 6174 6564 2074  erties related t
-00003d70: 6f20 7468 6520 6f62 6a65 6374 2e0a 0a20  o the object... 
-00003d80: 2020 2053 7461 6e64 6172 6420 4461 7461     Standard Data
-00003d90: 2053 746f 7265 3a20 5365 7420 7072 6f70   Store: Set prop
-00003da0: 6572 7479 2074 6f20 616c 6c20 6f62 6a65  erty to all obje
-00003db0: 6374 7320 636f 6e6e 6563 7465 6420 746f  cts connected to
-00003dc0: 2064 6f77 6e6c 6f61 6465 6420 6461 7461   downloaded data
-00003dd0: 7365 7473 2e0a 2020 2020 7230 0000 00da  sets..    r0....
-00003de0: 0a6f 626a 6563 745f 7365 7463 0100 0000  .object_setc....
-00003df0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00003e00: 1300 0000 72a9 0000 0072 1a00 0000 72aa  ....r....r....r.
-00003e10: 0000 0072 3200 0000 a902 722b 0000 0072  ...r2.....r+...r
-00003e20: e700 0000 7212 0000 0072 1300 0000 7236  ....r....r....r6
-00003e30: 0000 00a8 0100 0072 3700 0000 7a1c 6f62  .......r7...z.ob
-00003e40: 6a65 6374 5f73 6574 2e3c 6c6f 6361 6c73  ject_set.<locals
-00003e50: 3e2e 3c6c 616d 6264 613e 72ac 0000 0072  >.<lambda>r....r
-00003e60: e900 0000 7212 0000 0072 e900 0000 7213  ....r....r....r.
-00003e70: 0000 0072 e800 0000 a001 0000 f302 0000  ...r............
-00003e80: 001c 0872 e800 0000 6302 0000 0000 0000  ...r....c.......
-00003e90: 0000 0000 0002 0000 0006 0000 0003 0000  ................
-00003ea0: 0072 a700 0000 2905 7aa0 2045 7874 6572  .r....).z. Exter
-00003eb0: 6e61 6c20 4461 7461 2053 746f 7265 3a20  nal Data Store: 
-00003ec0: 5365 7420 7072 6f70 6572 7469 6573 2072  Set properties r
-00003ed0: 656c 6174 6564 2074 6f20 7468 6520 6f62  elated to the ob
-00003ee0: 6a65 6374 2e0a 0a20 2020 2053 7461 6e64  ject...    Stand
-00003ef0: 6172 6420 4461 7461 2053 746f 7265 3a20  ard Data Store: 
-00003f00: 4765 7420 6769 7665 6e20 7072 6f70 6572  Get given proper
-00003f10: 7469 6573 206f 6620 616c 6c20 6f62 6a65  ties of all obje
-00003f20: 6374 7320 636f 6e6e 6563 7465 6420 746f  cts connected to
-00003f30: 2064 6f77 6e6c 6f61 6465 6420 6461 7461   downloaded data
-00003f40: 7365 7473 2e0a 2020 2020 7230 0000 00da  sets..    r0....
-00003f50: 0a6f 626a 6563 745f 6765 7463 0100 0000  .object_getc....
-00003f60: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00003f70: 1300 0000 72a9 0000 0072 1a00 0000 72af  ....r....r....r.
-00003f80: 0000 0072 3200 0000 72e9 0000 0072 1200  ...r2...r....r..
-00003f90: 0000 7213 0000 0072 3600 0000 b301 0000  ..r....r6.......
-00003fa0: 7237 0000 007a 1c6f 626a 6563 745f 6765  r7...z.object_ge
-00003fb0: 742e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  t.<locals>.<lamb
-00003fc0: 6461 3e72 ac00 0000 72e9 0000 0072 1200  da>r....r....r..
-00003fd0: 0000 72e9 0000 0072 1300 0000 72eb 0000  ..r....r....r...
-00003fe0: 00ab 0100 0072 ea00 0000 72eb 0000 0063  .....r....r....c
-00003ff0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00004000: 0600 0000 0300 0000 72a7 0000 0029 057a  ........r....).z
-00004010: 3e20 4578 7465 726e 616c 2044 6174 6120  > External Data 
-00004020: 5374 6f72 653a 2043 6c65 6172 2070 726f  Store: Clear pro
-00004030: 7065 7274 6965 7320 7265 6c61 7465 6420  perties related 
-00004040: 746f 2074 6865 206f 626a 6563 742e 2072  to the object. r
-00004050: 3000 0000 da0c 6f62 6a65 6374 5f63 6c65  0.....object_cle
-00004060: 6172 6301 0000 0000 0000 0000 0000 0001  arc.............
-00004070: 0000 0003 0000 0013 0000 0072 a900 0000  ...........r....
-00004080: 721a 0000 0072 b200 0000 7232 0000 0072  r....r....r2...r
-00004090: e900 0000 7212 0000 0072 1300 0000 7236  ....r....r....r6
-000040a0: 0000 00bb 0100 0072 3700 0000 7a1e 6f62  .......r7...z.ob
-000040b0: 6a65 6374 5f63 6c65 6172 2e3c 6c6f 6361  ject_clear.<loca
-000040c0: 6c73 3e2e 3c6c 616d 6264 613e 72ac 0000  ls>.<lambda>r...
-000040d0: 0072 e900 0000 7212 0000 0072 e900 0000  .r....r....r....
-000040e0: 7213 0000 0072 ec00 0000 b601 0000 72ad  r....r........r.
-000040f0: 0000 0072 ec00 0000 7a20 4675 6c6c 2070  ...r....z Full p
-00004100: 726f 6a65 6374 2069 6465 6e74 6966 6963  roject identific
-00004110: 6174 696f 6e20 636f 6465 7a14 4675 6c6c  ation codez.Full
-00004120: 2063 6f6c 6c65 6374 696f 6e20 636f 6465   collection code
-00004130: 7a07 2d6f 626a 6563 747a 082d 2d6f 626a  z.-objectz.--obj
-00004140: 6563 747a 0954 7970 6520 636f 6465 7a2e  ectz.Type codez.
-00004150: 5365 6172 6368 2066 6f72 206f 626a 6563  Search for objec
-00004160: 7473 2075 7369 6e67 2061 2066 696c 7465  ts using a filte
-00004170: 7269 6e67 2063 7269 7465 7269 612e 630c  ring criteria.c.
-00004180: 0000 0000 0000 0000 0000 000d 0000 000a  ................
-00004190: 0000 0003 0000 0073 dc00 0000 7c01 7c02  .......s....|.|.
-000041a0: 7c03 7c04 7c05 7c06 7c08 7c09 6708 7d0c  |.|.|.|.|.|.g.}.
-000041b0: 7400 6401 6402 8400 7c0c 7c07 6701 1700  t.d.d...|.|.g...
-000041c0: 4400 8301 8301 721c 7401 6403 8301 0100  D.....r.t.d.....
-000041d0: 6404 5300 7c08 6405 7500 7224 7c09 6405  d.S.|.d.u.r$|.d.
-000041e0: 7501 732c 7c08 6405 7501 7232 7c09 6405  u.s,|.d.u.r2|.d.
-000041f0: 7500 7232 7401 6406 8301 0100 6404 5300  u.r2t.d.....d.S.
-00004200: 7402 7c00 6a03 6407 6408 8d02 7c00 6a03  t.|.j.d.d...|.j.
-00004210: 6409 3c00 7c07 6405 7501 7253 7404 640a  d.<.|.d.u.rSt.d.
-00004220: 6402 8400 7c0c 4400 8301 8301 724d 7401  d...|.D.....rMt.
-00004230: 640b 8301 0100 7405 7c07 640c 8d01 8900  d.....t.|.d.....
-00004240: 6e0c 7405 7c01 7c02 7c03 7c04 7c08 7c05  n.t.|.|.|.|.|.|.
-00004250: 7c06 7c09 640d 8d08 8900 7c00 6a03 6409  |.|.d.....|.j.d.
-00004260: 1900 a006 640e 8700 8701 8702 6603 640f  ....d.......f.d.
-00004270: 6410 8408 a102 5300 2911 7a58 5374 616e  d.....S.).zXStan
-00004280: 6461 7264 2044 6174 6120 5374 6f72 653a  dard Data Store:
-00004290: 2053 6561 7263 6820 666f 7220 6f62 6a65   Search for obje
-000042a0: 6374 7320 7573 696e 6720 6120 6669 6c74  cts using a filt
-000042b0: 6572 696e 6720 6372 6974 6572 6961 206f  ering criteria o
-000042c0: 7220 6f62 6a65 6374 2069 6465 6e74 6966  r object identif
-000042d0: 6965 722e 6301 0000 0000 0000 0000 0000  ier.c...........
-000042e0: 0002 0000 0003 0000 0073 0000 0072 ce00  .........s...r..
-000042f0: 0000 721a 0000 0072 1200 0000 72cf 0000  ..r....r....r...
-00004300: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-00004310: 72d2 0000 00da 0100 0072 d300 0000 7a20  r........r....z 
-00004320: 6f62 6a65 6374 5f73 6561 7263 682e 3c6c  object_search.<l
-00004330: 6f63 616c 733e 2e3c 6765 6e65 7870 723e  ocals>.<genexpr>
-00004340: 72d4 0000 0072 3b00 0000 4e7a 3650 726f  r....r;...Nz6Pro
-00004350: 7065 7274 7920 636f 6465 2061 6e64 2070  perty code and p
-00004360: 726f 7065 7274 7920 7661 6c75 6520 6e65  roperty value ne
-00004370: 6564 2074 6f20 6265 2073 7065 6369 6669  ed to be specifi
-00004380: 6564 2146 7299 0000 0072 3000 0000 6301  ed!Fr....r0...c.
-00004390: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000043a0: 0000 0073 0000 0072 d500 0000 721a 0000  ...s...r....r...
-000043b0: 0072 1200 0000 72cf 0000 0072 1200 0000  .r....r....r....
-000043c0: 7212 0000 0072 1300 0000 72d2 0000 00e3  r....r....r.....
-000043d0: 0100 0072 d300 0000 7a45 4f62 6a65 6374  ...r....zEObject
-000043e0: 2070 6172 616d 6574 6572 2064 6574 6563   parameter detec
-000043f0: 7465 6421 204f 7468 6572 2066 696c 7465  ted! Other filte
-00004400: 7269 6e67 2061 7267 756d 656e 7473 2077  ring arguments w
-00004410: 696c 6c20 6265 206f 6d69 7474 6564 2129  ill be omitted!)
-00004420: 01da 0b6f 626a 6563 745f 636f 6465 2908  ...object_code).
-00004430: 72b4 0000 0072 d600 0000 72d7 0000 0072  r....r....r....r
-00004440: e300 0000 72b5 0000 0072 b700 0000 72b8  ....r....r....r.
-00004450: 0000 0072 b600 0000 da0d 6f62 6a65 6374  ...r......object
-00004460: 5f73 6561 7263 6863 0100 0000 0000 0000  _searchc........
-00004470: 0000 0000 0100 0000 0500 0000 1300 0000  ................
-00004480: 72da 0000 0072 1a00 0000 2901 da0d 7365  r....r....)...se
-00004490: 6172 6368 5f6f 626a 6563 7472 3200 0000  arch_objectr2...
-000044a0: 72dc 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
-000044b0: 3600 0000 ec01 0000 72df 0000 007a 1f6f  6.......r....z.o
-000044c0: 626a 6563 745f 7365 6172 6368 2e3c 6c6f  bject_search.<lo
-000044d0: 6361 6c73 3e2e 3c6c 616d 6264 613e 2907  cals>.<lambda>).
-000044e0: 72e0 0000 0072 0800 0000 7209 0000 0072  r....r....r....r
-000044f0: 2a00 0000 72e1 0000 0072 e200 0000 7238  *...r....r....r8
-00004500: 0000 0029 0d72 2b00 0000 72b4 0000 0072  ...).r+...r....r
-00004510: d600 0000 72d7 0000 0072 e300 0000 72b7  ....r....r....r.
-00004520: 0000 0072 b800 0000 72be 0000 0072 b500  ...r....r....r..
-00004530: 0000 72b6 0000 0072 de00 0000 72b9 0000  ..r....r....r...
-00004540: 0072 e400 0000 7212 0000 0072 dc00 0000  .r....r....r....
-00004550: 7213 0000 0072 ee00 0000 d201 0000 7334  r....r........s4
-00004560: 0000 000a 0606 0104 ff18 0208 0104 0110  ................
-00004570: 0106 0102 ff06 0102 ff08 0204 0114 0108  ................
-00004580: 0112 0108 010c 0106 0206 0104 0102 0106  ................
-00004590: fd0c 040e 0104 ff72 ee00 0000 6302 0000  .......r....c...
-000045a0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-000045b0: 0043 0000 0072 a200 0000 2908 7aa8 2045  .C...r....).z. E
-000045c0: 7874 6572 6e61 6c20 4461 7461 2053 746f  xternal Data Sto
-000045d0: 7265 3a20 4765 742f 7365 7420 7365 7474  re: Get/set sett
-000045e0: 696e 6773 2072 656c 6174 6564 2074 6f20  ings related to 
-000045f0: 7468 6520 636f 6c6c 6563 7469 6f6e 2e0a  the collection..
-00004600: 0a20 2020 2053 7461 6e64 6172 6420 4461  .    Standard Da
-00004610: 7461 2053 746f 7265 3a20 4765 742f 7365  ta Store: Get/se
-00004620: 7420 7072 6f70 6572 7469 6573 206f 6620  t properties of 
-00004630: 616c 6c20 636f 6c6c 6563 7469 6f6e 7320  all collections 
-00004640: 636f 6e6e 6563 7465 6420 746f 2064 6f77  connected to dow
-00004650: 6e6c 6f61 6465 6420 6461 7461 7365 7473  nloaded datasets
-00004660: 2e0a 2020 2020 4672 9900 0000 7280 0000  ..    Fr....r...
-00004670: 0072 3000 0000 72e3 0000 0072 8100 0000  .r0...r....r....
-00004680: 4e72 a300 0000 72a4 0000 0072 1200 0000  Nr....r....r....
-00004690: 7212 0000 0072 1300 0000 72e3 0000 00f2  r....r....r.....
-000046a0: 0100 0072 e600 0000 72e3 0000 0063 0200  ...r....r....c..
-000046b0: 0000 0000 0000 0000 0000 0200 0000 0600  ................
-000046c0: 0000 0300 0000 72a7 0000 0029 057a a620  ......r....).z. 
-000046d0: 4578 7465 726e 616c 2044 6174 6120 5374  External Data St
-000046e0: 6f72 653a 2053 6574 2073 6574 7469 6e67  ore: Set setting
-000046f0: 7320 7265 6c61 7465 6420 746f 2074 6865  s related to the
-00004700: 2063 6f6c 6c65 6374 696f 6e2e 0a0a 2020   collection...  
-00004710: 2020 5374 616e 6461 7264 2044 6174 6120    Standard Data 
-00004720: 5374 6f72 653a 2053 6574 2067 6976 656e  Store: Set given
-00004730: 2070 726f 7065 7274 6965 7320 6f66 2061   properties of a
-00004740: 6c6c 2063 6f6c 6c65 6374 696f 6e73 2063  ll collections c
-00004750: 6f6e 6e65 6374 6564 2074 6f20 646f 776e  onnected to down
-00004760: 6c6f 6164 6564 2064 6174 6173 6574 732e  loaded datasets.
-00004770: 0a20 2020 2072 3000 0000 da0e 636f 6c6c  .    r0.....coll
-00004780: 6563 7469 6f6e 5f73 6574 6301 0000 0000  ection_setc.....
-00004790: 0000 0000 0000 0001 0000 0003 0000 0013  ................
-000047a0: 0000 0072 a900 0000 721a 0000 0072 aa00  ...r....r....r..
-000047b0: 0000 7232 0000 0072 ab00 0000 7212 0000  ..r2...r....r...
-000047c0: 0072 1300 0000 7236 0000 0008 0200 0072  .r....r6.......r
-000047d0: 3700 0000 7a20 636f 6c6c 6563 7469 6f6e  7...z collection
-000047e0: 5f73 6574 2e3c 6c6f 6361 6c73 3e2e 3c6c  _set.<locals>.<l
-000047f0: 616d 6264 613e 72ac 0000 0072 ab00 0000  ambda>r....r....
-00004800: 7212 0000 0072 ab00 0000 7213 0000 0072  r....r....r....r
-00004810: f000 0000 0002 0000 72ea 0000 0072 f000  ........r....r..
-00004820: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
-00004830: 0000 0006 0000 0003 0000 0072 a700 0000  ...........r....
-00004840: 2905 7aa6 2045 7874 6572 6e61 6c20 4461  ).z. External Da
-00004850: 7461 2053 746f 7265 3a20 4765 7420 7365  ta Store: Get se
-00004860: 7474 696e 6773 2072 656c 6174 6564 2074  ttings related t
-00004870: 6f20 7468 6520 636f 6c6c 6563 7469 6f6e  o the collection
-00004880: 2e0a 0a20 2020 2053 7461 6e64 6172 6420  ...    Standard 
-00004890: 4461 7461 2053 746f 7265 3a20 4765 7420  Data Store: Get 
-000048a0: 6769 7665 6e20 7072 6f70 6572 7469 6573  given properties
-000048b0: 206f 6620 616c 6c20 636f 6c6c 6563 7469   of all collecti
-000048c0: 6f6e 7320 636f 6e6e 6563 7465 6420 746f  ons connected to
-000048d0: 2064 6f77 6e6c 6f61 6465 6420 6461 7461   downloaded data
-000048e0: 7365 7473 2e0a 2020 2020 7230 0000 00da  sets..    r0....
-000048f0: 0e63 6f6c 6c65 6374 696f 6e5f 6765 7463  .collection_getc
-00004900: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00004910: 0300 0000 1300 0000 72a9 0000 0072 1a00  ........r....r..
-00004920: 0000 72af 0000 0072 3200 0000 72ab 0000  ..r....r2...r...
-00004930: 0072 1200 0000 7213 0000 0072 3600 0000  .r....r....r6...
-00004940: 1302 0000 7237 0000 007a 2063 6f6c 6c65  ....r7...z colle
-00004950: 6374 696f 6e5f 6765 742e 3c6c 6f63 616c  ction_get.<local
-00004960: 733e 2e3c 6c61 6d62 6461 3e72 ac00 0000  s>.<lambda>r....
-00004970: 72ab 0000 0072 1200 0000 72ab 0000 0072  r....r....r....r
-00004980: 1300 0000 72f1 0000 000b 0200 0072 ea00  ....r........r..
-00004990: 0000 72f1 0000 0063 0200 0000 0000 0000  ..r....c........
-000049a0: 0000 0000 0200 0000 0600 0000 0300 0000  ................
-000049b0: 72a7 0000 0029 057a 3e45 7874 6572 6e61  r....).z>Externa
-000049c0: 6c20 4461 7461 2053 746f 7265 3a20 436c  l Data Store: Cl
-000049d0: 6561 7220 7365 7474 696e 6773 2072 656c  ear settings rel
-000049e0: 6174 6564 2074 6f20 7468 6520 636f 6c6c  ated to the coll
-000049f0: 6563 7469 6f6e 2e72 3000 0000 da10 636f  ection.r0.....co
-00004a00: 6c6c 6563 7469 6f6e 5f63 6c65 6172 6301  llection_clearc.
-00004a10: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00004a20: 0000 0013 0000 0072 a900 0000 721a 0000  .......r....r...
-00004a30: 0072 b200 0000 7232 0000 0072 ab00 0000  .r....r2...r....
-00004a40: 7212 0000 0072 1300 0000 7236 0000 001b  r....r....r6....
-00004a50: 0200 0072 3700 0000 7a22 636f 6c6c 6563  ...r7...z"collec
-00004a60: 7469 6f6e 5f63 6c65 6172 2e3c 6c6f 6361  tion_clear.<loca
-00004a70: 6c73 3e2e 3c6c 616d 6264 613e 72ac 0000  ls>.<lambda>r...
-00004a80: 0072 ab00 0000 7212 0000 0072 ab00 0000  .r....r....r....
-00004a90: 7213 0000 0072 f200 0000 1602 0000 72ad  r....r........r.
-00004aa0: 0000 0072 f200 0000 6302 0000 0000 0000  ...r....c.......
-00004ab0: 0000 0000 0003 0000 0005 0000 0043 0000  .............C..
-00004ac0: 0073 4a00 0000 7c01 6401 7500 720d 7400  .sJ...|.d.u.r.t.
-00004ad0: 7c00 6a01 6402 6401 6403 8d03 7d02 6e07  |.j.d.d.d...}.n.
-00004ae0: 7400 7c00 6a01 6402 6404 8d02 7d02 7c01  t.|.j.d.d...}.|.
-00004af0: 7c00 6a01 6405 3c00 7c02 7c00 6a01 6406  |.j.d.<.|.|.j.d.
-00004b00: 3c00 6407 7c00 6a01 6408 3c00 6409 5300  <.d.|.j.d.<.d.S.
-00004b10: 290a 7a63 4578 7465 726e 616c 2044 6174  ).zcExternal Dat
-00004b20: 6120 5374 6f72 653a 2047 6574 2f73 6574  a Store: Get/set
-00004b30: 2063 6f6e 6669 6775 7261 7469 6f6e 732e   configurations.
-00004b40: 0a0a 2020 2020 5374 616e 6461 7264 2044  ..    Standard D
-00004b50: 6174 6120 5374 6f72 653a 2047 6574 2f73  ata Store: Get/s
-00004b60: 6574 2063 6f6e 6669 6775 7261 7469 6f6e  et configuration
-00004b70: 732e 0a20 2020 2054 46a9 0272 9a00 0000  s..    TF..r....
-00004b80: da0b 6973 5f70 6879 7369 6361 6c72 9900  ..is_physicalr..
-00004b90: 0000 7280 0000 0072 3000 0000 7285 0000  ..r....r0...r...
-00004ba0: 0072 8100 0000 4e72 a300 0000 72a4 0000  .r....Nr....r...
-00004bb0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-00004bc0: 7285 0000 0021 0200 0073 0c00 0000 0808  r....!...s......
-00004bd0: 1201 0e02 0a01 0a01 0e01 7285 0000 0063  ..........r....c
-00004be0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
-00004bf0: 0600 0000 0300 0000 72a7 0000 0029 057a  ........r....).z
-00004c00: 5b45 7874 6572 6e61 6c20 4461 7461 2053  [External Data S
-00004c10: 746f 7265 3a20 5365 7420 636f 6e66 6967  tore: Set config
-00004c20: 7572 6174 696f 6e73 2e0a 0a20 2020 2053  urations...    S
-00004c30: 7461 6e64 6172 6420 4461 7461 2053 746f  tandard Data Sto
-00004c40: 7265 3a20 5365 7420 636f 6e66 6967 7572  re: Set configur
-00004c50: 6174 696f 6e73 2e0a 2020 2020 7230 0000  ations..    r0..
-00004c60: 00da 0a63 6f6e 6669 675f 7365 7463 0100  ...config_setc..
-00004c70: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00004c80: 0000 1300 0000 72a9 0000 0072 1a00 0000  ......r....r....
-00004c90: 72aa 0000 0072 3200 0000 72ab 0000 0072  r....r2...r....r
-00004ca0: 1200 0000 7213 0000 0072 3600 0000 3a02  ....r....r6...:.
-00004cb0: 0000 7237 0000 007a 1c63 6f6e 6669 675f  ..r7...z.config_
-00004cc0: 7365 742e 3c6c 6f63 616c 733e 2e3c 6c61  set.<locals>.<la
-00004cd0: 6d62 6461 3e72 ac00 0000 72ab 0000 0072  mbda>r....r....r
-00004ce0: 1200 0000 72ab 0000 0072 1300 0000 72f5  ....r....r....r.
-00004cf0: 0000 0032 0200 0072 ea00 0000 72f5 0000  ...2...r....r...
-00004d00: 0063 0200 0000 0000 0000 0000 0000 0200  .c..............
-00004d10: 0000 0600 0000 0300 0000 72a7 0000 0029  ..........r....)
-00004d20: 057a 5b45 7874 6572 6e61 6c20 4461 7461  .z[External Data
-00004d30: 2053 746f 7265 3a20 4765 7420 636f 6e66   Store: Get conf
-00004d40: 6967 7572 6174 696f 6e73 2e0a 0a20 2020  igurations...   
-00004d50: 2053 7461 6e64 6172 6420 4461 7461 2053   Standard Data S
-00004d60: 746f 7265 3a20 4765 7420 636f 6e66 6967  tore: Get config
-00004d70: 7572 6174 696f 6e73 2e0a 2020 2020 7230  urations..    r0
-00004d80: 0000 00da 0a63 6f6e 6669 675f 6765 7463  .....config_getc
-00004d90: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00004da0: 0300 0000 1300 0000 72a9 0000 0072 1a00  ........r....r..
-00004db0: 0000 72af 0000 0072 3200 0000 72ab 0000  ..r....r2...r...
-00004dc0: 0072 1200 0000 7213 0000 0072 3600 0000  .r....r....r6...
-00004dd0: 4502 0000 7237 0000 007a 1c63 6f6e 6669  E...r7...z.confi
-00004de0: 675f 6765 742e 3c6c 6f63 616c 733e 2e3c  g_get.<locals>.<
-00004df0: 6c61 6d62 6461 3e72 ac00 0000 72ab 0000  lambda>r....r...
-00004e00: 0072 1200 0000 72ab 0000 0072 1300 0000  .r....r....r....
-00004e10: 72f6 0000 003d 0200 0072 ea00 0000 72f6  r....=...r....r.
-00004e20: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-00004e30: 0200 0000 0600 0000 0300 0000 72a7 0000  ............r...
-00004e40: 0029 057a 2f45 7874 6572 6e61 6c20 4461  .).z/External Da
-00004e50: 7461 2053 746f 7265 3a20 436c 6561 7220  ta Store: Clear 
-00004e60: 636f 6e66 6967 7572 6174 696f 6e73 2e0a  configurations..
-00004e70: 2020 2020 7230 0000 00da 0c63 6f6e 6669      r0.....confi
-00004e80: 675f 636c 6561 7263 0100 0000 0000 0000  g_clearc........
-00004e90: 0000 0000 0100 0000 0300 0000 1300 0000  ................
-00004ea0: 72a9 0000 0072 1a00 0000 72b2 0000 0072  r....r....r....r
-00004eb0: 3200 0000 72ab 0000 0072 1200 0000 7213  2...r....r....r.
-00004ec0: 0000 0072 3600 0000 4e02 0000 7237 0000  ...r6...N...r7..
-00004ed0: 007a 1e63 6f6e 6669 675f 636c 6561 722e  .z.config_clear.
-00004ee0: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-00004ef0: 3e72 ac00 0000 72ab 0000 0072 1200 0000  >r....r....r....
-00004f00: 72ab 0000 0072 1300 0000 72f7 0000 0048  r....r....r....H
-00004f10: 0200 0073 0200 0000 1c06 72f7 0000 007a  ...s......r....z
-00004f20: 022d 6d7a 052d 2d6d 7367 7a0b 6f62 6973  .-mz.--msgz.obis
-00004f30: 2063 6f6d 6d69 747a 2341 206d 6573 7361   commitz#A messa
-00004f40: 6765 2065 7870 6c61 696e 696e 6720 7768  ge explaining wh
-00004f50: 6174 2077 6173 2064 6f6e 652e 7a02 2d61  at was done.z.-a
-00004f60: 7a0a 2d2d 6175 746f 5f61 6464 7a26 4175  z.--auto_addz&Au
-00004f70: 746f 6d61 7469 6361 6c6c 7920 6164 6420  tomatically add 
-00004f80: 616c 6c20 756e 7472 6163 6b65 6420 6669  all untracked fi
-00004f90: 6c65 732e 7a02 2d69 7a17 2d2d 6967 6e6f  les.z.-iz.--igno
-00004fa0: 7265 5f6d 6973 7369 6e67 5f70 6172 656e  re_missing_paren
-00004fb0: 747a 2949 6620 7061 7265 6e74 2064 6174  tz)If parent dat
-00004fc0: 6120 7365 7420 6973 206d 6973 7369 6e67  a set is missing
-00004fd0: 2c20 6967 6e6f 7265 2069 742e 2902 da06  , ignore it.)...
-00004fe0: 6578 6973 7473 da09 6669 6c65 5f6f 6b61  exists..file_oka
-00004ff0: 7929 0272 0d00 0000 da08 7265 7175 6972  y).r......requir
-00005000: 6564 da06 636f 6d6d 6974 7a30 436f 6d6d  ed..commitz0Comm
-00005010: 6974 2074 6865 2072 6570 6f73 6974 6f72  it the repositor
-00005020: 7920 746f 2067 6974 2061 6e64 2069 6e66  y to git and inf
-00005030: 6f72 6d20 6f70 656e 4249 532e 6305 0000  orm openBIS.c...
-00005040: 0000 0000 0000 0000 0005 0000 0006 0000  ................
-00005050: 0003 0000 0073 2000 0000 7c00 6a00 6401  .....s ...|.j.d.
-00005060: 1900 a001 6402 8700 8701 8702 6603 6403  ....d.......f.d.
-00005070: 6404 8408 7c04 a103 5300 2905 fa4a 4578  d...|...S.)..JEx
-00005080: 7465 726e 616c 2044 6174 6120 5374 6f72  ternal Data Stor
-00005090: 653a 2043 6f6d 6d69 7420 7468 6520 7265  e: Commit the re
-000050a0: 706f 7369 746f 7279 2074 6f20 6769 7420  pository to git 
-000050b0: 616e 6420 696e 666f 726d 206f 7065 6e42  and inform openB
-000050c0: 4953 2e0a 2020 2020 7230 0000 0072 fb00  IS..    r0...r..
-000050d0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-000050e0: 0000 0005 0000 0013 0000 00f3 0e00 0000  ................
-000050f0: 7c00 a000 8802 8800 8801 a103 5300 721a  |...........S.r.
-00005100: 0000 0029 0172 fb00 0000 7232 0000 00a9  ...).r....r2....
-00005110: 03da 0861 7574 6f5f 6164 64da 1569 676e  ...auto_add..ign
-00005120: 6f72 655f 6d69 7373 696e 675f 7061 7265  ore_missing_pare
-00005130: 6e74 da03 6d73 6772 1200 0000 7213 0000  nt..msgr....r...
-00005140: 0072 3600 0000 6802 0000 72df 0000 007a  .r6...h...r....z
-00005150: 2372 6570 6f73 6974 6f72 795f 636f 6d6d  #repository_comm
-00005160: 6974 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  it.<locals>.<lam
-00005170: 6264 613e 72ac 0000 00a9 0572 2b00 0000  bda>r......r+...
-00005180: 7201 0100 0072 ff00 0000 7200 0100 0072  r....r....r....r
-00005190: 3900 0000 7212 0000 0072 fe00 0000 7213  9...r....r....r.
-000051a0: 0000 00da 1172 6570 6f73 6974 6f72 795f  .....repository_
-000051b0: 636f 6d6d 6974 6102 0000 7308 0000 000c  commita...s.....
-000051c0: 060e 0102 0104 fe72 0301 0000 6305 0000  .......r....c...
-000051d0: 0000 0000 0000 0000 0005 0000 0007 0000  ................
-000051e0: 0043 0000 0073 2c00 0000 7400 7c00 6a01  .C...s,...t.|.j.
-000051f0: 6401 6402 8d02 7c00 6a01 6403 3c00 7c00  d.d...|.j.d.<.|.
-00005200: 6a02 7403 7c01 7c02 7c03 7c04 6404 8d05  j.t.|.|.|.|.d...
-00005210: 0100 6405 5300 2906 72fc 0000 0046 7299  ..d.S.).r....Fr.
-00005220: 0000 0072 3000 0000 2904 7201 0100 0072  ...r0...).r....r
-00005230: ff00 0000 7200 0100 0072 3900 0000 4e29  ....r....r9...N)
-00005240: 0472 0900 0000 722a 0000 00da 0669 6e76  .r....r*.....inv
-00005250: 6f6b 6572 0301 0000 7202 0100 0072 1200  oker....r....r..
-00005260: 0000 7212 0000 0072 1300 0000 72fb 0000  ..r....r....r...
-00005270: 006c 0200 0073 0800 0000 1406 0a01 0401  .l...s..........
-00005280: 0aff da0f 7265 706f 7369 746f 7279 5f70  ....repository_p
-00005290: 6174 6872 3e00 0000 722f 0000 0029 0172  athr>...r/...).r
-000052a0: 2300 0000 da04 696e 6974 7a2b 496e 6974  #.....initz+Init
-000052b0: 6961 6c69 7a65 2074 6865 2066 6f6c 6465  ialize the folde
-000052c0: 7220 6173 2061 2064 6174 6120 7265 706f  r as a data repo
-000052d0: 7369 746f 7279 2e63 0300 0000 0000 0000  sitory.c........
-000052e0: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
-000052f0: 730c 0000 0074 007c 007c 017c 0283 0353  s....t.|.|.|...S
-00005300: 0029 017a 4545 7874 6572 6e61 6c20 4461  .).zEExternal Da
-00005310: 7461 2053 746f 7265 3a20 496e 6974 6961  ta Store: Initia
-00005320: 6c69 7a65 2074 6865 2066 6f6c 6465 7220  lize the folder 
-00005330: 6173 2061 2064 6174 6120 7265 706f 7369  as a data reposi
-00005340: 746f 7279 2e0a 2020 2020 2901 723a 0000  tory..    ).r:..
-00005350: 0029 0372 2b00 0000 7205 0100 0072 3e00  .).r+...r....r>.
-00005360: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00005370: 00da 0f72 6570 6f73 6974 6f72 795f 696e  ...repository_in
-00005380: 6974 8202 0000 7302 0000 000c 0672 0701  it....s......r..
-00005390: 0000 7a0a 2d2d 7068 7973 6963 616c 72f4  ..z.--physicalr.
-000053a0: 0000 007a 3849 6e69 7469 616c 697a 6520  ...z8Initialize 
-000053b0: 666f 6c64 6572 2066 6f72 2053 7461 6e64  folder for Stand
-000053c0: 6172 6420 4461 7461 2053 746f 7265 2064  ard Data Store d
-000053d0: 6174 6120 6861 6e64 6c69 6e67 2e63 0400  ata handling.c..
-000053e0: 0000 0000 0000 0000 0000 0400 0000 0500  ................
-000053f0: 0000 4300 0000 732a 0000 0074 007c 006a  ..C...s*...t.|.j
-00005400: 0164 017c 0364 028d 037c 006a 0164 033c  .d.|.d...|.j.d.<
-00005410: 007c 006a 0274 037c 017c 0264 048d 0301  .|.j.t.|.|.d....
-00005420: 0064 0553 0029 067a df45 7874 6572 6e61  .d.S.).z.Externa
-00005430: 6c20 4461 7461 2053 746f 7265 3a20 496e  l Data Store: In
-00005440: 6974 6961 6c69 7a65 2074 6865 2066 6f6c  itialize the fol
-00005450: 6465 7220 6173 2061 2064 6174 6120 7265  der as a data re
-00005460: 706f 7369 746f 7279 2066 6f72 2045 7874  pository for Ext
-00005470: 6572 6e61 6c20 4461 7461 2053 746f 7265  ernal Data Store
-00005480: 0a20 2020 2064 6174 6120 6861 6e64 6c69  .    data handli
-00005490: 6e67 2e0a 0a20 2020 2053 7461 6e64 6172  ng...    Standar
-000054a0: 6420 4461 7461 2053 746f 7265 3a20 496e  d Data Store: In
-000054b0: 6974 6961 6c69 7a65 2074 6865 2066 6f6c  itialize the fol
-000054c0: 6465 7220 6173 2061 2064 6174 6120 7265  der as a data re
-000054d0: 706f 7369 746f 7279 2066 6f72 2053 7461  pository for Sta
-000054e0: 6e64 6172 6420 4461 7461 2053 746f 7265  ndard Data Store
-000054f0: 0a20 2020 2064 6174 6120 6861 6e64 6c69  .    data handli
-00005500: 6e67 2e0a 2020 2020 4672 f300 0000 7230  ng..    Fr....r0
-00005510: 0000 0029 0272 0501 0000 723e 0000 004e  ...).r....r>...N
-00005520: 2904 7209 0000 0072 2a00 0000 7204 0100  ).r....r*...r...
-00005530: 0072 0701 0000 2904 722b 0000 0072 0501  .r....).r+...r..
-00005540: 0000 723e 0000 0072 f400 0000 7212 0000  ..r>...r....r...
-00005550: 0072 1200 0000 7213 0000 0072 0601 0000  .r....r....r....
-00005560: 9102 0000 7304 0000 0016 0a14 017a 082d  ....s........z.-
-00005570: 2d70 6172 656e 7429 0172 0d00 0000 723c  -parent).r....r<
-00005580: 0000 007a 2c49 6e69 7469 616c 697a 6520  ...z,Initialize 
-00005590: 7468 6520 666f 6c64 6572 2061 7320 616e  the folder as an
-000055a0: 2061 6e61 6c79 7369 7320 666f 6c64 6572   analysis folder
-000055b0: 2e63 0400 0000 0000 0000 0000 0000 0400  .c..............
-000055c0: 0000 0500 0000 4300 0000 730e 0000 0074  ......C...s....t
-000055d0: 007c 007c 017c 027c 0383 0453 0029 01fa  .|.|.|.|...S.)..
-000055e0: 4145 7874 6572 6e61 6c20 4461 7461 2053  AExternal Data S
-000055f0: 746f 7265 3a20 496e 6974 6961 6c69 7a65  tore: Initialize
-00005600: 2074 6865 2066 6f6c 6465 7220 6173 2061   the folder as a
-00005610: 6e20 616e 616c 7973 6973 2066 6f6c 6465  n analysis folde
-00005620: 722e 2901 7249 0000 00a9 0472 2b00 0000  r.).rI.....r+...
-00005630: 723f 0000 0072 0501 0000 723e 0000 0072  r?...r....r>...r
-00005640: 1200 0000 7212 0000 0072 1300 0000 da18  ....r....r......
-00005650: 7265 706f 7369 746f 7279 5f69 6e69 745f  repository_init_
-00005660: 616e 616c 7973 6973 a902 0000 7297 0000  analysis....r...
-00005670: 0072 0a01 0000 2902 7263 0000 0072 cd00  .r....).rc...r..
-00005680: 0000 6304 0000 0000 0000 0000 0000 0004  ..c.............
-00005690: 0000 0006 0000 0043 0000 0073 2a00 0000  .......C...s*...
-000056a0: 7400 7c00 6a01 6401 6402 8d02 7c00 6a01  t.|.j.d.d...|.j.
-000056b0: 6403 3c00 7c00 6a02 7403 7c01 7c02 7c03  d.<.|.j.t.|.|.|.
-000056c0: 6404 8d04 0100 6405 5300 2906 7208 0100  d.....d.S.).r...
-000056d0: 0046 7299 0000 0072 3000 0000 2903 723f  .Fr....r0...).r?
-000056e0: 0000 0072 0501 0000 723e 0000 004e 2904  ...r....r>...N).
-000056f0: 7209 0000 0072 2a00 0000 7204 0100 0072  r....r*...r....r
-00005700: 0a01 0000 7209 0100 0072 1200 0000 7212  ....r....r....r.
-00005710: 0000 0072 1300 0000 723c 0000 00b1 0200  ...r....r<......
-00005720: 0073 0800 0000 1405 0801 0401 0aff da06  .s..............
-00005730: 7374 6174 7573 7a26 5368 6f77 2074 6865  statusz&Show the
-00005740: 2073 7461 7465 206f 6620 7468 6520 6f62   state of the ob
-00005750: 6973 2072 6570 6f73 6974 6f72 792e 6302  is repository.c.
-00005760: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-00005770: 0000 0043 0000 00f3 1800 0000 7c00 6a00  ...C........|.j.
-00005780: 6401 1900 a001 6402 6403 6404 8400 7c01  d.....d.d.d...|.
-00005790: a103 5300 2905 fa3b 4578 7465 726e 616c  ..S.)..;External
-000057a0: 2044 6174 6120 5374 6f72 653a 2053 686f   Data Store: Sho
-000057b0: 7720 7468 6520 7374 6174 6520 6f66 2074  w the state of t
-000057c0: 6865 206f 6269 7320 7265 706f 7369 746f  he obis reposito
-000057d0: 7279 2e72 3000 0000 da11 7265 706f 7369  ry.r0.....reposi
-000057e0: 746f 7279 5f73 7461 7475 7363 0100 0000  tory_statusc....
-000057f0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00005800: 5300 0000 f308 0000 007c 00a0 00a1 0053  S........|.....S
-00005810: 0072 1a00 0000 2901 720b 0100 0072 3200  .r....).r....r2.
-00005820: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00005830: 0072 3600 0000 c902 0000 f302 0000 0008  .r6.............
-00005840: 007a 2372 6570 6f73 6974 6f72 795f 7374  .z#repository_st
-00005850: 6174 7573 2e3c 6c6f 6361 6c73 3e2e 3c6c  atus.<locals>.<l
-00005860: 616d 6264 613e 72ac 0000 00a9 0272 2b00  ambda>r......r+.
-00005870: 0000 7239 0000 0072 1200 0000 7212 0000  ..r9...r....r...
-00005880: 0072 1300 0000 720e 0100 00c4 0200 00f3  .r....r.........
-00005890: 0200 0000 1805 720e 0100 0063 0200 0000  ......r....c....
-000058a0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-000058b0: 4300 0000 f326 0000 0074 007c 006a 0164  C....&...t.|.j.d
-000058c0: 0164 028d 027c 006a 0164 033c 007c 006a  .d...|.j.d.<.|.j
-000058d0: 0274 037c 0164 048d 0201 0064 0553 0029  .t.|.d.....d.S.)
-000058e0: 0672 0d01 0000 4672 9900 0000 7230 0000  .r....Fr....r0..
-000058f0: 00a9 0172 3900 0000 4e29 0472 0900 0000  ...r9...N).r....
-00005900: 722a 0000 0072 0401 0000 720e 0100 0072  r*...r....r....r
-00005910: 1101 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00005920: 0000 0072 0b01 0000 cc02 0000 f304 0000  ...r............
-00005930: 0014 0512 0163 0200 0000 0000 0000 0000  .....c..........
-00005940: 0000 0200 0000 0200 0000 4300 0000 730e  ..........C...s.
-00005950: 0000 007c 017c 005f 007c 00a0 01a1 0053  ...|.|._.|.....S
-00005960: 0072 1a00 0000 2902 7200 0100 00da 0473  .r....).r......s
-00005970: 796e 6329 0272 3300 0000 7200 0100 0072  ync).r3...r....r
-00005980: 1200 0000 7212 0000 0072 1300 0000 da10  ....r....r......
-00005990: 5f72 6570 6f73 6974 6f72 795f 7379 6e63  _repository_sync
-000059a0: e002 0000 7304 0000 0006 0108 0172 1701  ....s........r..
-000059b0: 0000 7216 0100 007a 2153 796e 6320 7468  ..r....z!Sync th
-000059c0: 6520 7265 706f 7369 746f 7279 2077 6974  e repository wit
-000059d0: 6820 6f70 656e 4249 532e 6303 0000 0000  h openBIS.c.....
-000059e0: 0000 0000 0000 0003 0000 0006 0000 0003  ................
-000059f0: 0000 0073 1c00 0000 7c00 6a00 6401 1900  ...s....|.j.d...
-00005a00: a001 6402 8700 6601 6403 6404 8408 7c02  ..d...f.d.d...|.
-00005a10: a103 5300 2905 fa36 4578 7465 726e 616c  ..S.)..6External
-00005a20: 2044 6174 6120 5374 6f72 653a 2053 796e   Data Store: Syn
-00005a30: 6320 7468 6520 7265 706f 7369 746f 7279  c the repository
-00005a40: 2077 6974 6820 6f70 656e 4249 532e 7230   with openBIS.r0
-00005a50: 0000 0072 1601 0000 6301 0000 0000 0000  ...r....c.......
-00005a60: 0000 0000 0001 0000 0003 0000 0013 0000  ................
-00005a70: 0073 0a00 0000 7400 7c00 8800 8302 5300  .s....t.|.....S.
-00005a80: 721a 0000 0029 0172 1701 0000 7232 0000  r....).r....r2..
-00005a90: 00a9 0172 0001 0000 7212 0000 0072 1300  ...r....r....r..
-00005aa0: 0000 7236 0000 00ea 0200 0072 3700 0000  ..r6.......r7...
-00005ab0: 7a21 7265 706f 7369 746f 7279 5f73 796e  z!repository_syn
-00005ac0: 632e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  c.<locals>.<lamb
-00005ad0: 6461 3e72 ac00 0000 a903 722b 0000 0072  da>r......r+...r
-00005ae0: 0001 0000 7239 0000 0072 1200 0000 7219  ....r9...r....r.
-00005af0: 0100 0072 1300 0000 da0f 7265 706f 7369  ...r......reposi
-00005b00: 746f 7279 5f73 796e 63e5 0200 0073 0600  tory_sync....s..
-00005b10: 0000 1605 0201 04ff 721b 0100 0063 0300  ........r....c..
-00005b20: 0000 0000 0000 0000 0000 0300 0000 0500  ................
-00005b30: 0000 4300 0000 f328 0000 0074 007c 006a  ..C....(...t.|.j
-00005b40: 0164 0164 028d 027c 006a 0164 033c 007c  .d.d...|.j.d.<.|
-00005b50: 006a 0274 037c 017c 0264 048d 0301 0064  .j.t.|.|.d.....d
-00005b60: 0553 0029 0672 1801 0000 4672 9900 0000  .S.).r....Fr....
-00005b70: 7230 0000 0029 0272 0001 0000 7239 0000  r0...).r....r9..
-00005b80: 004e 2904 7209 0000 0072 2a00 0000 7204  .N).r....r*...r.
-00005b90: 0100 0072 1b01 0000 721a 0100 0072 1200  ...r....r....r..
-00005ba0: 0000 7212 0000 0072 1300 0000 7216 0100  ..r....r....r...
-00005bb0: 00ee 0200 0073 0800 0000 1405 0601 0401  .....s..........
-00005bc0: 0aff 7a1b 6372 6561 7465 2f73 686f 7720  ..z.create/show 
-00005bd0: 6120 6f70 656e 4249 5320 746f 6b65 6e63  a openBIS tokenc
-00005be0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00005bf0: 0100 0000 4300 0000 7304 0000 0064 0053  ....C...s....d.S
-00005c00: 0072 1a00 0000 7212 0000 0029 0172 2b00  .r....r....).r+.
-00005c10: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-00005c20: 00da 0574 6f6b 656e f802 0000 7302 0000  ...token....s...
-00005c30: 0004 0372 1d01 0000 7a36 4765 7420 6578  ...r....z6Get ex
-00005c40: 6973 7469 6e67 2070 6572 736f 6e61 6c20  isting personal 
-00005c50: 6163 6365 7373 2074 6f6b 656e 206f 7220  access token or 
-00005c60: 6372 6561 7465 2061 206e 6577 206f 6e65  create a new one
-00005c70: 7a0c 7365 7373 696f 6e2d 6e61 6d65 2901  z.session-name).
-00005c80: 72fa 0000 007a 0f2d 2d76 616c 6964 6974  r....z.--validit
-00005c90: 792d 6461 7973 7a21 4e75 6d62 6572 206f  y-daysz!Number o
-00005ca0: 6620 6461 7973 2074 6865 2074 6f6b 656e  f days the token
-00005cb0: 2069 7320 7661 6c69 6429 0172 2500 0000   is valid).r%...
-00005cc0: 7a10 2d2d 7661 6c69 6469 7479 2d77 6565  z.--validity-wee
-00005cd0: 6b73 7a22 4e75 6d62 6572 206f 6620 7765  ksz"Number of we
-00005ce0: 656b 7320 7468 6520 746f 6b65 6e20 6973  eks the token is
-00005cf0: 2076 616c 6964 7a11 2d2d 7661 6c69 6469   validz.--validi
-00005d00: 7479 2d6d 6f6e 7468 737a 234e 756d 6265  ty-monthsz#Numbe
-00005d10: 7220 6f66 206d 6f6e 7468 7320 7468 6520  r of months the 
-00005d20: 746f 6b65 6e20 6973 2076 616c 6964 6302  token is validc.
-00005d30: 0000 0000 0000 0000 0000 000e 0000 000a  ................
-00005d40: 0000 000b 0000 0073 e801 0000 7400 8800  .......s....t...
-00005d50: 6a01 6401 6402 8d02 7d03 7c03 a002 a100  j.d.d...}.|.....
-00005d60: 8901 7c01 7313 8801 6403 1900 6404 1900  ..|.s...d...d...
-00005d70: 7d01 7c01 721f 7403 a004 6405 7c01 9b00  }.|.r.t...d.|...
-00005d80: 6406 9d03 a101 0100 6e05 7403 a005 6407  d.......n.t...d.
-00005d90: a101 7d01 8801 6403 1900 6408 1900 7d04  ..}...d...d...}.
-00005da0: 7c04 7331 7403 a005 6409 a101 7d04 8801  |.s1t...d...}...
-00005db0: 6403 1900 640a 1900 7d05 7c05 7341 7403  d...d...}.|.sAt.
-00005dc0: a005 640b 7c04 9b00 9d02 a101 7d05 7403  ..d.|.......}.t.
-00005dd0: 6a05 640c 7c05 9b00 640d 7c04 9b00 9d04  j.d.|...d.|.....
-00005de0: 640e 640f 8d02 7d06 7406 7c04 8801 6403  d.d...}.t.|...d.
-00005df0: 1900 a007 6410 640e a102 6411 8d02 7d07  ....d.d...d...}.
-00005e00: 7a08 7c07 a008 7c05 7c06 a102 0100 5700  z.|...|.|.....W.
-00005e10: 6e16 0400 7409 740a 6602 7978 0100 7d08  n...t.t.f.yx..}.
-00005e20: 0100 7a08 7403 a00b 6412 7c08 9b00 9d02  ..z.t...d.|.....
-00005e30: a101 8201 6400 7d08 7e08 7701 7700 740c  ....d.}.~.w.w.t.
-00005e40: a00d a100 7d09 7c02 a007 6413 a101 728f  ....}.|...d...r.
-00005e50: 7c09 740e 740f 7c02 a007 6413 a101 8301  |.t.t.|...d.....
-00005e60: 6414 8d01 1700 7d0a 6e32 7c02 a007 6415  d.....}.n2|...d.
-00005e70: a101 72a1 7c09 740e 740f 7c02 a007 6415  ..r.|.t.t.|...d.
-00005e80: a101 8301 6416 8d01 1700 7d0a 6e20 7c02  ....d.....}.n |.
-00005e90: a007 6417 a101 72b3 7c09 740e 740f 7c02  ..d...r.|.t.t.|.
-00005ea0: a007 6417 a101 8301 6418 8d01 1700 7d0a  ..d.....d.....}.
-00005eb0: 6e0e 7c07 a010 a100 7d0b 7c0b 6a11 7d0c  n.|.....}.|.j.}.
-00005ec0: 7c09 740e 7c0c 6419 8d01 1700 7d0a 7c07  |.t.|.d.....}.|.
-00005ed0: 6a12 7c01 7c09 7c0a 641a 8d03 7d0d 640a  j.|.|.|.d...}.d.
-00005ee0: 7c05 6901 6408 7c04 6901 641b 7c0d 6a13  |.i.d.|.i.d.|.j.
-00005ef0: 6901 6404 7c01 6901 6604 8901 6401 8800  i.d.|.i.f...d...
-00005f00: 6a01 641c 3c00 7c03 8800 6a01 641d 3c00  j.d.<.|...j.d.<.
-00005f10: 6403 8800 6a01 641e 3c00 7c03 a014 641f  d...j.d.<.|...d.
-00005f20: 8700 8701 6602 6420 6421 8408 a102 0100  ....f.d d!......
-00005f30: 6400 5300 2922 4e46 7299 0000 0072 8500  d.S.)"NFr....r..
-00005f40: 0000 da0c 7365 7373 696f 6e5f 6e61 6d65  ....session_name
-00005f50: 7528 0000 0047 6574 2070 6572 736f 6e61  u(...Get persona
-00005f60: 6c20 6163 6365 7373 2074 6f6b 656e 2066  l access token f
-00005f70: 6f72 2073 6573 7369 6f6e 20c2 abf5 0200  or session .....
-00005f80: 0000 c2bb 7a1b 506c 6561 7365 2065 6e74  ....z.Please ent
-00005f90: 6572 2061 2073 6573 7369 6f6e 206e 616d  er a session nam
-00005fa0: 65da 0b6f 7065 6e62 6973 5f75 726c 7a1c  e..openbis_urlz.
-00005fb0: 506c 6561 7365 2065 6e74 6572 2074 6865  Please enter the
-00005fc0: 206f 7065 6e42 4953 2055 524c da04 7573   openBIS URL..us
-00005fd0: 6572 7a1a 506c 6561 7365 2065 6e74 6572  erz.Please enter
-00005fe0: 2075 7365 726e 616d 6520 666f 7220 7a0d   username for z.
-00005ff0: 5061 7373 776f 7264 2066 6f72 20fa 0140  Password for ..@
-00006000: 5429 01da 0a68 6964 655f 696e 7075 7472  T)...hide_inputr
-00006010: 2700 0000 2901 7227 0000 007a 1b43 616e  '...).r'...z.Can
-00006020: 6e6f 7420 636f 6e6e 6563 7420 746f 206f  not connect to o
-00006030: 7065 6e42 4953 3a20 da0f 7661 6c69 6469  penBIS: ..validi
-00006040: 7479 5f6d 6f6e 7468 7329 01da 066d 6f6e  ty_months)...mon
-00006050: 7468 73da 0e76 616c 6964 6974 795f 7765  ths..validity_we
-00006060: 656b 7329 01da 0577 6565 6b73 da0d 7661  eks)...weeks..va
-00006070: 6c69 6469 7479 5f64 6179 7329 01da 0464  lidity_days)...d
-00006080: 6179 7329 01da 0773 6563 6f6e 6473 2903  ays)...seconds).
-00006090: da0b 7365 7373 696f 6e4e 616d 65da 0976  ..sessionName..v
-000060a0: 616c 6964 4672 6f6d da07 7661 6c69 6454  alidFrom..validT
-000060b0: 6fda 0d6f 7065 6e62 6973 5f74 6f6b 656e  o..openbis_token
-000060c0: 7280 0000 0072 3000 0000 7281 0000 0072  r....r0...r....r
-000060d0: f500 0000 6301 0000 0000 0000 0000 0000  ....c...........
-000060e0: 0001 0000 0003 0000 0013 0000 0072 a900  .............r..
-000060f0: 0000 721a 0000 0072 aa00 0000 7232 0000  ..r....r....r2..
-00006100: 0072 ab00 0000 7212 0000 0072 1300 0000  .r....r....r....
-00006110: 7236 0000 0038 0300 0072 3700 0000 7a1b  r6...8...r7...z.
-00006120: 6e65 775f 746f 6b65 6e2e 3c6c 6f63 616c  new_token.<local
-00006130: 733e 2e3c 6c61 6d62 6461 3e29 1572 0900  s>.<lambda>).r..
-00006140: 0000 722a 0000 0072 9e00 0000 7216 0000  ..r*...r....r...
-00006150: 0072 1700 0000 da06 7072 6f6d 7074 7205  .r......promptr.
-00006160: 0000 0072 9800 0000 da05 6c6f 6769 6e72  ...r......loginr
-00006170: 0400 0000 da0a 5661 6c75 6545 7272 6f72  ......ValueError
-00006180: da0e 436c 6963 6b45 7863 6570 7469 6f6e  ..ClickException
-00006190: 7202 0000 00da 036e 6f77 7203 0000 00da  r......nowr.....
-000061a0: 0369 6e74 da16 6765 745f 7365 7276 6572  .int..get_server
-000061b0: 5f69 6e66 6f72 6d61 7469 6f6e da2a 7065  _information.*pe
-000061c0: 7273 6f6e 616c 5f61 6363 6573 735f 746f  rsonal_access_to
-000061d0: 6b65 6e73 5f6d 6178 5f76 616c 6964 6974  kens_max_validit
-000061e0: 795f 7065 7269 6f64 da23 6765 745f 6f72  y_period.#get_or
-000061f0: 5f63 7265 6174 655f 7065 7273 6f6e 616c  _create_personal
-00006200: 5f61 6363 6573 735f 746f 6b65 6eda 0670  _access_token..p
-00006210: 6572 6d49 6472 3800 0000 290e 722b 0000  ermIdr8...).r+..
-00006220: 0072 1e01 0000 da06 6b77 6172 6773 7230  .r......kwargsr0
-00006230: 0000 00da 0375 726c da08 7573 6572 6e61  .....url..userna
-00006240: 6d65 da08 7061 7373 776f 7264 da01 6fda  me..password..o.
-00006250: 0365 7863 722c 0100 0072 2d01 0000 da0a  .excr,...r-.....
-00006260: 7365 7276 6572 696e 666f 722a 0100 00da  serverinfor*....
-00006270: 0974 6f6b 656e 5f6f 626a 7212 0000 0072  .token_objr....r
-00006280: ab00 0000 7213 0000 00da 096e 6577 5f74  ....r......new_t
-00006290: 6f6b 656e fe02 0000 7366 0000 000e 0708  oken....sf......
-000062a0: 0104 020c 0104 0114 010a 020c 0204 010a  ................
-000062b0: 010c 0204 0110 011a 010c 0104 0108 ff02  ................
-000062c0: 0210 0112 0110 0108 8002 ff08 030a 0102  ................
-000062d0: 0112 0106 ff0a 0202 0112 0106 ff0a 0202  ................
-000062e0: 0112 0106 ff08 0306 010e 0104 0106 0106  ................
-000062f0: ff06 0306 0108 0106 0104 fc0a 070a 010a  ................
-00006300: 011a 0172 4101 0000 da06 6164 6472 6566  ...rA.....addref
-00006310: 7a33 4164 6420 7468 6520 6769 7665 6e20  z3Add the given 
-00006320: 7265 706f 7369 746f 7279 2061 7320 6120  repository as a 
-00006330: 7265 6665 7265 6e63 6520 746f 206f 7065  reference to ope
-00006340: 6e42 4953 2e63 0200 0000 0000 0000 0000  nBIS.c..........
-00006350: 0000 0200 0000 0500 0000 4300 0000 720c  ..........C...r.
-00006360: 0100 0029 05fa 2255 7365 6420 666f 7220  ...).."Used for 
-00006370: 4578 7465 726e 616c 2044 6174 6120 5374  External Data St
-00006380: 6f72 6520 6f6e 6c79 2e72 3000 0000 7242  ore only.r0...rB
-00006390: 0100 0063 0100 0000 0000 0000 0000 0000  ...c............
-000063a0: 0100 0000 0200 0000 5300 0000 720f 0100  ........S...r...
-000063b0: 0072 1a00 0000 2901 7242 0100 0072 3200  .r....).rB...r2.
-000063c0: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
-000063d0: 0072 3600 0000 4603 0000 7210 0100 007a  .r6...F...r....z
-000063e0: 2372 6570 6f73 6974 6f72 795f 6164 6472  #repository_addr
-000063f0: 6566 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  ef.<locals>.<lam
-00006400: 6264 613e 72ac 0000 0072 1101 0000 7212  bda>r....r....r.
-00006410: 0000 0072 1200 0000 7213 0000 00da 1172  ...r....r......r
-00006420: 6570 6f73 6974 6f72 795f 6164 6472 6566  epository_addref
-00006430: 4103 0000 7212 0100 0072 4401 0000 6302  A...r....rD...c.
-00006440: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00006450: 0000 0043 0000 0072 1301 0000 2906 7243  ...C...r....).rC
-00006460: 0100 0046 7299 0000 0072 3000 0000 7214  ...Fr....r0...r.
-00006470: 0100 004e 2904 7209 0000 0072 2a00 0000  ...N).r....r*...
-00006480: 7204 0100 0072 4401 0000 7211 0100 0072  r....rD...r....r
-00006490: 1200 0000 7212 0000 0072 1300 0000 7242  ....r....r....rB
-000064a0: 0100 0049 0300 0072 1501 0000 7a0d 2d2d  ...I...r....z.--
-000064b0: 6461 7461 5f73 6574 5f69 647a 4b52 656d  data_set_idzKRem
-000064c0: 6f76 6520 7265 6620 6279 2064 6174 6120  ove ref by data 
-000064d0: 7365 7420 6964 2c20 696e 2063 6173 6520  set id, in case 
-000064e0: 7468 6520 7265 706f 7369 746f 7279 2069  the repository i
-000064f0: 7320 6e6f 7420 6176 6169 6c61 626c 6520  s not available 
-00006500: 616e 796d 6f72 652e da09 7265 6d6f 7665  anymore...remove
-00006510: 7265 667a 3a52 656d 6f76 6520 7468 6520  refz:Remove the 
-00006520: 7265 6665 7265 6e63 6520 746f 2074 6865  reference to the
-00006530: 2067 6976 656e 2072 6570 6f73 6974 6f72   given repositor
-00006540: 7920 6672 6f6d 206f 7065 6e42 4953 2e63  y from openBIS.c
-00006550: 0300 0000 0000 0000 0000 0000 0300 0000  ................
-00006560: 0600 0000 0300 0000 7338 0000 0088 0064  ........s8.....d
-00006570: 0175 0172 0e7c 0264 0175 0172 0e74 0064  .u.r.|.d.u.r.t.d
-00006580: 0283 0101 0064 0353 007c 006a 0164 0419  .....d.S.|.j.d..
-00006590: 00a0 0264 0587 0066 0164 0664 0784 087c  ...d...f.d.d...|
-000065a0: 02a1 0353 0029 0872 4301 0000 4e7a 2f4f  ...S.).rC...Nz/O
-000065b0: 6e6c 7920 7072 6f76 6964 6520 7468 6520  nly provide the 
-000065c0: 6461 7461 5f73 6574 2069 6420 4f52 2074  data_set id OR t
-000065d0: 6865 2072 6570 6f73 6974 6f72 792e 723b  he repository.r;
-000065e0: 0000 0072 3000 0000 7245 0100 0063 0100  ...r0...rE...c..
-000065f0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00006600: 0000 1300 0000 730c 0000 007c 006a 0088  ......s....|.j..
-00006610: 0064 018d 0153 0029 024e a901 da0b 6461  .d...S.).N....da
-00006620: 7461 5f73 6574 5f69 6429 0172 4501 0000  ta_set_id).rE...
-00006630: 7232 0000 0072 4601 0000 7212 0000 0072  r2...rF...r....r
-00006640: 1300 0000 7236 0000 0066 0300 0072 4000  ....r6...f...r@.
-00006650: 0000 7a26 7265 706f 7369 746f 7279 5f72  ..z&repository_r
-00006660: 656d 6f76 6572 6566 2e3c 6c6f 6361 6c73  emoveref.<locals
-00006670: 3e2e 3c6c 616d 6264 613e 2903 7208 0000  >.<lambda>).r...
-00006680: 0072 2a00 0000 7238 0000 00a9 0372 2b00  .r*...r8.....r+.
-00006690: 0000 7247 0100 0072 3900 0000 7212 0000  ..rG...r9...r...
-000066a0: 0072 4601 0000 7213 0000 00da 1472 6570  .rF...r......rep
-000066b0: 6f73 6974 6f72 795f 7265 6d6f 7665 7265  ository_removere
-000066c0: 665d 0300 0073 0c00 0000 1006 0801 0401  f]...s..........
-000066d0: 1601 0201 04ff 7249 0100 0063 0300 0000  ......rI...c....
-000066e0: 0000 0000 0000 0000 0300 0000 0500 0000  ................
-000066f0: 4300 0000 721c 0100 0029 0672 4301 0000  C...r....).rC...
-00006700: 4672 9900 0000 7230 0000 0029 0272 4701  Fr....r0...).rG.
-00006710: 0000 7239 0000 004e 2904 7209 0000 0072  ..r9...N).r....r
-00006720: 2a00 0000 7204 0100 0072 4901 0000 7248  *...r....rI...rH
-00006730: 0100 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-00006740: 0000 7245 0100 006a 0300 0073 0800 0000  ..rE...j...s....
-00006750: 1405 0801 0201 0aff 7247 0100 007a 0a2d  ........rG...z.-
-00006760: 6672 6f6d 2d66 696c 657a 0b2d 2d66 726f  from-filez.--fro
-00006770: 6d2d 6669 6c65 da09 6672 6f6d 5f66 696c  m-file..from_fil
-00006780: 657a 6a41 6e20 6f75 7470 7574 202e 4353  ezjAn output .CS
-00006790: 5620 6669 6c65 2066 726f 6d20 606f 6269  V file from `obi
-000067a0: 7320 6461 7461 5f73 6574 2073 6561 7263  s data_set searc
-000067b0: 6860 2063 6f6d 6d61 6e64 2077 6974 6820  h` command with 
-000067c0: 7468 6520 6c69 7374 206f 6620 6f62 6a65  the list of obje
-000067d0: 6374 7320 746f 2064 6f77 6e6c 6f61 6420  cts to download 
-000067e0: 6461 7461 7365 7473 2066 726f 6d7a 022d  datasets fromz.-
-000067f0: 667a 062d 2d66 696c 65da 0466 696c 657a  fz.--file..filez
-00006800: 4046 696c 6520 696e 2074 6865 2064 6174  @File in the dat
-00006810: 6120 7365 7420 746f 2064 6f77 6e6c 6f61  a set to downloa
-00006820: 6420 2d20 646f 776e 6c6f 6164 696e 6720  d - downloading 
-00006830: 616c 6c20 6966 206e 6f74 2067 6976 656e  all if not given
-00006840: 2e7a 162d 2d73 6b69 705f 696e 7465 6772  .z.--skip_integr
-00006850: 6974 795f 6368 6563 6b7a 3046 6c61 6720  ity_checkz0Flag 
-00006860: 746f 2073 6b69 7020 6669 6c65 2069 6e74  to skip file int
-00006870: 6567 7269 7479 2063 6865 636b 2077 6974  egrity check wit
-00006880: 6820 6368 6563 6b73 756d 73da 0864 6f77  h checksums..dow
-00006890: 6e6c 6f61 647a 1d44 6f77 6e6c 6f61 6420  nloadz.Download 
-000068a0: 6669 6c65 7320 6f66 2061 2064 6174 6120  files of a data 
-000068b0: 7365 742e 6305 0000 0000 0000 0000 0000  set.c...........
-000068c0: 0005 0000 0007 0000 0003 0000 0073 6000  .............s`.
-000068d0: 0000 8800 6401 7500 7208 8802 6401 7500  ....d.u.r...d.u.
-000068e0: 7310 8800 6401 7501 7216 8802 6401 7501  s...d.u.r...d.u.
-000068f0: 7216 7400 6402 8301 0100 6403 5300 7401  r.t.d.....d.S.t.
-00006900: 7c00 6a02 6404 6405 8d02 7c00 6a02 6406  |.j.d.d...|.j.d.
-00006910: 3c00 7c00 6a02 6406 1900 a003 6407 8700  <.|.j.d.....d...
-00006920: 8701 8702 8703 6604 6408 6409 8408 a102  ......f.d.d.....
-00006930: 5300 290a 7a76 2044 6f77 6e6c 6f61 6473  S.).zv Downloads
-00006940: 2064 6174 6173 6574 2066 696c 6573 2066   dataset files f
-00006950: 726f 6d20 4f70 656e 4249 5320 696e 7374  rom OpenBIS inst
-00006960: 616e 6365 2e0a 0a20 2020 2044 4154 415f  ance...    DATA_
-00006970: 5345 5420 2020 2055 6e69 7175 6520 6964  SET    Unique id
-00006980: 656e 7469 6669 6572 206f 6620 6461 7461  entifier of data
-00006990: 7365 7420 7769 7468 696e 204f 7065 6e42  set within OpenB
-000069a0: 4953 2069 6e73 7461 6e63 652e 4e7a 2e27  IS instance.Nz.'
-000069b0: 6461 7461 5f73 6574 5f69 6427 206f 7220  data_set_id' or 
-000069c0: 2766 726f 6d5f 6669 6c65 2720 6d75 7374  'from_file' must
-000069d0: 2062 6520 7072 6f76 6964 6564 2172 3b00   be provided!r;.
-000069e0: 0000 4672 9900 0000 7230 0000 0072 4c01  ..Fr....r0...rL.
-000069f0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00006a00: 0000 0006 0000 0013 0000 0073 1200 0000  ...........s....
-00006a10: 7c00 6a00 8800 8802 8801 8803 6401 8d04  |.j.........d...
-00006a20: 5300 2902 4e29 0472 4701 0000 724a 0100  S.).N).rG...rJ..
-00006a30: 0072 4b01 0000 da14 736b 6970 5f69 6e74  .rK.....skip_int
-00006a40: 6567 7269 7479 5f63 6865 636b 2901 724c  egrity_check).rL
-00006a50: 0100 0072 3200 0000 a904 7247 0100 0072  ...r2.....rG...r
-00006a60: 4b01 0000 724a 0100 0072 4d01 0000 7212  K...rJ...rM...r.
-00006a70: 0000 0072 1300 0000 7236 0000 0091 0300  ...r....r6......
-00006a80: 0073 0800 0000 0600 0401 0201 06fe 7a1a  .s............z.
-00006a90: 646f 776e 6c6f 6164 2e3c 6c6f 6361 6c73  download.<locals
-00006aa0: 3e2e 3c6c 616d 6264 613e 2904 7208 0000  >.<lambda>).r...
-00006ab0: 0072 0900 0000 722a 0000 0072 3800 0000  .r....r*...r8...
-00006ac0: 2905 722b 0000 0072 4701 0000 724a 0100  ).r+...rG...rJ..
-00006ad0: 0072 4b01 0000 724d 0100 0072 1200 0000  .rK...rM...r....
-00006ae0: 724e 0100 0072 1300 0000 724c 0100 0085  rN...r....rL....
-00006af0: 0300 0073 1600 0000 1006 0601 02ff 0601  ...s............
-00006b00: 02ff 0802 0401 1401 0c01 1001 04ff da05  ................
-00006b10: 6669 6c65 737a 1c66 696c 6520 6f72 2064  filesz.file or d
-00006b20: 6972 6563 746f 7279 2074 6f20 7570 6c6f  irectory to uplo
-00006b30: 6164 2e29 0372 2500 0000 72fa 0000 00da  ad.).r%...r.....
-00006b40: 086d 756c 7469 706c 65da 0973 616d 706c  .multiple..sampl
-00006b50: 655f 6964 da0d 6461 7461 5f73 6574 5f74  e_id..data_set_t
-00006b60: 7970 65da 0675 706c 6f61 647a 2055 706c  ype..uploadz Upl
-00006b70: 6f61 6420 6669 6c65 7320 746f 2066 6f72  oad files to for
-00006b80: 6d20 6120 6461 7461 2073 6574 2e63 0400  m a data set.c..
-00006b90: 0000 0000 0000 0000 0000 0400 0000 0600  ................
-00006ba0: 0000 0300 0000 7336 0000 0074 007c 006a  ......s6...t.|.j
-00006bb0: 0164 0164 028d 027c 006a 0164 033c 007c  .d.d...|.j.d.<.|
-00006bc0: 006a 0164 0319 00a0 0264 0487 0087 0187  .j.d.....d......
-00006bd0: 0266 0364 0564 0684 08a1 0201 0064 0753  .f.d.d.......d.S
-00006be0: 0029 087a aa20 4372 6561 7465 7320 6461  .).z. Creates da
-00006bf0: 7461 2073 6574 2075 6e64 6572 206f 626a  ta set under obj
-00006c00: 6563 7420 616e 6420 7570 6c6f 6164 2066  ect and upload f
-00006c10: 696c 6573 2074 6f20 6974 2e0a 0a20 2020  iles to it...   
-00006c20: 2053 414d 504c 455f 4944 2020 2020 2020   SAMPLE_ID      
-00006c30: 2055 6e69 7175 6520 6964 656e 7469 6669   Unique identifi
-00006c40: 6572 2061 6e20 6f62 6a65 6374 2069 6e20  er an object in 
-00006c50: 4f70 656e 4249 532e 0a0a 2020 2020 4441  OpenBIS...    DA
-00006c60: 5441 5f53 4554 5f54 5950 4520 2020 4e65  TA_SET_TYPE   Ne
-00006c70: 776c 7920 6372 6561 7465 6420 6461 7461  wly created data
-00006c80: 2073 6574 2074 7970 652e 0a20 2020 2046   set type..    F
-00006c90: 7299 0000 0072 3000 0000 7253 0100 0063  r....r0...rS...c
-00006ca0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00006cb0: 0500 0000 1300 0000 72fd 0000 0072 1a00  ........r....r..
-00006cc0: 0000 2901 7253 0100 0072 3200 0000 a903  ..).rS...r2.....
-00006cd0: 7252 0100 0072 4f01 0000 7251 0100 0072  rR...rO...rQ...r
-00006ce0: 1200 0000 7213 0000 0072 3600 0000 ab03  ....r....r6.....
-00006cf0: 0000 72df 0000 007a 1875 706c 6f61 642e  ..r....z.upload.
-00006d00: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
-00006d10: 3e4e 2903 7209 0000 0072 2a00 0000 7238  >N).r....r*...r8
-00006d20: 0000 0029 0472 2b00 0000 7251 0100 0072  ...).r+...rQ...r
-00006d30: 5201 0000 724f 0100 0072 1200 0000 7254  R...rO...r....rT
-00006d40: 0100 0072 1300 0000 7253 0100 00a1 0300  ...r....rS......
-00006d50: 0073 0800 0000 1408 0c01 0e01 08ff 7a02  .s............z.
-00006d60: 2d75 7a0a 2d2d 7373 685f 7573 6572 7a29  -uz.--ssh_userz)
-00006d70: 5573 6572 2074 6f20 636f 6e6e 6563 7420  User to connect 
-00006d80: 746f 2072 656d 6f74 6520 7379 7374 656d  to remote system
-00006d90: 7320 7669 6120 7373 687a 022d 637a 142d  s via sshz.-cz.-
-00006da0: 2d63 6f6e 7465 6e74 5f63 6f70 795f 696e  -content_copy_in
-00006db0: 6465 787a 4949 6e64 6578 206f 6620 7468  dexzIIndex of th
-00006dc0: 6520 636f 6e74 656e 7420 636f 7079 2074  e content copy t
-00006dd0: 6f20 636c 6f6e 6520 6672 6f6d 2069 6e20  o clone from in 
-00006de0: 6361 7365 2074 6865 7265 2061 7265 206d  case there are m
-00006df0: 756c 7469 706c 6520 636f 7069 6573 2903  ultiple copies).
-00006e00: 720d 0000 0072 2300 0000 7225 0000 007a  r....r#...r%...z
-00006e10: 2953 6b69 7020 6669 6c65 2069 6e74 6567  )Skip file integ
-00006e20: 7269 7479 2063 6865 636b 2077 6974 6820  rity check with 
-00006e30: 6368 6563 6b73 756d 732e da05 636c 6f6e  checksums...clon
-00006e40: 657a 3443 6c6f 6e65 2074 6865 2072 6570  ez4Clone the rep
-00006e50: 6f73 6974 6f72 7920 666f 756e 6420 696e  ository found in
-00006e60: 2074 6865 2067 6976 656e 2064 6174 6120   the given data 
-00006e70: 7365 7420 6964 2e63 0500 0000 0000 0000  set id.c........
-00006e80: 0000 0000 0500 0000 0700 0000 0300 0000  ................
-00006e90: f320 0000 007c 006a 0064 0119 00a0 0164  . ...|.j.d.....d
-00006ea0: 0287 0087 0187 0287 0366 0464 0364 0484  .........f.d.d..
-00006eb0: 08a1 0253 0029 054e 7230 0000 0072 5501  ...S.).Nr0...rU.
-00006ec0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-00006ed0: 0000 0006 0000 0013 0000 00f3 1000 0000  ................
-00006ee0: 7c00 a000 8801 8803 8800 8802 a104 5300  |.............S.
-00006ef0: 721a 0000 0029 0172 5501 0000 7232 0000  r....).rU...r2..
-00006f00: 00a9 04da 1263 6f6e 7465 6e74 5f63 6f70  .....content_cop
-00006f10: 795f 696e 6465 7872 4701 0000 724d 0100  y_indexrG...rM..
-00006f20: 00da 0873 7368 5f75 7365 7272 1200 0000  ...ssh_userr....
-00006f30: 7213 0000 0072 3600 0000 c103 0000 f306  r....r6.........
-00006f40: 0000 000a 0002 0104 ff7a 2064 6174 615f  .........z data_
-00006f50: 7365 745f 636c 6f6e 652e 3c6c 6f63 616c  set_clone.<local
-00006f60: 733e 2e3c 6c61 6d62 6461 3e72 ac00 0000  s>.<lambda>r....
-00006f70: a905 722b 0000 0072 5a01 0000 7259 0100  ..r+...rZ...rY..
-00006f80: 0072 4701 0000 724d 0100 0072 1200 0000  .rG...rM...r....
-00006f90: 7258 0100 0072 1300 0000 da0e 6461 7461  rX...r......data
-00006fa0: 5f73 6574 5f63 6c6f 6e65 bc03 0000 f306  _set_clone......
-00006fb0: 0000 000c 0410 0104 ff72 5d01 0000 6305  .........r]...c.
-00006fc0: 0000 0000 0000 0000 0000 0005 0000 0007  ................
-00006fd0: 0000 0043 0000 00f3 2c00 0000 7400 7c00  ...C....,...t.|.
-00006fe0: 6a01 6401 6402 8d02 7c00 6a01 6403 3c00  j.d.d...|.j.d.<.
-00006ff0: 7c00 6a02 7403 7c01 7c02 7c03 7c04 6404  |.j.t.|.|.|.|.d.
-00007000: 8d05 0100 6400 5300 a905 4e46 7299 0000  ....d.S...NFr...
-00007010: 0072 3000 0000 2904 725a 0100 0072 5901  .r0...).rZ...rY.
-00007020: 0000 7247 0100 0072 4d01 0000 2904 7209  ..rG...rM...).r.
-00007030: 0000 0072 2a00 0000 7204 0100 0072 5d01  ...r*...r....r].
-00007040: 0000 725c 0100 0072 1200 0000 7212 0000  ..r\...r....r...
-00007050: 0072 1300 0000 7255 0100 00c5 0300 00f3  .r....rU........
-00007060: 0800 0000 1404 0a01 0401 0aff da04 6d6f  ..............mo
-00007070: 7665 7a33 4d6f 7665 2074 6865 2072 6570  vez3Move the rep
-00007080: 6f73 6974 6f72 7920 666f 756e 6420 696e  ository found in
-00007090: 2074 6865 2067 6976 656e 2064 6174 6120   the given data 
-000070a0: 7365 7420 6964 2e63 0500 0000 0000 0000  set id.c........
-000070b0: 0000 0000 0500 0000 0700 0000 0300 0000  ................
-000070c0: 7256 0100 0029 054e 7230 0000 0072 6201  rV...).Nr0...rb.
-000070d0: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-000070e0: 0000 0006 0000 0013 0000 0072 5701 0000  ...........rW...
-000070f0: 721a 0000 0029 0172 6201 0000 7232 0000  r....).rb...r2..
-00007100: 0072 5801 0000 7212 0000 0072 1300 0000  .rX...r....r....
-00007110: 7236 0000 00d5 0300 0072 5b01 0000 7a1f  r6.......r[...z.
-00007120: 6461 7461 5f73 6574 5f6d 6f76 652e 3c6c  data_set_move.<l
-00007130: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e72  ocals>.<lambda>r
-00007140: ac00 0000 725c 0100 0072 1200 0000 7258  ....r\...r....rX
-00007150: 0100 0072 1300 0000 da0d 6461 7461 5f73  ...r......data_s
-00007160: 6574 5f6d 6f76 65d0 0300 0072 5e01 0000  et_move....r^...
-00007170: 7263 0100 0063 0500 0000 0000 0000 0000  rc...c..........
-00007180: 0000 0500 0000 0700 0000 4300 0000 725f  ..........C...r_
-00007190: 0100 0072 6001 0000 2904 7209 0000 0072  ...r`...).r....r
-000071a0: 2a00 0000 7204 0100 0072 6301 0000 725c  *...r....rc...r\
-000071b0: 0100 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-000071c0: 0000 7262 0100 00d9 0300 0072 6101 0000  ..rb.......ra...
-000071d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000071e0: 0003 0000 0043 0000 0073 0e00 0000 7400  .....C...s....t.
-000071f0: 6900 6401 8d01 0100 6400 5300 2902 4e72  i.d.....d.S.).Nr
-00007200: 2900 0000 2901 722d 0000 0072 1200 0000  )...).r-...r....
-00007210: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
-00007220: 046d 6169 6ee2 0300 0073 0200 0000 0e01  .main....s......
-00007230: 7264 0100 00da 085f 5f6d 6169 6e5f 5f29  rd.....__main__)
-00007240: 024e 4e72 1a00 0000 296b da07 5f5f 646f  .NNr....)k..__do
-00007250: 635f 5f72 9f00 0000 7241 0000 0072 0200  c__r....rA...r..
-00007260: 0000 7216 0000 00da 1664 6174 6575 7469  ..r......dateuti
-00007270: 6c2e 7265 6c61 7469 7665 6465 6c74 6172  l.relativedeltar
-00007280: 0300 0000 da08 7265 7175 6573 7473 7204  ......requestsr.
-00007290: 0000 00da 0570 7962 6973 7205 0000 00da  .....pybisr.....
-000072a0: 0a63 6c69 636b 5f75 7469 6c72 0800 0000  .click_utilr....
-000072b0: da10 6461 7461 5f6d 676d 745f 7275 6e6e  ..data_mgmt_runn
-000072c0: 6572 7209 0000 00da 1164 6d2e 636f 6d6d  err......dm.comm
-000072d0: 616e 645f 7265 7375 6c74 720b 0000 00da  and_resultr.....
-000072e0: 0864 6d2e 7574 696c 7372 0c00 0000 7214  .dm.utilsr....r.
-000072f0: 0000 0072 1900 0000 7221 0000 00da 0567  ...r....r!.....g
-00007300: 726f 7570 da0e 7665 7273 696f 6e5f 6f70  roup..version_op
-00007310: 7469 6f6e da06 6f70 7469 6f6e da0c 7061  tion..option..pa
-00007320: 7373 5f63 6f6e 7465 7874 722d 0000 0072  ss_contextr-...r
-00007330: 3a00 0000 7249 0000 00da 0950 6172 616d  :...rI.....Param
-00007340: 5479 7065 724a 0000 0072 6400 0000 7265  TyperJ...rd...re
-00007350: 0000 0072 7c00 0000 727f 0000 0072 8700  ...r|...r....r..
-00007360: 0000 728d 0000 0072 9300 0000 7296 0000  ..r....r....r...
-00007370: 0072 6a00 0000 da07 636f 6d6d 616e 6472  .rj.....commandr
-00007380: 4b00 0000 7239 0000 00da 0861 7267 756d  K...r9.....argum
-00007390: 656e 7472 a800 0000 72ae 0000 0072 b100  entr....r....r..
-000073a0: 0000 da16 5f64 6174 6173 6574 5f73 6561  ...._dataset_sea
-000073b0: 7263 685f 7061 7261 6d73 da18 5f73 6561  rch_params.._sea
-000073c0: 7263 685f 6279 5f73 616d 706c 655f 7061  rch_by_sample_pa
-000073d0: 7261 6d73 72c3 0000 0072 c500 0000 72c7  ramsr....r....r.
-000073e0: 0000 0072 c800 0000 72cb 0000 0072 d900  ...r....r....r..
-000073f0: 0000 72e5 0000 0072 e800 0000 72eb 0000  ..r....r....r...
-00007400: 0072 ec00 0000 da15 5f6f 626a 6563 745f  .r......_object_
-00007410: 7365 6172 6368 5f70 6172 616d 7372 ee00  search_paramsr..
-00007420: 0000 72e3 0000 0072 f000 0000 72f1 0000  ..r....r....r...
-00007430: 0072 f200 0000 7285 0000 0072 f500 0000  .r....r....r....
-00007440: 72f6 0000 0072 f700 0000 da04 5061 7468  r....r......Path
-00007450: da0e 5f63 6f6d 6d69 745f 7061 7261 6d73  .._commit_params
-00007460: 7203 0100 0072 fb00 0000 da0c 5f69 6e69  r....r......_ini
-00007470: 745f 7061 7261 6d73 7207 0100 00da 155f  t_paramsr......_
-00007480: 696e 6974 5f70 6172 616d 735f 7068 7973  init_params_phys
-00007490: 6963 616c 7206 0100 00da 155f 696e 6974  icalr......_init
-000074a0: 5f61 6e61 6c79 7369 735f 7061 7261 6d73  _analysis_params
-000074b0: 720a 0100 0072 3c00 0000 da0e 5f73 7461  r....r<....._sta
-000074c0: 7475 735f 7061 7261 6d73 720e 0100 0072  tus_paramsr....r
-000074d0: 0b01 0000 da0c 5f73 796e 635f 7061 7261  ......_sync_para
-000074e0: 6d73 7217 0100 0072 1b01 0000 7216 0100  msr....r....r...
-000074f0: 0072 1d01 0000 7241 0100 00da 0e5f 6164  .r....rA....._ad
-00007500: 6472 6566 5f70 6172 616d 7372 4401 0000  dref_paramsrD...
-00007510: 7242 0100 00da 115f 7265 6d6f 7665 7265  rB....._removere
-00007520: 665f 7061 7261 6d73 7249 0100 0072 4501  f_paramsrI...rE.
-00007530: 0000 da10 5f64 6f77 6e6c 6f61 645f 7061  ...._download_pa
-00007540: 7261 6d73 724c 0100 00da 0e5f 7570 6c6f  ramsrL....._uplo
-00007550: 6164 5f70 6172 616d 7372 5301 0000 7234  ad_paramsrS...r4
-00007560: 0100 00da 125f 636c 6f6e 655f 6d6f 7665  ....._clone_move
-00007570: 5f70 6172 616d 7372 5d01 0000 7255 0100  _paramsr]...rU..
-00007580: 0072 6301 0000 7262 0100 0072 6401 0000  .rc...rb...rd...
-00007590: 7260 0000 0072 1200 0000 7212 0000 0072  r`...r....r....r
-000075a0: 1200 0000 7213 0000 00da 083c 6d6f 6475  ....r......<modu
-000075b0: 6c65 3e01 0000 0073 1603 0000 0412 0805  le>....s........
-000075c0: 0801 0c01 0802 0c01 0c01 0c02 0c01 0c01  ................
-000075d0: 0c01 0c01 0803 0805 0805 0609 0a01 1201  ................
-000075e0: 0c01 0201 04ff 1202 0401 1401 0807 0809  ................
-000075f0: 1214 100f 1204 082b 0808 0c07 080b 0807  .......+........
-00007600: 0809 060b 1201 0401 0e01 0805 0401 0c01  ................
-00007610: 060a 1201 0401 0e01 0808 1001 0401 0e01  ................
-00007620: 0805 1001 0401 0e01 0805 1001 0401 0e01  ................
-00007630: 1008 1001 1001 0c01 0201 04ff 1202 1001  ................
-00007640: 1001 0c01 0201 04ff 0c02 0201 04ff 1002  ................
-00007650: 0e01 0201 04ff 04f2 0c13 0201 04ff 0c02  ................
-00007660: 0201 04ff 0c02 0201 04ff 0c02 0201 04ff  ................
-00007670: 0c02 0201 04ff 0a02 0201 04ff 0a02 0201  ................
-00007680: 04ff 0802 0401 0201 04fe 0803 0401 0201  ................
-00007690: 04fe 04ee 0818 1201 0c01 0201 04ff 0402  ................
-000076a0: 1001 0809 1001 0401 0e01 0805 1001 0401  ................
-000076b0: 0e01 0805 1001 0401 0e01 0805 0c04 0a01  ................
-000076c0: 0401 0e01 062a 1201 0401 0e01 080b 1001  .....*..........
-000076d0: 0401 0e01 0808 1001 0401 0e01 0808 1001  ................
-000076e0: 0401 0e01 1006 1001 1001 0c01 0201 04ff  ................
-000076f0: 1202 1001 0a01 0201 04ff 0c02 0201 04ff  ................
-00007700: 0c02 0201 04ff 1002 0e01 0201 04ff 04f1  ................
-00007710: 0c14 0601 0401 0e01 061d 1201 0401 0e01  ................
-00007720: 080b 1001 0401 0e01 0808 1001 0401 0e01  ................
-00007730: 0808 1001 0401 0e01 0608 1201 0401 0e01  ................
-00007740: 080e 1001 0401 0e01 0808 1001 0401 0e01  ................
-00007750: 0808 1001 0401 0e01 0a0b 0201 04ff 0c02  ................
-00007760: 0201 04ff 0a02 0401 04ff 0a02 0401 04ff  ................
-00007770: 0201 04ff 04f9 0c0c 0401 0601 0e01 0a08  ................
-00007780: 0401 0601 0e01 0a0c 0401 04ff 0201 04ff  ................
-00007790: 0c02 04fd 0c08 0401 0601 0e01 0207 0e01  ................
-000077a0: 0201 06ff 02ff 02ff 0a06 0401 0601 0e01  ................
-000077b0: 080f 0c01 04ff 04ff 0804 0c03 0401 0601  ................
-000077c0: 0e01 0c05 0401 0601 0e01 0a0b 0401 04ff  ................
-000077d0: 0201 04ff 04ff 0c06 0401 0601 0e01 0a05  ................
-000077e0: 0401 0601 0e01 0a0a 0401 04ff 0a02 0401  ................
-000077f0: 04ff 0201 04ff 04fd 0808 0c05 0401 0601  ................
-00007800: 0e01 0a06 0401 0601 0e01 0a07 0401 0c01  ................
-00007810: 0c04 0c01 1201 1201 1201 0401 1c01 0a38  ...............8
-00007820: 0401 04ff 0201 04ff 04ff 1006 0401 0601  ................
-00007830: 1201 0c05 0401 0601 1201 0a0a 0401 06ff  ................
-00007840: 0a02 0401 04ff 0201 04ff 04fd 0808 0401  ................
-00007850: 04ff 0402 0601 1201 0c09 0401 0601 1201  ................
-00007860: 0e0c 1001 0401 06ff 0403 0c01 0401 06fe  ................
-00007870: 0e03 0401 04ff 04f8 100d 0601 0401 1201  ................
-00007880: 0412 1401 06ff 0a02 0a01 04fc 1008 0601  ................
-00007890: 0401 1201 0e0e 0401 04ff 1002 0401 06ff  ................
-000078a0: 0c02 0601 04ff 0a02 04f9 100b 0401 0601  ................
-000078b0: 1201 0c06 0401 0601 1201 1008 0401 0601  ................
-000078c0: 1201 0c06 0401 0601 1201 0c06 0c04 0a01  ................
-000078d0: 04ff                                     ..
+00000c30: 6417 6417 9001 6425 8d06 6504 6a18 6496  d.d...d%..e.j.d.
+00000c40: 9001 6426 9001 6427 9001 6428 6416 6417  ..d&..d'..d(d.d.
+00000c50: 6700 9001 6429 8d07 6504 a02b 9001 642a  g...d)..e..+..d*
+00000c60: a101 6504 a02b 9001 642b a101 6704 5a61  ..e..+..d+..g.Za
+00000c70: 651a 6a28 9001 642c 9001 642d 64a5 8d02  e.j(..d,..d-d...
+00000c80: 6515 6561 8301 6504 6a19 9001 642e 9001  e.ea..e.j...d...
+00000c90: 642c 8400 8301 8301 8301 5a62 6504 6a18  d,........Zbe.j.
+00000ca0: 9001 642f 9001 6430 6402 9001 6431 6450  ..d/..d0d...d1dP
+00000cb0: 8d04 6504 6a18 9001 6432 9001 6433 6563  ..e.j...d2..d3ec
+00000cc0: 6402 9001 6434 9001 6435 8d05 6504 6a18  d...d4..d5..e.j.
+00000cd0: 641a 9001 641e 6416 6417 9001 6436 6419  d...d.d.d...d6d.
+00000ce0: 8d05 6504 a02b 9001 6415 a101 6704 5a64  ..e..+..d...g.Zd
+00000cf0: 6531 6a28 9001 6437 9001 6438 64a5 8d02  e1j(..d7..d8d...
+00000d00: 6504 6a19 6515 6564 8301 9001 6439 9001  e.j.e.ed....d9..
+00000d10: 643a 8400 8301 8301 8301 5a65 651a 6a28  d:........Zee.j(
+00000d20: 9001 6438 64a5 8d01 6504 6a19 6515 6564  ..d8d...e.j.e.ed
+00000d30: 8301 9001 643b 9001 6437 8400 8301 8301  ....d;..d7......
+00000d40: 8301 5a66 6531 6a28 9001 643c 9001 643d  ..Zfe1j(..d<..d=
+00000d50: 64a5 8d02 6504 6a19 6515 6564 8301 9001  d...e.j.e.ed....
+00000d60: 643e 9001 643f 8400 8301 8301 8301 5a67  d>..d?........Zg
+00000d70: 651a 6a28 9001 643d 64a5 8d01 6504 6a19  e.j(..d=d...e.j.
+00000d80: 6515 6564 8301 9001 6440 9001 643c 8400  e.ed....d@..d<..
+00000d90: 8301 8301 8301 5a68 9001 6441 9001 6442  ......Zh..dA..dB
+00000da0: 8400 5a69 656a 9001 6443 6b02 9006 72c6  ..Ziej..dCk...r.
+00000db0: 6569 8300 0100 6402 5300 6402 5300 2846  ei....d.S.d.S.(F
+00000dc0: 0100 007a 360a 636c 692e 7079 0a0a 5468  ...z6.cli.py..Th
+00000dd0: 6520 6d6f 6475 6c65 2074 6861 7420 696d  e module that im
+00000de0: 706c 656d 656e 7473 2074 6865 2043 4c49  plements the CLI
+00000df0: 2066 6f72 206f 6269 732e 0ae9 0000 0000   for obis.......
+00000e00: 4e29 01da 0864 6174 6574 696d 6529 01da  N)...datetime)..
+00000e10: 0d72 656c 6174 6976 6564 656c 7461 2901  .relativedelta).
+00000e20: da0f 436f 6e6e 6563 7469 6f6e 4572 726f  ..ConnectionErro
+00000e30: 7229 01da 074f 7065 6e62 6973 e901 0000  r)...Openbis....
+00000e40: 00a9 01da 0a63 6c69 636b 5f65 6368 6f29  .....click_echo)
+00000e50: 01da 0e44 6174 614d 676d 7452 756e 6e65  ...DataMgmtRunne
+00000e60: 72e9 0200 0000 2901 da0d 436f 6d6d 616e  r.....)...Comman
+00000e70: 6452 6573 756c 7429 01da 0d4f 7065 7261  dResult)...Opera
+00000e80: 7469 6f6e 5479 7065 6301 0000 0000 0000  tionTypec.......
+00000e90: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00000ea0: 0073 2000 0000 7c00 6401 1900 6402 6b02  .s ...|.d...d.k.
+00000eb0: 720e 7400 7c00 6403 1900 8301 0100 6400  r.t.|.d.......d.
+00000ec0: 5300 6400 5300 2904 4eda 0474 7970 65da  S.d.S.).N..type.
+00000ed0: 0870 726f 6772 6573 73da 076d 6573 7361  .progress..messa
+00000ee0: 6765 7207 0000 00a9 01da 0d70 726f 6772  ger........progr
+00000ef0: 6573 735f 6461 7461 a900 7212 0000 00fa  ess_data..r.....
+00000f00: 5c2f 686f 6d65 2f61 6c61 736b 6f77 736b  \/home/alaskowsk
+00000f10: 692f 7265 706f 2f6f 7065 6e62 6973 5f70  i/repo/openbis_p
+00000f20: 7974 686f 6e2f 6170 702d 6f70 656e 6269  ython/app-openbi
+00000f30: 732d 636f 6d6d 616e 642d 6c69 6e65 2f73  s-command-line/s
+00000f40: 7263 2f70 7974 686f 6e2f 6f62 6973 2f73  rc/python/obis/s
+00000f50: 6372 6970 7473 2f63 6c69 2e70 79da 0e63  cripts/cli.py..c
+00000f60: 6c69 636b 5f70 726f 6772 6573 7327 0000  lick_progress'..
+00000f70: 0073 0600 0000 0c01 1001 04ff 7214 0000  .s..........r...
+00000f80: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00000f90: 0000 0600 0000 4300 0000 7328 0000 007c  ......C...s(...|
+00000fa0: 0064 0119 0064 026b 0272 1274 00a0 0164  .d...d.k.r.t...d
+00000fb0: 03a0 027c 0064 0419 00a1 01a1 0101 0064  ...|.d.........d
+00000fc0: 0053 0064 0053 0029 054e 720d 0000 0072  .S.d.S.).Nr....r
+00000fd0: 0e00 0000 fa02 7b7d 720f 0000 0029 03da  ......{}r....)..
+00000fe0: 0563 6c69 636b da04 6563 686f da06 666f  .click..echo..fo
+00000ff0: 726d 6174 7210 0000 0072 1200 0000 7212  rmatr....r....r.
+00001000: 0000 0072 1300 0000 da14 636c 6963 6b5f  ...r......click_
+00001010: 7072 6f67 7265 7373 5f6e 6f5f 7473 2c00  progress_no_ts,.
+00001020: 0000 7306 0000 000c 0118 0104 ff72 1900  ..s..........r..
+00001030: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00001040: 0000 0003 0000 0003 0000 0073 1000 0000  ...........s....
+00001050: 8700 6601 6401 6402 8408 7d01 7c01 5300  ..f.d.d...}.|.S.
+00001060: 2903 4e63 0100 0000 0000 0000 0000 0000  ).Nc............
+00001070: 0200 0000 0300 0000 1300 0000 731a 0000  ............s...
+00001080: 0074 0088 0083 0144 005d 067d 017c 017c  .t.....D.].}.|.|
+00001090: 0083 017d 0071 047c 0053 00a9 014e 2901  ...}.q.|.S...N).
+000010a0: da08 7265 7665 7273 6564 2902 da04 6675  ..reversed)...fu
+000010b0: 6e63 da05 7061 7261 6da9 01da 0670 6172  nc..param....par
+000010c0: 616d 7372 1200 0000 7213 0000 00da 0b5f  amsr....r......_
+000010d0: 6164 645f 7061 7261 6d73 3200 0000 7306  add_params2...s.
+000010e0: 0000 000c 010a 0104 017a 1f61 6464 5f70  .........z.add_p
+000010f0: 6172 616d 732e 3c6c 6f63 616c 733e 2e5f  arams.<locals>._
+00001100: 6164 645f 7061 7261 6d73 7212 0000 0029  add_paramsr....)
+00001110: 0272 1f00 0000 7220 0000 0072 1200 0000  .r....r ...r....
+00001120: 721e 0000 0072 1300 0000 da0a 6164 645f  r....r......add_
+00001130: 7061 7261 6d73 3100 0000 7304 0000 000c  params1...s.....
+00001140: 0104 0572 2100 0000 2901 da07 7665 7273  ...r!...)...vers
+00001150: 696f 6e7a 022d 717a 072d 2d71 7569 6574  ionz.-qz.--quiet
+00001160: 4654 7a1a 5375 7070 7265 7373 2073 7461  FTz.Suppress sta
+00001170: 7475 7320 7265 706f 7274 696e 672e 2903  tus reporting.).
+00001180: da07 6465 6661 756c 74da 0769 735f 666c  ..default..is_fl
+00001190: 6167 da04 6865 6c70 7a02 2d73 7a13 2d2d  ag..helpz.-sz.--
+000011a0: 736b 6970 5f76 6572 6966 6963 6174 696f  skip_verificatio
+000011b0: 6e7a 1944 6f20 6e6f 7420 7665 7269 6679  nz.Do not verify
+000011c0: 2063 6572 6669 6369 6174 6573 7a02 2d64   cerficiatesz.-d
+000011d0: 7a07 2d2d 6465 6275 677a 1a53 686f 7720  z.--debugz.Show 
+000011e0: 7374 6163 6b20 7472 6163 6520 6f6e 2065  stack trace on e
+000011f0: 7272 6f72 2e63 0400 0000 0000 0000 0000  rror.c..........
+00001200: 0000 0400 0000 0300 0000 4300 0000 7326  ..........C...s&
+00001210: 0000 007c 017c 006a 0064 013c 007c 0272  ...|.|.j.d.<.|.r
+00001220: 0c64 027c 006a 0064 033c 007c 037c 006a  .d.|.j.d.<.|.|.j
+00001230: 0064 043c 0064 0053 0029 054e da05 7175  .d.<.d.S.).N..qu
+00001240: 6965 7446 da13 7665 7269 6679 5f63 6572  ietF..verify_cer
+00001250: 7469 6669 6361 7465 73da 0564 6562 7567  tificates..debug
+00001260: a901 da03 6f62 6a29 04da 0363 7478 7226  ....obj)...ctxr&
+00001270: 0000 00da 1173 6b69 705f 7665 7269 6669  .....skip_verifi
+00001280: 6361 7469 6f6e 7228 0000 0072 1200 0000  cationr(...r....
+00001290: 7212 0000 0072 1300 0000 da03 636c 693a  r....r......cli:
+000012a0: 0000 0073 0800 0000 0a08 0401 0a01 0e01  ...s............
+000012b0: 722d 0000 0063 0300 0000 0000 0000 0000  r-...c..........
+000012c0: 0000 0300 0000 0600 0000 0300 0000 7346  ..............sF
+000012d0: 0000 007c 0164 0175 0072 0664 027d 0174  ...|.d.u.r.d.}.t
+000012e0: 0064 03a0 017c 01a1 0183 0101 0088 0064  .d...|.........d
+000012f0: 046b 0372 1388 006e 0164 0189 007c 006a  .k.r...n.d...|.j
+00001300: 0264 0519 00a0 0364 0687 0066 0164 0764  .d.....d...f.d.d
+00001310: 0884 087c 01a1 0353 0029 097a 3053 6861  ...|...S.).z0Sha
+00001320: 7265 6420 696d 706c 656d 656e 7461 7469  red implementati
+00001330: 6f6e 2066 6f72 2074 6865 2069 6e69 745f  on for the init_
+00001340: 6461 7461 2063 6f6d 6d61 6e64 2e4e da01  data command.N..
+00001350: 2e7a 0c69 6e69 745f 6461 7461 207b 7dda  .z.init_data {}.
+00001360: 00da 0672 756e 6e65 72da 0969 6e69 745f  ...runner..init_
+00001370: 6461 7461 6301 0000 0000 0000 0000 0000  datac...........
+00001380: 0001 0000 0003 0000 0013 0000 0073 0a00  .............s..
+00001390: 0000 7c00 a000 8800 a101 5300 721a 0000  ..|.......S.r...
+000013a0: 0029 0172 3100 0000 a901 da02 646d a901  .).r1.......dm..
+000013b0: da04 6465 7363 7212 0000 0072 1300 0000  ..descr....r....
+000013c0: da08 3c6c 616d 6264 613e 4e00 0000 f302  ..<lambda>N.....
+000013d0: 0000 000a 007a 2069 6e69 745f 6461 7461  .....z init_data
+000013e0: 5f69 6d70 6c2e 3c6c 6f63 616c 733e 2e3c  _impl.<locals>.<
+000013f0: 6c61 6d62 6461 3e29 0472 0800 0000 7218  lambda>).r....r.
+00001400: 0000 0072 2a00 0000 da03 7275 6e29 0372  ...r*.....run).r
+00001410: 2b00 0000 da0a 7265 706f 7369 746f 7279  +.....repository
+00001420: 7235 0000 0072 1200 0000 7234 0000 0072  r5...r....r4...r
+00001430: 1300 0000 da0e 696e 6974 5f64 6174 615f  ......init_data_
+00001440: 696d 706c 4800 0000 730a 0000 0008 0204  implH...s.......
+00001450: 010e 0110 011c 0172 3a00 0000 6304 0000  .......r:...c...
+00001460: 0000 0000 0000 0000 0006 0000 0006 0000  ................
+00001470: 0003 0000 0073 ce00 0000 7400 6401 a001  .....s....t.d...
+00001480: 7c02 a101 8301 0100 8801 6400 7501 7217  |.........d.u.r.
+00001490: 7402 6a03 a004 8801 a101 7217 7400 6402  t.j.......r.t.d.
+000014a0: 8301 0100 6403 5300 7c02 6400 7501 7227  ....d.S.|.d.u.r'
+000014b0: 7402 6a03 a004 7c02 a101 7227 7400 6404  t.j...|...r't.d.
+000014c0: 8301 0100 6403 5300 8800 6405 6b03 722d  ....d.S...d.k.r-
+000014d0: 8800 6e01 6400 8900 8801 6400 7500 7237  ..n.d.....d.u.r7
+000014e0: 7402 a005 a100 6e08 7402 6a03 a006 7402  t.....n.t.j...t.
+000014f0: a005 a100 8801 a102 7d04 7402 6a03 a006  ........}.t.j...
+00001500: 7402 a005 a100 7c02 a102 7d05 7402 6a03  t.....|...}.t.j.
+00001510: a007 7c04 7c05 a102 8901 8801 6400 7500  ..|.|.......d.u.
+00001520: 7256 6406 6e01 8801 8901 7c00 6a08 6407  rVd.n.....|.j.d.
+00001530: 1900 a009 6408 8700 8701 6602 6409 640a  ....d.....f.d.d.
+00001540: 8408 7c02 a103 5300 290b 4e7a 1069 6e69  ..|...S.).Nz.ini
+00001550: 745f 616e 616c 7973 6973 207b 7d7a 3345  t_analysis {}z3E
+00001560: 7272 6f72 3a20 5468 6520 7061 7265 6e74  rror: The parent
+00001570: 206d 7573 7420 6265 2067 6976 656e 2061   must be given a
+00001580: 7320 6120 7265 6c61 7469 7665 2070 6174  s a relative pat
+00001590: 682e e9ff ffff ff7a 3745 7272 6f72 3a20  h......z7Error: 
+000015a0: 5468 6520 7265 706f 7369 746f 7279 206d  The repository m
+000015b0: 7573 7420 6265 2067 6976 656e 2061 7320  ust be given as 
+000015c0: 6120 7265 6c61 7469 7665 2070 6174 682e  a relative path.
+000015d0: 722f 0000 007a 022e 2e72 3000 0000 da0d  r/...z...r0.....
+000015e0: 696e 6974 5f61 6e61 6c79 7369 7363 0100  init_analysisc..
+000015f0: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+00001600: 0000 1300 0000 730c 0000 007c 00a0 0088  ......s....|....
+00001610: 0188 00a1 0253 0072 1a00 0000 2901 723c  .....S.r....).r<
+00001620: 0000 0072 3200 0000 a902 da0b 6465 7363  ...r2.......desc
+00001630: 7269 7074 696f 6eda 0670 6172 656e 7472  ription..parentr
+00001640: 1200 0000 7213 0000 0072 3600 0000 5e00  ....r....r6...^.
+00001650: 0000 f302 0000 000c 007a 2469 6e69 745f  .........z$init_
+00001660: 616e 616c 7973 6973 5f69 6d70 6c2e 3c6c  analysis_impl.<l
+00001670: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e29  ocals>.<lambda>)
+00001680: 0a72 0800 0000 7218 0000 00da 026f 73da  .r....r......os.
+00001690: 0470 6174 68da 0569 7361 6273 da06 6765  .path..isabs..ge
+000016a0: 7463 7764 da04 6a6f 696e da07 7265 6c70  tcwd..join..relp
+000016b0: 6174 6872 2a00 0000 7238 0000 0029 0672  athr*...r8...).r
+000016c0: 2b00 0000 723f 0000 0072 3900 0000 723e  +...r?...r9...r>
+000016d0: 0000 00da 0a70 6172 656e 745f 6469 72da  .....parent_dir.
+000016e0: 0c61 6e61 6c79 7369 735f 6469 7272 1200  .analysis_dirr..
+000016f0: 0000 723d 0000 0072 1300 0000 da12 696e  ..r=...r......in
+00001700: 6974 5f61 6e61 6c79 7369 735f 696d 706c  it_analysis_impl
+00001710: 5100 0000 731e 0000 000e 0114 0108 0104  Q...s...........
+00001720: 0114 0108 0104 0110 0122 0112 010e 0110  ........."......
+00001730: 0118 0102 0104 ff72 4900 0000 6300 0000  .......rI...c...
+00001740: 0000 0000 0000 0000 0000 0000 0002 0000  ................
+00001750: 0040 0000 0073 2000 0000 6500 5a01 6400  .@...s ...e.Z.d.
+00001760: 5a02 6401 5a03 6402 6403 8400 5a04 6404  Z.d.Z.d.d...Z.d.
+00001770: 6405 8400 5a05 6406 5300 2907 da0b 5365  d...Z.d.S.)...Se
+00001780: 7474 696e 6773 4765 74da 0c73 6574 7469  ttingsGet..setti
+00001790: 6e67 735f 6765 7463 0400 0000 0000 0000  ngs_getc........
+000017a0: 0000 0000 0500 0000 0600 0000 4300 0000  ............C...
+000017b0: 7336 0000 007a 0f74 0074 0164 0164 0284  s6...z.t.t.d.d..
+000017c0: 007c 01a0 0264 03a1 0183 0283 017d 047c  .|...d.......}.|
+000017d0: 0457 0053 0001 0001 0001 007c 00a0 037c  .W.S.......|...|
+000017e0: 02a1 0101 0059 0064 0053 0029 044e 6301  .....Y.d.S.).Nc.
+000017f0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00001800: 0000 0053 0000 00f3 0c00 0000 7400 7c00  ...S........t.|.
+00001810: 8301 6401 6b04 5300 a902 4e72 0100 0000  ..d.k.S...Nr....
+00001820: a901 da03 6c65 6ea9 01da 0474 6572 6d72  ....len....termr
+00001830: 1200 0000 7212 0000 0072 1300 0000 7236  ....r....r....r6
+00001840: 0000 006a 0000 0072 4000 0000 7a25 5365  ...j...r@...z%Se
+00001850: 7474 696e 6773 4765 742e 636f 6e76 6572  ttingsGet.conver
+00001860: 742e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  t.<locals>.<lamb
+00001870: 6461 3efa 012c 2904 da04 6c69 7374 da06  da>..,)...list..
+00001880: 6669 6c74 6572 da05 7370 6c69 74da 055f  filter..split.._
+00001890: 6661 696c 2905 da04 7365 6c66 da05 7661  fail)...self..va
+000018a0: 6c75 6572 1d00 0000 722b 0000 0072 5500  luer....r+...rU.
+000018b0: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+000018c0: 00da 0763 6f6e 7665 7274 6800 0000 730a  ...converth...s.
+000018d0: 0000 0002 0118 0106 0106 0110 017a 1353  .............z.S
+000018e0: 6574 7469 6e67 7347 6574 2e63 6f6e 7665  ettingsGet.conve
+000018f0: 7274 6302 0000 0000 0000 0000 0000 0002  rtc.............
+00001900: 0000 0004 0000 0043 0000 00f3 1200 0000  .......C........
+00001910: 7c00 6a00 7c01 6401 6402 8d02 0100 6400  |.j.|.d.d.....d.
+00001920: 5300 2903 4e7a 2f53 6574 7469 6e67 7320  S.).Nz/Settings 
+00001930: 6d75 7374 2062 6520 696e 2074 6865 2066  must be in the f
+00001940: 6f72 6d61 743a 206b 6579 312c 206b 6579  ormat: key1, key
+00001950: 322c 202e 2e2e a902 721d 0000 0072 0f00  2, .....r....r..
+00001960: 0000 a901 da04 6661 696c a902 7257 0000  ......fail..rW..
+00001970: 0072 1d00 0000 7212 0000 0072 1200 0000  .r....r....r....
+00001980: 7213 0000 0072 5600 0000 6f00 0000 f306  r....rV...o.....
+00001990: 0000 0004 0104 010a ff7a 1153 6574 7469  .........z.Setti
+000019a0: 6e67 7347 6574 2e5f 6661 696c 4e29 06da  ngsGet._failN)..
+000019b0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+000019c0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+000019d0: 655f 5fda 046e 616d 6572 5900 0000 7256  e__..namerY...rV
+000019e0: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
+000019f0: 0000 7213 0000 0072 4a00 0000 6500 0000  ..r....rJ...e...
+00001a00: 7308 0000 0008 0004 0108 020c 0772 4a00  s............rJ.
+00001a10: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00001a20: 0000 0001 0000 0040 0000 0073 0c00 0000  .......@...s....
+00001a30: 6500 5a01 6400 5a02 6401 5300 2902 da0d  e.Z.d.Z.d.S.)...
+00001a40: 5365 7474 696e 6773 436c 6561 724e 2903  SettingsClearN).
+00001a50: 7260 0000 0072 6100 0000 7262 0000 0072  r`...ra...rb...r
+00001a60: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00001a70: 0000 0072 6400 0000 7400 0000 7304 0000  ...rd...t...s...
+00001a80: 0008 0004 0172 6400 0000 6300 0000 0000  .....rd...c.....
+00001a90: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
+00001aa0: 0000 0073 3000 0000 6500 5a01 6400 5a02  ...s0...e.Z.d.Z.
+00001ab0: 6401 5a03 6402 6403 8400 5a04 6404 6405  d.Z.d.d...Z.d.d.
+00001ac0: 8400 5a05 6406 6407 8400 5a06 6408 6409  ..Z.d.d...Z.d.d.
+00001ad0: 8400 5a07 640a 5300 290b da0b 5365 7474  ..Z.d.S.)...Sett
+00001ae0: 696e 6773 5365 74da 0c73 6574 7469 6e67  ingsSet..setting
+00001af0: 735f 7365 7463 0400 0000 0000 0000 0000  s_setc..........
+00001b00: 0000 0900 0000 0600 0000 4300 0000 738c  ..........C...s.
+00001b10: 0000 007a 3a7c 00a0 007c 01a1 017d 0169  ...z:|...|...}.i
+00001b20: 007d 0474 0174 0264 0164 0284 007c 01a0  .}.t.t.d.d...|..
+00001b30: 0364 03a1 0183 0283 017d 057c 0544 005d  .d.......}.|.D.]
+00001b40: 217d 067c 06a0 0364 04a1 017d 0774 047c  !}.|...d...}.t.|
+00001b50: 0783 0164 056b 0372 287c 00a0 057c 02a1  ...d.k.r(|...|..
+00001b60: 0101 007c 0764 0619 007d 087c 0764 0719  ...|.d...}.|.d..
+00001b70: 007d 017c 00a0 067c 01a1 017c 047c 083c  .}.|...|...|.|.<
+00001b80: 0071 167c 0457 0053 0001 0001 0001 007c  .q.|.W.S.......|
+00001b90: 00a0 057c 02a1 0101 0059 0064 0053 0029  ...|.....Y.d.S.)
+00001ba0: 084e 6301 0000 0000 0000 0000 0000 0001  .Nc.............
+00001bb0: 0000 0002 0000 0053 0000 0072 4c00 0000  .......S...rL...
+00001bc0: 724d 0000 0072 4e00 0000 7250 0000 0072  rM...rN...rP...r
+00001bd0: 1200 0000 7212 0000 0072 1300 0000 7236  ....r....r....r6
+00001be0: 0000 007f 0000 0072 4000 0000 7a25 5365  .......r@...z%Se
+00001bf0: 7474 696e 6773 5365 742e 636f 6e76 6572  ttingsSet.conver
+00001c00: 742e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  t.<locals>.<lamb
+00001c10: 6461 3e72 5200 0000 da01 3d72 0a00 0000  da>rR.....=r....
+00001c20: 7201 0000 0072 0600 0000 2907 da0c 5f65  r....r....)..._e
+00001c30: 6e63 6f64 655f 6a73 6f6e 7253 0000 0072  ncode_jsonrS...r
+00001c40: 5400 0000 7255 0000 0072 4f00 0000 7256  T...rU...rO...rV
+00001c50: 0000 00da 0c5f 6465 636f 6465 5f6a 736f  ....._decode_jso
+00001c60: 6e29 0972 5700 0000 7258 0000 0072 1d00  n).rW...rX...r..
+00001c70: 0000 722b 0000 00da 0873 6574 7469 6e67  ..r+.....setting
+00001c80: 7372 5500 0000 da07 7365 7474 696e 67da  srU.....setting.
+00001c90: 0d73 6574 7469 6e67 5f73 706c 6974 da03  .setting_split..
+00001ca0: 6b65 7972 1200 0000 7212 0000 0072 1300  keyr....r....r..
+00001cb0: 0000 7259 0000 007b 0000 0073 1c00 0000  ..rY...{...s....
+00001cc0: 0201 0a01 0401 1801 0801 0a01 0c01 0a01  ................
+00001cd0: 0801 0801 1001 0601 0601 1001 7a13 5365  ............z.Se
+00001ce0: 7474 696e 6773 5365 742e 636f 6e76 6572  ttingsSet.conver
+00001cf0: 7463 0200 0000 0000 0000 0000 0000 0700  tc..............
+00001d00: 0000 0600 0000 4300 0000 7362 0000 0064  ......C...sb...d
+00001d10: 017d 0264 027d 0364 037d 047c 037d 057c  .}.d.}.d.}.|.}.|
+00001d20: 0144 005d 247d 067c 0664 046b 0272 137c  .D.]$}.|.d.k.r.|
+00001d30: 047d 056e 067c 0664 056b 0272 197c 037d  .}.n.|.d.k.r.|.}
+00001d40: 057c 057c 036b 0272 227c 027c 0637 007d  .|.|.k.r"|.|.7.}
+00001d50: 0271 0a7c 057c 046b 0272 2e7c 027c 06a0  .q.|.|.k.r.|.|..
+00001d60: 0064 0664 07a1 0237 007d 0271 0a7c 0253  .d.d...7.}.q.|.S
+00001d70: 0029 084e 722f 0000 0072 0100 0000 7206  .).Nr/...r....r.
+00001d80: 0000 00da 017b da01 7d72 5200 0000 da01  .....{..}rR.....
+00001d90: 7ca9 01da 0772 6570 6c61 6365 2907 7257  |....replace).rW
+00001da0: 0000 0072 5800 0000 da07 656e 636f 6465  ...rX.....encode
+00001db0: 64da 0453 4545 4bda 0645 4e43 4f44 45da  d..SEEK..ENCODE.
+00001dc0: 046d 6f64 65da 0463 6861 7272 1200 0000  .mode..charr....
+00001dd0: 7212 0000 0072 1300 0000 7268 0000 008b  r....r....rh....
+00001de0: 0000 0073 1e00 0000 0401 0401 0401 0401  ...s............
+00001df0: 0801 0801 0601 0801 0401 0801 0a01 0801  ................
+00001e00: 1001 0280 0401 7a18 5365 7474 696e 6773  ......z.Settings
+00001e10: 5365 742e 5f65 6e63 6f64 655f 6a73 6f6e  Set._encode_json
+00001e20: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
+00001e30: 0004 0000 0043 0000 0073 0c00 0000 7c01  .....C...s....|.
+00001e40: a000 6401 6402 a102 5300 2903 4e72 7000  ..d.d...S.).Nrp.
+00001e50: 0000 7252 0000 0072 7100 0000 2902 7257  ..rR...rq...).rW
+00001e60: 0000 0072 5800 0000 7212 0000 0072 1200  ...rX...r....r..
+00001e70: 0000 7213 0000 0072 6900 0000 9b00 0000  ..r....ri.......
+00001e80: 7302 0000 000c 017a 1853 6574 7469 6e67  s......z.Setting
+00001e90: 7353 6574 2e5f 6465 636f 6465 5f6a 736f  sSet._decode_jso
+00001ea0: 6e63 0200 0000 0000 0000 0000 0000 0200  nc..............
+00001eb0: 0000 0400 0000 4300 0000 725a 0000 0029  ......C...rZ...)
+00001ec0: 034e 7a3d 5365 7474 696e 6773 206d 7573  .Nz=Settings mus
+00001ed0: 7420 6265 2069 6e20 7468 6520 666f 726d  t be in the form
+00001ee0: 6174 3a20 6b65 7931 3d76 616c 7565 312c  at: key1=value1,
+00001ef0: 206b 6579 323d 7661 6c75 6532 2c20 2e2e   key2=value2, ..
+00001f00: 2e72 5b00 0000 725c 0000 0072 5e00 0000  .r[...r\...r^...
+00001f10: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00001f20: 5600 0000 9e00 0000 725f 0000 007a 1153  V.......r_...z.S
+00001f30: 6574 7469 6e67 7353 6574 2e5f 6661 696c  ettingsSet._fail
+00001f40: 4e29 0872 6000 0000 7261 0000 0072 6200  N).r`...ra...rb.
+00001f50: 0000 7263 0000 0072 5900 0000 7268 0000  ..rc...rY...rh..
+00001f60: 0072 6900 0000 7256 0000 0072 1200 0000  .ri...rV...r....
+00001f70: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00001f80: 6500 0000 7800 0000 730c 0000 0008 0004  e...x...s.......
+00001f90: 0108 0208 1008 100c 0372 6500 0000 6301  .........re...c.
+00001fa0: 0000 0000 0000 0000 0000 0005 0000 0005  ................
+00001fb0: 0000 0043 0000 0073 2c00 0000 6900 7d01  ...C...s,...i.}.
+00001fc0: 7c00 4400 5d0f 7d02 7c02 a000 a100 4400  |.D.].}.|.....D.
+00001fd0: 5d08 5c02 7d03 7d04 7c04 7c01 7c03 3c00  ].\.}.}.|.|.|.<.
+00001fe0: 710a 7104 7c01 5300 721a 0000 0029 01da  q.q.|.S.r....)..
+00001ff0: 0569 7465 6d73 2905 da0d 7365 7474 696e  .items)...settin
+00002000: 675f 6469 6374 73da 066a 6f69 6e65 64da  g_dicts..joined.
+00002010: 0c73 6574 7469 6e67 5f64 6963 7472 6d00  .setting_dictrm.
+00002020: 0000 7258 0000 0072 1200 0000 7212 0000  ..rX...r....r...
+00002030: 0072 1300 0000 da12 5f6a 6f69 6e5f 7365  .r......_join_se
+00002040: 7474 696e 6773 5f73 6574 a300 0000 730c  ttings_set....s.
+00002050: 0000 0004 0108 0110 010a 0102 ff04 0272  ...............r
+00002060: 7c00 0000 6301 0000 0000 0000 0000 0000  |...c...........
+00002070: 0003 0000 0003 0000 0043 0000 0073 1a00  .........C...s..
+00002080: 0000 6700 7d01 7c00 4400 5d06 7d02 7c01  ..g.}.|.D.].}.|.
+00002090: 7c02 3700 7d01 7104 7c01 5300 721a 0000  |.7.}.q.|.S.r...
+000020a0: 0072 1200 0000 2903 da0d 7365 7474 696e  .r....)...settin
+000020b0: 675f 6c69 7374 7372 7a00 0000 da0c 7365  g_listsrz.....se
+000020c0: 7474 696e 675f 6c69 7374 7212 0000 0072  tting_listr....r
+000020d0: 1200 0000 7213 0000 00da 125f 6a6f 696e  ....r......_join
+000020e0: 5f73 6574 7469 6e67 735f 6765 74ab 0000  _settings_get...
+000020f0: 0073 0800 0000 0401 0801 0a01 0401 727f  .s............r.
+00002100: 0000 0063 0400 0000 0000 0000 0000 0000  ...c............
+00002110: 0800 0000 0800 0000 4300 0000 7350 0000  ........C...sP..
+00002120: 007c 006a 0064 0119 007d 047c 006a 0064  .|.j.d...}.|.j.d
+00002130: 0219 007d 057c 006a 0064 0319 007d 0664  ...}.|.j.d...}.d
+00002140: 047d 0764 057c 006a 0076 0072 1b7c 006a  .}.d.|.j.v.r.|.j
+00002150: 0064 0519 007d 077c 056a 017c 067c 047c  .d...}.|.j.|.|.|
+00002160: 077c 017c 027c 0364 068d 0601 0064 0053  .|.|.|.d.....d.S
+00002170: 0029 074e da09 6973 5f67 6c6f 6261 6c72  .).N..is_globalr
+00002180: 3000 0000 da08 7265 736f 6c76 6572 46da  0.....resolverF.
+00002190: 1469 735f 6461 7461 5f73 6574 5f70 726f  .is_data_set_pro
+000021a0: 7065 7274 79a9 02da 0470 726f 7072 5800  perty....proprX.
+000021b0: 0000 2902 722a 0000 00da 0663 6f6e 6669  ..).r*.....confi
+000021c0: 6729 0872 2b00 0000 da0e 6f70 6572 6174  g).r+.....operat
+000021d0: 696f 6e5f 7479 7065 7284 0000 0072 5800  ion_typer....rX.
+000021e0: 0000 7280 0000 0072 3000 0000 7281 0000  ..r....r0...r...
+000021f0: 0072 8200 0000 7212 0000 0072 1200 0000  .r....r....r....
+00002200: 7213 0000 00da 105f 6163 6365 7373 5f73  r......_access_s
+00002210: 6574 7469 6e67 73b2 0000 0073 1200 0000  ettings....s....
+00002220: 0a01 0a01 0a01 0401 0a01 0a01 0c01 0401  ................
+00002230: 0aff 7287 0000 0063 0200 0000 0000 0000  ..r....c........
+00002240: 0000 0000 0500 0000 0700 0000 4300 0000  ............C...
+00002250: 7338 0000 0074 007c 0183 017d 027c 02a0  s8...t.|...}.|..
+00002260: 01a1 0044 005d 0d5c 027d 037d 0474 027c  ...D.].\.}.}.t.|
+00002270: 0074 036a 047c 037c 0464 018d 0401 0071  .t.j.|.|.d.....q
+00002280: 0874 0564 0264 0364 048d 0253 0029 054e  .t.d.d.d...S.).N
+00002290: 7283 0000 0072 0100 0000 722f 0000 00a9  r....r....r/....
+000022a0: 02da 0a72 6574 7572 6e63 6f64 65da 066f  ...returncode..o
+000022b0: 7574 7075 7429 0672 7c00 0000 7278 0000  utput).r|...rx..
+000022c0: 0072 8700 0000 720c 0000 00da 0353 4554  .r....r......SET
+000022d0: 720b 0000 0029 0572 2b00 0000 726a 0000  r....).r+...rj..
+000022e0: 00da 0d73 6574 7469 6e67 735f 6469 6374  ...settings_dict
+000022f0: 7284 0000 0072 5800 0000 7212 0000 0072  r....rX...r....r
+00002300: 1200 0000 7213 0000 00da 045f 7365 74bd  ....r......_set.
+00002310: 0000 0073 0800 0000 0801 1001 1401 0c01  ...s............
+00002320: 728d 0000 0063 0200 0000 0000 0000 0000  r....c..........
+00002330: 0000 0400 0000 0600 0000 4300 0000 f340  ..........C....@
+00002340: 0000 0074 007c 0183 017d 0274 017c 0283  ...t.|...}.t.|..
+00002350: 0164 016b 0272 0d64 0067 017d 027c 0244  .d.k.r.d.g.}.|.D
+00002360: 005d 0a7d 0374 027c 0074 036a 047c 0364  .].}.t.|.t.j.|.d
+00002370: 028d 0301 0071 0f74 0564 0164 0364 048d  .....q.t.d.d.d..
+00002380: 0253 00a9 054e 7201 0000 0029 0172 8400  .S...Nr....).r..
+00002390: 0000 722f 0000 0072 8800 0000 2906 727f  ..r/...r....).r.
+000023a0: 0000 0072 4f00 0000 7287 0000 0072 0c00  ...rO...r....r..
+000023b0: 0000 da03 4745 5472 0b00 0000 a904 722b  ....GETr......r+
+000023c0: 0000 0072 6a00 0000 da0d 7365 7474 696e  ...rj.....settin
+000023d0: 6773 5f6c 6973 7472 8400 0000 7212 0000  gs_listr....r...
+000023e0: 0072 1200 0000 7213 0000 00da 045f 6765  .r....r......_ge
+000023f0: 74c4 0000 00f3 0c00 0000 0801 0c01 0601  t...............
+00002400: 0801 1201 0c01 7293 0000 0063 0200 0000  ......r....c....
+00002410: 0000 0000 0000 0000 0400 0000 0600 0000  ................
+00002420: 4300 0000 728e 0000 0072 8f00 0000 2906  C...r....r....).
+00002430: 727f 0000 0072 4f00 0000 7287 0000 0072  r....rO...r....r
+00002440: 0c00 0000 da05 434c 4541 5272 0b00 0000  ......CLEARr....
+00002450: 7291 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+00002460: 1300 0000 da06 5f63 6c65 6172 cd00 0000  ......_clear....
+00002470: 7294 0000 0072 9600 0000 7a02 2d67 7a0b  r....r....z.-gz.
+00002480: 2d2d 6973 5f67 6c6f 6261 6c7a 1447 6574  --is_globalz.Get
+00002490: 2067 6c6f 6261 6c20 6f72 206c 6f63 616c   global or local
+000024a0: 2e63 0200 0000 0000 0000 0000 0000 0200  .c..............
+000024b0: 0000 0300 0000 4300 0000 730e 0000 007c  ......C...s....|
+000024c0: 017c 006a 0064 013c 0064 0253 0029 037a  .|.j.d.<.d.S.).z
+000024d0: 2820 4578 7465 726e 616c 2044 6174 6120  ( External Data 
+000024e0: 5374 6f72 653a 2047 6574 2061 6c6c 2073  Store: Get all s
+000024f0: 6574 7469 6e67 732e 2072 8000 0000 4e72  ettings. r....Nr
+00002500: 2900 0000 2902 722b 0000 0072 8000 0000  )...).r+...r....
+00002510: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+00002520: 6a00 0000 d800 0000 f302 0000 000e 0572  j..............r
+00002530: 6a00 0000 da03 6765 7463 0100 0000 0000  j.....getc......
+00002540: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
+00002550: 0000 733a 0000 0074 007c 006a 0164 0164  ..s:...t.|.j.d.d
+00002560: 028d 027d 017c 01a0 02a1 007d 0274 036a  ...}.|.....}.t.j
+00002570: 047c 0264 0364 0464 058d 037d 0374 05a0  .|.d.d.d...}.t..
+00002580: 0664 06a0 077c 03a1 01a1 0101 0064 0753  .d...|.......d.S
+00002590: 0029 087a 2320 4578 7465 726e 616c 2044  .).z# External D
+000025a0: 6174 6120 5374 6f72 653a 2047 6574 2073  ata Store: Get s
+000025b0: 6574 7469 6e67 2e20 46a9 01da 1168 616c  etting. F....hal
+000025c0: 745f 6f6e 5f65 7272 6f72 5f6c 6f67 e904  t_on_error_log..
+000025d0: 0000 0054 2902 da06 696e 6465 6e74 da09  ...T)...indent..
+000025e0: 736f 7274 5f6b 6579 7372 1500 0000 4e29  sort_keysr....N)
+000025f0: 0872 0900 0000 722a 0000 00da 0c67 6574  .r....r*.....get
+00002600: 5f73 6574 7469 6e67 73da 046a 736f 6eda  _settings..json.
+00002610: 0564 756d 7073 7216 0000 0072 1700 0000  .dumpsr....r....
+00002620: 7218 0000 0029 0472 2b00 0000 7230 0000  r....).r+...r0..
+00002630: 0072 6a00 0000 da0c 7365 7474 696e 6773  .rj.....settings
+00002640: 5f73 7472 7212 0000 0072 1200 0000 7213  _strr....r....r.
+00002650: 0000 0072 4b00 0000 e000 0000 7308 0000  ...rK.......s...
+00002660: 000e 0408 0110 0114 0172 4b00 0000 7a18  .........rK...z.
+00002670: 5365 742f 6765 7420 676c 6f62 616c 206f  Set/get global o
+00002680: 7220 6c6f 6361 6c2e 6302 0000 0000 0000  r local.c.......
+00002690: 0000 0000 0003 0000 0004 0000 0043 0000  .............C..
+000026a0: 00f3 3000 0000 7400 7c00 6a01 6401 6402  ..0...t.|.j.d.d.
+000026b0: 8d02 7d02 7c01 7c00 6a01 6403 3c00 7c02  ..}.|.|.j.d.<.|.
+000026c0: 7c00 6a01 6404 3c00 6405 7c00 6a01 6406  |.j.d.<.d.|.j.d.
+000026d0: 3c00 6407 5300 2908 7a42 2045 7874 6572  <.d.S.).zB Exter
+000026e0: 6e61 6c20 4461 7461 2053 746f 7265 3a20  nal Data Store: 
+000026f0: 4765 742f 7365 7420 7365 7474 696e 6773  Get/set settings
+00002700: 2072 656c 6174 6564 2074 6f20 7468 6520   related to the 
+00002710: 7265 706f 7369 746f 7279 2e20 4672 9900  repository. Fr..
+00002720: 0000 7280 0000 0072 3000 0000 7239 0000  ..r....r0...r9..
+00002730: 0072 8100 0000 4ea9 0272 0900 0000 722a  .r....N..r....r*
+00002740: 0000 00a9 0372 2b00 0000 7280 0000 0072  .....r+...r....r
+00002750: 3000 0000 7212 0000 0072 1200 0000 7213  0...r....r....r.
+00002760: 0000 0072 3900 0000 ec00 0000 7308 0000  ...r9.......s...
+00002770: 000e 050a 010a 010e 0172 3900 0000 da03  .........r9.....
+00002780: 7365 7472 3b00 0000 2902 720d 0000 00da  setr;...).r.....
+00002790: 056e 6172 6773 6302 0000 0000 0000 0000  .nargsc.........
+000027a0: 0000 0002 0000 0006 0000 0003 0000 00f3  ................
+000027b0: 1c00 0000 8800 6a00 6401 1900 a001 6402  ......j.d.....d.
+000027c0: 8700 8701 6602 6403 6404 8408 a102 5300  ....f.d.d.....S.
+000027d0: 2905 7a3e 2045 7874 6572 6e61 6c20 4461  ).z> External Da
+000027e0: 7461 2053 746f 7265 3a20 5365 7420 7365  ta Store: Set se
+000027f0: 7474 696e 6773 2072 656c 6174 6564 2074  ttings related t
+00002800: 6f20 7468 6520 7265 706f 7369 746f 7279  o the repository
+00002810: 2e20 7230 0000 00da 0e72 6570 6f73 6974  . r0.....reposit
+00002820: 6f72 795f 7365 7463 0100 0000 0000 0000  ory_setc........
+00002830: 0000 0000 0100 0000 0300 0000 1300 0000  ................
+00002840: f30a 0000 0074 0088 0088 0183 0253 0072  .....t.......S.r
+00002850: 1a00 0000 a901 728d 0000 0072 3200 0000  ......r....r2...
+00002860: a902 722b 0000 0072 6a00 0000 7212 0000  ..r+...rj...r...
+00002870: 0072 1300 0000 7236 0000 00fc 0000 0072  .r....r6.......r
+00002880: 3700 0000 7a20 7265 706f 7369 746f 7279  7...z repository
+00002890: 5f73 6574 2e3c 6c6f 6361 6c73 3e2e 3c6c  _set.<locals>.<l
+000028a0: 616d 6264 613e a902 722a 0000 0072 3800  ambda>..r*...r8.
+000028b0: 0000 72ab 0000 0072 1200 0000 72ab 0000  ..r....r....r...
+000028c0: 0072 1300 0000 72a8 0000 00f7 0000 00f3  .r....r.........
+000028d0: 0200 0000 1c05 72a8 0000 0063 0200 0000  ......r....c....
+000028e0: 0000 0000 0000 0000 0200 0000 0600 0000  ................
+000028f0: 0300 0000 72a7 0000 0029 057a 3e20 4578  ....r....).z> Ex
+00002900: 7465 726e 616c 2044 6174 6120 5374 6f72  ternal Data Stor
+00002910: 653a 2047 6574 2073 6574 7469 6e67 7320  e: Get settings 
+00002920: 7265 6c61 7465 6420 746f 2074 6865 2072  related to the r
+00002930: 6570 6f73 6974 6f72 792e 2072 3000 0000  epository. r0...
+00002940: da0e 7265 706f 7369 746f 7279 5f67 6574  ..repository_get
+00002950: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00002960: 0003 0000 0013 0000 0072 a900 0000 721a  .........r....r.
+00002970: 0000 00a9 0172 9300 0000 7232 0000 0072  .....r....r2...r
+00002980: ab00 0000 7212 0000 0072 1300 0000 7236  ....r....r....r6
+00002990: 0000 0004 0100 0072 3700 0000 7a20 7265  .......r7...z re
+000029a0: 706f 7369 746f 7279 5f67 6574 2e3c 6c6f  pository_get.<lo
+000029b0: 6361 6c73 3e2e 3c6c 616d 6264 613e 72ac  cals>.<lambda>r.
+000029c0: 0000 0072 ab00 0000 7212 0000 0072 ab00  ...r....r....r..
+000029d0: 0000 7213 0000 0072 ae00 0000 ff00 0000  ..r....r........
+000029e0: 72ad 0000 0072 ae00 0000 da05 636c 6561  r....r......clea
+000029f0: 7263 0200 0000 0000 0000 0000 0000 0200  rc..............
+00002a00: 0000 0600 0000 0300 0000 72a7 0000 0029  ..........r....)
+00002a10: 057a 4020 4578 7465 726e 616c 2044 6174  .z@ External Dat
+00002a20: 6120 5374 6f72 653a 2043 6c65 6172 2073  a Store: Clear s
+00002a30: 6574 7469 6e67 7320 7265 6c61 7465 6420  ettings related 
+00002a40: 746f 2074 6865 2072 6570 6f73 6974 6f72  to the repositor
+00002a50: 792e 2072 3000 0000 da10 7265 706f 7369  y. r0.....reposi
+00002a60: 746f 7279 5f63 6c65 6172 6301 0000 0000  tory_clearc.....
+00002a70: 0000 0000 0000 0001 0000 0003 0000 0013  ................
+00002a80: 0000 0072 a900 0000 721a 0000 00a9 0172  ...r....r......r
+00002a90: 9600 0000 7232 0000 0072 ab00 0000 7212  ....r2...r....r.
+00002aa0: 0000 0072 1300 0000 7236 0000 000c 0100  ...r....r6......
+00002ab0: 0072 3700 0000 7a22 7265 706f 7369 746f  .r7...z"reposito
+00002ac0: 7279 5f63 6c65 6172 2e3c 6c6f 6361 6c73  ry_clear.<locals
+00002ad0: 3e2e 3c6c 616d 6264 613e 72ac 0000 0072  >.<lambda>r....r
+00002ae0: ab00 0000 7212 0000 0072 ab00 0000 7213  ....r....r....r.
+00002af0: 0000 0072 b100 0000 0701 0000 72ad 0000  ...r........r...
+00002b00: 0072 b100 0000 7a06 2d73 7061 6365 7a07  .r....z.-spacez.
+00002b10: 2d2d 7370 6163 657a 0a53 7061 6365 2063  --spacez.Space c
+00002b20: 6f64 6529 0272 2300 0000 7225 0000 007a  ode).r#...r%...z
+00002b30: 082d 7072 6f6a 6563 747a 092d 2d70 726f  .-projectz.--pro
+00002b40: 6a65 6374 7a1b 5072 6f6a 6563 7420 6964  jectz.Project id
+00002b50: 656e 7469 6669 6361 7469 6f6e 2063 6f64  entification cod
+00002b60: 657a 0b2d 636f 6c6c 6563 7469 6f6e 7a0c  ez.-collectionz.
+00002b70: 2d2d 636f 6c6c 6563 7469 6f6e 7a0f 436f  --collectionz.Co
+00002b80: 6c6c 6563 7469 6f6e 2063 6f64 657a 032d  llection codez.-
+00002b90: 6964 7a04 2d2d 6964 da0a 6461 7461 7365  idz.--id..datase
+00002ba0: 745f 6964 7a42 4461 7461 7365 7420 6964  t_idzBDataset id
+00002bb0: 656e 7469 6669 6361 7469 6f6e 2069 6e66  entification inf
+00002bc0: 6f72 6d61 7469 6f6e 2c20 6974 2063 616e  ormation, it can
+00002bd0: 2062 6520 7065 726d 4964 206f 7220 6964   be permId or id
+00002be0: 656e 7469 6669 6572 7a05 2d74 7970 657a  entifierz.-typez
+00002bf0: 062d 2d74 7970 65da 0974 7970 655f 636f  .--type..type_co
+00002c00: 6465 7a11 4461 7461 7365 7420 7479 7065  dez.Dataset type
+00002c10: 2063 6f64 657a 092d 7072 6f70 6572 7479   codez.-property
+00002c20: da0d 7072 6f70 6572 7479 5f63 6f64 657a  ..property_codez
+00002c30: 0d50 726f 7065 7274 7920 636f 6465 7a0f  .Property codez.
+00002c40: 2d70 726f 7065 7274 792d 7661 6c75 65da  -property-value.
+00002c50: 0e70 726f 7065 7274 795f 7661 6c75 657a  .property_valuez
+00002c60: 0e50 726f 7065 7274 7920 7661 6c75 657a  .Property valuez
+00002c70: 122d 7265 6769 7374 7261 7469 6f6e 2d64  .-registration-d
+00002c80: 6174 657a 132d 2d72 6567 6973 7472 6174  atez.--registrat
+00002c90: 696f 6e2d 6461 7465 da11 7265 6769 7374  ion-date..regist
+00002ca0: 7261 7469 6f6e 5f64 6174 657a 4d52 6567  ration_datezMReg
+00002cb0: 6973 7472 6174 696f 6e20 6461 7465 2c20  istration date, 
+00002cc0: 6974 2063 616e 2062 6520 696e 2074 6865  it can be in the
+00002cd0: 2066 6f72 6d61 7420 226f 5959 5959 2d4d   format "oYYYY-M
+00002ce0: 4d2d 4444 2220 2865 2e67 2e20 223e 3230  M-DD" (e.g. ">20
+00002cf0: 3233 2d30 312d 3031 2229 7a12 2d6d 6f64  23-01-01")z.-mod
+00002d00: 6966 6963 6174 696f 6e2d 6461 7465 7a13  ification-datez.
+00002d10: 2d2d 6d6f 6469 6669 6361 7469 6f6e 2d64  --modification-d
+00002d20: 6174 65da 116d 6f64 6966 6963 6174 696f  ate..modificatio
+00002d30: 6e5f 6461 7465 7a4d 4d6f 6469 6669 6361  n_datezMModifica
+00002d40: 7469 6f6e 2064 6174 652c 2069 7420 6361  tion date, it ca
+00002d50: 6e20 6265 2069 6e20 7468 6520 666f 726d  n be in the form
+00002d60: 6174 2022 6f59 5959 592d 4d4d 2d44 4422  at "oYYYY-MM-DD"
+00002d70: 2028 652e 672e 2022 3e32 3032 332d 3031   (e.g. ">2023-01
+00002d80: 2d30 3122 297a 052d 7361 7665 7a06 2d2d  -01")z.-savez.--
+00002d90: 7361 7665 7a18 4669 6c65 6e61 6d65 2074  savez.Filename t
+00002da0: 6f20 7361 7665 2072 6573 756c 7473 7a02  o save resultsz.
+00002db0: 2d72 7a0b 2d2d 7265 6375 7273 6976 65da  -rz.--recursive.
+00002dc0: 0972 6563 7572 7369 7665 7a17 5365 6172  .recursivez.Sear
+00002dd0: 6368 2064 6174 6120 7265 6375 7273 6976  ch data recursiv
+00002de0: 656c 7929 0372 2400 0000 7223 0000 0072  ely).r$...r#...r
+00002df0: 2500 0000 7a0c 2d6f 626a 6563 742d 7479  %...z.-object-ty
+00002e00: 7065 7a0d 2d2d 6f62 6a65 6374 2d74 7970  pez.--object-typ
+00002e10: 65da 106f 626a 6563 745f 7479 7065 5f63  e..object_type_c
+00002e20: 6f64 657a 1d4f 626a 6563 7420 7479 7065  odez.Object type
+00002e30: 2063 6f64 6520 746f 2066 696c 7465 7220   code to filter 
+00002e40: 6279 7a0d 2d6f 626a 6563 742d 7370 6163  byz.-object-spac
+00002e50: 657a 0e2d 2d6f 626a 6563 742d 7370 6163  ez.--object-spac
+00002e60: 65da 0c6f 626a 6563 745f 7370 6163 657a  e..object_spacez
+00002e70: 114f 626a 6563 7420 7370 6163 6520 636f  .Object space co
+00002e80: 6465 7a0f 2d6f 626a 6563 742d 7072 6f6a  dez.-object-proj
+00002e90: 6563 747a 102d 2d6f 626a 6563 742d 7072  ectz.--object-pr
+00002ea0: 6f6a 6563 74da 0e6f 626a 6563 745f 7072  oject..object_pr
+00002eb0: 6f6a 6563 747a 2746 756c 6c20 6f62 6a65  ojectz'Full obje
+00002ec0: 6374 2070 726f 6a65 6374 2069 6465 6e74  ct project ident
+00002ed0: 6966 6963 6174 696f 6e20 636f 6465 7a12  ification codez.
+00002ee0: 2d6f 626a 6563 742d 636f 6c6c 6563 7469  -object-collecti
+00002ef0: 6f6e 7a13 2d2d 6f62 6a65 6374 2d63 6f6c  onz.--object-col
+00002f00: 6c65 6374 696f 6eda 116f 626a 6563 745f  lection..object_
+00002f10: 636f 6c6c 6563 7469 6f6e 7a1b 4675 6c6c  collectionz.Full
+00002f20: 206f 626a 6563 7420 636f 6c6c 6563 7469   object collecti
+00002f30: 6f6e 2063 6f64 657a 0a2d 6f62 6a65 6374  on codez.-object
+00002f40: 2d69 647a 0b2d 2d6f 626a 6563 742d 6964  -idz.--object-id
+00002f50: da09 6f62 6a65 6374 5f69 647a 414f 626a  ..object_idzAObj
+00002f60: 6563 7420 6964 656e 7469 6669 6361 7469  ect identificati
+00002f70: 6f6e 2069 6e66 6f72 6d61 7469 6f6e 2c20  on information, 
+00002f80: 6974 2063 616e 2062 6520 7065 726d 4964  it can be permId
+00002f90: 206f 7220 6964 656e 7469 6669 6572 7a10   or identifierz.
+00002fa0: 2d6f 626a 6563 742d 7072 6f70 6572 7479  -object-property
+00002fb0: da14 6f62 6a65 6374 5f70 726f 7065 7274  ..object_propert
+00002fc0: 795f 636f 6465 7a14 4f62 6a65 6374 2070  y_codez.Object p
+00002fd0: 726f 7065 7274 7920 636f 6465 7a16 2d6f  roperty codez.-o
+00002fe0: 626a 6563 742d 7072 6f70 6572 7479 2d76  bject-property-v
+00002ff0: 616c 7565 da15 6f62 6a65 6374 5f70 726f  alue..object_pro
+00003000: 7065 7274 795f 7661 6c75 657a 154f 626a  perty_valuez.Obj
+00003010: 6563 7420 7072 6f70 6572 7479 2076 616c  ect property val
+00003020: 7565 7a19 2d6f 626a 6563 742d 7265 6769  uez.-object-regi
+00003030: 7374 7261 7469 6f6e 2d64 6174 657a 1a2d  stration-datez.-
+00003040: 2d6f 626a 6563 742d 7265 6769 7374 7261  -object-registra
+00003050: 7469 6f6e 2d64 6174 65da 186f 626a 6563  tion-date..objec
+00003060: 745f 7265 6769 7374 7261 7469 6f6e 5f64  t_registration_d
+00003070: 6174 657a 192d 6f62 6a65 6374 2d6d 6f64  atez.-object-mod
+00003080: 6966 6963 6174 696f 6e2d 6461 7465 7a1a  ification-datez.
+00003090: 2d2d 6f62 6a65 6374 2d6d 6f64 6966 6963  --object-modific
+000030a0: 6174 696f 6e2d 6461 7465 da18 6f62 6a65  ation-date..obje
+000030b0: 6374 5f6d 6f64 6966 6963 6174 696f 6e5f  ct_modification_
+000030c0: 6461 7465 da08 6461 7461 5f73 6574 7a02  date..data_setz.
+000030d0: 2d70 7a16 2d2d 6973 5f64 6174 615f 7365  -pz.--is_data_se
+000030e0: 745f 7072 6f70 6572 7479 7a1c 436f 6e66  t_propertyz.Conf
+000030f0: 6967 7572 6520 6461 7461 2073 6574 2070  igure data set p
+00003100: 726f 7065 7274 792e 6303 0000 0000 0000  roperty.c.......
+00003110: 0000 0000 0004 0000 0004 0000 0043 0000  .............C..
+00003120: 0073 3a00 0000 7400 7c00 6a01 6401 6402  .s:...t.|.j.d.d.
+00003130: 8d02 7d03 7c01 7c00 6a01 6403 3c00 7c02  ..}.|.|.j.d.<.|.
+00003140: 7c00 6a01 6404 3c00 7c03 7c00 6a01 6405  |.j.d.<.|.|.j.d.
+00003150: 3c00 6406 7c00 6a01 6407 3c00 6408 5300  <.d.|.j.d.<.d.S.
+00003160: 2909 7a40 2045 7874 6572 6e61 6c20 4461  ).z@ External Da
+00003170: 7461 2053 746f 7265 3a20 4765 742f 7365  ta Store: Get/se
+00003180: 7420 7365 7474 696e 6773 2072 656c 6174  t settings relat
+00003190: 6564 2074 6f20 7468 6520 6461 7461 2073  ed to the data s
+000031a0: 6574 2e20 4672 9900 0000 7280 0000 0072  et. Fr....r....r
+000031b0: 8200 0000 7230 0000 0072 c300 0000 7281  ....r0...r....r.
+000031c0: 0000 004e 72a3 0000 0029 0472 2b00 0000  ...Nr....).r+...
+000031d0: 7280 0000 0072 8200 0000 7230 0000 0072  r....r....r0...r
+000031e0: 1200 0000 7212 0000 0072 1300 0000 72c3  ....r....r....r.
+000031f0: 0000 003b 0100 0073 0a00 0000 0e07 0a01  ...;...s........
+00003200: 0a01 0a01 0e01 da11 6461 7461 5f73 6574  ........data_set
+00003210: 5f73 6574 7469 6e67 7363 0200 0000 0000  _settingsc......
+00003220: 0000 0000 0000 0200 0000 0600 0000 0300  ................
+00003230: 0000 72a7 0000 0029 057a 3c20 4578 7465  ..r....).z< Exte
+00003240: 726e 616c 2044 6174 6120 5374 6f72 653a  rnal Data Store:
+00003250: 2053 6574 2073 6574 7469 6e67 7320 7265   Set settings re
+00003260: 6c61 7465 6420 746f 2074 6865 2064 6174  lated to the dat
+00003270: 6120 7365 742e 2072 3000 0000 da0c 6461  a set. r0.....da
+00003280: 7461 5f73 6574 5f73 6574 6301 0000 0000  ta_set_setc.....
+00003290: 0000 0000 0000 0001 0000 0003 0000 0013  ................
+000032a0: 0000 0072 a900 0000 721a 0000 0072 aa00  ...r....r....r..
+000032b0: 0000 7232 0000 00a9 0272 2b00 0000 72c4  ..r2.....r+...r.
+000032c0: 0000 0072 1200 0000 7213 0000 0072 3600  ...r....r....r6.
+000032d0: 0000 4e01 0000 7237 0000 007a 1e64 6174  ..N...r7...z.dat
+000032e0: 615f 7365 745f 7365 742e 3c6c 6f63 616c  a_set_set.<local
+000032f0: 733e 2e3c 6c61 6d62 6461 3e72 ac00 0000  s>.<lambda>r....
+00003300: 72c6 0000 0072 1200 0000 72c6 0000 0072  r....r....r....r
+00003310: 1300 0000 72c5 0000 0049 0100 0072 ad00  ....r....I...r..
+00003320: 0000 72c5 0000 0063 0200 0000 0000 0000  ..r....c........
+00003330: 0000 0000 0200 0000 0600 0000 0300 0000  ................
+00003340: 72a7 0000 0029 057a 3c20 4578 7465 726e  r....).z< Extern
+00003350: 616c 2044 6174 6120 5374 6f72 653a 2047  al Data Store: G
+00003360: 6574 2073 6574 7469 6e67 7320 7265 6c61  et settings rela
+00003370: 7465 6420 746f 2074 6865 2064 6174 6120  ted to the data 
+00003380: 7365 742e 2072 3000 0000 da0c 6461 7461  set. r0.....data
+00003390: 5f73 6574 5f67 6574 6301 0000 0000 0000  _set_getc.......
+000033a0: 0000 0000 0001 0000 0003 0000 0013 0000  ................
+000033b0: 0072 a900 0000 721a 0000 0072 af00 0000  .r....r....r....
+000033c0: 7232 0000 0072 c600 0000 7212 0000 0072  r2...r....r....r
+000033d0: 1300 0000 7236 0000 0056 0100 0072 3700  ....r6...V...r7.
+000033e0: 0000 7a1e 6461 7461 5f73 6574 5f67 6574  ..z.data_set_get
+000033f0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00003400: 613e 72ac 0000 0072 c600 0000 7212 0000  a>r....r....r...
+00003410: 0072 c600 0000 7213 0000 0072 c700 0000  .r....r....r....
+00003420: 5101 0000 72ad 0000 0072 c700 0000 6302  Q...r....r....c.
+00003430: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+00003440: 0000 0003 0000 0072 a700 0000 2905 7a3e  .......r....).z>
+00003450: 2045 7874 6572 6e61 6c20 4461 7461 2053   External Data S
+00003460: 746f 7265 3a20 436c 6561 7220 7365 7474  tore: Clear sett
+00003470: 696e 6773 2072 656c 6174 6564 2074 6f20  ings related to 
+00003480: 7468 6520 6461 7461 2073 6574 2e20 7230  the data set. r0
+00003490: 0000 00da 0e64 6174 615f 7365 745f 636c  .....data_set_cl
+000034a0: 6561 7263 0100 0000 0000 0000 0000 0000  earc............
+000034b0: 0100 0000 0300 0000 1300 0000 72a9 0000  ............r...
+000034c0: 0072 1a00 0000 72b2 0000 0072 3200 0000  .r....r....r2...
+000034d0: 72c6 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+000034e0: 3600 0000 5e01 0000 7237 0000 007a 2064  6...^...r7...z d
+000034f0: 6174 615f 7365 745f 636c 6561 722e 3c6c  ata_set_clear.<l
+00003500: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e72  ocals>.<lambda>r
+00003510: ac00 0000 72c6 0000 0072 1200 0000 72c6  ....r....r....r.
+00003520: 0000 0072 1300 0000 72c8 0000 0059 0100  ...r....r....Y..
+00003530: 0072 ad00 0000 72c8 0000 0063 0200 0000  .r....r....c....
+00003540: 0000 0000 0000 0000 0200 0000 0200 0000  ................
+00003550: 4300 0000 7320 0000 007c 0064 0075 0072  C...s ...|.d.u.r
+00003560: 087c 0164 0075 0170 0f7c 0064 0075 016f  .|.d.u.p.|.d.u.o
+00003570: 0f7c 0164 0075 0053 0072 1a00 0000 7212  .|.d.u.S.r....r.
+00003580: 0000 0029 02da 0670 6172 616d 31da 0670  ...)...param1..p
+00003590: 6172 616d 3272 1200 0000 7212 0000 0072  aram2r....r....r
+000035a0: 1300 0000 da10 5f70 6169 725f 6973 5f6e  ......_pair_is_n
+000035b0: 6f74 5f73 6574 6101 0000 7302 0000 0020  ot_seta...s.... 
+000035c0: 0172 cb00 0000 da06 7365 6172 6368 7a2f  .r......searchz/
+000035d0: 5365 6172 6368 2066 6f72 2064 6174 6173  Search for datas
+000035e0: 6574 7320 7573 696e 6720 6120 6669 6c74  ets using a filt
+000035f0: 6572 696e 6720 6372 6974 6572 6961 2e29  ering criteria.)
+00003600: 01da 0a73 686f 7274 5f68 656c 7063 1500  ...short_helpc..
+00003610: 0000 0000 0000 0000 0000 1600 0000 1100  ................
+00003620: 0000 0300 0000 733c 0100 007c 017c 027c  ......s<...|.|.|
+00003630: 037c 047c 057c 067c 087c 097c 0c7c 0d7c  .|.|.|.|.|.|.|.|
+00003640: 0e7c 0f7c 107c 117c 127c 137c 1467 117d  .|.|.|.|.|.|.g.}
+00003650: 1574 0064 0164 0284 007c 157c 0767 0117  .t.d.d...|.|.g..
+00003660: 0044 0083 0183 0172 2574 0164 0383 0101  .D.....r%t.d....
+00003670: 0064 0453 0074 027c 087c 0983 0273 2f74  .d.S.t.|.|...s/t
+00003680: 027c 117c 1283 0272 3574 0164 0583 0101  .|.|...r5t.d....
+00003690: 0064 0453 0074 037c 006a 0464 0664 078d  .d.S.t.|.j.d.d..
+000036a0: 027c 006a 0464 083c 007c 0764 0975 0172  .|.j.d.<.|.d.u.r
+000036b0: 5674 0564 0a64 0284 007c 1544 0083 0183  Vt.d.d...|.D....
+000036c0: 0172 5074 0164 0b83 0101 0074 067c 0764  .rPt.d.....t.|.d
+000036d0: 0c8d 0189 006e 3874 0664 2169 0064 0d7c  .....n8t.d!i.d.|
+000036e0: 0193 0164 0e7c 0293 0164 0f7c 0393 0164  ...d.|...d.|...d
+000036f0: 107c 0493 0164 117c 0893 0164 127c 0593  .|...d.|...d.|..
+00003700: 0164 137c 0693 0164 147c 0993 0164 157c  .d.|...d.|...d.|
+00003710: 0c93 0164 167c 0d93 0164 177c 0e93 0164  ...d.|...d.|...d
+00003720: 187c 0f93 0164 197c 1093 0164 1a7c 1193  .|...d.|...d.|..
+00003730: 0164 1b7c 1293 0164 1c7c 1393 0164 1d7c  .d.|...d.|...d.|
+00003740: 1493 018e 0189 007c 006a 0464 0819 00a0  .......|.j.d....
+00003750: 0764 1e87 0087 0187 0266 0364 1f64 2084  .d.......f.d.d .
+00003760: 08a1 0266 0153 0029 227a 9453 7461 6e64  ...f.S.)"z.Stand
+00003770: 6172 6420 4461 7461 2053 746f 7265 3a20  ard Data Store: 
+00003780: 5365 6172 6368 2064 6174 6120 7365 7473  Search data sets
+00003790: 2067 6976 656e 2074 6865 2066 696c 7465   given the filte
+000037a0: 7269 6e67 2063 7269 7465 7269 6120 6f72  ring criteria or
+000037b0: 206f 626a 6563 7420 6964 656e 7469 6669   object identifi
+000037c0: 6572 2e0a 2020 2020 5265 7375 6c74 7320  er..    Results 
+000037d0: 6f66 2074 6869 7320 636f 6d6d 616e 6420  of this command 
+000037e0: 6361 6e20 6265 2075 7365 6420 696e 2060  can be used in `
+000037f0: 6f62 6973 2064 6f77 6e6c 6f61 6460 2e63  obis download`.c
+00003800: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00003810: 0300 0000 7300 0000 f318 0000 0081 007c  ....s..........|
+00003820: 005d 077d 017c 0164 0075 0056 0001 0071  .].}.|.d.u.V...q
+00003830: 0264 0053 0072 1a00 0000 7212 0000 00a9  .d.S.r....r.....
+00003840: 02da 022e 30da 0176 7212 0000 0072 1200  ....0..vr....r..
+00003850: 0000 7213 0000 00da 093c 6765 6e65 7870  ..r......<genexp
+00003860: 723e 7401 0000 f304 0000 0002 8016 007a  r>t............z
+00003870: 2264 6174 615f 7365 745f 7365 6172 6368  "data_set_search
+00003880: 2e3c 6c6f 6361 6c73 3e2e 3c67 656e 6578  .<locals>.<genex
+00003890: 7072 3efa 3159 6f75 206d 7573 7420 7072  pr>.1You must pr
+000038a0: 6f76 6964 6520 6174 206c 6561 7374 206f  ovide at least o
+000038b0: 6e65 2066 696c 7465 7269 6e67 2063 7269  ne filtering cri
+000038c0: 7465 7269 6121 723b 0000 007a 3c50 726f  teria!r;...z<Pro
+000038d0: 7065 7274 7920 636f 6465 2061 6e64 2070  perty code and p
+000038e0: 726f 7065 7274 7920 7661 6c75 6520 7061  roperty value pa
+000038f0: 6972 206e 6565 6473 2074 6f20 6265 2073  ir needs to be s
+00003900: 7065 6369 6669 6564 2146 7299 0000 0072  pecified!Fr....r
+00003910: 3000 0000 4e63 0100 0000 0000 0000 0000  0...Nc..........
+00003920: 0000 0200 0000 0300 0000 7300 0000 f318  ..........s.....
+00003930: 0000 0081 007c 005d 077d 017c 0164 0075  .....|.].}.|.d.u
+00003940: 0156 0001 0071 0264 0053 0072 1a00 0000  .V...q.d.S.r....
+00003950: 7212 0000 0072 cf00 0000 7212 0000 0072  r....r....r....r
+00003960: 1200 0000 7213 0000 0072 d200 0000 7d01  ....r....r....}.
+00003970: 0000 72d3 0000 007a 4944 6174 6173 6574  ..r....zIDataset
+00003980: 2069 6420 7061 7261 6d65 7465 7220 6465   id parameter de
+00003990: 7465 6374 6564 2120 4f74 6865 7220 6669  tected! Other fi
+000039a0: 6c74 6572 696e 6720 6172 6775 6d65 6e74  ltering argument
+000039b0: 7320 7769 6c6c 2062 6520 6f6d 6974 7465  s will be omitte
+000039c0: 6421 2901 72b3 0000 0072 b400 0000 da05  d!).r....r......
+000039d0: 7370 6163 65da 0770 726f 6a65 6374 da0a  space..project..
+000039e0: 6578 7065 7269 6d65 6e74 72b5 0000 0072  experimentr....r
+000039f0: b700 0000 72b8 0000 0072 b600 0000 72ba  ....r....r....r.
+00003a00: 0000 0072 bb00 0000 72bc 0000 0072 bd00  ...r....r....r..
+00003a10: 0000 72be 0000 0072 bf00 0000 72c0 0000  ..r....r....r...
+00003a20: 0072 c100 0000 72c2 0000 00da 0f64 6174  .r....r......dat
+00003a30: 615f 7365 745f 7365 6172 6368 6301 0000  a_set_searchc...
+00003a40: 0000 0000 0000 0000 0001 0000 0005 0000  ................
+00003a50: 0013 0000 00f3 0e00 0000 7c00 a000 8800  ..........|.....
+00003a60: 8801 8802 a103 5300 721a 0000 0029 01da  ......S.r....)..
+00003a70: 0f73 6561 7263 685f 6461 7461 5f73 6574  .search_data_set
+00003a80: 7232 0000 00a9 03da 0766 696c 7465 7273  r2.......filters
+00003a90: 72b9 0000 00da 0473 6176 6572 1200 0000  r......saver....
+00003aa0: 7213 0000 0072 3600 0000 8c01 0000 f302  r....r6.........
+00003ab0: 0000 000e 007a 2164 6174 615f 7365 745f  .....z!data_set_
+00003ac0: 7365 6172 6368 2e3c 6c6f 6361 6c73 3e2e  search.<locals>.
+00003ad0: 3c6c 616d 6264 613e 7212 0000 0029 08da  <lambda>r....)..
+00003ae0: 0361 6c6c 7208 0000 0072 cb00 0000 7209  .allr....r....r.
+00003af0: 0000 0072 2a00 0000 da03 616e 79da 0464  ...r*.....any..d
+00003b00: 6963 7472 3800 0000 2916 722b 0000 0072  ictr8...).r+...r
+00003b10: b400 0000 72d6 0000 0072 d700 0000 da0a  ....r....r......
+00003b20: 636f 6c6c 6563 7469 6f6e 72b7 0000 0072  collectionr....r
+00003b30: b800 0000 72b3 0000 0072 b500 0000 72b6  ....r....r....r.
+00003b40: 0000 0072 de00 0000 72b9 0000 0072 ba00  ...r....r....r..
+00003b50: 0000 72bb 0000 0072 bc00 0000 72bd 0000  ..r....r....r...
+00003b60: 0072 be00 0000 72bf 0000 0072 c000 0000  .r....r....r....
+00003b70: 72c1 0000 0072 c200 0000 da13 6669 6c74  r....r......filt
+00003b80: 6572 696e 675f 6172 6775 6d65 6e74 7372  ering_argumentsr
+00003b90: 1200 0000 72dc 0000 0072 1300 0000 72d9  ....r....r....r.
+00003ba0: 0000 0065 0100 0073 6a00 0000 0a0a 0601  ...e...sj.......
+00003bb0: 0801 0601 0401 04fc 1805 0801 0401 0e01  ................
+00003bc0: 0201 04ff 0802 0401 1401 0801 1201 0801  ................
+00003bd0: 0c01 1402 0401 02ff 0401 02ff 0401 02ff  ................
+00003be0: 0402 02fe 0402 02fe 0403 02fd 0403 02fd  ................
+00003bf0: 0404 02fc 0404 02fc 0405 02fb 0405 02fb  ................
+00003c00: 0406 02fa 0407 02f9 0408 02f8 0409 04f7  ................
+00003c10: 0c0a 0e01 06ff 72d9 0000 0063 0200 0000  ......r....c....
+00003c20: 0000 0000 0000 0000 0300 0000 0400 0000  ................
+00003c30: 4300 0000 72a2 0000 0029 087a 9e20 4578  C...r....).z. Ex
+00003c40: 7465 726e 616c 2044 6174 6120 5374 6f72  ternal Data Stor
+00003c50: 653a 2047 6574 2f73 6574 2070 726f 7065  e: Get/set prope
+00003c60: 7274 6965 7320 7265 6c61 7465 6420 746f  rties related to
+00003c70: 2074 6865 206f 626a 6563 742e 0a0a 2020   the object...  
+00003c80: 2020 5374 616e 6461 7264 2044 6174 6120    Standard Data 
+00003c90: 5374 6f72 653a 2047 6574 2f73 6574 2070  Store: Get/set p
+00003ca0: 726f 7065 7274 6965 7320 6f66 206f 626a  roperties of obj
+00003cb0: 6563 7473 2063 6f6e 6e65 6374 6564 2074  ects connected t
+00003cc0: 6f20 646f 776e 6c6f 6164 6564 2064 6174  o downloaded dat
+00003cd0: 6173 6574 732e 0a20 2020 2046 7299 0000  asets..    Fr...
+00003ce0: 0072 8000 0000 7230 0000 00da 066f 626a  .r....r0.....obj
+00003cf0: 6563 7472 8100 0000 4e72 a300 0000 72a4  ectr....Nr....r.
+00003d00: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+00003d10: 0000 72e5 0000 0092 0100 00f3 0800 0000  ..r.............
+00003d20: 0e08 0a01 0a01 0e01 72e5 0000 00da 0f6f  ........r......o
+00003d30: 626a 6563 745f 7365 7474 696e 6773 6302  bject_settingsc.
+00003d40: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+00003d50: 0000 0003 0000 0072 a700 0000 2905 7a98  .......r....).z.
+00003d60: 2045 7874 6572 6e61 6c20 4461 7461 2053   External Data S
+00003d70: 746f 7265 3a20 5365 7420 7072 6f70 6572  tore: Set proper
+00003d80: 7469 6573 2072 656c 6174 6564 2074 6f20  ties related to 
+00003d90: 7468 6520 6f62 6a65 6374 2e0a 0a20 2020  the object...   
+00003da0: 2053 7461 6e64 6172 6420 4461 7461 2053   Standard Data S
+00003db0: 746f 7265 3a20 5365 7420 7072 6f70 6572  tore: Set proper
+00003dc0: 7479 2074 6f20 616c 6c20 6f62 6a65 6374  ty to all object
+00003dd0: 7320 636f 6e6e 6563 7465 6420 746f 2064  s connected to d
+00003de0: 6f77 6e6c 6f61 6465 6420 6461 7461 7365  ownloaded datase
+00003df0: 7473 2e0a 2020 2020 7230 0000 00da 0a6f  ts..    r0.....o
+00003e00: 626a 6563 745f 7365 7463 0100 0000 0000  bject_setc......
+00003e10: 0000 0000 0000 0100 0000 0300 0000 1300  ................
+00003e20: 0000 72a9 0000 0072 1a00 0000 72aa 0000  ..r....r....r...
+00003e30: 0072 3200 0000 a902 722b 0000 0072 e700  .r2.....r+...r..
+00003e40: 0000 7212 0000 0072 1300 0000 7236 0000  ..r....r....r6..
+00003e50: 00a8 0100 0072 3700 0000 7a1c 6f62 6a65  .....r7...z.obje
+00003e60: 6374 5f73 6574 2e3c 6c6f 6361 6c73 3e2e  ct_set.<locals>.
+00003e70: 3c6c 616d 6264 613e 72ac 0000 0072 e900  <lambda>r....r..
+00003e80: 0000 7212 0000 0072 e900 0000 7213 0000  ..r....r....r...
+00003e90: 0072 e800 0000 a001 0000 f302 0000 001c  .r..............
+00003ea0: 0872 e800 0000 6302 0000 0000 0000 0000  .r....c.........
+00003eb0: 0000 0002 0000 0006 0000 0003 0000 0072  ...............r
+00003ec0: a700 0000 2905 7aa0 2045 7874 6572 6e61  ....).z. Externa
+00003ed0: 6c20 4461 7461 2053 746f 7265 3a20 5365  l Data Store: Se
+00003ee0: 7420 7072 6f70 6572 7469 6573 2072 656c  t properties rel
+00003ef0: 6174 6564 2074 6f20 7468 6520 6f62 6a65  ated to the obje
+00003f00: 6374 2e0a 0a20 2020 2053 7461 6e64 6172  ct...    Standar
+00003f10: 6420 4461 7461 2053 746f 7265 3a20 4765  d Data Store: Ge
+00003f20: 7420 6769 7665 6e20 7072 6f70 6572 7469  t given properti
+00003f30: 6573 206f 6620 616c 6c20 6f62 6a65 6374  es of all object
+00003f40: 7320 636f 6e6e 6563 7465 6420 746f 2064  s connected to d
+00003f50: 6f77 6e6c 6f61 6465 6420 6461 7461 7365  ownloaded datase
+00003f60: 7473 2e0a 2020 2020 7230 0000 00da 0a6f  ts..    r0.....o
+00003f70: 626a 6563 745f 6765 7463 0100 0000 0000  bject_getc......
+00003f80: 0000 0000 0000 0100 0000 0300 0000 1300  ................
+00003f90: 0000 72a9 0000 0072 1a00 0000 72af 0000  ..r....r....r...
+00003fa0: 0072 3200 0000 72e9 0000 0072 1200 0000  .r2...r....r....
+00003fb0: 7213 0000 0072 3600 0000 b301 0000 7237  r....r6.......r7
+00003fc0: 0000 007a 1c6f 626a 6563 745f 6765 742e  ...z.object_get.
+00003fd0: 3c6c 6f63 616c 733e 2e3c 6c61 6d62 6461  <locals>.<lambda
+00003fe0: 3e72 ac00 0000 72e9 0000 0072 1200 0000  >r....r....r....
+00003ff0: 72e9 0000 0072 1300 0000 72eb 0000 00ab  r....r....r.....
+00004000: 0100 0072 ea00 0000 72eb 0000 0063 0200  ...r....r....c..
+00004010: 0000 0000 0000 0000 0000 0200 0000 0600  ................
+00004020: 0000 0300 0000 72a7 0000 0029 057a 3e20  ......r....).z> 
+00004030: 4578 7465 726e 616c 2044 6174 6120 5374  External Data St
+00004040: 6f72 653a 2043 6c65 6172 2070 726f 7065  ore: Clear prope
+00004050: 7274 6965 7320 7265 6c61 7465 6420 746f  rties related to
+00004060: 2074 6865 206f 626a 6563 742e 2072 3000   the object. r0.
+00004070: 0000 da0c 6f62 6a65 6374 5f63 6c65 6172  ....object_clear
+00004080: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00004090: 0003 0000 0013 0000 0072 a900 0000 721a  .........r....r.
+000040a0: 0000 0072 b200 0000 7232 0000 0072 e900  ...r....r2...r..
+000040b0: 0000 7212 0000 0072 1300 0000 7236 0000  ..r....r....r6..
+000040c0: 00bb 0100 0072 3700 0000 7a1e 6f62 6a65  .....r7...z.obje
+000040d0: 6374 5f63 6c65 6172 2e3c 6c6f 6361 6c73  ct_clear.<locals
+000040e0: 3e2e 3c6c 616d 6264 613e 72ac 0000 0072  >.<lambda>r....r
+000040f0: e900 0000 7212 0000 0072 e900 0000 7213  ....r....r....r.
+00004100: 0000 0072 ec00 0000 b601 0000 72ad 0000  ...r........r...
+00004110: 0072 ec00 0000 7a20 4675 6c6c 2070 726f  .r....z Full pro
+00004120: 6a65 6374 2069 6465 6e74 6966 6963 6174  ject identificat
+00004130: 696f 6e20 636f 6465 7a14 4675 6c6c 2063  ion codez.Full c
+00004140: 6f6c 6c65 6374 696f 6e20 636f 6465 7a07  ollection codez.
+00004150: 2d6f 626a 6563 747a 082d 2d6f 626a 6563  -objectz.--objec
+00004160: 747a 0954 7970 6520 636f 6465 7a2e 5365  tz.Type codez.Se
+00004170: 6172 6368 2066 6f72 206f 626a 6563 7473  arch for objects
+00004180: 2075 7369 6e67 2061 2066 696c 7465 7269   using a filteri
+00004190: 6e67 2063 7269 7465 7269 612e 630c 0000  ng criteria.c...
+000041a0: 0000 0000 0000 0000 000d 0000 000a 0000  ................
+000041b0: 0003 0000 0073 dc00 0000 7c01 7c02 7c03  .....s....|.|.|.
+000041c0: 7c04 7c05 7c06 7c08 7c09 6708 7d0c 7400  |.|.|.|.|.g.}.t.
+000041d0: 6401 6402 8400 7c0c 7c07 6701 1700 4400  d.d...|.|.g...D.
+000041e0: 8301 8301 721c 7401 6403 8301 0100 6404  ....r.t.d.....d.
+000041f0: 5300 7c08 6405 7500 7224 7c09 6405 7501  S.|.d.u.r$|.d.u.
+00004200: 732c 7c08 6405 7501 7232 7c09 6405 7500  s,|.d.u.r2|.d.u.
+00004210: 7232 7401 6406 8301 0100 6404 5300 7402  r2t.d.....d.S.t.
+00004220: 7c00 6a03 6407 6408 8d02 7c00 6a03 6409  |.j.d.d...|.j.d.
+00004230: 3c00 7c07 6405 7501 7253 7404 640a 6402  <.|.d.u.rSt.d.d.
+00004240: 8400 7c0c 4400 8301 8301 724d 7401 640b  ..|.D.....rMt.d.
+00004250: 8301 0100 7405 7c07 640c 8d01 8900 6e0c  ....t.|.d.....n.
+00004260: 7405 7c01 7c02 7c03 7c04 7c08 7c05 7c06  t.|.|.|.|.|.|.|.
+00004270: 7c09 640d 8d08 8900 7c00 6a03 6409 1900  |.d.....|.j.d...
+00004280: a006 640e 8700 8701 8702 6603 640f 6410  ..d.......f.d.d.
+00004290: 8408 a102 5300 2911 7a58 5374 616e 6461  ....S.).zXStanda
+000042a0: 7264 2044 6174 6120 5374 6f72 653a 2053  rd Data Store: S
+000042b0: 6561 7263 6820 666f 7220 6f62 6a65 6374  earch for object
+000042c0: 7320 7573 696e 6720 6120 6669 6c74 6572  s using a filter
+000042d0: 696e 6720 6372 6974 6572 6961 206f 7220  ing criteria or 
+000042e0: 6f62 6a65 6374 2069 6465 6e74 6966 6965  object identifie
+000042f0: 722e 6301 0000 0000 0000 0000 0000 0002  r.c.............
+00004300: 0000 0003 0000 0073 0000 0072 ce00 0000  .......s...r....
+00004310: 721a 0000 0072 1200 0000 72cf 0000 0072  r....r....r....r
+00004320: 1200 0000 7212 0000 0072 1300 0000 72d2  ....r....r....r.
+00004330: 0000 00da 0100 0072 d300 0000 7a20 6f62  .......r....z ob
+00004340: 6a65 6374 5f73 6561 7263 682e 3c6c 6f63  ject_search.<loc
+00004350: 616c 733e 2e3c 6765 6e65 7870 723e 72d4  als>.<genexpr>r.
+00004360: 0000 0072 3b00 0000 4e7a 3650 726f 7065  ...r;...Nz6Prope
+00004370: 7274 7920 636f 6465 2061 6e64 2070 726f  rty code and pro
+00004380: 7065 7274 7920 7661 6c75 6520 6e65 6564  perty value need
+00004390: 2074 6f20 6265 2073 7065 6369 6669 6564   to be specified
+000043a0: 2146 7299 0000 0072 3000 0000 6301 0000  !Fr....r0...c...
+000043b0: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+000043c0: 0073 0000 0072 d500 0000 721a 0000 0072  .s...r....r....r
+000043d0: 1200 0000 72cf 0000 0072 1200 0000 7212  ....r....r....r.
+000043e0: 0000 0072 1300 0000 72d2 0000 00e3 0100  ...r....r.......
+000043f0: 0072 d300 0000 7a45 4f62 6a65 6374 2070  .r....zEObject p
+00004400: 6172 616d 6574 6572 2064 6574 6563 7465  arameter detecte
+00004410: 6421 204f 7468 6572 2066 696c 7465 7269  d! Other filteri
+00004420: 6e67 2061 7267 756d 656e 7473 2077 696c  ng arguments wil
+00004430: 6c20 6265 206f 6d69 7474 6564 2129 01da  l be omitted!)..
+00004440: 0b6f 626a 6563 745f 636f 6465 2908 72b4  .object_code).r.
+00004450: 0000 0072 d600 0000 72d7 0000 0072 e300  ...r....r....r..
+00004460: 0000 72b5 0000 0072 b700 0000 72b8 0000  ..r....r....r...
+00004470: 0072 b600 0000 da0d 6f62 6a65 6374 5f73  .r......object_s
+00004480: 6561 7263 6863 0100 0000 0000 0000 0000  earchc..........
+00004490: 0000 0100 0000 0500 0000 1300 0000 72da  ..............r.
+000044a0: 0000 0072 1a00 0000 2901 da0d 7365 6172  ...r....)...sear
+000044b0: 6368 5f6f 626a 6563 7472 3200 0000 72dc  ch_objectr2...r.
+000044c0: 0000 0072 1200 0000 7213 0000 0072 3600  ...r....r....r6.
+000044d0: 0000 ec01 0000 72df 0000 007a 1f6f 626a  ......r....z.obj
+000044e0: 6563 745f 7365 6172 6368 2e3c 6c6f 6361  ect_search.<loca
+000044f0: 6c73 3e2e 3c6c 616d 6264 613e 2907 72e0  ls>.<lambda>).r.
+00004500: 0000 0072 0800 0000 7209 0000 0072 2a00  ...r....r....r*.
+00004510: 0000 72e1 0000 0072 e200 0000 7238 0000  ..r....r....r8..
+00004520: 0029 0d72 2b00 0000 72b4 0000 0072 d600  .).r+...r....r..
+00004530: 0000 72d7 0000 0072 e300 0000 72b7 0000  ..r....r....r...
+00004540: 0072 b800 0000 72be 0000 0072 b500 0000  .r....r....r....
+00004550: 72b6 0000 0072 de00 0000 72b9 0000 0072  r....r....r....r
+00004560: e400 0000 7212 0000 0072 dc00 0000 7213  ....r....r....r.
+00004570: 0000 0072 ee00 0000 d201 0000 732e 0000  ...r........s...
+00004580: 000a 0606 0104 ff18 0208 0104 0110 0110  ................
+00004590: 0108 0104 0114 0108 0112 0108 010c 0106  ................
+000045a0: 0206 0104 0102 0106 fd0c 040e 0104 ff72  ...............r
+000045b0: ee00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+000045c0: 0003 0000 0004 0000 0043 0000 0072 a200  .........C...r..
+000045d0: 0000 2908 7aa8 2045 7874 6572 6e61 6c20  ..).z. External 
+000045e0: 4461 7461 2053 746f 7265 3a20 4765 742f  Data Store: Get/
+000045f0: 7365 7420 7365 7474 696e 6773 2072 656c  set settings rel
+00004600: 6174 6564 2074 6f20 7468 6520 636f 6c6c  ated to the coll
+00004610: 6563 7469 6f6e 2e0a 0a20 2020 2053 7461  ection...    Sta
+00004620: 6e64 6172 6420 4461 7461 2053 746f 7265  ndard Data Store
+00004630: 3a20 4765 742f 7365 7420 7072 6f70 6572  : Get/set proper
+00004640: 7469 6573 206f 6620 616c 6c20 636f 6c6c  ties of all coll
+00004650: 6563 7469 6f6e 7320 636f 6e6e 6563 7465  ections connecte
+00004660: 6420 746f 2064 6f77 6e6c 6f61 6465 6420  d to downloaded 
+00004670: 6461 7461 7365 7473 2e0a 2020 2020 4672  datasets..    Fr
+00004680: 9900 0000 7280 0000 0072 3000 0000 72e3  ....r....r0...r.
+00004690: 0000 0072 8100 0000 4e72 a300 0000 72a4  ...r....Nr....r.
+000046a0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+000046b0: 0000 72e3 0000 00f2 0100 0072 e600 0000  ..r........r....
+000046c0: 72e3 0000 0063 0200 0000 0000 0000 0000  r....c..........
+000046d0: 0000 0200 0000 0600 0000 0300 0000 72a7  ..............r.
+000046e0: 0000 0029 057a a620 4578 7465 726e 616c  ...).z. External
+000046f0: 2044 6174 6120 5374 6f72 653a 2053 6574   Data Store: Set
+00004700: 2073 6574 7469 6e67 7320 7265 6c61 7465   settings relate
+00004710: 6420 746f 2074 6865 2063 6f6c 6c65 6374  d to the collect
+00004720: 696f 6e2e 0a0a 2020 2020 5374 616e 6461  ion...    Standa
+00004730: 7264 2044 6174 6120 5374 6f72 653a 2053  rd Data Store: S
+00004740: 6574 2067 6976 656e 2070 726f 7065 7274  et given propert
+00004750: 6965 7320 6f66 2061 6c6c 2063 6f6c 6c65  ies of all colle
+00004760: 6374 696f 6e73 2063 6f6e 6e65 6374 6564  ctions connected
+00004770: 2074 6f20 646f 776e 6c6f 6164 6564 2064   to downloaded d
+00004780: 6174 6173 6574 732e 0a20 2020 2072 3000  atasets..    r0.
+00004790: 0000 da0e 636f 6c6c 6563 7469 6f6e 5f73  ....collection_s
+000047a0: 6574 6301 0000 0000 0000 0000 0000 0001  etc.............
+000047b0: 0000 0003 0000 0013 0000 0072 a900 0000  ...........r....
+000047c0: 721a 0000 0072 aa00 0000 7232 0000 0072  r....r....r2...r
+000047d0: ab00 0000 7212 0000 0072 1300 0000 7236  ....r....r....r6
+000047e0: 0000 0008 0200 0072 3700 0000 7a20 636f  .......r7...z co
+000047f0: 6c6c 6563 7469 6f6e 5f73 6574 2e3c 6c6f  llection_set.<lo
+00004800: 6361 6c73 3e2e 3c6c 616d 6264 613e 72ac  cals>.<lambda>r.
+00004810: 0000 0072 ab00 0000 7212 0000 0072 ab00  ...r....r....r..
+00004820: 0000 7213 0000 0072 f000 0000 0002 0000  ..r....r........
+00004830: 72ea 0000 0072 f000 0000 6302 0000 0000  r....r....c.....
+00004840: 0000 0000 0000 0002 0000 0006 0000 0003  ................
+00004850: 0000 0072 a700 0000 2905 7aa6 2045 7874  ...r....).z. Ext
+00004860: 6572 6e61 6c20 4461 7461 2053 746f 7265  ernal Data Store
+00004870: 3a20 4765 7420 7365 7474 696e 6773 2072  : Get settings r
+00004880: 656c 6174 6564 2074 6f20 7468 6520 636f  elated to the co
+00004890: 6c6c 6563 7469 6f6e 2e0a 0a20 2020 2053  llection...    S
+000048a0: 7461 6e64 6172 6420 4461 7461 2053 746f  tandard Data Sto
+000048b0: 7265 3a20 4765 7420 6769 7665 6e20 7072  re: Get given pr
+000048c0: 6f70 6572 7469 6573 206f 6620 616c 6c20  operties of all 
+000048d0: 636f 6c6c 6563 7469 6f6e 7320 636f 6e6e  collections conn
+000048e0: 6563 7465 6420 746f 2064 6f77 6e6c 6f61  ected to downloa
+000048f0: 6465 6420 6461 7461 7365 7473 2e0a 2020  ded datasets..  
+00004900: 2020 7230 0000 00da 0e63 6f6c 6c65 6374    r0.....collect
+00004910: 696f 6e5f 6765 7463 0100 0000 0000 0000  ion_getc........
+00004920: 0000 0000 0100 0000 0300 0000 1300 0000  ................
+00004930: 72a9 0000 0072 1a00 0000 72af 0000 0072  r....r....r....r
+00004940: 3200 0000 72ab 0000 0072 1200 0000 7213  2...r....r....r.
+00004950: 0000 0072 3600 0000 1302 0000 7237 0000  ...r6.......r7..
+00004960: 007a 2063 6f6c 6c65 6374 696f 6e5f 6765  .z collection_ge
+00004970: 742e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  t.<locals>.<lamb
+00004980: 6461 3e72 ac00 0000 72ab 0000 0072 1200  da>r....r....r..
+00004990: 0000 72ab 0000 0072 1300 0000 72f1 0000  ..r....r....r...
+000049a0: 000b 0200 0072 ea00 0000 72f1 0000 0063  .....r....r....c
+000049b0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000049c0: 0600 0000 0300 0000 72a7 0000 0029 057a  ........r....).z
+000049d0: 3e45 7874 6572 6e61 6c20 4461 7461 2053  >External Data S
+000049e0: 746f 7265 3a20 436c 6561 7220 7365 7474  tore: Clear sett
+000049f0: 696e 6773 2072 656c 6174 6564 2074 6f20  ings related to 
+00004a00: 7468 6520 636f 6c6c 6563 7469 6f6e 2e72  the collection.r
+00004a10: 3000 0000 da10 636f 6c6c 6563 7469 6f6e  0.....collection
+00004a20: 5f63 6c65 6172 6301 0000 0000 0000 0000  _clearc.........
+00004a30: 0000 0001 0000 0003 0000 0013 0000 0072  ...............r
+00004a40: a900 0000 721a 0000 0072 b200 0000 7232  ....r....r....r2
+00004a50: 0000 0072 ab00 0000 7212 0000 0072 1300  ...r....r....r..
+00004a60: 0000 7236 0000 001b 0200 0072 3700 0000  ..r6.......r7...
+00004a70: 7a22 636f 6c6c 6563 7469 6f6e 5f63 6c65  z"collection_cle
+00004a80: 6172 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  ar.<locals>.<lam
+00004a90: 6264 613e 72ac 0000 0072 ab00 0000 7212  bda>r....r....r.
+00004aa0: 0000 0072 ab00 0000 7213 0000 0072 f200  ...r....r....r..
+00004ab0: 0000 1602 0000 72ad 0000 0072 f200 0000  ......r....r....
+00004ac0: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00004ad0: 0005 0000 0043 0000 0073 4a00 0000 7c01  .....C...sJ...|.
+00004ae0: 6401 7500 720d 7400 7c00 6a01 6402 6401  d.u.r.t.|.j.d.d.
+00004af0: 6403 8d03 7d02 6e07 7400 7c00 6a01 6402  d...}.n.t.|.j.d.
+00004b00: 6404 8d02 7d02 7c01 7c00 6a01 6405 3c00  d...}.|.|.j.d.<.
+00004b10: 7c02 7c00 6a01 6406 3c00 6407 7c00 6a01  |.|.j.d.<.d.|.j.
+00004b20: 6408 3c00 6409 5300 290a 7a63 4578 7465  d.<.d.S.).zcExte
+00004b30: 726e 616c 2044 6174 6120 5374 6f72 653a  rnal Data Store:
+00004b40: 2047 6574 2f73 6574 2063 6f6e 6669 6775   Get/set configu
+00004b50: 7261 7469 6f6e 732e 0a0a 2020 2020 5374  rations...    St
+00004b60: 616e 6461 7264 2044 6174 6120 5374 6f72  andard Data Stor
+00004b70: 653a 2047 6574 2f73 6574 2063 6f6e 6669  e: Get/set confi
+00004b80: 6775 7261 7469 6f6e 732e 0a20 2020 2054  gurations..    T
+00004b90: 46a9 0272 9a00 0000 da0b 6973 5f70 6879  F..r......is_phy
+00004ba0: 7369 6361 6c72 9900 0000 7280 0000 0072  sicalr....r....r
+00004bb0: 3000 0000 7285 0000 0072 8100 0000 4e72  0...r....r....Nr
+00004bc0: a300 0000 72a4 0000 0072 1200 0000 7212  ....r....r....r.
+00004bd0: 0000 0072 1300 0000 7285 0000 0021 0200  ...r....r....!..
+00004be0: 0073 0c00 0000 0808 1201 0e02 0a01 0a01  .s..............
+00004bf0: 0e01 7285 0000 0063 0200 0000 0000 0000  ..r....c........
+00004c00: 0000 0000 0200 0000 0600 0000 0300 0000  ................
+00004c10: 72a7 0000 0029 057a 5b45 7874 6572 6e61  r....).z[Externa
+00004c20: 6c20 4461 7461 2053 746f 7265 3a20 5365  l Data Store: Se
+00004c30: 7420 636f 6e66 6967 7572 6174 696f 6e73  t configurations
+00004c40: 2e0a 0a20 2020 2053 7461 6e64 6172 6420  ...    Standard 
+00004c50: 4461 7461 2053 746f 7265 3a20 5365 7420  Data Store: Set 
+00004c60: 636f 6e66 6967 7572 6174 696f 6e73 2e0a  configurations..
+00004c70: 2020 2020 7230 0000 00da 0a63 6f6e 6669      r0.....confi
+00004c80: 675f 7365 7463 0100 0000 0000 0000 0000  g_setc..........
+00004c90: 0000 0100 0000 0300 0000 1300 0000 72a9  ..............r.
+00004ca0: 0000 0072 1a00 0000 72aa 0000 0072 3200  ...r....r....r2.
+00004cb0: 0000 72ab 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00004cc0: 0072 3600 0000 3a02 0000 7237 0000 007a  .r6...:...r7...z
+00004cd0: 1c63 6f6e 6669 675f 7365 742e 3c6c 6f63  .config_set.<loc
+00004ce0: 616c 733e 2e3c 6c61 6d62 6461 3e72 ac00  als>.<lambda>r..
+00004cf0: 0000 72ab 0000 0072 1200 0000 72ab 0000  ..r....r....r...
+00004d00: 0072 1300 0000 72f5 0000 0032 0200 0072  .r....r....2...r
+00004d10: ea00 0000 72f5 0000 0063 0200 0000 0000  ....r....c......
+00004d20: 0000 0000 0000 0200 0000 0600 0000 0300  ................
+00004d30: 0000 72a7 0000 0029 057a 5b45 7874 6572  ..r....).z[Exter
+00004d40: 6e61 6c20 4461 7461 2053 746f 7265 3a20  nal Data Store: 
+00004d50: 4765 7420 636f 6e66 6967 7572 6174 696f  Get configuratio
+00004d60: 6e73 2e0a 0a20 2020 2053 7461 6e64 6172  ns...    Standar
+00004d70: 6420 4461 7461 2053 746f 7265 3a20 4765  d Data Store: Ge
+00004d80: 7420 636f 6e66 6967 7572 6174 696f 6e73  t configurations
+00004d90: 2e0a 2020 2020 7230 0000 00da 0a63 6f6e  ..    r0.....con
+00004da0: 6669 675f 6765 7463 0100 0000 0000 0000  fig_getc........
+00004db0: 0000 0000 0100 0000 0300 0000 1300 0000  ................
+00004dc0: 72a9 0000 0072 1a00 0000 72af 0000 0072  r....r....r....r
+00004dd0: 3200 0000 72ab 0000 0072 1200 0000 7213  2...r....r....r.
+00004de0: 0000 0072 3600 0000 4502 0000 7237 0000  ...r6...E...r7..
+00004df0: 007a 1c63 6f6e 6669 675f 6765 742e 3c6c  .z.config_get.<l
+00004e00: 6f63 616c 733e 2e3c 6c61 6d62 6461 3e72  ocals>.<lambda>r
+00004e10: ac00 0000 72ab 0000 0072 1200 0000 72ab  ....r....r....r.
+00004e20: 0000 0072 1300 0000 72f6 0000 003d 0200  ...r....r....=..
+00004e30: 0072 ea00 0000 72f6 0000 0063 0200 0000  .r....r....c....
+00004e40: 0000 0000 0000 0000 0200 0000 0600 0000  ................
+00004e50: 0300 0000 72a7 0000 0029 057a 2f45 7874  ....r....).z/Ext
+00004e60: 6572 6e61 6c20 4461 7461 2053 746f 7265  ernal Data Store
+00004e70: 3a20 436c 6561 7220 636f 6e66 6967 7572  : Clear configur
+00004e80: 6174 696f 6e73 2e0a 2020 2020 7230 0000  ations..    r0..
+00004e90: 00da 0c63 6f6e 6669 675f 636c 6561 7263  ...config_clearc
+00004ea0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00004eb0: 0300 0000 1300 0000 72a9 0000 0072 1a00  ........r....r..
+00004ec0: 0000 72b2 0000 0072 3200 0000 72ab 0000  ..r....r2...r...
+00004ed0: 0072 1200 0000 7213 0000 0072 3600 0000  .r....r....r6...
+00004ee0: 4e02 0000 7237 0000 007a 1e63 6f6e 6669  N...r7...z.confi
+00004ef0: 675f 636c 6561 722e 3c6c 6f63 616c 733e  g_clear.<locals>
+00004f00: 2e3c 6c61 6d62 6461 3e72 ac00 0000 72ab  .<lambda>r....r.
+00004f10: 0000 0072 1200 0000 72ab 0000 0072 1300  ...r....r....r..
+00004f20: 0000 72f7 0000 0048 0200 0073 0200 0000  ..r....H...s....
+00004f30: 1c06 72f7 0000 007a 022d 6d7a 052d 2d6d  ..r....z.-mz.--m
+00004f40: 7367 7a0b 6f62 6973 2063 6f6d 6d69 747a  sgz.obis commitz
+00004f50: 2341 206d 6573 7361 6765 2065 7870 6c61  #A message expla
+00004f60: 696e 696e 6720 7768 6174 2077 6173 2064  ining what was d
+00004f70: 6f6e 652e 7a02 2d61 7a0a 2d2d 6175 746f  one.z.-az.--auto
+00004f80: 5f61 6464 7a26 4175 746f 6d61 7469 6361  _addz&Automatica
+00004f90: 6c6c 7920 6164 6420 616c 6c20 756e 7472  lly add all untr
+00004fa0: 6163 6b65 6420 6669 6c65 732e 7a02 2d69  acked files.z.-i
+00004fb0: 7a17 2d2d 6967 6e6f 7265 5f6d 6973 7369  z.--ignore_missi
+00004fc0: 6e67 5f70 6172 656e 747a 2949 6620 7061  ng_parentz)If pa
+00004fd0: 7265 6e74 2064 6174 6120 7365 7420 6973  rent data set is
+00004fe0: 206d 6973 7369 6e67 2c20 6967 6e6f 7265   missing, ignore
+00004ff0: 2069 742e 2902 da06 6578 6973 7473 da09   it.)...exists..
+00005000: 6669 6c65 5f6f 6b61 7929 0272 0d00 0000  file_okay).r....
+00005010: da08 7265 7175 6972 6564 da06 636f 6d6d  ..required..comm
+00005020: 6974 7a30 436f 6d6d 6974 2074 6865 2072  itz0Commit the r
+00005030: 6570 6f73 6974 6f72 7920 746f 2067 6974  epository to git
+00005040: 2061 6e64 2069 6e66 6f72 6d20 6f70 656e   and inform open
+00005050: 4249 532e 6305 0000 0000 0000 0000 0000  BIS.c...........
+00005060: 0005 0000 0006 0000 0003 0000 0073 2000  .............s .
+00005070: 0000 7c00 6a00 6401 1900 a001 6402 8700  ..|.j.d.....d...
+00005080: 8701 8702 6603 6403 6404 8408 7c04 a103  ....f.d.d...|...
+00005090: 5300 2905 fa4a 4578 7465 726e 616c 2044  S.)..JExternal D
+000050a0: 6174 6120 5374 6f72 653a 2043 6f6d 6d69  ata Store: Commi
+000050b0: 7420 7468 6520 7265 706f 7369 746f 7279  t the repository
+000050c0: 2074 6f20 6769 7420 616e 6420 696e 666f   to git and info
+000050d0: 726d 206f 7065 6e42 4953 2e0a 2020 2020  rm openBIS..    
+000050e0: 7230 0000 0072 fb00 0000 6301 0000 0000  r0...r....c.....
+000050f0: 0000 0000 0000 0001 0000 0005 0000 0013  ................
+00005100: 0000 0073 0e00 0000 7c00 a000 8802 8800  ...s....|.......
+00005110: 8801 a103 5300 721a 0000 0029 0172 fb00  ....S.r....).r..
+00005120: 0000 7232 0000 00a9 03da 0861 7574 6f5f  ..r2.......auto_
+00005130: 6164 64da 1569 676e 6f72 655f 6d69 7373  add..ignore_miss
+00005140: 696e 675f 7061 7265 6e74 da03 6d73 6772  ing_parent..msgr
+00005150: 1200 0000 7213 0000 0072 3600 0000 6802  ....r....r6...h.
+00005160: 0000 72df 0000 007a 2372 6570 6f73 6974  ..r....z#reposit
+00005170: 6f72 795f 636f 6d6d 6974 2e3c 6c6f 6361  ory_commit.<loca
+00005180: 6c73 3e2e 3c6c 616d 6264 613e 72ac 0000  ls>.<lambda>r...
+00005190: 00a9 0572 2b00 0000 7200 0100 0072 fe00  ...r+...r....r..
+000051a0: 0000 72ff 0000 0072 3900 0000 7212 0000  ..r....r9...r...
+000051b0: 0072 fd00 0000 7213 0000 00da 1172 6570  .r....r......rep
+000051c0: 6f73 6974 6f72 795f 636f 6d6d 6974 6102  ository_commita.
+000051d0: 0000 7308 0000 000c 060e 0102 0104 fe72  ..s............r
+000051e0: 0201 0000 6305 0000 0000 0000 0000 0000  ....c...........
+000051f0: 0005 0000 0007 0000 0043 0000 0073 2c00  .........C...s,.
+00005200: 0000 7400 7c00 6a01 6401 6402 8d02 7c00  ..t.|.j.d.d...|.
+00005210: 6a01 6403 3c00 7c00 6a02 7403 7c01 7c02  j.d.<.|.j.t.|.|.
+00005220: 7c03 7c04 6404 8d05 0100 6405 5300 2906  |.|.d.....d.S.).
+00005230: 72fc 0000 0046 7299 0000 0072 3000 0000  r....Fr....r0...
+00005240: 2904 7200 0100 0072 fe00 0000 72ff 0000  ).r....r....r...
+00005250: 0072 3900 0000 4e29 0472 0900 0000 722a  .r9...N).r....r*
+00005260: 0000 00da 0669 6e76 6f6b 6572 0201 0000  .....invoker....
+00005270: 7201 0100 0072 1200 0000 7212 0000 0072  r....r....r....r
+00005280: 1300 0000 72fb 0000 006c 0200 0073 0800  ....r....l...s..
+00005290: 0000 1406 0a01 0401 0aff da0f 7265 706f  ............repo
+000052a0: 7369 746f 7279 5f70 6174 6872 3e00 0000  sitory_pathr>...
+000052b0: 722f 0000 0029 0172 2300 0000 da04 696e  r/...).r#.....in
+000052c0: 6974 7a2b 496e 6974 6961 6c69 7a65 2074  itz+Initialize t
+000052d0: 6865 2066 6f6c 6465 7220 6173 2061 2064  he folder as a d
+000052e0: 6174 6120 7265 706f 7369 746f 7279 2e63  ata repository.c
+000052f0: 0300 0000 0000 0000 0000 0000 0300 0000  ................
+00005300: 0400 0000 4300 0000 730c 0000 0074 007c  ....C...s....t.|
+00005310: 007c 017c 0283 0353 0029 017a 4545 7874  .|.|...S.).zEExt
+00005320: 6572 6e61 6c20 4461 7461 2053 746f 7265  ernal Data Store
+00005330: 3a20 496e 6974 6961 6c69 7a65 2074 6865  : Initialize the
+00005340: 2066 6f6c 6465 7220 6173 2061 2064 6174   folder as a dat
+00005350: 6120 7265 706f 7369 746f 7279 2e0a 2020  a repository..  
+00005360: 2020 2901 723a 0000 0029 0372 2b00 0000    ).r:...).r+...
+00005370: 7204 0100 0072 3e00 0000 7212 0000 0072  r....r>...r....r
+00005380: 1200 0000 7213 0000 00da 0f72 6570 6f73  ....r......repos
+00005390: 6974 6f72 795f 696e 6974 8202 0000 7302  itory_init....s.
+000053a0: 0000 000c 0672 0601 0000 7a0a 2d2d 7068  .....r....z.--ph
+000053b0: 7973 6963 616c 72f4 0000 007a 3849 6e69  ysicalr....z8Ini
+000053c0: 7469 616c 697a 6520 666f 6c64 6572 2066  tialize folder f
+000053d0: 6f72 2053 7461 6e64 6172 6420 4461 7461  or Standard Data
+000053e0: 2053 746f 7265 2064 6174 6120 6861 6e64   Store data hand
+000053f0: 6c69 6e67 2e63 0400 0000 0000 0000 0000  ling.c..........
+00005400: 0000 0400 0000 0500 0000 4300 0000 732a  ..........C...s*
+00005410: 0000 0074 007c 006a 0164 017c 0364 028d  ...t.|.j.d.|.d..
+00005420: 037c 006a 0164 033c 007c 006a 0274 037c  .|.j.d.<.|.j.t.|
+00005430: 017c 0264 048d 0301 0064 0553 0029 067a  .|.d.....d.S.).z
+00005440: df45 7874 6572 6e61 6c20 4461 7461 2053  .External Data S
+00005450: 746f 7265 3a20 496e 6974 6961 6c69 7a65  tore: Initialize
+00005460: 2074 6865 2066 6f6c 6465 7220 6173 2061   the folder as a
+00005470: 2064 6174 6120 7265 706f 7369 746f 7279   data repository
+00005480: 2066 6f72 2045 7874 6572 6e61 6c20 4461   for External Da
+00005490: 7461 2053 746f 7265 0a20 2020 2064 6174  ta Store.    dat
+000054a0: 6120 6861 6e64 6c69 6e67 2e0a 0a20 2020  a handling...   
+000054b0: 2053 7461 6e64 6172 6420 4461 7461 2053   Standard Data S
+000054c0: 746f 7265 3a20 496e 6974 6961 6c69 7a65  tore: Initialize
+000054d0: 2074 6865 2066 6f6c 6465 7220 6173 2061   the folder as a
+000054e0: 2064 6174 6120 7265 706f 7369 746f 7279   data repository
+000054f0: 2066 6f72 2053 7461 6e64 6172 6420 4461   for Standard Da
+00005500: 7461 2053 746f 7265 0a20 2020 2064 6174  ta Store.    dat
+00005510: 6120 6861 6e64 6c69 6e67 2e0a 2020 2020  a handling..    
+00005520: 4672 f300 0000 7230 0000 0029 0272 0401  Fr....r0...).r..
+00005530: 0000 723e 0000 004e 2904 7209 0000 0072  ..r>...N).r....r
+00005540: 2a00 0000 7203 0100 0072 0601 0000 2904  *...r....r....).
+00005550: 722b 0000 0072 0401 0000 723e 0000 0072  r+...r....r>...r
+00005560: f400 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
+00005570: 0000 0072 0501 0000 9102 0000 7304 0000  ...r........s...
+00005580: 0016 0a14 017a 082d 2d70 6172 656e 7429  .....z.--parent)
+00005590: 0172 0d00 0000 723c 0000 007a 2c49 6e69  .r....r<...z,Ini
+000055a0: 7469 616c 697a 6520 7468 6520 666f 6c64  tialize the fold
+000055b0: 6572 2061 7320 616e 2061 6e61 6c79 7369  er as an analysi
+000055c0: 7320 666f 6c64 6572 2e63 0400 0000 0000  s folder.c......
+000055d0: 0000 0000 0000 0400 0000 0500 0000 4300  ..............C.
+000055e0: 0000 730e 0000 0074 007c 007c 017c 027c  ..s....t.|.|.|.|
+000055f0: 0383 0453 0029 01fa 4145 7874 6572 6e61  ...S.)..AExterna
+00005600: 6c20 4461 7461 2053 746f 7265 3a20 496e  l Data Store: In
+00005610: 6974 6961 6c69 7a65 2074 6865 2066 6f6c  itialize the fol
+00005620: 6465 7220 6173 2061 6e20 616e 616c 7973  der as an analys
+00005630: 6973 2066 6f6c 6465 722e 2901 7249 0000  is folder.).rI..
+00005640: 00a9 0472 2b00 0000 723f 0000 0072 0401  ...r+...r?...r..
+00005650: 0000 723e 0000 0072 1200 0000 7212 0000  ..r>...r....r...
+00005660: 0072 1300 0000 da18 7265 706f 7369 746f  .r......reposito
+00005670: 7279 5f69 6e69 745f 616e 616c 7973 6973  ry_init_analysis
+00005680: a902 0000 7297 0000 0072 0901 0000 2902  ....r....r....).
+00005690: 7263 0000 0072 cd00 0000 6304 0000 0000  rc...r....c.....
+000056a0: 0000 0000 0000 0004 0000 0006 0000 0043  ...............C
+000056b0: 0000 0073 2a00 0000 7400 7c00 6a01 6401  ...s*...t.|.j.d.
+000056c0: 6402 8d02 7c00 6a01 6403 3c00 7c00 6a02  d...|.j.d.<.|.j.
+000056d0: 7403 7c01 7c02 7c03 6404 8d04 0100 6405  t.|.|.|.d.....d.
+000056e0: 5300 2906 7207 0100 0046 7299 0000 0072  S.).r....Fr....r
+000056f0: 3000 0000 2903 723f 0000 0072 0401 0000  0...).r?...r....
+00005700: 723e 0000 004e 2904 7209 0000 0072 2a00  r>...N).r....r*.
+00005710: 0000 7203 0100 0072 0901 0000 7208 0100  ..r....r....r...
+00005720: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00005730: 723c 0000 00b1 0200 0073 0800 0000 1405  r<.......s......
+00005740: 0801 0401 0aff da06 7374 6174 7573 7a26  ........statusz&
+00005750: 5368 6f77 2074 6865 2073 7461 7465 206f  Show the state o
+00005760: 6620 7468 6520 6f62 6973 2072 6570 6f73  f the obis repos
+00005770: 6974 6f72 792e 6302 0000 0000 0000 0000  itory.c.........
+00005780: 0000 0002 0000 0005 0000 0043 0000 00f3  ...........C....
+00005790: 1800 0000 7c00 6a00 6401 1900 a001 6402  ....|.j.d.....d.
+000057a0: 6403 6404 8400 7c01 a103 5300 2905 fa3b  d.d...|...S.)..;
+000057b0: 4578 7465 726e 616c 2044 6174 6120 5374  External Data St
+000057c0: 6f72 653a 2053 686f 7720 7468 6520 7374  ore: Show the st
+000057d0: 6174 6520 6f66 2074 6865 206f 6269 7320  ate of the obis 
+000057e0: 7265 706f 7369 746f 7279 2e72 3000 0000  repository.r0...
+000057f0: da11 7265 706f 7369 746f 7279 5f73 7461  ..repository_sta
+00005800: 7475 7363 0100 0000 0000 0000 0000 0000  tusc............
+00005810: 0100 0000 0200 0000 5300 0000 f308 0000  ........S.......
+00005820: 007c 00a0 00a1 0053 0072 1a00 0000 2901  .|.....S.r....).
+00005830: 720a 0100 0072 3200 0000 7212 0000 0072  r....r2...r....r
+00005840: 1200 0000 7213 0000 0072 3600 0000 c902  ....r....r6.....
+00005850: 0000 f302 0000 0008 007a 2372 6570 6f73  .........z#repos
+00005860: 6974 6f72 795f 7374 6174 7573 2e3c 6c6f  itory_status.<lo
+00005870: 6361 6c73 3e2e 3c6c 616d 6264 613e 72ac  cals>.<lambda>r.
+00005880: 0000 00a9 0272 2b00 0000 7239 0000 0072  .....r+...r9...r
+00005890: 1200 0000 7212 0000 0072 1300 0000 720d  ....r....r....r.
+000058a0: 0100 00c4 0200 00f3 0200 0000 1805 720d  ..............r.
+000058b0: 0100 0063 0200 0000 0000 0000 0000 0000  ...c............
+000058c0: 0200 0000 0400 0000 4300 0000 f326 0000  ........C....&..
+000058d0: 0074 007c 006a 0164 0164 028d 027c 006a  .t.|.j.d.d...|.j
+000058e0: 0164 033c 007c 006a 0274 037c 0164 048d  .d.<.|.j.t.|.d..
+000058f0: 0201 0064 0553 0029 0672 0c01 0000 4672  ...d.S.).r....Fr
+00005900: 9900 0000 7230 0000 00a9 0172 3900 0000  ....r0.....r9...
+00005910: 4e29 0472 0900 0000 722a 0000 0072 0301  N).r....r*...r..
+00005920: 0000 720d 0100 0072 1001 0000 7212 0000  ..r....r....r...
+00005930: 0072 1200 0000 7213 0000 0072 0a01 0000  .r....r....r....
+00005940: cc02 0000 f304 0000 0014 0512 0163 0200  .............c..
+00005950: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+00005960: 0000 4300 0000 730e 0000 007c 017c 005f  ..C...s....|.|._
+00005970: 007c 00a0 01a1 0053 0072 1a00 0000 2902  .|.....S.r....).
+00005980: 72ff 0000 00da 0473 796e 6329 0272 3300  r......sync).r3.
+00005990: 0000 72ff 0000 0072 1200 0000 7212 0000  ..r....r....r...
+000059a0: 0072 1300 0000 da10 5f72 6570 6f73 6974  .r......_reposit
+000059b0: 6f72 795f 7379 6e63 e002 0000 7304 0000  ory_sync....s...
+000059c0: 0006 0108 0172 1601 0000 7215 0100 007a  .....r....r....z
+000059d0: 2153 796e 6320 7468 6520 7265 706f 7369  !Sync the reposi
+000059e0: 746f 7279 2077 6974 6820 6f70 656e 4249  tory with openBI
+000059f0: 532e 6303 0000 0000 0000 0000 0000 0003  S.c.............
+00005a00: 0000 0006 0000 0003 0000 0073 1c00 0000  ...........s....
+00005a10: 7c00 6a00 6401 1900 a001 6402 8700 6601  |.j.d.....d...f.
+00005a20: 6403 6404 8408 7c02 a103 5300 2905 fa36  d.d...|...S.)..6
+00005a30: 4578 7465 726e 616c 2044 6174 6120 5374  External Data St
+00005a40: 6f72 653a 2053 796e 6320 7468 6520 7265  ore: Sync the re
+00005a50: 706f 7369 746f 7279 2077 6974 6820 6f70  pository with op
+00005a60: 656e 4249 532e 7230 0000 0072 1501 0000  enBIS.r0...r....
+00005a70: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00005a80: 0003 0000 0013 0000 0073 0a00 0000 7400  .........s....t.
+00005a90: 7c00 8800 8302 5300 721a 0000 0029 0172  |.....S.r....).r
+00005aa0: 1601 0000 7232 0000 00a9 0172 ff00 0000  ....r2.....r....
+00005ab0: 7212 0000 0072 1300 0000 7236 0000 00ea  r....r....r6....
+00005ac0: 0200 0072 3700 0000 7a21 7265 706f 7369  ...r7...z!reposi
+00005ad0: 746f 7279 5f73 796e 632e 3c6c 6f63 616c  tory_sync.<local
+00005ae0: 733e 2e3c 6c61 6d62 6461 3e72 ac00 0000  s>.<lambda>r....
+00005af0: a903 722b 0000 0072 ff00 0000 7239 0000  ..r+...r....r9..
+00005b00: 0072 1200 0000 7218 0100 0072 1300 0000  .r....r....r....
+00005b10: da0f 7265 706f 7369 746f 7279 5f73 796e  ..repository_syn
+00005b20: 63e5 0200 0073 0600 0000 1605 0201 04ff  c....s..........
+00005b30: 721a 0100 0063 0300 0000 0000 0000 0000  r....c..........
+00005b40: 0000 0300 0000 0500 0000 4300 0000 f328  ..........C....(
+00005b50: 0000 0074 007c 006a 0164 0164 028d 027c  ...t.|.j.d.d...|
+00005b60: 006a 0164 033c 007c 006a 0274 037c 017c  .j.d.<.|.j.t.|.|
+00005b70: 0264 048d 0301 0064 0553 0029 0672 1701  .d.....d.S.).r..
+00005b80: 0000 4672 9900 0000 7230 0000 0029 0272  ..Fr....r0...).r
+00005b90: ff00 0000 7239 0000 004e 2904 7209 0000  ....r9...N).r...
+00005ba0: 0072 2a00 0000 7203 0100 0072 1a01 0000  .r*...r....r....
+00005bb0: 7219 0100 0072 1200 0000 7212 0000 0072  r....r....r....r
+00005bc0: 1300 0000 7215 0100 00ee 0200 0073 0800  ....r........s..
+00005bd0: 0000 1405 0601 0401 0aff 7a1b 6372 6561  ..........z.crea
+00005be0: 7465 2f73 686f 7720 6120 6f70 656e 4249  te/show a openBI
+00005bf0: 5320 746f 6b65 6e63 0100 0000 0000 0000  S tokenc........
+00005c00: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00005c10: 7304 0000 0064 0053 0072 1a00 0000 7212  s....d.S.r....r.
+00005c20: 0000 0029 0172 2b00 0000 7212 0000 0072  ...).r+...r....r
+00005c30: 1200 0000 7213 0000 00da 0574 6f6b 656e  ....r......token
+00005c40: f802 0000 7302 0000 0004 0372 1c01 0000  ....s......r....
+00005c50: 7a36 4765 7420 6578 6973 7469 6e67 2070  z6Get existing p
+00005c60: 6572 736f 6e61 6c20 6163 6365 7373 2074  ersonal access t
+00005c70: 6f6b 656e 206f 7220 6372 6561 7465 2061  oken or create a
+00005c80: 206e 6577 206f 6e65 7a0c 7365 7373 696f   new onez.sessio
+00005c90: 6e2d 6e61 6d65 2901 72fa 0000 007a 0f2d  n-name).r....z.-
+00005ca0: 2d76 616c 6964 6974 792d 6461 7973 7a21  -validity-daysz!
+00005cb0: 4e75 6d62 6572 206f 6620 6461 7973 2074  Number of days t
+00005cc0: 6865 2074 6f6b 656e 2069 7320 7661 6c69  he token is vali
+00005cd0: 6429 0172 2500 0000 7a10 2d2d 7661 6c69  d).r%...z.--vali
+00005ce0: 6469 7479 2d77 6565 6b73 7a22 4e75 6d62  dity-weeksz"Numb
+00005cf0: 6572 206f 6620 7765 656b 7320 7468 6520  er of weeks the 
+00005d00: 746f 6b65 6e20 6973 2076 616c 6964 7a11  token is validz.
+00005d10: 2d2d 7661 6c69 6469 7479 2d6d 6f6e 7468  --validity-month
+00005d20: 737a 234e 756d 6265 7220 6f66 206d 6f6e  sz#Number of mon
+00005d30: 7468 7320 7468 6520 746f 6b65 6e20 6973  ths the token is
+00005d40: 2076 616c 6964 6302 0000 0000 0000 0000   validc.........
+00005d50: 0000 000e 0000 000a 0000 000b 0000 0073  ...............s
+00005d60: e801 0000 7400 8800 6a01 6401 6402 8d02  ....t...j.d.d...
+00005d70: 7d03 7c03 a002 a100 8901 7c01 7313 8801  }.|.......|.s...
+00005d80: 6403 1900 6404 1900 7d01 7c01 721f 7403  d...d...}.|.r.t.
+00005d90: a004 6405 7c01 9b00 6406 9d03 a101 0100  ..d.|...d.......
+00005da0: 6e05 7403 a005 6407 a101 7d01 8801 6403  n.t...d...}...d.
+00005db0: 1900 6408 1900 7d04 7c04 7331 7403 a005  ..d...}.|.s1t...
+00005dc0: 6409 a101 7d04 8801 6403 1900 640a 1900  d...}...d...d...
+00005dd0: 7d05 7c05 7341 7403 a005 640b 7c04 9b00  }.|.sAt...d.|...
+00005de0: 9d02 a101 7d05 7403 6a05 640c 7c05 9b00  ....}.t.j.d.|...
+00005df0: 640d 7c04 9b00 9d04 640e 640f 8d02 7d06  d.|.....d.d...}.
+00005e00: 7406 7c04 8801 6403 1900 a007 6410 640e  t.|...d.....d.d.
+00005e10: a102 6411 8d02 7d07 7a08 7c07 a008 7c05  ..d...}.z.|...|.
+00005e20: 7c06 a102 0100 5700 6e16 0400 7409 740a  |.....W.n...t.t.
+00005e30: 6602 7978 0100 7d08 0100 7a08 7403 a00b  f.yx..}...z.t...
+00005e40: 6412 7c08 9b00 9d02 a101 8201 6400 7d08  d.|.........d.}.
+00005e50: 7e08 7701 7700 740c a00d a100 7d09 7c02  ~.w.w.t.....}.|.
+00005e60: a007 6413 a101 728f 7c09 740e 740f 7c02  ..d...r.|.t.t.|.
+00005e70: a007 6413 a101 8301 6414 8d01 1700 7d0a  ..d.....d.....}.
+00005e80: 6e32 7c02 a007 6415 a101 72a1 7c09 740e  n2|...d...r.|.t.
+00005e90: 740f 7c02 a007 6415 a101 8301 6416 8d01  t.|...d.....d...
+00005ea0: 1700 7d0a 6e20 7c02 a007 6417 a101 72b3  ..}.n |...d...r.
+00005eb0: 7c09 740e 740f 7c02 a007 6417 a101 8301  |.t.t.|...d.....
+00005ec0: 6418 8d01 1700 7d0a 6e0e 7c07 a010 a100  d.....}.n.|.....
+00005ed0: 7d0b 7c0b 6a11 7d0c 7c09 740e 7c0c 6419  }.|.j.}.|.t.|.d.
+00005ee0: 8d01 1700 7d0a 7c07 6a12 7c01 7c09 7c0a  ....}.|.j.|.|.|.
+00005ef0: 641a 8d03 7d0d 640a 7c05 6901 6408 7c04  d...}.d.|.i.d.|.
+00005f00: 6901 641b 7c0d 6a13 6901 6404 7c01 6901  i.d.|.j.i.d.|.i.
+00005f10: 6604 8901 6401 8800 6a01 641c 3c00 7c03  f...d...j.d.<.|.
+00005f20: 8800 6a01 641d 3c00 6403 8800 6a01 641e  ..j.d.<.d...j.d.
+00005f30: 3c00 7c03 a014 641f 8700 8701 6602 6420  <.|...d.....f.d 
+00005f40: 6421 8408 a102 0100 6400 5300 2922 4e46  d!......d.S.)"NF
+00005f50: 7299 0000 0072 8500 0000 da0c 7365 7373  r....r......sess
+00005f60: 696f 6e5f 6e61 6d65 7528 0000 0047 6574  ion_nameu(...Get
+00005f70: 2070 6572 736f 6e61 6c20 6163 6365 7373   personal access
+00005f80: 2074 6f6b 656e 2066 6f72 2073 6573 7369   token for sessi
+00005f90: 6f6e 20c2 abf5 0200 0000 c2bb 7a1b 506c  on .........z.Pl
+00005fa0: 6561 7365 2065 6e74 6572 2061 2073 6573  ease enter a ses
+00005fb0: 7369 6f6e 206e 616d 65da 0b6f 7065 6e62  sion name..openb
+00005fc0: 6973 5f75 726c 7a1c 506c 6561 7365 2065  is_urlz.Please e
+00005fd0: 6e74 6572 2074 6865 206f 7065 6e42 4953  nter the openBIS
+00005fe0: 2055 524c da04 7573 6572 7a1a 506c 6561   URL..userz.Plea
+00005ff0: 7365 2065 6e74 6572 2075 7365 726e 616d  se enter usernam
+00006000: 6520 666f 7220 7a0d 5061 7373 776f 7264  e for z.Password
+00006010: 2066 6f72 20fa 0140 5429 01da 0a68 6964   for ..@T)...hid
+00006020: 655f 696e 7075 7472 2700 0000 2901 7227  e_inputr'...).r'
+00006030: 0000 007a 1b43 616e 6e6f 7420 636f 6e6e  ...z.Cannot conn
+00006040: 6563 7420 746f 206f 7065 6e42 4953 3a20  ect to openBIS: 
+00006050: da0f 7661 6c69 6469 7479 5f6d 6f6e 7468  ..validity_month
+00006060: 7329 01da 066d 6f6e 7468 73da 0e76 616c  s)...months..val
+00006070: 6964 6974 795f 7765 656b 7329 01da 0577  idity_weeks)...w
+00006080: 6565 6b73 da0d 7661 6c69 6469 7479 5f64  eeks..validity_d
+00006090: 6179 7329 01da 0464 6179 7329 01da 0773  ays)...days)...s
+000060a0: 6563 6f6e 6473 2903 da0b 7365 7373 696f  econds)...sessio
+000060b0: 6e4e 616d 65da 0976 616c 6964 4672 6f6d  nName..validFrom
+000060c0: da07 7661 6c69 6454 6fda 0d6f 7065 6e62  ..validTo..openb
+000060d0: 6973 5f74 6f6b 656e 7280 0000 0072 3000  is_tokenr....r0.
+000060e0: 0000 7281 0000 0072 f500 0000 6301 0000  ..r....r....c...
+000060f0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00006100: 0013 0000 0072 a900 0000 721a 0000 0072  .....r....r....r
+00006110: aa00 0000 7232 0000 0072 ab00 0000 7212  ....r2...r....r.
+00006120: 0000 0072 1300 0000 7236 0000 0038 0300  ...r....r6...8..
+00006130: 0072 3700 0000 7a1b 6e65 775f 746f 6b65  .r7...z.new_toke
+00006140: 6e2e 3c6c 6f63 616c 733e 2e3c 6c61 6d62  n.<locals>.<lamb
+00006150: 6461 3e29 1572 0900 0000 722a 0000 0072  da>).r....r*...r
+00006160: 9e00 0000 7216 0000 0072 1700 0000 da06  ....r....r......
+00006170: 7072 6f6d 7074 7205 0000 0072 9800 0000  promptr....r....
+00006180: da05 6c6f 6769 6e72 0400 0000 da0a 5661  ..loginr......Va
+00006190: 6c75 6545 7272 6f72 da0e 436c 6963 6b45  lueError..ClickE
+000061a0: 7863 6570 7469 6f6e 7202 0000 00da 036e  xceptionr......n
+000061b0: 6f77 7203 0000 00da 0369 6e74 da16 6765  owr......int..ge
+000061c0: 745f 7365 7276 6572 5f69 6e66 6f72 6d61  t_server_informa
+000061d0: 7469 6f6e da2a 7065 7273 6f6e 616c 5f61  tion.*personal_a
+000061e0: 6363 6573 735f 746f 6b65 6e73 5f6d 6178  ccess_tokens_max
+000061f0: 5f76 616c 6964 6974 795f 7065 7269 6f64  _validity_period
+00006200: da23 6765 745f 6f72 5f63 7265 6174 655f  .#get_or_create_
+00006210: 7065 7273 6f6e 616c 5f61 6363 6573 735f  personal_access_
+00006220: 746f 6b65 6eda 0670 6572 6d49 6472 3800  token..permIdr8.
+00006230: 0000 290e 722b 0000 0072 1d01 0000 da06  ..).r+...r......
+00006240: 6b77 6172 6773 7230 0000 00da 0375 726c  kwargsr0.....url
+00006250: da08 7573 6572 6e61 6d65 da08 7061 7373  ..username..pass
+00006260: 776f 7264 da01 6fda 0365 7863 722b 0100  word..o..excr+..
+00006270: 0072 2c01 0000 da0a 7365 7276 6572 696e  .r,.....serverin
+00006280: 666f 7229 0100 00da 0974 6f6b 656e 5f6f  for).....token_o
+00006290: 626a 7212 0000 0072 ab00 0000 7213 0000  bjr....r....r...
+000062a0: 00da 096e 6577 5f74 6f6b 656e fe02 0000  ...new_token....
+000062b0: 7366 0000 000e 0708 0104 020c 0104 0114  sf..............
+000062c0: 010a 020c 0204 010a 010c 0204 0110 011a  ................
+000062d0: 010c 0104 0108 ff02 0210 0112 0110 0108  ................
+000062e0: 8002 ff08 030a 0102 0112 0106 ff0a 0202  ................
+000062f0: 0112 0106 ff0a 0202 0112 0106 ff08 0306  ................
+00006300: 010e 0104 0106 0106 ff06 0306 0108 0106  ................
+00006310: 0104 fc0a 070a 010a 011a 0172 4001 0000  ...........r@...
+00006320: da06 6164 6472 6566 7a33 4164 6420 7468  ..addrefz3Add th
+00006330: 6520 6769 7665 6e20 7265 706f 7369 746f  e given reposito
+00006340: 7279 2061 7320 6120 7265 6665 7265 6e63  ry as a referenc
+00006350: 6520 746f 206f 7065 6e42 4953 2e63 0200  e to openBIS.c..
+00006360: 0000 0000 0000 0000 0000 0200 0000 0500  ................
+00006370: 0000 4300 0000 720b 0100 0029 05fa 2255  ..C...r....).."U
+00006380: 7365 6420 666f 7220 4578 7465 726e 616c  sed for External
+00006390: 2044 6174 6120 5374 6f72 6520 6f6e 6c79   Data Store only
+000063a0: 2e72 3000 0000 7241 0100 0063 0100 0000  .r0...rA...c....
+000063b0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+000063c0: 5300 0000 720e 0100 0072 1a00 0000 2901  S...r....r....).
+000063d0: 7241 0100 0072 3200 0000 7212 0000 0072  rA...r2...r....r
+000063e0: 1200 0000 7213 0000 0072 3600 0000 4603  ....r....r6...F.
+000063f0: 0000 720f 0100 007a 2372 6570 6f73 6974  ..r....z#reposit
+00006400: 6f72 795f 6164 6472 6566 2e3c 6c6f 6361  ory_addref.<loca
+00006410: 6c73 3e2e 3c6c 616d 6264 613e 72ac 0000  ls>.<lambda>r...
+00006420: 0072 1001 0000 7212 0000 0072 1200 0000  .r....r....r....
+00006430: 7213 0000 00da 1172 6570 6f73 6974 6f72  r......repositor
+00006440: 795f 6164 6472 6566 4103 0000 7211 0100  y_addrefA...r...
+00006450: 0072 4301 0000 6302 0000 0000 0000 0000  .rC...c.........
+00006460: 0000 0002 0000 0004 0000 0043 0000 0072  ...........C...r
+00006470: 1201 0000 2906 7242 0100 0046 7299 0000  ....).rB...Fr...
+00006480: 0072 3000 0000 7213 0100 004e 2904 7209  .r0...r....N).r.
+00006490: 0000 0072 2a00 0000 7203 0100 0072 4301  ...r*...r....rC.
+000064a0: 0000 7210 0100 0072 1200 0000 7212 0000  ..r....r....r...
+000064b0: 0072 1300 0000 7241 0100 0049 0300 0072  .r....rA...I...r
+000064c0: 1401 0000 7a0d 2d2d 6461 7461 5f73 6574  ....z.--data_set
+000064d0: 5f69 647a 4b52 656d 6f76 6520 7265 6620  _idzKRemove ref 
+000064e0: 6279 2064 6174 6120 7365 7420 6964 2c20  by data set id, 
+000064f0: 696e 2063 6173 6520 7468 6520 7265 706f  in case the repo
+00006500: 7369 746f 7279 2069 7320 6e6f 7420 6176  sitory is not av
+00006510: 6169 6c61 626c 6520 616e 796d 6f72 652e  ailable anymore.
+00006520: da09 7265 6d6f 7665 7265 667a 3a52 656d  ..removerefz:Rem
+00006530: 6f76 6520 7468 6520 7265 6665 7265 6e63  ove the referenc
+00006540: 6520 746f 2074 6865 2067 6976 656e 2072  e to the given r
+00006550: 6570 6f73 6974 6f72 7920 6672 6f6d 206f  epository from o
+00006560: 7065 6e42 4953 2e63 0300 0000 0000 0000  penBIS.c........
+00006570: 0000 0000 0300 0000 0600 0000 0300 0000  ................
+00006580: 7338 0000 0088 0064 0175 0172 0e7c 0264  s8.....d.u.r.|.d
+00006590: 0175 0172 0e74 0064 0283 0101 0064 0353  .u.r.t.d.....d.S
+000065a0: 007c 006a 0164 0419 00a0 0264 0587 0066  .|.j.d.....d...f
+000065b0: 0164 0664 0784 087c 02a1 0353 0029 0872  .d.d...|...S.).r
+000065c0: 4201 0000 4e7a 2f4f 6e6c 7920 7072 6f76  B...Nz/Only prov
+000065d0: 6964 6520 7468 6520 6461 7461 5f73 6574  ide the data_set
+000065e0: 2069 6420 4f52 2074 6865 2072 6570 6f73   id OR the repos
+000065f0: 6974 6f72 792e 723b 0000 0072 3000 0000  itory.r;...r0...
+00006600: 7244 0100 0063 0100 0000 0000 0000 0000  rD...c..........
+00006610: 0000 0100 0000 0300 0000 1300 0000 730c  ..............s.
+00006620: 0000 007c 006a 0088 0064 018d 0153 0029  ...|.j...d...S.)
+00006630: 024e a901 da0b 6461 7461 5f73 6574 5f69  .N....data_set_i
+00006640: 6429 0172 4401 0000 7232 0000 0072 4501  d).rD...r2...rE.
+00006650: 0000 7212 0000 0072 1300 0000 7236 0000  ..r....r....r6..
+00006660: 0066 0300 0072 4000 0000 7a26 7265 706f  .f...r@...z&repo
+00006670: 7369 746f 7279 5f72 656d 6f76 6572 6566  sitory_removeref
+00006680: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00006690: 613e 2903 7208 0000 0072 2a00 0000 7238  a>).r....r*...r8
+000066a0: 0000 00a9 0372 2b00 0000 7246 0100 0072  .....r+...rF...r
+000066b0: 3900 0000 7212 0000 0072 4501 0000 7213  9...r....rE...r.
+000066c0: 0000 00da 1472 6570 6f73 6974 6f72 795f  .....repository_
+000066d0: 7265 6d6f 7665 7265 665d 0300 0073 0c00  removeref]...s..
+000066e0: 0000 1006 0801 0401 1601 0201 04ff 7248  ..............rH
+000066f0: 0100 0063 0300 0000 0000 0000 0000 0000  ...c............
+00006700: 0300 0000 0500 0000 4300 0000 721b 0100  ........C...r...
+00006710: 0029 0672 4201 0000 4672 9900 0000 7230  .).rB...Fr....r0
+00006720: 0000 0029 0272 4601 0000 7239 0000 004e  ...).rF...r9...N
+00006730: 2904 7209 0000 0072 2a00 0000 7203 0100  ).r....r*...r...
+00006740: 0072 4801 0000 7247 0100 0072 1200 0000  .rH...rG...r....
+00006750: 7212 0000 0072 1300 0000 7244 0100 006a  r....r....rD...j
+00006760: 0300 0073 0800 0000 1405 0801 0201 0aff  ...s............
+00006770: 7246 0100 007a 0a2d 6672 6f6d 2d66 696c  rF...z.-from-fil
+00006780: 657a 0b2d 2d66 726f 6d2d 6669 6c65 da09  ez.--from-file..
+00006790: 6672 6f6d 5f66 696c 657a 6a41 6e20 6f75  from_filezjAn ou
+000067a0: 7470 7574 202e 4353 5620 6669 6c65 2066  tput .CSV file f
+000067b0: 726f 6d20 606f 6269 7320 6461 7461 5f73  rom `obis data_s
+000067c0: 6574 2073 6561 7263 6860 2063 6f6d 6d61  et search` comma
+000067d0: 6e64 2077 6974 6820 7468 6520 6c69 7374  nd with the list
+000067e0: 206f 6620 6f62 6a65 6374 7320 746f 2064   of objects to d
+000067f0: 6f77 6e6c 6f61 6420 6461 7461 7365 7473  ownload datasets
+00006800: 2066 726f 6d7a 022d 667a 062d 2d66 696c   fromz.-fz.--fil
+00006810: 65da 0466 696c 657a 4046 696c 6520 696e  e..filez@File in
+00006820: 2074 6865 2064 6174 6120 7365 7420 746f   the data set to
+00006830: 2064 6f77 6e6c 6f61 6420 2d20 646f 776e   download - down
+00006840: 6c6f 6164 696e 6720 616c 6c20 6966 206e  loading all if n
+00006850: 6f74 2067 6976 656e 2e7a 162d 2d73 6b69  ot given.z.--ski
+00006860: 705f 696e 7465 6772 6974 795f 6368 6563  p_integrity_chec
+00006870: 6b7a 3046 6c61 6720 746f 2073 6b69 7020  kz0Flag to skip 
+00006880: 6669 6c65 2069 6e74 6567 7269 7479 2063  file integrity c
+00006890: 6865 636b 2077 6974 6820 6368 6563 6b73  heck with checks
+000068a0: 756d 73da 0864 6f77 6e6c 6f61 647a 1d44  ums..downloadz.D
+000068b0: 6f77 6e6c 6f61 6420 6669 6c65 7320 6f66  ownload files of
+000068c0: 2061 2064 6174 6120 7365 742e 6305 0000   a data set.c...
+000068d0: 0000 0000 0000 0000 0005 0000 0007 0000  ................
+000068e0: 0003 0000 0073 6000 0000 8800 6401 7500  .....s`.....d.u.
+000068f0: 7208 8802 6401 7500 7310 8800 6401 7501  r...d.u.s...d.u.
+00006900: 7216 8802 6401 7501 7216 7400 6402 8301  r...d.u.r.t.d...
+00006910: 0100 6403 5300 7401 7c00 6a02 6404 6405  ..d.S.t.|.j.d.d.
+00006920: 8d02 7c00 6a02 6406 3c00 7c00 6a02 6406  ..|.j.d.<.|.j.d.
+00006930: 1900 a003 6407 8700 8701 8702 8703 6604  ....d.........f.
+00006940: 6408 6409 8408 a102 5300 290a 7a76 2044  d.d.....S.).zv D
+00006950: 6f77 6e6c 6f61 6473 2064 6174 6173 6574  ownloads dataset
+00006960: 2066 696c 6573 2066 726f 6d20 4f70 656e   files from Open
+00006970: 4249 5320 696e 7374 616e 6365 2e0a 0a20  BIS instance... 
+00006980: 2020 2044 4154 415f 5345 5420 2020 2055     DATA_SET    U
+00006990: 6e69 7175 6520 6964 656e 7469 6669 6572  nique identifier
+000069a0: 206f 6620 6461 7461 7365 7420 7769 7468   of dataset with
+000069b0: 696e 204f 7065 6e42 4953 2069 6e73 7461  in OpenBIS insta
+000069c0: 6e63 652e 4e7a 2e27 6461 7461 5f73 6574  nce.Nz.'data_set
+000069d0: 5f69 6427 206f 7220 2766 726f 6d5f 6669  _id' or 'from_fi
+000069e0: 6c65 2720 6d75 7374 2062 6520 7072 6f76  le' must be prov
+000069f0: 6964 6564 2172 3b00 0000 4672 9900 0000  ided!r;...Fr....
+00006a00: 7230 0000 0072 4b01 0000 6301 0000 0000  r0...rK...c.....
+00006a10: 0000 0000 0000 0001 0000 0006 0000 0013  ................
+00006a20: 0000 0073 1200 0000 7c00 6a00 8800 8802  ...s....|.j.....
+00006a30: 8801 8803 6401 8d04 5300 2902 4e29 0472  ....d...S.).N).r
+00006a40: 4601 0000 7249 0100 0072 4a01 0000 da14  F...rI...rJ.....
+00006a50: 736b 6970 5f69 6e74 6567 7269 7479 5f63  skip_integrity_c
+00006a60: 6865 636b 2901 724b 0100 0072 3200 0000  heck).rK...r2...
+00006a70: a904 7246 0100 0072 4a01 0000 7249 0100  ..rF...rJ...rI..
+00006a80: 0072 4c01 0000 7212 0000 0072 1300 0000  .rL...r....r....
+00006a90: 7236 0000 0091 0300 0073 0800 0000 0600  r6.......s......
+00006aa0: 0401 0201 06fe 7a1a 646f 776e 6c6f 6164  ......z.download
+00006ab0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
+00006ac0: 613e 2904 7208 0000 0072 0900 0000 722a  a>).r....r....r*
+00006ad0: 0000 0072 3800 0000 2905 722b 0000 0072  ...r8...).r+...r
+00006ae0: 4601 0000 7249 0100 0072 4a01 0000 724c  F...rI...rJ...rL
+00006af0: 0100 0072 1200 0000 724d 0100 0072 1300  ...r....rM...r..
+00006b00: 0000 724b 0100 0085 0300 0073 1000 0000  ..rK.......s....
+00006b10: 1006 1001 0801 0401 1401 0c01 1001 04ff  ................
+00006b20: da05 6669 6c65 737a 1c66 696c 6520 6f72  ..filesz.file or
+00006b30: 2064 6972 6563 746f 7279 2074 6f20 7570   directory to up
+00006b40: 6c6f 6164 2e29 0372 2500 0000 72fa 0000  load.).r%...r...
+00006b50: 00da 086d 756c 7469 706c 657a 0a2d 2d70  ...multiplez.--p
+00006b60: 726f 7065 7274 79da 0a70 726f 7065 7274  roperty..propert
+00006b70: 6965 737a 2970 726f 7065 7274 7920 746f  iesz)property to
+00006b80: 2073 6574 2066 6f72 2074 6865 2075 706c   set for the upl
+00006b90: 6f61 6465 6420 6461 7461 7365 742e 2904  oaded dataset.).
+00006ba0: 7225 0000 0072 fa00 0000 724f 0100 0072  r%...r....rO...r
+00006bb0: 2300 0000 da09 7361 6d70 6c65 5f69 64da  #.....sample_id.
+00006bc0: 0d64 6174 615f 7365 745f 7479 7065 da06  .data_set_type..
+00006bd0: 7570 6c6f 6164 7a20 5570 6c6f 6164 2066  uploadz Upload f
+00006be0: 696c 6573 2074 6f20 666f 726d 2061 2064  iles to form a d
+00006bf0: 6174 6120 7365 742e 6305 0000 0000 0000  ata set.c.......
+00006c00: 0000 0000 0005 0000 0007 0000 0003 0000  ................
+00006c10: 0073 3800 0000 7400 7c00 6a01 6401 6402  .s8...t.|.j.d.d.
+00006c20: 8d02 7c00 6a01 6403 3c00 7c00 6a01 6403  ..|.j.d.<.|.j.d.
+00006c30: 1900 a002 6404 8700 8701 8702 8703 6604  ....d.........f.
+00006c40: 6405 6406 8408 a102 0100 6407 5300 2908  d.d.......d.S.).
+00006c50: 7aaa 2043 7265 6174 6573 2064 6174 6120  z. Creates data 
+00006c60: 7365 7420 756e 6465 7220 6f62 6a65 6374  set under object
+00006c70: 2061 6e64 2075 706c 6f61 6420 6669 6c65   and upload file
+00006c80: 7320 746f 2069 742e 0a0a 2020 2020 5341  s to it...    SA
+00006c90: 4d50 4c45 5f49 4420 2020 2020 2020 556e  MPLE_ID       Un
+00006ca0: 6971 7565 2069 6465 6e74 6966 6965 7220  ique identifier 
+00006cb0: 616e 206f 626a 6563 7420 696e 204f 7065  an object in Ope
+00006cc0: 6e42 4953 2e0a 0a20 2020 2044 4154 415f  nBIS...    DATA_
+00006cd0: 5345 545f 5459 5045 2020 204e 6577 6c79  SET_TYPE   Newly
+00006ce0: 2063 7265 6174 6564 2064 6174 6120 7365   created data se
+00006cf0: 7420 7479 7065 2e0a 2020 2020 4672 9900  t type..    Fr..
+00006d00: 0000 7230 0000 0072 5301 0000 6301 0000  ..r0...rS...c...
+00006d10: 0000 0000 0000 0000 0001 0000 0006 0000  ................
+00006d20: 0013 0000 0073 1000 0000 7c00 a000 8803  .....s....|.....
+00006d30: 8800 8801 8802 a104 5300 721a 0000 0029  ........S.r....)
+00006d40: 0172 5301 0000 7232 0000 00a9 0472 5201  .rS...r2.....rR.
+00006d50: 0000 724e 0100 0072 5001 0000 7251 0100  ..rN...rP...rQ..
+00006d60: 0072 1200 0000 7213 0000 0072 3600 0000  .r....r....r6...
+00006d70: ad03 0000 7302 0000 0010 007a 1875 706c  ....s......z.upl
+00006d80: 6f61 642e 3c6c 6f63 616c 733e 2e3c 6c61  oad.<locals>.<la
+00006d90: 6d62 6461 3e4e 2903 7209 0000 0072 2a00  mbda>N).r....r*.
+00006da0: 0000 7238 0000 0029 0572 2b00 0000 7251  ..r8...).r+...rQ
+00006db0: 0100 0072 5201 0000 724e 0100 0072 5001  ...rR...rN...rP.
+00006dc0: 0000 7212 0000 0072 5401 0000 7213 0000  ..r....rT...r...
+00006dd0: 0072 5301 0000 a303 0000 7308 0000 0014  .rS.......s.....
+00006de0: 080c 0110 0108 ff7a 022d 757a 0a2d 2d73  .......z.-uz.--s
+00006df0: 7368 5f75 7365 727a 2955 7365 7220 746f  sh_userz)User to
+00006e00: 2063 6f6e 6e65 6374 2074 6f20 7265 6d6f   connect to remo
+00006e10: 7465 2073 7973 7465 6d73 2076 6961 2073  te systems via s
+00006e20: 7368 7a02 2d63 7a14 2d2d 636f 6e74 656e  shz.-cz.--conten
+00006e30: 745f 636f 7079 5f69 6e64 6578 7a49 496e  t_copy_indexzIIn
+00006e40: 6465 7820 6f66 2074 6865 2063 6f6e 7465  dex of the conte
+00006e50: 6e74 2063 6f70 7920 746f 2063 6c6f 6e65  nt copy to clone
+00006e60: 2066 726f 6d20 696e 2063 6173 6520 7468   from in case th
+00006e70: 6572 6520 6172 6520 6d75 6c74 6970 6c65  ere are multiple
+00006e80: 2063 6f70 6965 7329 0372 0d00 0000 7223   copies).r....r#
+00006e90: 0000 0072 2500 0000 7a29 536b 6970 2066  ...r%...z)Skip f
+00006ea0: 696c 6520 696e 7465 6772 6974 7920 6368  ile integrity ch
+00006eb0: 6563 6b20 7769 7468 2063 6865 636b 7375  eck with checksu
+00006ec0: 6d73 2eda 0563 6c6f 6e65 7a34 436c 6f6e  ms...clonez4Clon
+00006ed0: 6520 7468 6520 7265 706f 7369 746f 7279  e the repository
+00006ee0: 2066 6f75 6e64 2069 6e20 7468 6520 6769   found in the gi
+00006ef0: 7665 6e20 6461 7461 2073 6574 2069 642e  ven data set id.
+00006f00: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
+00006f10: 0007 0000 0003 0000 00f3 2000 0000 7c00  .......... ...|.
+00006f20: 6a00 6401 1900 a001 6402 8700 8701 8702  j.d.....d.......
+00006f30: 8703 6604 6403 6404 8408 a102 5300 2905  ..f.d.d.....S.).
+00006f40: 4e72 3000 0000 7255 0100 0063 0100 0000  Nr0...rU...c....
+00006f50: 0000 0000 0000 0000 0100 0000 0600 0000  ................
+00006f60: 1300 0000 f310 0000 007c 00a0 0088 0188  .........|......
+00006f70: 0388 0088 02a1 0453 0072 1a00 0000 2901  .......S.r....).
+00006f80: 7255 0100 0072 3200 0000 a904 da12 636f  rU...r2.......co
+00006f90: 6e74 656e 745f 636f 7079 5f69 6e64 6578  ntent_copy_index
+00006fa0: 7246 0100 0072 4c01 0000 da08 7373 685f  rF...rL.....ssh_
+00006fb0: 7573 6572 7212 0000 0072 1300 0000 7236  userr....r....r6
+00006fc0: 0000 00c3 0300 00f3 0600 0000 0a00 0201  ................
+00006fd0: 04ff 7a20 6461 7461 5f73 6574 5f63 6c6f  ..z data_set_clo
+00006fe0: 6e65 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  ne.<locals>.<lam
+00006ff0: 6264 613e 72ac 0000 00a9 0572 2b00 0000  bda>r......r+...
+00007000: 725a 0100 0072 5901 0000 7246 0100 0072  rZ...rY...rF...r
+00007010: 4c01 0000 7212 0000 0072 5801 0000 7213  L...r....rX...r.
+00007020: 0000 00da 0e64 6174 615f 7365 745f 636c  .....data_set_cl
+00007030: 6f6e 65be 0300 00f3 0600 0000 0c04 1001  one.............
+00007040: 04ff 725d 0100 0063 0500 0000 0000 0000  ..r]...c........
+00007050: 0000 0000 0500 0000 0700 0000 4300 0000  ............C...
+00007060: f32c 0000 0074 007c 006a 0164 0164 028d  .,...t.|.j.d.d..
+00007070: 027c 006a 0164 033c 007c 006a 0274 037c  .|.j.d.<.|.j.t.|
+00007080: 017c 027c 037c 0464 048d 0501 0064 0053  .|.|.|.d.....d.S
+00007090: 00a9 054e 4672 9900 0000 7230 0000 0029  ...NFr....r0...)
+000070a0: 0472 5a01 0000 7259 0100 0072 4601 0000  .rZ...rY...rF...
+000070b0: 724c 0100 0029 0472 0900 0000 722a 0000  rL...).r....r*..
+000070c0: 0072 0301 0000 725d 0100 0072 5c01 0000  .r....r]...r\...
+000070d0: 7212 0000 0072 1200 0000 7213 0000 0072  r....r....r....r
+000070e0: 5501 0000 c703 0000 f308 0000 0014 040a  U...............
+000070f0: 0104 010a ffda 046d 6f76 657a 334d 6f76  .......movez3Mov
+00007100: 6520 7468 6520 7265 706f 7369 746f 7279  e the repository
+00007110: 2066 6f75 6e64 2069 6e20 7468 6520 6769   found in the gi
+00007120: 7665 6e20 6461 7461 2073 6574 2069 642e  ven data set id.
+00007130: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
+00007140: 0007 0000 0003 0000 0072 5601 0000 2905  .........rV...).
+00007150: 4e72 3000 0000 7262 0100 0063 0100 0000  Nr0...rb...c....
+00007160: 0000 0000 0000 0000 0100 0000 0600 0000  ................
+00007170: 1300 0000 7257 0100 0072 1a00 0000 2901  ....rW...r....).
+00007180: 7262 0100 0072 3200 0000 7258 0100 0072  rb...r2...rX...r
+00007190: 1200 0000 7213 0000 0072 3600 0000 d703  ....r....r6.....
+000071a0: 0000 725b 0100 007a 1f64 6174 615f 7365  ..r[...z.data_se
+000071b0: 745f 6d6f 7665 2e3c 6c6f 6361 6c73 3e2e  t_move.<locals>.
+000071c0: 3c6c 616d 6264 613e 72ac 0000 0072 5c01  <lambda>r....r\.
+000071d0: 0000 7212 0000 0072 5801 0000 7213 0000  ..r....rX...r...
+000071e0: 00da 0d64 6174 615f 7365 745f 6d6f 7665  ...data_set_move
+000071f0: d203 0000 725e 0100 0072 6301 0000 6305  ....r^...rc...c.
+00007200: 0000 0000 0000 0000 0000 0005 0000 0007  ................
+00007210: 0000 0043 0000 0072 5f01 0000 7260 0100  ...C...r_...r`..
+00007220: 0029 0472 0900 0000 722a 0000 0072 0301  .).r....r*...r..
+00007230: 0000 7263 0100 0072 5c01 0000 7212 0000  ..rc...r\...r...
+00007240: 0072 1200 0000 7213 0000 0072 6201 0000  .r....r....rb...
+00007250: db03 0000 7261 0100 0063 0000 0000 0000  ....ra...c......
+00007260: 0000 0000 0000 0000 0000 0300 0000 4300  ..............C.
+00007270: 0000 730e 0000 0074 0069 0064 018d 0101  ..s....t.i.d....
+00007280: 0064 0053 0029 024e 7229 0000 0029 0172  .d.S.).Nr)...).r
+00007290: 2d00 0000 7212 0000 0072 1200 0000 7212  -...r....r....r.
+000072a0: 0000 0072 1300 0000 da04 6d61 696e e403  ...r......main..
+000072b0: 0000 7302 0000 000e 0172 6401 0000 da08  ..s......rd.....
+000072c0: 5f5f 6d61 696e 5f5f 2902 4e4e 721a 0000  __main__).NNr...
+000072d0: 0029 6bda 075f 5f64 6f63 5f5f 729f 0000  .)k..__doc__r...
+000072e0: 0072 4100 0000 7202 0000 0072 1600 0000  .rA...r....r....
+000072f0: da16 6461 7465 7574 696c 2e72 656c 6174  ..dateutil.relat
+00007300: 6976 6564 656c 7461 7203 0000 00da 0872  ivedeltar......r
+00007310: 6571 7565 7374 7372 0400 0000 da05 7079  equestsr......py
+00007320: 6269 7372 0500 0000 da0a 636c 6963 6b5f  bisr......click_
+00007330: 7574 696c 7208 0000 00da 1064 6174 615f  utilr......data_
+00007340: 6d67 6d74 5f72 756e 6e65 7272 0900 0000  mgmt_runnerr....
+00007350: da11 646d 2e63 6f6d 6d61 6e64 5f72 6573  ..dm.command_res
+00007360: 756c 7472 0b00 0000 da08 646d 2e75 7469  ultr......dm.uti
+00007370: 6c73 720c 0000 0072 1400 0000 7219 0000  lsr....r....r...
+00007380: 0072 2100 0000 da05 6772 6f75 70da 0e76  .r!.....group..v
+00007390: 6572 7369 6f6e 5f6f 7074 696f 6eda 066f  ersion_option..o
+000073a0: 7074 696f 6eda 0c70 6173 735f 636f 6e74  ption..pass_cont
+000073b0: 6578 7472 2d00 0000 723a 0000 0072 4900  extr-...r:...rI.
+000073c0: 0000 da09 5061 7261 6d54 7970 6572 4a00  ....ParamTyperJ.
+000073d0: 0000 7264 0000 0072 6500 0000 727c 0000  ..rd...re...r|..
+000073e0: 0072 7f00 0000 7287 0000 0072 8d00 0000  .r....r....r....
+000073f0: 7293 0000 0072 9600 0000 726a 0000 00da  r....r....rj....
+00007400: 0763 6f6d 6d61 6e64 724b 0000 0072 3900  .commandrK...r9.
+00007410: 0000 da08 6172 6775 6d65 6e74 72a8 0000  ....argumentr...
+00007420: 0072 ae00 0000 72b1 0000 00da 165f 6461  .r....r......_da
+00007430: 7461 7365 745f 7365 6172 6368 5f70 6172  taset_search_par
+00007440: 616d 73da 185f 7365 6172 6368 5f62 795f  ams.._search_by_
+00007450: 7361 6d70 6c65 5f70 6172 616d 7372 c300  sample_paramsr..
+00007460: 0000 72c5 0000 0072 c700 0000 72c8 0000  ..r....r....r...
+00007470: 0072 cb00 0000 72d9 0000 0072 e500 0000  .r....r....r....
+00007480: 72e8 0000 0072 eb00 0000 72ec 0000 00da  r....r....r.....
+00007490: 155f 6f62 6a65 6374 5f73 6561 7263 685f  ._object_search_
+000074a0: 7061 7261 6d73 72ee 0000 0072 e300 0000  paramsr....r....
+000074b0: 72f0 0000 0072 f100 0000 72f2 0000 0072  r....r....r....r
+000074c0: 8500 0000 72f5 0000 0072 f600 0000 72f7  ....r....r....r.
+000074d0: 0000 00da 0450 6174 68da 0e5f 636f 6d6d  .....Path.._comm
+000074e0: 6974 5f70 6172 616d 7372 0201 0000 72fb  it_paramsr....r.
+000074f0: 0000 00da 0c5f 696e 6974 5f70 6172 616d  ....._init_param
+00007500: 7372 0601 0000 da15 5f69 6e69 745f 7061  sr......_init_pa
+00007510: 7261 6d73 5f70 6879 7369 6361 6c72 0501  rams_physicalr..
+00007520: 0000 da15 5f69 6e69 745f 616e 616c 7973  ...._init_analys
+00007530: 6973 5f70 6172 616d 7372 0901 0000 723c  is_paramsr....r<
+00007540: 0000 00da 0e5f 7374 6174 7573 5f70 6172  ....._status_par
+00007550: 616d 7372 0d01 0000 720a 0100 00da 0c5f  amsr....r......_
+00007560: 7379 6e63 5f70 6172 616d 7372 1601 0000  sync_paramsr....
+00007570: 721a 0100 0072 1501 0000 721c 0100 0072  r....r....r....r
+00007580: 4001 0000 da0e 5f61 6464 7265 665f 7061  @....._addref_pa
+00007590: 7261 6d73 7243 0100 0072 4101 0000 da11  ramsrC...rA.....
+000075a0: 5f72 656d 6f76 6572 6566 5f70 6172 616d  _removeref_param
+000075b0: 7372 4801 0000 7244 0100 00da 105f 646f  srH...rD....._do
+000075c0: 776e 6c6f 6164 5f70 6172 616d 7372 4b01  wnload_paramsrK.
+000075d0: 0000 da0e 5f75 706c 6f61 645f 7061 7261  ...._upload_para
+000075e0: 6d73 7253 0100 0072 3301 0000 da12 5f63  msrS...r3....._c
+000075f0: 6c6f 6e65 5f6d 6f76 655f 7061 7261 6d73  lone_move_params
+00007600: 725d 0100 0072 5501 0000 7263 0100 0072  r]...rU...rc...r
+00007610: 6201 0000 7264 0100 0072 6000 0000 7212  b...rd...r`...r.
+00007620: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+00007630: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00007640: 731c 0300 0004 1208 0508 010c 0108 020c  s...............
+00007650: 010c 010c 020c 010c 010c 010c 0108 0308  ................
+00007660: 0508 0506 090a 0112 010c 0102 0104 ff12  ................
+00007670: 0204 0114 0108 0708 0912 1410 0f12 0408  ................
+00007680: 2b08 080c 0708 0b08 0708 0906 0b12 0104  +...............
+00007690: 010e 0108 0504 010c 0106 0a12 0104 010e  ................
+000076a0: 0108 0810 0104 010e 0108 0510 0104 010e  ................
+000076b0: 0108 0510 0104 010e 0110 0810 0110 010c  ................
+000076c0: 0102 0104 ff12 0210 0110 010c 0102 0104  ................
+000076d0: ff0c 0202 0104 ff10 020e 0102 0104 ff04  ................
+000076e0: f20c 1302 0104 ff0c 0202 0104 ff0c 0202  ................
+000076f0: 0104 ff0c 0202 0104 ff0c 0202 0104 ff0a  ................
+00007700: 0202 0104 ff0a 0202 0104 ff08 0204 0102  ................
+00007710: 0104 fe08 0304 0102 0104 fe04 ee08 1812  ................
+00007720: 010c 0102 0104 ff04 0210 0108 0910 0104  ................
+00007730: 010e 0108 0510 0104 010e 0108 0510 0104  ................
+00007740: 010e 0108 050c 040a 0104 010e 0106 2a12  ..............*.
+00007750: 0104 010e 0108 0b10 0104 010e 0108 0810  ................
+00007760: 0104 010e 0108 0810 0104 010e 0110 0610  ................
+00007770: 0110 010c 0102 0104 ff12 0210 010a 0102  ................
+00007780: 0104 ff0c 0202 0104 ff0c 0202 0104 ff10  ................
+00007790: 020e 0102 0104 ff04 f10c 1406 0104 010e  ................
+000077a0: 0106 1d12 0104 010e 0108 0b10 0104 010e  ................
+000077b0: 0108 0810 0104 010e 0108 0810 0104 010e  ................
+000077c0: 0106 0812 0104 010e 0108 0e10 0104 010e  ................
+000077d0: 0108 0810 0104 010e 0108 0810 0104 010e  ................
+000077e0: 010a 0b02 0104 ff0c 0202 0104 ff0a 0204  ................
+000077f0: 0104 ff0a 0204 0104 ff02 0104 ff04 f90c  ................
+00007800: 0c04 0106 010e 010a 0804 0106 010e 010a  ................
+00007810: 0c04 0104 ff02 0104 ff0c 0204 fd0c 0804  ................
+00007820: 0106 010e 0102 070e 0102 0106 ff02 ff02  ................
+00007830: ff0a 0604 0106 010e 0108 0f0c 0104 ff04  ................
+00007840: ff08 040c 0304 0106 010e 010c 0504 0106  ................
+00007850: 010e 010a 0b04 0104 ff02 0104 ff04 ff0c  ................
+00007860: 0604 0106 010e 010a 0504 0106 010e 010a  ................
+00007870: 0a04 0104 ff0a 0204 0104 ff02 0104 ff04  ................
+00007880: fd08 080c 0504 0106 010e 010a 0604 0106  ................
+00007890: 010e 010a 0704 010c 010c 040c 0112 0112  ................
+000078a0: 0112 0104 011c 010a 3804 0104 ff02 0104  ........8.......
+000078b0: ff04 ff10 0604 0106 0112 010c 0504 0106  ................
+000078c0: 0112 010a 0a04 0106 ff0a 0204 0104 ff02  ................
+000078d0: 0104 ff04 fd08 0804 0104 ff04 0206 0112  ................
+000078e0: 010c 0904 0106 0112 010e 0c10 0104 0106  ................
+000078f0: ff04 030c 0104 0106 fe0e 0304 0104 ff04  ................
+00007900: f810 0d06 0104 0112 0104 1214 0106 ff04  ................
+00007910: 0214 0106 ff0a 020a 0104 fa10 0a06 0104  ................
+00007920: 0112 010e 0e04 0104 ff10 0204 0106 ff0c  ................
+00007930: 0206 0104 ff0a 0204 f910 0b04 0106 0112  ................
+00007940: 010c 0604 0106 0112 0110 0804 0106 0112  ................
+00007950: 010c 0604 0106 0112 010c 060c 040a 0104  ................
+00007960: ff                                       .
```

### Comparing `obis-0.4.5/obis/scripts/__pycache__/click_util.cpython-310.pyc` & `obis-0.4.6rc0/obis/scripts/__pycache__/click_util.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri Aug 25 13:48:21 2023 UTC, .py size: 1127 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 25b1 e864 6704 0000  o.......%..dg...
+00000000: 6f0d 0d0a 0000 0000 554f 0166 6704 0000  o.......UO.fg...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 5a01 6408 6404 6405 8401 5a02 6406 6407  Z.d.d.d...Z.d.d.
 00000050: 8400 5a03 6402 5300 2909 e900 0000 0029  ..Z.d.S.)......)
 00000060: 01da 0864 6174 6574 696d 654e 5463 0200  ...datetimeNTc..
 00000070: 0000 0000 0000 0000 0000 0300 0000 0600  ................
```

### Comparing `obis-0.4.5/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc` & `obis-0.4.6rc0/obis/scripts/__pycache__/data_mgmt_runner.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 30 10:59:06 2023 UTC, .py size: 5701 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 7a6b 2564 4516 0000  o.......zk%dE...
+00000000: 6f0d 0d0a 0000 0000 554f 0166 4516 0000  o.......UO.fE...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6402  d.l.Z.d.d.l.Z.d.
 00000040: 6403 6c02 6d03 5a03 6d04 5a04 0100 6404  d.l.m.Z.m.Z...d.
 00000050: 6405 6c05 6d06 5a06 0100 6404 6406 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6404 6407 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 0100 6404 6408 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `obis-0.4.5/obis/scripts/cli.py` & `obis-0.4.6rc0/obis/scripts/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -917,30 +917,32 @@
 
 # upload
 
 
 _upload_params = [
     click.option(
         '-f', '--file', "files", help='file or directory to upload.', required=True, multiple=True),
+    click.option(
+        '-p', '--property', "properties", help='property to set for the uploaded dataset.', required=False, multiple=True, default=[]),
     click.argument('sample_id'),
     click.argument('data_set_type'),
 ]
 
 
 @cli.command("upload", short_help="Upload files to form a data set.")
 @add_params(_upload_params)
 @click.pass_context
-def upload(ctx, sample_id, data_set_type, files):
+def upload(ctx, sample_id, data_set_type, files, properties):
     """ Creates data set under object and upload files to it.\n
     SAMPLE_ID       Unique identifier an object in OpenBIS.\n
     DATA_SET_TYPE   Newly created data set type.
     """
     ctx.obj['runner'] = DataMgmtRunner(ctx.obj, halt_on_error_log=False)
     ctx.obj['runner'].run("upload",
-                          lambda dm: dm.upload(sample_id, data_set_type, files))
+                          lambda dm: dm.upload(sample_id, data_set_type, files, properties))
 
 
 # clone
 
 
 _clone_move_params = [
     click.option('-u', '--ssh_user', default=None,
```

### Comparing `obis-0.4.5/obis/scripts/click_util.py` & `obis-0.4.6rc0/obis/scripts/click_util.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/scripts/data_mgmt_runner.py` & `obis-0.4.6rc0/obis/scripts/data_mgmt_runner.py`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis/test-data/snb-data.zip` & `obis-0.4.6rc0/obis/test-data/snb-data.zip`

 * *Files identical despite different names*

### Comparing `obis-0.4.5/obis.egg-info/PKG-INFO` & `obis-0.4.6rc0/obis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: obis
-Version: 0.4.5
+Version: 0.4.6rc0
 Summary: Local data management with assistance from OpenBIS.
 Home-page: https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line
 Author: ID SIS • ETH Zürich
 Author-email: openbis-support@id.ethz.ch
 License: Apache Software License Version 2.0
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -714,7 +715,9 @@
 
 ## 9. Literature
 
 V. Korolev, A. Joshi, V. Korolev, M.A. Grasso, A. Joshi, M.A. Grasso, et al., "PROB: A tool for
 tracking provenance and reproducibility of big data experiments", Reproduce '14. HPCA 2014, vol. 11,
 pp. 264-286, 2014.
 http://ebiquity.umbc.edu/_file_directory_/papers/693.pdf
+
+
```

### Comparing `obis-0.4.5/obis.egg-info/SOURCES.txt` & `obis-0.4.6rc0/obis.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 obis.egg-info/SOURCES.txt
 obis.egg-info/dependency_links.txt
 obis.egg-info/entry_points.txt
 obis.egg-info/not-zip-safe
 obis.egg-info/requires.txt
 obis.egg-info/top_level.txt
 obis/__pycache__/__init__.cpython-310.pyc
-obis/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
 obis/dm/__init__.py
 obis/dm/checksum.py
 obis/dm/command_log.py
 obis/dm/command_result.py
 obis/dm/config.py
 obis/dm/config_test.py
 obis/dm/data_mgmt.py
@@ -46,15 +45,14 @@
 obis/dm/utils_test.py
 obis/dm/__pycache__/__init__.cpython-310.pyc
 obis/dm/__pycache__/checksum.cpython-310.pyc
 obis/dm/__pycache__/command_log.cpython-310.pyc
 obis/dm/__pycache__/command_result.cpython-310.pyc
 obis/dm/__pycache__/config.cpython-310.pyc
 obis/dm/__pycache__/data_mgmt.cpython-310.pyc
-obis/dm/__pycache__/data_mgmt_test.cpython-310-pytest-7.2.1.pyc
 obis/dm/__pycache__/git.cpython-310.pyc
 obis/dm/__pycache__/repository_utils.cpython-310.pyc
 obis/dm/__pycache__/utils.cpython-310.pyc
 obis/dm/commands/__init__.py
 obis/dm/commands/addref.py
 obis/dm/commands/clone.py
 obis/dm/commands/collection.py
@@ -68,15 +66,14 @@
 obis/dm/commands/removeref.py
 obis/dm/commands/search.py
 obis/dm/commands/upload.py
 obis/dm/commands/__pycache__/__init__.cpython-310.pyc
 obis/dm/commands/__pycache__/addref.cpython-310.pyc
 obis/dm/commands/__pycache__/clone.cpython-310.pyc
 obis/dm/commands/__pycache__/collection.cpython-310.pyc
-obis/dm/commands/__pycache__/download.cpython-310.pyc
 obis/dm/commands/__pycache__/download_physical.cpython-310.pyc
 obis/dm/commands/__pycache__/move.cpython-310.pyc
 obis/dm/commands/__pycache__/object.cpython-310.pyc
 obis/dm/commands/__pycache__/openbis_command.cpython-310.pyc
 obis/dm/commands/__pycache__/openbis_sync.cpython-310.pyc
 obis/dm/commands/__pycache__/removeref.cpython-310.pyc
 obis/dm/commands/__pycache__/search.cpython-310.pyc
```

### Comparing `obis-0.4.5/setup.py` & `obis-0.4.6rc0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 data_dir = os.path.join("man", "man1")
 data_files = [
     (d, [os.path.join(d, f) for f in files]) for d, folders, files in os.walk(data_dir)
 ]
 
 setup(
     name="obis",
-    version="0.4.5",
+    version="0.4.6-rc0",
     description="Local data management with assistance from OpenBIS.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://sissource.ethz.ch/sispub/openbis/tree/master/app-openbis-command-line",
     author="ID SIS • ETH Zürich",
     author_email="openbis-support@id.ethz.ch",
     license="Apache Software License Version 2.0",
```

