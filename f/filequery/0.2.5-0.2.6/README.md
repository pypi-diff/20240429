# Comparing `tmp/filequery-0.2.5.tar.gz` & `tmp/filequery-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filequery-0.2.5.tar", last modified: Wed Apr 10 22:58:45 2024, max compression
+gzip compressed data, was "filequery-0.2.6.tar", last modified: Mon Apr 29 01:21:20 2024, max compression
```

## Comparing `filequery-0.2.5.tar` & `filequery-0.2.6.tar`

### file list

```diff
@@ -1,61 +1,64 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.207952 filequery-0.2.5/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1818 2023-02-19 00:56:16.000000 filequery-0.2.5/.gitignore
--rw-rw-r--   0 markus    (1000) markus    (1000)     1070 2023-02-19 00:24:28.000000 filequery-0.2.5/LICENSE
--rw-rw-r--   0 markus    (1000) markus    (1000)      330 2024-04-10 22:57:14.000000 filequery-0.2.5/Makefile
--rw-r--r--   0 markus    (1000) markus    (1000)     6323 2024-04-10 22:58:45.207952 filequery-0.2.5/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     5447 2024-02-29 04:12:58.000000 filequery-0.2.5/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.199952 filequery-0.2.5/example/
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.199952 filequery-0.2.5/example/config_files/
--rw-rw-r--   0 markus    (1000) markus    (1000)       86 2023-03-10 02:53:30.000000 filequery-0.2.5/example/config_files/example0.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      115 2023-03-10 02:53:30.000000 filequery-0.2.5/example/config_files/example1.json
--rw-rw-r--   0 markus    (1000) markus    (1000)       94 2023-03-10 02:53:30.000000 filequery-0.2.5/example/config_files/example2.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      117 2023-03-10 02:53:30.000000 filequery-0.2.5/example/config_files/example3.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      155 2023-03-10 02:53:30.000000 filequery-0.2.5/example/config_files/example4.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      186 2023-03-23 01:10:40.000000 filequery-0.2.5/example/config_files/example5.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      147 2023-03-23 01:10:40.000000 filequery-0.2.5/example/config_files/example6.json
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.199952 filequery-0.2.5/example/data/
--rw-rw-r--   0 markus    (1000) markus    (1000)      353 2023-03-11 23:35:48.000000 filequery-0.2.5/example/data/json_test.json
--rw-rw-r--   0 markus    (1000) markus    (1000)       54 2023-02-24 02:58:55.000000 filequery-0.2.5/example/data/test.csv
--rw-rw-r--   0 markus    (1000) markus    (1000)       69 2023-02-24 02:59:42.000000 filequery-0.2.5/example/data/test1.csv
--rw-rw-r--   0 markus    (1000) markus    (1000)       48 2024-04-10 22:55:58.000000 filequery-0.2.5/example/data/test_null.csv
--rw-rw-r--   0 markus    (1000) markus    (1000)      231 2023-03-11 23:35:48.000000 filequery-0.2.5/example/json_list_test.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      200 2023-03-11 23:35:48.000000 filequery-0.2.5/example/json_test.json
--rw-rw-r--   0 markus    (1000) markus    (1000)      260 2023-05-03 23:49:19.000000 filequery-0.2.5/example/ndjson_test.ndjson
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.203952 filequery-0.2.5/example/queries/
--rw-rw-r--   0 markus    (1000) markus    (1000)       75 2023-02-24 03:03:29.000000 filequery-0.2.5/example/queries/join.sql
--rw-rw-r--   0 markus    (1000) markus    (1000)      123 2023-03-11 23:35:48.000000 filequery-0.2.5/example/queries/json_csv_join.sql
--rw-rw-r--   0 markus    (1000) markus    (1000)      123 2023-03-11 23:35:48.000000 filequery-0.2.5/example/queries/json_query.sql
--rw-rw-r--   0 markus    (1000) markus    (1000)      120 2023-11-10 03:49:23.000000 filequery-0.2.5/example/queries/multi_query.sql
--rw-rw-r--   0 markus    (1000) markus    (1000)       54 2023-11-20 23:45:42.000000 filequery-0.2.5/example/test.csv
--rw-rw-r--   0 markus    (1000) markus    (1000)      632 2024-04-10 22:56:32.000000 filequery-0.2.5/pyproject.toml
--rw-rw-r--   0 markus    (1000) markus    (1000)      740 2024-03-29 01:47:08.000000 filequery-0.2.5/requirements-dev.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-03-29 01:46:52.000000 filequery-0.2.5/requirements.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       38 2024-04-10 22:58:45.207952 filequery-0.2.5/setup.cfg
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.195952 filequery-0.2.5/src/
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.203952 filequery-0.2.5/src/filequery/
--rw-rw-r--   0 markus    (1000) markus    (1000)     6422 2023-11-30 01:17:27.000000 filequery-0.2.5/src/filequery/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)       78 2023-11-10 03:49:23.000000 filequery-0.2.5/src/filequery/__main__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      225 2023-11-10 03:49:23.000000 filequery-0.2.5/src/filequery/exceptions.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      248 2023-11-10 03:49:23.000000 filequery-0.2.5/src/filequery/file_query_args.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     4067 2024-04-10 22:36:41.000000 filequery-0.2.5/src/filequery/filedb.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      102 2023-11-10 03:49:23.000000 filequery-0.2.5/src/filequery/filetype.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     2925 2024-03-01 05:00:43.000000 filequery-0.2.5/src/filequery/queryresult.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.203952 filequery-0.2.5/src/filequery/tui/
--rw-rw-r--   0 markus    (1000) markus    (1000)    12714 2024-04-10 22:55:58.000000 filequery-0.2.5/src/filequery/tui/duckui.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     2104 2024-01-13 23:26:57.000000 filequery-0.2.5/src/filequery/tui/help_content.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.203952 filequery-0.2.5/src/filequery/tui/screens/
--rw-rw-r--   0 markus    (1000) markus    (1000)      772 2024-02-29 04:13:13.000000 filequery-0.2.5/src/filequery/tui/screens/file_browser.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     1457 2024-02-29 04:13:13.000000 filequery-0.2.5/src/filequery/tui/screens/menu.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      159 2024-02-29 04:13:13.000000 filequery-0.2.5/src/filequery/tui/screens/menu_events.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.203952 filequery-0.2.5/src/filequery/tui/styles/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-02-29 04:13:13.000000 filequery-0.2.5/src/filequery/tui/styles/style.tcss
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.203952 filequery-0.2.5/src/filequery.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     6323 2024-04-10 22:58:45.000000 filequery-0.2.5/src/filequery.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1325 2024-04-10 22:58:45.000000 filequery-0.2.5/src/filequery.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-10 22:58:45.000000 filequery-0.2.5/src/filequery.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       55 2024-04-10 22:58:45.000000 filequery-0.2.5/src/filequery.egg-info/entry_points.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-04-10 22:58:45.000000 filequery-0.2.5/src/filequery.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       10 2024-04-10 22:58:45.000000 filequery-0.2.5/src/filequery.egg-info/top_level.txt
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-10 22:58:45.203952 filequery-0.2.5/tests/
--rw-rw-r--   0 markus    (1000) markus    (1000)        0 2023-02-19 00:27:10.000000 filequery-0.2.5/tests/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    10538 2024-04-08 02:25:37.000000 filequery-0.2.5/tests/test_filequery.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-29 01:21:20.264369 filequery-0.2.6/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1818 2023-02-19 00:56:16.000000 filequery-0.2.6/.gitignore
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1070 2023-02-19 00:24:28.000000 filequery-0.2.6/LICENSE
+-rw-rw-r--   0 markus    (1000) markus    (1000)      330 2024-04-10 22:57:14.000000 filequery-0.2.6/Makefile
+-rw-r--r--   0 markus    (1000) markus    (1000)     6547 2024-04-29 01:21:20.264369 filequery-0.2.6/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     5671 2024-04-29 01:18:46.000000 filequery-0.2.6/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-29 01:21:20.260369 filequery-0.2.6/example/
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-29 01:21:20.260369 filequery-0.2.6/example/config_files/
+-rw-rw-r--   0 markus    (1000) markus    (1000)       86 2023-03-10 02:53:30.000000 filequery-0.2.6/example/config_files/example0.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      115 2023-03-10 02:53:30.000000 filequery-0.2.6/example/config_files/example1.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)       94 2023-03-10 02:53:30.000000 filequery-0.2.6/example/config_files/example2.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      117 2023-03-10 02:53:30.000000 filequery-0.2.6/example/config_files/example3.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      155 2023-03-10 02:53:30.000000 filequery-0.2.6/example/config_files/example4.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      186 2023-03-23 01:10:40.000000 filequery-0.2.6/example/config_files/example5.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      147 2023-03-23 01:10:40.000000 filequery-0.2.6/example/config_files/example6.json
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-29 01:21:20.260369 filequery-0.2.6/example/data/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      353 2023-03-11 23:35:48.000000 filequery-0.2.6/example/data/json_test.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)       54 2024-04-29 01:19:09.000000 filequery-0.2.6/example/data/space filename.csv
+-rw-rw-r--   0 markus    (1000) markus    (1000)       54 2024-04-29 01:16:50.000000 filequery-0.2.6/example/data/test-filename.csv
+-rw-rw-r--   0 markus    (1000) markus    (1000)       54 2023-02-24 02:58:55.000000 filequery-0.2.6/example/data/test.csv
+-rw-rw-r--   0 markus    (1000) markus    (1000)       69 2023-02-24 02:59:42.000000 filequery-0.2.6/example/data/test1.csv
+-rw-rw-r--   0 markus    (1000) markus    (1000)       48 2024-04-10 22:55:58.000000 filequery-0.2.6/example/data/test_null.csv
+-rw-rw-r--   0 markus    (1000) markus    (1000)       80 2024-04-29 01:16:50.000000 filequery-0.2.6/example/data/test_special_chars.csv
+-rw-rw-r--   0 markus    (1000) markus    (1000)      231 2023-03-11 23:35:48.000000 filequery-0.2.6/example/json_list_test.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      200 2023-03-11 23:35:48.000000 filequery-0.2.6/example/json_test.json
+-rw-rw-r--   0 markus    (1000) markus    (1000)      260 2023-05-03 23:49:19.000000 filequery-0.2.6/example/ndjson_test.ndjson
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-29 01:21:20.264369 filequery-0.2.6/example/queries/
+-rw-rw-r--   0 markus    (1000) markus    (1000)       75 2023-02-24 03:03:29.000000 filequery-0.2.6/example/queries/join.sql
+-rw-rw-r--   0 markus    (1000) markus    (1000)      123 2023-03-11 23:35:48.000000 filequery-0.2.6/example/queries/json_csv_join.sql
+-rw-rw-r--   0 markus    (1000) markus    (1000)      123 2023-03-11 23:35:48.000000 filequery-0.2.6/example/queries/json_query.sql
+-rw-rw-r--   0 markus    (1000) markus    (1000)      120 2023-11-10 03:49:23.000000 filequery-0.2.6/example/queries/multi_query.sql
+-rw-rw-r--   0 markus    (1000) markus    (1000)       54 2023-11-20 23:45:42.000000 filequery-0.2.6/example/test.csv
+-rw-rw-r--   0 markus    (1000) markus    (1000)      632 2024-04-29 01:17:00.000000 filequery-0.2.6/pyproject.toml
+-rw-rw-r--   0 markus    (1000) markus    (1000)      740 2024-03-29 01:47:08.000000 filequery-0.2.6/requirements-dev.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-03-29 01:46:52.000000 filequery-0.2.6/requirements.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       38 2024-04-29 01:21:20.264369 filequery-0.2.6/setup.cfg
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-29 01:21:20.256370 filequery-0.2.6/src/
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-29 01:21:20.264369 filequery-0.2.6/src/filequery/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     6422 2023-11-30 01:17:27.000000 filequery-0.2.6/src/filequery/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)       78 2023-11-10 03:49:23.000000 filequery-0.2.6/src/filequery/__main__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      225 2023-11-10 03:49:23.000000 filequery-0.2.6/src/filequery/exceptions.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      248 2023-11-10 03:49:23.000000 filequery-0.2.6/src/filequery/file_query_args.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     5560 2024-04-29 01:16:50.000000 filequery-0.2.6/src/filequery/filedb.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      102 2023-11-10 03:49:23.000000 filequery-0.2.6/src/filequery/filetype.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     2964 2024-04-29 01:16:50.000000 filequery-0.2.6/src/filequery/queryresult.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-29 01:21:20.264369 filequery-0.2.6/src/filequery/tui/
+-rw-rw-r--   0 markus    (1000) markus    (1000)    12714 2024-04-10 23:12:34.000000 filequery-0.2.6/src/filequery/tui/duckui.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     2104 2024-01-13 23:26:57.000000 filequery-0.2.6/src/filequery/tui/help_content.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-29 01:21:20.264369 filequery-0.2.6/src/filequery/tui/screens/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      772 2024-02-29 04:13:13.000000 filequery-0.2.6/src/filequery/tui/screens/file_browser.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1457 2024-02-29 04:13:13.000000 filequery-0.2.6/src/filequery/tui/screens/menu.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      159 2024-02-29 04:13:13.000000 filequery-0.2.6/src/filequery/tui/screens/menu_events.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-29 01:21:20.264369 filequery-0.2.6/src/filequery/tui/styles/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-02-29 04:13:13.000000 filequery-0.2.6/src/filequery/tui/styles/style.tcss
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-29 01:21:20.264369 filequery-0.2.6/src/filequery.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     6547 2024-04-29 01:21:20.000000 filequery-0.2.6/src/filequery.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1424 2024-04-29 01:21:20.000000 filequery-0.2.6/src/filequery.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-29 01:21:20.000000 filequery-0.2.6/src/filequery.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       55 2024-04-29 01:21:20.000000 filequery-0.2.6/src/filequery.egg-info/entry_points.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)      286 2024-04-29 01:21:20.000000 filequery-0.2.6/src/filequery.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       10 2024-04-29 01:21:20.000000 filequery-0.2.6/src/filequery.egg-info/top_level.txt
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-29 01:21:20.264369 filequery-0.2.6/tests/
+-rw-rw-r--   0 markus    (1000) markus    (1000)        0 2023-02-19 00:27:10.000000 filequery-0.2.6/tests/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    12064 2024-04-29 01:16:50.000000 filequery-0.2.6/tests/test_filequery.py
```

### Comparing `filequery-0.2.5/.gitignore` & `filequery-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `filequery-0.2.5/LICENSE` & `filequery-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `filequery-0.2.5/PKG-INFO` & `filequery-0.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filequery
-Version: 0.2.5
+Version: 0.2.6
 Summary: Query CSV and Parquet files using SQL
 Author-email: Markus Hutnik <markus@markushutnik.com>
 License: MIT
 Project-URL: repository, https://github.com/MarkyMan4/filequery
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -84,15 +84,17 @@
   -c CONFIG, --config CONFIG
                         path to JSON config file
   -e, --editor          run SQL editor UI for exploring data
   -v, --version         show program's version number and exit
 ```
 
 For basic usage, provide a path to a CSV or Parquet file and a query to execute against it. The table name will be the 
-file name without the extension.
+file name without the extension. If the file name does not conform to DuckDB's rules for unquoted identifiers, the 
+table name will need to be wrapped in double quotes. For example, a file named `my data.csv` would be queried as 
+`select * from "my data"`.
 
 ```bash
 filequery --filename example/test.csv --query 'select * from test'
 ```
 
 ## TUI usage
```

### Comparing `filequery-0.2.5/README.md` & `filequery-0.2.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,17 @@
   -c CONFIG, --config CONFIG
                         path to JSON config file
   -e, --editor          run SQL editor UI for exploring data
   -v, --version         show program's version number and exit
 ```
 
 For basic usage, provide a path to a CSV or Parquet file and a query to execute against it. The table name will be the 
-file name without the extension.
+file name without the extension. If the file name does not conform to DuckDB's rules for unquoted identifiers, the 
+table name will need to be wrapped in double quotes. For example, a file named `my data.csv` would be queried as 
+`select * from "my data"`.
 
 ```bash
 filequery --filename example/test.csv --query 'select * from test'
 ```
 
 ## TUI usage
```

### Comparing `filequery-0.2.5/pyproject.toml` & `filequery-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "filequery"
 authors = [{ name = "Markus Hutnik", email = "markus@markushutnik.com" }]
 description = "Query CSV and Parquet files using SQL"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = ["Programming Language :: Python :: 3"]
 license = { text = "MIT" }
-version = "0.2.5"
+version = "0.2.6"
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
 
 [project.scripts]
 filequery = "filequery:fq_cli_handler"
```

### Comparing `filequery-0.2.5/requirements-dev.txt` & `filequery-0.2.6/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `filequery-0.2.5/src/filequery/__init__.py` & `filequery-0.2.6/src/filequery/__init__.py`

 * *Files identical despite different names*

### Comparing `filequery-0.2.5/src/filequery/queryresult.py` & `filequery-0.2.6/src/filequery/queryresult.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Dict, List
 
 import numpy as np
+from rich import markup
 from rich.console import Console
 from rich.table import Table
 
 
 class QueryResult:
     def __init__(self, result: Dict[str, np.ndarray]):
         self.result_cols = {}
@@ -70,15 +71,15 @@
             # otherwise create a table using rich
             table = Table()
             for col in self.result_cols:
                 justify = "left" if self.result_cols[col] == "object" else "right"
                 table.add_column(col, justify=justify)
 
             for rec in self.records:
-                stringified = [str(r) for r in rec]
+                stringified = [markup.escape(str(r)) for r in rec]
                 table.add_row(*stringified)
 
             console = Console()
             console.print(table)
 
     def save_to_file(self, filepath: str, delimiter: str = ","):
         """
```

### Comparing `filequery-0.2.5/src/filequery/tui/duckui.py` & `filequery-0.2.6/src/filequery/tui/duckui.py`

 * *Files identical despite different names*

### Comparing `filequery-0.2.5/src/filequery/tui/help_content.py` & `filequery-0.2.6/src/filequery/tui/help_content.py`

 * *Files identical despite different names*

### Comparing `filequery-0.2.5/src/filequery/tui/screens/file_browser.py` & `filequery-0.2.6/src/filequery/tui/screens/file_browser.py`

 * *Files identical despite different names*

### Comparing `filequery-0.2.5/src/filequery/tui/screens/menu.py` & `filequery-0.2.6/src/filequery/tui/screens/menu.py`

 * *Files identical despite different names*

### Comparing `filequery-0.2.5/src/filequery/tui/styles/style.tcss` & `filequery-0.2.6/src/filequery/tui/styles/style.tcss`

 * *Files identical despite different names*

### Comparing `filequery-0.2.5/src/filequery.egg-info/PKG-INFO` & `filequery-0.2.6/src/filequery.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filequery
-Version: 0.2.5
+Version: 0.2.6
 Summary: Query CSV and Parquet files using SQL
 Author-email: Markus Hutnik <markus@markushutnik.com>
 License: MIT
 Project-URL: repository, https://github.com/MarkyMan4/filequery
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -84,15 +84,17 @@
   -c CONFIG, --config CONFIG
                         path to JSON config file
   -e, --editor          run SQL editor UI for exploring data
   -v, --version         show program's version number and exit
 ```
 
 For basic usage, provide a path to a CSV or Parquet file and a query to execute against it. The table name will be the 
-file name without the extension.
+file name without the extension. If the file name does not conform to DuckDB's rules for unquoted identifiers, the 
+table name will need to be wrapped in double quotes. For example, a file named `my data.csv` would be queried as 
+`select * from "my data"`.
 
 ```bash
 filequery --filename example/test.csv --query 'select * from test'
 ```
 
 ## TUI usage
```

### Comparing `filequery-0.2.5/src/filequery.egg-info/SOURCES.txt` & `filequery-0.2.6/src/filequery.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,17 +13,20 @@
 example/config_files/example1.json
 example/config_files/example2.json
 example/config_files/example3.json
 example/config_files/example4.json
 example/config_files/example5.json
 example/config_files/example6.json
 example/data/json_test.json
+example/data/space filename.csv
+example/data/test-filename.csv
 example/data/test.csv
 example/data/test1.csv
 example/data/test_null.csv
+example/data/test_special_chars.csv
 example/queries/join.sql
 example/queries/json_csv_join.sql
 example/queries/json_query.sql
 example/queries/multi_query.sql
 src/filequery/__init__.py
 src/filequery/__main__.py
 src/filequery/exceptions.py
```

### Comparing `filequery-0.2.5/tests/test_filequery.py` & `filequery-0.2.6/tests/test_filequery.py`

 * *Files 23% similar despite different names*

```diff
@@ -129,25 +129,73 @@
         res = fdb.exec_query("select * from ndjson_test")
 
         self.assertEqual(len(res.dict_records), 4)
 
     def test_dict_records_keys_json(self):
         fdb = FileDb("example/ndjson_test.ndjson")
         res = fdb.exec_query("select * from ndjson_test")
-        
+
         for rec in res.dict_records:
             self.assertListEqual(list(rec.keys()), ["id", "value", "nested"])
 
     def test_dict_records_nested_keys_json(self):
         fdb = FileDb("example/ndjson_test.ndjson")
         res = fdb.exec_query("select * from ndjson_test")
-        
+
         for rec in res.dict_records:
             self.assertListEqual(list(rec["nested"].keys()), ["subid", "subval"])
 
+    def test_valid_unquoted_identifier(self):
+        fdb = FileDb("example/test.csv")
+        should_quote = fdb._should_quote_table_name("test_table")
+
+        self.assertFalse(should_quote)
+
+    def test_filename_with_leading_underscore(self):
+        fdb = FileDb("example/test.csv")
+        should_quote = fdb._should_quote_table_name("_test_table")
+
+        self.assertFalse(should_quote)
+
+    def test_filename_with_numbers(self):
+        fdb = FileDb("example/test.csv")
+        should_quote = fdb._should_quote_table_name("test_table_1")
+
+        self.assertFalse(should_quote)
+
+    def test_filename_with_hyphen(self):
+        fdb = FileDb("example/test.csv")
+        should_quote = fdb._should_quote_table_name("test-table")
+
+        self.assertTrue(should_quote)
+
+    def test_filename_with_leading_number(self):
+        fdb = FileDb("example/test.csv")
+        should_quote = fdb._should_quote_table_name("1test")
+
+        self.assertTrue(should_quote)
+
+    def test_filename_with_spaces(self):
+        fdb = FileDb("example/test.csv")
+        should_quote = fdb._should_quote_table_name("test table")
+
+        self.assertTrue(should_quote)
+
+    def test_filename_with_leading_special_char(self):
+        fdb = FileDb("example/test.csv")
+        should_quote = fdb._should_quote_table_name("$test")
+
+        self.assertTrue(should_quote)
+
+    def test_filename_with_leading_space(self):
+        fdb = FileDb("example/test.csv")
+        should_quote = fdb._should_quote_table_name(" test")
+
+        self.assertTrue(should_quote)
+
 
 class TestFileQueryCli(unittest.TestCase):
     #####################################################
     # tests for invalid arguments
     #####################################################
 
     def test_no_filename_or_filesdir(self):
```

