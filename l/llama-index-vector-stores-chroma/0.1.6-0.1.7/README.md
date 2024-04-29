# Comparing `tmp/llama_index_vector_stores_chroma-0.1.6.tar.gz` & `tmp/llama_index_vector_stores_chroma-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_chroma-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_chroma-0.1.7.tar", max compression
```

## Comparing `llama_index_vector_stores_chroma-0.1.6.tar` & `llama_index_vector_stores_chroma-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       47 2024-03-08 16:40:27.149148 llama_index_vector_stores_chroma-0.1.6/README.md
--rw-r--r--   0        0        0      101 2024-03-08 16:40:27.149148 llama_index_vector_stores_chroma-0.1.6/llama_index/vector_stores/chroma/__init__.py
--rw-r--r--   0        0        0    12753 2024-03-08 16:40:27.149148 llama_index_vector_stores_chroma-0.1.6/llama_index/vector_stores/chroma/base.py
--rw-r--r--   0        0        0     1480 2024-03-08 16:40:27.149148 llama_index_vector_stores_chroma-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 llama_index_vector_stores_chroma-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       47 2024-04-29 20:35:25.243285 llama_index_vector_stores_chroma-0.1.7/README.md
+-rw-r--r--   0        0        0      101 2024-04-29 20:35:25.243285 llama_index_vector_stores_chroma-0.1.7/llama_index/vector_stores/chroma/__init__.py
+-rw-r--r--   0        0        0    13268 2024-04-29 20:35:25.243285 llama_index_vector_stores_chroma-0.1.7/llama_index/vector_stores/chroma/base.py
+-rw-r--r--   0        0        0     1487 2024-04-29 20:35:25.243285 llama_index_vector_stores_chroma-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 llama_index_vector_stores_chroma-0.1.7/PKG-INFO
```

### Comparing `llama_index_vector_stores_chroma-0.1.6/llama_index/vector_stores/chroma/base.py` & `llama_index_vector_stores_chroma-0.1.7/llama_index/vector_stores/chroma/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,14 +112,29 @@
     During query time, the index uses ChromaDB to query for the top
     k most similar nodes.
 
     Args:
         chroma_collection (chromadb.api.models.Collection.Collection):
             ChromaDB collection instance
 
+    Examples:
+        `pip install llama-index-vector-stores-chroma`
+
+        ```python
+        import chromadb
+        from llama_index.vector_stores.chroma import ChromaVectorStore
+
+        # Create a Chroma client and collection
+        chroma_client = chromadb.EphemeralClient()
+        chroma_collection = chroma_client.create_collection("example_collection")
+
+        # Set up the ChromaVectorStore and StorageContext
+        vector_store = ChromaVectorStore(chroma_collection=chroma_collection)
+        ```
+
     """
 
     stores_text: bool = True
     flat_metadata: bool = True
 
     collection_name: Optional[str]
     host: Optional[str]
```

### Comparing `llama_index_vector_stores_chroma-0.1.6/pyproject.toml` & `llama_index_vector_stores_chroma-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores chroma integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-chroma"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
-chromadb = "^0.4.22"
+chromadb = ">=0.4.0,<0.6.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_vector_stores_chroma-0.1.6/PKG-INFO` & `llama_index_vector_stores_chroma-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-chroma
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index vector_stores chroma integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: chromadb (>=0.4.22,<0.5.0)
+Requires-Dist: chromadb (>=0.4.0,<0.6.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Vector_Stores Integration: Chroma
```

