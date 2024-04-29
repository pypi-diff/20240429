# Comparing `tmp/airflow_providers_wherobots-0.1.0.tar.gz` & `tmp/airflow_providers_wherobots-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_providers_wherobots-0.1.0.tar", max compression
+gzip compressed data, was "airflow_providers_wherobots-0.1.1.tar", max compression
```

## Comparing `airflow_providers_wherobots-0.1.0.tar` & `airflow_providers_wherobots-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-04-18 07:26:43.078861 airflow_providers_wherobots-0.1.0/LICENSE
--rw-r--r--   0        0        0     1999 2024-04-24 08:50:05.479191 airflow_providers_wherobots-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-16 06:44:10.398877 airflow_providers_wherobots-0.1.0/airflow_providers_wherobots/__init__.py
--rw-r--r--   0        0        0        0 2024-04-12 09:19:52.194210 airflow_providers_wherobots-0.1.0/airflow_providers_wherobots/hooks/__init__.py
--rw-r--r--   0        0        0     1873 2024-04-18 07:47:53.367508 airflow_providers_wherobots-0.1.0/airflow_providers_wherobots/hooks/sql.py
--rw-r--r--   0        0        0       57 2024-04-16 09:03:11.283716 airflow_providers_wherobots-0.1.0/airflow_providers_wherobots/hooks/wherobots.py
--rw-r--r--   0        0        0        0 2024-04-12 09:19:58.480236 airflow_providers_wherobots-0.1.0/airflow_providers_wherobots/operators/__init__.py
--rw-r--r--   0        0        0     2000 2024-04-18 07:46:38.306518 airflow_providers_wherobots-0.1.0/airflow_providers_wherobots/operators/sql.py
--rw-r--r--   0        0        0      568 2024-04-18 02:00:20.478005 airflow_providers_wherobots-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2624 1970-01-01 00:00:00.000000 airflow_providers_wherobots-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2441 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/hooks/__init__.py
+-rw-r--r--   0        0        0     1873 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/hooks/sql.py
+-rw-r--r--   0        0        0       57 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/hooks/wherobots.py
+-rw-r--r--   0        0        0        0 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/operators/__init__.py
+-rw-r--r--   0        0        0     2000 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/operators/sql.py
+-rw-r--r--   0        0        0      492 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 airflow_providers_wherobots-0.1.1/PKG-INFO
```

### Comparing `airflow_providers_wherobots-0.1.0/LICENSE` & `airflow_providers_wherobots-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_providers_wherobots-0.1.0/README.md` & `airflow_providers_wherobots-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,26 @@
-# Airflow Wherobots Provider
+Metadata-Version: 2.1
+Name: airflow-providers-wherobots
+Version: 0.1.1
+Summary: Airflow extension for communicating with Wherobots Cloud
+Author: zongsi.zhang
+Author-email: zongsi@wherobots.com
+Requires-Python: >=3.9,<3.13
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: wherobots-python-dbapi (>=0.4.0,<0.5.0)
+Description-Content-Type: text/markdown
 
-Airflow Provider that integrates [wherobots cloud](https://wherobots.com/)'s computation features into your workflows.
+# Airflow Providers for Wherobots
+
+Airflow providers to bring [Wherobots Cloud](https://www.wherobots.com)'s
+spatial compute to your data workflows and ETLs.
 
 ## Installation
 
 If you use [Poetry](https://python-poetry.org) in your project, add the
 dependency with `poetry add`:
 
 ```
@@ -15,46 +31,70 @@
 
 ```
 $ pip install git+https://github.com/wherobots/airflow-providers-wherobots
 ```
 
 ## Usage
 
-### Create Connection
-Create a connection first, the default wherobots connection name is `wherobots_default`.
-For any other name, please pass in the `wherobots_conn_id` parameter when initializing Wherobots Operators.
-Fill in the following fields in the connection detail page:
-1. Fill the wherobots API Service endpoint into the `Host` field
-2. Fill the personal API Token into the `Password` field
-
-### Execute SQL query
-You can use the `WherobotsSqlOperator` to run SQL queries on the Wherobots cloud.
-You can build your ETL jobs on Wherobots Catalogs.
-Check this [guidance](https://docs.wherobots.services/1.2.2/tutorials/sedonadb/vector-data/vector-load/) to learn how to **read data, transformation and write results by pure SQL in Wherobots Cloud**.  
-Below is an example dag that executes SQL query on Wherobots Cloud 
+### Create a connection
+
+You first need to create a Connection in Airflow. This can be done from
+the UI, or from the command-line. The default Wherobots connection name
+is `wherobots_default`; if you use another name you must specify that
+name with the `wherobots_conn_id` parameter when initializing Wherobots
+operators.
+
+The only required fields for the connection are:
+- the Wherobots API endpoint in the `host` field;
+- your Wherobots API key in the `password` field.
+
+```
+$ airflow connections add "wherobots_default" \
+    --conn-type "wherobots" \
+    --conn-host "api.cloud.wherobots.com" \
+    --conn-password "$(< api.key)"
+```
+
+### Execute a SQL query
+
+The `WherobotsSqlOperator` allows you to run SQL queries on the
+Wherobots cloud, from which you can build your ETLs and data
+transformation workflows by querying, manipulating, and producing
+datasets with WherobotsDB.
+
+Refer to the [Wherobots Documentation](https://docs.wherobots.com) and
+this [guidance](https://docs.wherobots.services/1.2.2/tutorials/sedonadb/vector-data/vector-load/)
+to learn how to read data, transform data, and write results in Spatial
+SQL with WherobotsDB.
+
+## Example
+
+Below is an example Airflow DAG that executes a SQL query on Wherobots
+Cloud:
+
 ```python
 import datetime
 
 from airflow import DAG
 from airflow_providers_wherobots.operators.sql import WherobotsSqlOperator
 
 
 with DAG(
     dag_id="example_wherobots_sql_dag",
-    start_date=datetime.datetime(2024, 1, 1),
+    start_date=datetime.datetime.date(datetime.datetime.now()),
     schedule="@hourly",
     catchup=False
 ):
-    # operator = PythonOperator(task_id="print_the_context", python_callable=print_context)
+    # Create a `wherobots.test.airflow_example` table with 100 records
+    # from the OMF `places_place` dataset.
     operator = WherobotsSqlOperator(
         task_id="execute_query",
         sql=f"""
-        INSERT INTO
-            wherobots.test_db.example_geom
-        SELECT
-            id, geometry, confidence, geohash
-        FROM
-            wherobots_open_data.overture.places_place
+        INSERT INTO wherobots.test.airflow_example
+        SELECT id, geometry, confidence, geohash
+        FROM wherobots_open_data.overture.places_place
+        LIMIT 100
         """,
         return_last=False,
     )
 ```
+
```

### Comparing `airflow_providers_wherobots-0.1.0/airflow_providers_wherobots/hooks/sql.py` & `airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/hooks/sql.py`

 * *Files identical despite different names*

### Comparing `airflow_providers_wherobots-0.1.0/airflow_providers_wherobots/operators/sql.py` & `airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/operators/sql.py`

 * *Files identical despite different names*

