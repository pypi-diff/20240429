# Comparing `tmp/labequipment-0.0.1.tar.gz` & `tmp/labequipment-0.0.2.tar.gz`

## Comparing `labequipment-0.0.1.tar` & `labequipment-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    63488 2020-02-02 00:00:00.000000 labequipment-0.0.1/UsbDllWrap.dll
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/__init__.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/in_progress/AQ3675_Test.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/in_progress/DS1104_Test.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/in_progress/E5052A_Test.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/in_progress/N9010A_Test.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/in_progress/R3465_Test.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/in_progress/SG384_Test.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/in_progress/TDS7404_Test.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/instruments/awg/signal_generator/SG384.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/instruments/esa/E4440A.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/instruments/esa/R3465.py
--rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/instruments/lasers/TLB6700.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/instruments/osa/AQ3675.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/instruments/oscilloscopes/DS1104.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/instruments/oscilloscopes/HP54810A.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/instruments/oscilloscopes/TDS7404.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/instruments/ssa/E5052A.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 labequipment-0.0.1/src/labequipment/instruments/ssa/N9010A.py
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 labequipment-0.0.1/LICENSE
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 labequipment-0.0.1/README.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 labequipment-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 labequipment-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    63488 2020-02-02 00:00:00.000000 labequipment-0.0.2/UsbDllWrap.dll
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/__init__.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/in_progress/AQ3675_Test.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/in_progress/DS1104_Test.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/in_progress/E5052A_Test.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/in_progress/N9010A_Test.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/in_progress/R3465_Test.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/in_progress/SG384_Test.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/in_progress/TDS7404_Test.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/instruments/awg/signal_generator/SG384.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/instruments/esa/E4440A.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/instruments/esa/R3465.py
+-rw-r--r--   0        0        0     7359 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/instruments/lasers/TLB6700.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/instruments/osa/AQ3675.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/instruments/oscilloscopes/DS1104.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/instruments/oscilloscopes/HP54810A.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/instruments/oscilloscopes/TDS7404.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/instruments/ssa/E5052A.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 labequipment-0.0.2/src/labequipment/instruments/ssa/N9010A.py
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 labequipment-0.0.2/LICENSE
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 labequipment-0.0.2/README.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 labequipment-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 labequipment-0.0.2/PKG-INFO
```

### Comparing `labequipment-0.0.1/UsbDllWrap.dll` & `labequipment-0.0.2/UsbDllWrap.dll`

 * *Files identical despite different names*

### Comparing `labequipment-0.0.1/src/labequipment/in_progress/DS1104_Test.py` & `labequipment-0.0.2/src/labequipment/in_progress/DS1104_Test.py`

 * *Files identical despite different names*

### Comparing `labequipment-0.0.1/src/labequipment/in_progress/E5052A_Test.py` & `labequipment-0.0.2/src/labequipment/in_progress/E5052A_Test.py`

 * *Files identical despite different names*

### Comparing `labequipment-0.0.1/src/labequipment/instruments/awg/signal_generator/SG384.py` & `labequipment-0.0.2/src/labequipment/instruments/awg/signal_generator/SG384.py`

 * *Files identical despite different names*

### Comparing `labequipment-0.0.1/src/labequipment/instruments/esa/E4440A.py` & `labequipment-0.0.2/src/labequipment/instruments/esa/E4440A.py`

 * *Files identical despite different names*

### Comparing `labequipment-0.0.1/src/labequipment/instruments/esa/R3465.py` & `labequipment-0.0.2/src/labequipment/instruments/esa/R3465.py`

 * *Files identical despite different names*

### Comparing `labequipment-0.0.1/src/labequipment/instruments/lasers/TLB6700.py` & `labequipment-0.0.2/src/labequipment/instruments/lasers/TLB6700.py`

 * *Files identical despite different names*

### Comparing `labequipment-0.0.1/src/labequipment/instruments/osa/AQ3675.py` & `labequipment-0.0.2/src/labequipment/instruments/osa/AQ3675.py`

 * *Files identical despite different names*

### Comparing `labequipment-0.0.1/src/labequipment/instruments/oscilloscopes/DS1104.py` & `labequipment-0.0.2/src/labequipment/instruments/oscilloscopes/DS1104.py`

 * *Files identical despite different names*

### Comparing `labequipment-0.0.1/src/labequipment/instruments/oscilloscopes/HP54810A.py` & `labequipment-0.0.2/src/labequipment/instruments/oscilloscopes/HP54810A.py`

 * *Files identical despite different names*

### Comparing `labequipment-0.0.1/src/labequipment/instruments/oscilloscopes/TDS7404.py` & `labequipment-0.0.2/src/labequipment/instruments/oscilloscopes/TDS7404.py`

 * *Files identical despite different names*

### Comparing `labequipment-0.0.1/src/labequipment/instruments/ssa/E5052A.py` & `labequipment-0.0.2/src/labequipment/instruments/ssa/E5052A.py`

 * *Files identical despite different names*

### Comparing `labequipment-0.0.1/src/labequipment/instruments/ssa/N9010A.py` & `labequipment-0.0.2/src/labequipment/instruments/ssa/N9010A.py`

 * *Files identical despite different names*

### Comparing `labequipment-0.0.1/LICENSE` & `labequipment-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `labequipment-0.0.1/pyproject.toml` & `labequipment-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "labequipment"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Tristan Melton", email="tristanmelton@proton.me" },
 ]
 description = "A library for control of common lab equipment."
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `labequipment-0.0.1/PKG-INFO` & `labequipment-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: labequipment
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for control of common lab equipment.
 Project-URL: Homepage, https://github.com/tristanmelton/LabDriver
 Project-URL: Issues, https://github.com/tristanmelton/LabDriver/issues
 Author-email: Tristan Melton <tristanmelton@proton.me>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 Requires-Dist: easy-scpi>=0.1.4
 Requires-Dist: numpy>=1.26.0
 Requires-Dist: pandas>=2.2.0
 Requires-Dist: pythonnet>=3.0.3
 Requires-Dist: pyvisa>=1.14.0
 Description-Content-Type: text/markdown
 
-# LabDriver
+# LabEquipment
 Library of classes for interfacing with common lab equipment in Python.
 
 # Required Libraries
 - NumPY
 - Pandas
 - pyVISA
 - EasySCPI
```

