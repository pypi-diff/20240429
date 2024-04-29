# Comparing `tmp/vlite-0.2.4.tar.gz` & `tmp/vlite-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlite-0.2.4.tar", last modified: Thu Apr 25 21:55:05 2024, max compression
+gzip compressed data, was "vlite-0.2.5.tar", last modified: Mon Apr 29 03:18:43 2024, max compression
```

## Comparing `vlite-0.2.4.tar` & `vlite-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-25 21:55:05.149555 vlite-0.2.4/
--rw-r--r--   0 sdan       (501) staff       (20)    34523 2024-03-27 04:16:34.000000 vlite-0.2.4/LICENSE
--rw-r--r--   0 sdan       (501) staff       (20)      595 2024-04-25 21:55:05.149421 vlite-0.2.4/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)     3247 2024-04-18 04:36:43.000000 vlite-0.2.4/README.md
--rw-r--r--   0 sdan       (501) staff       (20)       38 2024-04-25 21:55:05.149621 vlite-0.2.4/setup.cfg
--rw-r--r--   0 sdan       (501) staff       (20)     1043 2024-04-25 21:54:19.000000 vlite-0.2.4/setup.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-25 21:55:05.146670 vlite-0.2.4/tests/
--rw-r--r--   0 sdan       (501) staff       (20)     6320 2024-04-03 19:37:27.000000 vlite-0.2.4/tests/test_server.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-25 21:55:05.148598 vlite-0.2.4/vlite/
--rw-r--r--   0 sdan       (501) staff       (20)       57 2024-04-17 20:14:36.000000 vlite-0.2.4/vlite/__init__.py
--rw-r--r--   0 sdan       (501) staff       (20)     6744 2024-04-17 09:21:55.000000 vlite-0.2.4/vlite/ctx.py
--rw-r--r--   0 sdan       (501) staff       (20)     1313 2024-04-17 09:02:04.000000 vlite-0.2.4/vlite/index.py
--rw-r--r--   0 sdan       (501) staff       (20)    13387 2024-04-18 04:37:17.000000 vlite-0.2.4/vlite/main.py
--rw-r--r--   0 sdan       (501) staff       (20)     4484 2024-04-17 09:30:24.000000 vlite-0.2.4/vlite/model.py
--rw-r--r--   0 sdan       (501) staff       (20)     7781 2024-04-17 20:14:19.000000 vlite-0.2.4/vlite/server.py
--rw-r--r--   0 sdan       (501) staff       (20)     7980 2024-04-14 22:49:23.000000 vlite-0.2.4/vlite/utils.py
-drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-25 21:55:05.149261 vlite-0.2.4/vlite.egg-info/
--rw-r--r--   0 sdan       (501) staff       (20)      595 2024-04-25 21:55:05.000000 vlite-0.2.4/vlite.egg-info/PKG-INFO
--rw-r--r--   0 sdan       (501) staff       (20)      297 2024-04-25 21:55:05.000000 vlite-0.2.4/vlite.egg-info/SOURCES.txt
--rw-r--r--   0 sdan       (501) staff       (20)        1 2024-04-25 21:55:05.000000 vlite-0.2.4/vlite.egg-info/dependency_links.txt
--rw-r--r--   0 sdan       (501) staff       (20)      154 2024-04-25 21:55:05.000000 vlite-0.2.4/vlite.egg-info/requires.txt
--rw-r--r--   0 sdan       (501) staff       (20)        6 2024-04-25 21:55:05.000000 vlite-0.2.4/vlite.egg-info/top_level.txt
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-29 03:18:43.088370 vlite-0.2.5/
+-rw-r--r--   0 sdan       (501) staff       (20)    34523 2024-03-27 04:16:34.000000 vlite-0.2.5/LICENSE
+-rw-r--r--   0 sdan       (501) staff       (20)      595 2024-04-29 03:18:43.088235 vlite-0.2.5/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)     3247 2024-04-18 04:36:43.000000 vlite-0.2.5/README.md
+-rw-r--r--   0 sdan       (501) staff       (20)       38 2024-04-29 03:18:43.088411 vlite-0.2.5/setup.cfg
+-rw-r--r--   0 sdan       (501) staff       (20)     1043 2024-04-29 03:18:23.000000 vlite-0.2.5/setup.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-29 03:18:43.085956 vlite-0.2.5/tests/
+-rw-r--r--   0 sdan       (501) staff       (20)     6320 2024-04-03 19:37:27.000000 vlite-0.2.5/tests/test_server.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-29 03:18:43.087375 vlite-0.2.5/vlite/
+-rw-r--r--   0 sdan       (501) staff       (20)       57 2024-04-17 20:14:36.000000 vlite-0.2.5/vlite/__init__.py
+-rw-r--r--   0 sdan       (501) staff       (20)     6744 2024-04-17 09:21:55.000000 vlite-0.2.5/vlite/ctx.py
+-rw-r--r--   0 sdan       (501) staff       (20)     1331 2024-04-26 00:57:11.000000 vlite-0.2.5/vlite/index.py
+-rw-r--r--   0 sdan       (501) staff       (20)    13527 2024-04-29 03:14:09.000000 vlite-0.2.5/vlite/main.py
+-rw-r--r--   0 sdan       (501) staff       (20)     4484 2024-04-17 09:30:24.000000 vlite-0.2.5/vlite/model.py
+-rw-r--r--   0 sdan       (501) staff       (20)     7781 2024-04-17 20:14:19.000000 vlite-0.2.5/vlite/server.py
+-rw-r--r--   0 sdan       (501) staff       (20)     7980 2024-04-14 22:49:23.000000 vlite-0.2.5/vlite/utils.py
+drwxr-xr-x   0 sdan       (501) staff       (20)        0 2024-04-29 03:18:43.088033 vlite-0.2.5/vlite.egg-info/
+-rw-r--r--   0 sdan       (501) staff       (20)      595 2024-04-29 03:18:43.000000 vlite-0.2.5/vlite.egg-info/PKG-INFO
+-rw-r--r--   0 sdan       (501) staff       (20)      297 2024-04-29 03:18:43.000000 vlite-0.2.5/vlite.egg-info/SOURCES.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        1 2024-04-29 03:18:43.000000 vlite-0.2.5/vlite.egg-info/dependency_links.txt
+-rw-r--r--   0 sdan       (501) staff       (20)      154 2024-04-29 03:18:43.000000 vlite-0.2.5/vlite.egg-info/requires.txt
+-rw-r--r--   0 sdan       (501) staff       (20)        6 2024-04-29 03:18:43.000000 vlite-0.2.5/vlite.egg-info/top_level.txt
```

### Comparing `vlite-0.2.4/LICENSE` & `vlite-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vlite-0.2.4/PKG-INFO` & `vlite-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlite
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple and blazing fast vector database
 Author: Surya Dantuluri
 Author-email: surya@suryad.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

### Comparing `vlite-0.2.4/README.md` & `vlite-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `vlite-0.2.4/setup.py` & `vlite-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-__version__ = '0.2.4'
+__version__ = '0.2.5'
 
 setup(
     name='vlite',
     version=__version__,
     author='Surya Dantuluri',
     author_email='surya@suryad.com',
     description='A simple and blazing fast vector database',
```

### Comparing `vlite-0.2.4/tests/test_server.py` & `vlite-0.2.5/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `vlite-0.2.4/vlite/ctx.py` & `vlite-0.2.5/vlite/ctx.py`

 * *Files identical despite different names*

### Comparing `vlite-0.2.4/vlite/index.py` & `vlite-0.2.5/vlite/index.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 import struct
 import json
 from enum import Enum
 from typing import List, Union, Dict
 
+# not implemented
 class BinaryVectorIndex:
     def __init__(self, embedding_size=64):
         self.index = {}
         self.embedding_size = embedding_size
         
     def add(self, chunk_id, binary_vector):
         binary_vector = binary_vector.tolist()
```

### Comparing `vlite-0.2.4/vlite/main.py` & `vlite-0.2.5/vlite/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 from .utils import chop_and_chunk
 import datetime
 from .ctx import Ctx
 import time
 import logging
 
 # Configure logging
-logging.basicConfig(level=logging.WARNING, format='%(asctime)s - %(levelname)s - %(message)s')
+logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
 
 
 class VLite:
     def __init__(self, collection=None, device=None, model_name='mixedbread-ai/mxbai-embed-large-v1'):
         start_time = time.time()
         if device is None:
             if check_cuda_available():
                 device = 'cuda'
             elif check_mps_available():
                 device = 'mps'
             else:
                 device = 'cpu'
-        logger.info(f"[VLite.__init__] Initializing VLite with device: {device}")
+        print(f"[VLite.__init__] Initializing VLite with device: {device}")
         self.device = device
         if collection is None:
             current_datetime = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
             collection = f"vlite_{current_datetime}"
         self.collection = f"{collection}"
         self.model = EmbeddingModel(model_name, device=device) if model_name else EmbeddingModel()
         self.ctx = Ctx()
@@ -44,16 +44,16 @@
                 }
                 for idx, chunk_id in enumerate(ctx_file.metadata.keys())
             }
         except FileNotFoundError:
             logger.warning(f"[VLite.__init__] Collection file {self.collection} not found. Initializing empty attributes.")
 
         end_time = time.time()
-        logger.debug(f"[VLite.__init__] Execution time: {end_time - start_time:.5f} seconds")
-        logger.info(f"[VLite.__init__] Using device: {self.device}")
+        print(f"[VLite.__init__] Execution time: {end_time - start_time:.5f} seconds")
+        print(f"[VLite.__init__] Using device: {self.device}")
 
     def add(self, data, metadata=None, item_id=None, need_chunks=False, fast=True):
         start_time = time.time()
         data = [data] if not isinstance(data, list) else data
         results = []
         all_chunks = []
         all_metadata = []
@@ -68,15 +68,15 @@
             if item_id is None:
                 item_id = str(uuid4())
             item_metadata.update(metadata or {})
             if need_chunks:
                 chunks = chop_and_chunk(text_content, fast=fast)
             else:
                 chunks = [text_content]
-            logger.debug("[VLite.add] Encoding text... not chunking")
+            print("[VLite.add] Encoding text... not chunking")
             all_chunks.extend(chunks)
             all_metadata.extend([item_metadata] * len(chunks))
             all_ids.extend([item_id] * len(chunks))
         binary_encoded_data = self.model.embed(all_chunks, precision="binary")
 
 
         for idx, (chunk, binary_vector, metadata) in enumerate(zip(all_chunks, binary_encoded_data, all_metadata)):
@@ -86,92 +86,99 @@
                 'metadata': metadata,
                 'binary_vector': binary_vector.tolist()
             }
 
         if item_id not in [result[0] for result in results]:
             results.append((item_id, binary_encoded_data, metadata))
 
-        self.save()
-        logger.info("[VLite.add] Text added successfully.")
+        # self.save()
+        # print("[VLite.add] Text added successfully.")
         end_time = time.time()
-        logger.debug(f"[VLite.add] Execution time: {end_time - start_time:.5f} seconds")
+        print(f"[VLite.add] Execution time: {end_time - start_time:.5f} seconds")
         return results
 
         
 
-    def retrieve(self, text=None, top_k=5, metadata=None, return_scores=False):
+    def retrieve(self, text=None, top_k=5, metadata=None, return_scores=False, top_k_multiplier=4):
         start_time = time.time()
-        logger.info("[VLite.retrieve] Retrieving similar texts...")
+        print("[VLite.retrieve] Retrieving similar texts...")
         if text:
-            logger.info(f"[VLite.retrieve] Retrieving top {top_k} similar texts for query: {text}")
+            print(f"[VLite.retrieve] Retrieving top {top_k} similar texts for query: {text}")
             query_binary_vectors = self.model.embed(text, precision="binary")
             # Perform search on the query binary vectors
             results = []
             for query_binary_vector in query_binary_vectors:
-                chunk_results = self.rank_and_filter(query_binary_vector, top_k, metadata)
+                chunk_results = self.rank_and_filter(query_binary_vector, top_k, metadata, top_k_multiplier)
                 results.extend(chunk_results)
             # Sort the results by similarity score
             results.sort(key=lambda x: x[1])
             results = results[:top_k]
-            logger.info("[VLite.retrieve] Retrieval completed.")
+            print("[VLite.retrieve] Retrieval completed.")
             end_time = time.time()
-            logger.debug(f"[VLite.retrieve] Execution time: {end_time - start_time:.5f} seconds")
+            print(f"[VLite.retrieve] Execution time: {end_time - start_time:.5f} seconds")
             if return_scores:
                 return [(idx, self.index[idx]['text'], self.index[idx]['metadata'], score) for idx, score in results]
             else:
                 return [(idx, self.index[idx]['text'], self.index[idx]['metadata']) for idx, _ in results]
 
-    def rank_and_filter(self, query_binary_vector, top_k, metadata=None):
+    def rank_and_filter(self, query_binary_vector, top_k, metadata=None, top_k_multiplier=4):
         start_time = time.time()
-        logger.debug(f"[VLite.rank_and_filter] Shape of query vector: {query_binary_vector.shape}")
+        
+        # If metadata filter is provided, retrieve more items initially
+        if metadata:
+            initial_top_k = top_k * top_k_multiplier  # Adjust this factor as needed
+        else:
+            initial_top_k = top_k
+        
+        print(f"[VLite.rank_and_filter] Shape of query vector: {query_binary_vector.shape}")
         query_binary_vector = np.array(query_binary_vector).reshape(-1)
-        logger.debug(f"[VLite.rank_and_filter] Shape of query vector after reshaping: {query_binary_vector.shape}")
+        print(f"[VLite.rank_and_filter] Shape of query vector after reshaping: {query_binary_vector.shape}")
         # Collect all binary vectors and ensure they all have the same shape as the query vector
         binary_vectors = [item['binary_vector'] for item in self.index.values() if len(item['binary_vector']) == len(query_binary_vector)]        
         binary_vector_indices = [idx for idx, item in enumerate(self.index.values()) if len(item['binary_vector']) == len(query_binary_vector)]
         if binary_vectors:
             corpus_binary_vectors = np.asarray(binary_vectors, dtype=np.float32)
-            logger.debug(f"[VLite.rank_and_filter] Shape of corpus binary vectors array: {corpus_binary_vectors.shape}")
+            print(f"[VLite.rank_and_filter] Shape of corpus binary vectors array: {corpus_binary_vectors.shape}")
         else:
             raise ValueError("No valid binary vectors found for comparison.")
-        top_k_indices, top_k_scores = self.model.search(query_binary_vector, corpus_binary_vectors, top_k)
-        logger.debug(f"[VLite.rank_and_filter] Top {top_k} indices: {top_k_indices}")
-        logger.debug(f"[VLite.rank_and_filter] Top {top_k} scores: {top_k_scores}")
-        logger.debug(f"[VLite.rank_and_filter] No. of items in the collection: {len(self.index)}")
-        logger.debug(f"[VLite.rank_and_filter] Vlite count: {self.count()}")
+        top_k_indices, top_k_scores = self.model.search(query_binary_vector, corpus_binary_vectors, initial_top_k)
+        print(f"[VLite.rank_and_filter] Top {initial_top_k} indices: {top_k_indices}")
+        print(f"[VLite.rank_and_filter] Top {initial_top_k} scores: {top_k_scores}")
+        print(f"[VLite.rank_and_filter] No. of items in the collection: {len(self.index)}")
+        print(f"[VLite.rank_and_filter] Vlite count: {self.count()}")
 
         top_k_ids = [list(self.index.keys())[binary_vector_indices[idx]] for idx in top_k_indices]
         # Apply metadata filter on the retrieved top_k items
         filtered_ids = []
         if metadata:
             for chunk_id in top_k_ids:
                 item_metadata = self.index[chunk_id]['metadata']
                 if all(item_metadata.get(key) == value for key, value in metadata.items()):
                     filtered_ids.append(chunk_id)
             top_k_ids = filtered_ids[:top_k]
             top_k_scores = top_k_scores[:len(top_k_ids)]
         end_time = time.time()
-        logger.debug(f"[VLite.rank_and_filter] Execution time: {end_time - start_time:.5f} seconds")
+        print(f"[VLite.rank_and_filter] Execution time: {end_time - start_time:.5f} seconds")
         return list(zip(top_k_ids, top_k_scores))
 
     def update(self, id, text=None, metadata=None, vector=None):
         start_time = time.time()
         chunk_ids = [chunk_id for chunk_id in self.index if chunk_id.startswith(f"{id}_")]
         if chunk_ids:
             for chunk_id in chunk_ids:
                 if text is not None:
                     self.index[chunk_id]['text'] = text
                 if metadata is not None:
                     self.index[chunk_id]['metadata'].update(metadata)
                 if vector is not None:
                     self.index[chunk_id]['vector'] = vector
             self.save()
-            logger.info(f"[VLite.update] Item with ID '{id}' updated successfully.")
+            print(f"[VLite.update] Item with ID '{id}' updated successfully.")
             end_time = time.time()
-            logger.debug(f"[VLite.update] Execution time: {end_time - start_time:.5f} seconds")
+            print(f"[VLite.update] Execution time: {end_time - start_time:.5f} seconds")
             return True
         else:
             logger.warning(f"[VLite.update] Item with ID '{id}' not found.")
             return False
 
     def delete(self, ids):
         if isinstance(ids, str):
@@ -181,15 +188,15 @@
             chunk_ids = [chunk_id for chunk_id in self.index if chunk_id.startswith(f"{id}_")]
             for chunk_id in chunk_ids:
                 if chunk_id in self.index:
                     del self.index[chunk_id]
                     deleted_count += 1
         if deleted_count > 0:
             self.save()
-            logger.info(f"[VLite.delete] Deleted {deleted_count} item(s) from the collection.")
+            print(f"[VLite.delete] Deleted {deleted_count} item(s) from the collection.")
         else:
             logger.warning("[VLite.delete] No items found with the specified IDs.")
         return deleted_count
 
     def get(self, ids=None, where=None):
         if ids is not None:
             if isinstance(ids, str):
@@ -213,21 +220,21 @@
                 item_metadata = chunk_data['metadata']
                 items.append((item_id, item_text, item_metadata))
         if where is not None:
             items = [item for item in items if all(item[2].get(key) == value for key, value in where.items())]
         return items
 
     def set(self, id, text=None, metadata=None, vector=None):
-        logger.info(f"[VLite.set] Setting attributes for item with ID: {id}")
+        print(f"[VLite.set] Setting attributes for item with ID: {id}")
         chunk_ids = [chunk_id for chunk_id in self.index if chunk_id.startswith(f"{id}_")]
         if chunk_ids:
             self.update(id, text, metadata, vector)
         else:
             self.add(text, metadata=metadata, item_id=id)
-        logger.info(f"[VLite.set] Item with ID '{id}' created successfully.")
+        print(f"[VLite.set] Item with ID '{id}' created successfully.")
     
     
     def set_batch(self, texts, embeddings, metadatas=None):
         start_time = time.time()
         if not isinstance(texts, list):
             texts = [texts]
 
@@ -251,43 +258,43 @@
                 'text': text,
                 'metadata': metadata,
                 'binary_vector': embedding.tolist()
             }
     
 
         self.save()
-        logger.info("[VLite.set_batch] Texts added successfully.")
+        print("[VLite.set_batch] Texts added successfully.")
         end_time = time.time()
-        logger.debug(f"[VLite.set_batch] Execution time: {end_time - start_time:.5f} seconds")
+        print(f"[VLite.set_batch] Execution time: {end_time - start_time:.5f} seconds")
         
 
     def count(self):
         return len(self.index)
 
     def save(self):
-        logger.info(f"[VLite.save] Saving collection to {self.collection}")
+        print(f"[VLite.save] Saving collection to {self.collection}")
         with self.ctx.create(self.collection) as ctx_file:
             ctx_file.set_header(
                 embedding_model="mixedbread-ai/mxbai-embed-large-v1",
                 embedding_size=64,  # Set the correct embedding size here
                 embedding_dtype=self.model.embedding_dtype,
                 context_length=self.model.context_length
             )
             for chunk_id, chunk_data in self.index.items():
                 ctx_file.add_embedding(chunk_data['binary_vector'])
                 ctx_file.add_context(chunk_data['text'])
                 if 'metadata' in chunk_data:
                     ctx_file.add_metadata(chunk_id, chunk_data['metadata'])
-        logger.info("[VLite.save] Collection saved successfully.")
+        print("[VLite.save] Collection saved successfully.")
 
     def clear(self):
-        logger.info("[VLite.clear] Clearing the collection...")
+        print("[VLite.clear] Clearing the collection...")
         self.index = {}
         self.ctx.delete(self.collection)
-        logger.info("[VLite.clear] Collection cleared.")
+        print("[VLite.clear] Collection cleared.")
 
     def info(self):
         print("[VLite.info] Collection Information:")
         print(f"[VLite.info] Items: {self.count()}")
         print(f"[VLite.info] Collection file: {self.collection}")
         print(f"[VLite.info] Embedding model: {self.model}")
```

### Comparing `vlite-0.2.4/vlite/model.py` & `vlite-0.2.5/vlite/model.py`

 * *Files identical despite different names*

### Comparing `vlite-0.2.4/vlite/server.py` & `vlite-0.2.5/vlite/server.py`

 * *Files identical despite different names*

### Comparing `vlite-0.2.4/vlite/utils.py` & `vlite-0.2.5/vlite/utils.py`

 * *Files identical despite different names*

### Comparing `vlite-0.2.4/vlite.egg-info/PKG-INFO` & `vlite-0.2.5/vlite.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlite
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple and blazing fast vector database
 Author: Surya Dantuluri
 Author-email: surya@suryad.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

