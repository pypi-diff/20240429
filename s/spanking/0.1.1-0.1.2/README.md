# Comparing `tmp/spanking-0.1.1.tar.gz` & `tmp/spanking-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spanking-0.1.1.tar", last modified: Mon Apr 15 12:15:55 2024, max compression
+gzip compressed data, was "spanking-0.1.2.tar", last modified: Sun Apr 28 23:27:18 2024, max compression
```

## Comparing `spanking-0.1.1.tar` & `spanking-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:15:55.670854 spanking-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 12:15:46.000000 spanking-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-15 12:15:55.670854 spanking-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-04-15 12:15:46.000000 spanking-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 12:15:55.670854 spanking-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-15 12:15:46.000000 spanking-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:15:55.670854 spanking-0.1.1/spanking/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-15 12:15:55.000000 spanking-0.1.1/spanking/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 12:15:46.000000 spanking-0.1.1/spanking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-15 12:15:46.000000 spanking-0.1.1/spanking/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-15 12:15:46.000000 spanking-0.1.1/spanking/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 12:15:55.670854 spanking-0.1.1/spanking.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-15 12:15:55.000000 spanking-0.1.1/spanking.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-15 12:15:55.000000 spanking-0.1.1/spanking.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 12:15:55.000000 spanking-0.1.1/spanking.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-15 12:15:55.000000 spanking-0.1.1/spanking.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-15 12:15:55.000000 spanking-0.1.1/spanking.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 12:15:55.000000 spanking-0.1.1/spanking.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:27:18.282821 spanking-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-28 23:27:09.000000 spanking-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-28 23:27:18.282821 spanking-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-04-28 23:27:09.000000 spanking-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-28 23:27:18.282821 spanking-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-28 23:27:09.000000 spanking-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:27:18.278821 spanking-0.1.2/spanking/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-28 23:27:18.000000 spanking-0.1.2/spanking/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-28 23:27:09.000000 spanking-0.1.2/spanking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-28 23:27:09.000000 spanking-0.1.2/spanking/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-28 23:27:09.000000 spanking-0.1.2/spanking/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 23:27:18.278821 spanking-0.1.2/spanking.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4512 2024-04-28 23:27:18.000000 spanking-0.1.2/spanking.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-28 23:27:18.000000 spanking-0.1.2/spanking.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 23:27:18.000000 spanking-0.1.2/spanking.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-28 23:27:18.000000 spanking-0.1.2/spanking.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-28 23:27:18.000000 spanking-0.1.2/spanking.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-28 23:27:18.000000 spanking-0.1.2/spanking.egg-info/top_level.txt
```

### Comparing `spanking-0.1.1/LICENSE` & `spanking-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spanking-0.1.1/PKG-INFO` & `spanking-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: spanking
-Version: 0.1.1
+Version: 0.1.2
 Summary: 🍑👋
 Home-page: https://github.com/rishiraj/spanking
 Author: Rishiraj Acharya
 Author-email: heyrishiraj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jax==0.4.26
-Requires-Dist: sentence-transformers==2.6.1
+Requires-Dist: sentence-transformers==2.7.0
 Requires-Dist: pandas==2.0.3
+Requires-Dist: transformers==4.40.1
+Requires-Dist: Pillow==9.4.0
+Requires-Dist: requests==2.31.0
 
 # spanking 🍑👋
 
 To use the 🍑👋 `VectorDB` class, you can follow these steps:
 
 1. Create an instance of the 🍑👋 `VectorDB` class:
 ```python
@@ -29,21 +32,29 @@
 2. Add texts to the database:
 ```python
 texts = ["i eat pizza", "i play chess", "i drive bus"]
 vector_db.add_texts(texts)
 ```
 This will encode the texts into embeddings and store them in the database.
 
-3. Search for similar texts:
+3. Search for similar texts or images:
 ```python
-query = "we play football"
-top_results = vector_db.search(query, top_k=3)
-print(top_results)
+text_query = "we play football"
+text_results = vector_db.search(text_query, top_k=2, type='text')
+print("Text search results:")
+for text, similarity in text_results:
+    print(f"Text: {text}, Similarity: {similarity}")
+
+image_url = "https://example.com/image.jpg"
+image_results = vector_db.search(image_url, top_k=2, type='image')
+print("\nImage search results:")
+for text, similarity in image_results:
+    print(f"Text: {text}, Similarity: {similarity}")
 ```
-This will retrieve the top-3 most similar texts to the query based on cosine similarity. The `search` method returns a list of tuples, where each tuple contains the text and its similarity score.
+This will retrieve the top-2 most similar texts or images to the query based on cosine similarity. The `search` method returns a list of tuples, where each tuple contains the text and its similarity score. You can specify the search type using the `type` parameter (`'text'` for text search and `'image'` for image search).
 
 4. Delete a text from the database:
 ```python
 index = 1
 vector_db.delete_text(index)
 ```
 This will remove the text and its corresponding embedding at the specified index.
@@ -64,30 +75,36 @@
 
 7. Load the database from a file:
 ```python
 vector_db = VectorDB.load('vector_db.pkl')
 ```
 This will load the `VectorDB` instance from the file named 'vector_db.pkl' and return it.
 
-8. Iterate over the stored texts:
+8. Convert the database to a Pandas Dataframe
+```python
+df = vector_db.to_df()
+```
+This will convert the current state of the `VectorDB` instance to a Pandas Dataframe.
+
+9. Iterate over the stored texts:
 ```python
 for text in vector_db:
     print(text)
 ```
 This will iterate over all the texts stored in the database.
 
-9. Access individual texts by index:
+10. Access individual texts by index:
 ```python
 index = 2
 text = vector_db[index]
 print(text)
 ```
 This will retrieve the text at the specified index.
 
-10. Get the number of texts in the database:
+11. Get the number of texts in the database:
 ```python
 num_texts = len(vector_db)
 print(num_texts)
 ```
 This will return the number of texts currently stored in the database.
 
 Here's an example usage of the 🍑👋 `VectorDB` class:
@@ -119,10 +136,14 @@
 # Load the database
 loaded_vector_db = VectorDB.load('vector_db.pkl')
 
 # Iterate over the stored texts in the loaded database
 print("\nStored texts in the loaded database:")
 for text in loaded_vector_db:
     print(text)
+
+# Convert to dataframe
+df = loaded_vector_db.to_df()
+print(df.head())
 ```
 
 This example demonstrates how to create a 🍑👋 `VectorDB` instance, add texts, search for similar texts, update and delete texts, and iterate over the stored texts.
```

### Comparing `spanking-0.1.1/README.md` & `spanking-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -12,21 +12,29 @@
 2. Add texts to the database:
 ```python
 texts = ["i eat pizza", "i play chess", "i drive bus"]
 vector_db.add_texts(texts)
 ```
 This will encode the texts into embeddings and store them in the database.
 
-3. Search for similar texts:
+3. Search for similar texts or images:
 ```python
-query = "we play football"
-top_results = vector_db.search(query, top_k=3)
-print(top_results)
+text_query = "we play football"
+text_results = vector_db.search(text_query, top_k=2, type='text')
+print("Text search results:")
+for text, similarity in text_results:
+    print(f"Text: {text}, Similarity: {similarity}")
+
+image_url = "https://example.com/image.jpg"
+image_results = vector_db.search(image_url, top_k=2, type='image')
+print("\nImage search results:")
+for text, similarity in image_results:
+    print(f"Text: {text}, Similarity: {similarity}")
 ```
-This will retrieve the top-3 most similar texts to the query based on cosine similarity. The `search` method returns a list of tuples, where each tuple contains the text and its similarity score.
+This will retrieve the top-2 most similar texts or images to the query based on cosine similarity. The `search` method returns a list of tuples, where each tuple contains the text and its similarity score. You can specify the search type using the `type` parameter (`'text'` for text search and `'image'` for image search).
 
 4. Delete a text from the database:
 ```python
 index = 1
 vector_db.delete_text(index)
 ```
 This will remove the text and its corresponding embedding at the specified index.
@@ -47,30 +55,36 @@
 
 7. Load the database from a file:
 ```python
 vector_db = VectorDB.load('vector_db.pkl')
 ```
 This will load the `VectorDB` instance from the file named 'vector_db.pkl' and return it.
 
-8. Iterate over the stored texts:
+8. Convert the database to a Pandas Dataframe
+```python
+df = vector_db.to_df()
+```
+This will convert the current state of the `VectorDB` instance to a Pandas Dataframe.
+
+9. Iterate over the stored texts:
 ```python
 for text in vector_db:
     print(text)
 ```
 This will iterate over all the texts stored in the database.
 
-9. Access individual texts by index:
+10. Access individual texts by index:
 ```python
 index = 2
 text = vector_db[index]
 print(text)
 ```
 This will retrieve the text at the specified index.
 
-10. Get the number of texts in the database:
+11. Get the number of texts in the database:
 ```python
 num_texts = len(vector_db)
 print(num_texts)
 ```
 This will return the number of texts currently stored in the database.
 
 Here's an example usage of the 🍑👋 `VectorDB` class:
@@ -102,10 +116,14 @@
 # Load the database
 loaded_vector_db = VectorDB.load('vector_db.pkl')
 
 # Iterate over the stored texts in the loaded database
 print("\nStored texts in the loaded database:")
 for text in loaded_vector_db:
     print(text)
+
+# Convert to dataframe
+df = loaded_vector_db.to_df()
+print(df.head())
 ```
 
-This example demonstrates how to create a 🍑👋 `VectorDB` instance, add texts, search for similar texts, update and delete texts, and iterate over the stored texts.
+This example demonstrates how to create a 🍑👋 `VectorDB` instance, add texts, search for similar texts, update and delete texts, and iterate over the stored texts.
```

### Comparing `spanking-0.1.1/setup.py` & `spanking-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `spanking-0.1.1/spanking.egg-info/PKG-INFO` & `spanking-0.1.2/spanking.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: spanking
-Version: 0.1.1
+Version: 0.1.2
 Summary: 🍑👋
 Home-page: https://github.com/rishiraj/spanking
 Author: Rishiraj Acharya
 Author-email: heyrishiraj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jax==0.4.26
-Requires-Dist: sentence-transformers==2.6.1
+Requires-Dist: sentence-transformers==2.7.0
 Requires-Dist: pandas==2.0.3
+Requires-Dist: transformers==4.40.1
+Requires-Dist: Pillow==9.4.0
+Requires-Dist: requests==2.31.0
 
 # spanking 🍑👋
 
 To use the 🍑👋 `VectorDB` class, you can follow these steps:
 
 1. Create an instance of the 🍑👋 `VectorDB` class:
 ```python
@@ -29,21 +32,29 @@
 2. Add texts to the database:
 ```python
 texts = ["i eat pizza", "i play chess", "i drive bus"]
 vector_db.add_texts(texts)
 ```
 This will encode the texts into embeddings and store them in the database.
 
-3. Search for similar texts:
+3. Search for similar texts or images:
 ```python
-query = "we play football"
-top_results = vector_db.search(query, top_k=3)
-print(top_results)
+text_query = "we play football"
+text_results = vector_db.search(text_query, top_k=2, type='text')
+print("Text search results:")
+for text, similarity in text_results:
+    print(f"Text: {text}, Similarity: {similarity}")
+
+image_url = "https://example.com/image.jpg"
+image_results = vector_db.search(image_url, top_k=2, type='image')
+print("\nImage search results:")
+for text, similarity in image_results:
+    print(f"Text: {text}, Similarity: {similarity}")
 ```
-This will retrieve the top-3 most similar texts to the query based on cosine similarity. The `search` method returns a list of tuples, where each tuple contains the text and its similarity score.
+This will retrieve the top-2 most similar texts or images to the query based on cosine similarity. The `search` method returns a list of tuples, where each tuple contains the text and its similarity score. You can specify the search type using the `type` parameter (`'text'` for text search and `'image'` for image search).
 
 4. Delete a text from the database:
 ```python
 index = 1
 vector_db.delete_text(index)
 ```
 This will remove the text and its corresponding embedding at the specified index.
@@ -64,30 +75,36 @@
 
 7. Load the database from a file:
 ```python
 vector_db = VectorDB.load('vector_db.pkl')
 ```
 This will load the `VectorDB` instance from the file named 'vector_db.pkl' and return it.
 
-8. Iterate over the stored texts:
+8. Convert the database to a Pandas Dataframe
+```python
+df = vector_db.to_df()
+```
+This will convert the current state of the `VectorDB` instance to a Pandas Dataframe.
+
+9. Iterate over the stored texts:
 ```python
 for text in vector_db:
     print(text)
 ```
 This will iterate over all the texts stored in the database.
 
-9. Access individual texts by index:
+10. Access individual texts by index:
 ```python
 index = 2
 text = vector_db[index]
 print(text)
 ```
 This will retrieve the text at the specified index.
 
-10. Get the number of texts in the database:
+11. Get the number of texts in the database:
 ```python
 num_texts = len(vector_db)
 print(num_texts)
 ```
 This will return the number of texts currently stored in the database.
 
 Here's an example usage of the 🍑👋 `VectorDB` class:
@@ -119,10 +136,14 @@
 # Load the database
 loaded_vector_db = VectorDB.load('vector_db.pkl')
 
 # Iterate over the stored texts in the loaded database
 print("\nStored texts in the loaded database:")
 for text in loaded_vector_db:
     print(text)
+
+# Convert to dataframe
+df = loaded_vector_db.to_df()
+print(df.head())
 ```
 
 This example demonstrates how to create a 🍑👋 `VectorDB` instance, add texts, search for similar texts, update and delete texts, and iterate over the stored texts.
```

