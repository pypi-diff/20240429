# Comparing `tmp/dataaetherscan-0.0.1.tar.gz` & `tmp/dataaetherscan-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataaetherscan-0.0.1.tar", last modified: Tue Apr 23 13:42:17 2024, max compression
+gzip compressed data, was "dataaetherscan-1.0.0.tar", last modified: Mon Apr 29 09:01:21 2024, max compression
```

## Comparing `dataaetherscan-0.0.1.tar` & `dataaetherscan-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 onur      (1000) onur      (1000)        0 2024-04-23 13:42:17.319093 dataaetherscan-0.0.1/
--rwxrwxrwx   0 onur      (1000) onur      (1000)    35821 2024-04-23 13:32:52.000000 dataaetherscan-0.0.1/LICENSE
--rwxrwxrwx   0 onur      (1000) onur      (1000)      723 2024-04-23 13:42:17.292372 dataaetherscan-0.0.1/PKG-INFO
--rwxrwxrwx   0 onur      (1000) onur      (1000)      174 2024-04-23 13:31:55.000000 dataaetherscan-0.0.1/README.md
--rwxrwxrwx   0 onur      (1000) onur      (1000)      659 2024-04-23 13:31:14.000000 dataaetherscan-0.0.1/pyproject.toml
--rwxrwxrwx   0 onur      (1000) onur      (1000)       38 2024-04-23 13:42:17.321159 dataaetherscan-0.0.1/setup.cfg
-drwxrwxrwx   0 onur      (1000) onur      (1000)        0 2024-04-23 13:42:16.723492 dataaetherscan-0.0.1/src/
-drwxrwxrwx   0 onur      (1000) onur      (1000)        0 2024-04-23 13:42:16.932689 dataaetherscan-0.0.1/src/dataaetherscan/
--rwxrwxrwx   0 onur      (1000) onur      (1000)       45 2024-04-23 13:41:58.000000 dataaetherscan-0.0.1/src/dataaetherscan/__init__.py
--rwxrwxrwx   0 onur      (1000) onur      (1000)     3141 2024-04-23 13:41:55.000000 dataaetherscan-0.0.1/src/dataaetherscan/das.py
-drwxrwxrwx   0 onur      (1000) onur      (1000)        0 2024-04-23 13:42:17.265366 dataaetherscan-0.0.1/src/dataaetherscan.egg-info/
--rwxrwxrwx   0 onur      (1000) onur      (1000)      723 2024-04-23 13:42:16.000000 dataaetherscan-0.0.1/src/dataaetherscan.egg-info/PKG-INFO
--rwxrwxrwx   0 onur      (1000) onur      (1000)      257 2024-04-23 13:42:16.000000 dataaetherscan-0.0.1/src/dataaetherscan.egg-info/SOURCES.txt
--rwxrwxrwx   0 onur      (1000) onur      (1000)        1 2024-04-23 13:42:16.000000 dataaetherscan-0.0.1/src/dataaetherscan.egg-info/dependency_links.txt
--rwxrwxrwx   0 onur      (1000) onur      (1000)       15 2024-04-23 13:42:16.000000 dataaetherscan-0.0.1/src/dataaetherscan.egg-info/top_level.txt
+drwxrwxrwx   0 onur      (1000) onur      (1000)        0 2024-04-29 09:01:21.326419 dataaetherscan-1.0.0/
+-rwxrwxrwx   0 onur      (1000) onur      (1000)    35821 2024-04-23 13:32:52.000000 dataaetherscan-1.0.0/LICENSE
+-rwxrwxrwx   0 onur      (1000) onur      (1000)     5104 2024-04-29 09:01:21.299711 dataaetherscan-1.0.0/PKG-INFO
+-rwxrwxrwx   0 onur      (1000) onur      (1000)     4731 2024-04-29 08:53:58.000000 dataaetherscan-1.0.0/README.md
+-rwxrwxrwx   0 onur      (1000) onur      (1000)      659 2024-04-23 13:43:55.000000 dataaetherscan-1.0.0/pyproject.toml
+-rwxrwxrwx   0 onur      (1000) onur      (1000)       38 2024-04-29 09:01:21.329958 dataaetherscan-1.0.0/setup.cfg
+drwxrwxrwx   0 onur      (1000) onur      (1000)        0 2024-04-29 09:01:20.589831 dataaetherscan-1.0.0/src/
+drwxrwxrwx   0 onur      (1000) onur      (1000)        0 2024-04-29 09:01:20.831929 dataaetherscan-1.0.0/src/dataaetherscan/
+-rwxrwxrwx   0 onur      (1000) onur      (1000)       45 2024-04-23 13:43:38.000000 dataaetherscan-1.0.0/src/dataaetherscan/__init__.py
+-rwxrwxrwx   0 onur      (1000) onur      (1000)     3141 2024-04-23 13:43:41.000000 dataaetherscan-1.0.0/src/dataaetherscan/das.py
+drwxrwxrwx   0 onur      (1000) onur      (1000)        0 2024-04-29 09:01:21.259315 dataaetherscan-1.0.0/src/dataaetherscan.egg-info/
+-rwxrwxrwx   0 onur      (1000) onur      (1000)     5104 2024-04-29 09:01:20.000000 dataaetherscan-1.0.0/src/dataaetherscan.egg-info/PKG-INFO
+-rwxrwxrwx   0 onur      (1000) onur      (1000)      257 2024-04-29 09:01:20.000000 dataaetherscan-1.0.0/src/dataaetherscan.egg-info/SOURCES.txt
+-rwxrwxrwx   0 onur      (1000) onur      (1000)        1 2024-04-29 09:01:20.000000 dataaetherscan-1.0.0/src/dataaetherscan.egg-info/dependency_links.txt
+-rwxrwxrwx   0 onur      (1000) onur      (1000)       15 2024-04-29 09:01:20.000000 dataaetherscan-1.0.0/src/dataaetherscan.egg-info/top_level.txt
```

### Comparing `dataaetherscan-0.0.1/LICENSE` & `dataaetherscan-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataaetherscan-0.0.1/pyproject.toml` & `dataaetherscan-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "requests>=2.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dataaetherscan"
-version = "0.0.1"
+version = "1.0.0"
 authors = [
   { name="DataAetherScan", email="it@dataaetherscan.com" },
 ]
 description = "Python integration to DataAetherScan"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `dataaetherscan-0.0.1/src/dataaetherscan/das.py` & `dataaetherscan-1.0.0/src/dataaetherscan/das.py`

 * *Files identical despite different names*

