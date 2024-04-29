# Comparing `tmp/sqlxfluff-0.2.0.tar.gz` & `tmp/sqlxfluff-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlxfluff-0.2.0.tar", max compression
+gzip compressed data, was "sqlxfluff-0.3.0.tar", max compression
```

## Comparing `sqlxfluff-0.2.0.tar` & `sqlxfluff-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1056 2023-09-27 09:38:17.092643 sqlxfluff-0.2.0/LICENSE.md
--rw-r--r--   0        0        0        0 2023-09-27 09:38:17.092643 sqlxfluff-0.2.0/README.md
--rw-r--r--   0        0        0      490 2023-09-27 09:38:17.092643 sqlxfluff-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-27 09:38:17.092643 sqlxfluff-0.2.0/sqlxfluff/__init__.py
--rw-r--r--   0        0        0       46 2023-09-27 09:38:17.092643 sqlxfluff-0.2.0/sqlxfluff/constants.py
--rw-r--r--   0        0        0        0 2023-09-27 09:38:17.092643 sqlxfluff-0.2.0/sqlxfluff/formatters/__init__.py
--rw-r--r--   0        0        0      748 2023-09-27 09:38:17.092643 sqlxfluff-0.2.0/sqlxfluff/formatters/base.py
--rw-r--r--   0        0        0     1594 2023-09-27 09:38:17.092643 sqlxfluff-0.2.0/sqlxfluff/formatters/indent.py
--rw-r--r--   0        0        0     1010 2023-09-27 09:38:17.092643 sqlxfluff-0.2.0/sqlxfluff/formatters/javascript.py
--rw-r--r--   0        0        0      873 2023-09-27 09:38:17.092643 sqlxfluff-0.2.0/sqlxfluff/formatters/sqlx.py
--rw-r--r--   0        0        0      848 2023-09-27 09:38:17.092643 sqlxfluff-0.2.0/sqlxfluff/linting.py
--rw-r--r--   0        0        0     2627 2023-09-27 09:38:17.092643 sqlxfluff-0.2.0/sqlxfluff/main.py
--rw-r--r--   0        0        0     3024 2023-09-27 09:38:17.092643 sqlxfluff-0.2.0/sqlxfluff/parsing.py
--rw-r--r--   0        0        0      375 1970-01-01 00:00:00.000000 sqlxfluff-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-04-29 05:03:20.837744 sqlxfluff-0.3.0/LICENSE.md
+-rw-r--r--   0        0        0        0 2024-04-29 05:03:20.837744 sqlxfluff-0.3.0/README.md
+-rw-r--r--   0        0        0      490 2024-04-29 05:03:20.837744 sqlxfluff-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 05:03:20.837744 sqlxfluff-0.3.0/sqlxfluff/__init__.py
+-rw-r--r--   0        0        0       46 2024-04-29 05:03:20.837744 sqlxfluff-0.3.0/sqlxfluff/constants.py
+-rw-r--r--   0        0        0        0 2024-04-29 05:03:20.837744 sqlxfluff-0.3.0/sqlxfluff/formatters/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-29 05:03:20.837744 sqlxfluff-0.3.0/sqlxfluff/formatters/base.py
+-rw-r--r--   0        0        0     1988 2024-04-29 05:03:20.837744 sqlxfluff-0.3.0/sqlxfluff/formatters/indent.py
+-rw-r--r--   0        0        0     1010 2024-04-29 05:03:20.837744 sqlxfluff-0.3.0/sqlxfluff/formatters/javascript.py
+-rw-r--r--   0        0        0      986 2024-04-29 05:03:20.837744 sqlxfluff-0.3.0/sqlxfluff/formatters/sqlx.py
+-rw-r--r--   0        0        0      848 2024-04-29 05:03:20.837744 sqlxfluff-0.3.0/sqlxfluff/linting.py
+-rw-r--r--   0        0        0     2627 2024-04-29 05:03:20.837744 sqlxfluff-0.3.0/sqlxfluff/main.py
+-rw-r--r--   0        0        0     3516 2024-04-29 05:03:20.837744 sqlxfluff-0.3.0/sqlxfluff/parsing.py
+-rw-r--r--   0        0        0      426 1970-01-01 00:00:00.000000 sqlxfluff-0.3.0/PKG-INFO
```

### Comparing `sqlxfluff-0.2.0/LICENSE.md` & `sqlxfluff-0.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sqlxfluff-0.2.0/sqlxfluff/formatters/base.py` & `sqlxfluff-0.3.0/sqlxfluff/formatters/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from .indent import indent
+from .indent import deindent, indent
 from .javascript import format_with_prettier
 
 
 def format_template(string):
     """Formats JavaScript templates from the code."""
     formatted_javascript = format_with_prettier(
         string.removeprefix("${").removesuffix("}").strip()
@@ -17,7 +17,18 @@
 def format_config(string):
     """Formats an SQLX config block."""
     MOCK_VARIABLE_NAME = "var configMockVariable = "
     mock_javascript = re.sub(r"config\s+\{", MOCK_VARIABLE_NAME + "{", string)
     return "config " + format_with_prettier(mock_javascript).removeprefix(
         MOCK_VARIABLE_NAME
     )
+
+
+def format_js(string):
+    """Formats a js block."""
+    mock_javascript = re.sub(
+        r"}\s*$", "", re.sub(r"^\s*js\s+{", "", string, count=1), count=1
+    )
+    formatted_javascript_with_indent = indent(
+        format_with_prettier(deindent(mock_javascript, 2)), 2
+    )
+    return "js {\n" + formatted_javascript_with_indent + "\n}"
```

### Comparing `sqlxfluff-0.2.0/sqlxfluff/formatters/indent.py` & `sqlxfluff-0.3.0/sqlxfluff/formatters/indent.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,26 @@
         lst = string_or_lists.split("\n")
     else:
         lst = string_or_lists
     spaces = " " * indent_level
     return "\n".join(spaces + line if line.strip() else line for line in lst)
 
 
+def deindent(string_or_lists: str | list[str], indent_level: int):
+    """Indents each line of `string` by `indent_level` spaces."""
+    if isinstance(string_or_lists, str):
+        lst = string_or_lists.split("\n")
+    else:
+        lst = string_or_lists
+    spaces = " " * indent_level
+    return "\n".join(
+        line.removeprefix(spaces) if line.strip() else line for line in lst
+    )
+
+
 def replace_with_indentation(source, target, replacement):
     """Replace `target` in `source` with `replacement`, while maintaining the
     indentation level of `target`"""
     # Find target in source
     match = re.search(re.escape(target), source)
 
     if not match:
```

### Comparing `sqlxfluff-0.2.0/sqlxfluff/formatters/javascript.py` & `sqlxfluff-0.3.0/sqlxfluff/formatters/javascript.py`

 * *Files identical despite different names*

### Comparing `sqlxfluff-0.2.0/sqlxfluff/formatters/sqlx.py` & `sqlxfluff-0.3.0/sqlxfluff/formatters/sqlx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import sqlfluff
 from sqlfluff.core import FluffConfig
 
-from .base import format_config, format_template
+from .base import format_config, format_js, format_template
 from .indent import replace_with_indentation
 
 
 def format_sqlx(deconstructed_file: dict, config: FluffConfig):
     """Formats Dataform SQLX files using SQLFluff"""
     # run fix on modified text
     bq_fix_result = sqlfluff.fix(deconstructed_file["main"], config=config).rstrip(
@@ -16,8 +16,11 @@
         formatted_template = format_template(template)
         bq_fix_result = replace_with_indentation(
             bq_fix_result, mask, formatted_template
         )
 
     # recombine the config block and the fixed SQL
     formatted_config_block = format_config(deconstructed_file["config"])
-    return formatted_config_block + "\n\n" + bq_fix_result + "\n"
+    formatted_js_block = format_js(deconstructed_file["js"])
+    return (
+        "\n\n".join([formatted_config_block, formatted_js_block, bq_fix_result]) + "\n"
+    )
```

### Comparing `sqlxfluff-0.2.0/sqlxfluff/linting.py` & `sqlxfluff-0.3.0/sqlxfluff/linting.py`

 * *Files identical despite different names*

### Comparing `sqlxfluff-0.2.0/sqlxfluff/main.py` & `sqlxfluff-0.3.0/sqlxfluff/main.py`

 * *Files identical despite different names*

### Comparing `sqlxfluff-0.2.0/sqlxfluff/parsing.py` & `sqlxfluff-0.3.0/sqlxfluff/parsing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import re
 from uuid import uuid4 as uuid
 
 
 def extract_block(file_contents, block_name):
     """Find a block (if one exists)."""
     block_open_match = re.search(block_name + r"\s+\{", file_contents)
+    if block_name == "js":
+        print(f"{block_open_match = }")
     if block_open_match is None:
         return ""
     block_open_start, block_open_end = block_open_match.span()
     num_open_brackets = 1
     num_chars_in_block = block_open_end - block_open_start
     for char in file_contents[block_open_end:]:
         if char == "{":
@@ -29,15 +31,15 @@
     INSIDE_EXPR = 2
 
     state = OUTSIDE
     brace_count = 0
     expressions = []
     curr_expr = ""
 
-    for i, char in enumerate(text):
+    for char in text:
         if state == OUTSIDE:
             if char == "$":
                 state = INSIDE_DOLLAR
                 curr_expr += char
             continue
 
         if state == INSIDE_DOLLAR:
@@ -69,31 +71,38 @@
 
 
 def parse_sqlx(file_contents: str):
     """Parses an SQLX file and splits into multiple components."""
     # split the text into a config block section and remaining text
     config_block_string = extract_block(file_contents, "config")
     js_block_string = extract_block(file_contents, "js")
-    remaining_text = (
-        file_contents.replace(config_block_string, "")
-        .replace(js_block_string, "")
-        .strip()
-        + "\n"
-    )
+    pre_operations_block_string = extract_block(file_contents, "pre_operations")
+    post_operations_block_string = extract_block(file_contents, "post_operations")
+    blocks_to_replace = [
+        config_block_string,
+        js_block_string,
+        pre_operations_block_string,
+        post_operations_block_string,
+    ]
+    remaining_text = file_contents
+    for block in blocks_to_replace:
+        remaining_text = remaining_text.replace(block, "").strip() + "\n"
 
     # Identify each template and replace it with a temporary mask
     templates = extract_templates(remaining_text)
 
     masks = {}
     for match in templates:
-        # hacky way to generate a unique string that meets the BQ rules
+        # hacky way to generate a unique string that fits BigQuery's parsing rules
         # https://github.com/sqlfluff/sqlfluff/issues/1540#issuecomment-1110835283
         mask_string = "a" + str(uuid()).replace("-", ".a")
         remaining_text = remaining_text.replace(match, mask_string)
         masks[mask_string] = match
 
     return {
         "config": config_block_string,
         "js": js_block_string,
+        "pre_operations": pre_operations_block_string,
+        "post_operations": post_operations_block_string,
         "main": remaining_text,
         "templates": masks,
     }
```

