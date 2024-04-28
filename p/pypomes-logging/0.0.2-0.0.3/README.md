# Comparing `tmp/pypomes_logging-0.0.2.tar.gz` & `tmp/pypomes_logging-0.0.3.tar.gz`

## Comparing `pypomes_logging-0.0.2.tar` & `pypomes_logging-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pypomes_logging-0.0.2/src/pypomes_logging/__init__.py
--rw-r--r--   0        0        0    12772 2020-02-02 00:00:00.000000 pypomes_logging-0.0.2/src/pypomes_logging/logging_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_logging-0.0.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_logging-0.0.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_logging-0.0.2/README.md
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pypomes_logging-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pypomes_logging-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 pypomes_logging-0.0.3/src/pypomes_logging/__init__.py
+-rw-r--r--   0        0        0    12913 2020-02-02 00:00:00.000000 pypomes_logging-0.0.3/src/pypomes_logging/logging_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_logging-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_logging-0.0.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_logging-0.0.3/README.md
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 pypomes_logging-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pypomes_logging-0.0.3/PKG-INFO
```

### Comparing `pypomes_logging-0.0.2/src/pypomes_logging/__init__.py` & `pypomes_logging-0.0.3/src/pypomes_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_logging-0.0.2/src/pypomes_logging/logging_pomes.py` & `pypomes_logging-0.0.3/src/pypomes_logging/logging_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,20 +187,22 @@
         log_entries.seek(0)
         result = send_file(path_or_file=log_entries,
                            mimetype="text/plain",
                            as_attachment=attach,
                            download_name=log_file)
     else:
         # yes, report the failure
-        result = Response(json.dumps({"errors": errors}), status=400,  mimetype="application/json")
+        result = Response(response=json.dumps({"errors": errors}),
+                          status=400,
+                          mimetype="application/json")
 
     return result
 
 
-def logging_log_msgs(msgs: list[str],
+def logging_log_msgs(msgs: str | list[str],
                      output_dev: TextIO = None,
                      log_level: Literal["debug", "info", "warning", "error", "critical"] = "error",
                      logger: logging.Logger = PYPOMES_LOGGER) -> None:
     """
     Write all messages in *msgs* to *logger*'s logging file, and to *output_dev*.
 
     The output device is tipically *sys.stdout* or *sys.stderr*.
@@ -221,15 +223,16 @@
             log_writer = logger.warning
         case "error":
             log_writer = logger.error
         case "critical":
             log_writer = logger.critical
 
     # traverse the messages list
-    for msg in msgs:
+    msg_list: list[str] = [msgs] if isinstance(msgs, str) else msgs
+    for msg in msg_list:
         # has the log writer been defined ?
         if log_writer:
             # yes, log the message
             log_writer(msg)
 
         # write to output
         __write_to_output(msg, output_dev)
```

### Comparing `pypomes_logging-0.0.2/LICENSE` & `pypomes_logging-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_logging-0.0.2/pyproject.toml` & `pypomes_logging-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_logging"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (logging module)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "Flask>=3.0.2",
     "pip>=24.0",
-    "pypomes_core>=0.8.7",
-    "pypomes_http>=0.1.3",
+    "pypomes_core>=0.9.4",
+    "pypomes_http>=0.1.6",
     "python-dateutil>=2.8.2",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Logging"
```

### Comparing `pypomes_logging-0.0.2/PKG-INFO` & `pypomes_logging-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: pypomes_logging
-Version: 0.0.2
+Version: 0.0.3
 Summary: A collection of Python pomes, pennyeach (logging module)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Logging
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Logging/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: flask>=3.0.2
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.8.7
-Requires-Dist: pypomes-http>=0.1.3
+Requires-Dist: pypomes-core>=0.9.4
+Requires-Dist: pypomes-http>=0.1.6
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

