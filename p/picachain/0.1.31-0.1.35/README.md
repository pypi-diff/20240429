# Comparing `tmp/picachain-0.1.31.tar.gz` & `tmp/picachain-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picachain-0.1.31.tar", max compression
+gzip compressed data, was "picachain-0.1.35.tar", max compression
```

## Comparing `picachain-0.1.31.tar` & `picachain-0.1.35.tar`

### file list

```diff
@@ -1,18 +1,38 @@
--rw-r--r--   0        0        0     1070 2024-03-27 18:13:06.705397 picachain-0.1.31/LICENSE
--rw-r--r--   0        0        0     1916 2024-04-01 15:35:54.123339 picachain-0.1.31/README.md
--rw-r--r--   0        0        0        0 2024-03-27 17:21:07.953194 picachain-0.1.31/picachain/__init__.py
--rw-r--r--   0        0        0      230 2024-03-29 17:34:59.884284 picachain-0.1.31/picachain/datastore/__init__.py
--rw-r--r--   0        0        0     3239 2024-04-01 15:41:21.052985 picachain-0.1.31/picachain/datastore/chroma.py
--rw-r--r--   0        0        0      812 2024-04-01 16:56:46.230418 picachain-0.1.31/picachain/datastore/datastore.py
--rw-r--r--   0        0        0     4523 2024-04-01 17:07:15.694551 picachain-0.1.31/picachain/datastore/pinecone.py
--rw-r--r--   0        0        0      166 2024-03-29 17:30:15.708875 picachain-0.1.31/picachain/embedding/__init__.py
--rw-r--r--   0        0        0     1836 2024-03-30 17:40:26.622816 picachain-0.1.31/picachain/embedding/clip_embedding.py
--rw-r--r--   0        0        0      570 2024-03-29 13:24:42.213948 picachain-0.1.31/picachain/embedding/embedding.py
--rw-r--r--   0        0        0      169 2024-03-31 14:45:13.557494 picachain-0.1.31/picachain/retriever/__init__.py
--rw-r--r--   0        0        0     3383 2024-04-01 18:46:27.787337 picachain-0.1.31/picachain/retriever/image_retriever.py
--rw-r--r--   0        0        0      272 2024-03-31 14:40:10.519412 picachain-0.1.31/picachain/retriever/retriever.py
--rw-r--r--   0        0        0       81 2024-04-01 09:22:48.252396 picachain-0.1.31/picachain/search/__init__.py
--rw-r--r--   0        0        0      716 2024-04-01 18:45:01.928742 picachain-0.1.31/picachain/search/image_search.py
--rw-r--r--   0        0        0      457 2024-03-31 08:34:46.916761 picachain-0.1.31/picachain/utils/image_util.py
--rw-r--r--   0        0        0      784 2024-04-01 18:59:08.637479 picachain-0.1.31/pyproject.toml
--rw-r--r--   0        0        0     2926 1970-01-01 00:00:00.000000 picachain-0.1.31/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-17 07:30:12.529259 picachain-0.1.35/LICENSE
+-rw-r--r--   0        0        0     3408 2024-04-29 17:34:45.180425 picachain-0.1.35/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 07:30:12.529259 picachain-0.1.35/picachain/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:30:12.529259 picachain-0.1.35/picachain/chains/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-29 17:25:55.224130 picachain-0.1.35/picachain/chains/chain.py
+-rw-r--r--   0        0        0     1390 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/chains/image/search.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/chains/unstructured/__init__.py
+-rw-r--r--   0        0        0     1448 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/chains/unstructured/charts.py
+-rw-r--r--   0        0        0      230 2024-04-17 07:30:12.529259 picachain-0.1.35/picachain/datastore/__init__.py
+-rw-r--r--   0        0        0     3239 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/datastore/chroma.py
+-rw-r--r--   0        0        0      812 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/datastore/datastore.py
+-rw-r--r--   0        0        0     4523 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/datastore/pinecone.py
+-rw-r--r--   0        0        0      166 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/embedding/__init__.py
+-rw-r--r--   0        0        0     1836 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/embedding/clip_embedding.py
+-rw-r--r--   0        0        0      570 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/embedding/embedding.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/generation/__init__.py
+-rw-r--r--   0        0        0      950 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/generation/text2image.py
+-rw-r--r--   0        0        0      382 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/deplot/__init__.py
+-rw-r--r--   0        0        0      978 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/models/deplot/deplot.py
+-rw-r--r--   0        0        0      258 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/donut/__init__.py
+-rw-r--r--   0        0        0     2559 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/donut/classification.py
+-rw-r--r--   0        0        0     2571 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/donut/cord.py
+-rw-r--r--   0        0        0     2585 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/donut/docvqa.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/llava/__init__.py
+-rw-r--r--   0        0        0     2008 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/llava/llava.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/models/openai/__init__.py
+-rw-r--r--   0        0        0     1134 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/models/openai/openai.py
+-rw-r--r--   0        0        0       93 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/pydantic.py
+-rw-r--r--   0        0        0      169 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/retriever/__init__.py
+-rw-r--r--   0        0        0     2580 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/retriever/image_retriever.py
+-rw-r--r--   0        0        0      268 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/retriever/retriever.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/unstructured/__init__.py
+-rw-r--r--   0        0        0      513 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/unstructured/charts.py
+-rw-r--r--   0        0        0      385 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/unstructured/tables.py
+-rw-r--r--   0        0        0      457 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/utils/image_util.py
+-rw-r--r--   0        0        0      821 2024-04-29 17:41:29.743038 picachain-0.1.35/pyproject.toml
+-rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 picachain-0.1.35/PKG-INFO
```

### Comparing `picachain-0.1.31/LICENSE` & `picachain-0.1.35/LICENSE`

 * *Files identical despite different names*

### Comparing `picachain-0.1.31/picachain/datastore/chroma.py` & `picachain-0.1.35/picachain/datastore/chroma.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.31/picachain/datastore/datastore.py` & `picachain-0.1.35/picachain/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.31/picachain/datastore/pinecone.py` & `picachain-0.1.35/picachain/datastore/pinecone.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.31/picachain/embedding/clip_embedding.py` & `picachain-0.1.35/picachain/embedding/clip_embedding.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.31/picachain/embedding/embedding.py` & `picachain-0.1.35/picachain/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.31/picachain/retriever/image_retriever.py` & `picachain-0.1.35/picachain/retriever/image_retriever.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import uuid
-from collections import defaultdict
 from typing import List, Union
 
 from PIL.Image import Image
 
 from picachain.datastore import ChromaStore, PineconeStore
 from picachain.embedding import ClipEmbedding, Embedding
 from picachain.utils.image_util import image_to_base64
@@ -47,48 +46,32 @@
     def _push_embedding_to_datastore(self):
         """Push embeddings and documents to datastore."""
         try:
             embeddings = self.datastore.generate_embeddings(self.images, self.embedding)
             self.datastore_collection_index = self.datastore.create()
             documents = self._process_images_for_storage()
             ids = self._create_ids_for_images(documents)
-
-            if isinstance(self.datastore, ChromaStore):
-                self.datastore.add(
-                    collection=self.datastore_collection_index,
-                    embeddings=embeddings,
-                    documents=documents,
-                    ids=ids,
-                )
-            elif isinstance(self.datastore, PineconeStore):
-                self.datastore.add(
-                    index=self.datastore_collection_index,
-                    embeddings=embeddings,
-                    documents=documents,
-                    ids=ids,
-                )
+            self.datastore.add(
+                self.datastore_collection_index,
+                embeddings,
+                documents,
+                ids,
+            )
         except Exception as e:
             raise Exception("Failed to push embeddings", e)
 
-    def get_relevant_images(self, query_embedding: list, top_k: int) -> list:
+    def relevant_images(self, query_embedding: list, top_k: int) -> list:
         """Retrieve top k relevant images from datastore.
 
         Args:
         - query_embedding: query image embedding.
         - top_k (int): top k relevant images to retrieve.
 
         Returns:
         - list of relevant images.
         """
-        if isinstance(self.datastore, ChromaStore):
-            relevant_images = self.datastore.query(
-                collection=self.datastore_collection_index,
-                query_embedding=query_embedding,
-                top_k=top_k,
-            )
-        elif isinstance(self.datastore, PineconeStore):
-            relevant_images = self.datastore.query(
-                index=self.datastore_collection_index,
-                query_embedding=query_embedding,
-                top_k=top_k,
-            )
+        relevant_images = self.datastore.query(
+            self.datastore_collection_index,
+            query_embedding,
+            top_k,
+        )
         return relevant_images
```

### Comparing `picachain-0.1.31/pyproject.toml` & `picachain-0.1.35/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 authors = ["d1pankarmedhi <dipankarmedhi11@gmail.com>"]
-description = "Simple image search engine package."
+description = "Build quick LLM pipelines for image specific tasks."
 homepage = "https://github.com/d1pankarmedhi/picachain"
 keywords = [
   "python",
   "search-engine",
   "chromadb",
   "image",
   "search",
@@ -14,22 +14,23 @@
   "pinecone",
 ]
 license = "MIT"
 name = "picachain"
 packages = [{include = "picachain"}]
 readme = "README.md"
 repository = "https://github.com/d1pankarmedhi/picachain"
-version = "0.1.31"
+version = "0.1.35"
 
 [tool.poetry.dependencies]
 chromadb = "^0.4.24"
 matplotlib = "^3.8.3"
-pillow = "9.4.0"
+pillow = "^10.3.0"
 pinecone-client = "^3.2.1"
 pysqlite3-binary = "^0.5.2.post3"
 python = "^3.10"
-torch = "2.2.1"
-transformers = "^4.39.1"
+
+[tool.poetry.group.dev.dependencies]
+ipykernel = "^6.29.4"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
```

