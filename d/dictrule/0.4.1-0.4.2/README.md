# Comparing `tmp/dictrule-0.4.1.tar.gz` & `tmp/dictrule-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictrule-0.4.1.tar", last modified: Fri Apr 19 19:27:28 2024, max compression
+gzip compressed data, was "dictrule-0.4.2.tar", last modified: Mon Apr 29 10:10:28 2024, max compression
```

## Comparing `dictrule-0.4.1.tar` & `dictrule-0.4.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:27:28.072445 dictrule-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-19 19:27:25.000000 dictrule-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12889 2024-04-19 19:27:28.068445 dictrule-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11592 2024-04-19 19:27:25.000000 dictrule-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:27:28.072445 dictrule-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-19 19:27:25.000000 dictrule-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:27:28.064445 dictrule-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:27:28.068445 dictrule-0.4.1/src/dictrule/
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:27:28.068445 dictrule-0.4.1/src/dictrule/built_in_rules/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/block_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/comment_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/eval_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/for_in_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/format_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/indent_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/inline_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/join_block_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/join_eval_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/built_in_rules/stringify_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/dr_property.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/var_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-19 19:27:25.000000 dictrule-0.4.1/src/dictrule/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:27:28.068445 dictrule-0.4.1/src/dictrule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12889 2024-04-19 19:27:28.000000 dictrule-0.4.1/src/dictrule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-19 19:27:28.000000 dictrule-0.4.1/src/dictrule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:27:28.000000 dictrule-0.4.1/src/dictrule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:27:28.000000 dictrule-0.4.1/src/dictrule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-19 19:27:28.000000 dictrule-0.4.1/src/dictrule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:28.700837 dictrule-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-29 10:10:25.000000 dictrule-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-04-29 10:10:28.700837 dictrule-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-04-29 10:10:25.000000 dictrule-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 10:10:28.700837 dictrule-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-29 10:10:25.000000 dictrule-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:28.692836 dictrule-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:28.696836 dictrule-0.4.2/src/dictrule/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:28.700837 dictrule-0.4.2/src/dictrule/built_in_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/block_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/comment_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/eval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7339 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/for_in_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/format_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4104 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/indent_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/inline_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/join_block_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/join_eval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/built_in_rules/stringify_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3891 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/dr_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/var_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4281 2024-04-29 10:10:25.000000 dictrule-0.4.2/src/dictrule/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 10:10:28.700837 dictrule-0.4.2/src/dictrule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-04-29 10:10:28.000000 dictrule-0.4.2/src/dictrule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-29 10:10:28.000000 dictrule-0.4.2/src/dictrule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:10:28.000000 dictrule-0.4.2/src/dictrule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 10:10:28.000000 dictrule-0.4.2/src/dictrule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-29 10:10:28.000000 dictrule-0.4.2/src/dictrule.egg-info/top_level.txt
```

### Comparing `dictrule-0.4.1/LICENSE` & `dictrule-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/PKG-INFO` & `dictrule-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictrule
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python rules defined by a dict and a text generator from the rules
 Home-page: https://github.com/elhoangvu/dictrule
 Author: Zooxy Le
 Author-email: elhoangvu@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/elhoangvu/dictrule
 Project-URL: Source, https://github.com/elhoangvu/dictrule
@@ -174,15 +174,15 @@
 **Example**
 
 ```python
 >>> context = build_singleline_context("#")
 >>> dictrule.Generator({
 ...     "comment": "This is a single-line comment"
 ... }).generate(context)
-"# This is a single-line comment"
+# This is a single-line comment
 
 >>> context = build_multiline_context('"""')
 >>> dictrule.Generator({
 ...     "style": "multiline",
 ...     "comment": [
 ...         "line1": "Line 1 of multi-line comment",
 ...         "line2": "Line 2 of multi-line comment",
```

### Comparing `dictrule-0.4.1/README.md` & `dictrule-0.4.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
 **Example**
 
 ```python
 >>> context = build_singleline_context("#")
 >>> dictrule.Generator({
 ...     "comment": "This is a single-line comment"
 ... }).generate(context)
-"# This is a single-line comment"
+# This is a single-line comment
 
 >>> context = build_multiline_context('"""')
 >>> dictrule.Generator({
 ...     "style": "multiline",
 ...     "comment": [
 ...         "line1": "Line 1 of multi-line comment",
 ...         "line2": "Line 2 of multi-line comment",
```

### Comparing `dictrule-0.4.1/setup.py` & `dictrule-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/__init__.py` & `dictrule-0.4.2/src/dictrule/__init__.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/__version__.py` & `dictrule-0.4.2/src/dictrule/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 \__,_/_/\___/\__/_/   \__,_/_/\___/    |___/\___/_/  /____/_/\____/_/ /_/ 
                                                                           
 """
 
 __title__ = "dictrule"
 __description__ = "Python rules defined by a dict and a text generator from the rules"
 __url__ = "https://github.com/elhoangvu/dictrule"
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 __author__ = "Zooxy Le"
 __author_email__ = "elhoangvu@gmail.com"
 __license__ = "MIT License"
 __copyright__ = "Copyright Zooxy Le"
```

### Comparing `dictrule-0.4.1/src/dictrule/built_in_rules/__init__.py` & `dictrule-0.4.2/src/dictrule/built_in_rules/__init__.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/built_in_rules/block_rule.py` & `dictrule-0.4.2/src/dictrule/built_in_rules/block_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/built_in_rules/comment_rule.py` & `dictrule-0.4.2/src/dictrule/built_in_rules/comment_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     Examples:
     ---------
     >>> context = build_singleline_context("#")
     >>> dictrule.Generator({
     ...     "comment": "This is a single-line comment"
     ... }).generate(context)
-    "# This is a single-line comment"
+    # This is a single-line comment
 
     >>> context = build_multiline_context('\"""')
     >>> dictrule.Generator({
     ...     "style": "multiline",
     ...     "comment": [
     ...         "line1": "Line 1 of multi-line comment",
     ...         "line2": "Line 2 of multi-line comment",
```

### Comparing `dictrule-0.4.1/src/dictrule/built_in_rules/eval_rule.py` & `dictrule-0.4.2/src/dictrule/built_in_rules/eval_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/built_in_rules/for_in_rule.py` & `dictrule-0.4.2/src/dictrule/built_in_rules/for_in_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/built_in_rules/format_rule.py` & `dictrule-0.4.2/src/dictrule/built_in_rules/format_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/built_in_rules/indent_rule.py` & `dictrule-0.4.2/src/dictrule/built_in_rules/indent_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/built_in_rules/inline_rule.py` & `dictrule-0.4.2/src/dictrule/built_in_rules/inline_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/built_in_rules/join_block_rule.py` & `dictrule-0.4.2/src/dictrule/built_in_rules/join_block_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/built_in_rules/join_eval_rule.py` & `dictrule-0.4.2/src/dictrule/built_in_rules/join_eval_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/built_in_rules/stringify_rule.py` & `dictrule-0.4.2/src/dictrule/built_in_rules/stringify_rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/context.py` & `dictrule-0.4.2/src/dictrule/context.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/dr_property.py` & `dictrule-0.4.2/src/dictrule/dr_property.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/generator.py` & `dictrule-0.4.2/src/dictrule/generator.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/rule.py` & `dictrule-0.4.2/src/dictrule/rule.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule/var_property.py` & `dictrule-0.4.2/src/dictrule/var_property.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,57 +48,57 @@
         self.fset = fset
         self.fdel = fdel
         if doc is None and fget is not None:
             doc = fget.__doc__
         self.__doc__ = doc
         self.__name__ = fget.__name__
 
-    def __get__(self, obj, objtype=None):
+    def __get__(self, obj, objtype=None) -> Any:
         if obj is None:
             return self
         if self.fget is None:
             raise AttributeError("unreadable attribute")
         return self.fget(obj)
 
-    def __set__(self, obj, value):
+    def __set__(self, obj, value) -> None:
         if self.fset is None:
             raise AttributeError("can't set attribute")
         self.fset(obj, value)
 
-    def __delete__(self, obj):
+    def __delete__(self, obj) -> None:
         if self.fdel is None:
             raise AttributeError("can't delete attribute")
         self.fdel(obj)
 
-    def getter(self, fget):
+    def getter(self, fget) -> "var_property":
         """Getter decorator
 
         Examples:
         ---------
         >>> class Sample:
         ...     @var_property
         ...     def name(self):
         ...         return "Zooxy"
         >>> Sample().name
         Zooxy
         """
         return type(self)(fget, self.fset, self.fdel, self.__doc__)
 
-    def setter(self, fset):
+    def setter(self, fset) -> "var_property":
         """Setter decorator
 
         Examples:
         ---------
         >>> @name.setter
         ... def name(self, value: Any):
         ...     self._name = value
         """
         return type(self)(self.fget, fset, self.fdel, self.__doc__)
 
-    def deleter(self, fdel):
+    def deleter(self, fdel) -> "var_property":
         """Deleter decorator
 
         Examples:
         ---------
         >>> @name.deleter
         ... def name(self):
         ...     del self._name
```

### Comparing `dictrule-0.4.1/src/dictrule/variable.py` & `dictrule-0.4.2/src/dictrule/variable.py`

 * *Files identical despite different names*

### Comparing `dictrule-0.4.1/src/dictrule.egg-info/PKG-INFO` & `dictrule-0.4.2/src/dictrule.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictrule
-Version: 0.4.1
+Version: 0.4.2
 Summary: Python rules defined by a dict and a text generator from the rules
 Home-page: https://github.com/elhoangvu/dictrule
 Author: Zooxy Le
 Author-email: elhoangvu@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/elhoangvu/dictrule
 Project-URL: Source, https://github.com/elhoangvu/dictrule
@@ -174,15 +174,15 @@
 **Example**
 
 ```python
 >>> context = build_singleline_context("#")
 >>> dictrule.Generator({
 ...     "comment": "This is a single-line comment"
 ... }).generate(context)
-"# This is a single-line comment"
+# This is a single-line comment
 
 >>> context = build_multiline_context('"""')
 >>> dictrule.Generator({
 ...     "style": "multiline",
 ...     "comment": [
 ...         "line1": "Line 1 of multi-line comment",
 ...         "line2": "Line 2 of multi-line comment",
```

### Comparing `dictrule-0.4.1/src/dictrule.egg-info/SOURCES.txt` & `dictrule-0.4.2/src/dictrule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

