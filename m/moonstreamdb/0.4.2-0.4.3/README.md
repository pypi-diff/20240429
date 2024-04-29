# Comparing `tmp/moonstreamdb-0.4.2.tar.gz` & `tmp/moonstreamdb-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonstreamdb-0.4.2.tar", last modified: Wed Apr 17 12:59:52 2024, max compression
+gzip compressed data, was "moonstreamdb-0.4.3.tar", last modified: Mon Apr 29 13:44:40 2024, max compression
```

## Comparing `moonstreamdb-0.4.2.tar` & `moonstreamdb-0.4.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:59:52.294269 moonstreamdb-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-17 12:59:52.294269 moonstreamdb-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:59:52.294269 moonstreamdb-0.4.2/moonstreamdb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11634 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    65038 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/moonstreamdb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 12:59:52.294269 moonstreamdb-0.4.2/moonstreamdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-17 12:59:51.000000 moonstreamdb-0.4.2/moonstreamdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-17 12:59:52.000000 moonstreamdb-0.4.2/moonstreamdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:59:51.000000 moonstreamdb-0.4.2/moonstreamdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-17 12:59:51.000000 moonstreamdb-0.4.2/moonstreamdb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 12:59:39.000000 moonstreamdb-0.4.2/moonstreamdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-17 12:59:51.000000 moonstreamdb-0.4.2/moonstreamdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-17 12:59:51.000000 moonstreamdb-0.4.2/moonstreamdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 12:59:52.294269 moonstreamdb-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-17 12:59:33.000000 moonstreamdb-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:44:40.032055 moonstreamdb-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-29 13:44:40.032055 moonstreamdb-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:44:40.032055 moonstreamdb-0.4.3/moonstreamdb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11634 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65236 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:44:40.032055 moonstreamdb-0.4.3/moonstreamdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-29 13:44:39.000000 moonstreamdb-0.4.3/moonstreamdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-29 13:44:39.000000 moonstreamdb-0.4.3/moonstreamdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:44:39.000000 moonstreamdb-0.4.3/moonstreamdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 13:44:39.000000 moonstreamdb-0.4.3/moonstreamdb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:44:27.000000 moonstreamdb-0.4.3/moonstreamdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 13:44:39.000000 moonstreamdb-0.4.3/moonstreamdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 13:44:39.000000 moonstreamdb-0.4.3/moonstreamdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:44:40.032055 moonstreamdb-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/setup.py
```

### Comparing `moonstreamdb-0.4.2/PKG-INFO` & `moonstreamdb-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb
-Version: 0.4.2
+Version: 0.4.3
 Summary: Moonstream database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstream db
```

### Comparing `moonstreamdb-0.4.2/README.md` & `moonstreamdb-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.4.2/moonstreamdb/blockchain.py` & `moonstreamdb-0.4.3/moonstreamdb/blockchain.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.4.2/moonstreamdb/cli.py` & `moonstreamdb-0.4.3/moonstreamdb/cli.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.4.2/moonstreamdb/db.py` & `moonstreamdb-0.4.3/moonstreamdb/db.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.4.2/moonstreamdb/models.py` & `moonstreamdb-0.4.3/moonstreamdb/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     MetaData,
     Numeric,
     Text,
 )
 from sqlalchemy.dialects.postgresql import JSONB, UUID
 from sqlalchemy.ext.compiler import compiles
 from sqlalchemy.ext.declarative import declarative_base
-from sqlalchemy.sql import expression
+from sqlalchemy.sql import expression, text
 
 """
 Naming conventions doc
 https://docs.sqlalchemy.org/en/13/core/constraints.html#configuring-constraint-naming-conventions
 """
 convention = {
     "ix": "ix_%(column_0_label)s",
@@ -755,14 +755,20 @@
         ),
         Index(
             "ix_zksync_era_labels_address_block_timestamp",
             "address",
             "block_timestamp",
             unique=False,
         ),
+        Index(
+            "ix_zksync_era_labels_address_label_data_name",
+            "address",
+            text("(label_data ->> 'name')"),
+            postgresql_using="btree",
+        ),
     )
 
     id = Column(
         UUID(as_uuid=True),
         primary_key=True,
         default=uuid.uuid4,
         unique=True,
```

### Comparing `moonstreamdb-0.4.2/moonstreamdb/networks.py` & `moonstreamdb-0.4.3/moonstreamdb/networks.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.4.2/moonstreamdb/subscriptions.py` & `moonstreamdb-0.4.3/moonstreamdb/subscriptions.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.4.2/moonstreamdb.egg-info/PKG-INFO` & `moonstreamdb-0.4.3/moonstreamdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb
-Version: 0.4.2
+Version: 0.4.3
 Summary: Moonstream database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstream db
```

### Comparing `moonstreamdb-0.4.2/setup.py` & `moonstreamdb-0.4.3/setup.py`

 * *Files identical despite different names*

