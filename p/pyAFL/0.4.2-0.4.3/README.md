# Comparing `tmp/pyAFL-0.4.2.tar.gz` & `tmp/pyafl-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyAFL-0.4.2.tar", last modified: Tue Jan 16 18:24:21 2024, max compression
+gzip compressed data, was "pyafl-0.4.3.tar", last modified: Mon Apr 29 19:18:51 2024, max compression
```

## Comparing `pyAFL-0.4.2.tar` & `pyafl-0.4.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:21.018217 pyAFL-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-16 18:24:04.000000 pyAFL-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-16 18:24:04.000000 pyAFL-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-01-16 18:24:21.018217 pyAFL-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10342 2024-01-16 18:24:04.000000 pyAFL-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:21.014217 pyAFL-0.4.2/pyAFL/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:21.014217 pyAFL-0.4.2/pyAFL/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/base/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:21.014217 pyAFL-0.4.2/pyAFL/players/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/players/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/players/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:21.018217 pyAFL-0.4.2/pyAFL/players/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/players/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/players/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:21.018217 pyAFL-0.4.2/pyAFL/seasons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/seasons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10030 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/seasons/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:21.018217 pyAFL-0.4.2/pyAFL/seasons/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/seasons/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/seasons/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:21.018217 pyAFL-0.4.2/pyAFL/session/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:21.018217 pyAFL-0.4.2/pyAFL/session/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/session/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/session/tests/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:21.018217 pyAFL-0.4.2/pyAFL/teams/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/teams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/teams/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:21.018217 pyAFL-0.4.2/pyAFL/teams/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/teams/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-01-16 18:24:04.000000 pyAFL-0.4.2/pyAFL/teams/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 18:24:21.018217 pyAFL-0.4.2/pyAFL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-01-16 18:24:21.000000 pyAFL-0.4.2/pyAFL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-01-16 18:24:21.000000 pyAFL-0.4.2/pyAFL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 18:24:21.000000 pyAFL-0.4.2/pyAFL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-16 18:24:21.000000 pyAFL-0.4.2/pyAFL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-16 18:24:21.000000 pyAFL-0.4.2/pyAFL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-16 18:24:04.000000 pyAFL-0.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-16 18:24:21.018217 pyAFL-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-01-16 18:24:04.000000 pyAFL-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:51.161319 pyafl-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-29 19:18:42.000000 pyafl-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 19:18:42.000000 pyafl-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-29 19:18:51.161319 pyafl-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-29 19:18:42.000000 pyafl-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:51.157319 pyafl-0.4.3/pyAFL/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:51.157319 pyafl-0.4.3/pyAFL/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/base/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:51.157319 pyafl-0.4.3/pyAFL/players/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/players/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/players/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:51.157319 pyafl-0.4.3/pyAFL/players/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/players/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/players/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:51.157319 pyafl-0.4.3/pyAFL/seasons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/seasons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10030 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/seasons/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:51.157319 pyafl-0.4.3/pyAFL/seasons/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/seasons/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/seasons/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:51.157319 pyafl-0.4.3/pyAFL/session/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:51.157319 pyafl-0.4.3/pyAFL/session/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/session/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/session/tests/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:51.161319 pyafl-0.4.3/pyAFL/teams/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/teams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/teams/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:51.161319 pyafl-0.4.3/pyAFL/teams/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/teams/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-29 19:18:42.000000 pyafl-0.4.3/pyAFL/teams/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:18:51.161319 pyafl-0.4.3/pyAFL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-29 19:18:51.000000 pyafl-0.4.3/pyAFL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-29 19:18:51.000000 pyafl-0.4.3/pyAFL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:18:51.000000 pyafl-0.4.3/pyAFL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-29 19:18:51.000000 pyafl-0.4.3/pyAFL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-29 19:18:51.000000 pyafl-0.4.3/pyAFL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-29 19:18:42.000000 pyafl-0.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-29 19:18:51.161319 pyafl-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-29 19:18:42.000000 pyafl-0.4.3/setup.py
```

### Comparing `pyAFL-0.4.2/LICENSE` & `pyafl-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyAFL-0.4.2/PKG-INFO` & `pyafl-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAFL
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python data fetching library for the Australian Football League
 Home-page: https://github.com/RamParameswaran/pyAFL
 Author: Ram Parameswaran
 Author-email: ram@findram.dev
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyAFL-0.4.2/README.md` & `pyafl-0.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 ### Player()
 
 Instantiates the Player object. The **init** method finds the matching player on afltables.com based on the `name` argument string. `name` must be an exact match, in the format "Firstname Lastname" and must be a name listed at https://afltables.com/afl/stats/playersA_idx.html
 
 ### Player.get_player_stats()
 
-Pulls player stats (career totals, and season-by-season summary) and presents as a Python object.
+Pulls player bio (height, weight, dob, debut, and last) to store in Player attribute 'metadata', and player stats (career totals, and season-by-season summary) which is presented as a Python object.
 This function returns a PlayerStats object with attributes:
 
 - season_stats_total (Pandas dataframe)
 - season_stats_average (Pandas dataframe)
 - season_results (list of Pandas dataframes)
 
 **Example**
```

### Comparing `pyAFL-0.4.2/pyAFL/seasons/models.py` & `pyafl-0.4.3/pyAFL/seasons/models.py`

 * *Files identical despite different names*

### Comparing `pyAFL-0.4.2/pyAFL/seasons/tests/test_models.py` & `pyafl-0.4.3/pyAFL/seasons/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `pyAFL-0.4.2/pyAFL/session/session.py` & `pyafl-0.4.3/pyAFL/session/session.py`

 * *Files identical despite different names*

### Comparing `pyAFL-0.4.2/pyAFL/session/tests/test_session.py` & `pyafl-0.4.3/pyAFL/session/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `pyAFL-0.4.2/pyAFL/teams/__init__.py` & `pyafl-0.4.3/pyAFL/teams/__init__.py`

 * *Files identical despite different names*

### Comparing `pyAFL-0.4.2/pyAFL/teams/models.py` & `pyafl-0.4.3/pyAFL/teams/models.py`

 * *Files identical despite different names*

### Comparing `pyAFL-0.4.2/pyAFL/teams/tests/test_models.py` & `pyafl-0.4.3/pyAFL/teams/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `pyAFL-0.4.2/pyAFL.egg-info/PKG-INFO` & `pyafl-0.4.3/pyAFL.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAFL
-Version: 0.4.2
+Version: 0.4.3
 Summary: Python data fetching library for the Australian Football League
 Home-page: https://github.com/RamParameswaran/pyAFL
 Author: Ram Parameswaran
 Author-email: ram@findram.dev
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyAFL-0.4.2/pyAFL.egg-info/SOURCES.txt` & `pyafl-0.4.3/pyAFL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyAFL-0.4.2/setup.py` & `pyafl-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setuptools.setup(
     name="pyAFL",
-    version="0.4.2",
+    version="0.4.3",
     description="Python data fetching library for the Australian Football League",
     long_description="pyAFL is a AFL (Australian Football League) data fetching libary. It scrapes data from https://afltables.com/ and converts results to structured Python objects for easier analytics.",
     url="https://github.com/RamParameswaran/pyAFL",
     author="Ram Parameswaran",
     author_email="ram@findram.dev",
     license="MIT",
     packages=setuptools.find_packages(
```

