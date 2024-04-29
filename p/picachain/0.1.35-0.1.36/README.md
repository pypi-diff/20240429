# Comparing `tmp/picachain-0.1.35.tar.gz` & `tmp/picachain-0.1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picachain-0.1.35.tar", max compression
+gzip compressed data, was "picachain-0.1.36.tar", max compression
```

## Comparing `picachain-0.1.35.tar` & `picachain-0.1.36.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1070 2024-04-17 07:30:12.529259 picachain-0.1.35/LICENSE
--rw-r--r--   0        0        0     3408 2024-04-29 17:34:45.180425 picachain-0.1.35/README.md
--rw-r--r--   0        0        0        0 2024-04-17 07:30:12.529259 picachain-0.1.35/picachain/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 07:30:12.529259 picachain-0.1.35/picachain/chains/__init__.py
--rw-r--r--   0        0        0      140 2024-04-29 17:25:55.224130 picachain-0.1.35/picachain/chains/chain.py
--rw-r--r--   0        0        0     1390 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/chains/image/search.py
--rw-r--r--   0        0        0        0 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/chains/unstructured/__init__.py
--rw-r--r--   0        0        0     1448 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/chains/unstructured/charts.py
--rw-r--r--   0        0        0      230 2024-04-17 07:30:12.529259 picachain-0.1.35/picachain/datastore/__init__.py
--rw-r--r--   0        0        0     3239 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/datastore/chroma.py
--rw-r--r--   0        0        0      812 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/datastore/datastore.py
--rw-r--r--   0        0        0     4523 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/datastore/pinecone.py
--rw-r--r--   0        0        0      166 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/embedding/__init__.py
--rw-r--r--   0        0        0     1836 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/embedding/clip_embedding.py
--rw-r--r--   0        0        0      570 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/embedding/embedding.py
--rw-r--r--   0        0        0        0 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/generation/__init__.py
--rw-r--r--   0        0        0      950 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/generation/text2image.py
--rw-r--r--   0        0        0      382 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/deplot/__init__.py
--rw-r--r--   0        0        0      978 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/models/deplot/deplot.py
--rw-r--r--   0        0        0      258 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/donut/__init__.py
--rw-r--r--   0        0        0     2559 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/donut/classification.py
--rw-r--r--   0        0        0     2571 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/donut/cord.py
--rw-r--r--   0        0        0     2585 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/donut/docvqa.py
--rw-r--r--   0        0        0        0 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/llava/__init__.py
--rw-r--r--   0        0        0     2008 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/models/llava/llava.py
--rw-r--r--   0        0        0        0 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/models/openai/__init__.py
--rw-r--r--   0        0        0     1134 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/models/openai/openai.py
--rw-r--r--   0        0        0       93 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/pydantic.py
--rw-r--r--   0        0        0      169 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/retriever/__init__.py
--rw-r--r--   0        0        0     2580 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/retriever/image_retriever.py
--rw-r--r--   0        0        0      268 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/retriever/retriever.py
--rw-r--r--   0        0        0        0 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/unstructured/__init__.py
--rw-r--r--   0        0        0      513 2024-04-29 17:25:55.232130 picachain-0.1.35/picachain/unstructured/charts.py
--rw-r--r--   0        0        0      385 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/unstructured/tables.py
--rw-r--r--   0        0        0      457 2024-04-17 07:30:12.533259 picachain-0.1.35/picachain/utils/image_util.py
--rw-r--r--   0        0        0      821 2024-04-29 17:41:29.743038 picachain-0.1.35/pyproject.toml
--rw-r--r--   0        0        0     4366 1970-01-01 00:00:00.000000 picachain-0.1.35/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-17 07:30:12.529259 picachain-0.1.36/LICENSE
+-rw-r--r--   0        0        0     3408 2024-04-29 17:34:45.180425 picachain-0.1.36/README.md
+-rw-r--r--   0        0        0        0 2024-04-17 07:30:12.529259 picachain-0.1.36/picachain/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:30:12.529259 picachain-0.1.36/picachain/chains/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-29 17:25:55.224130 picachain-0.1.36/picachain/chains/chain.py
+-rw-r--r--   0        0        0     1390 2024-04-29 17:25:55.232130 picachain-0.1.36/picachain/chains/image/search.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:25:55.232130 picachain-0.1.36/picachain/chains/unstructured/__init__.py
+-rw-r--r--   0        0        0     1448 2024-04-29 17:25:55.232130 picachain-0.1.36/picachain/chains/unstructured/charts.py
+-rw-r--r--   0        0        0      230 2024-04-17 07:30:12.529259 picachain-0.1.36/picachain/datastore/__init__.py
+-rw-r--r--   0        0        0     3239 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/datastore/chroma.py
+-rw-r--r--   0        0        0      812 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/datastore/datastore.py
+-rw-r--r--   0        0        0     4523 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/datastore/pinecone.py
+-rw-r--r--   0        0        0      166 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/embedding/__init__.py
+-rw-r--r--   0        0        0     1836 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/embedding/clip_embedding.py
+-rw-r--r--   0        0        0      570 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/embedding/embedding.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/generation/__init__.py
+-rw-r--r--   0        0        0      950 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/generation/text2image.py
+-rw-r--r--   0        0        0      382 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/models/deplot/__init__.py
+-rw-r--r--   0        0        0      978 2024-04-29 17:25:55.232130 picachain-0.1.36/picachain/models/deplot/deplot.py
+-rw-r--r--   0        0        0      258 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/models/donut/__init__.py
+-rw-r--r--   0        0        0     2559 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/models/donut/classification.py
+-rw-r--r--   0        0        0     2571 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/models/donut/cord.py
+-rw-r--r--   0        0        0     2585 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/models/donut/docvqa.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/models/llava/__init__.py
+-rw-r--r--   0        0        0     2008 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/models/llava/llava.py
+-rw-r--r--   0        0        0        0 2024-04-29 17:25:55.232130 picachain-0.1.36/picachain/models/openai/__init__.py
+-rw-r--r--   0        0        0     1134 2024-04-29 17:25:55.232130 picachain-0.1.36/picachain/models/openai/openai.py
+-rw-r--r--   0        0        0       93 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/pydantic.py
+-rw-r--r--   0        0        0      169 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/retriever/__init__.py
+-rw-r--r--   0        0        0     2580 2024-04-29 17:25:55.232130 picachain-0.1.36/picachain/retriever/image_retriever.py
+-rw-r--r--   0        0        0      268 2024-04-29 17:25:55.232130 picachain-0.1.36/picachain/retriever/retriever.py
+-rw-r--r--   0        0        0        0 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/unstructured/__init__.py
+-rw-r--r--   0        0        0      513 2024-04-29 17:25:55.232130 picachain-0.1.36/picachain/unstructured/charts.py
+-rw-r--r--   0        0        0      385 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/unstructured/tables.py
+-rw-r--r--   0        0        0      457 2024-04-17 07:30:12.533259 picachain-0.1.36/picachain/utils/image_util.py
+-rw-r--r--   0        0        0      832 2024-04-29 17:58:09.320107 picachain-0.1.36/pyproject.toml
+-rw-r--r--   0        0        0     4385 1970-01-01 00:00:00.000000 picachain-0.1.36/PKG-INFO
```

### Comparing `picachain-0.1.35/LICENSE` & `picachain-0.1.36/LICENSE`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/README.md` & `picachain-0.1.36/README.md`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/chains/image/search.py` & `picachain-0.1.36/picachain/chains/image/search.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/chains/unstructured/charts.py` & `picachain-0.1.36/picachain/chains/unstructured/charts.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/datastore/chroma.py` & `picachain-0.1.36/picachain/datastore/chroma.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/datastore/datastore.py` & `picachain-0.1.36/picachain/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/datastore/pinecone.py` & `picachain-0.1.36/picachain/datastore/pinecone.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/embedding/clip_embedding.py` & `picachain-0.1.36/picachain/embedding/clip_embedding.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/embedding/embedding.py` & `picachain-0.1.36/picachain/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/generation/text2image.py` & `picachain-0.1.36/picachain/generation/text2image.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/models/deplot/deplot.py` & `picachain-0.1.36/picachain/models/deplot/deplot.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/models/donut/classification.py` & `picachain-0.1.36/picachain/models/donut/classification.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/models/donut/cord.py` & `picachain-0.1.36/picachain/models/donut/cord.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/models/donut/docvqa.py` & `picachain-0.1.36/picachain/models/donut/docvqa.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/models/llava/llava.py` & `picachain-0.1.36/picachain/models/llava/llava.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/models/openai/openai.py` & `picachain-0.1.36/picachain/models/openai/openai.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/retriever/image_retriever.py` & `picachain-0.1.36/picachain/retriever/image_retriever.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/picachain/unstructured/charts.py` & `picachain-0.1.36/picachain/unstructured/charts.py`

 * *Files identical despite different names*

### Comparing `picachain-0.1.35/pyproject.toml` & `picachain-0.1.36/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -14,20 +14,21 @@
   "pinecone",
 ]
 license = "MIT"
 name = "picachain"
 packages = [{include = "picachain"}]
 readme = "README.md"
 repository = "https://github.com/d1pankarmedhi/picachain"
-version = "0.1.35"
+version = "0.1.36"
 
 [tool.poetry.dependencies]
 chromadb = "^0.4.24"
+idna = "3.7"
 matplotlib = "^3.8.3"
-pillow = "^10.3.0"
+pillow = "9.4.0"
 pinecone-client = "^3.2.1"
 pysqlite3-binary = "^0.5.2.post3"
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.4"
```

### Comparing `picachain-0.1.35/PKG-INFO` & `picachain-0.1.36/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: picachain
-Version: 0.1.35
+Version: 0.1.36
 Summary: Build quick LLM pipelines for image specific tasks.
 Home-page: https://github.com/d1pankarmedhi/picachain
 License: MIT
 Keywords: python,search-engine,chromadb,image,search,packages,poetry,python-packages,pinecone
 Author: d1pankarmedhi
 Author-email: dipankarmedhi11@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: chromadb (>=0.4.24,<0.5.0)
+Requires-Dist: idna (==3.7)
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
-Requires-Dist: pillow (>=10.3.0,<11.0.0)
+Requires-Dist: pillow (==9.4.0)
 Requires-Dist: pinecone-client (>=3.2.1,<4.0.0)
 Requires-Dist: pysqlite3-binary (>=0.5.2.post3,<0.6.0)
 Project-URL: Repository, https://github.com/d1pankarmedhi/picachain
 Description-Content-Type: text/markdown
 
 <div align="center">
 <img src="https://github.com/d1pankarmedhi/picachain/assets/136924835/3a299c21-6590-4ee1-a3c1-73a92653f21e" height=150></img>
```

