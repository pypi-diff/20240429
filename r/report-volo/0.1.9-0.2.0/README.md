# Comparing `tmp/report_volo-0.1.9.tar.gz` & `tmp/report_volo-0.2.0.tar.gz`

## Comparing `report_volo-0.1.9.tar` & `report_volo-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 report_volo-0.1.9/LICESNE.txt
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 report_volo-0.1.9/requirements.txt
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 report_volo-0.1.9/data/abbreviations.txt
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 report_volo-0.1.9/src/report_volo/__init__.py
--rw-r--r--   0        0        0    12584 2020-02-02 00:00:00.000000 report_volo-0.1.9/src/report_volo/report.py
--rw-r--r--   0        0        0    10197 2020-02-02 00:00:00.000000 report_volo-0.1.9/test/test_report.py
--rw-r--r--   0        0        0     6716 2020-02-02 00:00:00.000000 report_volo-0.1.9/.gitignore
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 report_volo-0.1.9/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 report_volo-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 report_volo-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 report_volo-0.2.0/LICESNE.txt
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 report_volo-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 report_volo-0.2.0/data/abbreviations.txt
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 report_volo-0.2.0/src/report_volo/__init__.py
+-rw-r--r--   0        0        0    12583 2020-02-02 00:00:00.000000 report_volo-0.2.0/src/report_volo/report.py
+-rw-r--r--   0        0        0    10197 2020-02-02 00:00:00.000000 report_volo-0.2.0/test/test_report.py
+-rw-r--r--   0        0        0     6716 2020-02-02 00:00:00.000000 report_volo-0.2.0/.gitignore
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 report_volo-0.2.0/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 report_volo-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 report_volo-0.2.0/PKG-INFO
```

### Comparing `report_volo-0.1.9/LICESNE.txt` & `report_volo-0.2.0/LICESNE.txt`

 * *Files identical despite different names*

### Comparing `report_volo-0.1.9/data/abbreviations.txt` & `report_volo-0.2.0/data/abbreviations.txt`

 * *Files identical despite different names*

### Comparing `report_volo-0.1.9/src/report_volo/__init__.py` & `report_volo-0.2.0/src/report_volo/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 from .report import Record, FileNotFound, ReportInvalidOrder
 
 
+def dict_init(records_dict=None):
+    return Record.dict_init(records_dict)
+
+
+def read_file(path, insert_file):
+    return Record.read_file(path, insert_file)
+
+
 def read_abbr(path, records_dict=None, abbr_file="abbreviations.txt"):
     return Record.read_abbr(path, records_dict, abbr_file)
 
 
+def file_name(insert_file):
+    return Record.file_name(insert_file)
+
+
 def read_logs(path, records_dict=None, start_file="start.log", end_file="end.log"):
     return Record.read_logs(path, records_dict, start_file, end_file)
 
 
 def build_report(path, order="asc"):
     return Record.build_report(path, order)
 
@@ -17,22 +29,20 @@
     return Record.print_report(good_records, bad_records)
 
 
 def cli(args_list=None):
     return Record.cli(args_list)
 
 
-def record_report(args=None):
-    return Record.record_report(args)
-
-
 __all__ = [
     "FileNotFound",
     "ReportInvalidOrder",
     "Record",
-    "cli",
-    "build_report",
+    "dict_init",
+    "read_file",
     "read_abbr",
+    "file_name",
     "read_logs",
     "print_report",
-    "record_report",
+    "cli",
+    "build_report",
 ]
```

### Comparing `report_volo-0.1.9/src/report_volo/report.py` & `report_volo-0.2.0/src/report_volo/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,15 +345,15 @@
         parser.add_argument("--driver", help="Show statistics for a specific driver")
 
         args = parser.parse_args(args_list)
         print(args)
 
         args.sort = "asc" if args.asc else "desc"
 
-        good_records, bad_records = [], [] 
+        good_records, bad_records = [], []
 
         if args.driver:
             good_records = [rec for rec in good_records if rec.driver == args.driver]
             bad_records = [rec for rec in bad_records if rec.driver == args.driver]
 
         return args
```

### Comparing `report_volo-0.1.9/test/test_report.py` & `report_volo-0.2.0/test/test_report.py`

 * *Files identical despite different names*

### Comparing `report_volo-0.1.9/.gitignore` & `report_volo-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `report_volo-0.1.9/README.md` & `report_volo-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `report_volo-0.1.9/pyproject.toml` & `report_volo-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "report_volo"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="Volodymyr Perehuda", email="author@example.com" },
 ]
 description = "A report generation package for results of Monaco 2018 Racing"
 readme = "README.md"
-requires-python = ">=3.11.4"
+requires-python = ">=3.12.3"
 classifiers = [
-    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["your", "volo report", "report volo"]
 
 [project.urls]
 Homepage = "https://git.foxminded.ua/volodymyr-perehuda-nyc/task-6-report-of-monaco-2018-racing"
```

### Comparing `report_volo-0.1.9/PKG-INFO` & `report_volo-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: report_volo
-Version: 0.1.9
+Version: 0.2.0
 Summary: A report generation package for results of Monaco 2018 Racing
 Project-URL: Homepage, https://git.foxminded.ua/volodymyr-perehuda-nyc/task-6-report-of-monaco-2018-racing
 Project-URL: Issues, https://git.foxminded.ua/volodymyr-perehuda-nyc/task-6-report-of-monaco-2018-racing/issues
 Author-email: Volodymyr Perehuda <author@example.com>
 Keywords: report volo,volo report,your
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.11.4
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.12.3
 Description-Content-Type: text/markdown
 
 # Project description
 
 Module for report generation. Takes logs of start and end time, assing values by key to data from abbrevations.txt and provide records recults.
 
 ## Installation
```

