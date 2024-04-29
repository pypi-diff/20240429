# Comparing `tmp/LLM_Mediator-0.9.8.tar.gz` & `tmp/LLM_Mediator-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LLM_Mediator-0.9.8.tar", last modified: Tue Nov 14 09:18:36 2023, max compression
+gzip compressed data, was "LLM_Mediator-0.9.9.tar", last modified: Tue Nov 14 10:16:35 2023, max compression
```

## Comparing `LLM_Mediator-0.9.8.tar` & `LLM_Mediator-0.9.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-11-14 09:18:36.181131 LLM_Mediator-0.9.8/
--rw-rw-rw-   0        0        0     1091 2023-11-13 08:55:50.000000 LLM_Mediator-0.9.8/LICENSE
-drwxrwxrwx   0        0        0        0 2023-11-14 09:18:36.169548 LLM_Mediator-0.9.8/LLM_Mediator.egg-info/
--rw-rw-rw-   0        0        0     2091 2023-11-14 09:18:36.000000 LLM_Mediator-0.9.8/LLM_Mediator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-11-14 09:18:36.000000 LLM_Mediator-0.9.8/LLM_Mediator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-14 09:18:36.000000 LLM_Mediator-0.9.8/LLM_Mediator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-11-14 09:18:36.000000 LLM_Mediator-0.9.8/LLM_Mediator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-11-14 09:18:36.000000 LLM_Mediator-0.9.8/LLM_Mediator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2091 2023-11-14 09:18:36.180119 LLM_Mediator-0.9.8/PKG-INFO
--rw-rw-rw-   0        0        0     1181 2023-11-13 08:55:50.000000 LLM_Mediator-0.9.8/README.md
-drwxrwxrwx   0        0        0        0 2023-11-14 09:18:36.178128 LLM_Mediator-0.9.8/llm_mediator/
--rw-rw-rw-   0        0        0        0 2023-05-22 03:12:01.000000 LLM_Mediator-0.9.8/llm_mediator/__init__.py
--rw-rw-rw-   0        0        0     1454 2023-08-08 08:32:08.000000 LLM_Mediator-0.9.8/llm_mediator/cache.py
--rw-rw-rw-   0        0        0     2851 2023-09-12 18:25:37.000000 LLM_Mediator-0.9.8/llm_mediator/embedding.py
--rw-rw-rw-   0        0        0      993 2023-09-24 16:13:01.000000 LLM_Mediator-0.9.8/llm_mediator/folders.py
--rw-rw-rw-   0        0        0     1425 2023-07-27 03:22:50.000000 LLM_Mediator-0.9.8/llm_mediator/formatter.py
--rw-rw-rw-   0        0        0    19657 2023-11-14 08:13:13.000000 LLM_Mediator-0.9.8/llm_mediator/gpt.py
--rw-rw-rw-   0        0        0    20157 2023-09-25 03:05:58.000000 LLM_Mediator-0.9.8/llm_mediator/llm.py
--rw-rw-rw-   0        0        0     3929 2023-09-18 07:07:02.000000 LLM_Mediator-0.9.8/llm_mediator/parallel_tasks_queuer.py
--rw-rw-rw-   0        0        0       42 2023-11-14 09:18:36.181131 LLM_Mediator-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     3292 2023-11-14 09:18:26.000000 LLM_Mediator-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-11-14 10:16:35.644369 LLM_Mediator-0.9.9/
+-rw-rw-rw-   0        0        0     1091 2023-11-13 08:55:50.000000 LLM_Mediator-0.9.9/LICENSE
+drwxrwxrwx   0        0        0        0 2023-11-14 10:16:35.622653 LLM_Mediator-0.9.9/LLM_Mediator.egg-info/
+-rw-rw-rw-   0        0        0     2091 2023-11-14 10:16:35.000000 LLM_Mediator-0.9.9/LLM_Mediator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-11-14 10:16:35.000000 LLM_Mediator-0.9.9/LLM_Mediator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-11-14 10:16:35.000000 LLM_Mediator-0.9.9/LLM_Mediator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-11-14 10:16:35.000000 LLM_Mediator-0.9.9/LLM_Mediator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-11-14 10:16:35.000000 LLM_Mediator-0.9.9/LLM_Mediator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2091 2023-11-14 10:16:35.643369 LLM_Mediator-0.9.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1181 2023-11-13 08:55:50.000000 LLM_Mediator-0.9.9/README.md
+drwxrwxrwx   0        0        0        0 2023-11-14 10:16:35.641357 LLM_Mediator-0.9.9/llm_mediator/
+-rw-rw-rw-   0        0        0        0 2023-05-22 03:12:01.000000 LLM_Mediator-0.9.9/llm_mediator/__init__.py
+-rw-rw-rw-   0        0        0     1454 2023-08-08 08:32:08.000000 LLM_Mediator-0.9.9/llm_mediator/cache.py
+-rw-rw-rw-   0        0        0     2851 2023-09-12 18:25:37.000000 LLM_Mediator-0.9.9/llm_mediator/embedding.py
+-rw-rw-rw-   0        0        0      993 2023-09-24 16:13:01.000000 LLM_Mediator-0.9.9/llm_mediator/folders.py
+-rw-rw-rw-   0        0        0     1425 2023-07-27 03:22:50.000000 LLM_Mediator-0.9.9/llm_mediator/formatter.py
+-rw-rw-rw-   0        0        0    20698 2023-11-14 10:06:53.000000 LLM_Mediator-0.9.9/llm_mediator/gpt.py
+-rw-rw-rw-   0        0        0    20157 2023-09-25 03:05:58.000000 LLM_Mediator-0.9.9/llm_mediator/llm.py
+-rw-rw-rw-   0        0        0     3929 2023-09-18 07:07:02.000000 LLM_Mediator-0.9.9/llm_mediator/parallel_tasks_queuer.py
+-rw-rw-rw-   0        0        0       42 2023-11-14 10:16:35.644369 LLM_Mediator-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     3292 2023-11-14 10:06:51.000000 LLM_Mediator-0.9.9/setup.py
```

### Comparing `LLM_Mediator-0.9.8/LICENSE` & `LLM_Mediator-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `LLM_Mediator-0.9.8/LLM_Mediator.egg-info/PKG-INFO` & `LLM_Mediator-0.9.9/LLM_Mediator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLM-Mediator
-Version: 0.9.8
+Version: 0.9.9
 Summary: Just a simple mediator for different LLM models.
 Home-page: https://github.com/zeuscsc/llm_mediator.git
 Author: Zeus Chiu
 Author-email: zeuscsc@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `LLM_Mediator-0.9.8/PKG-INFO` & `LLM_Mediator-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LLM_Mediator
-Version: 0.9.8
+Version: 0.9.9
 Summary: Just a simple mediator for different LLM models.
 Home-page: https://github.com/zeuscsc/llm_mediator.git
 Author: Zeus Chiu
 Author-email: zeuscsc@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `LLM_Mediator-0.9.8/README.md` & `LLM_Mediator-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `LLM_Mediator-0.9.8/llm_mediator/cache.py` & `LLM_Mediator-0.9.9/llm_mediator/cache.py`

 * *Files identical despite different names*

### Comparing `LLM_Mediator-0.9.8/llm_mediator/embedding.py` & `LLM_Mediator-0.9.9/llm_mediator/embedding.py`

 * *Files identical despite different names*

### Comparing `LLM_Mediator-0.9.8/llm_mediator/folders.py` & `LLM_Mediator-0.9.9/llm_mediator/folders.py`

 * *Files identical despite different names*

### Comparing `LLM_Mediator-0.9.8/llm_mediator/formatter.py` & `LLM_Mediator-0.9.9/llm_mediator/formatter.py`

 * *Files identical despite different names*

### Comparing `LLM_Mediator-0.9.8/llm_mediator/gpt.py` & `LLM_Mediator-0.9.9/llm_mediator/gpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,81 +45,93 @@
             return GPT3_MODEL
         else:
             return None
     class BaseGeneratorExtractor(ABC):
         @abstractmethod
         def get_extraction_path(self,chunk):
             pass
-        def extract_text_from_generator_chunk(self,chunk:ChatCompletionChunk):
-            node=chunk.choices[0]
+        def get_choice0(self,chunk:ChatCompletionChunk|dict):
+            if hasattr(chunk,"choices") and len(chunk.choices)>0:
+                return chunk.choices[0]
+            elif "choices" in chunk and len(chunk["choices"])>0:
+                return chunk["choices"][0]
+        def extract_text_from_generator_chunk(self,chunk:ChatCompletionChunk|dict):
+            node=self.get_choice0(chunk)
             extraction_path=self.get_extraction_path(chunk)
             if extraction_path is None:
                 return ""
+            if isinstance(chunk,dict):
+                return self.extract_text_from_dict_chunk(chunk,extraction_path)
             for key in extraction_path:
                 if hasattr(node,key) and getattr(node,key) is not None:
                     node = getattr(node,key)
                 else:
                     return ""
             return node
         def append_text_into_generator_chunk(self,chunk:ChatCompletionChunk,text):
-            node=chunk.choices[0]
+            node=self.get_choice0(chunk)
             extraction_path=self.get_extraction_path(chunk)
             if extraction_path is None:
                 return chunk
+            if isinstance(chunk,dict):
+                return self.append_text_into_dict_chunk(chunk,text,extraction_path)
             for key in extraction_path:
                 if hasattr(node,key) and getattr(node,key) is not None:
                     parent_node=node
                     node = getattr(node,key)
             if isinstance(node,str) and isinstance(text,str):
-                original_text=getattr(parent_node,extraction_path[-1])
-                current_key=extraction_path[-1]
-                targeted_text=original_text+text
                 setattr(parent_node,extraction_path[-1],getattr(parent_node,extraction_path[-1])+text)
             return chunk
+        
+        def extract_text_from_dict_chunk(self,chunk,generator_extracting_path):
+            node=self.get_choice0(chunk)
+            for key in generator_extracting_path:
+                try:
+                    node = node[key]
+                except KeyError:
+                    return ""
+            return node
+        def append_text_into_dict_chunk(self,chunk,text,generator_extracting_path):
+            node=self.get_choice0(chunk)
+            for key in generator_extracting_path:
+                try:
+                    parent_node=node
+                    node = node[key]
+                except KeyError:
+                    return chunk
+            if isinstance(node,str) and isinstance(text,str):
+                parent_node[generator_extracting_path[-1]]+=text
+            return chunk
         pass
     class AutoGeneratorExtractor(BaseGeneratorExtractor):
         @staticmethod
-        def get_extraction_path(chunk:ChatCompletionChunk):
-            if hasattr(chunk,"choices") and len(chunk.choices)>0:
-                choice:Choice=chunk.choices[0]
-                if hasattr(choice,"delta") \
-                    and hasattr(choice.delta,"content") and choice.delta.content is not None:
-                    return ["delta","content"]
-                elif hasattr(choice,"delta") \
-                    and hasattr(choice.delta,"function_call") and hasattr(choice.delta.function_call,"arguments")\
-                        and choice.delta.function_call.arguments is not None:
-                    return ["delta","function_call","arguments"]
+        def get_extraction_path(chunk:ChatCompletionChunk|dict):
+            text_path=["delta","content"]
+            functional_path=["delta","function_call","arguments"]
+            if isinstance(chunk,dict):
+                if "choices" in chunk and len(chunk["choices"])>0:
+                    choice=chunk["choices"][0]
+                    if "delta" in choice and "content" in choice["delta"]:
+                        return text_path
+                    elif "delta" in choice and "function_call" in choice["delta"] and "arguments" in choice["delta"]["function_call"]:
+                        return functional_path
+            if isinstance(chunk,ChatCompletionChunk):
+                if hasattr(chunk,"choices") and len(chunk.choices)>0:
+                    choice:Choice=chunk.choices[0]
+                    if hasattr(choice,"delta") and hasattr(choice.delta,"content") and choice.delta.content is not None:
+                        return text_path
+                    elif hasattr(choice,"delta") and hasattr(choice.delta,"function_call") and hasattr(choice.delta.function_call,"arguments") and choice.delta.function_call.arguments is not None:
+                        return functional_path
             return None
         pass
     
     def extract_text_from_chat_completion_chunk(chunk,completion_extractor:BaseGeneratorExtractor=AutoGeneratorExtractor,**_):
         return completion_extractor().extract_text_from_generator_chunk(chunk)
     def append_text_into_chat_completion_chunk(chunk,text,completion_extractor:BaseGeneratorExtractor=AutoGeneratorExtractor,**_):
         return completion_extractor().append_text_into_generator_chunk(chunk,text)
-
-
-    def extract_text_from_generator_chunk(chunk,generator_extracting_path):
-        node=chunk
-        for key in generator_extracting_path:
-            try:
-                node = node[key]
-            except KeyError:
-                return ""
-        return node
-    def append_text_into_generator_chunk(chunk,text,generator_extracting_path):
-        node=chunk
-        for key in generator_extracting_path:
-            try:
-                parent_node=node
-                node = node[key]
-            except KeyError:
-                return chunk
-        if isinstance(node,str) and isinstance(text,str):
-            parent_node[generator_extracting_path[-1]]+=text
-        return chunk
     
     def get_embeddings(self,sentences:str|list[str]):
         origin_sentences_type=type(sentences)
         if origin_sentences_type.__name__=="str":
             return openai.embeddings.create(input = [sentences], model=EMBEDDING_MODEL)['data'][0]['embedding']
         embeddings=[]
         def split_list(input_list, n):
```

### Comparing `LLM_Mediator-0.9.8/llm_mediator/llm.py` & `LLM_Mediator-0.9.9/llm_mediator/llm.py`

 * *Files identical despite different names*

### Comparing `LLM_Mediator-0.9.8/llm_mediator/parallel_tasks_queuer.py` & `LLM_Mediator-0.9.9/llm_mediator/parallel_tasks_queuer.py`

 * *Files identical despite different names*

### Comparing `LLM_Mediator-0.9.8/setup.py` & `LLM_Mediator-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 NAME = 'LLM_Mediator'
 DESCRIPTION = 'Just a simple mediator for different LLM models.'
 URL = 'https://github.com/zeuscsc/llm_mediator.git'
 EMAIL = 'zeuscsc@gmail.com'
 AUTHOR = 'Zeus Chiu'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.9.8'
+VERSION = '0.9.9'
 
 with open('requirements.txt') as f:
     required_packages = f.readlines()
     required_packages = [pkg.strip() for pkg in required_packages]
 
 EXTRAS = {
 }
```

