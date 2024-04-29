# Comparing `tmp/lasertram-0.1.0.tar.gz` & `tmp/lasertram-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lasertram-0.1.0.tar", last modified: Thu Apr 25 17:37:28 2024, max compression
+gzip compressed data, was "lasertram-0.1.1.tar", last modified: Mon Apr 29 19:30:33 2024, max compression
```

## Comparing `lasertram-0.1.0.tar` & `lasertram-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:28.801510 lasertram-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-25 17:37:25.000000 lasertram-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-25 17:37:28.801510 lasertram-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-25 17:37:25.000000 lasertram-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:28.797510 lasertram-0.1.0/lasertram/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:28.801510 lasertram-0.1.0/lasertram/calc/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/calc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31659 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/calc/calc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:28.801510 lasertram-0.1.0/lasertram/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/helpers/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/helpers/conversions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:28.801510 lasertram-0.1.0/lasertram/tram/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/tram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-04-25 17:37:25.000000 lasertram-0.1.0/lasertram/tram/tram.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:28.801510 lasertram-0.1.0/lasertram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-25 17:37:28.000000 lasertram-0.1.0/lasertram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-25 17:37:28.000000 lasertram-0.1.0/lasertram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 17:37:28.000000 lasertram-0.1.0/lasertram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-25 17:37:28.000000 lasertram-0.1.0/lasertram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-25 17:37:28.000000 lasertram-0.1.0/lasertram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-25 17:37:25.000000 lasertram-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-25 17:37:28.801510 lasertram-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 17:37:28.801510 lasertram-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    37874 2024-04-25 17:37:25.000000 lasertram-0.1.0/tests/test_lasertram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:33.096996 lasertram-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-29 19:30:29.000000 lasertram-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-29 19:30:33.096996 lasertram-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-29 19:30:29.000000 lasertram-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:33.096996 lasertram-0.1.1/lasertram/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:33.096996 lasertram-0.1.1/lasertram/calc/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/calc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31599 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/calc/calc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:33.096996 lasertram-0.1.1/lasertram/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/helpers/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/helpers/conversions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:33.096996 lasertram-0.1.1/lasertram/tram/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/tram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11286 2024-04-29 19:30:29.000000 lasertram-0.1.1/lasertram/tram/tram.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:33.096996 lasertram-0.1.1/lasertram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-29 19:30:33.000000 lasertram-0.1.1/lasertram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-29 19:30:33.000000 lasertram-0.1.1/lasertram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:30:33.000000 lasertram-0.1.1/lasertram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-29 19:30:33.000000 lasertram-0.1.1/lasertram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 19:30:33.000000 lasertram-0.1.1/lasertram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 19:30:29.000000 lasertram-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-29 19:30:33.100996 lasertram-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:30:33.096996 lasertram-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    37829 2024-04-29 19:30:29.000000 lasertram-0.1.1/tests/test_lasertram.py
```

### Comparing `lasertram-0.1.0/LICENSE` & `lasertram-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lasertram-0.1.0/PKG-INFO` & `lasertram-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 Metadata-Version: 2.1
 Name: lasertram
-Version: 0.1.0
+Version: 0.1.1
 Summary: For processing LA-ICP-MS data
 Home-page: https://github.com/jlubbersgeo/lasertram
 Author: Jordan Lubbers
 Author-email: jelubber@gmail.com
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
+Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mendeleev>=0.14.0
 Requires-Dist: numpy>=1.25.2
 Requires-Dist: pandas>=2.0.3
 Requires-Dist: scipy>=1.11.1
 Requires-Dist: statsmodels>=0.14.0
 Requires-Dist: openpyxl>=3.0.0
 
 # lasertram
-[![PyPI version](https://badge.fury.io/py/lasertram.svg)](https://badge.fury.io/py/lasertram)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) !['coverage'](/images/COVERAGE.svg)
+
 
 Welcome to the repository for `lasertram`, a package for the time resolved analysis for processing laser ablation inductively coupled plasma mass spectrometry (LA-ICP-MS) data. It is utilized heavily in the dashboard [LaserTRAM-DB](https://github.com/jlubbersgeo/laserTRAM-DB).
 
 ## Documentation
 
 please see the [Documentation](https://jlubbersgeo.github.io/lasertram/) for more!
 
 ## Installation
-
+[![PyPI](https://img.shields.io/pypi/v/lasertram.svg?style=flat)](https://pypi.python.org/pypi/lasertram)
+[![Compatible Python Versions](https://img.shields.io/pypi/pyversions/lasertram.svg?style=flat)](https://pypi.org/project/lasertram/)
 ```
 pip install lasertram
 ```
 
 ## Contributing
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Code Quality](https://api.codacy.com/project/badge/Grade/fd9912a3faae43bf84a47e3da685d84c)](https://app.codacy.com/gh/jlubbersgeo/lasertram/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=jlubbersgeo/lasertram&amp;utm_campaign=Badge_Grade)
 
 If you have features you'd like to see please open an issue or consider contributing yourself! I'm always happy to have help.
 
--- Jordan
+**Maintainer** Jordan Lubbers (jlubbers _at_ usgs.gov)
```

### Comparing `lasertram-0.1.0/lasertram/calc/calc.py` & `lasertram-0.1.1/lasertram/calc/calc.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,15 +303,15 @@
                     ]
                 )
 
         # make our list an array for easier math going forward
         # std_conc_ratios = pd.DataFrame(np.array(std_conc_ratios)[np.newaxis,:],columns = myanalytes)
         self.calibration_std_conc_ratios = np.array(std_conc_ratios)
 
-    def set_internal_standard_concentrations(
+    def set_int_std_concentrations(
         self,
         spots=None,
         concentrations=None,
         uncertainties=None,
     ):
         """Assign the concentration and uncertainty of the internal standard analyte to
         a series of spots.
@@ -326,26 +326,26 @@
             uncertainties (array-like): values representing the internal standard relative uncertainty in percent. Must be the same shape as `spots`.
         """
         if spots is None:
             spots = (self.data["Spot"],)
             concentrations = (np.full(self.data["Spot"].shape[0], 10),)
             uncertainties = (np.full(self.data["Spot"].shape[0], 1),)
 
-        self.data["internal_std_comp"] = 10.0
-        self.data["internal_std_rel_unc"] = 1.0
+        self.data["int_std_comp"] = 10.0
+        self.data["int_std_rel_unc"] = 1.0
         df = self.data.reset_index().set_index("Spot")
 
         for spot, concentration, uncertainty in zip(
             spots, concentrations, uncertainties
         ):
-            df.loc[spot, "internal_std_comp"] = concentration
-            df.loc[spot, "internal_std_rel_unc"] = uncertainty
+            df.loc[spot, "int_std_comp"] = concentration
+            df.loc[spot, "int_std_rel_unc"] = uncertainty
 
-        self.data["internal_std_comp"] = df["internal_std_comp"].to_numpy()
-        self.data["internal_std_rel_unc"] = df["internal_std_rel_unc"].to_numpy()
+        self.data["int_std_comp"] = df["int_std_comp"].to_numpy()
+        self.data["int_std_rel_unc"] = df["int_std_rel_unc"].to_numpy()
 
     def calculate_concentrations(self):
         """
         Calculates the concentration and uncertainty of all spots in the experiment
         using the user specified calibration standard and internal standard
         concentrations/uncertainties.
 
@@ -431,15 +431,15 @@
                 concentrations.set_index("sample", inplace=True)
 
             secondary_standards_concentrations_list.append(concentrations)
 
         ###############################
         for sample in self.samples_nostandards:
             Cn_u = conversions.oxide_to_ppm(
-                self.data.loc[sample, "internal_std_comp"],
+                self.data.loc[sample, "int_std_comp"],
                 self.data.loc[sample, "norm"].unique()[0],
             ).to_numpy()
             Cin_std = self.calibration_std_conc_ratios
             Ni_std = self.calibration_std_stats["mean"][self.analytes].to_numpy()
             Ni_u = self.data.loc[sample, self.analytes].to_numpy()
 
             concentrations = pd.DataFrame(
@@ -669,15 +669,15 @@
 
         for sample in self.samples_nostandards:
             # concentration of internal standard in unknown uncertainties
             int_std_element = re.split(
                 r"(\d+)", self.calibration_std_data["norm"].unique()[0]
             )[2]
             # concentration of internal standard in unknown uncertainties
-            t1 = (self.data.loc[sample, "internal_std_rel_unc"] / 100) ** 2
+            t1 = (self.data.loc[sample, "int_std_rel_unc"] / 100) ** 2
             t1 = np.array(t1)
             t1 = t1[:, np.newaxis]
 
             # concentration of internal standard in calibration standard uncertainties
             t2 = (
                 self.standards_data.loc[self.calibration_std, f"{int_std_element}_std"]
                 / self.standards_data.loc[self.calibration_std, f"{int_std_element}"]
```

### Comparing `lasertram-0.1.0/lasertram/helpers/batch.py` & `lasertram-0.1.1/lasertram/helpers/batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def process_spot(
     spot,
     raw_data,
     bkgd,
     keep,
-    internal_std,
+    int_std,
     omit=None,
     despike=False,
     output_report=True,
 ):
     """a function to incorporate all the methods of the `LaserTRAM` class
     so a spot can be processed in an efficient and compact way.
 
@@ -31,15 +31,15 @@
     """
     # assign data to the spot
     spot.get_data(raw_data)
     # despike the data if desired
     if despike is True:
         spot.despike_data(analyte_list="all")
     # assign the internal standard analyte
-    spot.assign_int_std(internal_std)
+    spot.assign_int_std(int_std)
     # assign intervals for background and ablation signal
     spot.assign_intervals(bkgd=bkgd, keep=keep, omit=omit)
     # assign and save the median background values
     spot.get_bkgd_data()
     # remove the median background values from the ablation interval
     spot.subtract_bkgd()
     # calculate detection limits based off background values
```

### Comparing `lasertram-0.1.0/lasertram/helpers/conversions.py` & `lasertram-0.1.1/lasertram/helpers/conversions.py`

 * *Files identical despite different names*

### Comparing `lasertram-0.1.0/lasertram/tram/tram.py` & `lasertram-0.1.1/lasertram/tram/tram.py`

 * *Files identical despite different names*

### Comparing `lasertram-0.1.0/lasertram.egg-info/PKG-INFO` & `lasertram-0.1.1/lasertram.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 Metadata-Version: 2.1
 Name: lasertram
-Version: 0.1.0
+Version: 0.1.1
 Summary: For processing LA-ICP-MS data
 Home-page: https://github.com/jlubbersgeo/lasertram
 Author: Jordan Lubbers
 Author-email: jelubber@gmail.com
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
+Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mendeleev>=0.14.0
 Requires-Dist: numpy>=1.25.2
 Requires-Dist: pandas>=2.0.3
 Requires-Dist: scipy>=1.11.1
 Requires-Dist: statsmodels>=0.14.0
 Requires-Dist: openpyxl>=3.0.0
 
 # lasertram
-[![PyPI version](https://badge.fury.io/py/lasertram.svg)](https://badge.fury.io/py/lasertram)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff) !['coverage'](/images/COVERAGE.svg)
+
 
 Welcome to the repository for `lasertram`, a package for the time resolved analysis for processing laser ablation inductively coupled plasma mass spectrometry (LA-ICP-MS) data. It is utilized heavily in the dashboard [LaserTRAM-DB](https://github.com/jlubbersgeo/laserTRAM-DB).
 
 ## Documentation
 
 please see the [Documentation](https://jlubbersgeo.github.io/lasertram/) for more!
 
 ## Installation
-
+[![PyPI](https://img.shields.io/pypi/v/lasertram.svg?style=flat)](https://pypi.python.org/pypi/lasertram)
+[![Compatible Python Versions](https://img.shields.io/pypi/pyversions/lasertram.svg?style=flat)](https://pypi.org/project/lasertram/)
 ```
 pip install lasertram
 ```
 
 ## Contributing
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![Code Quality](https://api.codacy.com/project/badge/Grade/fd9912a3faae43bf84a47e3da685d84c)](https://app.codacy.com/gh/jlubbersgeo/lasertram/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=jlubbersgeo/lasertram&amp;utm_campaign=Badge_Grade)
 
 If you have features you'd like to see please open an issue or consider contributing yourself! I'm always happy to have help.
 
--- Jordan
+**Maintainer** Jordan Lubbers (jlubbers _at_ usgs.gov)
```

### Comparing `lasertram-0.1.0/tests/test_lasertram.py` & `lasertram-0.1.1/tests/test_lasertram.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,15 +357,15 @@
     spot2 = LaserTRAM(name="test")
     batch.process_spot(
         spot2,
         raw_data=load_data.loc[samples[0], :],
         bkgd=bkgd_interval,
         keep=keep_interval,
         omit=omit_interval,
-        internal_std="29Si",
+        int_std="29Si",
         despike=False,
         output_report=True,
     )
 
     pd.testing.assert_frame_equal(spot.output_report, spot2.output_report)
 
 
@@ -700,37 +700,37 @@
         ]
     )
     assert np.allclose(
         concentrations.calibration_std_conc_ratios, test_ratios
     ), "calibration standard concentration ratios are not correct, check again"
 
 
-def test_set_internal_standard_concentrations(load_SRM_data, load_LTcomplete_data):
+def test_set_int_std_concentrations(load_SRM_data, load_LTcomplete_data):
     """
     test to make sure concentration of the internal standard is being set correctly
     """
 
     concentrations = LaserCalc(name="test")
     concentrations.get_SRM_comps(load_SRM_data)
     concentrations.get_data(load_LTcomplete_data)
     concentrations.set_calibration_standard("BCR-2G")
     concentrations.drift_check()
     concentrations.get_calibration_std_ratios()
-    concentrations.set_internal_standard_concentrations(
+    concentrations.set_int_std_concentrations(
         concentrations.data["Spot"],
         np.full(concentrations.data["Spot"].shape[0], 71.9),
         np.full(concentrations.data["Spot"].shape[0], 1),
     )
 
     assert np.allclose(
-        concentrations.data.loc["unknown", "internal_std_comp"].values,
+        concentrations.data.loc["unknown", "int_std_comp"].values,
         np.array([71.9, 71.9, 71.9, 71.9, 71.9]),
     ), "internal standard concentrations for unknowns not set properly"
     assert np.allclose(
-        concentrations.data.loc["unknown", "internal_std_rel_unc"].values,
+        concentrations.data.loc["unknown", "int_std_rel_unc"].values,
         np.array([1.0, 1.0, 1.0, 1.0, 1.0]),
     ), "internal standard concentration uncertainties for unknowns not set properly"
 
 
 def test_calculate_concentrations(load_SRM_data, load_LTcomplete_data):
     """
     test to make sure concentrations are calculated correctly
@@ -738,15 +738,15 @@
 
     concentrations = LaserCalc(name="test")
     concentrations.get_SRM_comps(load_SRM_data)
     concentrations.get_data(load_LTcomplete_data)
     concentrations.set_calibration_standard("BCR-2G")
     concentrations.drift_check()
     concentrations.get_calibration_std_ratios()
-    concentrations.set_internal_standard_concentrations(
+    concentrations.set_int_std_concentrations(
         concentrations.data["Spot"],
         np.full(concentrations.data["Spot"].shape[0], 71.9),
         np.full(concentrations.data["Spot"].shape[0], 1),
     )
     concentrations.calculate_concentrations()
 
     test_unknown_concentrations = pd.DataFrame(
```

