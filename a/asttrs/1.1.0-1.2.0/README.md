# Comparing `tmp/asttrs-1.1.0.tar.gz` & `tmp/asttrs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asttrs-1.1.0.tar", last modified: Wed Apr 24 23:02:22 2024, max compression
+gzip compressed data, was "asttrs-1.2.0.tar", last modified: Mon Apr 29 13:40:07 2024, max compression
```

## Comparing `asttrs-1.1.0.tar` & `asttrs-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-24 23:02:22.837069 asttrs-1.1.0/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1062 2021-09-26 15:04:09.000000 asttrs-1.1.0/LICENSE
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2859 2024-04-24 23:02:22.837069 asttrs-1.1.0/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     2547 2023-12-23 20:09:41.000000 asttrs-1.1.0/README.md
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      546 2024-04-24 23:01:45.000000 asttrs-1.1.0/pyproject.toml
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       38 2024-04-24 23:02:22.837069 asttrs-1.1.0/setup.cfg
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-24 23:02:22.833069 asttrs-1.1.0/src/
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-24 23:02:22.837069 asttrs-1.1.0/src/asttrs/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       28 2022-04-04 10:33:54.000000 asttrs-1.1.0/src/asttrs/__init__.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1892 2024-04-23 16:30:14.000000 asttrs-1.1.0/src/asttrs/_ast.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     5719 2023-12-31 14:22:25.000000 asttrs-1.1.0/src/asttrs/_base.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    53618 2023-12-23 17:33:56.000000 asttrs-1.1.0/src/asttrs/_py3_10.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    56914 2024-04-23 16:24:32.000000 asttrs-1.1.0/src/asttrs/_py3_11.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    60807 2024-04-24 23:00:08.000000 asttrs-1.1.0/src/asttrs/_py3_12.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     8838 2023-12-23 17:28:57.000000 asttrs-1.1.0/src/asttrs/_py3_7.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     9314 2023-12-23 17:29:36.000000 asttrs-1.1.0/src/asttrs/_py3_8.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)    41099 2023-12-23 17:30:42.000000 asttrs-1.1.0/src/asttrs/_py3_9.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      857 2023-12-27 04:28:14.000000 asttrs-1.1.0/src/asttrs/utils.py
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-24 23:02:22.837069 asttrs-1.1.0/src/asttrs.egg-info/
--rw-r--r--   0 ryan      (1000) ryan      (1000)     2859 2024-04-24 23:02:22.000000 asttrs-1.1.0/src/asttrs.egg-info/PKG-INFO
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      512 2024-04-24 23:02:22.000000 asttrs-1.1.0/src/asttrs.egg-info/SOURCES.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2024-04-24 23:02:22.000000 asttrs-1.1.0/src/asttrs.egg-info/dependency_links.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)       40 2024-04-24 23:02:22.000000 asttrs-1.1.0/src/asttrs.egg-info/requires.txt
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        7 2024-04-24 23:02:22.000000 asttrs-1.1.0/src/asttrs.egg-info/top_level.txt
-drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-24 23:02:22.837069 asttrs-1.1.0/tests/
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-02-21 14:53:28.000000 asttrs-1.1.0/tests/test_expr.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)     1266 2022-04-04 12:18:55.000000 asttrs-1.1.0/tests/test_misc.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-02-21 17:08:43.000000 asttrs-1.1.0/tests/test_operator.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-02-21 14:54:10.000000 asttrs-1.1.0/tests/test_stmt.py
--rw-rw-r--   0 ryan      (1000) ryan      (1000)      420 2023-12-23 18:31:52.000000 asttrs-1.1.0/tests/test_utils.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-29 13:40:07.219015 asttrs-1.2.0/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1062 2021-09-26 15:04:09.000000 asttrs-1.2.0/LICENSE
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3180 2024-04-29 13:40:07.215015 asttrs-1.2.0/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2565 2024-04-28 12:37:31.000000 asttrs-1.2.0/README.md
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      838 2024-04-29 13:35:21.000000 asttrs-1.2.0/pyproject.toml
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       38 2024-04-29 13:40:07.219015 asttrs-1.2.0/setup.cfg
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-29 13:40:07.191015 asttrs-1.2.0/src/
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-29 13:40:07.215015 asttrs-1.2.0/src/asttrs/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       28 2022-04-04 10:33:54.000000 asttrs-1.2.0/src/asttrs/__init__.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1892 2024-04-23 16:30:14.000000 asttrs-1.2.0/src/asttrs/_ast.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     5719 2023-12-31 14:22:25.000000 asttrs-1.2.0/src/asttrs/_base.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    53618 2023-12-23 17:33:56.000000 asttrs-1.2.0/src/asttrs/_py3_10.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    56938 2024-04-28 12:30:48.000000 asttrs-1.2.0/src/asttrs/_py3_11.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    60927 2024-04-29 13:38:18.000000 asttrs-1.2.0/src/asttrs/_py3_12.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     8838 2023-12-23 17:28:57.000000 asttrs-1.2.0/src/asttrs/_py3_7.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     9314 2023-12-23 17:29:36.000000 asttrs-1.2.0/src/asttrs/_py3_8.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    41099 2023-12-23 17:30:42.000000 asttrs-1.2.0/src/asttrs/_py3_9.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      857 2023-12-27 04:28:14.000000 asttrs-1.2.0/src/asttrs/utils.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-29 13:40:07.215015 asttrs-1.2.0/src/asttrs.egg-info/
+-rw-r--r--   0 ryan      (1000) ryan      (1000)     3180 2024-04-29 13:40:07.000000 asttrs-1.2.0/src/asttrs.egg-info/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      512 2024-04-29 13:40:07.000000 asttrs-1.2.0/src/asttrs.egg-info/SOURCES.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2024-04-29 13:40:07.000000 asttrs-1.2.0/src/asttrs.egg-info/dependency_links.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       40 2024-04-29 13:40:07.000000 asttrs-1.2.0/src/asttrs.egg-info/requires.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        7 2024-04-29 13:40:07.000000 asttrs-1.2.0/src/asttrs.egg-info/top_level.txt
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2024-04-29 13:40:07.215015 asttrs-1.2.0/tests/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-02-21 14:53:28.000000 asttrs-1.2.0/tests/test_expr.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1266 2022-04-04 12:18:55.000000 asttrs-1.2.0/tests/test_misc.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-02-21 17:08:43.000000 asttrs-1.2.0/tests/test_operator.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        0 2022-02-21 14:54:10.000000 asttrs-1.2.0/tests/test_stmt.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      420 2023-12-23 18:31:52.000000 asttrs-1.2.0/tests/test_utils.py
```

### Comparing `asttrs-1.1.0/LICENSE` & `asttrs-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asttrs-1.1.0/PKG-INFO` & `asttrs-1.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,21 @@
-Metadata-Version: 2.1
-Name: asttrs
-Version: 1.1.0
-Summary: A attrs-style wrapper for python ast
-Author-email: ryanchao2012 <ryanchao2012@gmail.com>
-License: MIT
-Project-URL: repository, https://github.com/ryanchao2012/asttrs
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![](https://github.com/ryanchao2012/asttrs/actions/workflows/asttrs-run-unittests.yml/badge.svg)
 ![](https://img.shields.io/pypi/v/asttrs.svg)
 ![](https://img.shields.io/pypi/pyversions/asttrs)
 ![](https://img.shields.io/github/license/ryanchao2012/asttrs)
 
 # asttrs
 A attrs-style wrapper for python ast
 
 
 ## Features
 
-### 1. Developer-friendly version of `ast`, 1) easier to access docstring and 2) easier to do codegen.
-
+### Developer-friendly version of `ast`
+1. easier to access docstring.
+2. easier to do codegen.
 
 ```python
 from ast import FunctionDef
 
 help(FunctionDef)
 # Help on class FunctionDef in module ast:
 
@@ -64,27 +54,27 @@
 #  |  first (i.e. the first in the list will be applied last).
 #  |  * ``returns`` is the return annotation.
 #  |  .. attribute:: type_comment
 #  |  ``type_comment`` is an optional string with the type annotation as a comment.
 #  :
 
 
-# Then we can easily know how to build a function
+# It's easier to know how to build a function
 from asttrs import arguments, Return, Constant
 
 func = FunctionDef(name="foo", args=arguments(), body=[Return(value=Constant(value="Hello World"))])
 
 print(func.to_source())
 # def foo():
 #     return 'Hello World'
 #
 
 ```
 
-### 2. provide `Comment` to codegen comments
+### Provide `Comment` to codegen comments
 
 ```python
 from asttrs import Comment
 
 
 comment = Comment(body="This is a comment,\nsecond line,\nthird line.")
 print(comment.to_souce())
@@ -101,9 +91,9 @@
 $ (cd cpython; git checkout v3.11.7) 
 $ ln -vsfT .venv311 .venv
 
 # run codegen based on Python.asdl
 $ pdm run inv build | pdm run black - >! src/asttrs/_py3_11.py
 
 # run testing
-$ pdm run pytest --doctest-modules --cov=src --cov-report=term-missing tests
-```
+$ pdm run pytest --doctest-modules --cov=asttrs._py3_11 --cov-report=term-missing src/asttrs/_py3_11.py tests
+```
```

### Comparing `asttrs-1.1.0/README.md` & `asttrs-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,38 @@
+Metadata-Version: 2.1
+Name: asttrs
+Version: 1.2.0
+Summary: A attrs-style wrapper for python ast
+Author-email: ryanchao2012 <ryanchao2012@gmail.com>
+License: MIT
+Project-URL: repository, https://github.com/ryanchao2012/asttrs
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![](https://github.com/ryanchao2012/asttrs/actions/workflows/asttrs-run-unittests.yml/badge.svg)
 ![](https://img.shields.io/pypi/v/asttrs.svg)
 ![](https://img.shields.io/pypi/pyversions/asttrs)
 ![](https://img.shields.io/github/license/ryanchao2012/asttrs)
 
 # asttrs
 A attrs-style wrapper for python ast
 
 
 ## Features
 
-### 1. Developer-friendly version of `ast`, 1) easier to access docstring and 2) easier to do codegen.
-
+### Developer-friendly version of `ast`
+1. easier to access docstring.
+2. easier to do codegen.
 
 ```python
 from ast import FunctionDef
 
 help(FunctionDef)
 # Help on class FunctionDef in module ast:
 
@@ -53,27 +71,27 @@
 #  |  first (i.e. the first in the list will be applied last).
 #  |  * ``returns`` is the return annotation.
 #  |  .. attribute:: type_comment
 #  |  ``type_comment`` is an optional string with the type annotation as a comment.
 #  :
 
 
-# Then we can easily know how to build a function
+# It's easier to know how to build a function
 from asttrs import arguments, Return, Constant
 
 func = FunctionDef(name="foo", args=arguments(), body=[Return(value=Constant(value="Hello World"))])
 
 print(func.to_source())
 # def foo():
 #     return 'Hello World'
 #
 
 ```
 
-### 2. provide `Comment` to codegen comments
+### Provide `Comment` to codegen comments
 
 ```python
 from asttrs import Comment
 
 
 comment = Comment(body="This is a comment,\nsecond line,\nthird line.")
 print(comment.to_souce())
@@ -90,9 +108,9 @@
 $ (cd cpython; git checkout v3.11.7) 
 $ ln -vsfT .venv311 .venv
 
 # run codegen based on Python.asdl
 $ pdm run inv build | pdm run black - >! src/asttrs/_py3_11.py
 
 # run testing
-$ pdm run pytest --doctest-modules --cov=src --cov-report=term-missing tests
-```
+$ pdm run pytest --doctest-modules --cov=asttrs._py3_11 --cov-report=term-missing src/asttrs/_py3_11.py tests
+```
```

### Comparing `asttrs-1.1.0/src/asttrs/_ast.py` & `asttrs-1.2.0/src/asttrs/_ast.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.1.0/src/asttrs/_base.py` & `asttrs-1.2.0/src/asttrs/_base.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.1.0/src/asttrs/_py3_10.py` & `asttrs-1.2.0/src/asttrs/_py3_10.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.1.0/src/asttrs/_py3_11.py` & `asttrs-1.2.0/src/asttrs/_py3_11.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     >>> FunctionType(
     ...     argtypes=[
     ...         Name(id='int', ctx=Load()),
     ...         Name(id='str', ctx=Load())],
     ...     returns=Subscript(
     ...         value=Name(id='List', ctx=Load()),
     ...         slice=Name(id='int', ctx=Load()),
-    ...         ctx=Load())).show()
+    ...         ctx=Load())).show()        # doctest: +SKIP
     (int, str) -> List[int]
     """
 
     argtypes: LIST["expr"] = attr.ib(factory=list)
     returns: "expr"
```

### Comparing `asttrs-1.1.0/src/asttrs/_py3_12.py` & `asttrs-1.2.0/src/asttrs/_py3_12.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     >>> FunctionType(
     ...     argtypes=[
     ...         Name(id='int', ctx=Load()),
     ...         Name(id='str', ctx=Load())],
     ...     returns=Subscript(
     ...         value=Name(id='List', ctx=Load()),
     ...         slice=Name(id='int', ctx=Load()),
-    ...         ctx=Load())).show()
+    ...         ctx=Load())).show()        # doctest: +SKIP
     (int, str) -> List[int]
     """
 
     argtypes: LIST["expr"] = attr.ib(factory=list)
     returns: "expr"
 
 
@@ -306,15 +306,15 @@
 
     >>> Module(
     ...     body=[
     ...         TypeAlias(
     ...             name=Name(id='Alias', ctx=Store()),
     ...             type_params=[],
     ...             value=Name(id='int', ctx=Load()))],
-    ...     type_ignores=[]).show()
+    ...     type_ignores=[]).show()        # doctest: +SKIP
     type Alias = int
     """
 
     name: "expr"
     type_params: LIST["type_param"] = attr.ib(factory=list)
     value: "expr"
 
@@ -2146,15 +2146,15 @@
     ...                 TypeVar(
     ...                     name='T',
     ...                     bound=Name(id='int', ctx=Load()))],
     ...             value=Subscript(
     ...                 value=Name(id='list', ctx=Load()),
     ...                 slice=Name(id='T', ctx=Load()),
     ...                 ctx=Load()))],
-    ...     type_ignores=[]).show()
+    ...     type_ignores=[]).show()        # doctest: +SKIP
     type Alias[T: int] = list[T]
     """
 
     name: "identifier"
     bound: "expr" = None
 
 
@@ -2175,15 +2175,15 @@
     ...                 value=Name(id='Callable', ctx=Load()),
     ...                 slice=Tuple(
     ...                     elts=[
     ...                         Name(id='P', ctx=Load()),
     ...                         Name(id='int', ctx=Load())],
     ...                     ctx=Load()),
     ...                 ctx=Load()))],
-    ...     type_ignores=[]).show()
+    ...     type_ignores=[]).show()        # doctest: +SKIP
     type Alias[**P] = Callable[P, int]
     """
 
     name: "identifier"
 
 
 @immutable
@@ -2204,12 +2204,12 @@
     ...                 slice=Tuple(
     ...                     elts=[
     ...                         Starred(
     ...                             value=Name(id='Ts', ctx=Load()),
     ...                             ctx=Load())],
     ...                     ctx=Load()),
     ...                 ctx=Load()))],
-    ...     type_ignores=[]).show()
+    ...     type_ignores=[]).show()        # doctest: +SKIP
     type Alias[*Ts] = tuple[*Ts]
     """
 
     name: "identifier"
```

### Comparing `asttrs-1.1.0/src/asttrs/_py3_7.py` & `asttrs-1.2.0/src/asttrs/_py3_7.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.1.0/src/asttrs/_py3_8.py` & `asttrs-1.2.0/src/asttrs/_py3_8.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.1.0/src/asttrs/_py3_9.py` & `asttrs-1.2.0/src/asttrs/_py3_9.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.1.0/src/asttrs/utils.py` & `asttrs-1.2.0/src/asttrs/utils.py`

 * *Files identical despite different names*

### Comparing `asttrs-1.1.0/src/asttrs.egg-info/PKG-INFO` & `asttrs-1.2.0/src/asttrs.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Metadata-Version: 2.1
 Name: asttrs
-Version: 1.1.0
+Version: 1.2.0
 Summary: A attrs-style wrapper for python ast
 Author-email: ryanchao2012 <ryanchao2012@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/ryanchao2012/asttrs
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![](https://github.com/ryanchao2012/asttrs/actions/workflows/asttrs-run-unittests.yml/badge.svg)
 ![](https://img.shields.io/pypi/v/asttrs.svg)
 ![](https://img.shields.io/pypi/pyversions/asttrs)
@@ -16,16 +22,17 @@
 
 # asttrs
 A attrs-style wrapper for python ast
 
 
 ## Features
 
-### 1. Developer-friendly version of `ast`, 1) easier to access docstring and 2) easier to do codegen.
-
+### Developer-friendly version of `ast`
+1. easier to access docstring.
+2. easier to do codegen.
 
 ```python
 from ast import FunctionDef
 
 help(FunctionDef)
 # Help on class FunctionDef in module ast:
 
@@ -64,27 +71,27 @@
 #  |  first (i.e. the first in the list will be applied last).
 #  |  * ``returns`` is the return annotation.
 #  |  .. attribute:: type_comment
 #  |  ``type_comment`` is an optional string with the type annotation as a comment.
 #  :
 
 
-# Then we can easily know how to build a function
+# It's easier to know how to build a function
 from asttrs import arguments, Return, Constant
 
 func = FunctionDef(name="foo", args=arguments(), body=[Return(value=Constant(value="Hello World"))])
 
 print(func.to_source())
 # def foo():
 #     return 'Hello World'
 #
 
 ```
 
-### 2. provide `Comment` to codegen comments
+### Provide `Comment` to codegen comments
 
 ```python
 from asttrs import Comment
 
 
 comment = Comment(body="This is a comment,\nsecond line,\nthird line.")
 print(comment.to_souce())
@@ -101,9 +108,9 @@
 $ (cd cpython; git checkout v3.11.7) 
 $ ln -vsfT .venv311 .venv
 
 # run codegen based on Python.asdl
 $ pdm run inv build | pdm run black - >! src/asttrs/_py3_11.py
 
 # run testing
-$ pdm run pytest --doctest-modules --cov=src --cov-report=term-missing tests
+$ pdm run pytest --doctest-modules --cov=asttrs._py3_11 --cov-report=term-missing src/asttrs/_py3_11.py tests
 ```
```

### Comparing `asttrs-1.1.0/src/asttrs.egg-info/SOURCES.txt` & `asttrs-1.2.0/src/asttrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asttrs-1.1.0/tests/test_misc.py` & `asttrs-1.2.0/tests/test_misc.py`

 * *Files identical despite different names*

