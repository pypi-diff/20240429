# Comparing `tmp/chainmeta-0.0.3.tar.gz` & `tmp/chainmeta-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainmeta-0.0.3.tar", last modified: Wed Apr 17 20:55:56 2024, max compression
+gzip compressed data, was "chainmeta-0.0.4.tar", last modified: Mon Apr 29 03:33:14 2024, max compression
```

## Comparing `chainmeta-0.0.3.tar` & `chainmeta-0.0.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.807409 chainmeta-0.0.3/
--rw-r--r--   0 zhanwu     (501) staff       (20)    11357 2024-04-10 07:26:37.000000 chainmeta-0.0.3/LICENSE
--rw-r--r--   0 zhanwu     (501) staff       (20)     1581 2024-04-17 20:55:56.807243 chainmeta-0.0.3/PKG-INFO
--rw-r--r--   0 zhanwu     (501) staff       (20)      988 2024-04-10 07:26:37.000000 chainmeta-0.0.3/README.md
--rw-r--r--   0 zhanwu     (501) staff       (20)      784 2024-04-17 20:55:04.000000 chainmeta-0.0.3/pyproject.toml
--rw-r--r--   0 zhanwu     (501) staff       (20)       38 2024-04-17 20:55:56.807447 chainmeta-0.0.3/setup.cfg
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.802389 chainmeta-0.0.3/src/
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.804174 chainmeta-0.0.3/src/chainmeta/
--rw-r--r--   0 zhanwu     (501) staff       (20)     4925 2024-04-17 20:55:04.000000 chainmeta-0.0.3/src/chainmeta/__init__.py
--rw-r--r--   0 zhanwu     (501) staff       (20)     2746 2024-04-17 20:02:26.000000 chainmeta-0.0.3/src/chainmeta/artifact.py
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.805557 chainmeta-0.0.3/src/chainmeta/config/
--rw-r--r--   0 zhanwu     (501) staff       (20)     3510 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/config/__init__.py
--rw-r--r--   0 zhanwu     (501) staff       (20)    20519 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/config/categories.json
--rw-r--r--   0 zhanwu     (501) staff       (20)     2679 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/config/chains.json
--rw-r--r--   0 zhanwu     (501) staff       (20)    43396 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/config/entities.json
--rw-r--r--   0 zhanwu     (501) staff       (20)      404 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/config/sources.json
--rw-r--r--   0 zhanwu     (501) staff       (20)      979 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/constants.py
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.806090 chainmeta-0.0.3/src/chainmeta/contrib/
--rw-r--r--   0 zhanwu     (501) staff       (20)     4529 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/contrib/chaintool.py
--rw-r--r--   0 zhanwu     (501) staff       (20)     1342 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/contrib/chaintool_schema.json
--rw-r--r--   0 zhanwu     (501) staff       (20)     1293 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/contrib/messari.py
--rw-r--r--   0 zhanwu     (501) staff       (20)      423 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/contrib/messari_schema.json
--rw-r--r--   0 zhanwu     (501) staff       (20)    15395 2024-04-17 20:11:06.000000 chainmeta-0.0.3/src/chainmeta/db.py
--rw-r--r--   0 zhanwu     (501) staff       (20)      664 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/logger.py
--rw-r--r--   0 zhanwu     (501) staff       (20)     1979 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/metadata.py
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.806476 chainmeta-0.0.3/src/chainmeta/schema/
--rw-r--r--   0 zhanwu     (501) staff       (20)     2743 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/schema/__init__.py
--rw-r--r--   0 zhanwu     (501) staff       (20)     3320 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/schema/artifact_schema.json
--rw-r--r--   0 zhanwu     (501) staff       (20)     4124 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/schema/meta_schema.json
--rw-r--r--   0 zhanwu     (501) staff       (20)     2332 2024-04-10 07:26:37.000000 chainmeta-0.0.3/src/chainmeta/validator.py
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.807064 chainmeta-0.0.3/src/chainmeta.egg-info/
--rw-r--r--   0 zhanwu     (501) staff       (20)     1581 2024-04-17 20:55:56.000000 chainmeta-0.0.3/src/chainmeta.egg-info/PKG-INFO
--rw-r--r--   0 zhanwu     (501) staff       (20)      901 2024-04-17 20:55:56.000000 chainmeta-0.0.3/src/chainmeta.egg-info/SOURCES.txt
--rw-r--r--   0 zhanwu     (501) staff       (20)        1 2024-04-17 20:55:56.000000 chainmeta-0.0.3/src/chainmeta.egg-info/dependency_links.txt
--rw-r--r--   0 zhanwu     (501) staff       (20)       45 2024-04-17 20:55:56.000000 chainmeta-0.0.3/src/chainmeta.egg-info/requires.txt
--rw-r--r--   0 zhanwu     (501) staff       (20)       10 2024-04-17 20:55:56.000000 chainmeta-0.0.3/src/chainmeta.egg-info/top_level.txt
-drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-17 20:55:56.806884 chainmeta-0.0.3/tests/
--rw-r--r--   0 zhanwu     (501) staff       (20)      715 2024-04-10 07:26:37.000000 chainmeta-0.0.3/tests/test_config.py
--rw-r--r--   0 zhanwu     (501) staff       (20)     1738 2024-04-10 07:26:37.000000 chainmeta-0.0.3/tests/test_translator.py
--rw-r--r--   0 zhanwu     (501) staff       (20)     1600 2024-04-10 07:26:37.000000 chainmeta-0.0.3/tests/test_validator.py
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.578966 chainmeta-0.0.4/
+-rw-r--r--   0 zhanwu     (501) staff       (20)    11357 2024-04-10 07:26:37.000000 chainmeta-0.0.4/LICENSE
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1581 2024-04-29 03:33:14.578775 chainmeta-0.0.4/PKG-INFO
+-rw-r--r--   0 zhanwu     (501) staff       (20)      988 2024-04-10 07:26:37.000000 chainmeta-0.0.4/README.md
+-rw-r--r--   0 zhanwu     (501) staff       (20)      784 2024-04-29 03:32:06.000000 chainmeta-0.0.4/pyproject.toml
+-rw-r--r--   0 zhanwu     (501) staff       (20)       38 2024-04-29 03:33:14.579009 chainmeta-0.0.4/setup.cfg
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.574494 chainmeta-0.0.4/src/
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.576075 chainmeta-0.0.4/src/chainmeta/
+-rw-r--r--   0 zhanwu     (501) staff       (20)     4925 2024-04-29 02:33:52.000000 chainmeta-0.0.4/src/chainmeta/__init__.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     2746 2024-04-29 03:06:44.000000 chainmeta-0.0.4/src/chainmeta/artifact.py
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.577264 chainmeta-0.0.4/src/chainmeta/config/
+-rw-r--r--   0 zhanwu     (501) staff       (20)     3510 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/config/__init__.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)    20519 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/config/categories.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)     2679 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/config/chains.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)    43396 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/config/entities.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)      404 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/config/sources.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)      979 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/constants.py
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.577724 chainmeta-0.0.4/src/chainmeta/contrib/
+-rw-r--r--   0 zhanwu     (501) staff       (20)     4529 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/contrib/chaintool.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1342 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/contrib/chaintool_schema.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1293 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/contrib/messari.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)      423 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/contrib/messari_schema.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)    15594 2024-04-29 03:32:06.000000 chainmeta-0.0.4/src/chainmeta/db.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)      664 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/logger.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1979 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/metadata.py
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.578081 chainmeta-0.0.4/src/chainmeta/schema/
+-rw-r--r--   0 zhanwu     (501) staff       (20)     2743 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/schema/__init__.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     3320 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/schema/artifact_schema.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)     4124 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/schema/meta_schema.json
+-rw-r--r--   0 zhanwu     (501) staff       (20)     2332 2024-04-10 07:26:37.000000 chainmeta-0.0.4/src/chainmeta/validator.py
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.578587 chainmeta-0.0.4/src/chainmeta.egg-info/
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1581 2024-04-29 03:33:14.000000 chainmeta-0.0.4/src/chainmeta.egg-info/PKG-INFO
+-rw-r--r--   0 zhanwu     (501) staff       (20)      901 2024-04-29 03:33:14.000000 chainmeta-0.0.4/src/chainmeta.egg-info/SOURCES.txt
+-rw-r--r--   0 zhanwu     (501) staff       (20)        1 2024-04-29 03:33:14.000000 chainmeta-0.0.4/src/chainmeta.egg-info/dependency_links.txt
+-rw-r--r--   0 zhanwu     (501) staff       (20)       45 2024-04-29 03:33:14.000000 chainmeta-0.0.4/src/chainmeta.egg-info/requires.txt
+-rw-r--r--   0 zhanwu     (501) staff       (20)       10 2024-04-29 03:33:14.000000 chainmeta-0.0.4/src/chainmeta.egg-info/top_level.txt
+drwxr-xr-x   0 zhanwu     (501) staff       (20)        0 2024-04-29 03:33:14.578430 chainmeta-0.0.4/tests/
+-rw-r--r--   0 zhanwu     (501) staff       (20)      715 2024-04-10 07:26:37.000000 chainmeta-0.0.4/tests/test_config.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1738 2024-04-10 07:26:37.000000 chainmeta-0.0.4/tests/test_translator.py
+-rw-r--r--   0 zhanwu     (501) staff       (20)     1600 2024-04-10 07:26:37.000000 chainmeta-0.0.4/tests/test_validator.py
```

### Comparing `chainmeta-0.0.3/LICENSE` & `chainmeta-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/PKG-INFO` & `chainmeta-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainmeta
-Version: 0.0.3
+Version: 0.0.4
 Summary: Onchain metadata exchange protocol
 Project-URL: Homepage, https://github.com/microscopexyz/chainmeta-core
 Project-URL: Issues, https://github.com/microscopexyz/chainmeta-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `chainmeta-0.0.3/README.md` & `chainmeta-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/pyproject.toml` & `chainmeta-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chainmeta"
-version = "0.0.3"
+version = "0.0.4"
 authors = []
 description = "Onchain metadata exchange protocol"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `chainmeta-0.0.3/src/chainmeta/__init__.py` & `chainmeta-0.0.4/src/chainmeta/__init__.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta/artifact.py` & `chainmeta-0.0.4/src/chainmeta/artifact.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta/config/__init__.py` & `chainmeta-0.0.4/src/chainmeta/config/__init__.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta/config/categories.json` & `chainmeta-0.0.4/src/chainmeta/config/categories.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta/config/chains.json` & `chainmeta-0.0.4/src/chainmeta/config/chains.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta/config/entities.json` & `chainmeta-0.0.4/src/chainmeta/config/entities.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta/constants.py` & `chainmeta-0.0.4/src/chainmeta/constants.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta/contrib/chaintool.py` & `chainmeta-0.0.4/src/chainmeta/contrib/chaintool.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta/contrib/chaintool_schema.json` & `chainmeta-0.0.4/src/chainmeta/contrib/chaintool_schema.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta/contrib/messari.py` & `chainmeta-0.0.4/src/chainmeta/contrib/messari.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta/db.py` & `chainmeta-0.0.4/src/chainmeta/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,15 +275,18 @@
     for v in metadata_groups.values():
         reduced_list += _build_meta(v)
     return reduced_list
 
 
 @unsync
 def _upload_chainmeta_single_batch(
-    session_maker: Callable, items: Iterable[ChainmetaItem], *, skip_check: bool
+    session_maker: Callable,
+    items: Iterable[ChainmetaItem] | Iterable[ChainmetaRecord],
+    *,
+    skip_check: bool,
 ) -> int:
     """Upload a single batch of chain metadata to database."""
 
     with session_maker() as session:
 
         def _find_exist_item(record):
             """Check if the record already exists in the database."""
@@ -304,15 +307,19 @@
                     .first()
                 )
                 return found
 
         skipped = 0
         total = 0
         for item in items:
-            for record in flatten([item]):
+            if isinstance(item, ChainmetaItem):
+                recods = flatten([item])
+            else:
+                recods = [item]
+            for record in recods:
                 total += 1
                 exist_item = _find_exist_item(record)
                 if exist_item:
                     for key, value in item.__dict__.items():
                         setattr(exist_item, key, value)
                 else:
                     session.add(record)
@@ -323,15 +330,15 @@
             session.rollback()
             logger.error(e)
             return 0
         return total
 
 
 def upload_chainmeta(
-    items: Iterable[ChainmetaItem],
+    items: Iterable[ChainmetaItem] | Iterable[ChainmetaRecord],
     *,
     batch_size: int = 200,
     max_concurrency: int = 10,
     skip_check: bool = False,
 ) -> int:
     """Upload chain metadata to database.
```

### Comparing `chainmeta-0.0.3/src/chainmeta/logger.py` & `chainmeta-0.0.4/src/chainmeta/logger.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta/metadata.py` & `chainmeta-0.0.4/src/chainmeta/metadata.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta/schema/__init__.py` & `chainmeta-0.0.4/src/chainmeta/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta/schema/artifact_schema.json` & `chainmeta-0.0.4/src/chainmeta/schema/artifact_schema.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta/schema/meta_schema.json` & `chainmeta-0.0.4/src/chainmeta/schema/meta_schema.json`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta/validator.py` & `chainmeta-0.0.4/src/chainmeta/validator.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/src/chainmeta.egg-info/PKG-INFO` & `chainmeta-0.0.4/src/chainmeta.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainmeta
-Version: 0.0.3
+Version: 0.0.4
 Summary: Onchain metadata exchange protocol
 Project-URL: Homepage, https://github.com/microscopexyz/chainmeta-core
 Project-URL: Issues, https://github.com/microscopexyz/chainmeta-core/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
```

### Comparing `chainmeta-0.0.3/src/chainmeta.egg-info/SOURCES.txt` & `chainmeta-0.0.4/src/chainmeta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/tests/test_config.py` & `chainmeta-0.0.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/tests/test_translator.py` & `chainmeta-0.0.4/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `chainmeta-0.0.3/tests/test_validator.py` & `chainmeta-0.0.4/tests/test_validator.py`

 * *Files identical despite different names*

