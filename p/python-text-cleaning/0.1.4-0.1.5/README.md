# Comparing `tmp/python_text_cleaning-0.1.4.tar.gz` & `tmp/python_text_cleaning-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_text_cleaning-0.1.4.tar", max compression
+gzip compressed data, was "python_text_cleaning-0.1.5.tar", max compression
```

## Comparing `python_text_cleaning-0.1.4.tar` & `python_text_cleaning-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2024-03-26 06:15:20.571853 python_text_cleaning-0.1.4/LICENSE
--rw-r--r--   0        0        0      759 2024-03-26 06:15:20.571853 python_text_cleaning-0.1.4/README.md
--rw-r--r--   0        0        0      765 2024-03-26 06:15:32.719786 python_text_cleaning-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       73 2024-03-26 06:15:20.571853 python_text_cleaning-0.1.4/python_text_cleaning/__init__.py
--rw-r--r--   0        0        0     3808 2024-03-26 06:15:20.571853 python_text_cleaning-0.1.4/python_text_cleaning/asr_text_cleaning.py
--rw-r--r--   0        0        0      281 2024-03-26 06:15:20.575853 python_text_cleaning-0.1.4/python_text_cleaning/character_mappings/__init__.py
--rw-r--r--   0        0        0      872 2024-03-26 06:15:20.575853 python_text_cleaning-0.1.4/python_text_cleaning/character_mappings/cyrillic_character_maps.py
--rw-r--r--   0        0        0      954 2024-03-26 06:15:20.575853 python_text_cleaning-0.1.4/python_text_cleaning/character_mappings/german_text_cleaners.py
--rw-r--r--   0        0        0     2111 2024-03-26 06:15:20.575853 python_text_cleaning-0.1.4/python_text_cleaning/character_mappings/latin_character_maps.py
--rw-r--r--   0        0        0     2182 2024-03-26 06:15:20.575853 python_text_cleaning-0.1.4/python_text_cleaning/character_mappings/misc_language_text_cleaners.py
--rw-r--r--   0        0        0      219 2024-03-26 06:15:20.575853 python_text_cleaning-0.1.4/python_text_cleaning/character_mappings/not_str_translatable_maps.py
--rw-r--r--   0        0        0     3305 2024-03-26 06:15:20.575853 python_text_cleaning-0.1.4/python_text_cleaning/character_mappings/text_cleaning.py
--rw-r--r--   0        0        0     1346 2024-03-26 06:15:20.575853 python_text_cleaning-0.1.4/python_text_cleaning/character_mappings/todo.md
--rw-r--r--   0        0        0     1352 1970-01-01 00:00:00.000000 python_text_cleaning-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/LICENSE
+-rw-r--r--   0        0        0      759 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/README.md
+-rw-r--r--   0        0        0      765 2024-04-29 14:38:56.519110 python_text_cleaning-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       73 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/__init__.py
+-rw-r--r--   0        0        0     3889 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/asr_text_cleaning.py
+-rw-r--r--   0        0        0      281 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/__init__.py
+-rw-r--r--   0        0        0      872 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/cyrillic_character_maps.py
+-rw-r--r--   0        0        0      954 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/german_text_cleaners.py
+-rw-r--r--   0        0        0     2111 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/latin_character_maps.py
+-rw-r--r--   0        0        0     2182 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/misc_language_text_cleaners.py
+-rw-r--r--   0        0        0      219 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/not_str_translatable_maps.py
+-rw-r--r--   0        0        0     3305 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/text_cleaning.py
+-rw-r--r--   0        0        0     1346 2024-04-29 14:38:40.766933 python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/todo.md
+-rw-r--r--   0        0        0     1352 1970-01-01 00:00:00.000000 python_text_cleaning-0.1.5/PKG-INFO
```

### Comparing `python_text_cleaning-0.1.4/LICENSE` & `python_text_cleaning-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.4/README.md` & `python_text_cleaning-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.4/pyproject.toml` & `python_text_cleaning-0.1.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-text-cleaning"
-version = "0.1.4"
+version = "0.1.5"
 description = "mostly mapping characters"
 authors = ["Tilo Himmelsbach <dertilo@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/dertilo/python-text-cleaning"
 
 packages = [{ include = "python_text_cleaning" }]
```

### Comparing `python_text_cleaning-0.1.4/python_text_cleaning/asr_text_cleaning.py` & `python_text_cleaning-0.1.5/python_text_cleaning/asr_text_cleaning.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import re
 from collections.abc import Callable
 from dataclasses import dataclass
 from enum import Enum, auto
-
-from typing_extensions import Self
+from typing import TypeVar
 
 from python_text_cleaning.character_mappings.text_cleaning import (
     TEXT_CLEANERS,
     NeStr,
     TextCleaner,
 )
 
+TCasing = TypeVar("TCasing", bound="Casing")  # is this really the recommended way?
+
 
 class Casing(str, Enum):
     lower = auto()
     upper = auto()
     original = auto()
 
     def _to_dict(self, skip_keys: list[str] | None = None) -> dict:
@@ -31,29 +32,29 @@
             fun = CASING_FUNS[self](text)
         else:  # noqa: RET505
             msg = "unknown Casing"
             raise AssertionError(msg)
         return fun
 
     @staticmethod
-    def create(value: str | int) -> Self:
+    def create(value: str | int) -> TCasing:
         """
         # TODO: this is only necessary if someone else mis-interprets "1" as an integer! pythons json lib does it correctly -> somewhere in jina??
         """
         return Casing(str(value))
 
 
 CASING_FUNS: dict[Casing, Callable] = {
     Casing.upper: lambda s: s.upper(),
     Casing.lower: lambda s: s.lower(),
     Casing.original: lambda s: s,
 }
 
 
-Letters = str
+Letters = NeStr
 
 
 def upper_lower_text(text: str, casing: Casing = Casing.original) -> str:
     # first upper than check if in vocab actually makes sense for ß, cause "ß".upper()==SS
     return casing.apply(text)
```

### Comparing `python_text_cleaning-0.1.4/python_text_cleaning/character_mappings/cyrillic_character_maps.py` & `python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/cyrillic_character_maps.py`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.4/python_text_cleaning/character_mappings/german_text_cleaners.py` & `python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/german_text_cleaners.py`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.4/python_text_cleaning/character_mappings/latin_character_maps.py` & `python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/latin_character_maps.py`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.4/python_text_cleaning/character_mappings/misc_language_text_cleaners.py` & `python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/misc_language_text_cleaners.py`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.4/python_text_cleaning/character_mappings/text_cleaning.py` & `python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/text_cleaning.py`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.4/python_text_cleaning/character_mappings/todo.md` & `python_text_cleaning-0.1.5/python_text_cleaning/character_mappings/todo.md`

 * *Files identical despite different names*

### Comparing `python_text_cleaning-0.1.4/PKG-INFO` & `python_text_cleaning-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-text-cleaning
-Version: 0.1.4
+Version: 0.1.5
 Summary: mostly mapping characters
 Home-page: https://github.com/dertilo/python-text-cleaning
 Author: Tilo Himmelsbach
 Author-email: dertilo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

