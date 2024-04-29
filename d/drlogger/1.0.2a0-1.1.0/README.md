# Comparing `tmp/drlogger-1.0.2a0.tar.gz` & `tmp/drlogger-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drlogger-1.0.2a0.tar", max compression
+gzip compressed data, was "drlogger-1.1.0.tar", max compression
```

## Comparing `drlogger-1.0.2a0.tar` & `drlogger-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    35148 2022-10-10 12:27:29.215237 drlogger-1.0.2a0/LICENSE
--rw-r--r--   0        0        0      143 2022-10-10 12:27:29.215237 drlogger-1.0.2a0/README.md
--rw-r--r--   0        0        0       77 2022-10-10 12:27:29.215237 drlogger-1.0.2a0/drlogger/__init__.py
--rw-r--r--   0        0        0     4611 2022-10-10 12:27:29.215237 drlogger-1.0.2a0/drlogger/formatter.py
--rw-r--r--   0        0        0     2222 2022-10-10 12:27:29.215237 drlogger-1.0.2a0/drlogger/main.py
--rw-r--r--   0        0        0      561 2022-10-10 12:27:29.215237 drlogger-1.0.2a0/pyproject.toml
--rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 drlogger-1.0.2a0/setup.py
--rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 drlogger-1.0.2a0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-29 10:38:00.428287 drlogger-1.1.0/LICENSE
+-rw-r--r--   0        0        0      143 2024-04-29 10:38:00.428287 drlogger-1.1.0/README.md
+-rw-r--r--   0        0        0       77 2024-04-29 10:38:00.428287 drlogger-1.1.0/drlogger/__init__.py
+-rw-r--r--   0        0        0     4611 2024-04-29 10:38:00.428287 drlogger-1.1.0/drlogger/formatter.py
+-rw-r--r--   0        0        0     2327 2024-04-29 10:38:00.428287 drlogger-1.1.0/drlogger/main.py
+-rw-r--r--   0        0        0      559 2024-04-29 10:38:00.428287 drlogger-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 drlogger-1.1.0/PKG-INFO
```

### Comparing `drlogger-1.0.2a0/LICENSE` & `drlogger-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drlogger-1.0.2a0/drlogger/formatter.py` & `drlogger-1.1.0/drlogger/formatter.py`

 * *Files identical despite different names*

### Comparing `drlogger-1.0.2a0/drlogger/main.py` & `drlogger-1.1.0/drlogger/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,35 +8,39 @@
 
 
 class DrLogger:
     """DrLogger initialize Graylog Handler and create structured logs"""
     def __init__(
         self,
         name: str,
+        *,
         graylog_host: t.Optional[str] = None,
         graylog_port: t.Optional[int] = None,
         parameter_filter: t.Optional[t.List[str]] = None,
         header_filter: t.Optional[t.List[str]] = None,
         flask_app=None,
+        handler=None,
     ) -> None:
         """
         DrLogger - create a custom logger
 
         Args:
             name (str): name of the logger, this can be used as an identifier while filtering logs.
             graylog_host (str): graylog host. Defaults to None.
             graylog_port (int): graylog post for sending logs using UDP. Defaults to None.
             parameter_filter (List[str]): parameters to be excluded from logs. Defaults to None.
             header_filter (List[str]): request header to be excluded from logs. Defaults to None.
+            handler: custom handler
         """
         self.logger_name: str = name
 
-        handler = logging.StreamHandler()
-        if graylog_host and graylog_port:
-            handler = graypy.GELFUDPHandler(graylog_host, graylog_port)
+        if not handler:
+            handler = logging.StreamHandler()
+            if graylog_host and graylog_port:
+                handler = graypy.GELFUDPHandler(graylog_host, graylog_port)
 
         formatter = DrFormatter(
             parameter_filter=parameter_filter or [],
             header_filter=header_filter or [],
             has_flask_app=bool(flask_app)
         )
         handler.setFormatter(formatter)
```

### Comparing `drlogger-1.0.2a0/pyproject.toml` & `drlogger-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drlogger"
-version = "1.0.2a0"
+version = "1.1.0"
 description = ""
 authors = ["Ajamal Khan <13559558+khan-ajamal@users.noreply.github.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 graypy = "^2.1.0"
```

### Comparing `drlogger-1.0.2a0/PKG-INFO` & `drlogger-1.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: drlogger
-Version: 1.0.2a0
+Version: 1.1.0
 Summary: 
 Author: Ajamal Khan
 Author-email: 13559558+khan-ajamal@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: graypy (>=2.1.0,<3.0.0)
 Requires-Dist: python-json-logger (>=2.0.4,<3.0.0)
 Description-Content-Type: text/markdown
 
 <h1 align="center">DrLogger</h1>
 <p align="center">A python package for logging</p>
```

