# Comparing `tmp/allowed-1.3.0.tar.gz` & `tmp/allowed-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allowed-1.3.0.tar", max compression
+gzip compressed data, was "allowed-1.4.0.tar", max compression
```

## Comparing `allowed-1.3.0.tar` & `allowed-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3070 2024-02-10 11:49:42.096793 allowed-1.3.0/README.md
--rw-r--r--   0        0        0        0 2024-02-10 11:49:42.097631 allowed-1.3.0/allowed/__init__.py
--rw-r--r--   0        0        0       33 2024-02-10 11:49:42.098691 allowed-1.3.0/allowed/__main__.py
--rw-r--r--   0        0        0    23478 2024-02-13 11:39:39.536660 allowed-1.3.0/allowed/allowed.py
--rw-r--r--   0        0        0     1514 2024-02-10 11:49:42.100546 allowed-1.3.0/allowed/m269.json
--rw-r--r--   0        0        0      754 2024-02-10 11:49:42.101301 allowed-1.3.0/allowed/tm112.json
--rw-r--r--   0        0        0     1522 2024-02-13 11:39:28.758218 allowed-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 allowed-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3070 2024-02-10 11:49:42.096793 allowed-1.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-02-10 11:49:42.097631 allowed-1.4.0/allowed/__init__.py
+-rw-r--r--   0        0        0       33 2024-02-10 11:49:42.098691 allowed-1.4.0/allowed/__main__.py
+-rw-r--r--   0        0        0    26130 2024-04-29 12:24:24.435431 allowed-1.4.0/allowed/allowed.py
+-rw-r--r--   0        0        0     1488 2024-04-29 07:14:30.950701 allowed-1.4.0/allowed/m269.json
+-rw-r--r--   0        0        0      735 2024-04-29 07:14:38.862902 allowed-1.4.0/allowed/tm112.json
+-rw-r--r--   0        0        0     1522 2024-04-29 12:30:46.096764 allowed-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3853 1970-01-01 00:00:00.000000 allowed-1.4.0/PKG-INFO
```

### Comparing `allowed-1.3.0/README.md` & `allowed-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `allowed-1.3.0/allowed/allowed.py` & `allowed-1.4.0/allowed/allowed.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 """Check that Python and notebook files only use the allowed constructs."""
 
-__version__ = "1.3.0"  # same as in pyproject.toml
+__version__ = "1.4.0"  # same as in pyproject.toml
 
 import argparse
 import ast
 import json
 import os
 import re
 import sys
 from pathlib import Path
 
+issues = 0  # number of issues (unknown constructs) found
+py_checked = 0  # number of Python files checked
+nb_checked = 0  # number of notebooks checked
+unchecked = 0  # number of .py and .ipynb files skipped due to syntax or other errors
+
 try:
     import pytype
     from pytype.tools.annotate_ast import annotate_ast
 
     PYTYPE_OPTIONS = pytype.config.Options.create(python_version=(3, 10))
     PYTYPE_INSTALLED = True
 except ImportError:
@@ -279,17 +284,33 @@
         )
     return ""
 
 
 # ----- auxiliary functions -----
 
 
+def plural(number: int) -> str:
+    """Return 's' or '' depending on number."""
+    return "" if number == 1 else "s"
+
+
+def show_units(filename: str, last_unit: int) -> None:
+    """Print a message about the units being checked."""
+    if last_unit == 1:
+        units = "unit 1"
+    elif last_unit > 0:
+        units = f"units 1–{last_unit}"  # noqa: RUF001 (it's an en-dash)
+    else:
+        units = "all units"
+    print(f"INFO: checking {filename} against {units}")
+
+
 def get_unit(filename: str) -> int:
     """Return the file's unit or zero (consider all units)."""
-    if FILE_UNIT and (match := re.match(FILE_UNIT, filename)):
+    if FILE_UNIT and (match := re.search(FILE_UNIT, filename)):
         return int(match.group(1))
     return 0
 
 
 def get_language(last_unit: int) -> tuple[type[ast.AST], ...]:
     """Return the allowed language elements up to the given unit.
 
@@ -385,17 +406,14 @@
     return hasattr(node, "lineno") and source[node.lineno - 1].rstrip().endswith(
         "# allowed"
     )
 
 
 # ----- main functions -----
 
-read_nb = False  # remember if a notebook was read
-read_py = False  # remember if Python file was read
-
 
 def check_tree(
     tree: ast.AST,
     constructs: tuple,
     source: list,
     line_cell_map: list,
     errors: list,
@@ -478,87 +496,100 @@
 
 
 def check_folder(
     folder: str,
     last_unit: int,
     check_method_calls: bool,  # noqa: FBT001
     report_first: bool,  # noqa: FBT001
+    verbose: bool,  # noqa: FBT001
 ) -> None:
     """Check all Python files in `folder` and its subfolders."""
     global_constructs = get_constructs(last_unit)
     for current_folder, subfolders, files in os.walk(folder):
         subfolders.sort()
         for filename in sorted(files):
             if filename.endswith((".py", ".ipynb")):
+                fullname = str(Path(current_folder) / filename)
                 if not last_unit and (file_unit := get_unit(filename)):
                     constructs = get_constructs(file_unit)
+                    if verbose:
+                        show_units(fullname, file_unit)
                 else:
                     constructs = global_constructs
-                fullname = str(Path(current_folder) / filename)
+                    if verbose:
+                        show_units(fullname, last_unit)
                 check_file(fullname, constructs, check_method_calls, report_first)
 
 
 def check_file(
     filename: str,
     constructs: tuple,
     check_method_calls: bool,  # noqa: FBT001
     report_first: bool,  # noqa: FBT001
 ) -> None:
     """Check that the file only uses the allowed constructs."""
-    global read_nb, read_py
+    global py_checked, nb_checked, unchecked, issues
 
     try:
         with Path(filename).open(encoding="utf-8", errors="surrogateescape") as file:
             if filename.endswith(".ipynb"):
                 source, line_cell_map, errors = read_notebook(file.read())
-                read_nb = True
             else:
                 source = file.read()
                 line_cell_map = []
                 errors = []
-                read_py = True
         if check_method_calls and METHODS:
             tree = annotate_ast.annotate_source(source, ast, PYTYPE_OPTIONS)
         else:
             tree = ast.parse(source)
         check_tree(tree, constructs, source.splitlines(), line_cell_map, errors)
         errors.sort()
-        messages = set()
+        messages = set()  # for --first option: the unique messages (except errors)
         last_error = None
         for cell, line, message in errors:
             if (cell, line, message) != last_error and message not in messages:
                 if cell:
                     print(f"{filename}:cell_{cell}:{line}: {message}")
                 else:
                     print(f"{filename}:{line}: {message}")
-                if report_first and message != SYNTAX_MSG:
+                # don't count syntax errors as unknown constructs
+                if "ERROR" not in message:
+                    issues += 1
+                if report_first and "ERROR" not in message:
                     messages.add(message)
                 last_error = (cell, line, message)
+        if filename.endswith(".py"):
+            py_checked += 1
+        else:
+            nb_checked += 1
     except OSError as error:
         print(f"{filename}: OS ERROR: {error.strerror}")
+        unchecked += 1
     except SyntaxError as error:
         print(f"{filename}:{error.lineno}: SYNTAX ERROR: {error.msg}")
+        unchecked += 1
     except UnicodeError as error:
         print(f"{filename}: UNICODE ERROR: {error}")
+        unchecked += 1
     except json.decoder.JSONDecodeError as error:
         print(f"{filename}:{error.lineno}: FORMAT ERROR: invalid notebook format")
+        unchecked += 1
     except ValueError as error:
         print(f"{filename}: VALUE ERROR: {error}")
+        unchecked += 1
     except annotate_ast.PytypeError as error:
         #  write 'file:n: error' instead of 'Error reading file ... at line n: error'
         message = str(error)
         if match := re.match(r"Error .* at line (\d+): (.*)", message):
             line = int(match.group(1))
             message = match.group(2)
             print(f"{filename}:{line}: PYTYPE ERROR: {message}")
         else:
             print(f"{filename}: PYTYPE ERROR: {message}")
-
-
-SYNTAX_MSG = "SYNTAX ERROR: this cell wasn't checked"
+        unchecked += 1
 
 
 def read_notebook(file_contents: str) -> tuple[str, list, list]:
     """Return a triple (source, map, errors).
 
     source: the concatenated lines of the code cells without syntax errors
     map: an array mapping absolute lines 1, 2, ... to (cell, relative line) pairs
@@ -578,15 +609,15 @@
                 if IPYTHON_INSTALLED:
                     cell_source = Transformer().transform_cell(cell_source)
                 ast.parse(cell_source)
                 source_list.append(cell_source)
                 for cell_line_num in range(1, cell_source.count("\n") + 2):
                     line_cell_map.append((cell_num, cell_line_num))  # noqa: PERF401
             except SyntaxError as error:
-                errors.append((cell_num, error.lineno, SYNTAX_MSG))
+                errors.append((cell_num, error.lineno, f"SYNTAX ERROR: {error.msg}"))
     source_str = "\n".join(source_list)
     return source_str, line_cell_map, errors
 
 
 # ---- main program ----
 
 
@@ -621,39 +652,56 @@
         "-u",
         "--unit",
         type=int,
         default=0,
         help="only allow constructs from units 1 to UNIT (default: all units)",
     )
     argparser.add_argument(
+        "--file-unit",
+        default="",
+        help="regular expression of unit number in file name (default: '')",
+    )
+    argparser.add_argument(
         "-c",
         "--config",
         default="m269.json",
         help="allow the constructs given in CONFIG (default: m269.json)",
     )
+    argparser.add_argument(
+        "-v",
+        "--verbose",
+        action="store_true",
+        help="show additional info as files are processed",
+    )
     argparser.add_argument("file_or_folder", nargs="+", help="file or folder to check")
     args = argparser.parse_args()
 
     if args.methods and not PYTYPE_INSTALLED:
         print("ERROR: can't check method calls (pytype not installed)")
         sys.exit(1)
     if args.unit < 0:
         print("ERROR: unit must be positive")
         sys.exit(1)
 
     try:
-        for file in (Path(args.config), Path(__file__).parent / args.config):
+        filename = args.config
+        if not filename.endswith(".json"):
+            filename += ".json"
+        # Look for configuration locally, then in this script's folder.
+        for file in (Path(filename), Path(__file__).parent / filename):
             if file.exists():
                 with file.open() as config_file:
                     configuration = json.load(config_file)
+                    if args.verbose:
+                        print(f"INFO: using configuration {file.resolve()}")
                     break
         else:
-            print(f"CONFIGURATION ERROR: {args.config} not found")
+            print(f"CONFIGURATION ERROR: {filename} not found")
             sys.exit(1)
-        FILE_UNIT = configuration.get("FILE_UNIT", "")
+        FILE_UNIT = args.file_unit
         LANGUAGE = {}
         for key, value in configuration["LANGUAGE"].items():
             if not isinstance(value, list):
                 raise TypeError
             LANGUAGE[int(key)] = value
         IMPORTS = {}
         for key, value in configuration["IMPORTS"].items():
@@ -673,29 +721,53 @@
         sys.exit(1)
     if error := check_imports():
         print(error)
         sys.exit(1)
 
     for name in args.file_or_folder:
         if Path(name).is_dir():
-            check_folder(name, args.unit, args.methods, args.first)
+            check_folder(name, args.unit, args.methods, args.first, args.verbose)
         elif name.endswith((".py", ".ipynb")):
             unit = args.unit if args.unit else get_unit(Path(name).name)
+            if args.verbose:
+                show_units(name, unit)
             check_file(name, get_constructs(unit), args.methods, args.first)
         else:
             print(f"WARNING: {name} skipped: not a folder, Python file or notebook")
 
-    if (read_py or read_nb) and not args.methods:
+    if args.verbose:
+        print(
+            "INFO: checked",
+            f"{py_checked} Python file{plural(py_checked)} and",
+            f"{nb_checked} notebook{plural(nb_checked)}",
+        )
+        if issues:
+            print(
+                f"INFO: the {issues} Python construct{plural(issues)}",
+                f"listed above {'are' if issues > 1 else 'is'} not allowed",
+            )
+        elif nb_checked or py_checked:
+            print("INFO: found no disallowed Python constructs")
+        if unchecked:
+            print(
+                f"INFO: didn't check {unchecked} Python",
+                f"file{plural(unchecked)} or notebook{plural(unchecked)}",
+                "due to syntax or other errors",
+            )
+    if args.first and issues:
+        print(
+            "WARNING:",
+            "other occurrences of the listed constructs may exist (don't use option -f)",  # noqa: E501
+        )
+    if (py_checked or nb_checked) and not args.methods:
         print(
             "WARNING: didn't check method calls",
             "(use option -m)" if PYTYPE_INSTALLED else "(pytype not installed)",
         )
-    if read_nb and not IPYTHON_INSTALLED:
+    if nb_checked and not IPYTHON_INSTALLED:
         print(
-            "WARNING: didn't check notebook cells with %-commands (IPython not installed)" # noqa: E501
+            "WARNING: didn't check notebook cells with %-commands (IPython not installed)"  # noqa: E501
         )
-    if (read_py or read_nb) and args.first:
-        print("WARNING: each construct was reported once; other occurrences may exist")
 
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `allowed-1.3.0/allowed/m269.json` & `allowed-1.4.0/allowed/m269.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {'delete': "['FILE_UNIT']"}*

```diff
@@ -1,9 +1,8 @@
 {
-    "FILE_UNIT": "^(\\d+)",
     "IMPORTS": {
         "11": {
             "itertools": [
                 "permutations",
                 "combinations"
             ],
             "math": [
```

### Comparing `allowed-1.3.0/allowed/tm112.json` & `allowed-1.4.0/allowed/tm112.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {'delete': "['FILE_UNIT']"}*

```diff
@@ -1,9 +1,8 @@
 {
-    "FILE_UNIT": "",
     "IMPORTS": {
         "1": {
             "turtle": [
                 "left",
                 "right",
                 "forward",
                 "penup",
```

### Comparing `allowed-1.3.0/pyproject.toml` & `allowed-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "allowed"
-version = "1.3.0" # as in allowed.py
+version = "1.4.0" # as in allowed.py
 description = "Check if a program only uses a subset of the Python language."
 authors = ["Michel Wermelinger <michel.wermelinger@open.ac.uk>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 repository = "https://github.com/dsa-ou/allowed"
 homepage = "https://dsa-ou.github.io/allowed/"
 keywords = ["education"]
```

### Comparing `allowed-1.3.0/PKG-INFO` & `allowed-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allowed
-Version: 1.3.0
+Version: 1.4.0
 Summary: Check if a program only uses a subset of the Python language.
 Home-page: https://dsa-ou.github.io/allowed/
 License: BSD-3-Clause
 Keywords: education
 Author: Michel Wermelinger
 Author-email: michel.wermelinger@open.ac.uk
 Requires-Python: >=3.10,<4.0
```

