# Comparing `tmp/hdx_cli_toolkit-2024.4.3.tar.gz` & `tmp/hdx_cli_toolkit-2024.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx_cli_toolkit-2024.4.3.tar", last modified: Mon Apr 15 07:01:25 2024, max compression
+gzip compressed data, was "hdx_cli_toolkit-2024.4.4.tar", last modified: Mon Apr 29 07:42:06 2024, max compression
```

## Comparing `hdx_cli_toolkit-2024.4.3.tar` & `hdx_cli_toolkit-2024.4.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:01:25.445929 hdx_cli_toolkit-2024.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-15 07:01:25.445929 hdx_cli_toolkit-2024.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 07:01:25.445929 hdx_cli_toolkit-2024.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:01:25.441929 hdx_cli_toolkit-2024.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:01:25.441929 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15286 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    16068 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/hdx_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:01:25.445929 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-15 07:01:25.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-15 07:01:25.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 07:01:25.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-15 07:01:25.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-15 07:01:25.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 07:01:25.000000 hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 07:01:25.445929 hdx_cli_toolkit-2024.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/tests/test_cli_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/tests/test_hdx_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/tests/test_hdx_utilities_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-04-15 07:01:09.000000 hdx_cli_toolkit-2024.4.3/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:42:06.169075 hdx_cli_toolkit-2024.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-29 07:42:06.169075 hdx_cli_toolkit-2024.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 07:42:06.169075 hdx_cli_toolkit-2024.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:42:06.165075 hdx_cli_toolkit-2024.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:42:06.165075 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20000 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/hdx_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10036 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:42:06.169075 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-29 07:42:06.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-29 07:42:06.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 07:42:06.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-29 07:42:06.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-29 07:42:06.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-29 07:42:06.000000 hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 07:42:06.169075 hdx_cli_toolkit-2024.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/tests/test_cli_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/tests/test_hdx_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7066 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/tests/test_hdx_utilities_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-29 07:41:52.000000 hdx_cli_toolkit-2024.4.4/tests/test_utilities.py
```

### Comparing `hdx_cli_toolkit-2024.4.3/LICENSE` & `hdx_cli_toolkit-2024.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.3/PKG-INFO` & `hdx_cli_toolkit-2024.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx_cli_toolkit
-Version: 2024.4.3
+Version: 2024.4.4
 Summary: HDX CLI tool kit for commandline interaction with HDX
 Author: Ian Hopkinson
 Author-email: ian.hopkinson@un.org
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Ian Hopkinson
```

### Comparing `hdx_cli_toolkit-2024.4.3/README.md` & `hdx_cli_toolkit-2024.4.4/README.md`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.3/pyproject.toml` & `hdx_cli_toolkit-2024.4.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hdx_cli_toolkit"
-version = "2024.4.3"
+version = "2024.4.4"
 description = "HDX CLI tool kit for commandline interaction with HDX"
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 requires-python = ">=3.11"
 authors = [
   {email = "ian.hopkinson@un.org"},
   {name = "Ian Hopkinson"}
```

### Comparing `hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/cli.py` & `hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 
 from hdx_cli_toolkit.utilities import (
     write_dictionary,
     print_table_from_list_of_dicts,
     censor_secret,
     make_conversion_func,
     print_banner,
+    make_path_unique,
 )
 
 from hdx_cli_toolkit.hdx_utilities import (
     add_showcase,
     add_quickcharts,
     get_organizations_from_hdx,
     get_users_from_hdx,
     update_values_in_hdx,
+    update_values_in_hdx_from_file,
     configure_hdx_connection,
     update_resource_in_hdx,
     get_filtered_datasets,
     decorate_dataset_with_extras,
     download_hdx_datasets,
     get_approved_tag_list,
 )
@@ -127,64 +129,100 @@
         output_template[key_] = ""
 
     output = []
     for dataset in filtered_datasets:
         output_row = output_template.copy()
         output_row["dataset_name"] = dataset["name"]
         for key_ in keys:
-            output_row[key_] = dataset.get(key_, "")
+            output_row[key_] = dataset.get(key_, "Key absent")
         output.append(output_row)
 
     print_table_from_list_of_dicts(output)
     if output_path is not None:
+        output_path = make_path_unique(output_path)
         status = write_dictionary(output_path, output, append=False)
         print(status, flush=True)
 
 
 @hdx_toolkit.command(name="update")
 @multi_decorator(OPTIONS)
+@click.option(
+    "--output_path",
+    is_flag=False,
+    default=None,
+    help="A file path to export data from update to CSV",
+)
+@click.option(
+    "--from_path",
+    is_flag=False,
+    default=None,
+    help="A file path to a file with values to be updated, as generated by the update command",
+)
+@click.option(
+    "--undo",
+    is_flag=True,
+    default=False,
+    help="This flag indicates that the --from_path is an output from update being used for an undo",
+)
 def update(
     organization: str = "",
     key: str = "private",
     value: str = "value",
     dataset_filter: str = "*",
     query: str = None,
     hdx_site: str = "stage",
+    output_path: str = None,
+    from_path: str = None,
+    undo: bool = False,
 ):
     """Update datasets in HDX"""
     print_banner("Update")
-    filtered_datasets = get_filtered_datasets(
-        organization=organization,
-        dataset_filter=dataset_filter,
-        query=query,
-        hdx_site=hdx_site,
-    )
 
-    if len(filtered_datasets) == 0:
-        print("Specified filter returns no datasets", flush=True)
-        return
-
-    print(f"Updating key '{key}' with value '{value}'")
-    conversion_func, type_name = make_conversion_func(filtered_datasets[0][key])
-    if conversion_func is None:
-        print(f"Type name '{type_name}' is not recognised, aborting", flush=True)
-        return
-
-    print(f"Detected value type is '{type_name}'", flush=True)
-    print(
-        f"{'dataset_name':<70.70}{'old value':<20.20}{'new value':<20.20}"
-        f"{'Time to update/seconds':<25.25}",
-        flush=True,
-    )
-    n_changed, n_failures = update_values_in_hdx(
-        filtered_datasets, key, value, conversion_func, hdx_site=hdx_site
-    )
+    if from_path is not None:
+        update_values_in_hdx_from_file(hdx_site, from_path, undo=undo, output_path=output_path)
+    else:
+        filtered_datasets = get_filtered_datasets(
+            organization=organization,
+            dataset_filter=dataset_filter,
+            query=query,
+            hdx_site=hdx_site,
+        )
+
+        if len(filtered_datasets) == 0:
+            print("Specified filter returns no datasets", flush=True)
+            return
+
+        print(f"Updating key '{key}' with value '{value}'")
+        for filtered_dataset in filtered_datasets:
+            try:
+                conversion_func, type_name = make_conversion_func(filtered_dataset[key])
+            except KeyError:
+                continue
+
+        if conversion_func is None:
+            print(f"Type name '{type_name}' is not recognised, aborting", flush=True)
+            return
+
+        print(f"Detected value type is '{type_name}'", flush=True)
+        print(
+            f"{'dataset_name':<70.70}{'old value':<20.20}{'new value':<20.20}"
+            f"{'Time to update/seconds':<25.25}",
+            flush=True,
+        )
+        n_changed, n_failures, output_rows = update_values_in_hdx(
+            filtered_datasets, key, value, conversion_func, hdx_site=hdx_site
+        )
+
+        if output_path is not None:
+            output_path = make_path_unique(output_path)
+            status = write_dictionary(output_path, output_rows, append=False)
+            print(status, flush=True)
 
-    print(f"Changed {n_changed} values", flush=True)
-    print(f"{n_failures} failures as evidenced by HDXError", flush=True)
+        print(f"Changed {n_changed} values", flush=True)
+        print(f"{n_failures} failures as evidenced by HDXError", flush=True)
 
 
 @hdx_toolkit.command(name="print")
 @multi_decorator(OPTIONS)
 @click.option(
     "--with_extras",
     is_flag=True,
```

### Comparing `hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/hdx_utilities.py` & `hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/hdx_utilities.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
-
+import csv
 import fnmatch
 import functools
 import json
 import os
 import time
 import traceback
 import urllib3
@@ -22,35 +22,56 @@
 from hdx.data.hdxobject import HDXError
 from hdx.data.dataset import Dataset
 from hdx.data.showcase import Showcase
 from hdx.data.resource import Resource
 from hdx.data.user import User
 from hdx.utilities.path import script_dir_plus_file
 
-from hdx_cli_toolkit.utilities import read_attributes
+from hdx_cli_toolkit.utilities import (
+    read_attributes,
+    make_conversion_func,
+    write_dictionary,
+    make_path_unique,
+)
 
 
 def hdx_error_handler(f):
     @functools.wraps(f)
     def inner(*args, **kwargs):
         try:
             return f(*args, **kwargs)
         except HDXError:
-            if "Authorization Error" in traceback.format_exc():
+            message = parse_hdxerror_traceback(traceback.format_exc())
+            if message == "unknown":
                 click.secho(
-                    "Could not perform operation on HDX because of an authorization error",
+                    f"Could not perform operation on HDX because of an `{message}`",
                     fg="red",
                     color=True,
                 )
             else:
                 print(traceback.format_exc)
 
     return inner
 
 
+def parse_hdxerror_traceback(traceback_message: str):
+    message = "unknown"
+    if "Authorization Error" in traceback.format_exc():
+        message = "Authorization Error"
+    elif (
+        "{'extras': [{}, {'key': ['There is a schema field with the same name']}]"
+        in traceback.format_exc()
+    ):
+        message = "Extras Key Error"
+    elif "KeyError: 'resources'" in traceback.format_exc():
+        message = "No Resources Error"
+
+    return message
+
+
 @hdx_error_handler
 def get_filtered_datasets(
     organization: str = "",
     dataset_filter: str = "*",
     query: str = None,
     hdx_site: str = "stage",
     verbose: bool = True,
@@ -103,57 +124,149 @@
             flush=True,
         )
 
     return filtered_datasets
 
 
 @hdx_error_handler
+def update_values_in_hdx_from_file(
+    hdx_site: str, from_file: str, undo: bool = False, output_path: str = None
+):
+    configure_hdx_connection(hdx_site=hdx_site)
+    # Open the file
+    if not os.path.exists(from_file):
+        print(f"The file provided for input ({from_file}) does not exist. Exiting.", flush=True)
+        return
+    with open(from_file, "r", encoding="utf-8") as update_file_handle:
+        rows = list(csv.DictReader(update_file_handle))
+        # Check the file has rows, and the required columns.
+        if len(rows) == 0:
+            print(
+                f"The file provided for input ({from_file}) contains no rows. Exiting.", flush=True
+            )
+            return
+
+        # For each row
+        n_changed = 0
+        n_failures = 0
+        output_rows = []
+        print(f"From_file {from_file} contains {len(rows)} entries", flush=True)
+        print(
+            f"{'dataset_name':<70.70}{'old value':<20.20}{'new value':<20.20}"
+            f"{'Time to update/seconds':<25.25}",
+            flush=True,
+        )
+        new_value_key = "new_value"
+        if undo:
+            new_value_key = "old_value"
+        for row in rows:
+            dataset = Dataset.read_from_hdx(row["dataset_name"])
+            # Read in the dataset
+            if not dataset:
+                print(f"{row['dataset_name']} does not exist on {hdx_site}. Exiting", flush=True)
+                return
+
+            conversion_func, type_name = make_conversion_func(row[new_value_key])
+
+            if conversion_func is None:
+                print(f"Type name '{type_name}' is not recognised, aborting", flush=True)
+                return
+
+            dn_changed, dn_failures, doutput_rows = update_values_in_hdx(
+                [dataset], row["key"], row[new_value_key], conversion_func, hdx_site=hdx_site
+            )
+            n_changed += dn_changed
+            n_failures += dn_failures
+            output_rows.extend(doutput_rows)
+
+    # Make an output_path from the from_path?
+    if output_path is not None:
+        output_path = make_path_unique(output_path)
+    else:
+        filename, extension = os.path.splitext(from_file)
+        output_path = f"{filename}-redo{extension}"
+    status = write_dictionary(output_path, output_rows, append=False)
+    print(status, flush=True)
+
+    print(f"Changed {n_changed} values", flush=True)
+    print(f"{n_failures} failures as evidenced by HDXError", flush=True)
+
+
+@hdx_error_handler
 def update_values_in_hdx(
     filtered_datasets: list[Dataset], key, value, conversion_func, hdx_site: str = "stage"
 ):
     n_changed = 0
     n_failures = 0
+    row_template = {
+        "dataset_name": None,
+        "key": key,
+        "old_value": None,
+        "new_value": None,
+        "message": None,
+    }
+    output_rows = []
     for dataset in filtered_datasets:
         t0 = time.time()
-        old_value = str(dataset[key])
-        dataset[key] = conversion_func(value)
+        try:
+            old_value = str(dataset[key])
+        except KeyError:
+            old_value = ""
+        new_value = conversion_func(value)
+        dataset[key] = new_value
+
+        row = row_template.copy()
+        row["dataset_name"] = dataset["name"]
+        row["old_value"] = old_value
+        row["new_value"] = new_value
+
         if old_value != str(dataset[key]):
             n_changed += 1
         else:
+            message = "No update required"
             print(
-                f"{dataset['name']:<70.70}{old_value:<20.20}{str(dataset[key]):<20.20}"
-                f"{'No update required':<25.25}",
+                f"{dataset['name']:<70.70}{old_value:<20.20}{str(dataset[key]):<20.20} "
+                f"{message:<25.25}",
                 flush=True,
             )
+            row["message"] = message
+            output_rows.append(row)
             continue
         try:
+            if "extras" in dataset.data:
+                dataset.data.pop("extras")
             dataset.update_in_hdx(
                 update_resources=False,
                 hxl_update=False,
                 operation="patch",
                 batch_mode="KEEP_OLD",
                 skip_validation=True,
                 ignore_check=True,
             )
+            message = f"{time.time() - t0:.2f}"
             print(
-                f"{dataset['name']:<70.70}{old_value:<20.20}{str(dataset[key]):<20.20}"
-                f"{time.time()-t0:0.2f}",
+                f"{dataset['name']:<70.70}{old_value:<20.20}{str(dataset[key]):<20.20} "
+                f"{message}",
                 flush=True,
             )
+            row["message"] = message
+            output_rows.append(row)
         except (HDXError, KeyError):
-            print(f"Could not update {dataset['name']} on '{hdx_site}'", flush=True)
+            traceback_message = parse_hdxerror_traceback(traceback.format_exc())
+            message = f"Could not update {dataset['name']} on '{hdx_site}' - {traceback_message}"
             n_failures += 1
 
             print(
-                f"{dataset['name']:<70.70}{old_value:<20.20}{old_value:<20.20}"
-                f"{time.time()-t0:0.2f}",
+                f"{dataset['name']:<70.70}{old_value:<20.20}{old_value:<20.20} {message}",
                 flush=True,
             )
+            row["message"] = message
+            output_rows.append(row)
 
-    return n_changed, n_failures
+    return n_changed, n_failures, output_rows
 
 
 @hdx_error_handler
 def get_organizations_from_hdx(organization: str, hdx_site: str = "stage"):
     configure_hdx_connection(hdx_site)
     filtered_organizations = []
     all_organizations = Organization.get_all_organization_names(include_extras=True)
```

### Comparing `hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit/utilities.py` & `hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -278,7 +278,19 @@
     title = f"HDX CLI toolkit - {action}"
     timestamp = f"Invoked at: {datetime.datetime.now().isoformat()}"
     width = max(len(title), len(timestamp))
     click.secho((width + 4) * "*", bold=True)
     click.secho(f"* {title:<{width}} *", bold=True)
     click.secho(f"* {timestamp:<{width}} *", bold=True)
     click.secho((width + 4) * "*", bold=True)
+
+
+def make_path_unique(input_path: str) -> str:
+    filename, extension = os.path.splitext(input_path)
+    counter = 1
+
+    unique_path = input_path
+    while os.path.exists(unique_path):
+        unique_path = f"{filename}-{str(counter)}{extension}"
+        counter += 1
+
+    return unique_path
```

### Comparing `hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/PKG-INFO` & `hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx_cli_toolkit
-Version: 2024.4.3
+Version: 2024.4.4
 Summary: HDX CLI tool kit for commandline interaction with HDX
 Author: Ian Hopkinson
 Author-email: ian.hopkinson@un.org
 License: The MIT License (MIT)
         
         Copyright (c) 2024 Ian Hopkinson
```

### Comparing `hdx_cli_toolkit-2024.4.3/src/hdx_cli_toolkit.egg-info/SOURCES.txt` & `hdx_cli_toolkit-2024.4.4/src/hdx_cli_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.3/tests/test_cli.py` & `hdx_cli_toolkit-2024.4.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.3/tests/test_cli_integration.py` & `hdx_cli_toolkit-2024.4.4/tests/test_cli_integration.py`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.3/tests/test_hdx_utilities.py` & `hdx_cli_toolkit-2024.4.4/tests/test_hdx_utilities.py`

 * *Files identical despite different names*

### Comparing `hdx_cli_toolkit-2024.4.3/tests/test_hdx_utilities_integration.py` & `hdx_cli_toolkit-2024.4.4/tests/test_hdx_utilities_integration.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from hdx_cli_toolkit.hdx_utilities import (
     update_resource_in_hdx,
     configure_hdx_connection,
     update_values_in_hdx,
     add_showcase,
     add_quickcharts,
     get_approved_tag_list,
+    update_values_in_hdx_from_file,
 )
 
 from hdx_cli_toolkit.utilities import make_conversion_func
 
 
 DATASET_NAME = "hdx_cli_toolkit_test"
 TEST_RESOURCE_NAME = "test_resource_1"
@@ -133,20 +134,21 @@
 
 
 def test_update_key():
     dataset = Dataset.read_from_hdx(DATASET_NAME)
     key = "notes"
     value = "new notes"
     conversion_func, _ = make_conversion_func(value)
-    n_changed, n_failures = update_values_in_hdx(
+    n_changed, n_failures, output_rows = update_values_in_hdx(
         [dataset], key, value, conversion_func, hdx_site=HDX_SITE
     )
 
     assert n_changed == 1
     assert n_failures == 0
+    assert len(output_rows) == 1
     dataset = Dataset.read_from_hdx(DATASET_NAME)
 
     assert dataset["notes"] == "new notes"
 
 
 def test_add_showcase():
     attributes_file_path = os.path.join(os.path.dirname(__file__), "fixtures", "attributes.csv")
@@ -202,7 +204,14 @@
     assert len(quickchart_dicts) == 2
     assert quickchart_dicts[1]["title"] == "Quick Charts"
 
 
 def test_get_approved_tag_list():
     approved_tags = get_approved_tag_list()
     assert len(approved_tags) == 140
+
+
+def test_update_values_in_hdx_from_file():
+    update_file_path = os.path.join(os.path.dirname(__file__), "fixtures", "update-from-file.csv")
+    update_values_in_hdx_from_file(HDX_SITE, update_file_path)
+    dataset = Dataset.read_from_hdx(DATASET_NAME)
+    assert dataset["caveats"] == "Second value from_file"
```

### Comparing `hdx_cli_toolkit-2024.4.3/tests/test_utilities.py` & `hdx_cli_toolkit-2024.4.4/tests/test_utilities.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     write_dictionary,
     censor_secret,
     read_attributes,
     print_banner,
     print_table_from_list_of_dicts,
     str_to_bool,
     make_conversion_func,
+    make_path_unique,
 )
 
 
 ATTRIBUTES_FILE_PATH = os.path.join(os.path.dirname(__file__), "fixtures", "attributes.csv")
 DATASET_NAME = "climada-litpop-showcase"
 REFERENCE_ATTRIBUTES = read_attributes(DATASET_NAME, attributes_filepath=ATTRIBUTES_FILE_PATH)
 
@@ -118,7 +119,15 @@
 
 
 def test_make_conversion_func():
     test_values = [(1, "int"), ("string", "str"), (1.4, "float"), (True, "bool")]
     for test_value in test_values:
         _, func_name = make_conversion_func(test_value[0])
         assert func_name == test_value[1]
+
+
+def test_make_path_unique():
+    input_path = __file__
+    unique_path = make_path_unique(input_path)
+    input_filename = os.path.basename(input_path)
+
+    assert os.path.basename(unique_path) == input_filename.replace(".py", "-1.py")
```

