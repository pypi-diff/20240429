# Comparing `tmp/aivol-0.0.6.tar.gz` & `tmp/aivol-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aivol-0.0.6.tar", last modified: Mon Apr  1 08:37:03 2024, max compression
+gzip compressed data, was "aivol-0.0.7.tar", last modified: Mon Apr 29 11:30:59 2024, max compression
```

## Comparing `aivol-0.0.6.tar` & `aivol-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dmitry    (1000) dmitry    (1000)        0 2024-04-01 08:37:03.556056 aivol-0.0.6/
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)     1074 2024-03-14 07:38:11.000000 aivol-0.0.6/LICENSE
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)      474 2024-04-01 08:37:03.556056 aivol-0.0.6/PKG-INFO
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)       50 2024-03-11 08:49:25.000000 aivol-0.0.6/README.md
-drwxr-xr-x   0 dmitry    (1000) dmitry    (1000)        0 2024-04-01 08:37:03.556056 aivol-0.0.6/aivol/
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)       88 2024-03-14 08:57:27.000000 aivol-0.0.6/aivol/__init__.py
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)     4601 2024-03-26 12:58:43.000000 aivol-0.0.6/aivol/compare.py
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)     1941 2024-03-14 09:26:30.000000 aivol-0.0.6/aivol/config.py
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)     2436 2024-03-14 08:44:58.000000 aivol-0.0.6/aivol/experiment.py
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)     2825 2024-03-21 10:08:22.000000 aivol-0.0.6/aivol/resolve.py
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)     7199 2024-04-01 08:35:24.000000 aivol-0.0.6/aivol/sidecar.py
-drwxr-xr-x   0 dmitry    (1000) dmitry    (1000)        0 2024-04-01 08:37:03.556056 aivol-0.0.6/aivol.egg-info/
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)      474 2024-04-01 08:37:03.000000 aivol-0.0.6/aivol.egg-info/PKG-INFO
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)      290 2024-04-01 08:37:03.000000 aivol-0.0.6/aivol.egg-info/SOURCES.txt
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)        1 2024-04-01 08:37:03.000000 aivol-0.0.6/aivol.egg-info/dependency_links.txt
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)       24 2024-04-01 08:37:03.000000 aivol-0.0.6/aivol.egg-info/requires.txt
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)        6 2024-04-01 08:37:03.000000 aivol-0.0.6/aivol.egg-info/top_level.txt
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)      557 2024-04-01 08:35:58.000000 aivol-0.0.6/pyproject.toml
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)       38 2024-04-01 08:37:03.556056 aivol-0.0.6/setup.cfg
--rw-r--r--   0 dmitry    (1000) dmitry    (1000)       38 2024-03-14 08:16:07.000000 aivol-0.0.6/setup.py
+drwxr-xr-x   0 dmitry    (1000) dmitry    (1000)        0 2024-04-29 11:30:59.928004 aivol-0.0.7/
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)     1074 2024-03-14 07:38:11.000000 aivol-0.0.7/LICENSE
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)      474 2024-04-29 11:30:59.928004 aivol-0.0.7/PKG-INFO
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)       50 2024-03-11 08:49:25.000000 aivol-0.0.7/README.md
+drwxr-xr-x   0 dmitry    (1000) dmitry    (1000)        0 2024-04-29 11:30:59.918004 aivol-0.0.7/aivol/
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)       88 2024-03-14 08:57:27.000000 aivol-0.0.7/aivol/__init__.py
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)     4601 2024-03-26 12:58:43.000000 aivol-0.0.7/aivol/compare.py
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)     1973 2024-04-04 14:19:15.000000 aivol-0.0.7/aivol/config.py
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)     2436 2024-03-14 08:44:58.000000 aivol-0.0.7/aivol/experiment.py
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)     2825 2024-03-21 10:08:22.000000 aivol-0.0.7/aivol/resolve.py
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)     8416 2024-04-29 11:26:34.000000 aivol-0.0.7/aivol/sidecar.py
+drwxr-xr-x   0 dmitry    (1000) dmitry    (1000)        0 2024-04-29 11:30:59.928004 aivol-0.0.7/aivol.egg-info/
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)      474 2024-04-29 11:30:59.000000 aivol-0.0.7/aivol.egg-info/PKG-INFO
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)      290 2024-04-29 11:30:59.000000 aivol-0.0.7/aivol.egg-info/SOURCES.txt
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)        1 2024-04-29 11:30:59.000000 aivol-0.0.7/aivol.egg-info/dependency_links.txt
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)       24 2024-04-29 11:30:59.000000 aivol-0.0.7/aivol.egg-info/requires.txt
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)        6 2024-04-29 11:30:59.000000 aivol-0.0.7/aivol.egg-info/top_level.txt
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)      557 2024-04-29 11:29:00.000000 aivol-0.0.7/pyproject.toml
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)       38 2024-04-29 11:30:59.928004 aivol-0.0.7/setup.cfg
+-rw-r--r--   0 dmitry    (1000) dmitry    (1000)       38 2024-03-14 08:16:07.000000 aivol-0.0.7/setup.py
```

### Comparing `aivol-0.0.6/LICENSE` & `aivol-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aivol-0.0.6/aivol/compare.py` & `aivol-0.0.7/aivol/compare.py`

 * *Files identical despite different names*

### Comparing `aivol-0.0.6/aivol/config.py` & `aivol-0.0.7/aivol/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,11 +53,11 @@
                 items.extend(flatten_dict({f"{new_key}{sep}{i}": item}, sep=sep).items())
         else:
             items.append((new_key, v))
     return dict(items)
 
 def folder_to_file(fname):
     if os.path.isdir(fname):
-        files = glob.glob(fname + "/*.json") + glob.glob(fname + "/*.yml") + glob.glob(fname + "/*.pkl")
+        files = glob.glob(fname + "/*.json") + glob.glob(fname + "/*.yml") + glob.glob(fname + "/*.yaml") + glob.glob(fname + "/*.pkl")
         if files:
             fname = files[0]
-    return fname
+    return fname
```

### Comparing `aivol-0.0.6/aivol/experiment.py` & `aivol-0.0.7/aivol/experiment.py`

 * *Files identical despite different names*

### Comparing `aivol-0.0.6/aivol/resolve.py` & `aivol-0.0.7/aivol/resolve.py`

 * *Files identical despite different names*

### Comparing `aivol-0.0.6/aivol/sidecar.py` & `aivol-0.0.7/aivol/sidecar.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import glob
 import os
 from .config import universal_load, universal_store
 import sys
 import os
 from typing import Callable, Dict, Iterator
+import logging
+logging.basicConfig(level=logging.ERROR, format='%(message)s')
 
 # data format comparison for sidecar files:
 # json: the worst, because it's hard to append to it
 # yaml: ok
 # toml: ok
 # but text files are bad to store large chunks of data
 # pkl: fast, but not human-readable
@@ -100,53 +102,59 @@
 
 def load_to_pandas(directory: str, identifier: str):
     """
     Loads the data for the whole directory and returns a pandas dataframe
     """
     import pandas as pd
 
-    # Check if the given identifier is a directory
     if not os.path.isdir(directory):
-        sys.stderr.write(f"Error: The provided identifier '{identifier}' is not a directory.\n")
-        return pd.DataFrame()  # Return an empty DataFrame if the identifier is not a directory
+        sys.stderr.write(f"Error: '{directory}' is not a directory.\n")
+        return pd.DataFrame()
 
     # Use list_directory to organize files and then process sidecar files
     all_metadata = []
     non_sidecar_files, sidecar_files = list_directory(directory)
 
-    for base_file, sidecar_file_list in sidecar_files.items():
-        sidecar_handler = Handler(directory, base_file, load=False)
-        for sidecar_file in sidecar_file_list:
-            _, _, identifier = os.path.basename(sidecar_file).rpartition('---')
-            metadata = sidecar_handler.get(identifier)
-            if metadata:
-                all_metadata.append(metadata)
-            else:
-                sys.stderr.write(f"Warning: No {identifier} metadata found for '{sidecar_file}' in directory '{directory}'\n")
-
-    # Convert the list of metadata dictionaries to a pandas DataFrame
+    print ("Loading to pandas...")
+    for base_file in non_sidecar_files:
+        print (base_file, end='\r')
+        sidecar_handler = Handler(os.path.join(directory, base_file), load=False)
+        metadata = sidecar_handler.get(identifier)
+        if metadata:
+            all_metadata.append(metadata)
+        else:
+            sys.stderr.write(f"\nWarning: No {identifier} metadata found for '{base_file}'\n")
+    print ("...done")
     df = pd.DataFrame(all_metadata)
 
     return df
 
-def update_and_store_sidecar_files(directory: str, identifier: str, function: Callable[[str, Dict], Iterator[Dict]], save_interval: int = 10) -> None:
+def process_sidecar_files(directory: str, identifier: str, function: Callable[[str, str], None]) -> None:
     """
-    Unlike process_sidecar_files, it expects the function to return the updated file and stores it itself
-    Kind of wasteful (rewriting the whole file instead of appending), but it will work for most of cases
+    For each non-sidecar file calls the function(file_path, sidecar_file_path)
+    It expects the function to check whether the sidecar file exists, fully filled and so on
 
     Parameters:
-    - directory (str): The path to the directory where the non-sidecar and sidecar files are located.
-    - identifier (str): A unique identifier used to distinguish between different sidecar files.
-    - function (callable): A function that takes (source file path, current state of the sidecar file's data) and returns the updated state.
-    - save_interval (int): This parameter controls how often the updated sidecar file data is saved back to disk.
+    - directory (str): The path to the directory containing the files to process.
+    - identifier (str): The identifier used to distinguish sidecar files. Example: "identifier.json"
+    - function (callable): A function that takes two arguments (file_path, sidecar_file_path)
     """
+
     non_sidecar_files, sidecar_files = list_directory(directory)
 
-    total_files = len(non_sidecar_files)
-    for index, file in enumerate(non_sidecar_files):
+    for file in non_sidecar_files:
+        file_path = os.path.join(directory, file)
+        sidecar_file_path = os.path.join(self.directory, f"{file_path}---{identifier}")
+        function(file_path, sidecar_file_path)
+
+def update_and_store_sidecar_file(file, directory, identifier, function, save_interval, index, total_files):
+    """
+     Helper function for update_and_store_sidecar_files
+    """
+    try:
         print(f"update_and_store_sidecar_files: [{index+1}/{total_files}] {file}")
         file_path = os.path.join(directory, file)
         handler = Handler(file_path, load=False)
         initial_state = handler.get(identifier) or {}
         sidecar_file_path = f"{file_path}---{identifier}"
         updates_generator = function(file_path, initial_state)
 
@@ -154,27 +162,49 @@
         for updated_state in updates_generator:
             counter += 1
             if counter % save_interval == 0:
                 universal_store(sidecar_file_path, updated_state)
 
         if counter % save_interval != 0:
             universal_store(sidecar_file_path, updated_state)
+    except Exception as e:
+        print (e)
+        exit(-1)
 
-
-def process_sidecar_files(directory: str, identifier: str, function: Callable[[str, str], None]) -> None:
+def update_and_store_sidecar_files(directory: str, identifier: str, function: Callable[[str, Dict], Iterator[Dict]], save_interval: int = 10) -> None:
     """
-    For each non-sidecar file calls the function(file_path, sidecar_file_path)
-    It expects the function to check whether the sidecar file exists, fully filled and so on
+    Unlike process_sidecar_files, it expects the function to return the updated file and stores it itself
+    Kind of wasteful (rewriting the whole file instead of appending), but it will work for most of cases
 
     Parameters:
-    - directory (str): The path to the directory containing the files to process.
-    - identifier (str): The identifier used to distinguish sidecar files. Example: "identifier.json"
-    - function (callable): A function that takes two arguments (file_path, sidecar_file_path)
+    - directory (str): The path to the directory where the non-sidecar and sidecar files are located.
+    - identifier (str): A unique identifier used to distinguish between different sidecar files.
+    - function (callable): A function that takes (source file path, current state of the sidecar file's data) and returns the updated state.
+    - save_interval (int): This parameter controls how often the updated sidecar file data is saved back to disk.
+    """
+    non_sidecar_files, sidecar_files = list_directory(directory)
+
+    total_files = len(non_sidecar_files)
+    for index, file in enumerate(non_sidecar_files):
+        update_and_store_sidecar_file(file, directory, identifier, function, save_interval, index, total_files)
+
+def update_and_store_sidecar_files_multiprocess(directory: str,
+                                                identifier: str,
+                                                function: Callable[[str, Dict],
+                                                Iterator[Dict]],
+                                                save_interval: int = 10,
+                                                workers: int = 16) -> None:
+    """
+    Multiprocess version of update_and_store_sidecar_files
     """
 
+    import multiprocessing as mp
+    ctx = mp.get_context('spawn')
     non_sidecar_files, sidecar_files = list_directory(directory)
+    total_files = len(non_sidecar_files)
 
-    for file in non_sidecar_files:
-        file_path = os.path.join(directory, file)
-        sidecar_file_path = os.path.join(self.directory, f"{file_path}---{identifier}")
-        function(file_path, sidecar_file_path)
+    # non-multiprocess for sanity check first
+    #update_and_store_sidecar_file(non_sidecar_files.pop(), directory, identifier, function, save_interval, 0, total_files)
 
+    with ctx.Pool(workers, ) as p:
+        tasks = [(file, directory, identifier, function, save_interval, index, total_files) for index, file in enumerate(non_sidecar_files)]
+        p.starmap(update_and_store_sidecar_file, tasks, 1)
```

### Comparing `aivol-0.0.6/pyproject.toml` & `aivol-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 packages = ["aivol"]
 
 [project]
 name = "aivol"
-version = "0.0.6"
+version = "0.0.7"
 authors = [{ name = "Dmitry Galchinsky", email = "galchinsky@borisfx.com" }]
 description = "Utilities for AI volumes"
 readme = "README.md"
 license = { text = "MIT License" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

