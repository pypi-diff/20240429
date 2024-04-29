# Comparing `tmp/tracking_decorator-0.0.3.tar.gz` & `tmp/tracking_decorator-0.0.4.tar.gz`

## Comparing `tracking_decorator-0.0.3.tar` & `tracking_decorator-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/src/tracking_decorator/__init__.py
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/src/tracking_decorator/track_changes.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/src/tracking_decorator/trash_collections.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/tests/test_track_changes.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/LICENSE
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/README.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 tracking_decorator-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tracking_decorator-0.0.4/src/tracking_decorator/__init__.py
+-rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 tracking_decorator-0.0.4/src/tracking_decorator/track_changes.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 tracking_decorator-0.0.4/src/tracking_decorator/trash_collections.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 tracking_decorator-0.0.4/tests/test_time_track_changes.py
+-rw-r--r--   0        0        0     3051 2020-02-02 00:00:00.000000 tracking_decorator-0.0.4/tests/test_track_changes.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 tracking_decorator-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tracking_decorator-0.0.4/LICENSE
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 tracking_decorator-0.0.4/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 tracking_decorator-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 tracking_decorator-0.0.4/PKG-INFO
```

### Comparing `tracking_decorator-0.0.3/src/tracking_decorator/track_changes.py` & `tracking_decorator-0.0.4/src/tracking_decorator/track_changes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,80 @@
 from tracking_decorator.trash_collections import trash_collection
 
 def track_changes(*attributes):
     def class_decorator(cls):
         original_init = cls.__init__
 
+        def remove_specification(attribute_name):
+            if attribute_name.endswith('_r') or attribute_name.endswith('_d'):
+                return attribute_name[:-2]
+            return attribute_name
+
         def make_getter(attribute_name):
             storage_name = '_' + attribute_name
             def getter(self):
                 return getattr(self, storage_name)
             return getter
 
         def make_setter(attribute_name, attribute_to_track):
             storage_name = '_' + attribute_name
+
             def setter(self, value):
+                self.tracked_attributes.add(attribute_to_track)
+                setattr(self, storage_name, value)
+                    
+            return setter
+        
+        def make_only_change_setter(attribute_name, attribute_to_track):
+            storage_name = '_' + attribute_name
 
+            def setter(self, value):
                 if getattr(self, storage_name) != value:
                     self.tracked_attributes.add(attribute_to_track)
+                    setattr(self, storage_name, value)
+                    
+            return setter
+        
+        def make_collection_removal_setter(attribute_name, attribute_to_track):
+            storage_name = '_' + attribute_name
+
+            def setter(self, value):
+                self.tracked_attributes.add(attribute_to_track)
+                TrashCollection = trash_collection(value)
+                setattr(self, storage_name, TrashCollection)
 
-                    if isinstance(value, (list, set, dict)):
-                        TrashCollection = trash_collection(value)
-                        setattr(self, storage_name, TrashCollection)
-                    else:
-                        setattr(self, storage_name, value)
             return setter
 
         for attribute in attributes:
             if isinstance(attribute, tuple):
                 attribute, attribute_to_track = attribute
-                getter_func = make_getter(attribute)
-                setter_func = make_setter(attribute, attribute_to_track)
             else:
-                getter_func = make_getter(attribute)
-                setter_func = make_setter(attribute, attribute)
+                attribute, attribute_to_track = attribute, remove_specification(attribute)
+
+            if attribute.endswith('_r'):
+                attribute = attribute[:-2]
+                setter_func = make_collection_removal_setter(attribute, attribute_to_track)
+            elif attribute.endswith('_d'):
+                attribute = attribute[:-2]
+                setter_func = make_only_change_setter(attribute, attribute_to_track)
+            else:
+                setter_func = make_setter(attribute, attribute_to_track)
+
+            getter_func = make_getter(attribute)
+
             setattr(cls, attribute, property(getter_func, setter_func))
 
         # Modify the __init__ to initialize properties
         def new_init(self, *args, **kwargs):
             self.tracked_attributes = set()
 
             for attribute_name in attributes:
                 if isinstance(attribute_name, tuple):
                     attribute_name = attribute_name[0]
+                attribute_name = remove_specification(attribute_name)
                 storage_name = '_' + attribute_name
                 setattr(self, storage_name, None)
 
             original_init(self, *args, **kwargs)
             self.clear()
 
         def clear(self):
```

### Comparing `tracking_decorator-0.0.3/src/tracking_decorator/trash_collections.py` & `tracking_decorator-0.0.4/src/tracking_decorator/trash_collections.py`

 * *Files identical despite different names*

### Comparing `tracking_decorator-0.0.3/tests/test_track_changes.py` & `tracking_decorator-0.0.4/tests/test_track_changes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# import pytest
 from tracking_decorator.track_changes import track_changes
-from tracking_decorator.trash_collections import TrashList
- 
+
 class ReferenceClass:
     def __init__(self):
         self.var = 0
 
-@track_changes("base_variable", "reference")
+@track_changes("base_variable_d", "reference")
 class BaseClass():
     def __init__(self, reference: ReferenceClass):
         self.base_variable = 0
         self.reference = reference
         self.untracked = "hello"
 
 @track_changes("child_variable")
@@ -21,32 +19,36 @@
     
 @track_changes(("update_tuple_variable", "tracked_tuple_variable"))
 class TupleClass:
     def __init__(self):
         self.tracked_tuple_variable = "based"
 
 
-@track_changes("list_type", "set_type", "dict_type")
+@track_changes("list_type_r", "set_type_r", "dict_type_r")
 class CollectionClass:
     def __init__(self):
         self.list_type = [20, 40, 60, 80, 100]
         self.set_type = {1, 3, 5}
         self.dict_type = {"a": "b", "c": "d", "e": "f"}
     
-
 def test_tracks_correctly():
     ref = ReferenceClass()
     base = BaseClass(ref)
 
     base.base_variable = 5
     base.reference.var = 5 # doesn't track whether value changes, only pointer
     base.untracked = "hi" #doesn't track untracked variables
-
     assert base.tracked_attributes == {"base_variable"}
 
+    base.clear()
+
+    base.base_variable = 5 # _d means only track if value changes
+    base.reference = base.reference # will track even if value doesn't change
+    assert base.tracked_attributes == {'reference'}
+
 def test_tracks_tuples_correctly():
     tup = TupleClass()
 
     tup.update_tuple_variable = "hi" # adds tracked attribute
     assert tup.tracked_attributes == {"tracked_tuple_variable"}
 
     tup.clear()
@@ -88,8 +90,7 @@
     assert coll.set_type.trash == {1, 5}
     assert coll.dict_type.trash == {"a": "b", "c": "d"}
 
     # doesn't affect the original collection
     assert coll.list_type == [40, 100]
     assert coll.set_type == {3}
     assert coll.dict_type == {"e": "f"}
-
```

### Comparing `tracking_decorator-0.0.3/.gitignore` & `tracking_decorator-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `tracking_decorator-0.0.3/LICENSE` & `tracking_decorator-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tracking_decorator-0.0.3/README.md` & `tracking_decorator-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tracking_decorator-0.0.3/pyproject.toml` & `tracking_decorator-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 testpaths = ["tests"]
 
 [project]
 name = "tracking_decorator"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Ian Lavine", email="ian.lavine@mail.utoronto.ca" },
 ]
 description = "A small decorator for tracking changed attributes in a class"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tracking_decorator-0.0.3/PKG-INFO` & `tracking_decorator-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tracking_decorator
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small decorator for tracking changed attributes in a class
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Ian Lavine <ian.lavine@mail.utoronto.ca>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

