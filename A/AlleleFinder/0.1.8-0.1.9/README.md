# Comparing `tmp/allelefinder-0.1.8.tar.gz` & `tmp/allelefinder-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allelefinder-0.1.8.tar", last modified: Mon Apr 29 18:57:52 2024, max compression
+gzip compressed data, was "allelefinder-0.1.9.tar", last modified: Mon Apr 29 19:28:27 2024, max compression
```

## Comparing `allelefinder-0.1.8.tar` & `allelefinder-0.1.9.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:57:52.264701 allelefinder-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:57:52.264701 allelefinder-0.1.8/AlleleFinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-29 18:57:52.000000 allelefinder-0.1.8/AlleleFinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-29 18:57:52.000000 allelefinder-0.1.8/AlleleFinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 18:57:52.000000 allelefinder-0.1.8/AlleleFinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-29 18:57:52.000000 allelefinder-0.1.8/AlleleFinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 18:57:52.000000 allelefinder-0.1.8/AlleleFinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-29 18:57:43.000000 allelefinder-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-29 18:57:52.264701 allelefinder-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-29 18:57:43.000000 allelefinder-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:57:52.260701 allelefinder-0.1.8/allele_tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:57:43.000000 allelefinder-0.1.8/allele_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26836 2024-04-29 18:57:43.000000 allelefinder-0.1.8/allele_tools/allele_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    38776 2024-04-29 18:57:43.000000 allelefinder-0.1.8/allele_tools/allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-04-29 18:57:43.000000 allelefinder-0.1.8/allele_tools/allele_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)   121713 2024-04-29 18:57:43.000000 allelefinder-0.1.8/allele_tools/methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-04-29 18:57:43.000000 allelefinder-0.1.8/allele_tools/profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    53101 2024-04-29 18:57:43.000000 allelefinder-0.1.8/allele_tools/stec.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 18:57:43.000000 allelefinder-0.1.8/allele_tools/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 18:57:52.264701 allelefinder-0.1.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2048 2024-04-29 18:57:43.000000 allelefinder-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 18:57:52.264701 allelefinder-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 18:57:43.000000 allelefinder-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-04-29 18:57:43.000000 allelefinder-0.1.8/tests/test_0_profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-04-29 18:57:43.000000 allelefinder-0.1.8/tests/test_1_allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-04-29 18:57:43.000000 allelefinder-0.1.8/tests/test_2_allele_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-29 18:57:43.000000 allelefinder-0.1.8/tests/test_3_stec_profile_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-29 18:57:43.000000 allelefinder-0.1.8/tests/test_4_stec_allele_translate_reduce.py
--rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-29 18:57:43.000000 allelefinder-0.1.8/tests/test_5_stec_allele_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-29 18:57:43.000000 allelefinder-0.1.8/tests/test_6_stec_aa_allele_find.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-29 18:57:43.000000 allelefinder-0.1.8/tests/test_7_stec_allele_split.py
--rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-29 18:57:43.000000 allelefinder-0.1.8/tests/test_8_stec_allele_concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-29 18:57:43.000000 allelefinder-0.1.8/tests/test_9_stec_allele_translate_find.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:28:27.264323 allelefinder-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:28:27.264323 allelefinder-0.1.9/AlleleFinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-29 19:28:27.000000 allelefinder-0.1.9/AlleleFinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-29 19:28:27.000000 allelefinder-0.1.9/AlleleFinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 19:28:27.000000 allelefinder-0.1.9/AlleleFinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-29 19:28:27.000000 allelefinder-0.1.9/AlleleFinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-29 19:28:27.000000 allelefinder-0.1.9/AlleleFinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-29 19:28:19.000000 allelefinder-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-29 19:28:19.000000 allelefinder-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-04-29 19:28:27.264323 allelefinder-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-29 19:28:19.000000 allelefinder-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:28:27.264323 allelefinder-0.1.9/allele_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26836 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/allele_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38776 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31560 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121713 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53101 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/stec.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-29 19:28:19.000000 allelefinder-0.1.9/allele_tools/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-29 19:28:19.000000 allelefinder-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 19:28:27.264323 allelefinder-0.1.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2048 2024-04-29 19:28:19.000000 allelefinder-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 19:28:27.264323 allelefinder-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15501 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_0_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15193 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_1_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15736 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_2_allele_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_3_stec_profile_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_4_stec_allele_translate_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_5_stec_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_6_stec_aa_allele_find.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_7_stec_allele_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17176 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_8_stec_allele_concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-29 19:28:19.000000 allelefinder-0.1.9/tests/test_9_stec_allele_translate_find.py
```

### Comparing `allelefinder-0.1.8/AlleleFinder.egg-info/PKG-INFO` & `allelefinder-0.1.9/AlleleFinder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlleleFinder
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/OLC-Bioinformatics/AlleleFinder
 Author: Adam Koziol
 Author-email: adam.koziol@inspection.gc.ca
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `allelefinder-0.1.8/AlleleFinder.egg-info/SOURCES.txt` & `allelefinder-0.1.9/AlleleFinder.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 LICENSE
+MANIFEST.in
 README.md
+requirements.txt
 setup.py
 AlleleFinder.egg-info/PKG-INFO
 AlleleFinder.egg-info/SOURCES.txt
 AlleleFinder.egg-info/dependency_links.txt
 AlleleFinder.egg-info/requires.txt
 AlleleFinder.egg-info/top_level.txt
 allele_tools/__init__.py
```

### Comparing `allelefinder-0.1.8/LICENSE` & `allelefinder-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/PKG-INFO` & `allelefinder-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlleleFinder
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/OLC-Bioinformatics/AlleleFinder
 Author: Adam Koziol
 Author-email: adam.koziol@inspection.gc.ca
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `allelefinder-0.1.8/README.md` & `allelefinder-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/allele_tools/allele_profiler.py` & `allelefinder-0.1.9/allele_tools/allele_profiler.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/allele_tools/allele_translate_reduce.py` & `allelefinder-0.1.9/allele_tools/allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/allele_tools/allele_updater.py` & `allelefinder-0.1.9/allele_tools/allele_updater.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/allele_tools/methods.py` & `allelefinder-0.1.9/allele_tools/methods.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/allele_tools/profile_reduce.py` & `allelefinder-0.1.9/allele_tools/profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/allele_tools/stec.py` & `allelefinder-0.1.9/allele_tools/stec.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/setup.py` & `allelefinder-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/tests/test_0_profile_reduce.py` & `allelefinder-0.1.9/tests/test_0_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/tests/test_1_allele_translate_reduce.py` & `allelefinder-0.1.9/tests/test_1_allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/tests/test_2_allele_updater.py` & `allelefinder-0.1.9/tests/test_2_allele_updater.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/tests/test_3_stec_profile_reduce.py` & `allelefinder-0.1.9/tests/test_3_stec_profile_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/tests/test_4_stec_allele_translate_reduce.py` & `allelefinder-0.1.9/tests/test_4_stec_allele_translate_reduce.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/tests/test_5_stec_allele_find.py` & `allelefinder-0.1.9/tests/test_5_stec_allele_find.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/tests/test_6_stec_aa_allele_find.py` & `allelefinder-0.1.9/tests/test_6_stec_aa_allele_find.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/tests/test_7_stec_allele_split.py` & `allelefinder-0.1.9/tests/test_7_stec_allele_split.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/tests/test_8_stec_allele_concatenate.py` & `allelefinder-0.1.9/tests/test_8_stec_allele_concatenate.py`

 * *Files identical despite different names*

### Comparing `allelefinder-0.1.8/tests/test_9_stec_allele_translate_find.py` & `allelefinder-0.1.9/tests/test_9_stec_allele_translate_find.py`

 * *Files identical despite different names*

