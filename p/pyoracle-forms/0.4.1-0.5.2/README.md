# Comparing `tmp/pyoracle_forms-0.4.1.tar.gz` & `tmp/pyoracle_forms-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoracle_forms-0.4.1.tar", last modified: Sun May 22 16:50:12 2022, max compression
+gzip compressed data, was "pyoracle_forms-0.5.2.tar", last modified: Mon Apr 29 21:52:16 2024, max compression
```

## Comparing `pyoracle_forms-0.4.1.tar` & `pyoracle_forms-0.5.2.tar`

### file list

```diff
@@ -1,26 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-22 16:50:12.543638 pyoracle_forms-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1070 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       45 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3388 2022-05-22 16:50:12.543638 pyoracle_forms-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2825 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-22 16:50:12.543638 pyoracle_forms-0.4.1/pyoracle_forms/
--rw-r--r--   0 runner    (1001) docker     (116)     6094 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/pyoracle_forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11698 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/pyoracle_forms/constants.py
--rw-r--r--   0 runner    (1001) docker     (116)     8262 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/pyoracle_forms/context.py
--rw-r--r--   0 runner    (1001) docker     (116)     1726 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/pyoracle_forms/error_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-22 16:50:12.543638 pyoracle_forms-0.4.1/pyoracle_forms/forms_api/
--rw-r--r--   0 runner    (1001) docker     (116)   258123 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/pyoracle_forms/forms_api/parsed_10g.json
--rw-r--r--   0 runner    (1001) docker     (116)   275663 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/pyoracle_forms/forms_api/parsed_12c.json
--rw-r--r--   0 runner    (1001) docker     (116)   255388 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/pyoracle_forms/forms_api/parsed_6i.json
--rw-r--r--   0 runner    (1001) docker     (116)     1173 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/pyoracle_forms/forms_api.py
--rw-r--r--   0 runner    (1001) docker     (116)    89361 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/pyoracle_forms/forms_objects.py
--rw-r--r--   0 runner    (1001) docker     (116)     4268 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/pyoracle_forms/generic_object.py
--rw-r--r--   0 runner    (1001) docker     (116)     7171 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/pyoracle_forms/misc.py
--rw-r--r--   0 runner    (1001) docker     (116)    13808 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/pyoracle_forms/property_types.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-05-22 16:50:12.543638 pyoracle_forms-0.4.1/pyoracle_forms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3388 2022-05-22 16:50:12.000000 pyoracle_forms-0.4.1/pyoracle_forms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      576 2022-05-22 16:50:12.000000 pyoracle_forms-0.4.1/pyoracle_forms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-05-22 16:50:12.000000 pyoracle_forms-0.4.1/pyoracle_forms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       15 2022-05-22 16:50:12.000000 pyoracle_forms-0.4.1/pyoracle_forms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-05-22 16:50:12.543638 pyoracle_forms-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      876 2022-05-22 16:49:58.000000 pyoracle_forms-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:52:16.136255 pyoracle_forms-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-29 21:52:16.136255 pyoracle_forms-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:52:16.132255 pyoracle_forms-0.5.2/pyoracle_forms/
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/pyoracle_forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/pyoracle_forms/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9483 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/pyoracle_forms/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/pyoracle_forms/error_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:52:16.132255 pyoracle_forms-0.5.2/pyoracle_forms/forms_api/
+-rw-r--r--   0 runner    (1001) docker     (127)   258123 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/pyoracle_forms/forms_api/parsed_10g.json
+-rw-r--r--   0 runner    (1001) docker     (127)   275663 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/pyoracle_forms/forms_api/parsed_12c.json
+-rw-r--r--   0 runner    (1001) docker     (127)   255388 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/pyoracle_forms/forms_api/parsed_6i.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/pyoracle_forms/forms_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91388 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/pyoracle_forms/forms_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/pyoracle_forms/generic_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/pyoracle_forms/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/pyoracle_forms/property_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:52:16.136255 pyoracle_forms-0.5.2/pyoracle_forms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-29 21:52:16.000000 pyoracle_forms-0.5.2/pyoracle_forms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-29 21:52:16.000000 pyoracle_forms-0.5.2/pyoracle_forms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 21:52:16.000000 pyoracle_forms-0.5.2/pyoracle_forms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-29 21:52:16.000000 pyoracle_forms-0.5.2/pyoracle_forms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 21:52:16.136255 pyoracle_forms-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 21:52:16.136255 pyoracle_forms-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/tests/test_bruteforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/tests/test_canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/tests/test_context_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/tests/test_dlls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/tests/test_generic_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/tests/test_getters_setters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/tests/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/tests/test_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/tests/test_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/tests/test_object_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-29 21:52:12.000000 pyoracle_forms-0.5.2/tests/test_subclass.py
```

### Comparing `pyoracle_forms-0.4.1/LICENSE` & `pyoracle_forms-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoracle_forms-0.4.1/PKG-INFO` & `pyoracle_forms-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoracle_forms
-Version: 0.4.1
+Version: 0.5.2
 Summary: Python wrapper of the Oracle Forms API
 Home-page: https://github.com/LatvianPython/pyoracle_forms
 Author: LatvianPython
 Author-email: kalvans.rolands@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyoracle_forms-0.4.1/README.rst` & `pyoracle_forms-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `pyoracle_forms-0.4.1/pyoracle_forms/__init__.py` & `pyoracle_forms-0.5.2/pyoracle_forms/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 from .forms_objects import Library
 from .forms_objects import LibraryProgramUnit
 from .forms_objects import LOV
 from .forms_objects import LOVColumnMap
 from .forms_objects import Menu
 from .forms_objects import MenuItem
 from .forms_objects import Module
+from .forms_objects import ObjectLibrary
+from .forms_objects import ObjectLibraryTab
 from .forms_objects import ObjectChild
 from .forms_objects import ObjectGroup
 from .forms_objects import Point
 from .forms_objects import ProgramUnit
 from .forms_objects import PropertyClass
 from .forms_objects import RadioButton
 from .forms_objects import RecordGroup
@@ -141,15 +143,16 @@
 from .constants import GraphicFontSpacing
 from .constants import RelationType
 from .constants import DataLengthSemantics
 from .constants import EventType
 from .constants import Scope
 from .constants import ViewMode
 
-__version__ = "0.4.1"
+
+__version__ = "0.5.2"
 
 
 def initialize_context(version: str = "12c", encoding: str = "utf-8") -> None:
     context.init(version=version, encoding=encoding)
 
     api_objects = read_api_objects(version=version)
```

### Comparing `pyoracle_forms-0.4.1/pyoracle_forms/constants.py` & `pyoracle_forms-0.5.2/pyoracle_forms/constants.py`

 * *Files identical despite different names*

### Comparing `pyoracle_forms-0.4.1/pyoracle_forms/context.py` & `pyoracle_forms-0.5.2/pyoracle_forms/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from .error_handling import raise_for_code
 from .forms_api import dlls
 
 if TYPE_CHECKING:  # pragma: no cover
     from ctypes import _FuncPointer
     from .generic_object import BaseObject
-    from .forms_objects import Module
+    from .forms_objects import Module, ObjectLibrary, ObjectLibraryTab
 
 T = TypeVar("T")
 
 Setter = Callable[["BaseObject", int, T], None]
 Getter = Callable[["BaseObject", int], T]
 CTypes = Union[Type[c_void_p], Type[c_bool], Type[c_int], Type["String"]]
 
@@ -175,14 +175,20 @@
 
 def load_module(form_path: str) -> c_void_p:
     return handled_api_function(
         "d2ffmdld_Load", (c_void_p, c_char_p, c_bool), return_value_index=0
     )(c_void_p(), form_path.encode(context.encoding), False)
 
 
+def load_object_library(object_library_path: str) -> c_void_p:
+    return handled_api_function(
+        "d2folbld_Load", (c_void_p, c_char_p, c_bool), return_value_index=0
+    )(c_void_p(), object_library_path.encode(context.encoding), False)
+
+
 def create_module(name: str) -> c_void_p:
     return handled_api_function(
         "d2ffmdcr_Create", (c_void_p, c_char_p), return_value_index=0
     )(c_void_p(), name.encode(context.encoding))
 
 
 def save_module(module: Module, path: str) -> None:
@@ -257,7 +263,34 @@
     handled_api_function("d2fobsc_SubClass", (c_void_p, c_void_p, c_bool))(
         to_subclass, parent, keep_path
     )
 
 
 def remove_subclass(to_un_subclass: BaseObject) -> None:
     handled_api_function("d2fobus_UnSubClass", (c_void_p,))(to_un_subclass)
+
+
+def find_library_object_by_position(
+    object_library: ObjectLibrary, position: int
+) -> c_void_p:
+    return handled_api_function(
+        "d2folbf2_Findobjbypos", (c_void_p, c_int, c_void_p), return_value_index=2
+    )(
+        object_library, position, c_void_p()
+    )  # pragma: nocover
+
+
+def find_library_tab_object_by_position(
+    object_library: ObjectLibraryTab, position: int
+) -> c_void_p:
+    return handled_api_function(
+        "d2foltf2_Findobjbypos", (c_void_p, c_int, c_void_p), return_value_index=2
+    )(object_library, position, c_void_p())
+
+
+def duplicate(new_owner: BaseObject, source: BaseObject, new_name: str) -> c_void_p:
+    # d2fobdu_Duplicate(ctx, new_owner, pd2fob_src, & pd2fob_dst, new_name)
+    return handled_api_function(
+        "d2fobdu_Duplicate",
+        (c_void_p, c_void_p, c_void_p, c_char_p),
+        return_value_index=2,
+    )(new_owner, source, c_void_p(), new_name.encode(context.encoding))
```

### Comparing `pyoracle_forms-0.4.1/pyoracle_forms/error_handling.py` & `pyoracle_forms-0.5.2/pyoracle_forms/error_handling.py`

 * *Files identical despite different names*

### Comparing `pyoracle_forms-0.4.1/pyoracle_forms/forms_api/parsed_10g.json` & `pyoracle_forms-0.5.2/pyoracle_forms/forms_api/parsed_10g.json`

 * *Files identical despite different names*

### Comparing `pyoracle_forms-0.4.1/pyoracle_forms/forms_api/parsed_12c.json` & `pyoracle_forms-0.5.2/pyoracle_forms/forms_api/parsed_12c.json`

 * *Files identical despite different names*

### Comparing `pyoracle_forms-0.4.1/pyoracle_forms/forms_api/parsed_6i.json` & `pyoracle_forms-0.5.2/pyoracle_forms/forms_api/parsed_6i.json`

 * *Files identical despite different names*

### Comparing `pyoracle_forms-0.4.1/pyoracle_forms/forms_api.py` & `pyoracle_forms-0.5.2/pyoracle_forms/forms_api.py`

 * *Files identical despite different names*

### Comparing `pyoracle_forms-0.4.1/pyoracle_forms/forms_objects.py` & `pyoracle_forms-0.5.2/pyoracle_forms/forms_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 from types import TracebackType
 from typing import Optional, Type, Union, List, TypeVar
 
 from .context import create_module
 from .context import load_module
 from .context import save_module
 from .context import load_library
+from .context import load_object_library
 from .generic_object import GenericObject, BaseObject, FormsObjects
 from .misc import (
     forms_object,
     Text,
     Number,
     Object,
     Bool,
     Subobjects,
     Unknown,
     Constant,
+    ObjectLibraryTabObjects,
 )
 from .constants import *
 
 
 # satisfy both MyPy and PyCharm IDE autocomplete
 U = TypeVar("U")
 ObjectList = Union[List[U], Subobjects[U]]
+ObjectLibraryTabObjectList = Union[List[U], ObjectLibraryTabObjects]
 Obj = Union[U, Object[U]]
 
 
 @forms_object
 class Module(BaseObject):
     object_type = FormsObjects.module
 
@@ -157,14 +160,71 @@
 
     @classmethod
     def load(cls, path: str) -> Library:
         return cls(load_library(path), path=path)
 
 
 @forms_object
+class ObjectLibrary(GenericObject):
+    # auto-generated
+    object_type = FormsObjects.object_library
+
+    object_library_tabs: ObjectList[ObjectLibraryTab] = Subobjects("OBJ_LIB_TAB")
+
+    case_info = Unknown("CLIENT_INFO")
+    comments = Text("COMMENT")
+    name = Text("NAME")
+    next_object: Object[ObjectLibrary] = Object("NEXT")
+    previous_object: Object[ObjectLibrary] = Object("PREVIOUS")
+    count_of_objects = Number("OBJ_COUNT")
+    persistent_client_info_storage = Unknown("PERSIST_CLIENT_INFO")
+    persistent_client_info_storage_length = Number("PERSIST_CLT_INF_LEN")
+
+    def __init__(self, module: Union[c_void_p, BaseObject], path: Optional[str] = None):
+        super().__init__(module)
+        self.path = path
+
+    def __enter__(self) -> ObjectLibrary:
+        return self
+
+    def __exit__(
+        self,
+        exc_type: Optional[Type[BaseException]],
+        exc_val: Optional[BaseException],
+        exc_tb: Optional[TracebackType],
+    ) -> None:
+        self.destroy()
+
+    @classmethod
+    def load(cls, path: str) -> ObjectLibrary:
+        return cls(load_object_library(path), path=path)
+
+
+@forms_object
+class ObjectLibraryTab(GenericObject):
+    # auto-generated
+    object_type = FormsObjects.object_library_tab
+
+    # object_library_tabs: ObjectList[ObjectLibraryTab] = Subobjects("OBJ_LIB_TAB")
+    objects: ObjectLibraryTabObjectList[
+        ObjectLibraryTabObjects
+    ] = ObjectLibraryTabObjects()
+
+    case_info = Unknown("CLIENT_INFO")
+    comments = Text("COMMENT")
+    label = Text("LABEL")
+    name = Text("NAME")
+    next_object: Object[ObjectLibraryTab] = Object("NEXT")
+    previous_object: Object[ObjectLibraryTab] = Object("PREVIOUS")
+    count_of_objects = Number("OBJ_COUNT")
+    persistent_client_info_storage = Unknown("PERSIST_CLIENT_INFO")
+    persistent_client_info_storage_length = Number("PERSIST_CLT_INF_LEN")
+
+
+@forms_object
 class LibraryProgramUnit(GenericObject):
     # auto-generated
     object_type = FormsObjects.library_program_unit
 
     name = Text("NAME")
     next_object: Obj[LibraryProgramUnit] = Object("NEXT")
     program_unit_text = Text("PGU_TXT")
```

### Comparing `pyoracle_forms-0.4.1/pyoracle_forms/generic_object.py` & `pyoracle_forms-0.5.2/pyoracle_forms/generic_object.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .context import destroy
 from .context import has_property
 from .context import remove_subclass
 from .context import set_subclass
 from .context import move
 from .context import query_type
 from .context import is_subclassed
+from .context import duplicate
 
 from .property_types import Properties
 
 
 class FormsObjects(enum.Enum):
     canvas = "D2FFO_CANVAS"
     alert = "D2FFO_ALERT"
@@ -44,14 +45,16 @@
     library_program_unit = "D2FFO_LIB_PROG_UNIT"
     lov = "D2FFO_LOV"
     lov_column_map = "D2FFO_LV_COLMAP"
     menu = "D2FFO_MENU"
     menu_item = "D2FFO_MENU_ITEM"
     object_group = "D2FFO_OBJ_GROUP"
     object_child = "D2FFO_OBG_CHILD"
+    object_library = "D2FFO_OBJ_LIB"
+    object_library_tab = "D2FFO_OBJ_LIB_TAB"
     record_group = "D2FFO_REC_GROUP"
     record_group_colspec = "D2FFO_RG_COLSPEC"
     report = "D2FFO_REPORT"
     column_value = "D2FFO_COLUMN_VALUE"
 
 
 class ValueTypes(enum.IntEnum):
@@ -93,16 +96,16 @@
 
     def move(self, next_object: GenericObject) -> None:
         move(self, next_object)
 
     def query_type(self) -> int:
         return query_type(self)
 
-    def duplicate(self, new_owner: GenericObject, new_name: str) -> NoReturn:
-        raise NotImplementedError()
+    def duplicate(self, new_owner: GenericObject, new_name: str) -> BaseObject:
+        return self.__class__(duplicate(new_owner, self, new_name))
 
     def replicate(self, new_owner: GenericObject, new_name: str) -> NoReturn:
         raise NotImplementedError()
 
     def find_object(self, name: str, object_type: FormsObjects) -> NoReturn:
         raise NotImplementedError()
```

### Comparing `pyoracle_forms-0.4.1/pyoracle_forms/misc.py` & `pyoracle_forms-0.5.2/pyoracle_forms/misc.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,33 +12,35 @@
     TypeVar,
     Generic,
     Any,
     TYPE_CHECKING,
     Optional,
 )
 
-from .context import context, property_type
+from .context import context, property_type, find_library_tab_object_by_position
 from .context import get_boolean
 from .context import get_number
 from .context import get_object
 from .context import get_text
 from .context import object_name
 from .context import property_constant_name
 from .context import property_constant_number
 from .context import property_name
 from .context import query_type
 from .context import set_boolean
 from .context import set_number
 from .context import set_object
 from .context import set_text
+from .context import find_library_object_by_position
 from .generic_object import BaseObject, ValueTypes, GenericObject
 from .property_types import Properties
 from .constants import Justification
 
 if TYPE_CHECKING:  # pragma: no cover
+    from . import ObjectLibraryTab
     from . import Module
     from . import Library
 
 objects = Union[Type["Module"], Type["Library"], Type[GenericObject]]
 registered_objects: Dict[str, objects] = {}
 
 
@@ -204,14 +206,35 @@
         subobjects = list(gen_subobjects())
         return subobjects
 
     def __set__(self, instance: BaseObject, value: List[BaseObject]) -> NoReturn:
         raise AttributeError("can't set attribute")
 
 
+class ObjectLibraryTabObjects:
+    def __get__(
+        self, instance: ObjectLibraryTab, owner: Type[ObjectLibraryTab]
+    ) -> List[BaseObject]:
+        def gen_subobjects() -> Iterable[BaseObject]:
+            for i in range(1, instance.count_of_objects + 1):
+                first_child = find_library_tab_object_by_position(instance, i)
+
+                klass = get_object_constructor(BaseObject(first_child))
+
+                child = klass(first_child)
+
+                yield child
+
+        subobjects = list(gen_subobjects())
+        return subobjects
+
+    def __set__(self, instance: BaseObject, value: List[BaseObject]) -> NoReturn:
+        raise AttributeError("can't set attribute")  # pragma: nocover
+
+
 def add_properties(klass: Type[BaseObject], api_objects: Dict) -> Type[BaseObject]:  # type: ignore
     try:
         obj_type = api_objects[klass.object_type.value]
     except KeyError:
         # todo: clean up dirty hack
         #  mostly for column_value, which seems to be not documented by orcl anyway
         #  other objects also do not have their own specific entries
```

### Comparing `pyoracle_forms-0.4.1/pyoracle_forms/property_types.py` & `pyoracle_forms-0.5.2/pyoracle_forms/property_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,14 +341,15 @@
     database_data_block = 377
     query_data_source_type = 378
     query_all_records = 379
     dml_data_target_type = 380
     dml_array_size = 381
     tooltip_visual_attribute_group = 382
     tooltip_va_object = 383
+    object_library_tab = 418
     insert_procedure_name = 419
     update_procedure_name = 422
     delete_procedure_name = 425
     lock_procedure_name = 428
     single_record = 431
     trigger_internal_type = 432
     length = 433
@@ -408,14 +409,15 @@
     graphic_object_font_style = 495
     graphic_object_text = 496
     parent_objects_module = 497
     parent_objects_module_type = 498
     parent_object_name = 499
     parent_objects_file_name = 500
     parent_objects_file_path = 501
+    count_of_objects = 502
     count_of_roles = 503
     program_unit_type = 504
     submenu_name = 505
     submenu_object = 506
     menu_item_code = 507
     query_column_object = 508
     query_argument_object = 509
```

### Comparing `pyoracle_forms-0.4.1/pyoracle_forms.egg-info/PKG-INFO` & `pyoracle_forms-0.5.2/pyoracle_forms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pyoracle-forms
-Version: 0.4.1
+Name: pyoracle_forms
+Version: 0.5.2
 Summary: Python wrapper of the Oracle Forms API
 Home-page: https://github.com/LatvianPython/pyoracle_forms
 Author: LatvianPython
 Author-email: kalvans.rolands@gmail.com
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyoracle_forms-0.4.1/setup.py` & `pyoracle_forms-0.5.2/setup.py`

 * *Files identical despite different names*

