# Comparing `tmp/SPLADERunner-0.1.4.tar.gz` & `tmp/SPLADERunner-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPLADERunner-0.1.4.tar", last modified: Thu Apr 25 04:50:57 2024, max compression
+gzip compressed data, was "SPLADERunner-0.1.5.tar", last modified: Mon Apr 29 18:58:37 2024, max compression
```

## Comparing `SPLADERunner-0.1.4.tar` & `SPLADERunner-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-25 04:50:57.901768 SPLADERunner-0.1.4/
--rw-r--r--   0 prithivida   (501) staff       (20)     4684 2024-04-25 04:50:57.901654 SPLADERunner-0.1.4/PKG-INFO
--rw-r--r--   0 prithivida   (501) staff       (20)     4127 2024-02-17 05:49:13.000000 SPLADERunner-0.1.4/README.md
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-25 04:50:57.900923 SPLADERunner-0.1.4/SPLADERunner.egg-info/
--rw-r--r--   0 prithivida   (501) staff       (20)     4684 2024-04-25 04:50:57.000000 SPLADERunner-0.1.4/SPLADERunner.egg-info/PKG-INFO
--rw-r--r--   0 prithivida   (501) staff       (20)      270 2024-04-25 04:50:57.000000 SPLADERunner-0.1.4/SPLADERunner.egg-info/SOURCES.txt
--rw-r--r--   0 prithivida   (501) staff       (20)        1 2024-04-25 04:50:57.000000 SPLADERunner-0.1.4/SPLADERunner.egg-info/dependency_links.txt
--rw-r--r--   0 prithivida   (501) staff       (20)       47 2024-04-25 04:50:57.000000 SPLADERunner-0.1.4/SPLADERunner.egg-info/requires.txt
--rw-r--r--   0 prithivida   (501) staff       (20)       13 2024-04-25 04:50:57.000000 SPLADERunner-0.1.4/SPLADERunner.egg-info/top_level.txt
--rw-r--r--   0 prithivida   (501) staff       (20)       38 2024-04-25 04:50:57.901806 SPLADERunner-0.1.4/setup.cfg
--rw-r--r--   0 prithivida   (501) staff       (20)      882 2024-04-25 04:50:03.000000 SPLADERunner-0.1.4/setup.py
-drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-25 04:50:57.901381 SPLADERunner-0.1.4/spladerunner/
--rw-r--r--   0 prithivida   (501) staff       (20)      196 2024-04-25 04:49:03.000000 SPLADERunner-0.1.4/spladerunner/Config.py
--rw-r--r--   0 prithivida   (501) staff       (20)     6765 2024-02-21 10:54:20.000000 SPLADERunner-0.1.4/spladerunner/Expander.py
--rw-r--r--   0 prithivida   (501) staff       (20)       30 2024-02-16 16:58:15.000000 SPLADERunner-0.1.4/spladerunner/__init__.py
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-29 18:58:37.604096 SPLADERunner-0.1.5/
+-rw-r--r--   0 prithivida   (501) staff       (20)     4963 2024-04-29 18:58:37.603947 SPLADERunner-0.1.5/PKG-INFO
+-rw-r--r--   0 prithivida   (501) staff       (20)     4406 2024-04-29 18:57:11.000000 SPLADERunner-0.1.5/README.md
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-29 18:58:37.603072 SPLADERunner-0.1.5/SPLADERunner.egg-info/
+-rw-r--r--   0 prithivida   (501) staff       (20)     4963 2024-04-29 18:58:37.000000 SPLADERunner-0.1.5/SPLADERunner.egg-info/PKG-INFO
+-rw-r--r--   0 prithivida   (501) staff       (20)      270 2024-04-29 18:58:37.000000 SPLADERunner-0.1.5/SPLADERunner.egg-info/SOURCES.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)        1 2024-04-29 18:58:37.000000 SPLADERunner-0.1.5/SPLADERunner.egg-info/dependency_links.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)       47 2024-04-29 18:58:37.000000 SPLADERunner-0.1.5/SPLADERunner.egg-info/requires.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)       13 2024-04-29 18:58:37.000000 SPLADERunner-0.1.5/SPLADERunner.egg-info/top_level.txt
+-rw-r--r--   0 prithivida   (501) staff       (20)       38 2024-04-29 18:58:37.604143 SPLADERunner-0.1.5/setup.cfg
+-rw-r--r--   0 prithivida   (501) staff       (20)      882 2024-04-29 18:55:14.000000 SPLADERunner-0.1.5/setup.py
+drwxr-xr-x   0 prithivida   (501) staff       (20)        0 2024-04-29 18:58:37.603656 SPLADERunner-0.1.5/spladerunner/
+-rw-r--r--   0 prithivida   (501) staff       (20)      196 2024-04-25 04:49:03.000000 SPLADERunner-0.1.5/spladerunner/Config.py
+-rw-r--r--   0 prithivida   (501) staff       (20)     6888 2024-04-29 18:56:49.000000 SPLADERunner-0.1.5/spladerunner/Expander.py
+-rw-r--r--   0 prithivida   (501) staff       (20)       30 2024-02-16 16:58:15.000000 SPLADERunner-0.1.5/spladerunner/__init__.py
```

### Comparing `SPLADERunner-0.1.4/PKG-INFO` & `SPLADERunner-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPLADERunner
-Version: 0.1.4
+Version: 0.1.5
 Summary: Ultralight and Fast wrapper for the independent implementation of SPLADE++ models for your search & retrieval pipelines. Models and Library created by Prithivi Da, For PRs and Collaboration to checkout the readme.
 Home-page: https://github.com/PrithivirajDamodaran/SPLADERunner
 Author: Prithivi Da
 Author-email: 
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,19 @@
 
 # One-time only init
 from spladerunner import Expander
 expander = Expander('Splade_PP_en_v1', 128) #pass model, max_seq_len
 
 # Sample passage expansion
 sparse_rep = expander.expand("The Manhattan Project and its atomic bomb helped bring an end to World War II. Its legacy of peaceful uses of atomic energy continues to have an impact on history and science.")
+
+
+# For solr or elastic or vanilla lucene stores.
+sparse_rep = expander.expand("The Manhattan Project and its atomic bomb helped bring an end to World War II. Its legacy of peaceful uses of atomic energy continues to have an impact on history and science.", outformat="lucene")
+
 print(sparse_rep)
 
 ```
 
 (Feel free to skip to 3 If you are expert in sparse and dense representations)
 
 ## 2. Why Sparse Representations?
```

### Comparing `SPLADERunner-0.1.4/README.md` & `SPLADERunner-0.1.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,19 @@
 
 # One-time only init
 from spladerunner import Expander
 expander = Expander('Splade_PP_en_v1', 128) #pass model, max_seq_len
 
 # Sample passage expansion
 sparse_rep = expander.expand("The Manhattan Project and its atomic bomb helped bring an end to World War II. Its legacy of peaceful uses of atomic energy continues to have an impact on history and science.")
+
+
+# For solr or elastic or vanilla lucene stores.
+sparse_rep = expander.expand("The Manhattan Project and its atomic bomb helped bring an end to World War II. Its legacy of peaceful uses of atomic energy continues to have an impact on history and science.", outformat="lucene")
+
 print(sparse_rep)
 
 ```
 
 (Feel free to skip to 3 If you are expert in sparse and dense representations)
 
 ## 2. Why Sparse Representations?
```

### Comparing `SPLADERunner-0.1.4/SPLADERunner.egg-info/PKG-INFO` & `SPLADERunner-0.1.5/SPLADERunner.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPLADERunner
-Version: 0.1.4
+Version: 0.1.5
 Summary: Ultralight and Fast wrapper for the independent implementation of SPLADE++ models for your search & retrieval pipelines. Models and Library created by Prithivi Da, For PRs and Collaboration to checkout the readme.
 Home-page: https://github.com/PrithivirajDamodaran/SPLADERunner
 Author: Prithivi Da
 Author-email: 
 License: Apache 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,19 @@
 
 # One-time only init
 from spladerunner import Expander
 expander = Expander('Splade_PP_en_v1', 128) #pass model, max_seq_len
 
 # Sample passage expansion
 sparse_rep = expander.expand("The Manhattan Project and its atomic bomb helped bring an end to World War II. Its legacy of peaceful uses of atomic energy continues to have an impact on history and science.")
+
+
+# For solr or elastic or vanilla lucene stores.
+sparse_rep = expander.expand("The Manhattan Project and its atomic bomb helped bring an end to World War II. Its legacy of peaceful uses of atomic energy continues to have an impact on history and science.", outformat="lucene")
+
 print(sparse_rep)
 
 ```
 
 (Feel free to skip to 3 If you are expert in sparse and dense representations)
 
 ## 2. Why Sparse Representations?
```

### Comparing `SPLADERunner-0.1.4/setup.py` & `SPLADERunner-0.1.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SPLADERunner', 
-    version='0.1.4', 
+    version='0.1.5', 
     packages=find_packages(),
     install_requires=[
         'tokenizers',
         'onnxruntime-gpu',
         'numpy',
         'requests',
         'tqdm'
```

### Comparing `SPLADERunner-0.1.4/spladerunner/Expander.py` & `SPLADERunner-0.1.5/spladerunner/Expander.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
           
         providers = self.session.get_providers()
         print(f"Using {providers[0]}")
         self.tokenizer = self._get_tokenizer(max_length)
 
         # self.session = ort.InferenceSession(self.cache_dir / model_name / model_file)
         # self.tokenizer = self._get_tokenizer(max_length)
-        # self.reverse_voc = {v: k for k, v in self.tokenizer.get_vocab().items()}
+        self.reverse_voc = {v: k for k, v in self.tokenizer.get_vocab().items()}
 
     def _download_model_files(self, model_name):
         
         # The local file path to which the file should be downloaded
         local_zip_file = self.cache_dir / f"{model_name}.zip"
 
         formatted_model_url = MODEL_URL.format(model_name)
@@ -119,15 +119,15 @@
         # vocab_file = self.model_dir / "vocab.txt"
         # if vocab_file.exists():
         #     tokenizer.vocab = self._load_vocab(vocab_file)
         #     tokenizer.ids_to_tokens = collections.OrderedDict([(ids, tok) for tok, ids in tokenizer.vocab.items()])                
 
         return tokenizer
     
-    def expand(self, request):
+    def expand(self, request, outformat="hybrid"):
         
         if isinstance(request, str):
             plain_input = [request]
         else:
             plain_input = request
 
         encoded_input = self.tokenizer.encode_batch(plain_input)
@@ -159,23 +159,24 @@
             # Find max values for the current example
             max_val = np.max(single_weighted_log, axis=0)
 
             # Find non-zero columns for the current example
             example_cols = np.nonzero(max_val)[0]
             weights = max_val[example_cols].tolist()
 
-            sparse_representations.append({"indices": example_cols.tolist(), "values": weights})
-
-        # Create dictionary and sort it
-        # d = dict(zip(cols, weights))
-        # sorted_d = dict(sorted(d.items(), key=lambda item: item[1], reverse=True))
-
-        # # Construct SPLADE BoW representation for the current sentence
-        # sparse_representation = {self.reverse_voc[k]: round(v, 2) for k, v in sorted_d.items()}
-        # sparse_representations.append(sparse_representation)
+            if outformat == "lucene":
+                # Create dictionary and sort it
+                d = dict(zip(example_cols, weights))
+                sorted_d = dict(sorted(d.items(), key=lambda item: item[1], reverse=True))
+
+                # Construct SPLADE BoW representation for the current sentence
+                sparse_representation = {self.reverse_voc[k]: round(v, 2) for k, v in sorted_d.items()}
+                sparse_representations.append(sparse_representation)
+            else:
+                sparse_representations.append({"indices": example_cols.tolist(), "values": weights})
 
         return sparse_representations
```

