# Comparing `tmp/onion_clustering-0.1.4.tar.gz` & `tmp/onion_clustering-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onion_clustering-0.1.4.tar", last modified: Tue Apr 23 13:36:47 2024, max compression
+gzip compressed data, was "onion_clustering-0.1.5.tar", last modified: Mon Apr 29 14:35:36 2024, max compression
```

## Comparing `onion_clustering-0.1.4.tar` & `onion_clustering-0.1.5.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.651843 onion_clustering-0.1.4/
--rw-r--r--   0 mattebecchi   (501) staff       (20)    53248 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/.coverage
--rw-r--r--   0 mattebecchi   (501) staff       (20)       50 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/.gitignore
--rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.1.4/LICENSE
--rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-04-23 13:36:47.650762 onion_clustering-0.1.4/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)     5652 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/README.md
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.621250 onion_clustering-0.1.4/examples/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3664 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/examples/example_script.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3669 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/examples/example_script_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)      635 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/justfile
--rw-r--r--   0 mattebecchi   (501) staff       (20)      942 2024-04-23 13:36:22.000000 onion_clustering-0.1.4/pyproject.toml
--rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.1.4/pytest.ini
--rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-04-23 13:36:47.652041 onion_clustering-0.1.4/setup.cfg
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.608999 onion_clustering-0.1.4/src/
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.630698 onion_clustering-0.1.4/src/onion_clustering/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/src/onion_clustering/__init__.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)      465 2024-02-26 12:16:27.000000 onion_clustering-0.1.4/src/onion_clustering/__version__.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    34309 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/src/onion_clustering/classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    19431 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/src/onion_clustering/first_classes.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    23224 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/src/onion_clustering/functions.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    17172 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/src/onion_clustering/main.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    23148 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/src/onion_clustering/main_2d.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/src/onion_clustering/utilities.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.649444 onion_clustering-0.1.4/src/onion_clustering.egg-info/
--rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-04-23 13:36:47.000000 onion_clustering-0.1.4/src/onion_clustering.egg-info/PKG-INFO
--rw-r--r--   0 mattebecchi   (501) staff       (20)      878 2024-04-23 13:36:47.000000 onion_clustering-0.1.4/src/onion_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-04-23 13:36:47.000000 onion_clustering-0.1.4/src/onion_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-04-23 13:36:47.000000 onion_clustering-0.1.4/src/onion_clustering.egg-info/requires.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-04-23 13:36:47.000000 onion_clustering-0.1.4/src/onion_clustering.egg-info/top_level.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.639323 onion_clustering-0.1.4/test/
--rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.1.4/test/__init__.py
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.643144 onion_clustering-0.1.4/test/output_multi/
--rw-r--r--   0 mattebecchi   (501) staff       (20)      409 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/output_multi/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/output_multi/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/output_multi/number_of_states.txt
-drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-23 13:36:47.648433 onion_clustering-0.1.4/test/output_uni/
--rw-r--r--   0 mattebecchi   (501) staff       (20)      265 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/output_uni/final_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/output_uni/fraction_0.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/output_uni/number_of_states.txt
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3361 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/test_multi.py
--rw-r--r--   0 mattebecchi   (501) staff       (20)     3271 2024-04-23 13:35:32.000000 onion_clustering-0.1.4/test/test_uni.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.540272 onion_clustering-0.1.5/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    53248 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/.coverage
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       50 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/.gitignore
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     1068 2024-02-16 13:11:19.000000 onion_clustering-0.1.5/LICENSE
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-04-29 14:35:36.539260 onion_clustering-0.1.5/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     5652 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/README.md
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.523382 onion_clustering-0.1.5/examples/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3664 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/examples/example_script.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3669 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/examples/example_script_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      635 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/justfile
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      942 2024-04-29 14:35:03.000000 onion_clustering-0.1.5/pyproject.toml
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       26 2024-02-21 15:08:50.000000 onion_clustering-0.1.5/pytest.ini
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       38 2024-04-29 14:35:36.540594 onion_clustering-0.1.5/setup.cfg
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.517796 onion_clustering-0.1.5/src/
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.528542 onion_clustering-0.1.5/src/onion_clustering/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/__init__.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      465 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/__version__.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    34309 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    19431 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/first_classes.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    23244 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/functions.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    17172 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/main.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    23148 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/main_2d.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)    15728 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/src/onion_clustering/utilities.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.538152 onion_clustering-0.1.5/src/onion_clustering.egg-info/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     6088 2024-04-29 14:35:36.000000 onion_clustering-0.1.5/src/onion_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      878 2024-04-29 14:35:36.000000 onion_clustering-0.1.5/src/onion_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        1 2024-04-29 14:35:36.000000 onion_clustering-0.1.5/src/onion_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       30 2024-04-29 14:35:36.000000 onion_clustering-0.1.5/src/onion_clustering.egg-info/requires.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       17 2024-04-29 14:35:36.000000 onion_clustering-0.1.5/src/onion_clustering.egg-info/top_level.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.533722 onion_clustering-0.1.5/test/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)        0 2024-02-16 13:11:19.000000 onion_clustering-0.1.5/test/__init__.py
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.535537 onion_clustering-0.1.5/test/output_multi/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      409 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/output_multi/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/output_multi/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/output_multi/number_of_states.txt
+drwxr-xr-x   0 mattebecchi   (501) staff       (20)        0 2024-04-29 14:35:36.537357 onion_clustering-0.1.5/test/output_uni/
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      265 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/output_uni/final_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)      204 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/output_uni/fraction_0.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)       67 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/output_uni/number_of_states.txt
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3361 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/test_multi.py
+-rw-r--r--   0 mattebecchi   (501) staff       (20)     3271 2024-04-29 14:33:59.000000 onion_clustering-0.1.5/test/test_uni.py
```

### Comparing `onion_clustering-0.1.4/.coverage` & `onion_clustering-0.1.5/.coverage`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.4/LICENSE` & `onion_clustering-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.4/PKG-INFO` & `onion_clustering-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.1.4
+Version: 0.1.5
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `onion_clustering-0.1.4/README.md` & `onion_clustering-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.4/examples/example_script.py` & `onion_clustering-0.1.5/examples/example_script.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.4/examples/example_script_2d.py` & `onion_clustering-0.1.5/examples/example_script_2d.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.4/justfile` & `onion_clustering-0.1.5/justfile`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.4/pyproject.toml` & `onion_clustering-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "onion_clustering"
-version = "0.1.4"
+version = "0.1.5"
 description = "Code for unsupervised clustering of time-correlated data."
 # license = "MIT"
 maintainers = [
   { name = "Matteo Becchi", email = "bechmath@gmail.com" },
 ]
 dependencies = [
   "matplotlib",
```

### Comparing `onion_clustering-0.1.4/src/onion_clustering/classes.py` & `onion_clustering-0.1.5/src/onion_clustering/classes.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.4/src/onion_clustering/first_classes.py` & `onion_clustering-0.1.5/src/onion_clustering/first_classes.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.4/src/onion_clustering/functions.py` & `onion_clustering-0.1.5/src/onion_clustering/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -491,25 +491,25 @@
         updated_states[i].th_sup[1] = th_type
         updated_states[i + 1].th_inf[0] = th_val
         updated_states[i + 1].th_inf[1] = th_type
 
     updated_states[-1].th_sup[0] = m_range[1]
     updated_states[-1].th_sup[1] = 0
 
-    if updated_states[0].th_sup[0] < m_range[0]:
-        updated_states.pop(0)
-        updated_states[0].th_inf[0] = m_range[0]
-        mask = all_the_labels > 1
-        all_the_labels[mask] -= 1
+    # if updated_states[0].th_sup[0] < m_range[0]:
+    #     updated_states.pop(0)
+    #     updated_states[0].th_inf[0] = m_range[0]
+    #     mask = all_the_labels > 1
+    #     all_the_labels[mask] -= 1
 
-    if updated_states[-1].th_inf[0] > m_range[1]:
-        updated_states.pop(-1)
-        updated_states[-1].th_inf[1] = m_range[1]
-        mask = all_the_labels == np.max(all_the_labels)
-        all_the_labels[mask] -= 1
+    # if updated_states[-1].th_inf[0] > m_range[1]:
+    #     updated_states.pop(-1)
+    #     updated_states[-1].th_inf[1] = m_range[1]
+    #     mask = all_the_labels == np.max(all_the_labels)
+    #     all_the_labels[mask] -= 1
 
     # Step 3: Write the final states and final thresholds to text files.
     # The data is saved in two separate files:
     # 'final_states.txt' and 'final_thresholds.txt'.
     with open("final_states.txt", "w", encoding="utf-8") as file:
         print("# Mu \t Sigma \t A \t state_fraction", file=file)
         for state in updated_states:
```

### Comparing `onion_clustering-0.1.4/src/onion_clustering/main.py` & `onion_clustering-0.1.5/src/onion_clustering/main.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.4/src/onion_clustering/main_2d.py` & `onion_clustering-0.1.5/src/onion_clustering/main_2d.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.4/src/onion_clustering/utilities.py` & `onion_clustering-0.1.5/src/onion_clustering/utilities.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.4/src/onion_clustering.egg-info/PKG-INFO` & `onion_clustering-0.1.5/src/onion_clustering.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onion_clustering
-Version: 0.1.4
+Version: 0.1.5
 Summary: Code for unsupervised clustering of time-correlated data.
 Maintainer-email: Matteo Becchi <bechmath@gmail.com>
 Project-URL: github, https://github.com/matteobecchi/timeseries_analysis/
 Requires-Python: <3.11,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib
```

### Comparing `onion_clustering-0.1.4/src/onion_clustering.egg-info/SOURCES.txt` & `onion_clustering-0.1.5/src/onion_clustering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.4/test/test_multi.py` & `onion_clustering-0.1.5/test/test_multi.py`

 * *Files identical despite different names*

### Comparing `onion_clustering-0.1.4/test/test_uni.py` & `onion_clustering-0.1.5/test/test_uni.py`

 * *Files identical despite different names*

