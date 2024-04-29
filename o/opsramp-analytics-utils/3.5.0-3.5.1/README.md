# Comparing `tmp/opsramp-analytics-utils-3.5.0.tar.gz` & `tmp/opsramp-analytics-utils-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opsramp-analytics-utils-3.5.0.tar", last modified: Tue Apr 23 07:25:10 2024, max compression
+gzip compressed data, was "opsramp-analytics-utils-3.5.1.tar", last modified: Mon Apr 29 12:20:31 2024, max compression
```

## Comparing `opsramp-analytics-utils-3.5.0.tar` & `opsramp-analytics-utils-3.5.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-23 07:25:10.314687 opsramp-analytics-utils-3.5.0/
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1073 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/LICENSE
--rw-r--r--   0 rajumummidi   (502) staff       (20)      186 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/MANIFEST.in
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-04-23 07:25:10.314565 opsramp-analytics-utils-3.5.0/PKG-INFO
--rw-r--r--   0 rajumummidi   (502) staff       (20)      711 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/README.md
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-23 07:25:10.307367 opsramp-analytics-utils-3.5.0/analytics_sdk/
--rw-r--r--   0 rajumummidi   (502) staff       (20)       30 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/__init__.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-23 07:25:10.309597 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/
--rw-r--r--   0 rajumummidi   (502) staff       (20)      921 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/main.js
--rw-r--r--   0 rajumummidi   (502) staff       (20)  3321723 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/main.wrapper.css
--rw-r--r--   0 rajumummidi   (502) staff       (20)  2628164 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/main.wrapper.js
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-23 07:25:10.312700 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/
--rw-r--r--   0 rajumummidi   (502) staff       (20)      320 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)    34172 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
--rw-r--r--   0 rajumummidi   (502) staff       (20)   148200 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)    64440 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
--rw-r--r--   0 rajumummidi   (502) staff       (20)    29136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
--rw-r--r--   0 rajumummidi   (502) staff       (20)    64608 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
--rw-r--r--   0 rajumummidi   (502) staff       (20)      602 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)      861 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1403 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
--rw-r--r--   0 rajumummidi   (502) staff       (20)     7536 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
--rw-r--r--   0 rajumummidi   (502) staff       (20)    11968 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
--rw-r--r--   0 rajumummidi   (502) staff       (20)    12136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
--rw-r--r--   0 rajumummidi   (502) staff       (20)      733 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-23 07:25:10.313120 opsramp-analytics-utils-3.5.0/analytics_sdk/api/
--rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/api/__init__.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    17387 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/api/api_client.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     9382 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/api/api_task.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)      992 2024-01-29 06:36:39.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/api/thread_process.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    17374 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/api_client.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     4100 2024-03-08 08:04:41.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/components.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/constants.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     4730 2024-03-08 08:03:00.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/oap_dash.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-23 07:25:10.313519 opsramp-analytics-utils-3.5.0/analytics_sdk/process/
--rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/process/__init__.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     5809 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/process/process.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     4692 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/process/querybuilder.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-23 07:25:10.313868 opsramp-analytics-utils-3.5.0/analytics_sdk/renderer/
--rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/renderer/__init__.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    35042 2024-01-29 09:30:11.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/renderer/excel.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)     2887 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/renderer/pdf.py
--rw-r--r--   0 rajumummidi   (502) staff       (20)    43575 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.0/analytics_sdk/utilities.py
-drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-23 07:25:10.314398 opsramp-analytics-utils-3.5.0/opsramp_analytics_utils.egg-info/
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-04-23 07:25:10.000000 opsramp-analytics-utils-3.5.0/opsramp_analytics_utils.egg-info/PKG-INFO
--rw-r--r--   0 rajumummidi   (502) staff       (20)     1698 2024-04-23 07:25:10.000000 opsramp-analytics-utils-3.5.0/opsramp_analytics_utils.egg-info/SOURCES.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)        1 2024-04-23 07:25:10.000000 opsramp-analytics-utils-3.5.0/opsramp_analytics_utils.egg-info/dependency_links.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)      125 2024-04-23 07:25:10.000000 opsramp-analytics-utils-3.5.0/opsramp_analytics_utils.egg-info/requires.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)       14 2024-04-23 07:25:10.000000 opsramp-analytics-utils-3.5.0/opsramp_analytics_utils.egg-info/top_level.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)      139 2024-04-23 07:16:43.000000 opsramp-analytics-utils-3.5.0/requires-install.txt
--rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2024-04-23 07:25:10.314735 opsramp-analytics-utils-3.5.0/setup.cfg
--rw-r--r--   0 rajumummidi   (502) staff       (20)      943 2024-04-23 07:18:57.000000 opsramp-analytics-utils-3.5.0/setup.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.133774 opsramp-analytics-utils-3.5.1/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1073 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/LICENSE
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      186 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/MANIFEST.in
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-04-29 12:20:31.133632 opsramp-analytics-utils-3.5.1/PKG-INFO
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      711 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/README.md
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.119335 opsramp-analytics-utils-3.5.1/analytics_sdk/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       30 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/__init__.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.122779 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      921 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/main.js
+-rw-r--r--   0 rajumummidi   (502) staff       (20)  3321723 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/main.wrapper.css
+-rw-r--r--   0 rajumummidi   (502) staff       (20)  2628164 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/main.wrapper.js
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.130369 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      320 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/close.82b1ae2d.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    34172 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff
+-rw-r--r--   0 rajumummidi   (502) staff       (20)   148200 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    64440 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    29136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    64608 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      602 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      861 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1403 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     7536 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    11968 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    12136 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      733 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.130945 opsramp-analytics-utils-3.5.1/analytics_sdk/api/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/api/__init__.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    17387 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/api/api_client.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     9382 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/api/api_task.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      992 2024-01-29 06:36:39.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/api/thread_process.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    17374 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/api_client.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     4100 2024-03-08 08:04:41.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/components.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/constants.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     4730 2024-03-08 08:03:00.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/oap_dash.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.132497 opsramp-analytics-utils-3.5.1/analytics_sdk/process/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/process/__init__.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     5809 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/process/process.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     4692 2024-02-15 10:44:56.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/process/querybuilder.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.132871 opsramp-analytics-utils-3.5.1/analytics_sdk/renderer/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        0 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/renderer/__init__.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    35159 2024-04-29 12:18:52.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/renderer/excel.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     2887 2023-11-28 12:48:38.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/renderer/pdf.py
+-rw-r--r--   0 rajumummidi   (502) staff       (20)    44741 2024-04-29 12:18:52.000000 opsramp-analytics-utils-3.5.1/analytics_sdk/utilities.py
+drwxr-xr-x   0 rajumummidi   (502) staff       (20)        0 2024-04-29 12:20:31.133448 opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1328 2024-04-29 12:20:31.000000 opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/PKG-INFO
+-rw-r--r--   0 rajumummidi   (502) staff       (20)     1698 2024-04-29 12:20:31.000000 opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)        1 2024-04-29 12:20:31.000000 opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      130 2024-04-29 12:20:31.000000 opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/requires.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       14 2024-04-29 12:20:31.000000 opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/top_level.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      144 2024-04-26 11:14:56.000000 opsramp-analytics-utils-3.5.1/requires-install.txt
+-rw-r--r--   0 rajumummidi   (502) staff       (20)       38 2024-04-29 12:20:31.133829 opsramp-analytics-utils-3.5.1/setup.cfg
+-rw-r--r--   0 rajumummidi   (502) staff       (20)      943 2024-04-29 10:22:13.000000 opsramp-analytics-utils-3.5.1/setup.py
```

### Comparing `opsramp-analytics-utils-3.5.0/LICENSE` & `opsramp-analytics-utils-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/PKG-INFO` & `opsramp-analytics-utils-3.5.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.5.0
+Version: 3.5.1
 Summary: OpsRamp Analytics SDK
 Home-page: UNKNOWN
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.5.0/README.md` & `opsramp-analytics-utils-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/main.js` & `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/main.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/main.wrapper.css` & `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/main.wrapper.css`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/main.wrapper.js` & `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/main.wrapper.js`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff` & `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.487f60cd.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg` & `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.52a41d35.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf` & `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.8be26641.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2` & `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.8fcd07de.woff2`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot` & `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/fontello.d35868c4.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg` & `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/icon-copy.c16adda9.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg` & `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/icon-edit.ae3b1e05.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg` & `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/icon-remove.184d1ffb.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff` & `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/revicons.04eb8fc5.woff`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf` & `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/revicons.17629a5d.ttf`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot` & `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/revicons.2feb69cc.eot`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg` & `opsramp-analytics-utils-3.5.1/analytics_sdk/analysis-wrapper/media/transparent-bg.5f803547.svg`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/api/api_client.py` & `opsramp-analytics-utils-3.5.1/analytics_sdk/api/api_client.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/api/api_task.py` & `opsramp-analytics-utils-3.5.1/analytics_sdk/api/api_task.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/api/thread_process.py` & `opsramp-analytics-utils-3.5.1/analytics_sdk/api/thread_process.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/api_client.py` & `opsramp-analytics-utils-3.5.1/analytics_sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/components.py` & `opsramp-analytics-utils-3.5.1/analytics_sdk/components.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/oap_dash.py` & `opsramp-analytics-utils-3.5.1/analytics_sdk/oap_dash.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/process/process.py` & `opsramp-analytics-utils-3.5.1/analytics_sdk/process/process.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/process/querybuilder.py` & `opsramp-analytics-utils-3.5.1/analytics_sdk/process/querybuilder.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/renderer/excel.py` & `opsramp-analytics-utils-3.5.1/analytics_sdk/renderer/excel.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,16 @@
     Series,
     LineChart,
     PieChart
 )
 from openpyxl.chart.series import DataPoint
 from openpyxl.cell.cell import ILLEGAL_CHARACTERS_RE
 import re
+from decimal import Decimal
+from fractions import Fraction
 
 from analytics_sdk.utilities import (
     BASE_API_URL,
     APP_ID,
     API_KEY,
     API_SECRET,
     API_RETRY,
@@ -110,14 +112,24 @@
         api_proce_after_time = time.time()
         api_proce_diff = diff_sec(api_proce_before_time, api_proce_after_time)
         if api_proce_diff > API_TIME_STACKS:
             logging.info('Get excel summary API response took %d (greater than %d) seconds', api_proce_diff, API_TIME_STACKS)
 
         self.res = res
 
+    def get_value(self, value):
+        if value:
+            try:
+                value = float(value)
+                return value
+            except ValueError:
+                return value
+        return value
+    
+
     def _load_data(self, ws, data, row_start, col_start, adjust_column=True, x_axis_date_format=None):
         column_widths = {}
         if isinstance(data, list):
             if len(data) >= 1000005:
                 data = data[0:1000005]
 
         for row_delta, row in enumerate(data):
@@ -125,28 +137,26 @@
                 col = col_start + col_delta
                 cell = ws.cell(row=row_start+row_delta, column=col)
                 if x_axis_date_format and row_delta > 0 and col_delta == 0:
                     cell.value = datetime.strptime(val, x_axis_date_format).date()
                 else:
                     try:
                         if APP_ID == 'AVAILABILITY-DETAILS':
-                            if isinstance(val, str) and 'AVAILABILITY_PERCENT_' in val:
-                                val = val.replace('AVAILABILITY_PERCENT_', '')
-                                if float(val) == 100:
-                                    cell.fill = PatternFill("solid", fgColor="27ae60")
-                                elif float(val)>=90 and float(val)<100:
-                                    cell.fill = PatternFill("solid", fgColor="f39c12")
-                                elif float(val) > 0 and float(val) < 90:
-                                    cell.fill = PatternFill("solid", fgColor="e85242")
-                        cell.value = val
+                            if isinstance(val, str) and 'COLOR-CODE_' in val:
+                                vals = val.split('_') #COLOR-CODE_{color_code}_{value}
+                                if len(vals) == 3:
+                                    val = vals[2]
+                                    if vals[1] is not None and len(vals[1]):
+                                        cell.fill = PatternFill("solid", fgColor=vals[1])
+                        cell.value = self.get_value(val)
                     except Exception as e:
                         if isinstance(val, str):
                             cell.value = ILLEGAL_CHARACTERS_RE.sub(r'', val)
                         else:
-                            cell.value = val
+                            cell.value = self.get_value(val)
                 if col in column_widths:
                     column_widths[col] = max(len(str(val)), column_widths[col])
                 else:
                     column_widths[col] = max(len(str(val)), ws.column_dimensions[get_column_letter(col)].width)
         # handle cell width
         if adjust_column:
             for col, column_width in column_widths.items():
```

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/renderer/pdf.py` & `opsramp-analytics-utils-3.5.1/analytics_sdk/renderer/pdf.py`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/analytics_sdk/utilities.py` & `opsramp-analytics-utils-3.5.1/analytics_sdk/utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import os
 import time
 import datetime
 import logging
 import random
 from io import BytesIO
-from datetime import datetime
 import json
 import traceback
+from datetime import datetime
+import pytz
 
 from urllib.request import urlopen
 from email.mime.text import MIMEText
 from email.mime.application import MIMEApplication
 from email.mime.multipart import MIMEMultipart
 from flask.wrappers import Response
 
@@ -41,14 +42,17 @@
 global ACCESS_KEY_ID, SECRET_ACCESS_KEY, REGION_NAME, BUCKET_NAME, ACCESS_HEADER, TOKEN_RETRIES
 
 if storage_name == 's3':
     ACCESS_KEY_ID = os.getenv('ACCESS_KEY_ID')
     SECRET_ACCESS_KEY = os.getenv('SECRET_ACCESS_KEY')
     REGION_NAME = os.getenv('REGION_NAME')
     BUCKET_NAME = os.getenv('BUCKET_NAME')
+    S3_ENDPOINT_URL = os.getenv('S3_ENDPOINT_URL', None) # This Property used for on-prime pods to connect cloud
+    if S3_ENDPOINT_URL is not None and 'https://' not in S3_ENDPOINT_URL:
+        S3_ENDPOINT_URL = 'https://'+S3_ENDPOINT_URL
 elif storage_name == 'ceph':
     ACCESS_KEY_ID = os.getenv('ACCESS_KEY_ID')
     SECRET_ACCESS_KEY = os.getenv('SECRET_ACCESS_KEY')
     BUCKET_NAME = os.getenv('BUCKET_NAME', 'analytics-apps')
     ENDPOINT_URL = os.getenv('ENDPOINT_URL')
 else:
     logger.info("No storages are found")
@@ -235,16 +239,17 @@
             res_object = data.getvalue()
             result = json.loads(res_object)
             if field:
                 result = result.get(field, default_value)
             return result
         else:
             logger.info("No storages are found")
-    except Exception:
+    except Exception as e:
         logger.error('An error occurred (NoSuchKey) when calling the GetObject operation: The specified key does not exist')
+        traceback.print_stack()
         pass
 
 
 def get_response(url, type, params=None):
     start_time = int(time.time())
     logging.info(f'api type: {type}, : url : {url}')
     res = call_get_requests(url, params=None, verify=True)
@@ -261,15 +266,17 @@
                         aws_secret_access_key=SECRET_ACCESS_KEY)
 
 
 def get_s3_client():
     return boto3.client('s3',
                         region_name=REGION_NAME,
                         aws_access_key_id=ACCESS_KEY_ID,
-                        aws_secret_access_key=SECRET_ACCESS_KEY)
+                        aws_secret_access_key=SECRET_ACCESS_KEY,
+                        endpoint_url=S3_ENDPOINT_URL
+                        )
     
 
 def get_ceph_resource():
     return boto3.resource('s3',
                             endpoint_url=ENDPOINT_URL,
                             aws_access_key_id=ACCESS_KEY_ID,
                             aws_secret_access_key=SECRET_ACCESS_KEY)
@@ -315,15 +322,16 @@
     :param: content: bytes
     :param: location: str
     '''
     if storage_name == 's3':
         s3 = boto3.resource('s3',
                             region_name=REGION_NAME,
                             aws_access_key_id=ACCESS_KEY_ID,
-                            aws_secret_access_key=SECRET_ACCESS_KEY)
+                            aws_secret_access_key=SECRET_ACCESS_KEY,
+                            endpoint_url=S3_ENDPOINT_URL)
         object_url = f'https://{BUCKET_NAME}.s3.{REGION_NAME}.amazonaws.com/{location}'
         try:
             s3.Bucket(BUCKET_NAME).put_object(Body=content,
                                                  Key=location)
             #return object_url
             return location
         except Exception:
@@ -970,14 +978,38 @@
     #colors = []
     for _ in range(num_colors):
         hex_color = '#{:06x}'.format(random.randint(0, 0xFFFFFF))
         colors.append(hex_color)
     return colors
 
 
+def convert_datetime_tz_to_tz(date, format, fromTz, toTz):
+    if date is None or date == '-' or format is None:
+        return '-'
+    if fromTz is not None:
+        date = date.astimezone(fromTz)
+    if toTz is None or len(toTz) <= 0:
+        toTz = 'UTC'
+    if toTz is not None:
+        date_obj = datetime.strptime(date, "%Y-%m-%dT%H:%M:%S%z")
+        date = date_obj.astimezone(pytz.timezone(toTz))
+        date = date.strftime(format)
+        return date
+    return '-'
+
+
+def convert_date_time_with_format(date, format):
+    try:
+        date_obj = datetime.strptime(date, '%Y-%m-%dT%H:%M:%S%z')
+        formatted_date_str = date_obj.strftime(format)
+        return formatted_date_str
+    except Exception as e:
+        return '-'
+
+
 def update_run_progress(tenant_id, run_id, percent, message):
     url = BASE_API_URL + f'/reporting/api/v3/tenants/{tenant_id}/runs/{run_id}/progress'
     data = {
         "runningPercentage" : percent
     }
     res = call_put_requests(url , data=json.dumps(data), verify=False);
     if res == None or not res.ok:
```

### Comparing `opsramp-analytics-utils-3.5.0/opsramp_analytics_utils.egg-info/PKG-INFO` & `opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opsramp-analytics-utils
-Version: 3.5.0
+Version: 3.5.1
 Summary: OpsRamp Analytics SDK
 Home-page: UNKNOWN
 Author: OpsRamp
 Author-email: opsramp@support.com
 License: UNKNOWN
 Description: ## OpsRamp Analytics Utilities
```

### Comparing `opsramp-analytics-utils-3.5.0/opsramp_analytics_utils.egg-info/SOURCES.txt` & `opsramp-analytics-utils-3.5.1/opsramp_analytics_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opsramp-analytics-utils-3.5.0/setup.py` & `opsramp-analytics-utils-3.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     with open("requires-{}.txt".format(req_type)) as fp:
         requires = (line.strip() for line in fp)
         return [req for req in requires if req and not req.startswith("#")]
 
 
 setuptools.setup(
     name="opsramp-analytics-utils",
-    version="3.5.0",
+    version="3.5.1",
     author="OpsRamp",
     author_email="opsramp@support.com",
     description="OpsRamp Analytics SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=read_req_file("install"),
     # url="https://github.com/opsramp/analytics-sdk",
```

