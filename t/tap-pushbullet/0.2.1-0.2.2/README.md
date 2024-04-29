# Comparing `tmp/tap_pushbullet-0.2.1.tar.gz` & `tmp/tap_pushbullet-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_pushbullet-0.2.1.tar", max compression
+gzip compressed data, was "tap_pushbullet-0.2.2.tar", max compression
```

## Comparing `tap_pushbullet-0.2.1.tar` & `tap_pushbullet-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2303 2024-04-03 06:29:13.514945 tap_pushbullet-0.2.1/README.md
--rw-r--r--   0        0        0     2660 2024-04-03 06:29:17.498952 tap_pushbullet-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       85 2024-04-03 06:29:13.514945 tap_pushbullet-0.2.1/tap_pushbullet/__init__.py
--rw-r--r--   0        0        0      125 2024-04-03 06:29:13.514945 tap_pushbullet-0.2.1/tap_pushbullet/__main__.py
--rw-r--r--   0        0        0     3995 2024-04-03 06:29:13.514945 tap_pushbullet-0.2.1/tap_pushbullet/client.py
--rw-r--r--   0        0        0    15889 2024-04-03 06:29:13.518945 tap_pushbullet-0.2.1/tap_pushbullet/streams.py
--rw-r--r--   0        0        0     1086 2024-04-03 06:29:13.518945 tap_pushbullet-0.2.1/tap_pushbullet/tap.py
--rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 tap_pushbullet-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2303 2024-04-29 21:46:17.703711 tap_pushbullet-0.2.2/README.md
+-rw-r--r--   0        0        0     2660 2024-04-29 21:46:23.207747 tap_pushbullet-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       85 2024-04-29 21:46:17.703711 tap_pushbullet-0.2.2/tap_pushbullet/__init__.py
+-rw-r--r--   0        0        0      125 2024-04-29 21:46:17.703711 tap_pushbullet-0.2.2/tap_pushbullet/__main__.py
+-rw-r--r--   0        0        0     3995 2024-04-29 21:46:17.703711 tap_pushbullet-0.2.2/tap_pushbullet/client.py
+-rw-r--r--   0        0        0    15889 2024-04-29 21:46:17.703711 tap_pushbullet-0.2.2/tap_pushbullet/streams.py
+-rw-r--r--   0        0        0     1086 2024-04-29 21:46:17.703711 tap_pushbullet-0.2.2/tap_pushbullet/tap.py
+-rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 tap_pushbullet-0.2.2/PKG-INFO
```

### Comparing `tap_pushbullet-0.2.1/README.md` & `tap_pushbullet-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `tap_pushbullet-0.2.1/pyproject.toml` & `tap_pushbullet-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-pushbullet"
-version = "0.2.1"
+version = "0.2.2"
 description = "`tap-pushbullet` is a Singer tap for Pushbullet, built with the Meltano SDK for Singer Taps."
 authors = ["Edgar Ramírez-Mondragón <edgarrm358@gmail.com>"]
 keywords = [
   "ELT",
   "singer.io",
   "Pushbullet",
 ]
@@ -13,15 +13,15 @@
 homepage = "https://github.com/edgarrmondragon/tap-pushbullet"
 repository = "https://github.com/edgarrmondragon/tap-pushbullet"
 documentation = "https://github.com/edgarrmondragon/tap-pushbullet#readme"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 requests-cache = ">=1.1.0,<2"
-singer-sdk = "~=0.36.0"
+singer-sdk = "~=0.37.0"
 
 [tool.poetry.dev-dependencies]
 singer-sdk = { version = "*", extras = ["testing"] }
 
 [tool.pytest.ini_options]
 addopts = "-vvv"
 filterwarnings = [
```

### Comparing `tap_pushbullet-0.2.1/tap_pushbullet/client.py` & `tap_pushbullet-0.2.2/tap_pushbullet/client.py`

 * *Files identical despite different names*

### Comparing `tap_pushbullet-0.2.1/tap_pushbullet/streams.py` & `tap_pushbullet-0.2.2/tap_pushbullet/streams.py`

 * *Files identical despite different names*

### Comparing `tap_pushbullet-0.2.1/tap_pushbullet/tap.py` & `tap_pushbullet-0.2.2/tap_pushbullet/tap.py`

 * *Files identical despite different names*

### Comparing `tap_pushbullet-0.2.1/PKG-INFO` & `tap_pushbullet-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-pushbullet
-Version: 0.2.1
+Version: 0.2.2
 Summary: `tap-pushbullet` is a Singer tap for Pushbullet, built with the Meltano SDK for Singer Taps.
 Home-page: https://github.com/edgarrmondragon/tap-pushbullet
 License: Apache-2.0
 Keywords: ELT,singer.io,Pushbullet
 Author: Edgar Ramírez-Mondragón
 Author-email: edgarrm358@gmail.com
 Requires-Python: >=3.8
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests-cache (>=1.1.0,<2)
-Requires-Dist: singer-sdk (>=0.36.0,<0.37.0)
+Requires-Dist: singer-sdk (>=0.37.0,<0.38.0)
 Project-URL: Documentation, https://github.com/edgarrmondragon/tap-pushbullet#readme
 Project-URL: Repository, https://github.com/edgarrmondragon/tap-pushbullet
 Description-Content-Type: text/markdown
 
 # `tap-pushbullet`
 
 Singer tap for Pushbullet.
```

