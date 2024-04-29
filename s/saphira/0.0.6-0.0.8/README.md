# Comparing `tmp/saphira-0.0.6.tar.gz` & `tmp/saphira-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saphira-0.0.6.tar", last modified: Tue Apr  9 06:30:57 2024, max compression
+gzip compressed data, was "saphira-0.0.8.tar", last modified: Mon Apr 29 15:58:40 2024, max compression
```

## Comparing `saphira-0.0.6.tar` & `saphira-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-09 06:30:57.710459 saphira-0.0.6/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     1063 2023-12-22 05:35:11.000000 saphira-0.0.6/LICENSE
--rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-09 06:30:57.709797 saphira-0.0.6/PKG-INFO
--rw-r--r--   0 akshaychalana   (501) staff       (20)       71 2023-12-19 02:46:29.000000 saphira-0.0.6/README.md
--rw-r--r--   0 akshaychalana   (501) staff       (20)      718 2024-04-09 06:30:43.000000 saphira-0.0.6/pyproject.toml
--rw-r--r--   0 akshaychalana   (501) staff       (20)       38 2024-04-09 06:30:57.710593 saphira-0.0.6/setup.cfg
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-09 06:30:57.696519 saphira-0.0.6/src/
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-09 06:30:57.700679 saphira-0.0.6/src/saphira/
--rw-r--r--   0 akshaychalana   (501) staff       (20)       45 2024-04-09 06:30:35.000000 saphira-0.0.6/src/saphira/__init__.py
--rw-r--r--   0 akshaychalana   (501) staff       (20)     2314 2024-04-08 22:53:39.000000 saphira-0.0.6/src/saphira/saphira.py
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-09 06:30:57.708224 saphira-0.0.6/src/saphira.egg-info/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-09 06:30:57.000000 saphira-0.0.6/src/saphira.egg-info/PKG-INFO
--rw-r--r--   0 akshaychalana   (501) staff       (20)      310 2024-04-09 06:30:57.000000 saphira-0.0.6/src/saphira.egg-info/SOURCES.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)        1 2024-04-09 06:30:57.000000 saphira-0.0.6/src/saphira.egg-info/dependency_links.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)       53 2024-04-09 06:30:57.000000 saphira-0.0.6/src/saphira.egg-info/requires.txt
--rw-r--r--   0 akshaychalana   (501) staff       (20)        8 2024-04-09 06:30:57.000000 saphira-0.0.6/src/saphira.egg-info/top_level.txt
-drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-09 06:30:57.707249 saphira-0.0.6/tests/
--rw-r--r--   0 akshaychalana   (501) staff       (20)     1686 2024-04-08 23:08:05.000000 saphira-0.0.6/tests/test_battery_capacity.py
--rw-r--r--   0 akshaychalana   (501) staff       (20)      596 2023-11-18 02:00:44.000000 saphira-0.0.6/tests/test_jama_server.py
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-29 15:58:40.316375 saphira-0.0.8/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     1063 2023-12-22 05:35:11.000000 saphira-0.0.8/LICENSE
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-29 15:58:40.314785 saphira-0.0.8/PKG-INFO
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       71 2023-12-19 02:46:29.000000 saphira-0.0.8/README.md
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      718 2024-04-29 15:57:58.000000 saphira-0.0.8/pyproject.toml
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       38 2024-04-29 15:58:40.316511 saphira-0.0.8/setup.cfg
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-29 15:58:40.287562 saphira-0.0.8/src/
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-29 15:58:40.296326 saphira-0.0.8/src/saphira/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       45 2024-04-29 15:57:44.000000 saphira-0.0.8/src/saphira/__init__.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     3898 2024-04-28 08:11:22.000000 saphira-0.0.8/src/saphira/saphira.py
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-29 15:58:40.313184 saphira-0.0.8/src/saphira.egg-info/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     2008 2024-04-29 15:58:40.000000 saphira-0.0.8/src/saphira.egg-info/PKG-INFO
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      373 2024-04-29 15:58:40.000000 saphira-0.0.8/src/saphira.egg-info/SOURCES.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)        1 2024-04-29 15:58:40.000000 saphira-0.0.8/src/saphira.egg-info/dependency_links.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)       53 2024-04-29 15:58:40.000000 saphira-0.0.8/src/saphira.egg-info/requires.txt
+-rw-r--r--   0 akshaychalana   (501) staff       (20)        8 2024-04-29 15:58:40.000000 saphira-0.0.8/src/saphira.egg-info/top_level.txt
+drwxr-xr-x   0 akshaychalana   (501) staff       (20)        0 2024-04-29 15:58:40.311064 saphira-0.0.8/tests/
+-rw-r--r--   0 akshaychalana   (501) staff       (20)     1743 2024-04-27 00:19:40.000000 saphira-0.0.8/tests/test_battery_capacity.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      660 2024-04-09 06:41:30.000000 saphira-0.0.8/tests/test_energy_density.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      596 2023-11-18 02:00:44.000000 saphira-0.0.8/tests/test_jama_server.py
+-rw-r--r--   0 akshaychalana   (501) staff       (20)      782 2024-04-28 17:31:20.000000 saphira-0.0.8/tests/test_radar_state_machine.py
```

### Comparing `saphira-0.0.6/LICENSE` & `saphira-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `saphira-0.0.6/PKG-INFO` & `saphira-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saphira
-Version: 0.0.6
+Version: 0.0.8
 Summary: Access parameters from the Saphira.ai SysEng SSoT
 Author-email: Saphira AI <contact@saphira.ai>
 License: MIT License
         
         Copyright (c) 2023 Saphira
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `saphira-0.0.6/pyproject.toml` & `saphira-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saphira"
-version = "0.0.6"
+version = "0.0.8"
 description = "Access parameters from the Saphira.ai SysEng SSoT"
 readme = "README.md"
 authors = [{ name = "Saphira AI", email = "contact@saphira.ai" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `saphira-0.0.6/src/saphira.egg-info/PKG-INFO` & `saphira-0.0.8/src/saphira.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saphira
-Version: 0.0.6
+Version: 0.0.8
 Summary: Access parameters from the Saphira.ai SysEng SSoT
 Author-email: Saphira AI <contact@saphira.ai>
 License: MIT License
         
         Copyright (c) 2023 Saphira
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `saphira-0.0.6/tests/test_battery_capacity.py` & `saphira-0.0.8/tests/test_battery_capacity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import traceback
 import unittest
 import os
 os.environ['SAPHIRA_URL'] = 'http://localhost:8081'
 import saphira
 
 PROJECT = '83092519-da63-4882-a899-297e3e62b65d.json'
 REQ = 'BattRef-0001'
@@ -18,17 +19,18 @@
         
         # Calculate the minimum required battery capacity in kWh
         min_battery_capacity_kWh = minimum_range * energy_density / 1000
         
         # Assert the minimum battery capacity supports the required range
         self.assertGreaterEqual(battery_weight, 0, "Battery weight cannot be negative")
         self.assertTrue(min_battery_capacity_kWh > 0, "Minimum battery capacity must be positive")
-        self.assertTrue(battery_weight < 500, "Battery weight should be reasonable (< 500 kg)")
+        self.assertTrue(battery_weight > 500, "Battery weight should be reasonable (< 500 kg)")
         self.assertTrue(min_battery_capacity_kWh * 1000 / energy_density >= minimum_range, f"Minimum battery capacity should support at least {minimum_range} km range, is " + str(min_battery_capacity_kWh))
         self.assertTrue(min_battery_capacity_kWh <= 250, "Minimum battery capacity should not exceed required energy density")
 
 if __name__ == '__main__':
     try:
         test = unittest.main(exit=False)
-        saphira.update_test_status(PROJECT, REQ, test.result.wasSuccessful())
+        saphira.update_test_status(PROJECT, REQ, test_result=test.result)
     except Exception as e:
-        saphira.update_test_status(PROJECT, REQ, False)
+        print(traceback.format_exc())
+        saphira.update_test_status(PROJECT, REQ, exception=e)
```

### Comparing `saphira-0.0.6/tests/test_jama_server.py` & `saphira-0.0.8/tests/test_jama_server.py`

 * *Files identical despite different names*

