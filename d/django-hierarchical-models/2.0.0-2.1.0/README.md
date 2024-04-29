# Comparing `tmp/django_hierarchical_models-2.0.0.tar.gz` & `tmp/django_hierarchical_models-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hierarchical_models-2.0.0.tar", max compression
+gzip compressed data, was "django_hierarchical_models-2.1.0.tar", max compression
```

## Comparing `django_hierarchical_models-2.0.0.tar` & `django_hierarchical_models-2.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/LICENSE
--rw-r--r--   0        0        0     4920 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/README.md
--rw-r--r--   0        0        0       22 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/django_hierarchical_models/__init__.py
--rw-r--r--   0        0        0      285 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/django_hierarchical_models/models/__init__.py
--rw-r--r--   0        0        0      597 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/django_hierarchical_models/models/exceptions.py
--rw-r--r--   0        0        0     6132 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/django_hierarchical_models/models/hierarchical_model.py
--rw-r--r--   0        0        0      900 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/django_hierarchical_models/models/node.py
--rw-r--r--   0        0        0     1116 2024-04-28 18:53:27.451842 django_hierarchical_models-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     5712 1970-01-01 00:00:00.000000 django_hierarchical_models-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-29 00:42:51.769617 django_hierarchical_models-2.1.0/LICENSE
+-rw-r--r--   0        0        0     5356 2024-04-29 00:42:51.769617 django_hierarchical_models-2.1.0/README.md
+-rw-r--r--   0        0        0       22 2024-04-29 00:42:51.769617 django_hierarchical_models-2.1.0/django_hierarchical_models/__init__.py
+-rw-r--r--   0        0        0      285 2024-04-29 00:42:51.769617 django_hierarchical_models-2.1.0/django_hierarchical_models/models/__init__.py
+-rw-r--r--   0        0        0      597 2024-04-29 00:42:51.769617 django_hierarchical_models-2.1.0/django_hierarchical_models/models/exceptions.py
+-rw-r--r--   0        0        0     5441 2024-04-29 00:42:51.769617 django_hierarchical_models-2.1.0/django_hierarchical_models/models/hierarchical_model.py
+-rw-r--r--   0        0        0      900 2024-04-29 00:42:51.773617 django_hierarchical_models-2.1.0/django_hierarchical_models/models/node.py
+-rw-r--r--   0        0        0     1116 2024-04-29 00:42:51.773617 django_hierarchical_models-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 1970-01-01 00:00:00.000000 django_hierarchical_models-2.1.0/PKG-INFO
```

### Comparing `django_hierarchical_models-2.0.0/LICENSE` & `django_hierarchical_models-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hierarchical_models-2.0.0/README.md` & `django_hierarchical_models-2.1.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -22,46 +22,57 @@
 
 class MyModel(HierarchicalModel):
     name = models.CharField(max_length=100)
 
 ...
 
 child = MyModel.objects.create(name="Betty")
-child.parent()  # None
+child.parent  # None
 
 parent = MyModel.objects.create(name="Simon")
+# checks for pesky cycles
 child.set_parent(parent)
-child.parent()  # <MyModel: "Simon">
+# alternative
+# child.parent = parent
+child.parent  # <MyModel: "Simon">
 
 child.root()  # <MyModel: "Simon">
 parent.root()  # <MyModel: "Simon">
 
 parent.direct_children()  # [<MyModel: "Betty">]
 
 child.is_child_of(parent)  # True
 parent.is_child_of(child)  # False
 ```
 
+## parent = vs .set_parent()
+
+`parent` is a `ForeignKeyField` which may be directly accessed or set. The
+`.set_parent()` method checks to see if the operation would create a cycle, which can
+be bad for some of the other instance methods. The `.set_parent()` method is slower
+because it must determine if a cycle would be formed. `.set_parent()` makes a call to
+`.save(update_fields=("parent",))`, so it is not necessary to call `.save()` after
+updating the parent this way.
+
 ## Refreshing from database
 
-External changes to an instance's parent are not automatically reflected in the
-instance. This leads to the following behavior:
+The following is expected behavior:
 
 ```python
 instance_1 = MyModel.objects.create(name="Betty")
 instance_2 = MyModel.objects.create(parent=instance_1, name="Simon")
-insstance_2.parent()  # <MyModel: "Betty">
+instance_2.parent  # <MyModel: "Betty">
 
 instance_1.delete()
 
-instance_2.parent()  # <MyModel: "Betty">
+instance_2.parent  # <MyModel: "Betty">
 
 instance_2.refresh_from_db()
 
-instance_2.parent()  # None
+instance_2.parent  # None
 ```
 
 ```python
 instance_1 = MyModel.objects.create(name="Betty")
 instance_2 = MyModel.objects.create(parent=instance_1, name="Simon")
 instance_3 = MyModel.objects.create(parent=instance_2, name="Finn")
 instance_3_copy = MyModel.objects.get(pk=instance_3.pk)
@@ -82,16 +93,16 @@
 
 instance_1.root()  # <MyModel: "Betty">
 instance_2.root()  # <MyModel: "Simon">
 instance_3.root()  # <MyModel: "Simon">
 instance_3_copy.root()  # <MyModel: "Simon">
 ```
 
-Moral of the story, if your instance's parent might have been edited/deleted,
-you will want to refresh your instance for that change to be reflected.  
+Moral of the story, if your instance's parent might have been edited/deleted, you will
+want to refresh your instance for that change to be reflected.  
 
 ## Benchmarks
 
 The following benchmarks demonstrate that the query performance of the model stays the
 same from 10,000 to 1,000,000 models. These tests were done with Postgres. The results
 are in the form `total time (s) / per instance (ms)`. Eventually the query performance
 of this model should scale down with the total number of instances in the database,
```

### Comparing `django_hierarchical_models-2.0.0/django_hierarchical_models/models/exceptions.py` & `django_hierarchical_models-2.1.0/django_hierarchical_models/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_hierarchical_models-2.0.0/django_hierarchical_models/models/hierarchical_model.py` & `django_hierarchical_models-2.1.0/django_hierarchical_models/models/hierarchical_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,91 +9,69 @@
 from django_hierarchical_models.models.exceptions import CycleException
 from django_hierarchical_models.models.node import Node
 
 T = TypeVar("T", bound="HierarchicalModel")
 
 
 class HierarchicalModel(models.Model):
-    """An abstract Django model supporting hierarchical data."""
+    """An abstract Django model supporting hierarchical data.
 
-    _parent = models.ForeignKey(
-        "self", on_delete=models.SET_NULL, blank=True, null=True
-    )
+    Attributes:
+        parent: ForeignKey to self.
+    """
 
-    def __init__(self, *args, **kwargs):
-        """Initialize with an optional "parent" kwarg.
-
-        Keyword Args:
-            parent: Parent model of this instance.
-        """
-        if len(args) == 0 and "parent" in kwargs:
-            kwargs["_parent"] = kwargs.pop("parent")
-        super().__init__(*args, **kwargs)
+    parent = models.ForeignKey("self", on_delete=models.SET_NULL, blank=True, null=True)
 
     class Meta:
         abstract = True
 
-    def parent(self: T) -> T | None:
-        """The parent of this instance.
-
-        Returns:
-            The instance of the parent, or None if this instance has no parent.
-        """
-        return self._parent  # type: ignore
-
-    def set_parent(self: T, parent: T | None, unchecked: bool = False):
-        """Set the parent of this instance.
+    def set_parent(self: T, parent: T | None):
+        """Set the parent of this instance and checks for cycles.
 
         Args:
             parent: The new parent of this instance, or None to make this
               instance an orphan.
-            unchecked: If true, there will be no check for cycles. Default
-              False.
 
         Raises:
             CycleException: This operation would create a cycle.
         """
 
-        if (
-            not unchecked
-            and parent is not None
-            and (parent == self or parent.is_child_of(self))
-        ):
+        if parent is not None and (parent == self or parent.is_child_of(self)):
             raise CycleException(parent, self)
-        self._parent = parent
-        self.save(update_fields=("_parent",))
+        self.parent = parent
+        self.save(update_fields=("parent",))
 
     def is_child_of(self: T, parent: T) -> bool:
         """Checks if this instance is a child of parent.
 
         Args:
             parent: Potential parent instance.
 
         Returns:
             True if the instance is a child of parent at any level. Returns
             false when checked against itself.
         """
 
-        ancestor = self._parent
+        ancestor = self.parent
         while ancestor is not None:
             if ancestor == parent:
                 return True
-            ancestor = ancestor._parent
+            ancestor = ancestor.parent
         return False
 
     def root(self: T) -> T:
         """Root of this instance.
 
         Returns:
             The top level root of this instance. Will return self if an orphan.
         """
 
         root = self
-        while root._parent is not None:
-            root = root._parent  # type: ignore
+        while root.parent is not None:
+            root = root.parent  # type: ignore
         return root
 
     def ancestors(
         self: T,
         max_level: int | None = None,
     ) -> list[T]:
         """Ancestors of this instance.
@@ -106,18 +84,18 @@
             at the lowest index of the list.
         """
 
         if max_level is None:
             max_level = -1
         ancestors = []
         ancestor: T | None
-        ancestor = self._parent  # type: ignore
+        ancestor = self.parent  # type: ignore
         while ancestor is not None and max_level != 0:
             ancestors.append(ancestor)
-            ancestor = ancestor._parent  # type: ignore
+            ancestor = ancestor.parent  # type: ignore
             max_level -= 1
         return ancestors
 
     def direct_children(
         self: T,
         object_manager: BaseManager[T] | None = None,
     ) -> QuerySet[T]:
@@ -130,15 +108,15 @@
         Returns:
             An unordered QuerySet containing all the direct children of this
             instance.
         """
 
         if object_manager is None:
             object_manager = self.__class__._default_manager
-        return object_manager.filter(_parent=self)
+        return object_manager.filter(parent=self)
 
     def children(
         self: T,
         max_generations: int | None = None,
         max_siblings: int | None = None,
         max_total: int | None = None,
         sibling_transform: Callable[[QuerySet[T]], QuerySet[T]] | None = None,
```

### Comparing `django_hierarchical_models-2.0.0/django_hierarchical_models/models/node.py` & `django_hierarchical_models-2.1.0/django_hierarchical_models/models/node.py`

 * *Files identical despite different names*

### Comparing `django_hierarchical_models-2.0.0/pyproject.toml` & `django_hierarchical_models-2.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-hierarchical-models"
-version = "2.0.0"
+version = "2.1.0"
 description = "Adds hierarchical models to Django"
 authors = ["Josh Bedwell <rcxwhiz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/rcxwhiz/django-hierarchical-models"
 packages = [{include = "django_hierarchical_models"}]
 classifiers = [
```

### Comparing `django_hierarchical_models-2.0.0/PKG-INFO` & `django_hierarchical_models-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hierarchical-models
-Version: 2.0.0
+Version: 2.1.0
 Summary: Adds hierarchical models to Django
 Home-page: https://github.com/rcxwhiz/django-hierarchical-models
 License: MIT
 Author: Josh Bedwell
 Author-email: rcxwhiz@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Framework :: Django
@@ -43,46 +43,57 @@
 
 class MyModel(HierarchicalModel):
     name = models.CharField(max_length=100)
 
 ...
 
 child = MyModel.objects.create(name="Betty")
-child.parent()  # None
+child.parent  # None
 
 parent = MyModel.objects.create(name="Simon")
+# checks for pesky cycles
 child.set_parent(parent)
-child.parent()  # <MyModel: "Simon">
+# alternative
+# child.parent = parent
+child.parent  # <MyModel: "Simon">
 
 child.root()  # <MyModel: "Simon">
 parent.root()  # <MyModel: "Simon">
 
 parent.direct_children()  # [<MyModel: "Betty">]
 
 child.is_child_of(parent)  # True
 parent.is_child_of(child)  # False
 ```
 
+## parent = vs .set_parent()
+
+`parent` is a `ForeignKeyField` which may be directly accessed or set. The
+`.set_parent()` method checks to see if the operation would create a cycle, which can
+be bad for some of the other instance methods. The `.set_parent()` method is slower
+because it must determine if a cycle would be formed. `.set_parent()` makes a call to
+`.save(update_fields=("parent",))`, so it is not necessary to call `.save()` after
+updating the parent this way.
+
 ## Refreshing from database
 
-External changes to an instance's parent are not automatically reflected in the
-instance. This leads to the following behavior:
+The following is expected behavior:
 
 ```python
 instance_1 = MyModel.objects.create(name="Betty")
 instance_2 = MyModel.objects.create(parent=instance_1, name="Simon")
-insstance_2.parent()  # <MyModel: "Betty">
+instance_2.parent  # <MyModel: "Betty">
 
 instance_1.delete()
 
-instance_2.parent()  # <MyModel: "Betty">
+instance_2.parent  # <MyModel: "Betty">
 
 instance_2.refresh_from_db()
 
-instance_2.parent()  # None
+instance_2.parent  # None
 ```
 
 ```python
 instance_1 = MyModel.objects.create(name="Betty")
 instance_2 = MyModel.objects.create(parent=instance_1, name="Simon")
 instance_3 = MyModel.objects.create(parent=instance_2, name="Finn")
 instance_3_copy = MyModel.objects.get(pk=instance_3.pk)
@@ -103,16 +114,16 @@
 
 instance_1.root()  # <MyModel: "Betty">
 instance_2.root()  # <MyModel: "Simon">
 instance_3.root()  # <MyModel: "Simon">
 instance_3_copy.root()  # <MyModel: "Simon">
 ```
 
-Moral of the story, if your instance's parent might have been edited/deleted,
-you will want to refresh your instance for that change to be reflected.  
+Moral of the story, if your instance's parent might have been edited/deleted, you will
+want to refresh your instance for that change to be reflected.  
 
 ## Benchmarks
 
 The following benchmarks demonstrate that the query performance of the model stays the
 same from 10,000 to 1,000,000 models. These tests were done with Postgres. The results
 are in the form `total time (s) / per instance (ms)`. Eventually the query performance
 of this model should scale down with the total number of instances in the database,
```

