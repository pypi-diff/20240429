# Comparing `tmp/llm_parse-0.1.2.tar.gz` & `tmp/llm_parse-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm_parse-0.1.2.tar", max compression
+gzip compressed data, was "llm_parse-0.1.3.tar", max compression
```

## Comparing `llm_parse-0.1.2.tar` & `llm_parse-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-19 15:47:45.995075 llm_parse-0.1.2/LICENSE
--rw-r--r--   0        0        0     1382 2024-04-22 15:12:40.636191 llm_parse-0.1.2/README.md
--rw-r--r--   0        0        0      244 2024-04-22 15:00:37.104345 llm_parse-0.1.2/llm_parse/__init__.py
--rw-r--r--   0        0        0      354 2024-04-22 14:53:02.976941 llm_parse-0.1.2/llm_parse/base.py
--rw-r--r--   0        0        0     1127 2024-04-23 02:26:47.191955 llm_parse-0.1.2/llm_parse/llamaparse_parser.py
--rw-r--r--   0        0        0    12567 2024-04-23 02:01:16.137883 llm_parse-0.1.2/llm_parse/pdf_2_md_parser.py
--rw-r--r--   0        0        0     1585 2024-04-21 02:28:18.395369 llm_parse-0.1.2/llm_parse/pdf_2_text_parser.py
--rw-r--r--   0        0        0     4252 2024-04-22 10:42:53.827780 llm_parse-0.1.2/llm_parse/utils.py
--rw-r--r--   0        0        0      471 2024-04-23 02:28:04.535938 llm_parse-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 llm_parse-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-19 15:47:45.995075 llm_parse-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1382 2024-04-23 11:12:09.477070 llm_parse-0.1.3/README.md
+-rw-r--r--   0        0        0      244 2024-04-23 11:12:09.480271 llm_parse-0.1.3/llm_parse/__init__.py
+-rw-r--r--   0        0        0      354 2024-04-23 11:12:09.484315 llm_parse-0.1.3/llm_parse/base.py
+-rw-r--r--   0        0        0     1127 2024-04-23 11:12:09.489996 llm_parse-0.1.3/llm_parse/llamaparse_parser.py
+-rw-r--r--   0        0        0    12567 2024-04-23 11:12:09.494616 llm_parse-0.1.3/llm_parse/pdf_2_md_parser.py
+-rw-r--r--   0        0        0     1585 2024-04-24 14:45:41.206971 llm_parse-0.1.3/llm_parse/pdf_2_text_parser.py
+-rw-r--r--   0        0        0     4342 2024-04-29 13:11:02.034017 llm_parse-0.1.3/llm_parse/utils.py
+-rw-r--r--   0        0        0      493 2024-04-29 13:15:20.163699 llm_parse-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2030 1970-01-01 00:00:00.000000 llm_parse-0.1.3/PKG-INFO
```

### Comparing `llm_parse-0.1.2/LICENSE` & `llm_parse-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm_parse-0.1.2/README.md` & `llm_parse-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `llm_parse-0.1.2/llm_parse/llamaparse_parser.py` & `llm_parse-0.1.3/llm_parse/llamaparse_parser.py`

 * *Files identical despite different names*

### Comparing `llm_parse-0.1.2/llm_parse/pdf_2_md_parser.py` & `llm_parse-0.1.3/llm_parse/pdf_2_md_parser.py`

 * *Files identical despite different names*

### Comparing `llm_parse-0.1.2/llm_parse/pdf_2_text_parser.py` & `llm_parse-0.1.3/llm_parse/pdf_2_text_parser.py`

 * *Files identical despite different names*

### Comparing `llm_parse-0.1.2/llm_parse/utils.py` & `llm_parse-0.1.3/llm_parse/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,34 +70,35 @@
 
 def merge_bold(text: str) -> str:
     r"""
     If there are multiple groups of text in Markdown bold (enclosed by **), on a single line of text,
     the whole line can be grouped as a single group of bold text.
 
     Regex explanation
-    - ^(\*{2}[^*]*\*{2}[ \r\t\f]*)+:
+    - ^([ \r\t\f]*\*{2}[^*]*\*{2}[ \r\t\f]*)+:
         - ^: Starts with this group.
-        - \*{2}[^*]*\*{2}: Matches text enclosed within **.
         - [ \r\t\f]*: Matches zero or more whitespace characters except \n.
+        - \*{2}[^*]*\*{2}: Matches text enclosed within **.
         - +: Matches one or more of this group.
-    - \*{2}[^*]*\*{2}$: Ends with text enclosed within **.
+    - (\*{2}[^*]*\*{2}[ \r\t\f]*)$: Ends with text enclosed within **.
 
     Args:
         text: Text string to process.
 
     Returns:
         str: Processed text.
     """
 
     def remove_stars(match):
         matched_group = match.group(0)
+        matched_group = matched_group.strip()
         replaced_group = matched_group.replace("*", "")
         return f"**{replaced_group}**"
 
-    pattern = r"^(\*{2}[^*]*\*{2}[ \r\t\f]*)+\*{2}[^*]*\*{2}$"
+    pattern = r"^([ \r\t\f]*\*{2}[^*]*\*{2}[ \r\t\f]*)+(\*{2}[^*]*\*{2}[ \r\t\f]*)$"
     pattern = re.compile(pattern, re.MULTILINE)
     text = re.sub(pattern, remove_stars, text)
 
     return text
 
 
 def merge_spaces(text: str) -> str:
```

### Comparing `llm_parse-0.1.2/PKG-INFO` & `llm_parse-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm-parse
-Version: 0.1.2
+Version: 0.1.3
 Summary: Parse data from documents optimised for downstream llm tasks.
 License: MIT
 Author: tanchangsheng
 Author-email: tancs1994@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

