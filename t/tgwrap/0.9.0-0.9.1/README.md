# Comparing `tmp/tgwrap-0.9.0.tar.gz` & `tmp/tgwrap-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgwrap-0.9.0.tar", max compression
+gzip compressed data, was "tgwrap-0.9.1.tar", max compression
```

## Comparing `tgwrap-0.9.0.tar` & `tgwrap-0.9.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.9.0/LICENSE
--rw-r--r--   0        0        0    12159 2024-04-24 11:33:21.171629 tgwrap-0.9.0/README.md
--rw-r--r--   0        0        0      922 2024-04-24 11:29:31.368994 tgwrap-0.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.9.0/tgwrap/__init__.py
--rw-r--r--   0        0        0     8726 2023-10-20 14:35:12.875311 tgwrap-0.9.0/tgwrap/analyze.py
--rwxr-xr-x   0        0        0    29727 2024-04-24 07:14:54.956803 tgwrap-0.9.0/tgwrap/cli.py
--rw-r--r--   0        0        0    10421 2024-04-15 08:15:36.473440 tgwrap-0.9.0/tgwrap/deploy.py
--rwxr-xr-x   0        0        0    80691 2024-04-24 11:32:17.978883 tgwrap-0.9.0/tgwrap/main.py
--rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.9.0/tgwrap/printer.py
--rw-r--r--   0        0        0    13334 1970-01-01 00:00:00.000000 tgwrap-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.9.1/LICENSE
+-rw-r--r--   0        0        0    12159 2024-04-24 11:33:21.171629 tgwrap-0.9.1/README.md
+-rw-r--r--   0        0        0      922 2024-04-29 11:10:57.134281 tgwrap-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.9.1/tgwrap/__init__.py
+-rw-r--r--   0        0        0     8726 2023-10-20 14:35:12.875311 tgwrap-0.9.1/tgwrap/analyze.py
+-rwxr-xr-x   0        0        0    29727 2024-04-24 07:14:54.956803 tgwrap-0.9.1/tgwrap/cli.py
+-rw-r--r--   0        0        0    10243 2024-04-29 11:10:37.178306 tgwrap-0.9.1/tgwrap/deploy.py
+-rwxr-xr-x   0        0        0    80691 2024-04-24 11:32:17.978883 tgwrap-0.9.1/tgwrap/main.py
+-rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.9.1/tgwrap/printer.py
+-rw-r--r--   0        0        0    13334 1970-01-01 00:00:00.000000 tgwrap-0.9.1/PKG-INFO
```

### Comparing `tgwrap-0.9.0/LICENSE` & `tgwrap-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.0/README.md` & `tgwrap-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.0/pyproject.toml` & `tgwrap-0.9.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgwrap"
-version = "0.9.0"
+version = "0.9.1"
 description = "A (terragrunt) wrapper around a (terraform) wrapper around ...."
 authors = ["Gerco Grandia <gerco.grandia@4synergy.nl>", "Pascal Alma <pascal.alma@4synergy.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/lunadata/tgwrap"
 repository = "https://gitlab.com/lunadata/tgwrap"
 documentation = "https://gitlab.com/lunadata/tgwrap/"
```

### Comparing `tgwrap-0.9.0/tgwrap/analyze.py` & `tgwrap-0.9.1/tgwrap/analyze.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.0/tgwrap/cli.py` & `tgwrap-0.9.1/tgwrap/cli.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.0/tgwrap/deploy.py` & `tgwrap-0.9.1/tgwrap/deploy.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,26 +184,26 @@
             }
             target_path = os.path.join(
                 target_dir, substack['target'], ''
                 )
 
             printer.verbose(f'Include substack modules: {include_modules}')
 
-    # printer.verbose(f'Found modules: {source_modules}')
-        # include_modules = config['include_modules'] if len(config.get('include_modules')) > 0 else source_modules
-            include_modules = substack['include_modules'] if len(substack.get('include_modules', {})) > 0 else source_modules
-            printer.verbose(f'Include modules: {include_modules}')
+            include_modules = substack.get('include_modules', [])
 
             if include_modules:
                 # get all directories in the substack and create an exlude_modules list from that
                 source_directories = get_directories(source_path)
                 exclude_modules = list(set(source_directories) - set(include_modules))
             else:
                 exclude_modules = substack.get('exclude_modules', [])
-            
+
+            printer.verbose(f'Include modules: {include_modules}')
+            printer.verbose(f'Exclude modules: {include_modules}')
+
             if os.path.exists(source_path):
                 deploy_actions[f'substack -> {substack["target"]}'] = {
                     "source": source_path,
                     "target": target_path,
                     "excludes": exclude_modules,
                 }
             else:
```

### Comparing `tgwrap-0.9.0/tgwrap/main.py` & `tgwrap-0.9.1/tgwrap/main.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.0/tgwrap/printer.py` & `tgwrap-0.9.1/tgwrap/printer.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.0/PKG-INFO` & `tgwrap-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgwrap
-Version: 0.9.0
+Version: 0.9.1
 Summary: A (terragrunt) wrapper around a (terraform) wrapper around ....
 Home-page: https://gitlab.com/lunadata/tgwrap
 License: MIT
 Keywords: terraform,terragrunt,terrasafe,python
 Author: Gerco Grandia
 Author-email: gerco.grandia@4synergy.nl
 Requires-Python: >=3.8,<4.0
```

