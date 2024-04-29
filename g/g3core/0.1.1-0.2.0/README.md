# Comparing `tmp/g3core-0.1.1.tar.gz` & `tmp/g3core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g3core-0.1.1.tar", last modified: Tue Feb  6 17:05:34 2024, max compression
+gzip compressed data, was "g3core-0.2.0.tar", last modified: Mon Apr 29 12:49:55 2024, max compression
```

## Comparing `g3core-0.1.1.tar` & `g3core-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-02-06 17:05:34.792319 g3core-0.1.1/
--rw-rw-rw-   0        0        0     1091 2023-06-02 14:34:32.000000 g3core-0.1.1/LICENCE
--rw-rw-rw-   0        0        0      886 2024-02-06 17:05:34.792319 g3core-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      364 2024-02-06 13:12:10.000000 g3core-0.1.1/README.md
--rw-rw-rw-   0        0        0      697 2024-02-06 17:04:00.000000 g3core-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-06 17:05:34.807947 g3core-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-06 17:05:34.649706 g3core-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2024-02-06 17:05:34.672547 g3core-0.1.1/src/g3core/
--rw-rw-rw-   0        0        0      320 2024-01-17 14:23:51.000000 g3core-0.1.1/src/g3core/__init__.py
--rw-rw-rw-   0        0        0     3767 2024-01-17 14:23:39.000000 g3core-0.1.1/src/g3core/_g3core.py
-drwxrwxrwx   0        0        0        0 2024-02-06 17:05:34.715071 g3core-0.1.1/src/g3core/file/
--rw-rw-rw-   0        0        0      113 2023-08-23 14:12:21.000000 g3core-0.1.1/src/g3core/file/__init__.py
--rw-rw-rw-   0        0        0     1424 2023-10-23 17:12:28.000000 g3core-0.1.1/src/g3core/file/_base_file.py
--rw-rw-rw-   0        0        0      906 2023-10-24 12:33:54.000000 g3core-0.1.1/src/g3core/file/_fun_file.py
--rw-rw-rw-   0        0        0      771 2023-10-23 17:07:10.000000 g3core-0.1.1/src/g3core/file/_typ_file.py
-drwxrwxrwx   0        0        0        0 2024-02-06 17:05:34.744068 g3core-0.1.1/src/g3core/file_system/
--rw-rw-rw-   0        0        0      266 2023-08-23 14:21:26.000000 g3core-0.1.1/src/g3core/file_system/__init__.py
--rw-rw-rw-   0        0        0      951 2023-09-18 17:51:25.000000 g3core-0.1.1/src/g3core/file_system/_base_file_system.py
--rw-rw-rw-   0        0        0     2085 2024-01-30 20:18:04.000000 g3core-0.1.1/src/g3core/file_system/_gitlab_file_system.py
--rw-rw-rw-   0        0        0     1098 2023-09-18 17:52:32.000000 g3core-0.1.1/src/g3core/file_system/_local_file_system.py
--rw-rw-rw-   0        0        0        0 2023-08-14 16:24:28.000000 g3core-0.1.1/src/g3core/py.typed
-drwxrwxrwx   0        0        0        0 2024-02-06 17:05:34.792319 g3core-0.1.1/src/g3core/st_parser/
--rw-rw-rw-   0        0        0      267 2023-08-22 14:16:14.000000 g3core-0.1.1/src/g3core/st_parser/__init__.py
--rw-rw-rw-   0        0        0     1954 2023-09-24 13:12:32.000000 g3core-0.1.1/src/g3core/st_parser/_st_base_structure.py
--rw-rw-rw-   0        0        0     1629 2023-09-24 13:12:17.000000 g3core-0.1.1/src/g3core/st_parser/_st_enum.py
--rw-rw-rw-   0        0        0     1821 2023-09-18 16:57:57.000000 g3core-0.1.1/src/g3core/st_parser/_st_func.py
--rw-rw-rw-   0        0        0      685 2023-10-23 17:00:26.000000 g3core-0.1.1/src/g3core/st_parser/_st_struct.py
--rw-rw-rw-   0        0        0     3631 2023-12-05 12:10:01.000000 g3core-0.1.1/src/g3core/st_parser/_st_var.py
-drwxrwxrwx   0        0        0        0 2024-02-06 17:05:34.792319 g3core-0.1.1/src/g3core.egg-info/
--rw-rw-rw-   0        0        0      886 2024-02-06 17:05:34.000000 g3core-0.1.1/src/g3core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      761 2024-02-06 17:05:34.000000 g3core-0.1.1/src/g3core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-06 17:05:34.000000 g3core-0.1.1/src/g3core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-02-06 17:05:34.000000 g3core-0.1.1/src/g3core.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-02-06 17:05:34.000000 g3core-0.1.1/src/g3core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-29 12:49:55.383352 g3core-0.2.0/
+-rw-rw-rw-   0        0        0     1091 2023-06-02 14:34:32.000000 g3core-0.2.0/LICENCE
+-rw-rw-rw-   0        0        0     1087 2024-04-29 12:49:55.377350 g3core-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       68 2024-04-22 19:15:49.000000 g3core-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1133 2024-04-23 10:20:13.000000 g3core-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-29 12:49:55.384378 g3core-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-29 12:49:54.711340 g3core-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-29 12:49:54.788359 g3core-0.2.0/src/g3core/
+-rw-rw-rw-   0        0        0      320 2024-01-17 14:23:51.000000 g3core-0.2.0/src/g3core/__init__.py
+-rw-rw-rw-   0        0        0     7527 2024-04-22 19:15:49.000000 g3core-0.2.0/src/g3core/_g3core.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:49:55.289355 g3core-0.2.0/src/g3core/file/
+-rw-rw-rw-   0        0        0      100 2024-04-22 19:15:49.000000 g3core-0.2.0/src/g3core/file/__init__.py
+-rw-rw-rw-   0        0        0     2336 2024-04-22 19:15:49.000000 g3core-0.2.0/src/g3core/file/_base_file.py
+-rw-rw-rw-   0        0        0     1508 2024-04-22 19:15:49.000000 g3core-0.2.0/src/g3core/file/_fun_file.py
+-rw-rw-rw-   0        0        0     1358 2024-04-25 13:54:38.000000 g3core-0.2.0/src/g3core/file/_typ_file.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:49:55.305375 g3core-0.2.0/src/g3core/file_system/
+-rw-rw-rw-   0        0        0       78 2024-04-22 19:15:49.000000 g3core-0.2.0/src/g3core/file_system/__init__.py
+-rw-rw-rw-   0        0        0     5351 2024-04-22 19:15:49.000000 g3core-0.2.0/src/g3core/file_system/_file_system.py
+-rw-rw-rw-   0        0        0        0 2023-08-14 16:24:28.000000 g3core-0.2.0/src/g3core/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-29 12:49:55.367371 g3core-0.2.0/src/g3core/st_parser/
+-rw-rw-rw-   0        0        0      288 2024-04-22 19:15:49.000000 g3core-0.2.0/src/g3core/st_parser/__init__.py
+-rw-rw-rw-   0        0        0     3674 2024-04-22 19:15:49.000000 g3core-0.2.0/src/g3core/st_parser/_st_base_structure.py
+-rw-rw-rw-   0        0        0     2321 2024-04-22 19:15:49.000000 g3core-0.2.0/src/g3core/st_parser/_st_enum.py
+-rw-rw-rw-   0        0        0     2495 2024-04-22 19:15:49.000000 g3core-0.2.0/src/g3core/st_parser/_st_func.py
+-rw-rw-rw-   0        0        0      897 2024-04-22 19:15:49.000000 g3core-0.2.0/src/g3core/st_parser/_st_struct.py
+-rw-rw-rw-   0        0        0     7370 2024-04-23 13:33:26.000000 g3core-0.2.0/src/g3core/st_parser/_st_var.py
+drwxrwxrwx   0        0        0        0 2024-04-29 12:49:55.375352 g3core-0.2.0/src/g3core.egg-info/
+-rw-rw-rw-   0        0        0     1087 2024-04-29 12:49:54.000000 g3core-0.2.0/src/g3core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2024-04-29 12:49:54.000000 g3core-0.2.0/src/g3core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-29 12:49:54.000000 g3core-0.2.0/src/g3core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-04-29 12:49:54.000000 g3core-0.2.0/src/g3core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-29 12:49:54.000000 g3core-0.2.0/src/g3core.egg-info/top_level.txt
```

### Comparing `g3core-0.1.1/LICENCE` & `g3core-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `g3core-0.1.1/src/g3core/file/_base_file.py` & `g3core-0.2.0/src/g3core/file/_typ_file.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,45 @@
-import re
-import typing
-import functools
-
 from dataclasses import dataclass
 
-if typing.TYPE_CHECKING:
-    from gitlab.v4.objects import Project
+from ._base_file import BaseFile
+from ..st_parser import STStruct, STIntEnum
+
+
+@dataclass(frozen=True)
+class TypFile(BaseFile):
+    """A wrapper around a `.typ` SystemG3Core file.
+
+    Attributes:
+        contents (str): The contents of the file.
+    """
+
+    def get_struct(self, struct_name: str) -> STStruct:
+        """Get a struct wrapper from the file.
+
+        Args:
+            struct_name (str): The name of the struct to get.
+
+        Returns:
+            STStruct: The struct wrapper object.
+        """
+        fb_contents = self._get_structure(
+            structure_name=struct_name,
+            structure_type='Struct',
+            search_pattern=f'(^\\s*{struct_name}\\s*:\\s*STRUCT.*?END_STRUCT)',
+            )
+        return STStruct(fb_contents)
+
+    def get_int_enum(self, enum_name: str) -> STIntEnum:
+        """Get an integer enum wrapper from the file.
 
+        Args:
+            enum_name (str): The name of the integer enum to get.
 
-@functools.cache
-def extract_from_file_contents(
-    file_contents: str,
-    structure_name: str,
-    structure_type: str,
-    search_pattern: str
-) -> str:
-    contents = re.search(
-        search_pattern, file_contents, flags=re.DOTALL | re.MULTILINE
-        )
-    if contents:
-        return contents.group(1)
-    raise ValueError(
-        f'{structure_type} "{structure_name}" was not found in the file.'
-        )
-
-
-@dataclass
-class BaseFile:
-    contents: str
-
-    @classmethod
-    def from_local_path(cls, path: str) -> typing.Self:
-        with open(path, 'r', encoding='utf-8') as file:
-            return cls(file.read())
-
-    @classmethod
-    def from_gitlab(
-        cls,
-        g3core: 'Project',
-        file_path: str,
-        branch: str = 'master',
-    ) -> typing.Self:
-        file = g3core.files.raw(file_path, ref=branch)
-        assert isinstance(file, bytes), "Unexpected file contents format"
-        return cls(file.decode())
-
-    def _get_structure(
-        self,
-        structure_name: str,
-        structure_type: str,
-        search_pattern: str
-    ) -> str:
-        return extract_from_file_contents(
-            self.contents, structure_name, structure_type, search_pattern
+        Returns:
+            STIntEnum: The integer enum wrapper object.
+        """
+        e_contents = self._get_structure(
+            structure_name=enum_name,
+            structure_type='Enum',
+            search_pattern=f"^\\s*{enum_name}\\s*:\\s*\\(.*?\\);",
             )
+        return STIntEnum(e_contents)
```

### Comparing `g3core-0.1.1/src/g3core.egg-info/SOURCES.txt` & `g3core-0.2.0/src/g3core.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,14 @@
 src/g3core.egg-info/requires.txt
 src/g3core.egg-info/top_level.txt
 src/g3core/file/__init__.py
 src/g3core/file/_base_file.py
 src/g3core/file/_fun_file.py
 src/g3core/file/_typ_file.py
 src/g3core/file_system/__init__.py
-src/g3core/file_system/_base_file_system.py
-src/g3core/file_system/_gitlab_file_system.py
-src/g3core/file_system/_local_file_system.py
+src/g3core/file_system/_file_system.py
 src/g3core/st_parser/__init__.py
 src/g3core/st_parser/_st_base_structure.py
 src/g3core/st_parser/_st_enum.py
 src/g3core/st_parser/_st_func.py
 src/g3core/st_parser/_st_struct.py
 src/g3core/st_parser/_st_var.py
```

