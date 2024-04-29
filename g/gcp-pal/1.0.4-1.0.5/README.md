# Comparing `tmp/gcp_pal-1.0.4.tar.gz` & `tmp/gcp_pal-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp_pal-1.0.4.tar", max compression
+gzip compressed data, was "gcp_pal-1.0.5.tar", max compression
```

## Comparing `gcp_pal-1.0.4.tar` & `gcp_pal-1.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    25169 2024-04-27 23:17:45.290956 gcp_pal-1.0.4/README.md
--rw-r--r--   0        0        0      810 2024-04-27 23:17:45.290956 gcp_pal-1.0.4/gcp_pal/__init__.py
--rw-r--r--   0        0        0    31402 2024-04-27 23:17:45.290956 gcp_pal-1.0.4/gcp_pal/bigquery.py
--rw-r--r--   0        0        0    13156 2024-04-27 23:17:45.290956 gcp_pal-1.0.4/gcp_pal/cloudfunctions.py
--rw-r--r--   0        0        0    13855 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/cloudrun.py
--rw-r--r--   0        0        0     7754 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/cloudscheduler.py
--rw-r--r--   0        0        0       42 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/config/__init__.py
--rw-r--r--   0        0        0      965 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/config/vars.py
--rw-r--r--   0        0        0    12490 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/firestore.py
--rw-r--r--   0        0        0     3170 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/project.py
--rw-r--r--   0        0        0     1674 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/pubsub.py
--rw-r--r--   0        0        0     3873 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/pydocker.py
--rw-r--r--   0        0        0     6860 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/pylogging.py
--rw-r--r--   0        0        0     4737 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/request.py
--rw-r--r--   0        0        0    23631 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/schema.py
--rw-r--r--   0        0        0     6332 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/secretmanager.py
--rw-r--r--   0        0        0       88 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/storage/__init__.py
--rw-r--r--   0        0        0     8735 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/storage/parquet.py
--rw-r--r--   0        0        0    17133 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/storage/storage.py
--rw-r--r--   0        0        0       82 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/utils/__init__.py
--rw-r--r--   0        0        0      935 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/utils/lazy_loader.py
--rw-r--r--   0        0        0    11431 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/gcp_pal/utils/utils.py
--rw-r--r--   0        0        0      958 2024-04-27 23:17:45.294956 gcp_pal-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    25559 1970-01-01 00:00:00.000000 gcp_pal-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    25169 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/README.md
+-rw-r--r--   0        0        0      810 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/__init__.py
+-rw-r--r--   0        0        0    31402 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/bigquery.py
+-rw-r--r--   0        0        0    13156 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/cloudfunctions.py
+-rw-r--r--   0        0        0    13855 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/cloudrun.py
+-rw-r--r--   0        0        0     7754 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/cloudscheduler.py
+-rw-r--r--   0        0        0       42 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/config/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/config/vars.py
+-rw-r--r--   0        0        0    12490 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/firestore.py
+-rw-r--r--   0        0        0     3170 2024-04-29 08:11:37.221001 gcp_pal-1.0.5/gcp_pal/project.py
+-rw-r--r--   0        0        0     1674 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/pubsub.py
+-rw-r--r--   0        0        0     3873 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/pydocker.py
+-rw-r--r--   0        0        0     6975 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/pylogging.py
+-rw-r--r--   0        0        0     4737 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/request.py
+-rw-r--r--   0        0        0    23631 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/schema.py
+-rw-r--r--   0        0        0     6332 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/secretmanager.py
+-rw-r--r--   0        0        0       88 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/storage/__init__.py
+-rw-r--r--   0        0        0     8735 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/storage/parquet.py
+-rw-r--r--   0        0        0    17133 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/storage/storage.py
+-rw-r--r--   0        0        0       82 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/utils/__init__.py
+-rw-r--r--   0        0        0      935 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/utils/lazy_loader.py
+-rw-r--r--   0        0        0    11431 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/gcp_pal/utils/utils.py
+-rw-r--r--   0        0        0      958 2024-04-29 08:11:37.225000 gcp_pal-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    25559 1970-01-01 00:00:00.000000 gcp_pal-1.0.5/PKG-INFO
```

### Comparing `gcp_pal-1.0.4/README.md` & `gcp_pal-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/__init__.py` & `gcp_pal-1.0.5/gcp_pal/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/bigquery.py` & `gcp_pal-1.0.5/gcp_pal/bigquery.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/cloudfunctions.py` & `gcp_pal-1.0.5/gcp_pal/cloudfunctions.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/cloudrun.py` & `gcp_pal-1.0.5/gcp_pal/cloudrun.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/cloudscheduler.py` & `gcp_pal-1.0.5/gcp_pal/cloudscheduler.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/config/vars.py` & `gcp_pal-1.0.5/gcp_pal/config/vars.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     "google.cloud.bigquery": "google-cloud-bigquery",
     "google.cloud.firestore": "google-cloud-firestore",
     "google.cloud.functions_v1": "google-cloud-functions",
     "google.cloud.functions_v2": "google-cloud-functions",
     "google.cloud.scheduler_v1": "google-cloud-scheduler",
     "google.cloud.secretmanager": "google-cloud-secret-manager",
     "google.cloud.resource_manager": "google-cloud-resource-manager",
+    "google.cloud.resourcemanager_v3": "google-cloud-resource-manager",
     "google.cloud.run_v1": "google-cloud-run",
     "google.cloud.run_v2": "google-cloud-run",
     "gcsfs": "gcsfs",
     "pyarrow": "pyarrow",
     "pandas": "pandas",
     "pandas_gbq": "pandas-gbq",
     "docker": "docker",
```

### Comparing `gcp_pal-1.0.4/gcp_pal/firestore.py` & `gcp_pal-1.0.5/gcp_pal/firestore.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/project.py` & `gcp_pal-1.0.5/gcp_pal/project.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/pubsub.py` & `gcp_pal-1.0.5/gcp_pal/pubsub.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/pydocker.py` & `gcp_pal-1.0.5/gcp_pal/pydocker.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/pylogging.py` & `gcp_pal-1.0.5/gcp_pal/pylogging.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,16 @@
         - (list[dict]): List of log entries
         """
         if time_range:
             time_end = datetime.datetime.now(datetime.timezone.utc)
             time_start = time_end - datetime.timedelta(hours=time_range)
         query = self._generate_query(query, severity, time_start, time_end)
         log(f"Logging - Filter: {query}")
+        if limit is None and query is None:
+            limit = 100
         logs = self.client.list_entries(
             filter_=query, max_results=limit, order_by=order_by
         )
         output = []
         for log_entry in logs:
             output.append(
                 LogEntry(
@@ -190,12 +192,13 @@
         if time_end:
             if not isinstance(time_end, str):
                 time_end = time_end.isoformat()
             filter_str = f'timestamp<="{time_end}"'
             self.filters.append(filter_str)
         query = " AND ".join(self.filters)
         self.filters = []  # Reset filters
+        query = None if query == "" else query
         return query
 
 
 if __name__ == "__main__":
     Logging().stream()
```

### Comparing `gcp_pal-1.0.4/gcp_pal/request.py` & `gcp_pal-1.0.5/gcp_pal/request.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/schema.py` & `gcp_pal-1.0.5/gcp_pal/schema.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/secretmanager.py` & `gcp_pal-1.0.5/gcp_pal/secretmanager.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/storage/parquet.py` & `gcp_pal-1.0.5/gcp_pal/storage/parquet.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/storage/storage.py` & `gcp_pal-1.0.5/gcp_pal/storage/storage.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/utils/lazy_loader.py` & `gcp_pal-1.0.5/gcp_pal/utils/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/gcp_pal/utils/utils.py` & `gcp_pal-1.0.5/gcp_pal/utils/utils.py`

 * *Files identical despite different names*

### Comparing `gcp_pal-1.0.4/pyproject.toml` & `gcp_pal-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcp-pal"
-version = "1.0.4"
+version = "1.0.5"
 description = ""
 authors = ["VitaminB16 <artemiy.nosov@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gcp_pal-1.0.4/PKG-INFO` & `gcp_pal-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-pal
-Version: 1.0.4
+Version: 1.0.5
 Summary: 
 Author: VitaminB16
 Author-email: artemiy.nosov@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

