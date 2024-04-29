# Comparing `tmp/shipyard_snowflake-0.2.4.tar.gz` & `tmp/shipyard_snowflake-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_snowflake-0.2.4.tar", max compression
+gzip compressed data, was "shipyard_snowflake-0.2.5.tar", max compression
```

## Comparing `shipyard_snowflake-0.2.4.tar` & `shipyard_snowflake-0.2.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3302 2024-03-08 19:26:38.998001 shipyard_snowflake-0.2.4/README.md
--rw-r--r--   0        0        0      851 2024-04-25 03:17:27.631966 shipyard_snowflake-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      140 2024-03-08 19:26:38.999894 shipyard_snowflake-0.2.4/shipyard_snowflake/__init__.py
--rw-r--r--   0        0        0        0 2024-03-08 19:26:38.999947 shipyard_snowflake-0.2.4/shipyard_snowflake/cli/__init__.py
--rw-r--r--   0        0        0      606 2024-03-08 19:26:39.000305 shipyard_snowflake-0.2.4/shipyard_snowflake/cli/authtest.py
--rw-r--r--   0        0        0     2388 2024-03-08 19:26:39.000532 shipyard_snowflake-0.2.4/shipyard_snowflake/cli/execute_sql.py
--rw-r--r--   0        0        0     3896 2024-03-08 19:26:39.000783 shipyard_snowflake-0.2.4/shipyard_snowflake/cli/fetch.py
--rw-r--r--   0        0        0     8755 2024-03-08 19:26:39.001114 shipyard_snowflake-0.2.4/shipyard_snowflake/cli/upload.py
--rw-r--r--   0        0        0    11150 2024-04-25 03:17:21.305242 shipyard_snowflake-0.2.4/shipyard_snowflake/snowflake.py
--rw-r--r--   0        0        0     4448 2023-10-07 02:13:54.059430 shipyard_snowflake-0.2.4/shipyard_snowflake/snowpark.py
--rw-r--r--   0        0        0     2109 2024-03-08 19:26:39.001675 shipyard_snowflake-0.2.4/shipyard_snowflake/test/snowflake_test.py
--rw-r--r--   0        0        0     2023 2023-10-07 02:13:54.060283 shipyard_snowflake-0.2.4/shipyard_snowflake/test/snowpark_test.py
--rw-r--r--   0        0        0     1846 2024-03-08 19:26:39.001946 shipyard_snowflake-0.2.4/shipyard_snowflake/test/tests.py
--rw-r--r--   0        0        0     1795 2024-03-08 19:26:39.002454 shipyard_snowflake-0.2.4/shipyard_snowflake/utils/exceptions.py
--rw-r--r--   0        0        0     9674 2024-03-08 19:26:39.002564 shipyard_snowflake-0.2.4/shipyard_snowflake/utils/utils.py
--rw-r--r--   0        0        0     4091 1970-01-01 00:00:00.000000 shipyard_snowflake-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     3302 2024-03-08 19:26:38.998001 shipyard_snowflake-0.2.5/README.md
+-rw-r--r--   0        0        0      851 2024-04-29 17:31:01.846747 shipyard_snowflake-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      140 2024-03-08 19:26:38.999894 shipyard_snowflake-0.2.5/shipyard_snowflake/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-08 19:26:38.999947 shipyard_snowflake-0.2.5/shipyard_snowflake/cli/__init__.py
+-rw-r--r--   0        0        0      606 2024-03-08 19:26:39.000305 shipyard_snowflake-0.2.5/shipyard_snowflake/cli/authtest.py
+-rw-r--r--   0        0        0     2388 2024-03-08 19:26:39.000532 shipyard_snowflake-0.2.5/shipyard_snowflake/cli/execute_sql.py
+-rw-r--r--   0        0        0     3896 2024-03-08 19:26:39.000783 shipyard_snowflake-0.2.5/shipyard_snowflake/cli/fetch.py
+-rw-r--r--   0        0        0     8755 2024-03-08 19:26:39.001114 shipyard_snowflake-0.2.5/shipyard_snowflake/cli/upload.py
+-rw-r--r--   0        0        0    11152 2024-04-29 17:30:56.681352 shipyard_snowflake-0.2.5/shipyard_snowflake/snowflake.py
+-rw-r--r--   0        0        0     4448 2023-10-07 02:13:54.059430 shipyard_snowflake-0.2.5/shipyard_snowflake/snowpark.py
+-rw-r--r--   0        0        0     2109 2024-03-08 19:26:39.001675 shipyard_snowflake-0.2.5/shipyard_snowflake/test/snowflake_test.py
+-rw-r--r--   0        0        0     2023 2023-10-07 02:13:54.060283 shipyard_snowflake-0.2.5/shipyard_snowflake/test/snowpark_test.py
+-rw-r--r--   0        0        0     1846 2024-03-08 19:26:39.001946 shipyard_snowflake-0.2.5/shipyard_snowflake/test/tests.py
+-rw-r--r--   0        0        0     1795 2024-03-08 19:26:39.002454 shipyard_snowflake-0.2.5/shipyard_snowflake/utils/exceptions.py
+-rw-r--r--   0        0        0     9674 2024-03-08 19:26:39.002564 shipyard_snowflake-0.2.5/shipyard_snowflake/utils/utils.py
+-rw-r--r--   0        0        0     4091 1970-01-01 00:00:00.000000 shipyard_snowflake-0.2.5/PKG-INFO
```

### Comparing `shipyard_snowflake-0.2.4/README.md` & `shipyard_snowflake-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.2.4/pyproject.toml` & `shipyard_snowflake-0.2.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-snowflake"
-version = "0.2.4"
+version = "0.2.5"
 description = "A local client for conecting and working with Snowflake"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 packages = [{include = "shipyard_snowflake"}]
 
 [tool.poetry.dependencies]
```

### Comparing `shipyard_snowflake-0.2.4/shipyard_snowflake/cli/authtest.py` & `shipyard_snowflake-0.2.5/shipyard_snowflake/cli/authtest.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.2.4/shipyard_snowflake/cli/execute_sql.py` & `shipyard_snowflake-0.2.5/shipyard_snowflake/cli/execute_sql.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.2.4/shipyard_snowflake/cli/fetch.py` & `shipyard_snowflake-0.2.5/shipyard_snowflake/cli/fetch.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.2.4/shipyard_snowflake/cli/upload.py` & `shipyard_snowflake-0.2.5/shipyard_snowflake/cli/upload.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.2.4/shipyard_snowflake/snowflake.py` & `shipyard_snowflake-0.2.5/shipyard_snowflake/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                     user=self.username,
                     account=self.account,
                     private_key=private_key,
                     warehouse=self.warehouse,
                     database=self.database,
                     schema=self.schema,
                     role=self.role,
-                    application = self.application
+                    application=self.application,
                 )
                 logger.info("Successfully connected to Snowflake")
                 self.conn = con
                 return con
             except Exception as e:
                 raise ExitCodeException(
                     message=f"Could not authenticate to Snowflake for user {self.username} with credentials in {self.rsa_key}",
@@ -93,15 +93,15 @@
                     user=self.username,
                     password=self.password,
                     account=self.account,
                     warehouse=self.warehouse,
                     database=self.database,
                     schema=self.schema,
                     role=self.role,
-                    application = self.application
+                    application=self.application,
                 )
                 logger.info("Successfully connected to snowflake")
                 self.conn = con
                 return con
             except Exception as e:
                 raise ExitCodeException(
                     f"Could not authenticate to Snowflake due to {e}",
@@ -238,17 +238,17 @@
         """Returns the SQL for to create or replace a table in Snowflake
         Args:
             table_name (str): The name of the table to create
             columns (List[List[str,str]]): A list of lists of the column name and the data type. Example: [("column1","varchar(100)"),("column2","varchar(100)")]. Defaults to None
         """
         # this is for backwards compatibility
         if isinstance(columns, list):
-            column_string = ",".join([f"{col[0]} {col[1]}" for col in columns])
+            column_string = ",".join([f'"{col[0]}" {col[1]}' for col in columns])
         else:
-            column_string = ",".join([f"{k} {v}" for k, v in columns.items()])
+            column_string = ",".join([f'"{k}" {v}' for k, v in columns.items()])
 
         create_statement = f"""CREATE OR REPLACE TABLE {table_name} ({column_string})"""
         return create_statement
 
     def create_table(self, sql: str):
         """Helper function to create a table in Snowflake
```

### Comparing `shipyard_snowflake-0.2.4/shipyard_snowflake/snowpark.py` & `shipyard_snowflake-0.2.5/shipyard_snowflake/snowpark.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.2.4/shipyard_snowflake/test/snowflake_test.py` & `shipyard_snowflake-0.2.5/shipyard_snowflake/test/snowflake_test.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.2.4/shipyard_snowflake/test/snowpark_test.py` & `shipyard_snowflake-0.2.5/shipyard_snowflake/test/snowpark_test.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.2.4/shipyard_snowflake/test/tests.py` & `shipyard_snowflake-0.2.5/shipyard_snowflake/test/tests.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.2.4/shipyard_snowflake/utils/exceptions.py` & `shipyard_snowflake-0.2.5/shipyard_snowflake/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.2.4/shipyard_snowflake/utils/utils.py` & `shipyard_snowflake-0.2.5/shipyard_snowflake/utils/utils.py`

 * *Files identical despite different names*

### Comparing `shipyard_snowflake-0.2.4/PKG-INFO` & `shipyard_snowflake-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-snowflake
-Version: 0.2.4
+Version: 0.2.5
 Summary: A local client for conecting and working with Snowflake
 License: Apache 2.0
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

