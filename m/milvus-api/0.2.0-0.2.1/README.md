# Comparing `tmp/milvus_api-0.2.0.tar.gz` & `tmp/milvus_api-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "milvus_api-0.2.0.tar", last modified: Sat Apr 27 08:06:55 2024, max compression
+gzip compressed data, was "milvus_api-0.2.1.tar", last modified: Mon Apr 29 04:37:51 2024, max compression
```

## Comparing `milvus_api-0.2.0.tar` & `milvus_api-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 08:06:55.830603 milvus_api-0.2.0/
--rw-rw-rw-   0        0        0     3203 2024-04-27 08:06:55.814584 milvus_api-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2744 2024-04-27 08:05:46.000000 milvus_api-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 08:06:55.782937 milvus_api-0.2.0/milvus_api/
--rw-rw-rw-   0        0        0        0 2024-04-25 15:55:58.000000 milvus_api-0.2.0/milvus_api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-27 08:06:55.814584 milvus_api-0.2.0/milvus_api/db_model/
--rw-rw-rw-   0        0        0        0 2024-04-25 13:02:02.000000 milvus_api-0.2.0/milvus_api/db_model/__init__.py
--rw-rw-rw-   0        0        0     7450 2024-04-27 07:57:47.000000 milvus_api-0.2.0/milvus_api/db_model/milvus_db.py
-drwxrwxrwx   0        0        0        0 2024-04-27 08:06:55.814584 milvus_api-0.2.0/milvus_api/embed_model/
--rw-rw-rw-   0        0        0        0 2024-04-25 15:06:57.000000 milvus_api-0.2.0/milvus_api/embed_model/__init__.py
--rw-rw-rw-   0        0        0     1257 2024-04-25 15:29:44.000000 milvus_api-0.2.0/milvus_api/embed_model/bgem3.py
-drwxrwxrwx   0        0        0        0 2024-04-27 08:06:55.810077 milvus_api-0.2.0/milvus_api.egg-info/
--rw-rw-rw-   0        0        0     3203 2024-04-27 08:06:55.000000 milvus_api-0.2.0/milvus_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-04-27 08:06:55.000000 milvus_api-0.2.0/milvus_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 08:06:55.000000 milvus_api-0.2.0/milvus_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      113 2024-04-27 08:06:55.000000 milvus_api-0.2.0/milvus_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-27 08:06:55.000000 milvus_api-0.2.0/milvus_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 08:06:55.830603 milvus_api-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      616 2024-04-27 08:06:39.000000 milvus_api-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:37:51.605375 milvus_api-0.2.1/
+-rw-rw-rw-   0        0        0     3419 2024-04-29 04:37:51.605375 milvus_api-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2960 2024-04-29 04:35:56.000000 milvus_api-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 04:37:51.558611 milvus_api-0.2.1/milvus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-25 15:55:58.000000 milvus_api-0.2.1/milvus_api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:37:51.589749 milvus_api-0.2.1/milvus_api/db_model/
+-rw-rw-rw-   0        0        0        0 2024-04-25 13:02:02.000000 milvus_api-0.2.1/milvus_api/db_model/__init__.py
+-rw-rw-rw-   0        0        0     7790 2024-04-29 02:54:35.000000 milvus_api-0.2.1/milvus_api/db_model/milvus_db.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:37:51.605375 milvus_api-0.2.1/milvus_api/embed_model/
+-rw-rw-rw-   0        0        0        0 2024-04-25 15:06:57.000000 milvus_api-0.2.1/milvus_api/embed_model/__init__.py
+-rw-rw-rw-   0        0        0     1257 2024-04-25 15:29:44.000000 milvus_api-0.2.1/milvus_api/embed_model/bgem3.py
+drwxrwxrwx   0        0        0        0 2024-04-29 04:37:51.589749 milvus_api-0.2.1/milvus_api.egg-info/
+-rw-rw-rw-   0        0        0     3419 2024-04-29 04:37:51.000000 milvus_api-0.2.1/milvus_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-04-29 04:37:51.000000 milvus_api-0.2.1/milvus_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 04:37:51.000000 milvus_api-0.2.1/milvus_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      113 2024-04-29 04:37:51.000000 milvus_api-0.2.1/milvus_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-29 04:37:51.000000 milvus_api-0.2.1/milvus_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-29 04:37:51.605375 milvus_api-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      634 2024-04-29 04:37:48.000000 milvus_api-0.2.1/setup.py
```

### Comparing `milvus_api-0.2.0/PKG-INFO` & `milvus_api-0.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: milvus_api
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Milvus API used for quickly setting up a Milvus vector database
 Author: ShengWen
 Author-email: shengwen8785@example.com
 Description-Content-Type: text/markdown
 Requires-Dist: pymilvus==2.4.0
 Requires-Dist: milvus-model==0.2.0
 Requires-Dist: pydantic==2.7.0
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: FlagEmbedding==1.2.9
 Requires-Dist: torch==2.2.2
 Requires-Dist: numpy==1.24.4
 
-# milvus_api
+<div align="center">
+    <img src="figures/milvus_logo_with_a_steampunk_and_industrial_style.jpg" alt="描述文字">
+</div>
 
-`milvus_api` is a Python library that primarily provides functionalities to manage databases, including creating collections, inserting data, and searching.
+# milvus_api
+`milvus_api` is a Python library that primarily provides functionalities to manage databases, including creating collections, inserting data, searching and updating index.
 
 ## Installation
-
 This project depends on several Python libraries. Use the following command to install the necessary libraries:
 
 ```bash
 pip install pymilvus==2.4.0 milvus-model==0.2.0 pydantic==2.7.0 tqdm==4.66.2 FlagEmbedding==1.2.9 torch==2.2.2 numpy==1.24.4
 ```
 
 ## Usage Examples
@@ -55,14 +57,15 @@
 model_name = 'bgem3_model'
 
 # Initialize the model
 bgem3 = PyMilvusBGEM3(model_name)
 results = bgem3.encode(query)
 ```
 ## Release Note
+- 0.2.1:(Feat): support **IVF_PQ** indexing algorithm for `switch_index`.
 - 0.2.0:(Feat): add the `switch_index` operation to `MilvusDB` object.
 ```
 from milvus_api.db_model.milvus_db import MilvusDB
 
 db = MilvusDB(host, port)
 
 # Assume you already have a collection with index.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `milvus_api-0.2.0/README.md` & `milvus_api-0.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-# milvus_api
+<div align="center">
+    <img src="figures/milvus_logo_with_a_steampunk_and_industrial_style.jpg" alt="描述文字">
+</div>
 
-`milvus_api` is a Python library that primarily provides functionalities to manage databases, including creating collections, inserting data, and searching.
+# milvus_api
+`milvus_api` is a Python library that primarily provides functionalities to manage databases, including creating collections, inserting data, searching and updating index.
 
 ## Installation
-
 This project depends on several Python libraries. Use the following command to install the necessary libraries:
 
 ```bash
 pip install pymilvus==2.4.0 milvus-model==0.2.0 pydantic==2.7.0 tqdm==4.66.2 FlagEmbedding==1.2.9 torch==2.2.2 numpy==1.24.4
 ```
 
 ## Usage Examples
@@ -40,14 +42,15 @@
 model_name = 'bgem3_model'
 
 # Initialize the model
 bgem3 = PyMilvusBGEM3(model_name)
 results = bgem3.encode(query)
 ```
 ## Release Note
+- 0.2.1:(Feat): support **IVF_PQ** indexing algorithm for `switch_index`.
 - 0.2.0:(Feat): add the `switch_index` operation to `MilvusDB` object.
 ```
 from milvus_api.db_model.milvus_db import MilvusDB
 
 db = MilvusDB(host, port)
 
 # Assume you already have a collection with index.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `milvus_api-0.2.0/milvus_api/db_model/milvus_db.py` & `milvus_api-0.2.1/milvus_api/db_model/milvus_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,25 +50,29 @@
 
     @staticmethod
     def switch_index(
             collection_name: str,
             drop_index_name: str,
             new_index_type: str,
             field_name: str = "embeddings",
-            metric_type: str = "COSINE"
+            metric_type: str = "COSINE",
+            m: int = 1,
+            nbits: int = 8
     ) -> None:
         """
         Replace the index of specific field.
 
         Args:
-            collection_name: the name of the collection.
-            drop_index_name: the index name that you want to drop.
-            new_index_type: the new indexing algorithm that you want to use.
-            field_name: the specific filed that you attempt to build an index.
+            collection_name: the name of the collection
+            drop_index_name: the index name that you want to drop
+            new_index_type: the new indexing algorithm that you want to use
+            field_name: the specific filed that you attempt to build an index
             metric_type: to measure the metric of distance between vectors. ref: https://milvus.io/docs/v2.3.x/metric.md
+            m: the number of factors of product quantization, default value 1 (no quantization)
+            nbits: the number of bits in which each low-dimensional vector is stored, default value 8
         """
         if utility.has_collection(collection_name):  # True if collection exists, false if it does not.
             collection = Collection(collection_name)
             # The collection must be released before dropping index.
             if str(utility.load_state(collection_name)) == "Loaded":
                 collection.release()
         else:
@@ -78,15 +82,19 @@
         collection.drop_index(index_name=drop_index_name)
 
         # Build a new index.
         nlist = 4 * (collection.num_entities ** 0.5)
         index = {
             "index_type": new_index_type,
             "metric_type": metric_type,
-            "params": {"nlist": nlist}
+            "params": {
+                "nlist": nlist,
+                "m": m,
+                "nbits": nbits
+            }
         }
         collection.create_index(field_name=field_name, index_params=index)
         collection.load()
 
         time.sleep(10)
 
     def create_collection(
```

### Comparing `milvus_api-0.2.0/milvus_api/embed_model/bgem3.py` & `milvus_api-0.2.1/milvus_api/embed_model/bgem3.py`

 * *Files identical despite different names*

### Comparing `milvus_api-0.2.0/milvus_api.egg-info/PKG-INFO` & `milvus_api-0.2.1/milvus_api.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: milvus-api
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Milvus API used for quickly setting up a Milvus vector database
 Author: ShengWen
 Author-email: shengwen8785@example.com
 Description-Content-Type: text/markdown
 Requires-Dist: pymilvus==2.4.0
 Requires-Dist: milvus-model==0.2.0
 Requires-Dist: pydantic==2.7.0
 Requires-Dist: tqdm==4.66.2
 Requires-Dist: FlagEmbedding==1.2.9
 Requires-Dist: torch==2.2.2
 Requires-Dist: numpy==1.24.4
 
-# milvus_api
+<div align="center">
+    <img src="figures/milvus_logo_with_a_steampunk_and_industrial_style.jpg" alt="描述文字">
+</div>
 
-`milvus_api` is a Python library that primarily provides functionalities to manage databases, including creating collections, inserting data, and searching.
+# milvus_api
+`milvus_api` is a Python library that primarily provides functionalities to manage databases, including creating collections, inserting data, searching and updating index.
 
 ## Installation
-
 This project depends on several Python libraries. Use the following command to install the necessary libraries:
 
 ```bash
 pip install pymilvus==2.4.0 milvus-model==0.2.0 pydantic==2.7.0 tqdm==4.66.2 FlagEmbedding==1.2.9 torch==2.2.2 numpy==1.24.4
 ```
 
 ## Usage Examples
@@ -55,14 +57,15 @@
 model_name = 'bgem3_model'
 
 # Initialize the model
 bgem3 = PyMilvusBGEM3(model_name)
 results = bgem3.encode(query)
 ```
 ## Release Note
+- 0.2.1:(Feat): support **IVF_PQ** indexing algorithm for `switch_index`.
 - 0.2.0:(Feat): add the `switch_index` operation to `MilvusDB` object.
 ```
 from milvus_api.db_model.milvus_db import MilvusDB
 
 db = MilvusDB(host, port)
 
 # Assume you already have a collection with index.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `milvus_api-0.2.0/setup.py` & `milvus_api-0.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='milvus_api',
-    version='0.2.0',
+    version='0.2.1',
     packages=find_packages(),
     install_requires=[
         "pymilvus==2.4.0",
         "milvus-model==0.2.0",
         "pydantic==2.7.0",
         "tqdm==4.66.2",
         "FlagEmbedding==1.2.9",
         "torch==2.2.2",
         "numpy==1.24.4"
     ],
     author='ShengWen',
     author_email='shengwen8785@example.com',
     description='A Milvus API used for quickly setting up a Milvus vector database',
-    long_description=open('README.md').read(),
+    long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown'
 )
```

