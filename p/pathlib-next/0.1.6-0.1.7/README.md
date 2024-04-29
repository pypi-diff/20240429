# Comparing `tmp/pathlib_next-0.1.6.tar.gz` & `tmp/pathlib_next-0.1.7.tar.gz`

## Comparing `pathlib_next-0.1.6.tar` & `pathlib_next-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/example.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/__init__.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/fspath.py
--rw-r--r--   0        0        0     5241 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/mempath.py
--rw-r--r--   0        0        0    17831 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/path.py
--rw-r--r--   0        0        0    15459 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/uri/__init__.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/uri/query.py
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/uri/source.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/uri/schemes/__init__.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/uri/schemes/file.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/uri/schemes/http.py
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/uri/schemes/sftp.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/utils/__init__.py
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/utils/glob.py
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/utils/stat.py
--rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/src/pathlib_next/utils/sync.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/tests/test_local.py
--rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/tests/test_uri.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/LICENSE
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pathlib_next-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/example.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/pathlib_next/__init__.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/pathlib_next/fspath.py
+-rw-r--r--   0        0        0     5174 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/pathlib_next/mempath.py
+-rw-r--r--   0        0        0    18058 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/pathlib_next/path.py
+-rw-r--r--   0        0        0    15459 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/pathlib_next/uri/__init__.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/pathlib_next/uri/query.py
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/pathlib_next/uri/source.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/pathlib_next/uri/schemes/__init__.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/pathlib_next/uri/schemes/file.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/pathlib_next/uri/schemes/http.py
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/pathlib_next/uri/schemes/sftp.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/pathlib_next/utils/__init__.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/pathlib_next/utils/glob.py
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/pathlib_next/utils/stat.py
+-rw-r--r--   0        0        0     2880 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/src/pathlib_next/utils/sync.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/tests/test_local.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/tests/test_uri.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/LICENSE
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 pathlib_next-0.1.7/PKG-INFO
```

### Comparing `pathlib_next-0.1.6/src/example.py` & `pathlib_next-0.1.7/src/example.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.6/src/pathlib_next/fspath.py` & `pathlib_next-0.1.7/src/pathlib_next/fspath.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.6/src/pathlib_next/mempath.py` & `pathlib_next-0.1.7/src/pathlib_next/mempath.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,17 +88,14 @@
 
     def with_segments(self, *segments: str):
         return type(self)(*segments, backend=self.backend)
 
     def as_uri(self):
         return f"mempath:{_urlquote(self.as_posix())}"
 
-    def as_posix(self):
-        return "/".join(self.segments)
-
     def _parent_container(self) -> tuple[dict[str, bytearray], str]:
         parent = self.backend
         *ancestors, name = self.normalized
         for path in ancestors:
             if path not in parent:
                 raise FileNotFoundError(self.parent)
             else:
```

### Comparing `pathlib_next-0.1.6/src/pathlib_next/path.py` & `pathlib_next-0.1.7/src/pathlib_next/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Object-oriented filesystem paths.
 
 This module provides classes to represent abstract paths and concrete
 paths with operations that have semantics appropriate for different
 operating systems.
 """
 
+import abc as _abc
+import io as _io
 import os as _os
 import re as _re
+import shutil as _shutil
 import stat as _stat
-from pathlib import _ignore_error
 import typing as _ty
-import abc as _abc
-import io as _io
-import shutil as _shutil
+from pathlib import _ignore_error
 
 from . import utils as _utils
 from .utils import glob as _glob
 from .utils.stat import FileStatLike
 
 P = _ty.TypeVar("P", bound="Path")
 PN = _ty.TypeVar("PN", bound="Pathname")
@@ -32,14 +32,15 @@
 
 
 _os.PathLike.register(FsPathLike)
 
 
 _FsPathLike = str | FsPathLike
 
+
 class _PathnameParents(_ty.Sequence[PN]):
     """This object provides sequence-like access to the logical ancestors
     of a path.  Don't try to construct it yourself."""
 
     __slots__ = ("_path", "_segments")
 
     def __init__(self, path: PN):
@@ -65,14 +66,15 @@
         if idx < 0:
             idx += len(self)
         return self._path.with_segments(*self._segments[: -idx - 1])
 
     def __repr__(self):
         return "<{}.parents>".format(type(self._path).__name__)
 
+
 class Pathname(FsPathLike, _ty.Generic[_P]):
     """Base class for manipulating paths without I/O."""
 
     __slots__ = ()
 
     @property
     def _is_case_sensitive(self) -> bool:
@@ -180,18 +182,17 @@
 
     @property
     @_abc.abstractmethod
     def parent(self) -> _ty.Self:
         """The logical parent of the path."""
 
     @property
-    def parents(self)->_ty.Sequence[_ty.Self]:
+    def parents(self) -> _ty.Sequence[_ty.Self]:
         return _PathnameParents(self)
 
-
     @_utils.notimplemented
     def is_absolute(self) -> bool:
         """True if the path is absolute (has both a root and, if applicable,
         a drive)."""
         ...
 
     def match(self, path_pattern: str | _re.Pattern, *, case_sensitive=None):
@@ -204,15 +205,22 @@
         if not isinstance(path_pattern, _re.Pattern):
             if isinstance(str, path_pattern):
                 path_pattern = type(self)(path_pattern).__path__()
             path_pattern = _glob.compile_pattern(path_pattern, case_sensitive)
         return path_pattern.match(path) is not None
 
     @_utils.notimplemented
-    def as_posix(self) -> str: ...
+    def as_posix(self) -> str:
+        return "/".join(self.segments)
+
+    def has_glob_pattern(self):
+        for segment in self.segments:
+            if _glob.WILCARD_PATTERN.match(segment) != None:
+                return True
+        return False
 
 
 PurePathLike = str | Pathname
 
 
 class Path(Pathname):
     """Base class for manipulating paths with I/O."""
```

### Comparing `pathlib_next-0.1.6/src/pathlib_next/uri/__init__.py` & `pathlib_next-0.1.7/src/pathlib_next/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.6/src/pathlib_next/uri/query.py` & `pathlib_next-0.1.7/src/pathlib_next/uri/query.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.6/src/pathlib_next/uri/source.py` & `pathlib_next-0.1.7/src/pathlib_next/uri/source.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.6/src/pathlib_next/uri/schemes/file.py` & `pathlib_next-0.1.7/src/pathlib_next/uri/schemes/file.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.6/src/pathlib_next/uri/schemes/http.py` & `pathlib_next-0.1.7/src/pathlib_next/uri/schemes/http.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.6/src/pathlib_next/uri/schemes/sftp.py` & `pathlib_next-0.1.7/src/pathlib_next/uri/schemes/sftp.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.6/src/pathlib_next/utils/__init__.py` & `pathlib_next-0.1.7/src/pathlib_next/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.6/src/pathlib_next/utils/glob.py` & `pathlib_next-0.1.7/src/pathlib_next/utils/glob.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # Based on glob built-in on python modified to work with Uri/anything that implemetns fspath/iterdir that is similar to pathlib.Path
 
 
 """Filename globbing utility."""
 
 import fnmatch as _fnmatch
-import typing as _ty
 import functools as _func
 import re as _re
-
+import typing as _ty
 
 RECURSIVE = "**"
 ANY_PATTERN = _re.compile(_fnmatch.translate("*"))
 WILCARD_PATTERN = _re.compile("([*?[])")
 
 if _ty.TYPE_CHECKING:
     from ..path import P as _Globable
@@ -29,15 +28,15 @@
 def glob(
     path: _Globable,
     *,
     dironly: bool = False,
     root_dir: _Globable | None = None,
     recursive: bool = False,
     include_hidden: bool = False,
-    case_sensitive: bool | None = None
+    case_sensitive: bool | None = None,
 ) -> _ty.Iterable[_Globable]:
     """Return an iterator which yields the paths matching a pathname pattern.
 
     The pattern may contain simple shell-style wildcards a la
     fnmatch. However, unlike fnmatch, filenames starting with a
     dot are special cases that are not matched by '*' and '?'
     patterns.
@@ -48,20 +47,16 @@
     if case_sensitive is None:
         case_sensitive = path._is_case_sensitive
 
     include_hidden = include_hidden or path.is_hidden()
     pattern = compile_pattern(path.name, case_sensitive) if path.name else ANY_PATTERN
 
     name_is_pattern = WILCARD_PATTERN.match(path.name) != None
-    wildcard_in_path = name_is_pattern
+    wildcard_in_path = name_is_pattern or path.has_glob_pattern()
     parent = next(iter(path.parents), None)
-    for segment in path.segments:
-        if WILCARD_PATTERN.match(segment) != None:
-            wildcard_in_path = True
-            break
 
     root: _Globable = (
         (root_dir or parent) if not root_dir or not parent else (root_dir / parent)
     )
 
     if recursive and path.name == RECURSIVE:
         globber = _glob_recursive
```

### Comparing `pathlib_next-0.1.6/src/pathlib_next/utils/stat.py` & `pathlib_next-0.1.7/src/pathlib_next/utils/stat.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.6/src/pathlib_next/utils/sync.py` & `pathlib_next-0.1.7/src/pathlib_next/utils/sync.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.6/tests/test_local.py` & `pathlib_next-0.1.7/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.6/tests/test_uri.py` & `pathlib_next-0.1.7/tests/test_uri.py`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.6/LICENSE` & `pathlib_next-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pathlib_next-0.1.6/pyproject.toml` & `pathlib_next-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pathlib_next"
-version = "0.1.6"
+version = "0.1.7"
 authors = [{ name = "Jose A" }]
 description = "Generic Path Protocol based pathlib"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pathlib_next-0.1.6/PKG-INFO` & `pathlib_next-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pathlib_next
-Version: 0.1.6
+Version: 0.1.7
 Summary: Generic Path Protocol based pathlib
 Project-URL: Homepage, https://github.com/jose-pr/pathlib_next/
 Project-URL: Issues, https://github.com/jose-pr/pathlib_next/issues
 Author: Jose A
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

