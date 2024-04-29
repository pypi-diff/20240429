# Comparing `tmp/askquinta-2.0.8.tar.gz` & `tmp/askquinta-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askquinta-2.0.8.tar", last modified: Mon Apr 29 05:02:43 2024, max compression
+gzip compressed data, was "askquinta-2.0.9.tar", last modified: Mon Apr 29 10:33:34 2024, max compression
```

## Comparing `askquinta-2.0.8.tar` & `askquinta-2.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 05:02:43.415348 askquinta-2.0.8/
--rw-rw-rw-   0        0        0     1074 2024-04-29 04:57:00.000000 askquinta-2.0.8/LICENSE
--rw-rw-rw-   0        0        0    12233 2024-04-29 05:02:43.414347 askquinta-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    11522 2024-04-29 04:57:00.000000 askquinta-2.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-29 05:02:43.383052 askquinta-2.0.8/askquinta/
-drwxrwxrwx   0        0        0        0 2024-04-29 05:02:43.393284 askquinta-2.0.8/askquinta/ETL/
--rw-rw-rw-   0        0        0    11533 2024-04-29 04:57:00.000000 askquinta-2.0.8/askquinta/ETL/NLP.py
--rw-rw-rw-   0        0        0      247 2024-04-29 04:57:00.000000 askquinta-2.0.8/askquinta/ETL/__init__.py
--rw-rw-rw-   0        0        0      409 2024-04-29 04:58:40.000000 askquinta-2.0.8/askquinta/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 05:02:43.397282 askquinta-2.0.8/askquinta/blastmessage/
--rw-rw-rw-   0        0        0     8154 2024-04-29 04:57:00.000000 askquinta-2.0.8/askquinta/blastmessage/Blast_Message.py
--rw-rw-rw-   0        0        0      276 2024-04-29 04:57:00.000000 askquinta-2.0.8/askquinta/blastmessage/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 05:02:43.405287 askquinta-2.0.8/askquinta/connector/
--rw-rw-rw-   0        0        0     1253 2024-04-29 04:57:00.000000 askquinta-2.0.8/askquinta/connector/API.py
--rw-rw-rw-   0        0        0     6148 2024-04-29 04:57:00.000000 askquinta-2.0.8/askquinta/connector/ArangoDB.py
--rw-rw-rw-   0        0        0     5752 2024-04-29 04:57:00.000000 askquinta-2.0.8/askquinta/connector/MySQL.py
--rw-rw-rw-   0        0        0      322 2024-04-29 04:57:00.000000 askquinta-2.0.8/askquinta/connector/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 05:02:43.412347 askquinta-2.0.8/askquinta/google/
--rw-rw-rw-   0        0        0     6863 2024-04-29 05:00:18.000000 askquinta-2.0.8/askquinta/google/BQ.py
--rw-rw-rw-   0        0        0     5627 2024-04-29 04:57:00.000000 askquinta-2.0.8/askquinta/google/Gsheet.py
--rw-rw-rw-   0        0        0      281 2024-04-29 04:57:00.000000 askquinta-2.0.8/askquinta/google/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 05:02:43.389561 askquinta-2.0.8/askquinta.egg-info/
--rw-rw-rw-   0        0        0    12233 2024-04-29 05:02:43.000000 askquinta-2.0.8/askquinta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2024-04-29 05:02:43.000000 askquinta-2.0.8/askquinta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 05:02:43.000000 askquinta-2.0.8/askquinta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-29 05:02:43.000000 askquinta-2.0.8/askquinta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      775 2024-04-29 04:58:01.000000 askquinta-2.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 05:02:43.416348 askquinta-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1111 2024-04-29 04:57:10.000000 askquinta-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:33:34.545162 askquinta-2.0.9/
+-rw-rw-rw-   0        0        0     1074 2024-04-29 04:57:00.000000 askquinta-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0    12233 2024-04-29 10:33:34.543174 askquinta-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11522 2024-04-29 04:57:00.000000 askquinta-2.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-29 10:33:34.471193 askquinta-2.0.9/askquinta/
+drwxrwxrwx   0        0        0        0 2024-04-29 10:33:34.498483 askquinta-2.0.9/askquinta/ETL/
+-rw-rw-rw-   0        0        0    11533 2024-04-29 04:57:00.000000 askquinta-2.0.9/askquinta/ETL/NLP.py
+-rw-rw-rw-   0        0        0      247 2024-04-29 04:57:00.000000 askquinta-2.0.9/askquinta/ETL/__init__.py
+-rw-rw-rw-   0        0        0      409 2024-04-29 10:32:23.000000 askquinta-2.0.9/askquinta/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:33:34.506952 askquinta-2.0.9/askquinta/blastmessage/
+-rw-rw-rw-   0        0        0     8154 2024-04-29 04:57:00.000000 askquinta-2.0.9/askquinta/blastmessage/Blast_Message.py
+-rw-rw-rw-   0        0        0      276 2024-04-29 04:57:00.000000 askquinta-2.0.9/askquinta/blastmessage/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:33:34.525479 askquinta-2.0.9/askquinta/connector/
+-rw-rw-rw-   0        0        0     1253 2024-04-29 04:57:00.000000 askquinta-2.0.9/askquinta/connector/API.py
+-rw-rw-rw-   0        0        0     6258 2024-04-29 10:33:12.000000 askquinta-2.0.9/askquinta/connector/ArangoDB.py
+-rw-rw-rw-   0        0        0     5752 2024-04-29 04:57:00.000000 askquinta-2.0.9/askquinta/connector/MySQL.py
+-rw-rw-rw-   0        0        0      322 2024-04-29 04:57:00.000000 askquinta-2.0.9/askquinta/connector/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:33:34.536381 askquinta-2.0.9/askquinta/google/
+-rw-rw-rw-   0        0        0     6863 2024-04-29 05:00:18.000000 askquinta-2.0.9/askquinta/google/BQ.py
+-rw-rw-rw-   0        0        0     5627 2024-04-29 04:57:00.000000 askquinta-2.0.9/askquinta/google/Gsheet.py
+-rw-rw-rw-   0        0        0      281 2024-04-29 04:57:00.000000 askquinta-2.0.9/askquinta/google/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-29 10:33:34.487777 askquinta-2.0.9/askquinta.egg-info/
+-rw-rw-rw-   0        0        0    12233 2024-04-29 10:33:34.000000 askquinta-2.0.9/askquinta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2024-04-29 10:33:34.000000 askquinta-2.0.9/askquinta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 10:33:34.000000 askquinta-2.0.9/askquinta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-29 10:33:34.000000 askquinta-2.0.9/askquinta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      775 2024-04-29 10:32:07.000000 askquinta-2.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 10:33:34.546182 askquinta-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1111 2024-04-29 10:31:56.000000 askquinta-2.0.9/setup.py
```

### Comparing `askquinta-2.0.8/LICENSE` & `askquinta-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `askquinta-2.0.8/PKG-INFO` & `askquinta-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askquinta
-Version: 2.0.8
+Version: 2.0.9
 Summary: Package for daily usage of data team at Paper.id
 Home-page: https://github.com/paper-indonesia/composer
 Author: Paper Data Team
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `askquinta-2.0.8/README.md` & `askquinta-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `askquinta-2.0.8/askquinta/ETL/NLP.py` & `askquinta-2.0.9/askquinta/ETL/NLP.py`

 * *Files identical despite different names*

### Comparing `askquinta-2.0.8/askquinta/blastmessage/Blast_Message.py` & `askquinta-2.0.9/askquinta/blastmessage/Blast_Message.py`

 * *Files identical despite different names*

### Comparing `askquinta-2.0.8/askquinta/connector/API.py` & `askquinta-2.0.9/askquinta/connector/API.py`

 * *Files identical despite different names*

### Comparing `askquinta-2.0.8/askquinta/connector/ArangoDB.py` & `askquinta-2.0.9/askquinta/connector/ArangoDB.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,20 @@
         """
         # Try to connect
         if not self.connection:
             self.connect()
         collection_connection = self.connection[collection_name]
         # Config the connection
         query_result = collection_connection.AQLQuery(query, batchSize = int(batch_size)).response['result']
-        return pd.json_normalize(query_result, max_level=max_level)
+        
+        try:
+            return pd.json_normalize(query_result, max_level=max_level)
+        except Exception as e:
+            print(e)
+            return query_result
 
     def to_push_data(self, data, database_name, collection_name):
         """
         Push data to a specified collection in a given database.
 
         Args:
             data (pd.DataFrame): Data to push as a DataFrame.
```

### Comparing `askquinta-2.0.8/askquinta/connector/MySQL.py` & `askquinta-2.0.9/askquinta/connector/MySQL.py`

 * *Files identical despite different names*

### Comparing `askquinta-2.0.8/askquinta/google/BQ.py` & `askquinta-2.0.9/askquinta/google/BQ.py`

 * *Files identical despite different names*

### Comparing `askquinta-2.0.8/askquinta/google/Gsheet.py` & `askquinta-2.0.9/askquinta/google/Gsheet.py`

 * *Files identical despite different names*

### Comparing `askquinta-2.0.8/askquinta.egg-info/PKG-INFO` & `askquinta-2.0.9/askquinta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: askquinta
-Version: 2.0.8
+Version: 2.0.9
 Summary: Package for daily usage of data team at Paper.id
 Home-page: https://github.com/paper-indonesia/composer
 Author: Paper Data Team
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `askquinta-2.0.8/askquinta.egg-info/SOURCES.txt` & `askquinta-2.0.9/askquinta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `askquinta-2.0.8/pyproject.toml` & `askquinta-2.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "askquinta"
-version = "2.0.8"
+version = "2.0.9"
 description = "Package for data team Paper.id"
 authors = ["Data Team <data.drive@paper.id>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.2"
 # timeout_decorator = ">=0.5.0"
```

### Comparing `askquinta-2.0.8/setup.py` & `askquinta-2.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='askquinta',                # Package name
-    version='2.0.8',                   # Package version
+    version='2.0.9',                   # Package version
     packages=find_packages(),        # Automatically find all packages and sub-packages
     #install_requires=required_packages,  # Required dependencies listed in requirements.txt
     author='Paper Data Team',        # Author name
     description='Package for daily usage of data team at Paper.id',  # Package description
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/paper-indonesia/composer',  # Package URL or project repository URL
```

