# Comparing `tmp/riassigner-0.4.0.tar.gz` & `tmp/riassigner-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "riassigner-0.4.0.tar", max compression
+gzip compressed data, was "riassigner-0.4.1.tar", max compression
```

## Comparing `riassigner-0.4.0.tar` & `riassigner-0.4.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1064 2024-02-13 10:37:40.170909 riassigner-0.4.0/LICENSE
--rw-r--r--   0        0        0     5611 2024-02-13 10:37:40.170909 riassigner-0.4.0/README.md
--rw-r--r--   0        0        0      159 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/__init__.py
--rw-r--r--   0        0        0     2150 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/__main__.py
--rw-r--r--   0        0        0       22 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/__version__.py
--rw-r--r--   0        0        0     1122 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/cli/CreateMethodAction.py
--rw-r--r--   0        0        0     1263 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/cli/LoadDataAction.py
--rw-r--r--   0        0        0      247 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/cli/__init__.py
--rw-r--r--   0        0        0     1471 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/compute/ComputationMethod.py
--rw-r--r--   0        0        0      845 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/compute/CubicSpline.py
--rw-r--r--   0        0        0     4048 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/compute/Kovats.py
--rw-r--r--   0        0        0      278 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/compute/__init__.py
--rw-r--r--   0        0        0     6873 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/data/Data.py
--rw-r--r--   0        0        0     5172 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/data/MatchMSData.py
--rw-r--r--   0        0        0     5747 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/data/PandasData.py
--rw-r--r--   0        0        0     1360 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/data/SimpleData.py
--rw-r--r--   0        0        0     1436 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/data/ValidateSimpleData.py
--rw-r--r--   0        0        0      382 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/data/__init__.py
--rw-r--r--   0        0        0     1783 2024-02-13 10:37:40.170909 riassigner-0.4.0/RIAssigner/utils.py
--rw-r--r--   0        0        0     1148 2024-02-13 10:37:40.170909 riassigner-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6748 1970-01-01 00:00:00.000000 riassigner-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-29 06:58:10.387846 riassigner-0.4.1/LICENSE
+-rw-r--r--   0        0        0     5611 2024-04-29 06:58:10.387846 riassigner-0.4.1/README.md
+-rw-r--r--   0        0        0      159 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/__init__.py
+-rw-r--r--   0        0        0     2150 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/__version__.py
+-rw-r--r--   0        0        0     1122 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/cli/CreateMethodAction.py
+-rw-r--r--   0        0        0     1263 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/cli/LoadDataAction.py
+-rw-r--r--   0        0        0      247 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/cli/__init__.py
+-rw-r--r--   0        0        0     1471 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/compute/ComputationMethod.py
+-rw-r--r--   0        0        0      845 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/compute/CubicSpline.py
+-rw-r--r--   0        0        0     4048 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/compute/Kovats.py
+-rw-r--r--   0        0        0      278 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/compute/__init__.py
+-rw-r--r--   0        0        0     6873 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/data/Data.py
+-rw-r--r--   0        0        0     5333 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/data/MatchMSData.py
+-rw-r--r--   0        0        0     5747 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/data/PandasData.py
+-rw-r--r--   0        0        0     1360 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/data/SimpleData.py
+-rw-r--r--   0        0        0     1436 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/data/ValidateSimpleData.py
+-rw-r--r--   0        0        0      382 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/data/__init__.py
+-rw-r--r--   0        0        0     1783 2024-04-29 06:58:10.387846 riassigner-0.4.1/RIAssigner/utils.py
+-rw-r--r--   0        0        0     1148 2024-04-29 06:58:10.387846 riassigner-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6748 1970-01-01 00:00:00.000000 riassigner-0.4.1/PKG-INFO
```

### Comparing `riassigner-0.4.0/LICENSE` & `riassigner-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `riassigner-0.4.0/README.md` & `riassigner-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `riassigner-0.4.0/RIAssigner/__main__.py` & `riassigner-0.4.1/RIAssigner/__main__.py`

 * *Files identical despite different names*

### Comparing `riassigner-0.4.0/RIAssigner/cli/CreateMethodAction.py` & `riassigner-0.4.1/RIAssigner/cli/CreateMethodAction.py`

 * *Files identical despite different names*

### Comparing `riassigner-0.4.0/RIAssigner/cli/LoadDataAction.py` & `riassigner-0.4.1/RIAssigner/cli/LoadDataAction.py`

 * *Files identical despite different names*

### Comparing `riassigner-0.4.0/RIAssigner/compute/ComputationMethod.py` & `riassigner-0.4.1/RIAssigner/compute/ComputationMethod.py`

 * *Files identical despite different names*

### Comparing `riassigner-0.4.0/RIAssigner/compute/CubicSpline.py` & `riassigner-0.4.1/RIAssigner/compute/CubicSpline.py`

 * *Files identical despite different names*

### Comparing `riassigner-0.4.0/RIAssigner/compute/Kovats.py` & `riassigner-0.4.1/RIAssigner/compute/Kovats.py`

 * *Files identical despite different names*

### Comparing `riassigner-0.4.0/RIAssigner/data/Data.py` & `riassigner-0.4.1/RIAssigner/data/Data.py`

 * *Files identical despite different names*

### Comparing `riassigner-0.4.0/RIAssigner/data/MatchMSData.py` & `riassigner-0.4.1/RIAssigner/data/MatchMSData.py`

 * *Files 3% similar despite different names*

```diff
@@ -143,7 +143,13 @@
     Args:
         spectrum (Spectrum): Spectrum to add RI to
         value (Data.RetentionIndexType): RI to be added to Spectrum
     """
     if value > 0:
         retention_index = ('%f' % float(value)).rstrip('0').rstrip('.')
         spectrum.set(key=key, value=retention_index)
+    else:
+        if spectrum.get(key):
+            metadata = spectrum.metadata
+            del metadata[key]
+            spectrum.metadata = metadata
+
```

### Comparing `riassigner-0.4.0/RIAssigner/data/PandasData.py` & `riassigner-0.4.1/RIAssigner/data/PandasData.py`

 * *Files identical despite different names*

### Comparing `riassigner-0.4.0/RIAssigner/data/SimpleData.py` & `riassigner-0.4.1/RIAssigner/data/SimpleData.py`

 * *Files identical despite different names*

### Comparing `riassigner-0.4.0/RIAssigner/data/ValidateSimpleData.py` & `riassigner-0.4.1/RIAssigner/data/ValidateSimpleData.py`

 * *Files identical despite different names*

### Comparing `riassigner-0.4.0/RIAssigner/utils.py` & `riassigner-0.4.1/RIAssigner/utils.py`

 * *Files identical despite different names*

### Comparing `riassigner-0.4.0/pyproject.toml` & `riassigner-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "RIAssigner"
-version = "0.4.0"
+version = "0.4.1"
 description = "Python library for retention index calculation."
 authors = ["Helge Hecht <helge.hecht@recetox.muni.cz>", "Maksym Skoryk <maksym.skoryk@recetox.muni.cz>"]
 
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/RECETOX/RIAssigner"
 keywords=[
```

### Comparing `riassigner-0.4.0/PKG-INFO` & `riassigner-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RIAssigner
-Version: 0.4.0
+Version: 0.4.1
 Summary: Python library for retention index calculation.
 Home-page: https://github.com/RECETOX/RIAssigner
 License: MIT
 Keywords: gas chromatography,mass spectrometry,retention index
 Author: Helge Hecht
 Author-email: helge.hecht@recetox.muni.cz
 Requires-Python: >=3.10,<3.13
```

