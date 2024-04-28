# Comparing `tmp/mecha-0.93.1.tar.gz` & `tmp/mecha-0.94.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mecha-0.93.1.tar", max compression
+gzip compressed data, was "mecha-0.94.0.tar", max compression
```

## Comparing `mecha-0.93.1.tar` & `mecha-0.94.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1073 2024-04-11 00:33:48.108998 mecha-0.93.1/LICENSE
--rw-r--r--   0        0        0     8612 2024-04-11 00:33:48.108998 mecha-0.93.1/README.md
--rw-r--r--   0        0        0      344 2024-04-11 00:34:07.009225 mecha-0.93.1/mecha/__init__.py
--rw-r--r--   0        0        0       35 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/__main__.py
--rw-r--r--   0        0        0    22660 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/api.py
--rw-r--r--   0        0        0    36695 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/ast.py
--rw-r--r--   0        0        0     3057 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/cli.py
--rw-r--r--   0        0        0      719 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/commands.py
--rw-r--r--   0        0        0     6147 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/config.py
--rw-r--r--   0        0        0        0 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/__init__.py
--rw-r--r--   0        0        0     1840 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/annotate_diagnostics.py
--rw-r--r--   0        0        0    12498 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/bake_macros.py
--rw-r--r--   0        0        0      177 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/clear_diagnostics.py
--rw-r--r--   0        0        0     1096 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/debug_ast.py
--rw-r--r--   0        0        0     5840 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/embed.py
--rw-r--r--   0        0        0     2932 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/implicit_execute.py
--rw-r--r--   0        0        0     2592 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/inline_function_tag.py
--rw-r--r--   0        0        0     6358 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/json_files.py
--rw-r--r--   0        0        0     2561 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/lint_basic.py
--rw-r--r--   0        0        0     2678 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/messages.py
--rw-r--r--   0        0        0     6188 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/nested_location.py
--rw-r--r--   0        0        0    12727 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/nested_resources.py
--rw-r--r--   0        0        0     9514 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/nested_yaml.py
--rw-r--r--   0        0        0    15453 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/nesting.py
--rw-r--r--   0        0        0     1050 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/raw.py
--rw-r--r--   0        0        0     2468 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/relative_location.py
--rw-r--r--   0        0        0     2234 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/source_map.py
--rw-r--r--   0        0        0    11944 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/statistics.py
--rw-r--r--   0        0        0       21 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/validation/__init__.py
--rw-r--r--   0        0        0    38232 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/contrib/validation/mcdoc.py
--rw-r--r--   0        0        0     6205 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/database.py
--rw-r--r--   0        0        0     5964 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/diagnostic.py
--rw-r--r--   0        0        0    13332 2024-04-11 00:33:48.116998 mecha-0.93.1/mecha/dispatch.py
--rw-r--r--   0        0        0      106 2024-04-11 00:33:48.120998 mecha-0.93.1/mecha/error.py
--rw-r--r--   0        0        0    72796 2024-04-11 00:33:48.120998 mecha-0.93.1/mecha/parse.py
--rw-r--r--   0        0        0      205 2024-04-11 00:33:48.120998 mecha-0.93.1/mecha/plugin.py
--rw-r--r--   0        0        0     1181 2024-04-11 00:33:48.120998 mecha-0.93.1/mecha/preprocess.py
--rw-r--r--   0        0        0     1214 2024-04-11 00:33:48.120998 mecha-0.93.1/mecha/prototype.py
--rw-r--r--   0        0        0        0 2024-04-11 00:33:48.120998 mecha-0.93.1/mecha/py.typed
--rw-r--r--   0        0        0   257142 2024-04-11 00:33:48.120998 mecha-0.93.1/mecha/resources/1_16.json
--rw-r--r--   0        0        0   266016 2024-04-11 00:33:48.120998 mecha-0.93.1/mecha/resources/1_17.json
--rw-r--r--   0        0        0   265402 2024-04-11 00:33:48.120998 mecha-0.93.1/mecha/resources/1_18.json
--rw-r--r--   0        0        0   393608 2024-04-11 00:33:48.124998 mecha-0.93.1/mecha/resources/1_19.json
--rw-r--r--   0        0        0   392539 2024-04-11 00:33:48.124998 mecha-0.93.1/mecha/resources/1_20.json
--rw-r--r--   0        0        0        0 2024-04-11 00:33:48.124998 mecha-0.93.1/mecha/resources/__init__.py
--rw-r--r--   0        0        0      369 2024-04-11 00:33:48.124998 mecha-0.93.1/mecha/resources/inline_function_tag.json
--rw-r--r--   0        0        0     7984 2024-04-11 00:33:48.124998 mecha-0.93.1/mecha/resources/nesting.json
--rw-r--r--   0        0        0      526 2024-04-11 00:33:48.124998 mecha-0.93.1/mecha/resources/patches.json
--rw-r--r--   0        0        0    12620 2024-04-11 00:33:48.124998 mecha-0.93.1/mecha/serialize.py
--rw-r--r--   0        0        0     3440 2024-04-11 00:33:48.124998 mecha-0.93.1/mecha/spec.py
--rw-r--r--   0        0        0     6393 2024-04-11 00:33:48.124998 mecha-0.93.1/mecha/utils.py
--rw-r--r--   0        0        0     1293 2024-04-11 00:34:07.037225 mecha-0.93.1/pyproject.toml
--rw-r--r--   0        0        0     9352 1970-01-01 00:00:00.000000 mecha-0.93.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-28 23:54:56.629248 mecha-0.94.0/LICENSE
+-rw-r--r--   0        0        0     8612 2024-04-28 23:54:56.629248 mecha-0.94.0/README.md
+-rw-r--r--   0        0        0      344 2024-04-28 23:55:42.117950 mecha-0.94.0/mecha/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/__main__.py
+-rw-r--r--   0        0        0    22660 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/api.py
+-rw-r--r--   0        0        0    36695 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/ast.py
+-rw-r--r--   0        0        0     3057 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/cli.py
+-rw-r--r--   0        0        0      719 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/commands.py
+-rw-r--r--   0        0        0     6147 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/config.py
+-rw-r--r--   0        0        0        0 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/__init__.py
+-rw-r--r--   0        0        0     1840 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/annotate_diagnostics.py
+-rw-r--r--   0        0        0    12498 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/bake_macros.py
+-rw-r--r--   0        0        0      177 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/clear_diagnostics.py
+-rw-r--r--   0        0        0     1096 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/debug_ast.py
+-rw-r--r--   0        0        0     5840 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/embed.py
+-rw-r--r--   0        0        0     2932 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/implicit_execute.py
+-rw-r--r--   0        0        0     2592 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/inline_function_tag.py
+-rw-r--r--   0        0        0     6358 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/json_files.py
+-rw-r--r--   0        0        0     2561 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/lint_basic.py
+-rw-r--r--   0        0        0     2678 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/messages.py
+-rw-r--r--   0        0        0     6188 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/nested_location.py
+-rw-r--r--   0        0        0    12727 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/nested_resources.py
+-rw-r--r--   0        0        0     9514 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/nested_yaml.py
+-rw-r--r--   0        0        0    15453 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/nesting.py
+-rw-r--r--   0        0        0     1050 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/raw.py
+-rw-r--r--   0        0        0     2468 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/relative_location.py
+-rw-r--r--   0        0        0     2234 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/source_map.py
+-rw-r--r--   0        0        0    11944 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/statistics.py
+-rw-r--r--   0        0        0       21 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/validation/__init__.py
+-rw-r--r--   0        0        0    38232 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/contrib/validation/mcdoc.py
+-rw-r--r--   0        0        0     6205 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/database.py
+-rw-r--r--   0        0        0     5964 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/diagnostic.py
+-rw-r--r--   0        0        0    13332 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/dispatch.py
+-rw-r--r--   0        0        0      106 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/error.py
+-rw-r--r--   0        0        0    72796 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/parse.py
+-rw-r--r--   0        0        0      205 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/plugin.py
+-rw-r--r--   0        0        0     1181 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/preprocess.py
+-rw-r--r--   0        0        0     1214 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/prototype.py
+-rw-r--r--   0        0        0        0 2024-04-28 23:54:56.637248 mecha-0.94.0/mecha/py.typed
+-rw-r--r--   0        0        0   257142 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/1_16.json
+-rw-r--r--   0        0        0   266016 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/1_17.json
+-rw-r--r--   0        0        0   265402 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/1_18.json
+-rw-r--r--   0        0        0   393608 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/1_19.json
+-rw-r--r--   0        0        0   396856 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/1_20.json
+-rw-r--r--   0        0        0        0 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/__init__.py
+-rw-r--r--   0        0        0      369 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/inline_function_tag.json
+-rw-r--r--   0        0        0     7984 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/nesting.json
+-rw-r--r--   0        0        0      526 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/resources/patches.json
+-rw-r--r--   0        0        0    12620 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/serialize.py
+-rw-r--r--   0        0        0     3440 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/spec.py
+-rw-r--r--   0        0        0     6393 2024-04-28 23:54:56.641248 mecha-0.94.0/mecha/utils.py
+-rw-r--r--   0        0        0     1293 2024-04-28 23:55:42.141951 mecha-0.94.0/pyproject.toml
+-rw-r--r--   0        0        0     9352 1970-01-01 00:00:00.000000 mecha-0.94.0/PKG-INFO
```

### Comparing `mecha-0.93.1/LICENSE` & `mecha-0.94.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/README.md` & `mecha-0.94.0/README.md`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/api.py` & `mecha-0.94.0/mecha/api.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/ast.py` & `mecha-0.94.0/mecha/ast.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/cli.py` & `mecha-0.94.0/mecha/cli.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/commands.py` & `mecha-0.94.0/mecha/commands.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/config.py` & `mecha-0.94.0/mecha/config.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/annotate_diagnostics.py` & `mecha-0.94.0/mecha/contrib/annotate_diagnostics.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/bake_macros.py` & `mecha-0.94.0/mecha/contrib/bake_macros.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/debug_ast.py` & `mecha-0.94.0/mecha/contrib/debug_ast.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/embed.py` & `mecha-0.94.0/mecha/contrib/embed.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/implicit_execute.py` & `mecha-0.94.0/mecha/contrib/implicit_execute.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/inline_function_tag.py` & `mecha-0.94.0/mecha/contrib/inline_function_tag.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/json_files.py` & `mecha-0.94.0/mecha/contrib/json_files.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/lint_basic.py` & `mecha-0.94.0/mecha/contrib/lint_basic.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/messages.py` & `mecha-0.94.0/mecha/contrib/messages.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/nested_location.py` & `mecha-0.94.0/mecha/contrib/nested_location.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/nested_resources.py` & `mecha-0.94.0/mecha/contrib/nested_resources.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/nested_yaml.py` & `mecha-0.94.0/mecha/contrib/nested_yaml.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/nesting.py` & `mecha-0.94.0/mecha/contrib/nesting.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/raw.py` & `mecha-0.94.0/mecha/contrib/raw.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/relative_location.py` & `mecha-0.94.0/mecha/contrib/relative_location.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/source_map.py` & `mecha-0.94.0/mecha/contrib/source_map.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/statistics.py` & `mecha-0.94.0/mecha/contrib/statistics.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/contrib/validation/mcdoc.py` & `mecha-0.94.0/mecha/contrib/validation/mcdoc.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/database.py` & `mecha-0.94.0/mecha/database.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/diagnostic.py` & `mecha-0.94.0/mecha/diagnostic.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/dispatch.py` & `mecha-0.94.0/mecha/dispatch.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/parse.py` & `mecha-0.94.0/mecha/parse.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/preprocess.py` & `mecha-0.94.0/mecha/preprocess.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/prototype.py` & `mecha-0.94.0/mecha/prototype.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/resources/1_16.json` & `mecha-0.94.0/mecha/resources/1_16.json`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/resources/1_17.json` & `mecha-0.94.0/mecha/resources/1_17.json`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/resources/1_18.json` & `mecha-0.94.0/mecha/resources/1_18.json`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/resources/1_19.json` & `mecha-0.94.0/mecha/resources/1_19.json`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/resources/1_20.json` & `mecha-0.94.0/mecha/resources/1_20.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999483824228702%*

 * *Differences: {"'children'": "{'attribute': {'children': {'target': {'children': {'attribute': {'children': "*

 * *               "{'modifier': {'children': {'add': {'children': {'uuid': {'children': {'name': "*

 * *               "{'children': {'value': {'children': {replace: OrderedDict([('add_multiplied_base', "*

 * *               "OrderedDict([('type', 'literal'), ('executable', True)])), "*

 * *               "('add_multiplied_total', OrderedDict([('type', 'literal'), ('executable', "*

 * *               "True)])), ('add_value', OrderedDic […]*

```diff
@@ -192,23 +192,23 @@
                                             "children": {
                                                 "uuid": {
                                                     "children": {
                                                         "name": {
                                                             "children": {
                                                                 "value": {
                                                                     "children": {
-                                                                        "add": {
+                                                                        "add_multiplied_base": {
                                                                             "executable": true,
                                                                             "type": "literal"
                                                                         },
-                                                                        "multiply": {
+                                                                        "add_multiplied_total": {
                                                                             "executable": true,
                                                                             "type": "literal"
                                                                         },
-                                                                        "multiply_base": {
+                                                                        "add_value": {
                                                                             "executable": true,
                                                                             "type": "literal"
                                                                         }
                                                                     },
                                                                     "parser": "brigadier:double",
                                                                     "type": "argument"
                                                                 }
@@ -4080,15 +4080,15 @@
                                                             "parser": "brigadier:bool",
                                                             "type": "argument"
                                                         }
                                                     },
                                                     "executable": true,
                                                     "parser": "brigadier:integer",
                                                     "properties": {
-                                                        "max": 127,
+                                                        "max": 255,
                                                         "min": 0
                                                     },
                                                     "type": "argument"
                                                 }
                                             },
                                             "executable": true,
                                             "type": "literal"
@@ -4102,15 +4102,15 @@
                                                             "parser": "brigadier:bool",
                                                             "type": "argument"
                                                         }
                                                     },
                                                     "executable": true,
                                                     "parser": "brigadier:integer",
                                                     "properties": {
-                                                        "max": 127,
+                                                        "max": 255,
                                                         "min": 0
                                                     },
                                                     "type": "argument"
                                                 }
                                             },
                                             "executable": true,
                                             "parser": "brigadier:integer",
@@ -4451,14 +4451,73 @@
                                         "execute"
                                     ],
                                     "type": "argument"
                                 }
                             },
                             "type": "literal"
                         },
+                        "items": {
+                            "children": {
+                                "block": {
+                                    "children": {
+                                        "pos": {
+                                            "children": {
+                                                "slots": {
+                                                    "children": {
+                                                        "item_predicate": {
+                                                            "executable": true,
+                                                            "parser": "minecraft:item_predicate",
+                                                            "redirect": [
+                                                                "execute"
+                                                            ],
+                                                            "type": "argument"
+                                                        }
+                                                    },
+                                                    "parser": "minecraft:item_slots",
+                                                    "type": "argument"
+                                                }
+                                            },
+                                            "parser": "minecraft:block_pos",
+                                            "type": "argument"
+                                        }
+                                    },
+                                    "type": "literal"
+                                },
+                                "entity": {
+                                    "children": {
+                                        "entities": {
+                                            "children": {
+                                                "slots": {
+                                                    "children": {
+                                                        "item_predicate": {
+                                                            "executable": true,
+                                                            "parser": "minecraft:item_predicate",
+                                                            "redirect": [
+                                                                "execute"
+                                                            ],
+                                                            "type": "argument"
+                                                        }
+                                                    },
+                                                    "parser": "minecraft:item_slots",
+                                                    "type": "argument"
+                                                }
+                                            },
+                                            "parser": "minecraft:entity",
+                                            "properties": {
+                                                "amount": "multiple",
+                                                "type": "entities"
+                                            },
+                                            "type": "argument"
+                                        }
+                                    },
+                                    "type": "literal"
+                                }
+                            },
+                            "type": "literal"
+                        },
                         "loaded": {
                             "children": {
                                 "pos": {
                                     "executable": true,
                                     "parser": "minecraft:block_pos",
                                     "redirect": [
                                         "execute"
@@ -4468,15 +4527,15 @@
                             },
                             "type": "literal"
                         },
                         "predicate": {
                             "children": {
                                 "predicate": {
                                     "executable": true,
-                                    "parser": "minecraft:resource_location",
+                                    "parser": "minecraft:loot_predicate",
                                     "redirect": [
                                         "execute"
                                     ],
                                     "type": "argument"
                                 }
                             },
                             "type": "literal"
@@ -5607,14 +5666,73 @@
                                         "execute"
                                     ],
                                     "type": "argument"
                                 }
                             },
                             "type": "literal"
                         },
+                        "items": {
+                            "children": {
+                                "block": {
+                                    "children": {
+                                        "pos": {
+                                            "children": {
+                                                "slots": {
+                                                    "children": {
+                                                        "item_predicate": {
+                                                            "executable": true,
+                                                            "parser": "minecraft:item_predicate",
+                                                            "redirect": [
+                                                                "execute"
+                                                            ],
+                                                            "type": "argument"
+                                                        }
+                                                    },
+                                                    "parser": "minecraft:item_slots",
+                                                    "type": "argument"
+                                                }
+                                            },
+                                            "parser": "minecraft:block_pos",
+                                            "type": "argument"
+                                        }
+                                    },
+                                    "type": "literal"
+                                },
+                                "entity": {
+                                    "children": {
+                                        "entities": {
+                                            "children": {
+                                                "slots": {
+                                                    "children": {
+                                                        "item_predicate": {
+                                                            "executable": true,
+                                                            "parser": "minecraft:item_predicate",
+                                                            "redirect": [
+                                                                "execute"
+                                                            ],
+                                                            "type": "argument"
+                                                        }
+                                                    },
+                                                    "parser": "minecraft:item_slots",
+                                                    "type": "argument"
+                                                }
+                                            },
+                                            "parser": "minecraft:entity",
+                                            "properties": {
+                                                "amount": "multiple",
+                                                "type": "entities"
+                                            },
+                                            "type": "argument"
+                                        }
+                                    },
+                                    "type": "literal"
+                                }
+                            },
+                            "type": "literal"
+                        },
                         "loaded": {
                             "children": {
                                 "pos": {
                                     "executable": true,
                                     "parser": "minecraft:block_pos",
                                     "redirect": [
                                         "execute"
@@ -5624,15 +5742,15 @@
                             },
                             "type": "literal"
                         },
                         "predicate": {
                             "children": {
                                 "predicate": {
                                     "executable": true,
-                                    "parser": "minecraft:resource_location",
+                                    "parser": "minecraft:loot_predicate",
                                     "redirect": [
                                         "execute"
                                     ],
                                     "type": "argument"
                                 }
                             },
                             "type": "literal"
@@ -6742,15 +6860,15 @@
                             "children": {
                                 "pos": {
                                     "children": {
                                         "slot": {
                                             "children": {
                                                 "modifier": {
                                                     "executable": true,
-                                                    "parser": "minecraft:resource_location",
+                                                    "parser": "minecraft:loot_modifier",
                                                     "type": "argument"
                                                 }
                                             },
                                             "parser": "minecraft:item_slot",
                                             "type": "argument"
                                         }
                                     },
@@ -6764,15 +6882,15 @@
                             "children": {
                                 "targets": {
                                     "children": {
                                         "slot": {
                                             "children": {
                                                 "modifier": {
                                                     "executable": true,
-                                                    "parser": "minecraft:resource_location",
+                                                    "parser": "minecraft:loot_modifier",
                                                     "type": "argument"
                                                 }
                                             },
                                             "parser": "minecraft:item_slot",
                                             "type": "argument"
                                         }
                                     },
@@ -6803,15 +6921,15 @@
                                                             "children": {
                                                                 "source": {
                                                                     "children": {
                                                                         "sourceSlot": {
                                                                             "children": {
                                                                                 "modifier": {
                                                                                     "executable": true,
-                                                                                    "parser": "minecraft:resource_location",
+                                                                                    "parser": "minecraft:loot_modifier",
                                                                                     "type": "argument"
                                                                                 }
                                                                             },
                                                                             "executable": true,
                                                                             "parser": "minecraft:item_slot",
                                                                             "type": "argument"
                                                                         }
@@ -6826,15 +6944,15 @@
                                                             "children": {
                                                                 "source": {
                                                                     "children": {
                                                                         "sourceSlot": {
                                                                             "children": {
                                                                                 "modifier": {
                                                                                     "executable": true,
-                                                                                    "parser": "minecraft:resource_location",
+                                                                                    "parser": "minecraft:loot_modifier",
                                                                                     "type": "argument"
                                                                                 }
                                                                             },
                                                                             "executable": true,
                                                                             "parser": "minecraft:item_slot",
                                                                             "type": "argument"
                                                                         }
@@ -6856,15 +6974,15 @@
                                                     "children": {
                                                         "item": {
                                                             "children": {
                                                                 "count": {
                                                                     "executable": true,
                                                                     "parser": "brigadier:integer",
                                                                     "properties": {
-                                                                        "max": 64,
+                                                                        "max": 99,
                                                                         "min": 1
                                                                     },
                                                                     "type": "argument"
                                                                 }
                                                             },
                                                             "executable": true,
                                                             "parser": "minecraft:item_stack",
@@ -6896,15 +7014,15 @@
                                                             "children": {
                                                                 "source": {
                                                                     "children": {
                                                                         "sourceSlot": {
                                                                             "children": {
                                                                                 "modifier": {
                                                                                     "executable": true,
-                                                                                    "parser": "minecraft:resource_location",
+                                                                                    "parser": "minecraft:loot_modifier",
                                                                                     "type": "argument"
                                                                                 }
                                                                             },
                                                                             "executable": true,
                                                                             "parser": "minecraft:item_slot",
                                                                             "type": "argument"
                                                                         }
@@ -6919,15 +7037,15 @@
                                                             "children": {
                                                                 "source": {
                                                                     "children": {
                                                                         "sourceSlot": {
                                                                             "children": {
                                                                                 "modifier": {
                                                                                     "executable": true,
-                                                                                    "parser": "minecraft:resource_location",
+                                                                                    "parser": "minecraft:loot_modifier",
                                                                                     "type": "argument"
                                                                                 }
                                                                             },
                                                                             "executable": true,
                                                                             "parser": "minecraft:item_slot",
                                                                             "type": "argument"
                                                                         }
@@ -6949,15 +7067,15 @@
                                                     "children": {
                                                         "item": {
                                                             "children": {
                                                                 "count": {
                                                                     "executable": true,
                                                                     "parser": "brigadier:integer",
                                                                     "properties": {
-                                                                        "max": 64,
+                                                                        "max": 99,
                                                                         "min": 1
                                                                     },
                                                                     "type": "argument"
                                                                 }
                                                             },
                                                             "executable": true,
                                                             "parser": "minecraft:item_stack",
@@ -7117,15 +7235,15 @@
                                                         }
                                                     },
                                                     "executable": true,
                                                     "parser": "minecraft:block_pos",
                                                     "type": "argument"
                                                 }
                                             },
-                                            "parser": "minecraft:resource_location",
+                                            "parser": "minecraft:loot_table",
                                             "type": "argument"
                                         }
                                     },
                                     "type": "literal"
                                 },
                                 "kill": {
                                     "children": {
@@ -7141,15 +7259,15 @@
                                     },
                                     "type": "literal"
                                 },
                                 "loot": {
                                     "children": {
                                         "loot_table": {
                                             "executable": true,
-                                            "parser": "minecraft:resource_location",
+                                            "parser": "minecraft:loot_table",
                                             "type": "argument"
                                         }
                                     },
                                     "type": "literal"
                                 },
                                 "mine": {
                                     "children": {
@@ -7212,15 +7330,15 @@
                                                         }
                                                     },
                                                     "executable": true,
                                                     "parser": "minecraft:block_pos",
                                                     "type": "argument"
                                                 }
                                             },
-                                            "parser": "minecraft:resource_location",
+                                            "parser": "minecraft:loot_table",
                                             "type": "argument"
                                         }
                                     },
                                     "type": "literal"
                                 },
                                 "kill": {
                                     "children": {
@@ -7236,15 +7354,15 @@
                                     },
                                     "type": "literal"
                                 },
                                 "loot": {
                                     "children": {
                                         "loot_table": {
                                             "executable": true,
-                                            "parser": "minecraft:resource_location",
+                                            "parser": "minecraft:loot_table",
                                             "type": "argument"
                                         }
                                     },
                                     "type": "literal"
                                 },
                                 "mine": {
                                     "children": {
@@ -7309,15 +7427,15 @@
                                                                                 }
                                                                             },
                                                                             "executable": true,
                                                                             "parser": "minecraft:block_pos",
                                                                             "type": "argument"
                                                                         }
                                                                     },
-                                                                    "parser": "minecraft:resource_location",
+                                                                    "parser": "minecraft:loot_table",
                                                                     "type": "argument"
                                                                 }
                                                             },
                                                             "type": "literal"
                                                         },
                                                         "kill": {
                                                             "children": {
@@ -7333,15 +7451,15 @@
                                                             },
                                                             "type": "literal"
                                                         },
                                                         "loot": {
                                                             "children": {
                                                                 "loot_table": {
                                                                     "executable": true,
-                                                                    "parser": "minecraft:resource_location",
+                                                                    "parser": "minecraft:loot_table",
                                                                     "type": "argument"
                                                                 }
                                                             },
                                                             "type": "literal"
                                                         },
                                                         "mine": {
                                                             "children": {
@@ -7396,15 +7514,15 @@
                                                                         }
                                                                     },
                                                                     "executable": true,
                                                                     "parser": "minecraft:block_pos",
                                                                     "type": "argument"
                                                                 }
                                                             },
-                                                            "parser": "minecraft:resource_location",
+                                                            "parser": "minecraft:loot_table",
                                                             "type": "argument"
                                                         }
                                                     },
                                                     "type": "literal"
                                                 },
                                                 "kill": {
                                                     "children": {
@@ -7420,15 +7538,15 @@
                                                     },
                                                     "type": "literal"
                                                 },
                                                 "loot": {
                                                     "children": {
                                                         "loot_table": {
                                                             "executable": true,
-                                                            "parser": "minecraft:resource_location",
+                                                            "parser": "minecraft:loot_table",
                                                             "type": "argument"
                                                         }
                                                     },
                                                     "type": "literal"
                                                 },
                                                 "mine": {
                                                     "children": {
@@ -7495,15 +7613,15 @@
                                                                                 }
                                                                             },
                                                                             "executable": true,
                                                                             "parser": "minecraft:block_pos",
                                                                             "type": "argument"
                                                                         }
                                                                     },
-                                                                    "parser": "minecraft:resource_location",
+                                                                    "parser": "minecraft:loot_table",
                                                                     "type": "argument"
                                                                 }
                                                             },
                                                             "type": "literal"
                                                         },
                                                         "kill": {
                                                             "children": {
@@ -7519,15 +7637,15 @@
                                                             },
                                                             "type": "literal"
                                                         },
                                                         "loot": {
                                                             "children": {
                                                                 "loot_table": {
                                                                     "executable": true,
-                                                                    "parser": "minecraft:resource_location",
+                                                                    "parser": "minecraft:loot_table",
                                                                     "type": "argument"
                                                                 }
                                                             },
                                                             "type": "literal"
                                                         },
                                                         "mine": {
                                                             "children": {
@@ -7582,15 +7700,15 @@
                                                                         }
                                                                     },
                                                                     "executable": true,
                                                                     "parser": "minecraft:block_pos",
                                                                     "type": "argument"
                                                                 }
                                                             },
-                                                            "parser": "minecraft:resource_location",
+                                                            "parser": "minecraft:loot_table",
                                                             "type": "argument"
                                                         }
                                                     },
                                                     "type": "literal"
                                                 },
                                                 "kill": {
                                                     "children": {
@@ -7606,15 +7724,15 @@
                                                     },
                                                     "type": "literal"
                                                 },
                                                 "loot": {
                                                     "children": {
                                                         "loot_table": {
                                                             "executable": true,
-                                                            "parser": "minecraft:resource_location",
+                                                            "parser": "minecraft:loot_table",
                                                             "type": "argument"
                                                         }
                                                     },
                                                     "type": "literal"
                                                 },
                                                 "mine": {
                                                     "children": {
@@ -7684,15 +7802,15 @@
                                                         }
                                                     },
                                                     "executable": true,
                                                     "parser": "minecraft:block_pos",
                                                     "type": "argument"
                                                 }
                                             },
-                                            "parser": "minecraft:resource_location",
+                                            "parser": "minecraft:loot_table",
                                             "type": "argument"
                                         }
                                     },
                                     "type": "literal"
                                 },
                                 "kill": {
                                     "children": {
@@ -7708,15 +7826,15 @@
                                     },
                                     "type": "literal"
                                 },
                                 "loot": {
                                     "children": {
                                         "loot_table": {
                                             "executable": true,
-                                            "parser": "minecraft:resource_location",
+                                            "parser": "minecraft:loot_table",
                                             "type": "argument"
                                         }
                                     },
                                     "type": "literal"
                                 },
                                 "mine": {
                                     "children": {
@@ -7938,15 +8056,15 @@
                                                     "parser": "minecraft:block_pos",
                                                     "type": "argument"
                                                 }
                                             },
                                             "executable": true,
                                             "parser": "brigadier:integer",
                                             "properties": {
-                                                "max": 7,
+                                                "max": 20,
                                                 "min": 1
                                             },
                                             "type": "argument"
                                         }
                                     },
                                     "parser": "minecraft:resource_location",
                                     "type": "argument"
@@ -8084,14 +8202,15 @@
                                     "properties": {
                                         "amount": "multiple",
                                         "type": "players"
                                     },
                                     "type": "argument"
                                 }
                             },
+                            "executable": true,
                             "type": "literal"
                         },
                         "block": {
                             "children": {
                                 "targets": {
                                     "children": {
                                         "pos": {
@@ -8137,14 +8256,15 @@
                                     "properties": {
                                         "amount": "multiple",
                                         "type": "players"
                                     },
                                     "type": "argument"
                                 }
                             },
+                            "executable": true,
                             "type": "literal"
                         },
                         "hostile": {
                             "children": {
                                 "targets": {
                                     "children": {
                                         "pos": {
@@ -8190,14 +8310,15 @@
                                     "properties": {
                                         "amount": "multiple",
                                         "type": "players"
                                     },
                                     "type": "argument"
                                 }
                             },
+                            "executable": true,
                             "type": "literal"
                         },
                         "master": {
                             "children": {
                                 "targets": {
                                     "children": {
                                         "pos": {
@@ -8243,14 +8364,15 @@
                                     "properties": {
                                         "amount": "multiple",
                                         "type": "players"
                                     },
                                     "type": "argument"
                                 }
                             },
+                            "executable": true,
                             "type": "literal"
                         },
                         "music": {
                             "children": {
                                 "targets": {
                                     "children": {
                                         "pos": {
@@ -8296,14 +8418,15 @@
                                     "properties": {
                                         "amount": "multiple",
                                         "type": "players"
                                     },
                                     "type": "argument"
                                 }
                             },
+                            "executable": true,
                             "type": "literal"
                         },
                         "neutral": {
                             "children": {
                                 "targets": {
                                     "children": {
                                         "pos": {
@@ -8349,14 +8472,15 @@
                                     "properties": {
                                         "amount": "multiple",
                                         "type": "players"
                                     },
                                     "type": "argument"
                                 }
                             },
+                            "executable": true,
                             "type": "literal"
                         },
                         "player": {
                             "children": {
                                 "targets": {
                                     "children": {
                                         "pos": {
@@ -8402,14 +8526,15 @@
                                     "properties": {
                                         "amount": "multiple",
                                         "type": "players"
                                     },
                                     "type": "argument"
                                 }
                             },
+                            "executable": true,
                             "type": "literal"
                         },
                         "record": {
                             "children": {
                                 "targets": {
                                     "children": {
                                         "pos": {
@@ -8455,14 +8580,15 @@
                                     "properties": {
                                         "amount": "multiple",
                                         "type": "players"
                                     },
                                     "type": "argument"
                                 }
                             },
+                            "executable": true,
                             "type": "literal"
                         },
                         "voice": {
                             "children": {
                                 "targets": {
                                     "children": {
                                         "pos": {
@@ -8508,14 +8634,15 @@
                                     "properties": {
                                         "amount": "multiple",
                                         "type": "players"
                                     },
                                     "type": "argument"
                                 }
                             },
+                            "executable": true,
                             "type": "literal"
                         },
                         "weather": {
                             "children": {
                                 "targets": {
                                     "children": {
                                         "pos": {
@@ -8561,17 +8688,19 @@
                                     "properties": {
                                         "amount": "multiple",
                                         "type": "players"
                                     },
                                     "type": "argument"
                                 }
                             },
+                            "executable": true,
                             "type": "literal"
                         }
                     },
+                    "executable": true,
                     "parser": "minecraft:resource_location",
                     "type": "argument"
                 }
             },
             "type": "literal"
         },
         "publish": {
```

### Comparing `mecha-0.93.1/mecha/resources/nesting.json` & `mecha-0.94.0/mecha/resources/nesting.json`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/resources/patches.json` & `mecha-0.94.0/mecha/resources/patches.json`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/serialize.py` & `mecha-0.94.0/mecha/serialize.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/spec.py` & `mecha-0.94.0/mecha/spec.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/mecha/utils.py` & `mecha-0.94.0/mecha/utils.py`

 * *Files identical despite different names*

### Comparing `mecha-0.93.1/pyproject.toml` & `mecha-0.94.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mecha"
-version = "0.93.1"
+version = "0.94.0"
 description = "A powerful Minecraft command library"
 authors = ["Valentin Berlier <berlier.v@gmail.com>"]
 license = "MIT"
 
 homepage = "https://github.com/mcbeet/mecha"
 repository = "https://github.com/mcbeet/mecha"
 documentation = "https://github.com/mcbeet/mecha"
@@ -19,15 +19,15 @@
   "mcfunction"
 ]
 
 include = ["mecha/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-beet = ">=0.104.0"
+beet = ">=0.105.0"
 tokenstream = "^1.7.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 pytest = "^7.4.3"
 isort = "^5.12.0"
 python-semantic-release = "^7.33.3"
```

### Comparing `mecha-0.93.1/PKG-INFO` & `mecha-0.94.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: mecha
-Version: 0.93.1
+Version: 0.94.0
 Summary: A powerful Minecraft command library
 Home-page: https://github.com/mcbeet/mecha
 License: MIT
 Keywords: beet,minecraft,datapack,minecraft-commands,mcfunction
 Author: Valentin Berlier
 Author-email: berlier.v@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beet (>=0.104.0)
+Requires-Dist: beet (>=0.105.0)
 Requires-Dist: tokenstream (>=1.7.0,<2.0.0)
 Project-URL: Documentation, https://github.com/mcbeet/mecha
 Project-URL: Repository, https://github.com/mcbeet/mecha
 Description-Content-Type: text/markdown
 
 <img align="right" src="https://raw.githubusercontent.com/mcbeet/mecha/main/logo.png" alt="logo" width="76">
```

