# Comparing `tmp/effidict-0.0.3.tar.gz` & `tmp/effidict-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "effidict-0.0.3.tar", last modified: Mon Feb 19 16:04:45 2024, max compression
+gzip compressed data, was "effidict-0.0.4.tar", last modified: Mon Apr 29 08:47:48 2024, max compression
```

## Comparing `effidict-0.0.3.tar` & `effidict-0.0.4.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:04:45.267717 effidict-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:04:45.255717 effidict-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:04:45.259717 effidict-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-02-19 16:04:31.000000 effidict-0.0.3/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-19 16:04:31.000000 effidict-0.0.3/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-19 16:04:31.000000 effidict-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-19 16:04:31.000000 effidict-0.0.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-02-19 16:04:31.000000 effidict-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-19 16:04:45.267717 effidict-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-02-19 16:04:31.000000 effidict-0.0.3/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)    87532 2024-02-19 16:04:31.000000 effidict-0.0.3/comparative_notebook.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:04:45.259717 effidict-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-19 16:04:31.000000 effidict-0.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 16:04:31.000000 effidict-0.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:04:45.259717 effidict-0.0.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:04:45.259717 effidict-0.0.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    93746 2024-02-19 16:04:31.000000 effidict-0.0.3/docs/source/_static/logo_effidict.png
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-02-19 16:04:31.000000 effidict-0.0.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-19 16:04:31.000000 effidict-0.0.3/docs/source/effidict.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-02-19 16:04:31.000000 effidict-0.0.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-19 16:04:31.000000 effidict-0.0.3/docs/source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:04:45.263717 effidict-0.0.3/effidict/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-19 16:04:31.000000 effidict-0.0.3/effidict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-02-19 16:04:31.000000 effidict-0.0.3/effidict/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-19 16:04:45.000000 effidict-0.0.3/effidict/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-02-19 16:04:31.000000 effidict-0.0.3/effidict/db_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-02-19 16:04:31.000000 effidict-0.0.3/effidict/lru_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:04:45.267717 effidict-0.0.3/effidict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-19 16:04:45.000000 effidict-0.0.3/effidict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-02-19 16:04:45.000000 effidict-0.0.3/effidict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 16:04:45.000000 effidict-0.0.3/effidict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-19 16:04:45.000000 effidict-0.0.3/effidict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-19 16:04:45.000000 effidict-0.0.3/effidict.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:04:45.267717 effidict-0.0.3/images/
--rw-r--r--   0 runner    (1001) docker     (127)    59857 2024-02-19 16:04:31.000000 effidict-0.0.3/images/comparative.png
--rw-r--r--   0 runner    (1001) docker     (127)    51212 2024-02-19 16:04:31.000000 effidict-0.0.3/images/custom_100.png
--rw-r--r--   0 runner    (1001) docker     (127)    55710 2024-02-19 16:04:31.000000 effidict-0.0.3/images/custom_1000.png
--rw-r--r--   0 runner    (1001) docker     (127)    45813 2024-02-19 16:04:31.000000 effidict-0.0.3/images/custom_1000_db.png
--rw-r--r--   0 runner    (1001) docker     (127)    45280 2024-02-19 16:04:31.000000 effidict-0.0.3/images/custom_1000_db_10.png
--rw-r--r--   0 runner    (1001) docker     (127)   195221 2024-02-19 16:04:31.000000 effidict-0.0.3/images/logo_effidict.png
--rw-r--r--   0 runner    (1001) docker     (127)    93746 2024-02-19 16:04:31.000000 effidict-0.0.3/images/logo_effidict_no_bg.png
--rw-r--r--   0 runner    (1001) docker     (127)    55050 2024-02-19 16:04:31.000000 effidict-0.0.3/images/named_tuple.png
--rw-r--r--   0 runner    (1001) docker     (127)    55777 2024-02-19 16:04:31.000000 effidict-0.0.3/images/normal_dict.png
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-19 16:04:31.000000 effidict-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 16:04:45.267717 effidict-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:04:45.267717 effidict-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-19 16:04:31.000000 effidict-0.0.3/tests/test_db_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-02-19 16:04:31.000000 effidict-0.0.3/tests/test_lru_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-02-19 16:04:31.000000 effidict-0.0.3/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:47:48.669011 effidict-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:47:48.657011 effidict-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:47:48.661011 effidict-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-29 08:47:37.000000 effidict-0.0.4/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-29 08:47:37.000000 effidict-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-29 08:47:37.000000 effidict-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-29 08:47:37.000000 effidict-0.0.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-29 08:47:37.000000 effidict-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-29 08:47:48.669011 effidict-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-29 08:47:37.000000 effidict-0.0.4/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)    87532 2024-04-29 08:47:37.000000 effidict-0.0.4/comparative_notebook.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:47:48.661011 effidict-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-29 08:47:37.000000 effidict-0.0.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 08:47:37.000000 effidict-0.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:47:48.661011 effidict-0.0.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:47:48.661011 effidict-0.0.4/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    93746 2024-04-29 08:47:37.000000 effidict-0.0.4/docs/source/_static/logo_effidict.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-29 08:47:37.000000 effidict-0.0.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-29 08:47:37.000000 effidict-0.0.4/docs/source/effidict.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-29 08:47:37.000000 effidict-0.0.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-29 08:47:37.000000 effidict-0.0.4/docs/source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:47:48.661011 effidict-0.0.4/effidict/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 08:47:37.000000 effidict-0.0.4/effidict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-29 08:47:37.000000 effidict-0.0.4/effidict/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-29 08:47:48.000000 effidict-0.0.4/effidict/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-04-29 08:47:37.000000 effidict-0.0.4/effidict/db_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10116 2024-04-29 08:47:37.000000 effidict-0.0.4/effidict/lru_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:47:48.665012 effidict-0.0.4/effidict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-29 08:47:48.000000 effidict-0.0.4/effidict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-29 08:47:48.000000 effidict-0.0.4/effidict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 08:47:48.000000 effidict-0.0.4/effidict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-29 08:47:48.000000 effidict-0.0.4/effidict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 08:47:48.000000 effidict-0.0.4/effidict.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:47:48.665012 effidict-0.0.4/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    59857 2024-04-29 08:47:37.000000 effidict-0.0.4/images/comparative.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51212 2024-04-29 08:47:37.000000 effidict-0.0.4/images/custom_100.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55710 2024-04-29 08:47:37.000000 effidict-0.0.4/images/custom_1000.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45813 2024-04-29 08:47:37.000000 effidict-0.0.4/images/custom_1000_db.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45280 2024-04-29 08:47:37.000000 effidict-0.0.4/images/custom_1000_db_10.png
+-rw-r--r--   0 runner    (1001) docker     (127)   195221 2024-04-29 08:47:37.000000 effidict-0.0.4/images/logo_effidict.png
+-rw-r--r--   0 runner    (1001) docker     (127)    93746 2024-04-29 08:47:37.000000 effidict-0.0.4/images/logo_effidict_no_bg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55050 2024-04-29 08:47:37.000000 effidict-0.0.4/images/named_tuple.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55777 2024-04-29 08:47:37.000000 effidict-0.0.4/images/normal_dict.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-29 08:47:37.000000 effidict-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 08:47:48.669011 effidict-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 08:47:48.665012 effidict-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 08:47:37.000000 effidict-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-04-29 08:47:37.000000 effidict-0.0.4/tests/test_db_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-29 08:47:37.000000 effidict-0.0.4/tests/test_lru_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-29 08:47:37.000000 effidict-0.0.4/utils.py
```

### Comparing `effidict-0.0.3/.github/workflows/release.yaml` & `effidict-0.0.4/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/.readthedocs.yaml` & `effidict-0.0.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/LICENSE` & `effidict-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/PKG-INFO` & `effidict-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effidict
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fast Python package providing enhanced dictionary-like data structures with advanced caching capabilities.
 Author-email: Isra Mekki <isra.mekki@helmholtz-munich.de>, Lisa Barros de Andrade e Sousa <lisa.barros.andrade.sousa@gmail.com>, Francesco Campi <francesco.campi@helmholtz-munich.de>
 Maintainer-email: Isra Mekki <isra.mekki@helmholtz-munich.de>
 Project-URL: documentation, https://oligo-designer-toolsuite.readthedocs.io/
 Project-URL: repository, https://github.com/HelmholtzAI-Consultants-Munich/oligo-designer-toolsuite
 Keywords: data structures,efficient dictionary
 Classifier: Programming Language :: Python :: 3
```

### Comparing `effidict-0.0.3/comparative_notebook.ipynb` & `effidict-0.0.4/comparative_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/docs/Makefile` & `effidict-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/docs/source/_static/logo_effidict.png` & `effidict-0.0.4/docs/source/_static/logo_effidict.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/docs/source/conf.py` & `effidict-0.0.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/docs/source/index.rst` & `effidict-0.0.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/effidict/db_dict.py` & `effidict-0.0.4/effidict/db_dict.py`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/effidict/lru_dict.py` & `effidict-0.0.4/effidict/lru_dict.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import inspect
 import json
 import os
 import pickle
+import shutil
 import sqlite3
+import warnings
 
 from ._base import EffiDictBase
 
 
 class LRUDict(EffiDictBase):
     """
     A class implementing a Least Recently Used (LRU) cache.
@@ -30,16 +33,15 @@
         :param max_in_memory: The maximum number of items to keep in memory.
         :type max_in_memory: int
         :param storage_path: The path to the directory where items will be stored on disk.
         :type storage_path: str
 
         """
         super().__init__(max_in_memory, storage_path)
-        if not os.path.exists(storage_path):
-            os.makedirs(storage_path)
+        os.makedirs(self.storage_path)
 
     def _serialize(self, key, value):
         """
         Serialize and store the value associated with the key to the disk.
 
         This method is used to store items that are evicted from the memory cache.
 
@@ -137,14 +139,28 @@
         This method is used to populate the cache with items from a dictionary.
 
         :param dictionary: A dictionary containing items to load into the cache.
         """
         for key, value in dictionary.items():
             self[key] = value
 
+    def destroy(self):
+        """
+        Destroy the cache and remove all serialized files on disk.
+        """
+        # Problem with joblib: don't delete the storage_path if called by joblib
+        called_by_joblib = any(
+            record.function == "_process_worker" for record in inspect.stack()
+        )
+
+        if not called_by_joblib:
+            shutil.rmtree(self.storage_path)
+
+        del self.memory
+
 
 class LRUDBDict(EffiDictBase):
     """
     A class implementing a Least Recently Used (LRU) cache with a SQLite backend.
 
     This class manages a cache that stores a limited number of items in memory and
     the rest in a SQLite database. It extends the functionality of EffiDictBase by
@@ -152,17 +168,17 @@
 
     :param max_in_memory: The maximum number of items to keep in memory.
     :type max_in_memory: int
     :param storage_path: The file path to the SQLite database.
     :type storage_path: str
     """
 
-    def __init__(self, max_in_memory=100, storage_path="cache.db"):
+    def __init__(self, max_in_memory=100, storage_path="cache"):
         super().__init__(max_in_memory, storage_path)
-        self.conn = sqlite3.connect(storage_path)
+        self.conn = sqlite3.connect(self.storage_path + ".db")
         self.cursor = self.conn.cursor()
         self.cursor.execute(
             "CREATE TABLE IF NOT EXISTS data (key TEXT PRIMARY KEY, value TEXT)"
         )
 
     def _serialize(self, key, value):
         """
@@ -261,7 +277,15 @@
             items_to_insert = [
                 (key, json.dumps(value)) for key, value in dictionary.items()
             ]
             self.cursor.executemany(
                 "REPLACE INTO data (key, value) VALUES (?, ?)",
                 items_to_insert,
             )
+
+    def destroy(self):
+        """
+        Destroy the cache and remove the SQLite database file.
+        """
+        del self.memory
+        self.conn.close()
+        os.remove(self.storage_path + ".db")
```

### Comparing `effidict-0.0.3/effidict.egg-info/PKG-INFO` & `effidict-0.0.4/effidict.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: effidict
-Version: 0.0.3
+Version: 0.0.4
 Summary: Fast Python package providing enhanced dictionary-like data structures with advanced caching capabilities.
 Author-email: Isra Mekki <isra.mekki@helmholtz-munich.de>, Lisa Barros de Andrade e Sousa <lisa.barros.andrade.sousa@gmail.com>, Francesco Campi <francesco.campi@helmholtz-munich.de>
 Maintainer-email: Isra Mekki <isra.mekki@helmholtz-munich.de>
 Project-URL: documentation, https://oligo-designer-toolsuite.readthedocs.io/
 Project-URL: repository, https://github.com/HelmholtzAI-Consultants-Munich/oligo-designer-toolsuite
 Keywords: data structures,efficient dictionary
 Classifier: Programming Language :: Python :: 3
```

### Comparing `effidict-0.0.3/effidict.egg-info/SOURCES.txt` & `effidict-0.0.4/effidict.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -29,9 +29,10 @@
 images/custom_1000.png
 images/custom_1000_db.png
 images/custom_1000_db_10.png
 images/logo_effidict.png
 images/logo_effidict_no_bg.png
 images/named_tuple.png
 images/normal_dict.png
+tests/__init__.py
 tests/test_db_dict.py
 tests/test_lru_dict.py
```

### Comparing `effidict-0.0.3/images/comparative.png` & `effidict-0.0.4/images/comparative.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/images/custom_100.png` & `effidict-0.0.4/images/custom_100.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/images/custom_1000.png` & `effidict-0.0.4/images/custom_1000.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/images/custom_1000_db.png` & `effidict-0.0.4/images/custom_1000_db.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/images/custom_1000_db_10.png` & `effidict-0.0.4/images/custom_1000_db_10.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/images/logo_effidict.png` & `effidict-0.0.4/images/logo_effidict.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/images/logo_effidict_no_bg.png` & `effidict-0.0.4/images/logo_effidict_no_bg.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/images/named_tuple.png` & `effidict-0.0.4/images/named_tuple.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/images/normal_dict.png` & `effidict-0.0.4/images/normal_dict.png`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/pyproject.toml` & `effidict-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/tests/test_db_dict.py` & `effidict-0.0.4/tests/test_db_dict.py`

 * *Files identical despite different names*

### Comparing `effidict-0.0.3/tests/test_lru_dict.py` & `effidict-0.0.4/tests/test_lru_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import os
-import shutil
 
 import pytest
 
 from effidict import LRUDBDict, LRUDict
 
 
 @pytest.fixture
 def lru_dict(tmp_path):
     """Fixture to create an LRUDict instance and clean up after tests."""
     cache = LRUDict(max_in_memory=2, storage_path=str(tmp_path / "lrudict_cache"))
     yield cache
-    shutil.rmtree(str(tmp_path / "lrudict_cache"), ignore_errors=True)
 
 
 def test_lrudict_set_and_get_item(lru_dict):
     lru_dict["key1"] = "value1"
     assert lru_dict["key1"] == "value1", "Value should be value1"
 
 
@@ -74,15 +72,14 @@
 @pytest.fixture
 def lrudb_dict(tmp_path):
     """Fixture to create an LRUDBDict instance and clean up after tests."""
     db_path = str(tmp_path / "lrudbdict_cache.db")
     cache = LRUDBDict(max_in_memory=2, storage_path=db_path)
     yield cache
     cache.conn.close()
-    os.remove(db_path)
 
 
 def test_lrudbdict_initialization(lrudb_dict):
     assert lrudb_dict.max_in_memory == 2
     # Ensure the SQLite table exists
     lrudb_dict.cursor.execute(
         "SELECT name FROM sqlite_master WHERE type='table' AND name='data';"
```

### Comparing `effidict-0.0.3/utils.py` & `effidict-0.0.4/utils.py`

 * *Files identical despite different names*

