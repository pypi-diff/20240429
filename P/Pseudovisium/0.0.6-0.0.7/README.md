# Comparing `tmp/Pseudovisium-0.0.6.tar.gz` & `tmp/Pseudovisium-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pseudovisium-0.0.6.tar", last modified: Sun Apr 28 09:37:10 2024, max compression
+gzip compressed data, was "Pseudovisium-0.0.7.tar", last modified: Mon Apr 29 10:56:38 2024, max compression
```

## Comparing `Pseudovisium-0.0.6.tar` & `Pseudovisium-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-28 09:37:10.208483 Pseudovisium-0.0.6/
--rw-r--r--   0 k23030440   (504) staff       (20)     1065 2024-04-08 13:33:17.000000 Pseudovisium-0.0.6/LICENSE
--rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-28 09:37:10.208262 Pseudovisium-0.0.6/PKG-INFO
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-28 09:37:10.206135 Pseudovisium-0.0.6/Pseudovisium/
--rw-r--r--   0 k23030440   (504) staff       (20)        0 2024-04-18 09:05:07.000000 Pseudovisium-0.0.6/Pseudovisium/__init__.py
--rw-r--r--   0 k23030440   (504) staff       (20)    58610 2024-04-28 08:09:58.000000 Pseudovisium-0.0.6/Pseudovisium/pseudovisium_generate.py
--rw-r--r--   0 k23030440   (504) staff       (20)    14501 2024-04-23 21:00:08.000000 Pseudovisium-0.0.6/Pseudovisium/pseudovisium_merge.py
--rw-r--r--   0 k23030440   (504) staff       (20)    68606 2024-04-24 16:52:07.000000 Pseudovisium-0.0.6/Pseudovisium/pseudovisium_qc.py
-drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-28 09:37:10.207891 Pseudovisium-0.0.6/Pseudovisium.egg-info/
--rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-28 09:37:10.000000 Pseudovisium-0.0.6/Pseudovisium.egg-info/PKG-INFO
--rw-r--r--   0 k23030440   (504) staff       (20)      335 2024-04-28 09:37:10.000000 Pseudovisium-0.0.6/Pseudovisium.egg-info/SOURCES.txt
--rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-04-28 09:37:10.000000 Pseudovisium-0.0.6/Pseudovisium.egg-info/dependency_links.txt
--rw-r--r--   0 k23030440   (504) staff       (20)       39 2024-04-28 09:37:10.000000 Pseudovisium-0.0.6/Pseudovisium.egg-info/requires.txt
--rw-r--r--   0 k23030440   (504) staff       (20)       13 2024-04-28 09:37:10.000000 Pseudovisium-0.0.6/Pseudovisium.egg-info/top_level.txt
--rw-r--r--   0 k23030440   (504) staff       (20)     3637 2024-04-26 08:21:23.000000 Pseudovisium-0.0.6/README.md
--rw-r--r--   0 k23030440   (504) staff       (20)       38 2024-04-28 09:37:10.208534 Pseudovisium-0.0.6/setup.cfg
--rw-r--r--   0 k23030440   (504) staff       (20)      911 2024-04-28 09:36:31.000000 Pseudovisium-0.0.6/setup.py
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-29 10:56:38.125072 Pseudovisium-0.0.7/
+-rw-r--r--   0 k23030440   (504) staff       (20)     1065 2024-04-08 13:33:17.000000 Pseudovisium-0.0.7/LICENSE
+-rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-29 10:56:38.124775 Pseudovisium-0.0.7/PKG-INFO
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-29 10:56:38.120919 Pseudovisium-0.0.7/Pseudovisium/
+-rw-r--r--   0 k23030440   (504) staff       (20)        0 2024-04-18 09:05:07.000000 Pseudovisium-0.0.7/Pseudovisium/__init__.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    58663 2024-04-29 10:55:34.000000 Pseudovisium-0.0.7/Pseudovisium/pseudovisium_generate.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    14501 2024-04-23 21:00:08.000000 Pseudovisium-0.0.7/Pseudovisium/pseudovisium_merge.py
+-rw-r--r--   0 k23030440   (504) staff       (20)    68606 2024-04-24 16:52:07.000000 Pseudovisium-0.0.7/Pseudovisium/pseudovisium_qc.py
+drwxr-xr-x   0 k23030440   (504) staff       (20)        0 2024-04-29 10:56:38.123590 Pseudovisium-0.0.7/Pseudovisium.egg-info/
+-rw-r--r--   0 k23030440   (504) staff       (20)      591 2024-04-29 10:56:38.000000 Pseudovisium-0.0.7/Pseudovisium.egg-info/PKG-INFO
+-rw-r--r--   0 k23030440   (504) staff       (20)      335 2024-04-29 10:56:38.000000 Pseudovisium-0.0.7/Pseudovisium.egg-info/SOURCES.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)        1 2024-04-29 10:56:38.000000 Pseudovisium-0.0.7/Pseudovisium.egg-info/dependency_links.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)       39 2024-04-29 10:56:38.000000 Pseudovisium-0.0.7/Pseudovisium.egg-info/requires.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)       13 2024-04-29 10:56:38.000000 Pseudovisium-0.0.7/Pseudovisium.egg-info/top_level.txt
+-rw-r--r--   0 k23030440   (504) staff       (20)     3637 2024-04-26 08:21:23.000000 Pseudovisium-0.0.7/README.md
+-rw-r--r--   0 k23030440   (504) staff       (20)       38 2024-04-29 10:56:38.125271 Pseudovisium-0.0.7/setup.cfg
+-rw-r--r--   0 k23030440   (504) staff       (20)      911 2024-04-29 10:56:35.000000 Pseudovisium-0.0.7/setup.py
```

### Comparing `Pseudovisium-0.0.6/LICENSE` & `Pseudovisium-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `Pseudovisium-0.0.6/PKG-INFO` & `Pseudovisium-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pseudovisium
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package for hexagonal binning of high-resolution spatial transcriptomic data
 Author: Bence Kover
 Author-email: <kover.bence@gmail.com>
 Keywords: spatial,transcriptomics,visium,xenium,cosmx
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Pseudovisium-0.0.6/Pseudovisium/pseudovisium_generate.py` & `Pseudovisium-0.0.7/Pseudovisium/pseudovisium_generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,27 +277,14 @@
         returning_items.append(hexagon_quality)
     if quality_per_probe==True:
         returning_items.append(probe_quality)
     return tuple(returning_items)
 
 
 
-    
-
-
-def process_batch_hexagons(batch,hexagon_counts,hexagon_names,features):
-        batch_matrix_data = []
-        for hexagon in batch:
-            count_dict = hexagon_counts.get(hexagon, {})
-            hexagon_index = hexagon_names.index(hexagon)
-            for feature, count in count_dict.items():
-                feature_index = features.index(feature)
-                batch_matrix_data.append([feature_index+1, hexagon_index+1, count])
-        return batch_matrix_data
-
 
 def write_10X_h5(adata, file):
     """Writes adata to a 10X-formatted h5 file.
     
     Note that this function is not fully tested and may not work for all cases.
     It will not write the following keys to the h5 file compared to 10X:
     '_all_tag_keys', 'pattern', 'read', 'sequence'
@@ -538,20 +525,21 @@
 
 
 
 def process_hexagon(hexagon, hexagon_index, features, hexagon_counts):
         return [[features.index(feature) + 1, hexagon_index + 1, count]
                 for feature, count in hexagon_counts[hexagon].items()]
 
-def hex_to_rows(hexagon_batch, start_index, features, hexagon_counts):
+def hex_to_rows(hexagon_batch, start_index, features, hexagon_counts,hexagon_names):
     matrix_data = []
-    for hexagon_index, hexagon in enumerate(hexagon_batch, start=start_index): ###Here is the error!!! HExagon indices are scrambled!!!!!
+    for hexagon in hexagon_batch: ###Here is the error!!! HExagon indices are scrambled!!!!!
         count_dict = hexagon_counts.get(hexagon, {})
         for feature, count in count_dict.items():
             feature_index = features.index(feature)
+            hexagon_index = hexagon_names.index(hexagon)
             matrix_data.append([feature_index + 1, hexagon_index + 1, count])
     print(f"Batch total count: {sum(row[2] for row in matrix_data)}")
     return matrix_data
 
 def create_pseudovisium(path,hexagon_counts,hexagon_cell_counts,hexagon_quality, probe_quality,
                         img_file_path=None,  project_name="project",
                          alignment_matrix_file=None,image_pixels_per_um=1/0.2125,hexagon_size=100,tissue_hires_scalef=0.2,
@@ -695,28 +683,32 @@
 
     print("Putting together the matrix.mtx file")
     matrix_data = []
 
     n_total_hexagons = len(ordered_hexagon_counts)
 
     total_count = 0
-    matrix_data = []
+    n_processes = min(max_workers, multiprocessing.cpu_count())
+    batch_size_n_hexagons = n_total_hexagons // (n_processes * 4)
+    print(f"Using {n_processes} processes")
+    print(f"Processing {n_total_hexagons} hexagons in batches of {batch_size_n_hexagons} hexagons")
+    with concurrent.futures.ProcessPoolExecutor(max_workers=n_processes) as executor:
+        futures = []
+        for i in range(0, n_total_hexagons, batch_size_n_hexagons):
+            hexagon_batch = hexagon_names[i:i + batch_size_n_hexagons]
+            future = executor.submit(hex_to_rows, hexagon_batch, i, features, ordered_hexagon_counts,hexagon_names)
+            futures.append(future)
 
-    for hexagon, count_dict in hexagon_counts.items():
-        if sum(count_dict.values()) > 0:
-            hexagon_index = hexagon_names.index(hexagon)
-            for feature, count in count_dict.items():
-                feature_index = features.index(feature)
-                matrix_data.append([feature_index+1, hexagon_index+1, count])
-                total_count += count
-    
+        with tqdm(total=len(futures), desc="Processing batches") as pbar:
+            for future in concurrent.futures.as_completed(futures):
+                batch_matrix_data = future.result()
+                matrix_data.extend(batch_matrix_data)
+                total_count += sum(row[2] for row in batch_matrix_data)
+                pbar.update(1)
 
-    data = np.array(matrix_data)[:, 2]
-    row_indices = np.array(matrix_data)[:, 0] - 1
-    col_indices = np.array(matrix_data)[:, 1] - 1
     print(f"Total matrix count: {total_count}")
     unique_hexagons = len(set(hexagon_names))
     print(f"Number of unique hexagons: {unique_hexagons}")
     print(f"Number of hexagons in ordered_hexagon_counts: {len(ordered_hexagon_counts)}")
 
     
 
@@ -1069,15 +1061,15 @@
     parser.add_argument("--csv_file", "-c", type=str, help="CSV file path", default=None)
     parser.add_argument("--output_path", "-o", type=str, help="Output path", default='.')
     parser.add_argument("--hexagon_size", "-hs", type=int, help="Hexagon size", default=100)
     parser.add_argument("--img_file_path", "-i", type=str, help="Image file path", default=None)
     parser.add_argument("--alignment_matrix_file", "-am", type=str, help="Alignment matrix file path", default=None)
     parser.add_argument("--batch_size", "-b", type=int, help="Batch size", default=1000000)
     parser.add_argument("--project_name", "-p", type=str, help="Project name", default='project')
-    parser.add_argument("--image_pixels_per_um", "-ppu", type=float, help="Image pixels per um", default=1/0.2125)#change!
+    parser.add_argument("--image_pixels_per_um", "-ppu", type=float, help="Image pixels per um", default=1)#changed from 1/0.2125 that was set for Xenium
     parser.add_argument("--tissue_hires_scalef", "-ths", type=float, help="Tissue hires scale factor", default=0.2)
     parser.add_argument("--technology", "-t", type=str, help="Technology", default="Xenium")
     parser.add_argument("--feature_colname", "-fc", type=str, help="Feature column name", default="feature_name")
     parser.add_argument("--x_colname", "-xc", type=str, help="X column name", default="x_location")
     parser.add_argument("--y_colname", "-yc", type=str, help="Y column name", default="y_location")
     parser.add_argument("--cell_id_colname", "-cc", type=str, help="Cell ID column name", default="None")
     parser.add_argument("--pixel_to_micron", "-ptm", action="store_true", help="Convert pixel to micron")
```

### Comparing `Pseudovisium-0.0.6/Pseudovisium/pseudovisium_merge.py` & `Pseudovisium-0.0.7/Pseudovisium/pseudovisium_merge.py`

 * *Files identical despite different names*

### Comparing `Pseudovisium-0.0.6/Pseudovisium/pseudovisium_qc.py` & `Pseudovisium-0.0.7/Pseudovisium/pseudovisium_qc.py`

 * *Files identical despite different names*

### Comparing `Pseudovisium-0.0.6/Pseudovisium.egg-info/PKG-INFO` & `Pseudovisium-0.0.7/Pseudovisium.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pseudovisium
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python package for hexagonal binning of high-resolution spatial transcriptomic data
 Author: Bence Kover
 Author-email: <kover.bence@gmail.com>
 Keywords: spatial,transcriptomics,visium,xenium,cosmx
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Pseudovisium-0.0.6/README.md` & `Pseudovisium-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `Pseudovisium-0.0.6/setup.py` & `Pseudovisium-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #this is a setup.py file
 from setuptools import setup, find_packages
 
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Python package for hexagonal binning of high-resolution spatial transcriptomic data'
 LONG_DESCRIPTION = 'Python package for hexagonal binning of high-resolution spatial transcriptomic data, for more information see https://github.com/BKover99/pseudovisium'
 
 
 setup(
     name="Pseudovisium",
     version=VERSION,
```

