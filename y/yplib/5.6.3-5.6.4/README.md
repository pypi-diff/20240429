# Comparing `tmp/yplib-5.6.3.tar.gz` & `tmp/yplib-5.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-5.6.3.tar", last modified: Mon Apr 15 07:19:54 2024, max compression
+gzip compressed data, was "yplib-5.6.4.tar", last modified: Mon Apr 29 03:54:07 2024, max compression
```

## Comparing `yplib-5.6.3.tar` & `yplib-5.6.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 07:19:54.290249 yplib-5.6.3/
--rw-rw-rw-   0        0        0      400 2024-04-15 07:19:54.290249 yplib-5.6.3/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.6.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-15 07:19:54.290249 yplib-5.6.3/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-04-15 07:19:44.000000 yplib-5.6.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-15 07:19:54.273923 yplib-5.6.3/yplib/
--rw-rw-rw-   0        0        0      617 2023-07-03 02:25:38.000000 yplib-5.6.3/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.6.3/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.6.3/yplib/chart_html.py
--rw-rw-rw-   0        0        0    10673 2024-04-15 07:19:32.000000 yplib-5.6.3/yplib/db.py
--rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.6.3/yplib/file.py
--rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.6.3/yplib/http_util.py
--rw-rw-rw-   0        0        0    40804 2024-04-10 06:44:07.000000 yplib-5.6.3/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.6.3/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.6.3/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.6.3/yplib/markdown.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.6.3/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-04-15 07:19:54.290249 yplib-5.6.3/yplib.egg-info/
--rw-rw-rw-   0        0        0      400 2024-04-15 07:19:54.000000 yplib-5.6.3/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      312 2024-04-15 07:19:54.000000 yplib-5.6.3/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 07:19:54.000000 yplib-5.6.3/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-15 07:19:54.000000 yplib-5.6.3/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 03:54:07.705259 yplib-5.6.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.6.4/LICENSE
+-rw-rw-rw-   0        0        0      355 2024-04-29 03:54:07.705259 yplib-5.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.6.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-29 03:54:07.705259 yplib-5.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-04-29 02:56:51.000000 yplib-5.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:54:07.690279 yplib-5.6.4/yplib/
+-rw-rw-rw-   0        0        0      617 2023-07-03 02:25:38.000000 yplib-5.6.4/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.6.4/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.6.4/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    11273 2024-04-29 02:56:36.000000 yplib-5.6.4/yplib/db.py
+-rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.6.4/yplib/file.py
+-rw-rw-rw-   0        0        0     7355 2024-03-13 10:43:36.000000 yplib-5.6.4/yplib/http_util.py
+-rw-rw-rw-   0        0        0    40804 2024-04-10 06:44:07.000000 yplib-5.6.4/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.6.4/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.6.4/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.6.4/yplib/markdown.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.6.4/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-04-29 03:54:07.705259 yplib-5.6.4/yplib.egg-info/
+-rw-rw-rw-   0        0        0      355 2024-04-29 03:54:07.000000 yplib-5.6.4/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      320 2024-04-29 03:54:07.000000 yplib-5.6.4/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 03:54:07.000000 yplib-5.6.4/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-29 03:54:07.000000 yplib-5.6.4/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.6.3/setup.py` & `yplib-5.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.6.3",
+    version="5.6.4",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.6.3/yplib/__init__.py` & `yplib-5.6.4/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.3/yplib/chart.py` & `yplib-5.6.4/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.3/yplib/chart_html.py` & `yplib-5.6.4/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.3/yplib/db.py` & `yplib-5.6.4/yplib/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from yplib.index import *
 from yplib.http_util import *
 import pymysql
+import adbc_driver_manager
+import adbc_driver_flightsql.dbapi as flight_sql
 
 
 # 有关数据库操作的类
 def get_connect(database=None, user=None, password=None, charset='utf8mb4', port=3306, host=None):
     return pymysql.connect(database=database, user=user, password=password, charset=charset, port=port, host=host)
 
 
@@ -36,14 +38,28 @@
         if is_log:
             to_log_file(sql)
         db_cursor.execute(str(sql))
     if commit:
         db_conn.commit()
 
 
+# 执行 sql 语句, 并且提交, 默认值提交的了
+def exec_doris_sql(sql='', db_config='doris'):
+    config_db = get_config_data(db_config)
+    my_uri = config_db['uri']
+    my_db_kwargs = {
+        adbc_driver_manager.DatabaseOptions.USERNAME.value: config_db['username'],
+        adbc_driver_manager.DatabaseOptions.PASSWORD.value: config_db['password'],
+    }
+    conn = flight_sql.connect(uri=my_uri, db_kwargs=my_db_kwargs)
+    cursor = conn.cursor()
+    cursor.execute(sql)
+    cursor.close()
+
+
 # 执行 sql 语句, 不提交
 def exec_sql_un_commit(sql='', db_conn=None, database=None):
     exec_sql(sql=sql, db_conn=db_conn, commit=False, database=database)
 
 
 # 执行 sql 获得 数据
 def get_data_from_sql(sql='', db_conn=None, db_config='stock_db', is_log=False, database=None):
```

### Comparing `yplib-5.6.3/yplib/file.py` & `yplib-5.6.4/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.3/yplib/http_util.py` & `yplib-5.6.4/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.3/yplib/index.py` & `yplib-5.6.4/yplib/index.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.3/yplib/mail.py` & `yplib-5.6.4/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.3/yplib/mail_html.py` & `yplib-5.6.4/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.6.3/yplib/markdown.py` & `yplib-5.6.4/yplib/markdown.py`

 * *Files identical despite different names*

