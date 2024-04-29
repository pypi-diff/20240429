# Comparing `tmp/lcpcli-0.1.2.tar.gz` & `tmp/lcpcli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcpcli-0.1.2.tar", last modified: Wed Mar 20 15:14:00 2024, max compression
+gzip compressed data, was "lcpcli-0.1.3.tar", last modified: Mon Apr 29 16:56:20 2024, max compression
```

## Comparing `lcpcli-0.1.2.tar` & `lcpcli-0.1.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.877719 lcpcli-0.1.2/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1058 2023-12-13 14:52:19.000000 lcpcli-0.1.2/LICENSE.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)    10342 2024-03-20 15:14:00.877719 lcpcli-0.1.2/PKG-INFO
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     9377 2024-03-19 10:00:31.000000 lcpcli-0.1.2/README.md
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.873718 lcpcli-0.1.2/bin/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       41 2023-12-05 17:05:43.000000 lcpcli-0.1.2/bin/lcpcli
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.873718 lcpcli-0.1.2/corpert/
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.873718 lcpcli-0.1.2/corpert/_legacy_process_files/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    16490 2023-12-05 17:12:56.000000 lcpcli-0.1.2/corpert/_legacy_process_files/process_opensubtitles.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    12104 2023-12-05 17:12:56.000000 lcpcli-0.1.2/corpert/_legacy_process_files/process_sparcling.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.873718 lcpcli-0.1.2/corpert/build/
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.873718 lcpcli-0.1.2/corpert/build/lib/
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.873718 lcpcli-0.1.2/corpert/build/lib/corpert/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       52 2023-12-05 17:12:56.000000 lcpcli-0.1.2/corpert/build/lib/corpert/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      205 2023-12-05 17:12:56.000000 lcpcli-0.1.2/corpert/build/lib/corpert/__main__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1318 2023-12-05 17:12:56.000000 lcpcli-0.1.2/corpert/build/lib/corpert/cli.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    17713 2024-02-28 15:54:29.000000 lcpcli-0.1.2/corpert/build/lib/corpert/corpert.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.877719 lcpcli-0.1.2/corpert/build/lib/corpert/parsers/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        0 2023-12-05 17:12:56.000000 lcpcli-0.1.2/corpert/build/lib/corpert/parsers/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     3039 2024-02-28 15:58:27.000000 lcpcli-0.1.2/corpert/build/lib/corpert/parsers/_parser.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     7418 2024-02-27 16:14:48.000000 lcpcli-0.1.2/corpert/build/lib/corpert/parsers/conllu.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      370 2023-12-05 17:12:56.000000 lcpcli-0.1.2/corpert/build/lib/corpert/parsers/json.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    10547 2024-02-27 16:14:48.000000 lcpcli-0.1.2/corpert/build/lib/corpert/parsers/tei.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     5885 2024-02-27 16:14:48.000000 lcpcli-0.1.2/corpert/build/lib/corpert/parsers/vert.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    13067 2024-02-29 13:04:27.000000 lcpcli-0.1.2/corpert/build/lib/corpert/utils.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.877719 lcpcli-0.1.2/corpert/corpert/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       52 2023-12-05 17:12:56.000000 lcpcli-0.1.2/corpert/corpert/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      205 2023-12-05 17:12:56.000000 lcpcli-0.1.2/corpert/corpert/__main__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1318 2023-12-05 17:12:56.000000 lcpcli-0.1.2/corpert/corpert/cli.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    19440 2024-03-18 14:41:46.000000 lcpcli-0.1.2/corpert/corpert/corpert.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     6227 2024-03-18 14:41:46.000000 lcpcli-0.1.2/corpert/corpert/lcp_corpus_template.json
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.877719 lcpcli-0.1.2/corpert/corpert/parsers/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        0 2023-12-05 17:12:56.000000 lcpcli-0.1.2/corpert/corpert/parsers/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    22998 2024-03-18 14:41:46.000000 lcpcli-0.1.2/corpert/corpert/parsers/_parser.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    11195 2024-03-18 14:41:46.000000 lcpcli-0.1.2/corpert/corpert/parsers/conllu.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      370 2023-12-05 17:12:56.000000 lcpcli-0.1.2/corpert/corpert/parsers/json.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    10547 2024-02-27 16:14:48.000000 lcpcli-0.1.2/corpert/corpert/parsers/tei.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     5885 2024-02-27 16:14:48.000000 lcpcli-0.1.2/corpert/corpert/parsers/vert.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    16596 2024-03-18 14:41:46.000000 lcpcli-0.1.2/corpert/corpert/utils.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       71 2024-03-18 14:41:46.000000 lcpcli-0.1.2/corpert/requirements.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      809 2023-12-06 14:34:53.000000 lcpcli-0.1.2/corpert/setup.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.877719 lcpcli-0.1.2/lcp-upload/
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.873718 lcpcli-0.1.2/lcp-upload/build/
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.873718 lcpcli-0.1.2/lcp-upload/build/lib/
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.877719 lcpcli-0.1.2/lcp-upload/build/lib/lcp_upload/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      109 2023-12-05 17:12:33.000000 lcpcli-0.1.2/lcp-upload/build/lib/lcp_upload/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      118 2023-12-05 17:12:33.000000 lcpcli-0.1.2/lcp-upload/build/lib/lcp_upload/__main__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1880 2023-12-05 17:12:33.000000 lcpcli-0.1.2/lcp-upload/build/lib/lcp_upload/cli.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    10696 2023-12-06 08:28:09.000000 lcpcli-0.1.2/lcp-upload/build/lib/lcp_upload/lcp_upload.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.877719 lcpcli-0.1.2/lcp-upload/lcp_upload/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      109 2023-12-05 17:12:33.000000 lcpcli-0.1.2/lcp-upload/lcp_upload/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      118 2023-12-05 17:12:33.000000 lcpcli-0.1.2/lcp-upload/lcp_upload/__main__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1880 2023-12-05 17:12:33.000000 lcpcli-0.1.2/lcp-upload/lcp_upload/cli.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    10696 2023-12-06 08:28:09.000000 lcpcli-0.1.2/lcp-upload/lcp_upload/lcp_upload.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       89 2023-12-05 17:12:33.000000 lcpcli-0.1.2/lcp-upload/requirements.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      761 2023-12-05 17:12:33.000000 lcpcli-0.1.2/lcp-upload/setup.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.877719 lcpcli-0.1.2/lcpcli/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       50 2023-12-05 17:03:46.000000 lcpcli-0.1.2/lcpcli/__init__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      199 2023-12-05 17:04:24.000000 lcpcli-0.1.2/lcpcli/__main__.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2843 2023-12-06 14:11:50.000000 lcpcli-0.1.2/lcpcli/cli.py
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2371 2024-03-18 16:39:46.000000 lcpcli-0.1.2/lcpcli/lcpcli.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-03-20 15:14:00.877719 lcpcli-0.1.2/lcpcli.egg-info/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)    10342 2024-03-20 15:14:00.000000 lcpcli-0.1.2/lcpcli.egg-info/PKG-INFO
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1614 2024-03-20 15:14:00.000000 lcpcli-0.1.2/lcpcli.egg-info/SOURCES.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        1 2024-03-20 15:14:00.000000 lcpcli-0.1.2/lcpcli.egg-info/dependency_links.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      162 2024-03-20 15:14:00.000000 lcpcli-0.1.2/lcpcli.egg-info/requires.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       26 2024-03-20 15:14:00.000000 lcpcli-0.1.2/lcpcli.egg-info/top_level.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        1 2023-12-06 08:55:49.000000 lcpcli-0.1.2/lcpcli.egg-info/zip-safe
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1062 2024-03-20 15:13:48.000000 lcpcli-0.1.2/pyproject.toml
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       38 2024-03-20 15:14:00.877719 lcpcli-0.1.2/setup.cfg
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      735 2024-02-28 10:19:59.000000 lcpcli-0.1.2/setup.py
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1058 2023-12-13 14:52:19.000000 lcpcli-0.1.3/LICENSE.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)    11986 2024-04-29 16:56:20.530002 lcpcli-0.1.3/PKG-INFO
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    11021 2024-04-09 11:16:26.000000 lcpcli-0.1.3/README.md
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/bin/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       41 2023-12-05 17:05:43.000000 lcpcli-0.1.3/bin/lcpcli
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/_legacy_process_files/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    16490 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/_legacy_process_files/process_opensubtitles.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    12104 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/_legacy_process_files/process_sparcling.py
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/build/
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/build/lib/
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/build/lib/corpert/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       52 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/build/lib/corpert/__init__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      205 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/build/lib/corpert/__main__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1318 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/build/lib/corpert/cli.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    17713 2024-02-28 15:54:29.000000 lcpcli-0.1.3/corpert/build/lib/corpert/corpert.py
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/build/lib/corpert/parsers/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        0 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/build/lib/corpert/parsers/__init__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     3039 2024-02-28 15:58:27.000000 lcpcli-0.1.3/corpert/build/lib/corpert/parsers/_parser.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     7418 2024-02-27 16:14:48.000000 lcpcli-0.1.3/corpert/build/lib/corpert/parsers/conllu.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      370 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/build/lib/corpert/parsers/json.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    10547 2024-02-27 16:14:48.000000 lcpcli-0.1.3/corpert/build/lib/corpert/parsers/tei.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     5885 2024-02-27 16:14:48.000000 lcpcli-0.1.3/corpert/build/lib/corpert/parsers/vert.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    13067 2024-02-29 13:04:27.000000 lcpcli-0.1.3/corpert/build/lib/corpert/utils.py
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/corpert/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       52 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/corpert/__init__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      205 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/corpert/__main__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1318 2024-04-24 13:45:22.000000 lcpcli-0.1.3/corpert/corpert/cli.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    16353 2024-04-24 13:52:37.000000 lcpcli-0.1.3/corpert/corpert/corpert.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    13554 2024-04-12 14:57:44.000000 lcpcli-0.1.3/corpert/corpert/lcp_corpus_template.json
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/corpert/corpert/parsers/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        0 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/corpert/parsers/__init__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    30262 2024-04-29 16:47:45.000000 lcpcli-0.1.3/corpert/corpert/parsers/_parser.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    12612 2024-04-24 14:00:59.000000 lcpcli-0.1.3/corpert/corpert/parsers/conllu.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      370 2023-12-05 17:12:56.000000 lcpcli-0.1.3/corpert/corpert/parsers/json.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    10547 2024-02-27 16:14:48.000000 lcpcli-0.1.3/corpert/corpert/parsers/tei.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     5885 2024-02-27 16:14:48.000000 lcpcli-0.1.3/corpert/corpert/parsers/vert.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    17393 2024-04-29 16:35:07.000000 lcpcli-0.1.3/corpert/corpert/utils.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       71 2024-03-18 14:41:46.000000 lcpcli-0.1.3/corpert/requirements.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      809 2023-12-06 14:34:53.000000 lcpcli-0.1.3/corpert/setup.py
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/lcp-upload/
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/lcp-upload/build/
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/lcp-upload/build/lib/
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/lcp-upload/build/lib/lcp_upload/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      109 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/build/lib/lcp_upload/__init__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      118 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/build/lib/lcp_upload/__main__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1880 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/build/lib/lcp_upload/cli.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    10696 2023-12-06 08:28:09.000000 lcpcli-0.1.3/lcp-upload/build/lib/lcp_upload/lcp_upload.py
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/lcp-upload/lcp_upload/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      109 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/lcp_upload/__init__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      118 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/lcp_upload/__main__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1880 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/lcp_upload/cli.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    10696 2023-12-06 08:28:09.000000 lcpcli-0.1.3/lcp-upload/lcp_upload/lcp_upload.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       89 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/requirements.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      761 2023-12-05 17:12:33.000000 lcpcli-0.1.3/lcp-upload/setup.py
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/lcpcli/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       50 2023-12-05 17:03:46.000000 lcpcli-0.1.3/lcpcli/__init__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      199 2023-12-05 17:04:24.000000 lcpcli-0.1.3/lcpcli/__main__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2843 2023-12-06 14:11:50.000000 lcpcli-0.1.3/lcpcli/cli.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2371 2024-03-18 16:39:46.000000 lcpcli-0.1.3/lcpcli/lcpcli.py
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-29 16:56:20.530002 lcpcli-0.1.3/lcpcli.egg-info/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)    11986 2024-04-29 16:56:20.000000 lcpcli-0.1.3/lcpcli.egg-info/PKG-INFO
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1614 2024-04-29 16:56:20.000000 lcpcli-0.1.3/lcpcli.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        1 2024-04-29 16:56:20.000000 lcpcli-0.1.3/lcpcli.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      162 2024-04-29 16:56:20.000000 lcpcli-0.1.3/lcpcli.egg-info/requires.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       26 2024-04-29 16:56:20.000000 lcpcli-0.1.3/lcpcli.egg-info/top_level.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        1 2023-12-06 08:55:49.000000 lcpcli-0.1.3/lcpcli.egg-info/zip-safe
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     1062 2024-04-29 16:56:13.000000 lcpcli-0.1.3/pyproject.toml
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       38 2024-04-29 16:56:20.530002 lcpcli-0.1.3/setup.cfg
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      735 2024-02-28 10:19:59.000000 lcpcli-0.1.3/setup.py
```

### Comparing `lcpcli-0.1.2/LICENSE.txt` & `lcpcli-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/PKG-INFO` & `lcpcli-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcpcli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Helper for converting CONLLU files and uploading the corpus to LCP
 Home-page: 
 Author: Jeremy Zehr and Jonathan Schaber
 Author-email: Jeremy Zehr <jeremy.zehr@uzh.ch>
 Project-URL: Homepage, https://gitlab.uzh.ch/LiRI/projects/lcpcli
 Project-URL: Issues, https://gitlab.uzh.ch/LiRI/projects/lcpcli/-/issues
 Keywords: corpus,linguistics,corpora,conll,tei,vert
@@ -133,14 +133,81 @@
         }
     }
 },
 ```
 
 Make sure to set the `abstract`, `layerType` and `contains` attributes as illustrated above. See the section [Convert and Upload](#convert-and-upload) for a full example of a template `.json` file.
 
+
+#### Global attributes
+
+In some cases, it makes sense for multiple entity types to share references: in those cases, they can define _global attributes_. An example of a global attribute is a speaker or an agent that can have a name, an age, etc. and be associated with both a segment (a sentence) and, say, a gesture. The corpus template would include definitions along these lines:
+
+```json
+"globalAttributes": {
+    "agent": {
+        "type": "dict",
+        "keys": {
+            "name": {
+                "type": "text"
+            },
+            "age": {
+                "type": "number"
+            }
+        }
+    }
+},
+"layer": {
+    "Segment": {
+        "abstract": false,
+        "layerType": "span",
+        "contains": "Token",
+        "attributes": {
+            "agent": {
+                "ref": "agent"
+            }
+        }
+    },
+    "Gesture": {
+        "abstract": false,
+        "layerType": "unit",
+        "anchoring": {
+            "time": true
+        },
+        "attributes": {
+            "agent": {
+                "ref": "agent"
+            }
+        }
+    }
+}
+```
+
+You should include a file named `global_attribute_agent.csv` (mind the singular on `attribute`) with three columns: `agent_id`, `name` and `age`, and reference the values of `agent_id` appropriately as a sentence-level comment in your CoNLL-U files as well as in a file named `gesture.tsv`. For example:
+
+*global_attribute_agent.tsv*:
+```tsv
+agent_id	agent
+10	{"name": "Jane Doe", "age": 37}
+```
+
+CoNLL-U file:
+```conllu
+# sent_id = 1
+# agent_id = 10
+The the _ _ _
+```
+
+*gesture.tsv*:
+```tsv
+gesture_id	agent_id	frame_range
+1	10	[2345,5678]
+```
+
+
 ### Convert and Upload
 
 1. Create a directory in which you have all your properly-fromatted CONLLU files
 
 2. In the same directory, create a template `.json` file that describes your corpus structure (see above about the `attributes` key on `Document` and `Segment`), for example:
 
 ```json
```

### Comparing `lcpcli-0.1.2/README.md` & `lcpcli-0.1.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -106,14 +106,81 @@
         }
     }
 },
 ```
 
 Make sure to set the `abstract`, `layerType` and `contains` attributes as illustrated above. See the section [Convert and Upload](#convert-and-upload) for a full example of a template `.json` file.
 
+
+#### Global attributes
+
+In some cases, it makes sense for multiple entity types to share references: in those cases, they can define _global attributes_. An example of a global attribute is a speaker or an agent that can have a name, an age, etc. and be associated with both a segment (a sentence) and, say, a gesture. The corpus template would include definitions along these lines:
+
+```json
+"globalAttributes": {
+    "agent": {
+        "type": "dict",
+        "keys": {
+            "name": {
+                "type": "text"
+            },
+            "age": {
+                "type": "number"
+            }
+        }
+    }
+},
+"layer": {
+    "Segment": {
+        "abstract": false,
+        "layerType": "span",
+        "contains": "Token",
+        "attributes": {
+            "agent": {
+                "ref": "agent"
+            }
+        }
+    },
+    "Gesture": {
+        "abstract": false,
+        "layerType": "unit",
+        "anchoring": {
+            "time": true
+        },
+        "attributes": {
+            "agent": {
+                "ref": "agent"
+            }
+        }
+    }
+}
+```
+
+You should include a file named `global_attribute_agent.csv` (mind the singular on `attribute`) with three columns: `agent_id`, `name` and `age`, and reference the values of `agent_id` appropriately as a sentence-level comment in your CoNLL-U files as well as in a file named `gesture.tsv`. For example:
+
+*global_attribute_agent.tsv*:
+```tsv
+agent_id	agent
+10	{"name": "Jane Doe", "age": 37}
+```
+
+CoNLL-U file:
+```conllu
+# sent_id = 1
+# agent_id = 10
+The the _ _ _
+```
+
+*gesture.tsv*:
+```tsv
+gesture_id	agent_id	frame_range
+1	10	[2345,5678]
+```
+
+
 ### Convert and Upload
 
 1. Create a directory in which you have all your properly-fromatted CONLLU files
 
 2. In the same directory, create a template `.json` file that describes your corpus structure (see above about the `attributes` key on `Document` and `Segment`), for example:
 
 ```json
```

### Comparing `lcpcli-0.1.2/corpert/_legacy_process_files/process_opensubtitles.py` & `lcpcli-0.1.3/corpert/_legacy_process_files/process_opensubtitles.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/corpert/_legacy_process_files/process_sparcling.py` & `lcpcli-0.1.3/corpert/_legacy_process_files/process_sparcling.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/corpert/build/lib/corpert/cli.py` & `lcpcli-0.1.3/corpert/build/lib/corpert/cli.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/corpert/build/lib/corpert/corpert.py` & `lcpcli-0.1.3/corpert/build/lib/corpert/corpert.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/corpert/build/lib/corpert/parsers/_parser.py` & `lcpcli-0.1.3/corpert/build/lib/corpert/parsers/_parser.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/corpert/build/lib/corpert/parsers/conllu.py` & `lcpcli-0.1.3/corpert/build/lib/corpert/parsers/conllu.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/corpert/build/lib/corpert/parsers/tei.py` & `lcpcli-0.1.3/corpert/build/lib/corpert/parsers/tei.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/corpert/build/lib/corpert/parsers/vert.py` & `lcpcli-0.1.3/corpert/build/lib/corpert/parsers/vert.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/corpert/build/lib/corpert/utils.py` & `lcpcli-0.1.3/corpert/build/lib/corpert/utils.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/corpert/corpert/cli.py` & `lcpcli-0.1.3/corpert/corpert/cli.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/corpert/corpert/parsers/conllu.py` & `lcpcli-0.1.3/corpert/corpert/parsers/conllu.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     "deprel",
     "deps",
     "misc",
 ]
 
 
 class CONLLUParser(Parser):
-    def __init__(self):
-        super().__init__()
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
         self.word      = CustomDict()
         self.lemma     = CustomDict()
         self.ufeats    = CustomDict()
         self.jsonbMisc = CustomDict()
         self.xpos      = set()
         self.cur_idx   = 1
         self.cur_word  = 1
@@ -61,15 +61,15 @@
 
 
     @property
     def right(self):
         return self.left + 1
 
 
-    def parse_sentence(self, sentence_lines) -> tuple[Document | None, Segment | None]:
+    def parse_sentence(self, sentence_lines, config={}) -> tuple[Document | None, Segment | None]:
         """
         Take a list of ConLLU lines (comments + tokens) and output (sentence, new_doc | None)
         """
         new_doc = None
         current_sentence = {"meta": {}, "text": []}
         for line in sentence_lines:
             if re.match(r"# newdoc", line):
@@ -133,57 +133,81 @@
                             pv = pv.strip()
                             if pk in ("start","end"):
                                 token.frame_range = token.frame_range or [0,0]
                                 token.frame_range[0 if pk=="start" else 1] = int(25.0 * float(pv))
                                 has_frame_range = True
                             else:
                                 misc[pk] = str(pv)
-                        if misc:
-                            token.attributes["misc"] = Meta("misc", misc)
+                        token.attributes["misc"] = Meta("misc", misc)
                     else:
                         token.attributes[k] = Text(k,v)
 
             # if has_frame_range:
             #     assert all(t.frame_range is not None for t in sentence.tokens), AttributeError("Some tokens miss start-end time information")
 
             # sentence.tokens = current_sentence["text"]
-            if current_sentence["meta"]:
-                sentence.attributes["meta"] = Meta("meta", current_sentence["meta"])
+            meta = current_sentence["meta"]
+            if config:
+                # If a config was provided, pop any entry from meta that's listed as a main attribute
+                seg_layer = config.get("firstClass", {}).get("segment", "")
+                seg_config = config.get("layer", {}).get(seg_layer, {}).get("attributes", {})
+                segment_containers = [
+                    layer.lower()
+                    for layer, props in config.get("layer", {}).items()
+                    if props.get("layerType", "") == "span" and props.get("contains", "") == seg_layer
+                ]
+                for attr_name in seg_config:
+                    name = attr_name
+                    if name+"_id" in meta:
+                        name = name + "_id"
+                    elif name not in meta:
+                        continue
+                    a = meta.pop(name)
+                    sentence.attributes[name] = Attribute(name, a)
+                for seg_container in segment_containers:
+                    attr_name = next( (k for k in meta.keys() if k.lower() == seg_container) , None )
+                    if attr_name is None:
+                        continue
+                    sentence.attributes[attr_name] = Text(attr_name, meta.pop(attr_name))
+            if meta:
+                if name.lower() in segment_containers:
+                    sentence.attributes[name] = Text(name, meta.pop(name))
+                sentence.attributes["meta"] = Meta("meta", meta)
 
         if new_doc:
             doc = Document()
             if id := new_doc.get("id"):
                 new_doc["meta"]["name"] = id
             doc.attributes["meta"] = Meta("meta", new_doc["meta"])
             doc.first_sentence = sentence
             new_doc = doc
 
         return (sentence, new_doc)
         # return (current_sentence, new_doc)
 
 
-    def parse_generator(self, reader):
+    def parse_generator(self, reader, config={}):
         checked_first_line_for_conllu_plus = False
         sentence_lines = []
         while line := reader.readline():
             l = line.strip()
             if l:
                 if not checked_first_line_for_conllu_plus and l.startswith("# global.columns = "):
                     self._features = [f.lower() for f in l[19:].split()]
                 else:
                     sentence_lines.append(line)
             else:
                 # empty line: new sentence
                 if sentence_lines:
-                    yield self.parse_sentence(sentence_lines)
+                    yield self.parse_sentence(sentence_lines, config=config)
                 sentence_lines = []
             checked_first_line_for_conllu_plus = True
 
         if sentence_lines:
-            yield self.parse_sentence(sentence_lines)
+            yield self.parse_sentence(sentence_lines, config=config)
 
 
     def parse(self, content):
         """
         When iterator is True, yield ({id,meta,text},None|{id,meta}) -- content should have a readline method and 
         When iterator is False, return a writable string
         """
```

### Comparing `lcpcli-0.1.2/corpert/corpert/parsers/tei.py` & `lcpcli-0.1.3/corpert/corpert/parsers/tei.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/corpert/corpert/parsers/vert.py` & `lcpcli-0.1.3/corpert/corpert/parsers/vert.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/corpert/corpert/utils.py` & `lcpcli-0.1.3/corpert/corpert/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 import json
+import os
 import re
 import uuid
 
 from datetime import date
 
+def get_ci(d: dict, p: str, default={}):
+    """
+    Case-insensitive get on an object
+    """
+    return next((v for n, v in d.items() if n.lower() == p.lower()), default)
+
 class CustomDict:
     def __init__(self, is_ufeat=False):
         self._dictionary = {}
         self._max        = 1
 
     def __str__(self):
         return str(dict(sorted(self._dictionary)))
@@ -402,14 +409,35 @@
         #     else:
         #         self.glob.docs[self._id] = [start_char, end_char]
 
     def process(self):
         self._process_lines()
 
 
+class Table:
+    def __init__(self, name, path, config = {}):
+        self.name = name
+        self.path = os.path.join(path,f"{name}.csv")
+        self.file = open(self.path, "a")
+        self.config = config
+        self.cursor = 1
+        self.currentEntity = dict()
+        self.previousEntity = None
+        self.colNames = [],
+        self.labels = dict()
+        self.texts = dict()
+        self.deps = dict()
+        self.anchor_right = 0
+        self.non_null_attributes = {}
+        self.sep = "\t"
+
+    def write(self, row: list):
+        self.file.write( self.sep.join([str(x) for x in row]) + "\n" )
+
+
 class Attribute:
     def __init__(self, name, value):
         self.name = name
         self._value = value
     @property
     def value(self):
         if not self._value:
@@ -468,15 +496,15 @@
 
 doc_id = 0
 class Document(EntityType):
     def __init__(self):
         super().__init__()
         global doc_id
         doc_id += 1
-        self.id = token_id
+        self.id = doc_id
         self.char_range_start: int = 0
         self.frame_range: list[int] = [0,0]
         self.left = 1
         self.right = 2
 
 # Compute left/right from parent only once
 class NestedSet:
```

### Comparing `lcpcli-0.1.2/corpert/setup.py` & `lcpcli-0.1.3/corpert/setup.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/lcp-upload/build/lib/lcp_upload/cli.py` & `lcpcli-0.1.3/lcp-upload/build/lib/lcp_upload/cli.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/lcp-upload/build/lib/lcp_upload/lcp_upload.py` & `lcpcli-0.1.3/lcp-upload/build/lib/lcp_upload/lcp_upload.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/lcp-upload/lcp_upload/cli.py` & `lcpcli-0.1.3/lcp-upload/lcp_upload/cli.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/lcp-upload/lcp_upload/lcp_upload.py` & `lcpcli-0.1.3/lcp-upload/lcp_upload/lcp_upload.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/lcp-upload/setup.py` & `lcpcli-0.1.3/lcp-upload/setup.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/lcpcli/cli.py` & `lcpcli-0.1.3/lcpcli/cli.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/lcpcli/lcpcli.py` & `lcpcli-0.1.3/lcpcli/lcpcli.py`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/lcpcli.egg-info/PKG-INFO` & `lcpcli-0.1.3/lcpcli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lcpcli
-Version: 0.1.2
+Version: 0.1.3
 Summary: Helper for converting CONLLU files and uploading the corpus to LCP
 Home-page: 
 Author: Jeremy Zehr and Jonathan Schaber
 Author-email: Jeremy Zehr <jeremy.zehr@uzh.ch>
 Project-URL: Homepage, https://gitlab.uzh.ch/LiRI/projects/lcpcli
 Project-URL: Issues, https://gitlab.uzh.ch/LiRI/projects/lcpcli/-/issues
 Keywords: corpus,linguistics,corpora,conll,tei,vert
@@ -133,14 +133,81 @@
         }
     }
 },
 ```
 
 Make sure to set the `abstract`, `layerType` and `contains` attributes as illustrated above. See the section [Convert and Upload](#convert-and-upload) for a full example of a template `.json` file.
 
+
+#### Global attributes
+
+In some cases, it makes sense for multiple entity types to share references: in those cases, they can define _global attributes_. An example of a global attribute is a speaker or an agent that can have a name, an age, etc. and be associated with both a segment (a sentence) and, say, a gesture. The corpus template would include definitions along these lines:
+
+```json
+"globalAttributes": {
+    "agent": {
+        "type": "dict",
+        "keys": {
+            "name": {
+                "type": "text"
+            },
+            "age": {
+                "type": "number"
+            }
+        }
+    }
+},
+"layer": {
+    "Segment": {
+        "abstract": false,
+        "layerType": "span",
+        "contains": "Token",
+        "attributes": {
+            "agent": {
+                "ref": "agent"
+            }
+        }
+    },
+    "Gesture": {
+        "abstract": false,
+        "layerType": "unit",
+        "anchoring": {
+            "time": true
+        },
+        "attributes": {
+            "agent": {
+                "ref": "agent"
+            }
+        }
+    }
+}
+```
+
+You should include a file named `global_attribute_agent.csv` (mind the singular on `attribute`) with three columns: `agent_id`, `name` and `age`, and reference the values of `agent_id` appropriately as a sentence-level comment in your CoNLL-U files as well as in a file named `gesture.tsv`. For example:
+
+*global_attribute_agent.tsv*:
+```tsv
+agent_id	agent
+10	{"name": "Jane Doe", "age": 37}
+```
+
+CoNLL-U file:
+```conllu
+# sent_id = 1
+# agent_id = 10
+The the _ _ _
+```
+
+*gesture.tsv*:
+```tsv
+gesture_id	agent_id	frame_range
+1	10	[2345,5678]
+```
+
+
 ### Convert and Upload
 
 1. Create a directory in which you have all your properly-fromatted CONLLU files
 
 2. In the same directory, create a template `.json` file that describes your corpus structure (see above about the `attributes` key on `Document` and `Segment`), for example:
 
 ```json
```

### Comparing `lcpcli-0.1.2/lcpcli.egg-info/SOURCES.txt` & `lcpcli-0.1.3/lcpcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lcpcli-0.1.2/pyproject.toml` & `lcpcli-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lcpcli"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Jeremy Zehr", email="jeremy.zehr@uzh.ch" },
 ]
 description = "Helper for converting CONLLU files and uploading the corpus to LCP"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `lcpcli-0.1.2/setup.py` & `lcpcli-0.1.3/setup.py`

 * *Files identical despite different names*

