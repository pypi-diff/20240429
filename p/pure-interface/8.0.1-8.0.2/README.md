# Comparing `tmp/pure-interface-8.0.1.tar.gz` & `tmp/pure_interface-8.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pure-interface-8.0.1.tar", last modified: Tue Mar  5 03:48:44 2024, max compression
+gzip compressed data, was "pure_interface-8.0.2.tar", last modified: Sun Apr 28 22:38:51 2024, max compression
```

## Comparing `pure-interface-8.0.1.tar` & `pure_interface-8.0.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-03-05 03:48:44.955882 pure-interface-8.0.1/
--rw-rw-rw-   0        0        0     1070 2021-09-21 22:43:47.000000 pure-interface-8.0.1/LICENSE
--rw-rw-rw-   0        0        0    38685 2024-03-05 03:48:44.953875 pure-interface-8.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    36311 2024-03-05 03:42:39.000000 pure-interface-8.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2024-03-05 03:48:44.799773 pure-interface-8.0.1/pure_interface/
--rw-rw-rw-   0        0        0      559 2024-03-05 02:18:50.000000 pure-interface-8.0.1/pure_interface/__init__.py
--rw-rw-rw-   0        0        0     2858 2023-11-16 00:00:03.000000 pure-interface-8.0.1/pure_interface/_sub_interface.py
--rw-rw-rw-   0        0        0     7972 2023-11-16 00:00:03.000000 pure-interface-8.0.1/pure_interface/adaption.py
--rw-rw-rw-   0        0        0     8730 2023-11-16 00:00:03.000000 pure-interface-8.0.1/pure_interface/delegation.py
--rw-rw-rw-   0        0        0      374 2023-07-21 02:33:09.000000 pure-interface-8.0.1/pure_interface/errors.py
--rw-rw-rw-   0        0        0    35237 2024-03-05 03:23:27.000000 pure-interface-8.0.1/pure_interface/interface.py
--rw-rw-rw-   0        0        0     8775 2023-11-16 00:00:03.000000 pure-interface-8.0.1/pure_interface/mypy_plugin.py
--rw-rw-rw-   0        0        0        0 2023-05-11 00:43:53.000000 pure-interface-8.0.1/pure_interface/py.typed
-drwxrwxrwx   0        0        0        0 2024-03-05 03:48:44.951875 pure-interface-8.0.1/pure_interface.egg-info/
--rw-rw-rw-   0        0        0    38685 2024-03-05 03:48:44.000000 pure-interface-8.0.1/pure_interface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      920 2024-03-05 03:48:44.000000 pure-interface-8.0.1/pure_interface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-05 03:48:44.000000 pure-interface-8.0.1/pure_interface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-03-05 03:48:44.000000 pure-interface-8.0.1/pure_interface.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-05 03:48:44.000000 pure-interface-8.0.1/pure_interface.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1259 2023-11-16 00:00:03.000000 pure-interface-8.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-05 03:48:44.956875 pure-interface-8.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-05 03:48:44.949874 pure-interface-8.0.1/tests/
--rw-rw-rw-   0        0        0     4281 2023-11-16 00:00:03.000000 pure-interface-8.0.1/tests/test_adapt_args_anno.py
--rw-rw-rw-   0        0        0     2836 2023-11-16 00:00:03.000000 pure-interface-8.0.1/tests/test_adapt_args_no_anno.py
--rw-rw-rw-   0        0        0    12672 2023-11-16 00:00:03.000000 pure-interface-8.0.1/tests/test_adaption.py
--rw-rw-rw-   0        0        0     2883 2024-03-05 03:47:14.000000 pure-interface-8.0.1/tests/test_dataclass_support.py
--rw-rw-rw-   0        0        0     9760 2023-11-16 00:00:03.000000 pure-interface-8.0.1/tests/test_delegate.py
--rw-rw-rw-   0        0        0     5930 2023-07-21 02:33:09.000000 pure-interface-8.0.1/tests/test_func_sigs3.py
--rw-rw-rw-   0        0        0     2729 2023-11-16 00:00:03.000000 pure-interface-8.0.1/tests/test_func_sigs_po.py
--rw-rw-rw-   0        0        0    11706 2023-11-16 00:00:03.000000 pure-interface-8.0.1/tests/test_function_sigs.py
--rw-rw-rw-   0        0        0     1061 2023-11-16 00:00:03.000000 pure-interface-8.0.1/tests/test_generic_support.py
--rw-rw-rw-   0        0        0    16258 2023-11-16 00:00:03.000000 pure-interface-8.0.1/tests/test_implementation_checks.py
--rw-rw-rw-   0        0        0     2773 2023-11-16 00:00:03.000000 pure-interface-8.0.1/tests/test_inheritance.py
--rw-rw-rw-   0        0        0     3784 2023-11-16 00:00:03.000000 pure-interface-8.0.1/tests/test_isinstance.py
--rw-rw-rw-   0        0        0     2346 2023-03-01 20:08:43.000000 pure-interface-8.0.1/tests/test_meta_classes.py
--rw-rw-rw-   0        0        0     2872 2023-11-16 00:00:03.000000 pure-interface-8.0.1/tests/test_module_funcs.py
--rw-rw-rw-   0        0        0     3360 2023-11-16 00:00:03.000000 pure-interface-8.0.1/tests/test_no_content_checks.py
--rw-rw-rw-   0        0        0     3385 2023-11-16 00:00:03.000000 pure-interface-8.0.1/tests/test_sub_interfaces.py
--rw-rw-rw-   0        0        0     2690 2023-11-16 00:00:03.000000 pure-interface-8.0.1/tests/test_tracker.py
+drwxrwxrwx   0        0        0        0 2024-04-28 22:38:51.891735 pure_interface-8.0.2/
+-rw-rw-rw-   0        0        0     1070 2021-09-21 22:43:47.000000 pure_interface-8.0.2/LICENSE
+-rw-rw-rw-   0        0        0    38685 2024-04-28 22:38:51.888734 pure_interface-8.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    36311 2024-03-05 03:42:39.000000 pure_interface-8.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-28 22:38:51.823206 pure_interface-8.0.2/pure_interface/
+-rw-rw-rw-   0        0        0      559 2024-04-28 22:38:20.000000 pure_interface-8.0.2/pure_interface/__init__.py
+-rw-rw-rw-   0        0        0     2858 2023-11-16 00:00:03.000000 pure_interface-8.0.2/pure_interface/_sub_interface.py
+-rw-rw-rw-   0        0        0     8071 2024-04-28 22:38:20.000000 pure_interface-8.0.2/pure_interface/adaption.py
+-rw-rw-rw-   0        0        0     8730 2023-11-16 00:00:03.000000 pure_interface-8.0.2/pure_interface/delegation.py
+-rw-rw-rw-   0        0        0      374 2023-07-21 02:33:09.000000 pure_interface-8.0.2/pure_interface/errors.py
+-rw-rw-rw-   0        0        0    35707 2024-04-28 22:38:20.000000 pure_interface-8.0.2/pure_interface/interface.py
+-rw-rw-rw-   0        0        0     8775 2023-11-16 00:00:03.000000 pure_interface-8.0.2/pure_interface/mypy_plugin.py
+-rw-rw-rw-   0        0        0        0 2023-05-11 00:43:53.000000 pure_interface-8.0.2/pure_interface/py.typed
+drwxrwxrwx   0        0        0        0 2024-04-28 22:38:51.886736 pure_interface-8.0.2/pure_interface.egg-info/
+-rw-rw-rw-   0        0        0    38685 2024-04-28 22:38:51.000000 pure_interface-8.0.2/pure_interface.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      949 2024-04-28 22:38:51.000000 pure_interface-8.0.2/pure_interface.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-28 22:38:51.000000 pure_interface-8.0.2/pure_interface.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-04-28 22:38:51.000000 pure_interface-8.0.2/pure_interface.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-28 22:38:51.000000 pure_interface-8.0.2/pure_interface.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1259 2023-11-16 00:00:03.000000 pure_interface-8.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-28 22:38:51.891735 pure_interface-8.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-28 22:38:51.884737 pure_interface-8.0.2/tests/
+-rw-rw-rw-   0        0        0     4281 2023-11-16 00:00:03.000000 pure_interface-8.0.2/tests/test_adapt_args_anno.py
+-rw-rw-rw-   0        0        0     2836 2023-11-16 00:00:03.000000 pure_interface-8.0.2/tests/test_adapt_args_no_anno.py
+-rw-rw-rw-   0        0        0    12674 2024-04-28 22:38:20.000000 pure_interface-8.0.2/tests/test_adaption.py
+-rw-rw-rw-   0        0        0     2883 2024-03-05 03:47:14.000000 pure_interface-8.0.2/tests/test_dataclass_support.py
+-rw-rw-rw-   0        0        0     9760 2023-11-16 00:00:03.000000 pure_interface-8.0.2/tests/test_delegate.py
+-rw-rw-rw-   0        0        0     5930 2023-07-21 02:33:09.000000 pure_interface-8.0.2/tests/test_func_sigs3.py
+-rw-rw-rw-   0        0        0     2729 2023-11-16 00:00:03.000000 pure_interface-8.0.2/tests/test_func_sigs_po.py
+-rw-rw-rw-   0        0        0    11706 2023-11-16 00:00:03.000000 pure_interface-8.0.2/tests/test_function_sigs.py
+-rw-rw-rw-   0        0        0     1061 2023-11-16 00:00:03.000000 pure_interface-8.0.2/tests/test_generic_support.py
+-rw-rw-rw-   0        0        0    16258 2023-11-16 00:00:03.000000 pure_interface-8.0.2/tests/test_implementation_checks.py
+-rw-rw-rw-   0        0        0     2773 2023-11-16 00:00:03.000000 pure_interface-8.0.2/tests/test_inheritance.py
+-rw-rw-rw-   0        0        0     3784 2023-11-16 00:00:03.000000 pure_interface-8.0.2/tests/test_isinstance.py
+-rw-rw-rw-   0        0        0     2346 2023-03-01 20:08:43.000000 pure_interface-8.0.2/tests/test_meta_classes.py
+-rw-rw-rw-   0        0        0     2872 2023-11-16 00:00:03.000000 pure_interface-8.0.2/tests/test_module_funcs.py
+-rw-rw-rw-   0        0        0     3360 2023-11-16 00:00:03.000000 pure_interface-8.0.2/tests/test_no_content_checks.py
+-rw-rw-rw-   0        0        0      896 2024-04-28 22:38:20.000000 pure_interface-8.0.2/tests/test_singledispatch.py
+-rw-rw-rw-   0        0        0     3385 2023-11-16 00:00:03.000000 pure_interface-8.0.2/tests/test_sub_interfaces.py
+-rw-rw-rw-   0        0        0     2690 2023-11-16 00:00:03.000000 pure_interface-8.0.2/tests/test_tracker.py
```

### Comparing `pure-interface-8.0.1/LICENSE` & `pure_interface-8.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/PKG-INFO` & `pure_interface-8.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-interface
-Version: 8.0.1
+Version: 8.0.2
 Summary: A Python interface library that disallows function body content on interfaces and supports adaption.
 Author-email: Tim Mitchell <tim.mitchell@seequent.com>
 License: MIT License
         
         Copyright (c) 2020 Seequent Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pure-interface-8.0.1/README.rst` & `pure_interface-8.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/pure_interface/__init__.py` & `pure_interface-8.0.2/pure_interface/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,8 +3,8 @@
 from .interface import type_is_interface, get_type_interfaces
 from .interface import get_interface_names, get_interface_method_names, get_interface_attribute_names
 from .interface import get_is_development, set_is_development, get_missing_method_warnings
 from ._sub_interface import sub_interface_of
 from .adaption import adapts, register_adapter, AdapterTracker, adapt_args
 from .delegation import Delegate
 
-__version__ = '8.0.1'
+__version__ = '8.0.2'
```

### Comparing `pure-interface-8.0.1/pure_interface/_sub_interface.py` & `pure_interface-8.0.2/pure_interface/_sub_interface.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/pure_interface/adaption.py` & `pure_interface-8.0.2/pure_interface/adaption.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import division, absolute_import, print_function
 
 import functools
 import inspect
 import types
-from typing import Any, Type, Callable, Optional
+from typing import Any, Type, TypeVar, Callable, Optional, Union
 import typing
 import warnings
 
 from .errors import InterfaceError, AdaptionError
 from .interface import AnInterface, Interface, InterfaceType, type_is_interface
 from .interface import get_type_interfaces, get_pi_attribute
 
@@ -42,24 +42,28 @@
             interface = to_interface
         register_adapter(cls, from_type, interface)
         return cls
 
     return decorator
 
 
+T = TypeVar('T')
+U = TypeVar('U')  # U can be a structural type so can't expect it to be a subclass of Interface
+
+
 def register_adapter(
-        adapter: Callable[[Type], Type[Interface]],
-        from_type: Type,
+        adapter: Union[Callable[[T], U], Type[U]],
+        from_type: Type[T],
         to_interface: Type[Interface]) -> None:
     """ Registers adapter to convert instances of from_type to objects that provide to_interface
     for the to_interface.adapt() method.
 
     :param adapter: callable that takes an instance of from_type and returns an object providing to_interface.
     :param from_type: a type to adapt from
-    :param to_interface: a (non-concrete) Interface subclass to adapt to.
+    :param to_interface: an Interface class to adapt to.
     """
     if not callable(adapter):
         raise AdaptionError('adapter must be callable')
     if not isinstance(from_type, type):
         raise AdaptionError('{} must be a type'.format(from_type))
     if not (isinstance(to_interface, type) and get_pi_attribute(to_interface, 'type_is_interface', False)):
         raise AdaptionError('{} is not an interface'.format(to_interface))
@@ -106,24 +110,24 @@
             adapters = self._adapters[interface] = self._factory()
         adapters[obj] = adapted
         return adapted
 
 
 def _interface_from_anno(annotation: Any) -> Optional[InterfaceType]:
     """ Typically the annotation is the interface,  but if a default value of None is given the annotation is
-    a typing.Union[interface, None] a.k.a. Optional[interface]. Lets be nice and support those too.
+    a Union[interface, None] a.k.a. Optional[interface]. Lets be nice and support those too.
     """
     try:
         if issubclass(annotation, Interface):
             return annotation
     except TypeError:
         pass
     if hasattr(annotation, '__origin__') and hasattr(annotation, '__args__'):
-        # could be a typing.Union
-        if annotation.__origin__ is not typing.Union:
+        # could be a Union
+        if annotation.__origin__ is not Union:
             return None
         for arg_type in annotation.__args__:
             if type_is_interface(arg_type):
                 return arg_type
 
     return None
```

### Comparing `pure-interface-8.0.1/pure_interface/delegation.py` & `pure_interface-8.0.2/pure_interface/delegation.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/pure_interface/interface.py` & `pure_interface-8.0.2/pure_interface/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 from __future__ import absolute_import, division, print_function
 
 import abc
 from abc import abstractclassmethod, abstractmethod, abstractstaticmethod
 import collections
 import dis
+import functools
 import inspect
 from inspect import Parameter, signature, Signature
 import sys
 import types
 from typing import Any, Callable, Dict, FrozenSet, Generic, Iterable, List, Optional, Set, Tuple, Type, TypeVar
 import warnings
 import weakref
@@ -378,61 +379,68 @@
             elif isinstance(value, property):
                 interface_attribute_names.append(name)
                 continue  # do not add to class namespace
         elif isinstance(value, staticmethod):
             func = value.__func__
             functions.append(func)
             interface_method_signatures[name] = signature(func)
-            value = abstractstaticmethod(func)
+            value = staticmethod(abstractmethod(func))
         elif isinstance(value, classmethod):
             func = value.__func__
             interface_method_signatures[name] = signature(func)
             functions.append(func)
-            value = abstractclassmethod(func)
+            value = classmethod(abstractmethod(func))
         elif isinstance(value, types.FunctionType):
             functions.append(value)
             interface_method_signatures[name] = signature(value)
             value = abstractmethod(value)
+        elif isinstance(value, functools.singledispatchmethod):
+            func = value.func
+            functions.append(func)
+            interface_method_signatures[name] = signature(func)
+            value = func  # ignore the singledispatchmethod decorator
         elif isinstance(value, property):
             interface_attribute_names.append(name)
             functions.extend([value.fget, value.fset, value.fdel])  # may contain Nones
             continue  # do not add to class namespace
         else:
             raise InterfaceError('Interface class attributes must have a value of None\n{}={}'.format(name, value))
         namespace[name] = value
     return namespace, functions, interface_method_signatures, interface_attribute_names
 
 
 def _ensure_annotations(names, namespace, base_interfaces):
     # annotations need to be kept in order for dataclass decorator
     # we only want dataclass annotations for attributes that don't already exist
-    annotations = {}
-    base_annos = {}
+    annotations: Dict[str, Any] = {}
+    base_annos: Dict[str, Any] = {}
     for base in reversed(base_interfaces):
-        base_annos.update(base.__annotations__)
+        base_annos.update(getattr(base, '__annotations__', {}))
     for name in names:
         if name not in annotations and name not in namespace:
             annotations[name] = base_annos.get(name, Any)
     annotations.update(namespace.get('__annotations__', {}))
     namespace['__annotations__'] = annotations
 
 
 def _check_method_signatures(attributes, clsname, interface_method_signatures):
     """ Scan attributes dict for interface method overrides and check the function signatures are consistent """
     for name, base_sig in interface_method_signatures.items():
         if name not in attributes:
             continue
         value = attributes[name]
-        if not isinstance(value, (staticmethod, classmethod, types.FunctionType)):
+        if not isinstance(value, (staticmethod, classmethod, types.FunctionType, functools.singledispatchmethod)):
             if _is_descriptor(value):
                 continue
             else:
                 raise InterfaceError('Interface method over-ridden with non-method')
         if isinstance(value, (staticmethod, classmethod)):
             func = value.__func__
+        elif isinstance(value, functools.singledispatchmethod):
+            func = value.func
         else:
             func = value
         func_sig = signature(func)
         if not _signatures_are_consistent(func_sig, base_sig):
             msg = '{module}.{clsname}.{name} arguments do not match base method'.format(
                 module=attributes['__module__'], clsname=clsname, name=name)
             raise InterfaceError(msg)
```

### Comparing `pure-interface-8.0.1/pure_interface/mypy_plugin.py` & `pure_interface-8.0.2/pure_interface/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/pure_interface.egg-info/PKG-INFO` & `pure_interface-8.0.2/pure_interface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pure-interface
-Version: 8.0.1
+Version: 8.0.2
 Summary: A Python interface library that disallows function body content on interfaces and supports adaption.
 Author-email: Tim Mitchell <tim.mitchell@seequent.com>
 License: MIT License
         
         Copyright (c) 2020 Seequent Ltd.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pure-interface-8.0.1/pure_interface.egg-info/SOURCES.txt` & `pure_interface-8.0.2/pure_interface.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -25,9 +25,10 @@
 tests/test_generic_support.py
 tests/test_implementation_checks.py
 tests/test_inheritance.py
 tests/test_isinstance.py
 tests/test_meta_classes.py
 tests/test_module_funcs.py
 tests/test_no_content_checks.py
+tests/test_singledispatch.py
 tests/test_sub_interfaces.py
 tests/test_tracker.py
```

### Comparing `pure-interface-8.0.1/pyproject.toml` & `pure_interface-8.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_adapt_args_anno.py` & `pure_interface-8.0.2/tests/test_adapt_args_anno.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_adapt_args_no_anno.py` & `pure_interface-8.0.2/tests/test_adapt_args_no_anno.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_adaption.py` & `pure_interface-8.0.2/tests/test_adaption.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,14 +333,15 @@
     def test_adapter_to_sub_interface_used(self):
         a_sleeper = Sleeper()
         speaker = ISpeaker.adapt_or_none(a_sleeper, interface_only=False)
         self.assertIsInstance(speaker, SleepSpeaker)
 
     def test_adapter_preference(self):
         """ adapt should prefer interface adapter over sub-interface adapter """
+
         class IA(Interface):
             foo = None
 
         class IB(IA, Interface):
             bar = None
 
         @pure_interface.adapts(int)
```

### Comparing `pure-interface-8.0.1/tests/test_dataclass_support.py` & `pure_interface-8.0.2/tests/test_dataclass_support.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_delegate.py` & `pure_interface-8.0.2/tests/test_delegate.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_func_sigs3.py` & `pure_interface-8.0.2/tests/test_func_sigs3.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_func_sigs_po.py` & `pure_interface-8.0.2/tests/test_func_sigs_po.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_function_sigs.py` & `pure_interface-8.0.2/tests/test_function_sigs.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_generic_support.py` & `pure_interface-8.0.2/tests/test_generic_support.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_implementation_checks.py` & `pure_interface-8.0.2/tests/test_implementation_checks.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_inheritance.py` & `pure_interface-8.0.2/tests/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_isinstance.py` & `pure_interface-8.0.2/tests/test_isinstance.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_meta_classes.py` & `pure_interface-8.0.2/tests/test_meta_classes.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_module_funcs.py` & `pure_interface-8.0.2/tests/test_module_funcs.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_no_content_checks.py` & `pure_interface-8.0.2/tests/test_no_content_checks.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_sub_interfaces.py` & `pure_interface-8.0.2/tests/test_sub_interfaces.py`

 * *Files identical despite different names*

### Comparing `pure-interface-8.0.1/tests/test_tracker.py` & `pure_interface-8.0.2/tests/test_tracker.py`

 * *Files identical despite different names*

