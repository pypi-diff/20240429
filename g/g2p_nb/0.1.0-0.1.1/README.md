# Comparing `tmp/g2p_nb-0.1.0.tar.gz` & `tmp/g2p_nb-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g2p_nb-0.1.0.tar", max compression
+gzip compressed data, was "g2p_nb-0.1.1.tar", max compression
```

## Comparing `g2p_nb-0.1.0.tar` & `g2p_nb-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     7048 2024-02-09 17:35:42.220900 g2p_nb-0.1.0/LICENSE
--rw-r--r--   0        0        0     9384 2024-02-09 17:35:42.220900 g2p_nb-0.1.0/README.md
--rwxr-xr-x   0        0        0     3275 2024-04-26 15:10:29.441503 g2p_nb-0.1.0/g2p_nb/evaluate.py
--rw-r--r--   0        0        0     2453 2024-04-26 15:15:24.593455 g2p_nb-0.1.0/g2p_nb/predict.py
--rw-r--r--   0        0        0     1417 2024-02-09 17:35:42.220900 g2p_nb-0.1.0/g2p_nb/stats.py
--rw-r--r--   0        0        0      479 2024-04-26 13:08:08.981353 g2p_nb-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10115 1970-01-01 00:00:00.000000 g2p_nb-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7048 2024-02-09 17:35:42.220900 g2p_nb-0.1.1/LICENSE
+-rw-r--r--   0        0        0     9384 2024-02-09 17:35:42.220900 g2p_nb-0.1.1/README.md
+-rw-r--r--   0        0        0      113 2024-04-29 07:55:08.582252 g2p_nb-0.1.1/g2p_nb/__init__.py
+-rwxr-xr-x   0        0        0     3275 2024-04-26 15:10:29.441503 g2p_nb-0.1.1/g2p_nb/evaluate.py
+-rw-r--r--   0        0        0     2453 2024-04-26 15:15:24.593455 g2p_nb-0.1.1/g2p_nb/predict.py
+-rw-r--r--   0        0        0     1417 2024-02-09 17:35:42.220900 g2p_nb-0.1.1/g2p_nb/stats.py
+-rw-r--r--   0        0        0      479 2024-04-29 07:56:14.575326 g2p_nb-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10115 1970-01-01 00:00:00.000000 g2p_nb-0.1.1/PKG-INFO
```

### Comparing `g2p_nb-0.1.0/LICENSE` & `g2p_nb-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `g2p_nb-0.1.0/README.md` & `g2p_nb-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `g2p_nb-0.1.0/g2p_nb/evaluate.py` & `g2p_nb-0.1.1/g2p_nb/evaluate.py`

 * *Files identical despite different names*

### Comparing `g2p_nb-0.1.0/g2p_nb/predict.py` & `g2p_nb-0.1.1/g2p_nb/predict.py`

 * *Files identical despite different names*

### Comparing `g2p_nb-0.1.0/g2p_nb/stats.py` & `g2p_nb-0.1.1/g2p_nb/stats.py`

 * *Files identical despite different names*

### Comparing `g2p_nb-0.1.0/PKG-INFO` & `g2p_nb-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g2p_nb
-Version: 0.1.0
+Version: 0.1.1
 Summary: Grapheme-to-phoneme models for Norwegian bokmål to dialectal phonemic transcriptions
 License: CC0 1.0 Deed
 Author: Ingerid Dale
 Author-email: ingerid.dale@nb.no
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

