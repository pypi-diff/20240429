# Comparing `tmp/asserts-0.9.0-py2.py3-none-any.whl.zip` & `tmp/asserts-0.9.1-py3.5.egg`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 11766 bytes, number of entries: 8
--rw-r--r--  2.0 unx    45556 b- defN 18-Aug-31 12:01 asserts/__init__.py
--rw-r--r--  2.0 unx     4899 b- defN 18-Aug-31 11:07 asserts/__init__.pyi
--rw-r--r--  2.0 unx        0 b- defN 18-May-23 18:03 asserts/py.typed
--rw-r--r--  2.0 unx     1083 b- defN 18-Aug-31 12:15 asserts-0.9.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx        8 b- defN 18-Aug-31 12:15 asserts-0.9.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx      110 b- defN 18-Aug-31 12:15 asserts-0.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx     2601 b- defN 18-Aug-31 12:15 asserts-0.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx      622 b- defN 18-Aug-31 12:15 asserts-0.9.0.dist-info/RECORD
-8 files, 54879 bytes uncompressed, 10700 bytes compressed:  80.5%
+Zip file size: 23479 bytes, number of entries: 9
+-rw-r--r--  2.0 unx     3004 b- defN 19-Mar-23 16:15 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      219 b- defN 19-Mar-23 16:15 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 19-Mar-23 16:15 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx        8 b- defN 19-Mar-23 16:15 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 19-Mar-23 16:15 EGG-INFO/zip-safe
+-rw-r--r--  2.0 unx    46625 b- defN 19-Mar-23 16:13 asserts/__init__.py
+-rw-r--r--  2.0 unx     4959 b- defN 19-Mar-23 16:13 asserts/__init__.pyi
+-rw-r--r--  2.0 unx        0 b- defN 19-Mar-23 15:50 asserts/py.typed
+-rw-r--r--  2.0 unx    48700 b- defN 19-Mar-23 16:15 asserts/__pycache__/__init__.cpython-35.pyc
+9 files, 103517 bytes uncompressed, 22367 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
-Filename: asserts/__init__.py
+Filename: EGG-INFO/PKG-INFO
 Comment: 
 
-Filename: asserts/__init__.pyi
+Filename: EGG-INFO/SOURCES.txt
 Comment: 
 
-Filename: asserts/py.typed
+Filename: EGG-INFO/dependency_links.txt
+Comment: 
+
+Filename: EGG-INFO/top_level.txt
 Comment: 
 
-Filename: asserts-0.9.0.dist-info/LICENSE.txt
+Filename: EGG-INFO/zip-safe
 Comment: 
 
-Filename: asserts-0.9.0.dist-info/top_level.txt
+Filename: asserts/__init__.py
 Comment: 
 
-Filename: asserts-0.9.0.dist-info/WHEEL
+Filename: asserts/__init__.pyi
 Comment: 
 
-Filename: asserts-0.9.0.dist-info/METADATA
+Filename: asserts/py.typed
 Comment: 
 
-Filename: asserts-0.9.0.dist-info/RECORD
+Filename: asserts/__pycache__/__init__.cpython-35.pyc
 Comment: 
 
 Zip file comment:
```

## asserts/__init__.py

```diff
@@ -191,15 +191,16 @@
 
     if first == second:
         msg = "{!r} == {!r}".format(first, second)
         fail(msg_fmt.format(msg=msg, first=first, second=second))
 
 
 def assert_almost_equal(
-        first, second, msg_fmt="{msg}", places=None, delta=None):
+    first, second, msg_fmt="{msg}", places=None, delta=None
+):
     """Fail if first and second are not equal after rounding.
 
     By default, the difference between first and second is rounded to
     7 decimal places. This can be configured with the places argument.
     Alternatively, delta can be used to specify the maximum allowed
     difference between first and second.
 
@@ -233,20 +234,24 @@
     else:
         if places is None:
             places = 7
         success = not round(second - first, places)
         detail_msg = "within {} places".format(places)
     if not success:
         msg = "{!r} != {!r} {}".format(first, second, detail_msg)
-        fail(msg_fmt.format(msg=msg, first=first, second=second,
-                            places=places, delta=delta))
+        fail(
+            msg_fmt.format(
+                msg=msg, first=first, second=second, places=places, delta=delta
+            )
+        )
 
 
-def assert_not_almost_equal(first, second, msg_fmt="{msg}",
-                            places=None, delta=None):
+def assert_not_almost_equal(
+    first, second, msg_fmt="{msg}", places=None, delta=None
+):
     """Fail if first and second are equal after rounding.
 
     By default, the difference between first and second is rounded to
     7 decimal places. This can be configured with the places argument.
     Alternatively, delta can be used to specify the maximum allowed
     difference between first and second.
 
@@ -286,20 +291,24 @@
     else:
         if places is None:
             places = 7
         success = bool(round(second - first, places))
         detail_msg = "within {} places".format(places)
     if not success:
         msg = "{!r} == {!r} {}".format(first, second, detail_msg)
-        fail(msg_fmt.format(msg=msg, first=first, second=second,
-                            places=places, delta=delta))
+        fail(
+            msg_fmt.format(
+                msg=msg, first=first, second=second, places=places, delta=delta
+            )
+        )
 
 
-def assert_dict_equal(first, second, key_msg_fmt="{msg}",
-                      value_msg_fmt="{msg}"):
+def assert_dict_equal(
+    first, second, key_msg_fmt="{msg}", value_msg_fmt="{msg}"
+):
     """Fail unless first dictionary equals second.
 
     The dictionaries are considered equal, if they both contain the same
     keys, and their respective values are also equal.
 
     >>> assert_dict_equal({"foo": 5}, {"foo": 5})
     >>> assert_dict_equal({"foo": 5}, {})
@@ -327,44 +336,57 @@
     first_keys = set(first.keys())
     second_keys = set(second.keys())
     missing_keys = list(first_keys - second_keys)
     extra_keys = list(second_keys - first_keys)
     if missing_keys or extra_keys:
         if missing_keys:
             if len(missing_keys) == 1:
-                msg = "key {!r} missing from right dict".format(missing_keys[0])
+                msg = "key {!r} missing from right dict".format(
+                    missing_keys[0]
+                )
             else:
                 keys = ", ".join(sorted(repr(k) for k in missing_keys))
                 msg = "keys {} missing from right dict".format(keys)
         else:
             if len(extra_keys) == 1:
                 msg = "extra key {!r} in right dict".format(extra_keys[0])
             else:
                 keys = ", ".join(sorted(repr(k) for k in extra_keys))
                 msg = "extra keys {} in right dict".format(keys)
         if key_msg_fmt:
             msg = key_msg_fmt.format(
-                msg=msg, first=first, second=second,
-                missing_keys=missing_keys, extra_keys=extra_keys)
+                msg=msg,
+                first=first,
+                second=second,
+                missing_keys=missing_keys,
+                extra_keys=extra_keys,
+            )
         raise AssertionError(msg)
     for key in first:
         first_value = first[key]
         second_value = second[key]
         msg = "key '{}' differs: {!r} != {!r}".format(
-            key, first_value, second_value)
+            key, first_value, second_value
+        )
         if value_msg_fmt:
             msg = value_msg_fmt.format(
-                msg=msg, first=first, second=second,
-                key=key, first_value=first_value, second_value=second_value)
+                msg=msg,
+                first=first,
+                second=second,
+                key=key,
+                first_value=first_value,
+                second_value=second_value,
+            )
         msg = msg.replace("{", "{{").replace("}", "}}")
         assert_equal(first_value, second_value, msg_fmt=msg)
 
 
-def assert_dict_superset(first, second, key_msg_fmt="{msg}",
-                         value_msg_fmt="{msg}"):
+def assert_dict_superset(
+    first, second, key_msg_fmt="{msg}", value_msg_fmt="{msg}"
+):
     """Fail unless second dictionary is a superset of the first.
 
     The second dictionary must contain all keys of the first and their
     values are equal (or a superset in case of dicts). But the second
     dictionary can contain additional keys.
 
     >>> assert_dict_superset({"foo": 5}, {"foo": 5, "bar": 10})
@@ -396,25 +418,32 @@
         if len(missing_keys) == 1:
             msg = "key {!r} missing from right dict".format(missing_keys[0])
         else:
             keys = ", ".join(sorted(repr(k) for k in missing_keys))
             msg = "keys {} missing from right dict".format(keys)
         if key_msg_fmt:
             msg = key_msg_fmt.format(
-                msg=msg, first=first, second=second, missing_keys=missing_keys)
+                msg=msg, first=first, second=second, missing_keys=missing_keys
+            )
         raise AssertionError(msg)
     for key in first:
         first_value = first[key]
         second_value = second[key]
         msg = "key '{}' differs: {!r} != {!r}".format(
-            key, first_value, second_value)
+            key, first_value, second_value
+        )
         if value_msg_fmt:
             msg = value_msg_fmt.format(
-                msg=msg, first=first, second=second,
-                key=key, first_value=first_value, second_value=second_value)
+                msg=msg,
+                first=first,
+                second=second,
+                key=key,
+                first_value=first_value,
+                second_value=second_value,
+            )
         msg = msg.replace("{", "{{").replace("}", "}}")
         assert_equal(first_value, second_value, msg_fmt=msg)
 
 
 def assert_less(first, second, msg_fmt="{msg}"):
     """Fail if first is not less than second.
 
@@ -500,15 +529,15 @@
 def assert_regex(text, regex, msg_fmt="{msg}"):
     """Fail if text does not match the regular expression.
 
     regex can be either a regular expression string or a compiled regular
     expression object.
 
     >>> assert_regex("Hello World!", r"llo.*rld!$")
-    >>> assert_regex("Hello World!", r"\d")
+    >>> assert_regex("Hello World!", r"\\d")
     Traceback (most recent call last):
         ...
     AssertionError: 'Hello World!' does not match '\\\\d'
 
     The following msg_fmt arguments are supported:
     * msg - the default error message
     * text - text that is matched
@@ -640,26 +669,31 @@
                 missing2.append(item)
         return missing1, missing2
 
     def build_message():
         msg = ""
         if missing_from_1:
             msg += "missing from sequence 1: " + ", ".join(
-                repr(i) for i in missing_from_1)
+                repr(i) for i in missing_from_1
+            )
         if missing_from_1 and missing_from_2:
             msg += "; "
         if missing_from_2:
             msg += "missing from sequence 2: " + ", ".join(
-                repr(i) for i in missing_from_2)
+                repr(i) for i in missing_from_2
+            )
         return msg
 
     missing_from_1, missing_from_2 = compare()
     if missing_from_1 or missing_from_2:
-        fail(msg_fmt.format(
-            msg=build_message(), first=sequence1, second=sequence2))
+        fail(
+            msg_fmt.format(
+                msg=build_message(), first=sequence1, second=sequence2
+            )
+        )
 
 
 def assert_between(lower_bound, upper_bound, expr, msg_fmt="{msg}"):
     """Fail if an expression is not between certain bounds (inclusive).
 
     >>> assert_between(5, 15, 5)
     >>> assert_between(5, 15, 15)
@@ -673,17 +707,21 @@
     * lower - lower bound
     * upper - upper bound
     * expr - tested expression
     """
 
     if not lower_bound <= expr <= upper_bound:
         msg = "{!r} is not between {} and {}".format(
-            expr, lower_bound, upper_bound)
-        fail(msg_fmt.format(msg=msg, lower=lower_bound, upper=upper_bound,
-                            expr=expr))
+            expr, lower_bound, upper_bound
+        )
+        fail(
+            msg_fmt.format(
+                msg=msg, lower=lower_bound, upper=upper_bound, expr=expr
+            )
+        )
 
 
 def assert_is_instance(obj, cls, msg_fmt="{msg}"):
     """Fail if an object is not an instance of a class or tuple of classes.
 
     >>> assert_is_instance(5, int)
     >>> assert_is_instance('foo', (str, bytes))
@@ -695,16 +733,17 @@
     The following msg_fmt arguments are supported:
     * msg - the default error message
     * obj - object to test
     * types - tuple of types tested against
     """
     if not isinstance(obj, cls):
         msg = "{!r} is an instance of {!r}, expected {!r}".format(
-            obj, obj.__class__, cls)
-        types = cls if isinstance(cls, tuple) else (cls, )
+            obj, obj.__class__, cls
+        )
+        types = cls if isinstance(cls, tuple) else (cls,)
         fail(msg_fmt.format(msg=msg, obj=obj, types=types))
 
 
 def assert_not_is_instance(obj, cls, msg_fmt="{msg}"):
     """Fail if an object is an instance of a class or tuple of classes.
 
     >>> assert_not_is_instance(5, str)
@@ -855,16 +894,18 @@
             return False
         for test in self._tests:
             test(exc_val)
         return True
 
     def format_message(self, default_msg):
         return self.msg_fmt.format(
-            msg=default_msg, exc_type=self._exc_type,
-            exc_name=self._exception_name)
+            msg=default_msg,
+            exc_type=self._exc_type,
+            exc_name=self._exception_name,
+        )
 
     def add_test(self, cb):
         """Add a test callback.
 
         This callback is called after determining that the right exception
         class was raised. The callback will get the raised exception as only
         argument.
@@ -879,31 +920,38 @@
 
     def __init__(self, exception, pattern, msg_fmt="{msg}"):
         super(AssertRaisesRegexContext, self).__init__(exception, msg_fmt)
         self.pattern = pattern
 
     def format_message(self, default_msg):
         return self.msg_fmt.format(
-            msg=default_msg, exc_type=self._exc_type,
-            exc_name=self._exception_name, pattern=self.pattern, text="")
+            msg=default_msg,
+            exc_type=self._exc_type,
+            exc_name=self._exception_name,
+            pattern=self.pattern,
+            text="",
+        )
 
 
 class AssertRaisesErrnoContext(AssertRaisesContext):
 
     """A context manager to test for exceptions with errnos."""
 
     def __init__(self, exception, expected_errno, msg_fmt="{msg}"):
         super(AssertRaisesErrnoContext, self).__init__(exception, msg_fmt)
         self.expected_errno = expected_errno
 
     def format_message(self, default_msg):
         return self.msg_fmt.format(
-            msg=default_msg, exc_type=self._exc_type,
+            msg=default_msg,
+            exc_type=self._exc_type,
             exc_name=self._exception_name,
-            expected_errno=self.expected_errno, actual_errno=None)
+            expected_errno=self.expected_errno,
+            actual_errno=None,
+        )
 
 
 def assert_raises(exception, msg_fmt="{msg}"):
     """Fail unless a specific exception is raised inside the context.
 
     If a different type of exception is raised, it will not be caught.
 
@@ -934,18 +982,18 @@
 
 def assert_raises_regex(exception, regex, msg_fmt="{msg}"):
     """Fail unless an exception with a message that matches a regular
      expression is raised within the context.
 
     The regular expression can be a regular expression string or object.
 
-    >>> with assert_raises_regex(ValueError, r"\d+"):
+    >>> with assert_raises_regex(ValueError, r"\\d+"):
     ...     raise ValueError("Error #42")
     ...
-    >>> with assert_raises_regex(ValueError, r"\d+"):
+    >>> with assert_raises_regex(ValueError, r"\\d+"):
     ...     raise ValueError("Generic Error")
     ...
     Traceback (most recent call last):
         ...
     AssertionError: 'Generic Error' does not match '\\\\d+'
 
     The following msg_fmt arguments are supported:
@@ -956,23 +1004,35 @@
     * pattern - expected error message as regular expression string
     """
 
     def test(exc):
         compiled = re.compile(regex)
         if not exc.args:
             msg = "{} without message".format(exception.__name__)
-            fail(msg_fmt.format(
-                msg=msg, text=None, pattern=compiled.pattern,
-                exc_type=exception, exc_name=exception.__name__))
+            fail(
+                msg_fmt.format(
+                    msg=msg,
+                    text=None,
+                    pattern=compiled.pattern,
+                    exc_type=exception,
+                    exc_name=exception.__name__,
+                )
+            )
         text = exc.args[0]
         if not compiled.search(text):
             msg = "{!r} does not match {!r}".format(text, compiled.pattern)
-            fail(msg_fmt.format(
-                msg=msg, text=text, pattern=compiled.pattern,
-                exc_type=exception, exc_name=exception.__name__))
+            fail(
+                msg_fmt.format(
+                    msg=msg,
+                    text=text,
+                    pattern=compiled.pattern,
+                    exc_type=exception,
+                    exc_name=exception.__name__,
+                )
+            )
 
     context = AssertRaisesRegexContext(exception, regex, msg_fmt)
     context.add_test(test)
     return context
 
 
 def assert_raises_errno(exception, errno, msg_fmt="{msg}"):
@@ -996,17 +1056,24 @@
     * expected_errno -
     * actual_errno - raised errno or None if no matching exception was raised
     """
 
     def check_errno(exc):
         if errno != exc.errno:
             msg = "wrong errno: {!r} != {!r}".format(errno, exc.errno)
-            fail(msg_fmt.format(msg=msg, exc_type=exception,
-                                exc_name=exception.__name__,
-                                expected_errno=errno, actual_errno=exc.errno))
+            fail(
+                msg_fmt.format(
+                    msg=msg,
+                    exc_type=exception,
+                    exc_name=exception.__name__,
+                    expected_errno=errno,
+                    actual_errno=exc.errno,
+                )
+            )
+
     context = AssertRaisesErrnoContext(exception, errno, msg_fmt)
     context.add_test(check_errno)
     return context
 
 
 def assert_succeeds(exception, msg_fmt="{msg}"):
     """Fail if a specific exception is raised within the context.
@@ -1038,24 +1105,28 @@
     * msg - the default error message
     * exc_type - exception type
     * exc_name - exception type name
     * exception - exception that was raised
     """
 
     class _AssertSucceeds(object):
-
         def __enter__(self):
             pass
 
         def __exit__(self, exc_type, exc_val, exc_tb):
             if exc_type and issubclass(exc_type, exception):
                 msg = exception.__name__ + " was unexpectedly raised"
-                fail(msg_fmt.format(
-                    msg=msg, exc_type=exception, exc_name=exception.__name__,
-                    exception=exc_val))
+                fail(
+                    msg_fmt.format(
+                        msg=msg,
+                        exc_type=exception,
+                        exc_name=exception.__name__,
+                        exception=exc_val,
+                    )
+                )
 
     return _AssertSucceeds()
 
 
 class AssertWarnsContext(object):
 
     """A context manager to test for warnings with certain properties.
@@ -1100,16 +1171,18 @@
         self._warning_context.__exit__(exc_type, exc_val, exc_tb)
         if not any(self._is_expected_warning(w) for w in self._warnings):
             fail(self.format_message())
 
     def format_message(self):
         msg = "{} not issued".format(self._warning_class.__name__)
         return self._msg_fmt.format(
-            msg=msg, exc_type=self._warning_class,
-            exc_name=self._warning_class.__name__)
+            msg=msg,
+            exc_type=self._warning_class,
+            exc_name=self._warning_class.__name__,
+        )
 
     def _is_expected_warning(self, warning):
         if not issubclass(warning.category, self._warning_class):
             return False
         return all(test(warning) for test in self._tests)
 
     def add_test(self, cb):
@@ -1128,20 +1201,23 @@
     """A context manager to test for warnings and their messages."""
 
     def __init__(self, warning_class, pattern, msg_fmt="{msg}"):
         super(AssertWarnsRegexContext, self).__init__(warning_class, msg_fmt)
         self.pattern = pattern
 
     def format_message(self):
-        msg = "no {} matching {} issued".format(self._warning_class.__name__,
-                                                repr(self.pattern))
+        msg = "no {} matching {} issued".format(
+            self._warning_class.__name__, repr(self.pattern)
+        )
         return self._msg_fmt.format(
-            msg=msg, exc_type=self._warning_class,
+            msg=msg,
+            exc_type=self._warning_class,
             exc_name=self._warning_class.__name__,
-            pattern=self.pattern)
+            pattern=self.pattern,
+        )
 
 
 def assert_warns(warning_type, msg_fmt="{msg}"):
     """Fail unless a specific warning is issued inside the context.
 
     If a different type of warning is issued, it will not be caught.
 
@@ -1172,15 +1248,15 @@
 
 def assert_warns_regex(warning_type, regex, msg_fmt="{msg}"):
     """Fail unless a warning with a message is issued inside the context.
 
     The message can be a regular expression string or object.
 
     >>> from warnings import warn
-    >>> with assert_warns_regex(UserWarning, r"#\d+"):
+    >>> with assert_warns_regex(UserWarning, r"#\\d+"):
     ...     warn("Error #42", UserWarning)
     ...
     >>> with assert_warns_regex(UserWarning, r"Expected Error"):
     ...     warn("Generic Error", UserWarning)
     ...
     Traceback (most recent call last):
         ...
@@ -1200,15 +1276,15 @@
     context.add_test(test)
     return context
 
 
 if sys.version_info >= (3,):
     _Str = str
 else:
-    _Str = unicode
+    _Str = unicode  # noqa: F821
 
 
 def assert_json_subset(first, second):
     """Assert that a JSON object or array is a subset of another JSON object
     or array.
 
     The first JSON object or array must be supplied as a JSON-compatible
@@ -1251,16 +1327,19 @@
         second = second.decode("utf-8")
     if isinstance(second, _Str):
         parsed_second = json_loads(second)
     else:
         parsed_second = second
 
     if not isinstance(parsed_second, (dict, list)):
-        raise AssertionError("second must decode to dict or list, not {}".
-                             format(type(parsed_second)))
+        raise AssertionError(
+            "second must decode to dict or list, not {}".format(
+                type(parsed_second)
+            )
+        )
 
     comparer = _JSONComparer(_JSONPath("$"), first, parsed_second)
     comparer.assert_()
 
 
 class _JSONComparer:
     def __init__(self, path, expected, actual):
@@ -1316,40 +1395,47 @@
 
     def _assert_fundamental_values_equal(self):
         if self._expected != self._actual:
             self._raise_different_values()
 
     def _raise_different_values(self):
         self._raise_assertion_error(
-            "element {path} differs: {expected} != {actual}")
+            "element {path} differs: {expected} != {actual}"
+        )
 
     def _raise_different_sizes(self):
         self._raise_assertion_error(
             "JSON array {path} differs in size: "
             "{expected_len} != {actual_len}",
             expected_len=len(self._expected),
-            actual_len=len(self._actual))
+            actual_len=len(self._actual),
+        )
 
     def _raise_missing_element(self, keys):
         if len(keys) == 1:
             format_string = "element {elements} missing from element {path}"
             elements = repr(next(iter(keys)))
         else:
             format_string = "elements {elements} missing from element {path}"
             sorted_keys = sorted(keys)
-            elements = (", ".join(repr(k) for k in sorted_keys[:-1]) +
-                        ", and " + repr(sorted_keys[-1]))
+            elements = (
+                ", ".join(repr(k) for k in sorted_keys[:-1])
+                + ", and "
+                + repr(sorted_keys[-1])
+            )
         self._raise_assertion_error(format_string, elements=elements)
 
     def _raise_assertion_error(self, format_, **kwargs):
-        kwargs.update({
-            "path": self._path,
-            "expected": repr(self._expected),
-            "actual": repr(self._actual),
-        })
+        kwargs.update(
+            {
+                "path": self._path,
+                "expected": repr(self._expected),
+                "actual": repr(self._actual),
+            }
+        )
         raise AssertionError(format_.format(**kwargs))
 
 
 class _JSONPath:
     def __init__(self, path):
         self._path = path
```

## asserts/__init__.pyi

```diff
@@ -1,32 +1,47 @@
 import datetime
 
 from types import TracebackType
-from typing import \
-    Any, Container, Type, Callable, Tuple, Union, ContextManager, \
-    Pattern, Optional, Iterable, Text, NoReturn
+from typing import (
+    Any,
+    Callable,
+    Container,
+    ContextManager,
+    Generic,
+    Iterable,
+    NoReturn,
+    Optional,
+    Pattern,
+    Text,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
 
-class AssertRaisesContext:
-    exception: Type[BaseException]
+_E = TypeVar("_E", bound=BaseException)
+
+class AssertRaisesContext(Generic[_E]):
+    exception: Type[_E]
     msg_fmt: Text
-    def __init__(self, exception: Type[BaseException], msg_fmt: Text = ...) -> None: ...
+    def __init__(self, exception: Type[_E], msg_fmt: Text = ...) -> None: ...
     def __enter__(self) -> AssertRaisesContext: ...
-    def __exit__(self, exc_type: Optional[Type[BaseException]],
-                 exc_val: Optional[BaseException],
-                 exc_tb: Optional[TracebackType]) -> Optional[bool]: ...
+    def __exit__(
+        self, exc_type: Optional[Type[BaseException]], exc_val: Optional[BaseException], exc_tb: Optional[TracebackType]
+    ) -> Optional[bool]: ...
     def format_message(self, default_msg: Text) -> Text: ...
-    def add_test(self, cb: Callable[[BaseException], None]) -> None: ...
+    def add_test(self, cb: Callable[[_E], None]) -> None: ...
 
-class AssertRaisesErrnoContext(AssertRaisesContext):
+class AssertRaisesErrnoContext(AssertRaisesContext[_E]):
     expected_errno: int
-    def __init__(self, exception: Type[BaseException], expected_errno: int, msg_fmt: Text = ...) -> None: ...
+    def __init__(self, exception: Type[_E], expected_errno: int, msg_fmt: Text = ...) -> None: ...
 
-class AssertRaisesRegexContext(AssertRaisesContext):
+class AssertRaisesRegexContext(AssertRaisesContext[_E]):
     pattern: Text
-    def __init__(self, exception: Type[BaseException], pattern: Text, msg_fmt: Text = ...) -> None: ...
+    def __init__(self, exception: Type[_E], pattern: Text, msg_fmt: Text = ...) -> None: ...
 
 class AssertWarnsContext:
     def __init__(self, warning_class: Type[Warning], msg_fmt: Text = ...) -> None: ...
     def __enter__(self) -> None: ...
     def __exit__(self, exc_type: Type[BaseException], exc_val: BaseException, exc_tb: Any) -> None: ...
     def format_message(self) -> Text: ...
     def add_test(self, cb: Callable[[Warning], None]) -> None: ...
@@ -61,13 +76,15 @@
 def assert_is_instance(obj: Any, cls: Union[type, Tuple[type, ...]], msg_fmt: Text = ...) -> None: ...
 def assert_not_is_instance(obj: Any, cls: Union[type, Tuple[type, ...]], msg_fmt: Text = ...) -> None: ...
 def assert_count_equal(sequence1: Iterable[Any], sequence2: Iterable[Any], msg_fmt: Text = ...) -> None: ...
 def assert_has_attr(obj: Any, attribute: str, msg_fmt: Text = ...) -> None: ...
 def assert_datetime_about_now(actual: Optional[datetime.datetime], msg_fmt: Text = ...) -> None: ...
 def assert_datetime_about_now_utc(actual: Optional[datetime.datetime], msg_fmt: Text = ...) -> None: ...
 def assert_raises(exception: Type[BaseException], msg_fmt: Text = ...) -> AssertRaisesContext: ...
-def assert_raises_regex(exception: Type[BaseException], regex: Union[Text, Pattern[Text]], msg_fmt: Text = ...) -> AssertRaisesContext: ...
+def assert_raises_regex(
+    exception: Type[BaseException], regex: Union[Text, Pattern[Text]], msg_fmt: Text = ...
+) -> AssertRaisesContext: ...
 def assert_raises_errno(exception: Type[BaseException], errno: int, msg_fmt: Text = ...) -> AssertRaisesContext: ...
 def assert_succeeds(exception: Type[BaseException], msg_fmt: Text = ...) -> ContextManager: ...
 def assert_warns(warning_type: Type[Warning], msg_fmt: Text = ...) -> AssertWarnsContext: ...
 def assert_warns_regex(warning_type: Type[Warning], regex: Text, msg_fmt: Text = ...) -> AssertWarnsContext: ...
 def assert_json_subset(first: Union[dict, list], second: Union[dict, list, str, bytes]) -> None: ...
```

## Comparing `asserts-0.9.0.dist-info/METADATA` & `EGG-INFO/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,74 +1,72 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: asserts
-Version: 0.9.0
+Version: 0.9.1
 Summary: Stand-alone Assertions
 Home-page: https://github.com/srittau/python-asserts
 Author: Sebastian Rittau
 Author-email: srittau@rittau.biz
 License: MIT
+Description: Python Asserts
+        ==============
+        
+        .. image:: https://img.shields.io/pypi/l/asserts.svg
+           :target: https://pypi.python.org/pypi/asserts/
+        .. image:: https://img.shields.io/github/release/srittau/python-asserts/all.svg
+           :target: https://github.com/srittau/python-asserts/releases/
+        .. image:: https://img.shields.io/pypi/v/asserts.svg
+           :target: https://pypi.python.org/pypi/asserts/
+        .. image:: https://travis-ci.org/srittau/python-asserts.svg?branch=master
+           :target: https://travis-ci.org/srittau/python-asserts
+        
+        Stand-alone Assertions for Python
+        
+        This package provides a few advantages over the assertions provided by
+        unittest.TestCase:
+        
+        * Can be used stand-alone, for example:
+        
+          * In test cases, not derived from TestCase.
+          * In fake and mock classes.
+          * In implementations as rich alternative to the assert statement.
+        
+        * PEP 8 compliance.
+        * Custom stand-alone assertions can be written easily.
+        * Arguably a better separation of concerns, since TestCase is responsible
+          for test running only, if assertion functions are used exclusively.
+        
+        There are a few regressions compared to assertions from TestCase:
+        
+        * The default assertion class (AssertionError) can not be overwritten. This
+          is rarely a problem in practice.
+        * asserts does not support the addTypeEqualityFunc() functionality.
+        
+        Usage:
+        
+        >>> from asserts import assert_true, assert_equal, assert_raises
+        >>> my_var = 13
+        >>> assert_equal(13, my_var)
+        >>> assert_true(True, msg="custom failure message")
+        >>> with assert_raises(KeyError):
+        ...     raise KeyError()
+        
+        Failure messages can be customized:
+        
+        >>> assert_equal(13, 14, msg_fmt="{got} is wrong, expected {expected}")
+        Traceback (most recent call last):
+          ...
+        AssertionError: 14 is wrong, expected 13
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
-
-Python Asserts
-==============
-
-.. image:: https://img.shields.io/pypi/l/asserts.svg
-   :target: https://pypi.python.org/pypi/asserts/
-.. image:: https://img.shields.io/github/release/srittau/python-asserts/all.svg
-   :target: https://github.com/srittau/python-asserts/releases/
-.. image:: https://img.shields.io/pypi/v/asserts.svg
-   :target: https://pypi.python.org/pypi/asserts/
-.. image:: https://travis-ci.org/srittau/python-asserts.svg?branch=master
-   :target: https://travis-ci.org/srittau/python-asserts
-
-Stand-alone Assertions for Python
-
-This package provides a few advantages over the assertions provided by
-unittest.TestCase:
-
-* Can be used stand-alone, for example:
-
-  * In test cases, not derived from TestCase.
-  * In fake and mock classes.
-  * In implementations as rich alternative to the assert statement.
-
-* PEP 8 compliance.
-* Custom stand-alone assertions can be written easily.
-* Arguably a better separation of concerns, since TestCase is responsible
-  for test running only, if assertion functions are used exclusively.
-
-There are a few regressions compared to assertions from TestCase:
-
-* The default assertion class (AssertionError) can not be overwritten. This
-  is rarely a problem in practice.
-* asserts does not support the addTypeEqualityFunc() functionality.
-
-Usage:
-
->>> from asserts import assert_true, assert_equal, assert_raises
->>> my_var = 13
->>> assert_equal(13, my_var)
->>> assert_true(True, msg="custom failure message")
->>> with assert_raises(KeyError):
-...     raise KeyError()
-
-Failure messages can be customized:
-
->>> assert_equal(13, 14, msg_fmt="{got} is wrong, expected {expected}")
-Traceback (most recent call last):
-  ...
-AssertionError: 14 is wrong, expected 13
-
-
```

