# Comparing `tmp/enconnect-0.2.3.tar.gz` & `tmp/enconnect-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enconnect-0.2.3.tar", last modified: Thu Apr 25 02:32:11 2024, max compression
+gzip compressed data, was "enconnect-0.3.0.tar", last modified: Mon Apr 29 04:53:00 2024, max compression
```

## Comparing `enconnect-0.2.3.tar` & `enconnect-0.3.0.tar`

### file list

```diff
@@ -1,53 +1,59 @@
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:11.689740 enconnect-0.2.3/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-04-08 22:20:24.000000 enconnect-0.2.3/LICENSE
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       33 2024-04-08 22:21:35.000000 enconnect-0.2.3/MANIFEST.in
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2753 2024-04-25 02:32:11.689740 enconnect-0.2.3/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2363 2024-04-14 13:59:58.000000 enconnect-0.2.3/README.md
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:11.688740 enconnect-0.2.3/enconnect/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-08 22:22:18.000000 enconnect-0.2.3/enconnect/__init__.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:11.688740 enconnect-0.2.3/enconnect/instagram/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      405 2024-04-13 00:00:49.000000 enconnect-0.2.3/enconnect/instagram/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3870 2024-04-25 02:26:38.000000 enconnect-0.2.3/enconnect/instagram/instagram.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      982 2024-04-12 05:18:12.000000 enconnect-0.2.3/enconnect/instagram/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:11.688740 enconnect-0.2.3/enconnect/instagram/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 04:42:12.000000 enconnect-0.2.3/enconnect/instagram/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1896 2024-04-15 09:01:50.000000 enconnect-0.2.3/enconnect/instagram/test/test_instagram.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:11.689740 enconnect-0.2.3/enconnect/philipshue/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:18.000000 enconnect-0.2.3/enconnect/philipshue/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2254 2024-04-14 11:29:01.000000 enconnect-0.2.3/enconnect/philipshue/bridge.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      955 2024-04-14 11:21:24.000000 enconnect-0.2.3/enconnect/philipshue/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:11.689740 enconnect-0.2.3/enconnect/philipshue/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:44.000000 enconnect-0.2.3/enconnect/philipshue/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1773 2024-04-15 09:01:50.000000 enconnect-0.2.3/enconnect/philipshue/test/test_bridge.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 22:21:56.000000 enconnect-0.2.3/enconnect/py.typed
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:11.689740 enconnect-0.2.3/enconnect/reddit/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      385 2024-04-13 11:18:53.000000 enconnect-0.2.3/enconnect/reddit/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      954 2024-04-25 02:11:28.000000 enconnect-0.2.3/enconnect/reddit/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4102 2024-04-25 02:26:38.000000 enconnect-0.2.3/enconnect/reddit/reddit.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:11.689740 enconnect-0.2.3/enconnect/reddit/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-13 07:05:56.000000 enconnect-0.2.3/enconnect/reddit/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1681 2024-04-15 09:01:50.000000 enconnect-0.2.3/enconnect/reddit/test/test_reddit.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:11.689740 enconnect-0.2.3/enconnect/ubiquiti/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:46.000000 enconnect-0.2.3/enconnect/ubiquiti/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1127 2024-04-14 11:21:29.000000 enconnect-0.2.3/enconnect/ubiquiti/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4320 2024-04-25 02:26:38.000000 enconnect-0.2.3/enconnect/ubiquiti/router.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:11.689740 enconnect-0.2.3/enconnect/ubiquiti/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:52.000000 enconnect-0.2.3/enconnect/ubiquiti/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2199 2024-04-15 09:01:50.000000 enconnect-0.2.3/enconnect/ubiquiti/test/test_router.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-25 02:28:10.000000 enconnect-0.2.3/enconnect/version.txt
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:11.689740 enconnect-0.2.3/enconnect/youtube/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      391 2024-04-12 07:52:09.000000 enconnect-0.2.3/enconnect/youtube/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      979 2024-04-12 06:47:27.000000 enconnect-0.2.3/enconnect/youtube/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:11.689740 enconnect-0.2.3/enconnect/youtube/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 07:23:02.000000 enconnect-0.2.3/enconnect/youtube/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1927 2024-04-15 09:01:50.000000 enconnect-0.2.3/enconnect/youtube/test/test_youtube.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4941 2024-04-25 02:26:38.000000 enconnect-0.2.3/enconnect/youtube/youtube.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-25 02:32:11.689740 enconnect-0.2.3/enconnect.egg-info/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2753 2024-04-25 02:32:11.000000 enconnect-0.2.3/enconnect.egg-info/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1126 2024-04-25 02:32:11.000000 enconnect-0.2.3/enconnect.egg-info/SOURCES.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-25 02:32:11.000000 enconnect-0.2.3/enconnect.egg-info/dependency_links.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       18 2024-04-25 02:32:11.000000 enconnect-0.2.3/enconnect.egg-info/requires.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       10 2024-04-25 02:32:11.000000 enconnect-0.2.3/enconnect.egg-info/top_level.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      529 2024-04-08 22:22:47.000000 enconnect-0.2.3/pyproject.toml
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       18 2024-04-08 22:20:24.000000 enconnect-0.2.3/reqs-install.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      305 2024-04-25 02:32:11.690740 enconnect-0.2.3/setup.cfg
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-04-08 22:20:24.000000 enconnect-0.3.0/LICENSE
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       33 2024-04-08 22:21:35.000000 enconnect-0.3.0/MANIFEST.in
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2774 2024-04-29 04:53:00.083427 enconnect-0.3.0/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2363 2024-04-14 13:59:58.000000 enconnect-0.3.0/README.md
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.082427 enconnect-0.3.0/enconnect/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-08 22:22:18.000000 enconnect-0.3.0/enconnect/__init__.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.082427 enconnect-0.3.0/enconnect/instagram/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      405 2024-04-13 00:00:49.000000 enconnect-0.3.0/enconnect/instagram/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6100 2024-04-29 04:47:32.000000 enconnect-0.3.0/enconnect/instagram/instagram.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      982 2024-04-12 05:18:12.000000 enconnect-0.3.0/enconnect/instagram/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.082427 enconnect-0.3.0/enconnect/instagram/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 04:42:12.000000 enconnect-0.3.0/enconnect/instagram/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3160 2024-04-29 04:47:32.000000 enconnect-0.3.0/enconnect/instagram/test/test_instagram.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.082427 enconnect-0.3.0/enconnect/philipshue/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:18.000000 enconnect-0.3.0/enconnect/philipshue/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2254 2024-04-14 11:29:01.000000 enconnect-0.3.0/enconnect/philipshue/bridge.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      955 2024-04-14 11:21:24.000000 enconnect-0.3.0/enconnect/philipshue/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.082427 enconnect-0.3.0/enconnect/philipshue/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:44.000000 enconnect-0.3.0/enconnect/philipshue/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1773 2024-04-15 09:01:50.000000 enconnect-0.3.0/enconnect/philipshue/test/test_bridge.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 22:21:56.000000 enconnect-0.3.0/enconnect/py.typed
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.082427 enconnect-0.3.0/enconnect/reddit/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      385 2024-04-13 11:18:53.000000 enconnect-0.3.0/enconnect/reddit/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      954 2024-04-25 02:11:28.000000 enconnect-0.3.0/enconnect/reddit/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7184 2024-04-29 04:47:32.000000 enconnect-0.3.0/enconnect/reddit/reddit.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect/reddit/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-13 07:05:56.000000 enconnect-0.3.0/enconnect/reddit/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3117 2024-04-29 04:47:32.000000 enconnect-0.3.0/enconnect/reddit/test/test_reddit.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect/ubiquiti/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      330 2024-04-14 11:22:46.000000 enconnect-0.3.0/enconnect/ubiquiti/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1127 2024-04-14 11:21:29.000000 enconnect-0.3.0/enconnect/ubiquiti/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4320 2024-04-25 02:26:38.000000 enconnect-0.3.0/enconnect/ubiquiti/router.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect/ubiquiti/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-14 11:30:52.000000 enconnect-0.3.0/enconnect/ubiquiti/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2199 2024-04-15 09:01:50.000000 enconnect-0.3.0/enconnect/ubiquiti/test/test_router.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect/utils/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      283 2024-04-29 00:13:14.000000 enconnect-0.3.0/enconnect/utils/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6507 2024-04-29 04:47:32.000000 enconnect-0.3.0/enconnect/utils/http.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect/utils/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-29 00:13:14.000000 enconnect-0.3.0/enconnect/utils/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2862 2024-04-29 00:13:14.000000 enconnect-0.3.0/enconnect/utils/test/test_http.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-29 04:48:48.000000 enconnect-0.3.0/enconnect/version.txt
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect/youtube/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      391 2024-04-12 07:52:09.000000 enconnect-0.3.0/enconnect/youtube/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      979 2024-04-12 06:47:27.000000 enconnect-0.3.0/enconnect/youtube/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect/youtube/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-12 07:23:02.000000 enconnect-0.3.0/enconnect/youtube/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3212 2024-04-29 04:47:32.000000 enconnect-0.3.0/enconnect/youtube/test/test_youtube.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7648 2024-04-29 04:47:32.000000 enconnect-0.3.0/enconnect/youtube/youtube.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-29 04:53:00.083427 enconnect-0.3.0/enconnect.egg-info/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2774 2024-04-29 04:53:00.000000 enconnect-0.3.0/enconnect.egg-info/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1245 2024-04-29 04:53:00.000000 enconnect-0.3.0/enconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-29 04:53:00.000000 enconnect-0.3.0/enconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       24 2024-04-29 04:53:00.000000 enconnect-0.3.0/enconnect.egg-info/requires.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       10 2024-04-29 04:53:00.000000 enconnect-0.3.0/enconnect.egg-info/top_level.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      529 2024-04-08 22:22:47.000000 enconnect-0.3.0/pyproject.toml
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       24 2024-04-29 00:13:14.000000 enconnect-0.3.0/reqs-install.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      305 2024-04-29 04:53:00.084427 enconnect-0.3.0/setup.cfg
```

### Comparing `enconnect-0.2.3/LICENSE` & `enconnect-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.3/PKG-INFO` & `enconnect-0.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: enconnect
-Version: 0.2.3
+Version: 0.3.0
 Summary: Enasis Network Remote Connect
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: encommon
+Requires-Dist: httpx
 Requires-Dist: requests
 
 # Enasis Network Remote Connect
 
 > :children_crossing: This project has not released its first major version.
 
 Functions and classes for connecting to remote services and whatnot.
```

### Comparing `enconnect-0.2.3/README.md` & `enconnect-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.3/enconnect/__init__.py` & `enconnect-0.3.0/enconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.3/enconnect/instagram/instagram.py` & `enconnect-0.3.0/enconnect/ubiquiti/router.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,178 +7,176 @@
 
 
 
 from typing import Any
 from typing import Optional
 from typing import TYPE_CHECKING
 
-from pydantic import BaseModel
-
 from requests import Response
-from requests import request
+from requests import Session
 
 if TYPE_CHECKING:
-    from .params import InstagramParams
-
-
-
-MEDIA_FIELDS = [
-    'caption',
-    'id',
-    'is_shared_to_feed',
-    'media_type',
-    'media_url',
-    'permalink',
-    'thumbnail_url',
-    'timestamp',
-    'username']
-
-MEDIA_RENAME = {
-    'is_shared_to_feed': 'shared',
-    'media_type': 'type',
-    'media_url': 'location',
-    'thumbnail_url': 'thumbnail'}
+    from .params import RouterParams
 
 
 
-class InstagramMedia(BaseModel, extra='allow'):
+class Router:
     """
-    Contains information returned from the upstream response.
-
-    .. note::
-       Fields are not completely documented for this model.
+    Interact with the cloud service API with various methods.
 
-    :param data: Keyword arguments passed to Pydantic model.
-        Parameter is picked up by autodoc, please ignore.
+    :param params: Parameters for instantiating the instance.
     """
 
-    caption: Optional[str] = None
-    id: str
-    shared: Optional[bool] = None
-    type: str
-    location: str
-    permalink: Optional[str] = None
-    thumbnail: Optional[str] = None
-    timestamp: str
-    username: str
+    __params: 'RouterParams'
+    __session: Session
 
 
     def __init__(
         self,
-        **data: Any,
+        params: 'RouterParams',
     ) -> None:
         """
         Initialize instance for class using provided parameters.
         """
 
-        items = MEDIA_RENAME.items()
-
-        for old, new in items:
-
-            if old not in data:
-                continue
+        self.__params = params
+        self.__session = Session()
 
-            data[new] = data[old]
 
-            del data[old]
+    @property
+    def params(
+        self,
+    ) -> 'RouterParams':
+        """
+        Return the Pydantic model containing the configuration.
 
-        super().__init__(**data)
+        :returns: Pydantic model containing the configuration.
+        """
 
+        return self.__params
 
 
-class Instagram:
-    """
-    Interact with the cloud service API with various methods.
+    @property
+    def session(
+        self,
+    ) -> Session:
+        """
+        Return the value for the attribute from class instance.
 
-    :param params: Parameters for instantiating the instance.
-    """
+        :returns: Value for the attribute from class instance.
+        """
 
-    __params: 'InstagramParams'
+        return self.__session
 
 
-    def __init__(
+    def request_cookie(
         self,
-        params: 'InstagramParams',
-    ) -> None:
+    ) -> Response:
         """
-        Initialize instance for class using provided parameters.
+        Establish new session obtaining cookie for authorization.
+
+        :returns: Response for upstream request to the server.
         """
 
-        self.__params = params
+        params = self.params
 
+        payload = {
+            'username': params.username,
+            'password': params.password}
 
-    @property
-    def params(
-        self,
-    ) -> 'InstagramParams':
-        """
-        Return the Pydantic model containing the configuration.
+        response = self.request(
+            method='post',
+            path='api/auth/login',
+            json=payload)
 
-        :returns: Pydantic model containing the configuration.
-        """
+        response.raise_for_status()
 
-        return self.__params
+        return response
 
 
     def request(
         self,
         method: str,
         path: str,
         params: Optional[dict[str, Any]] = None,
+        json: Optional[dict[str, Any]] = None,
     ) -> Response:
         """
         Return the response for upstream request to the server.
 
         :param method: Method for operation with the API server.
         :param path: Path for the location to upstream endpoint.
         :param params: Optional parameters included in request.
+        :param json: Optional JSON payload included in request.
         :returns: Response for upstream request to the server.
         """
 
         params = dict(params or {})
+        json = dict(json or {})
+
+        request = self.session.request
 
         server = self.params.server
         verify = self.params.ssl_verify
         capem = self.params.ssl_capem
 
-
-        params['access_token'] = (
-            self.params.token)
-
         location = (
             f'https://{server}/{path}')
 
-
         return request(
             method=method,
             url=location,
             timeout=self.params.timeout,
             params=params,
+            json=json,
             verify=capem or verify)
 
 
-    def get_media(
+    def request_proxy(
         self,
-    ) -> list[InstagramMedia]:
+        method: str,
+        path: str,
+        params: Optional[dict[str, Any]] = None,
+        json: Optional[dict[str, Any]] = None,
+    ) -> Response:
         """
-        Return the posts from the account associated with user.
+        Return the response for upstream request to the server.
+
+        .. note::
+           Most endpoints on Ubiquiti routers are prefixed with
+           not only the site but also `/proxy/network/api`. The
+           method will handle concatenating the values for you.
+           It will also handle authenticating if not already.
 
-        :returns: Posts from the account associated with user.
+        :param method: Method for operation with the API server.
+        :param path: Path for the location to upstream endpoint.
+        :param params: Optional parameters included in request.
+        :param json: Optional JSON payload included in request.
+        :returns: Response for upstream request to the server.
         """
 
-        fields = ','.join(MEDIA_FIELDS)
+        site = self.params.site
 
+        path = (
+            'proxy/network/api'
+            f'/s/{site}/{path}')
 
-        response = self.request(
-            'get', 'me/media',
-            {'fields': fields})
 
-        response.raise_for_status()
+        def _request() -> Response:
+
+            return self.request(
+                method, path,
+                params, json)
+
 
-        fetched = response.json()
+        response = _request()
 
-        assert isinstance(fetched, dict)
+        if response.status_code == 401:
+
+            self.request_cookie()
+
+            response = _request()
+
+        response.raise_for_status()
 
 
-        return [
-            InstagramMedia(**x)
-            for x in fetched['data']]
+        return response
```

### Comparing `enconnect-0.2.3/enconnect/instagram/params.py` & `enconnect-0.3.0/enconnect/instagram/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.3/enconnect/instagram/test/test_instagram.py` & `enconnect-0.3.0/enconnect/ubiquiti/test/test_router.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,86 +13,104 @@
 from encommon.utils import load_sample
 from encommon.utils import prep_sample
 from encommon.utils import read_text
 
 from requests_mock import Mocker
 
 from . import SAMPLES
-from ..instagram import Instagram
-from ..instagram import MEDIA_FIELDS
-from ..params import InstagramParams
+from ..params import RouterParams
+from ..router import Router
 
 
 
-def test_Instagram() -> None:
+def test_Router() -> None:
     """
     Perform various tests associated with relevant routines.
     """
 
-    params = InstagramParams(
-        token='mocked')
+    params = RouterParams(
+        server='192.168.1.1',
+        username='mocked',
+        password='mocked')
 
-    social = Instagram(params)
+    router = Router(params)
 
 
-    attrs = list(social.__dict__)
+    attrs = list(router.__dict__)
 
     assert attrs == [
-        '_Instagram__params']
+        '_Router__params',
+        '_Router__session']
 
 
     assert inrepr(
-        'instagram.Instagram object',
-        social)
+        'router.Router object',
+        router)
 
-    assert hash(social) > 0
+    assert hash(router) > 0
 
     assert instr(
-        'instagram.Instagram object',
-        social)
+        'router.Router object',
+        router)
 
 
-    assert social.params is params
+    assert router.params is params
 
+    assert router.session is not None
 
-    def _mocker_media() -> None:
+
+    def _mocker_cookie() -> None:
 
         server = params.server
-        token = params.token
 
-        fields = ','.join(MEDIA_FIELDS)
+        location = (
+            f'https://{server}'
+            '/api/auth/login')
+
+        mocker.post(location)
+
+
+    def _mocker_users() -> None:
+
+        server = params.server
 
         location = (
-            f'https://{server}/'
-            'me/media'
-            f'?fields={fields}'
-            f'&access_token={token}')
+            f'https://{server}'
+            '/proxy/network'
+            '/api/s/default/rest/user')
 
         source = read_text(
             f'{SAMPLES}/source.json')
 
-        mocker.get(
-            url=location,
-            text=source)
+        mocker.register_uri(
+            'get', location,
+            [{'text': source,
+              'status_code': 401},
+             {'text': source}])
 
 
     with Mocker() as mocker:
 
-        _mocker_media()
+        _mocker_cookie()
+        _mocker_users()
+
+        request = router.request_proxy
+
+        response = request(
+            'get', 'rest/user')
+
+
+    response.raise_for_status()
 
-        media = social.get_media()
+    fetched = response.json()
 
 
     sample_path = (
         f'{SAMPLES}/dumped.json')
 
     sample = load_sample(
-        sample_path,
-        [x.model_dump()
-         for x in media],
+        sample_path, fetched,
         update=ENPYRWS)
 
-    expect = prep_sample([
-        x.model_dump()
-        for x in media])
+    expect = prep_sample(fetched)
 
     assert sample == expect
```

### Comparing `enconnect-0.2.3/enconnect/philipshue/bridge.py` & `enconnect-0.3.0/enconnect/philipshue/bridge.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.3/enconnect/philipshue/params.py` & `enconnect-0.3.0/enconnect/philipshue/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.3/enconnect/philipshue/test/test_bridge.py` & `enconnect-0.3.0/enconnect/philipshue/test/test_bridge.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.3/enconnect/reddit/params.py` & `enconnect-0.3.0/enconnect/reddit/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.3/enconnect/ubiquiti/params.py` & `enconnect-0.3.0/enconnect/ubiquiti/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.3/enconnect/youtube/params.py` & `enconnect-0.3.0/enconnect/youtube/params.py`

 * *Files identical despite different names*

### Comparing `enconnect-0.2.3/enconnect.egg-info/PKG-INFO` & `enconnect-0.3.0/enconnect.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: enconnect
-Version: 0.2.3
+Version: 0.3.0
 Summary: Enasis Network Remote Connect
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: encommon
+Requires-Dist: httpx
 Requires-Dist: requests
 
 # Enasis Network Remote Connect
 
 > :children_crossing: This project has not released its first major version.
 
 Functions and classes for connecting to remote services and whatnot.
```

### Comparing `enconnect-0.2.3/enconnect.egg-info/SOURCES.txt` & `enconnect-0.3.0/enconnect.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -28,12 +28,16 @@
 enconnect/reddit/test/__init__.py
 enconnect/reddit/test/test_reddit.py
 enconnect/ubiquiti/__init__.py
 enconnect/ubiquiti/params.py
 enconnect/ubiquiti/router.py
 enconnect/ubiquiti/test/__init__.py
 enconnect/ubiquiti/test/test_router.py
+enconnect/utils/__init__.py
+enconnect/utils/http.py
+enconnect/utils/test/__init__.py
+enconnect/utils/test/test_http.py
 enconnect/youtube/__init__.py
 enconnect/youtube/params.py
 enconnect/youtube/youtube.py
 enconnect/youtube/test/__init__.py
 enconnect/youtube/test/test_youtube.py
```

### Comparing `enconnect-0.2.3/pyproject.toml` & `enconnect-0.3.0/pyproject.toml`

 * *Files identical despite different names*

