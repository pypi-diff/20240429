# Comparing `tmp/fmtutil-1.0.2.tar.gz` & `tmp/fmtutil-1.0.3.tar.gz`

## Comparing `fmtutil-1.0.2.tar` & `fmtutil-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/__about__.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/__main__.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/__type.py
--rw-r--r--   0        0        0    36758 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/__version.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/cli.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/exceptions.py
--rw-r--r--   0        0        0   133452 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/formatter.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/utils.py
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 fmtutil-1.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fmtutil-1.0.2/LICENSE
--rw-r--r--   0        0        0     7978 2020-02-02 00:00:00.000000 fmtutil-1.0.2/README.md
--rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 fmtutil-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 fmtutil-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/__about__.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/__main__.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/__type.py
+-rw-r--r--   0        0        0    36848 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/__version.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/cli.py
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/exceptions.py
+-rw-r--r--   0        0        0   133534 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/formatter.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 fmtutil-1.0.3/fmtutil/utils.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 fmtutil-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fmtutil-1.0.3/LICENSE
+-rw-r--r--   0        0        0     7978 2020-02-02 00:00:00.000000 fmtutil-1.0.3/README.md
+-rw-r--r--   0        0        0     3407 2020-02-02 00:00:00.000000 fmtutil-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 fmtutil-1.0.3/PKG-INFO
```

### Comparing `fmtutil-1.0.2/fmtutil/__init__.py` & `fmtutil-1.0.3/fmtutil/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 )
 from .exceptions import (
     FormatterArgumentError,
     FormatterError,
     FormatterGroupArgumentError,
     FormatterGroupValueError,
     FormatterKeyError,
-    FormatterNotFoundError,
-    FormatterTypeError,
     FormatterValueError,
 )
 from .formatter import (
     Constant,
     ConstantType,
     Datetime,
     EnvConst,
@@ -62,16 +60,14 @@
     "make_const",
     "FormatterGroup",
     "FormatterGroupType",
     "make_group",
     "FormatterArgumentError",
     "FormatterError",
     "FormatterKeyError",
-    "FormatterNotFoundError",
-    "FormatterTypeError",
     "FormatterValueError",
     "FormatterGroupArgumentError",
     "FormatterGroupValueError",
     "Ver",
     "VerPackage",
     "VerSemver",
     "__version__",
```

### Comparing `fmtutil-1.0.2/fmtutil/__type.py` & `fmtutil-1.0.3/fmtutil/__type.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.2/fmtutil/__version.py` & `fmtutil-1.0.3/fmtutil/__version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ------------------------------------------------------------------------------
-# This file license under the BSD-3 License of ``python-semver`` package and
-# BSD and Apache-2.0 License of ``packaging`` package.
+# This file license under the BSD-3 License of the ``python-semver`` package and
+# BSD and Apache-2.0 Licenses of the ``packaging`` package the provide by PyPA.
 # ------------------------------------------------------------------------------
-# refs:
-# * https://github.com/python-semver/python-semver
-# * https://github.com/pypa/packaging
+# references:
+# * [GitHub: Python - semver](https://github.com/python-semver/python-semver)
+# * [GitHub: PYPA - Packaging](https://github.com/pypa/packaging)
 # ------------------------------------------------------------------------------
 from __future__ import annotations
 
 import itertools
 import re
 from collections.abc import Collection, Iterable
 from functools import wraps
```

### Comparing `fmtutil-1.0.2/fmtutil/cli.py` & `fmtutil-1.0.3/fmtutil/cli.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.2/fmtutil/exceptions.py` & `fmtutil-1.0.3/fmtutil/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,35 +17,31 @@
     """
 
 
 class FormatterError(BaseError):
     """Core Base Error object for formatter"""
 
 
-class FormatterNotFoundError(FormatterError):
-    """Error raise for a method not found the config file or data."""
-
-
-class FormatterTypeError(FormatterError):
-    """Error raise for typing does not match or support."""
-
-
 class FormatterValueError(FormatterError):
     """Error raise for value does not valid"""
 
 
 class FormatterKeyError(FormatterError):
     """Error raise for key does not exist"""
 
 
 class FormatterArgumentError(FormatterError):
     """Error raise for a wrong configuration argument.
 
-    >>> FormatterArgumentError(argument='demo', message='does not support')
-    FormatterArgumentError("with 'demo', does not support")
+    Examples:
+        >>> FormatterArgumentError(
+        ...     argument='demo',
+        ...     message='does not support',
+        ... )
+        FormatterArgumentError("with 'demo', does not support")
 
     :param argument: An argument of this error that raise to client
     :type argument: Union[str, tuple]
     :param message: A string message of this error
     :type message: str
     """
 
@@ -71,17 +67,13 @@
                 else f"{_last_arg!r}"
             )
         else:
             _argument = f"{argument!r}"
         super().__init__(f"with {_argument}, {message}")
 
 
-class FormatterGroupError(FormatterError):
-    """Core Base Error object for formatter group"""
-
-
 class FormatterGroupValueError(FormatterValueError):
     """Error raise for value does not valid"""
 
 
 class FormatterGroupArgumentError(FormatterArgumentError):
     """Error raise for a wrong configuration argument."""
```

### Comparing `fmtutil-1.0.2/fmtutil/formatter.py` & `fmtutil-1.0.3/fmtutil/formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,33 +505,37 @@
                     "fmt",
                     (
                         f"The format string, {fmt_str!r}, does not exists in "
                         f"``cls.regex``."
                     ),
                 )
             regex: str = regexes[fmt_str]
-            if _alias_match := re.search(
-                r"^\(\?P<(?P<alias_name>\w+)>(?P<fmt_regex>.+)?\)$",
+            insided: bool = False
+            for fmt_inside in re.finditer(
+                r"\(\?P<(?P<alias>\w+)>(?P<fmt>(?:(?!\(\?P<\w+>).)*)\)",
                 regex,
             ):
-                _sr_re: str = _alias_match.group("alias_name")
-                if alias:
-                    regex = re.sub(
-                        rf"\(\?P<{_sr_re}>",
-                        f"(?P<{_prefix}{_sr_re}__{_cache[fmt_str]}{_suffix}>",
-                        regex,
-                    )
-                else:
-                    regex = re.sub(rf"\(\?P<{_sr_re}>", "(", regex)
-            else:
+                _sr_re: str = fmt_inside.group("alias")
+                regex = re.sub(
+                    rf"\(\?P<{_sr_re}>",
+                    (
+                        f"(?P<{_prefix}{_sr_re}__{_cache[_sr_re]}{_suffix}>"
+                        if alias
+                        else "("
+                    ),
+                    regex,
+                    count=1,
+                )
+                _cache[_sr_re] += 1
+                insided = True
+            if not insided:
                 raise FormatterValueError(
-                    "Regex format string does not set group name for parsing "
-                    "value to its class."
+                    "Regex format string does not set group name for "
+                    "parsing value to its class."
                 )
-            _cache[fmt_str] += 1
             fmt = fmt.replace(fmt_str, regex, 1)
         return fmt
 
     @classmethod
     @lru_cache(maxsize=None)
     def regex(cls) -> DictStr:
         """Return a dict of format string, and it's regular expression value
```

### Comparing `fmtutil-1.0.2/fmtutil/utils.py` & `fmtutil-1.0.3/fmtutil/utils.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.2/.gitignore` & `fmtutil-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.2/LICENSE` & `fmtutil-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.2/README.md` & `fmtutil-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.2/pyproject.toml` & `fmtutil-1.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,17 @@
 perf = [
     "memory-profiler==0.61.0",
 ]
 
 [project.scripts]
 fmtutil = "fmtutil.__main__:main"
 
+[tool.shelf.git]
+commit_prefix_force_fix = true
+
 [tool.shelf.version]
 version = "./fmtutil/__about__.py"
 changelog = "./docs/en/docs/CHANGELOG.md"
 
 [tool.coverage.run]
 branch = true
 concurrency = ["thread", "multiprocessing"]
@@ -70,14 +73,15 @@
     "scripts/",
     "fmtutil/__about__.py",
     "fmtutil/__main__.py",
     "fmtutil/__type.py",
     "fmtutil/__version.py",
     "fmtutil/cli.py",
     "fmtutil/utils.py",
+    "fmtutil/migrate/",
 ]
 relative_files = true
 
 [tool.hatch.version]
 scheme = "standard"
 source = "code"
 path = "fmtutil/__about__.py"
```

### Comparing `fmtutil-1.0.2/PKG-INFO` & `fmtutil-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fmtutil
-Version: 1.0.2
+Version: 1.0.3
 Summary: The Utility Formatter Objects
 Project-URL: Homepage, https://github.com/korawica/fmtutil/
 Project-URL: Source Code, https://github.com/korawica/fmtutil/
 Author-email: korawica <korawich.anu@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: formatter,utility
```

