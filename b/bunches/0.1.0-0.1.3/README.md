# Comparing `tmp/bunches-0.1.0.tar.gz` & `tmp/bunches-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bunches-0.1.0.tar", max compression
+gzip compressed data, was "bunches-0.1.3.tar", last modified: Mon Apr 29 08:11:28 2024, max compression
```

## Comparing `bunches-0.1.0.tar` & `bunches-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0     2884 2021-10-26 16:37:12.189180 bunches-0.1.0/bunches/__init__.py
--rw-r--r--   0        0        0     9622 2021-10-26 16:56:10.266078 bunches-0.1.0/bunches/base.py
--rw-r--r--   0        0        0    20487 2021-10-26 17:45:15.304703 bunches-0.1.0/bunches/mappings.py
--rw-r--r--   0        0        0    15760 2021-10-26 16:37:12.192183 bunches-0.1.0/bunches/sequences.py
--rw-r--r--   0        0        0     2679 2021-10-26 17:10:44.764307 bunches-0.1.0/bunches/utilities.py
--rw-r--r--   0        0        0      552 2021-10-26 18:02:12.831885 bunches-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1932 2021-10-26 18:00:30.774187 bunches-0.1.0/README.md
--rw-r--r--   0        0        0     2616 2021-10-26 18:03:56.795191 bunches-0.1.0/setup.py
--rw-r--r--   0        0        0     2472 2021-10-26 18:03:56.796192 bunches-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      608 2024-04-29 08:11:15.031423 bunches-0.1.3/LICENSE
+-rw-r--r--   0        0        0     6913 2024-04-29 08:11:15.031423 bunches-0.1.3/README.md
+-rw-r--r--   0        0        0     3847 2024-04-29 08:11:28.831556 bunches-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      438 2024-04-29 08:11:15.031423 bunches-0.1.3/src/bunches/__init__.py
+-rw-r--r--   0        0        0     5120 2024-04-29 08:11:15.031423 bunches-0.1.3/src/bunches/base.py
+-rw-r--r--   0        0        0     1494 2024-04-29 08:11:15.031423 bunches-0.1.3/src/bunches/kinds.py
+-rw-r--r--   0        0        0    23790 2024-04-29 08:11:15.031423 bunches-0.1.3/src/bunches/mappings.py
+-rw-r--r--   0        0        0    13661 2024-04-29 08:11:15.031423 bunches-0.1.3/src/bunches/sequences.py
+-rw-r--r--   0        0        0     1687 2024-04-29 08:11:15.031423 bunches-0.1.3/src/bunches/settings.py
+-rw-r--r--   0        0        0     4326 2024-04-29 08:11:15.031423 bunches-0.1.3/src/bunches/utilities.py
+-rw-r--r--   0        0        0     4063 2024-04-29 08:11:15.031423 bunches-0.1.3/tests/test_bunches.py
+-rw-r--r--   0        0        0      166 2024-04-29 08:11:15.031423 bunches-0.1.3/tests/test_main.py
+-rw-r--r--   0        0        0     7770 1970-01-01 00:00:00.000000 bunches-0.1.3/PKG-INFO
```

### Comparing `bunches-0.1.0/bunches/sequences.py` & `bunches-0.1.3/src/bunches/sequences.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,401 +1,372 @@
-"""
-sequences: extensible, flexible, lightweight list-like classes
-Corey Rayburn Yung <coreyrayburnyung@gmail.com>
-Copyright 2021, Corey Rayburn Yung
-License: Apache-2.0
-
-    Licensed under the Apache License, Version 2.0 (the "License");
-    you may not use this file except in compliance with the License.
-    You may obtain a copy of the License at
-
-        http://www.apache.org/licenses/LICENSE-2.0
-
-    Unless required by applicable law or agreed to in writing, software
-    distributed under the License is distributed on an "AS IS" BASIS,
-    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-    See the License for the specific language governing permissions and
-    limitations under the License.
+"""List-like classes
 
 Contents:
-    Listing (Bunch, MutableSequence): drop-in replacement for a python list with 
-        additional functionality.
-    Hybrid (Listing): iterable with both dict and list interfaces. Stored items
-        must be hashable or have a 'name' attribute.
-    
-ToDo:
+    Listing (base.Bunch, MutableSequence): drop-in replacement for a python
+        `list` with additional functionality.
+    DictList (Listing): iterable with both `dict` and `list` interfaces. Stored
+        items must be hashable or have a `name` attribute.
+
+To Do:
+
 
-        
 """
 from __future__ import annotations
-from collections.abc import Hashable, Mapping, MutableSequence, Sequence
+
 import copy
 import dataclasses
-from typing import Any, Optional, Union
+from collections.abc import Hashable, Mapping, MutableSequence
+from typing import TYPE_CHECKING, Any
+
+from . import base, utilities
+
+if TYPE_CHECKING:
+    from .kinds import GenericList
 
-from . import base
-from . import utilities
 
-                          
-@dataclasses.dataclass # type: ignore
-class Listing(base.Bunch, MutableSequence): # type: ignore
-    """Basic bunches list replacement.
-    
-    A Listing differs from an ordinary python list in ways required by 
-    inheriting from Bunch: 'add' and 'subset' methods, storing data in 
-    'contents', and allowing the '+' operator to join Listings with other lists 
-    and Listings) and in 1 other way.
-        1) It includes a 'prepend' method for adding one or more items to the
+@dataclasses.dataclass
+class Listing(base.Bunch, MutableSequence):
+    """Basic `list` replacement.
+
+    A `Listing` differs from an ordinary python `list` in ways required by
+    inheriting from `Bunch`: `add`, `delete`, and `subset` methods, and allowing
+    the "+" operator to join `Listing`s with other `list`-like objects) and in 1
+    other way:
+        1) It includes a `prepend` method for adding one or more items to the
             beginning of the stored list.
-    
-    The 'add' method attempts to extend 'contents' with the item to be added.
-    If this fails, it appends the item to 'contents'.
-            
+
+    The `add` method attempts to extend `contents` with the item to be added.
+    If this fails, it appends the item to `contents`.
+
     Args:
-        contents (MutableSequence[Any]): items to store in a list. Defaults to 
-            an empty list.
-        
+        contents: items to store in a `list`. Defaults to an empty `list`.
+
     """
-    contents: MutableSequence[Any] = dataclasses.field(default_factory = list)
 
-    """ Public Methods """
+    contents: GenericList = dataclasses.field(default_factory = list)
+
+    """ Instance Methods """
 
-    def add(self, item: Union[Any, Sequence[Any]]) -> None:
-        """Tries to extend 'contents' with 'item'. Otherwise, it appends.
+    def add(self, item: Any | GenericList) -> None:
+        """Tries to extend `contents` with `item`. Otherwise, it appends.
 
         The method will extend all passed sequences, except str types, which it
         will append.
-        
+
         Args:
-            item (Union[Any, Sequence[Any]]): item(s) to add to the 'contents' 
-                attribute.
-                
+            item: item(s) to add to `contents`.
+
         """
-        if isinstance(item, Sequence) and not isinstance(item, str):
+        if utilities._is_sequence(item = item):
             self.contents.extend(item)
         else:
             self.contents.append(item)
         return
 
+    def delete(self, item: int) -> None:
+        """Deletes item at the index in `contents`.
+
+        Args:
+            item: index in `contents` to delete.
+
+        """
+        del self.contents[item]
+        return
+
     def insert(self, index: int, item: Any) -> None:
-        """Inserts 'item' at 'index' in 'contents'.
+        """Inserts `item` at `index` in `contents`.
 
         Args:
-            index (int): index to insert 'item' at.
-            item (Any): object to be inserted.
-            
+            index: index to insert `item` at.
+            item: object to be inserted.
+
         """
         self.contents.insert(index, item)
         return
 
-    def prepend(self, item: Union[Any, Sequence[Any]]) -> None:
-        """Prepends 'item' to 'contents'.
+    def prepend(self, item: Any | GenericList) -> None:
+        """Prepends `item` to `contents`.
+
+        If `item` is a non-str sequence, `prepend` adds its contents to the
+        stored list in the order they appear in `item`.
+
+        Args:
+            item: item(s) to prepend to `contents`.
 
-        If 'item' is a non-str sequence, 'prepend' adds its contents to the 
-        stored list in the order they appear in 'item'.
-        
-        Args:
-            item (Union[Any, Sequence[Any]]): item(s) to prepend to the 
-                'contents' attribute.
-                
         """
-        if isinstance(item, Sequence) and not isinstance(item, str):
+        if utilities._is_sequence(item = item):
             for thing in reversed(item):
                 self.prepend(item = thing)
         else:
             self.insert(0, item)
         return
-                   
+
     def subset(
-        self, 
-        include: Optional[Union[Sequence[Any], Any]] = None, 
-        exclude: Optional[Union[Sequence[Any], Any]] = None) -> Listing:
-        """Returns a new instance with a subset of 'contents'.
-
-        This method applies 'include' before 'exclude' if both are passed. If
-        'include' is None, all existing keys will be added before 'exclude' is
-        applied.
-        
+        self,
+        include: Any | GenericList | None = None,
+        exclude: Any | GenericList | None = None) -> Listing:
+        """Returns a new instance with a subset of `contents`.
+
+        This method applies `include` before `exclude` if both are passed. If
+        `include` is None, all existing items will be added to the new subset
+        class instance before `exclude` is applied.
+
         Args:
-            include (Optional[Union[Sequence[Any], Any]]): item(s) to include in 
+            include (Optional[Any | GenericList]): item(s) to include in
+                the new instance. Defaults to None.
+            exclude (Optional[Any | GenericList]): item(s) to exclude in
                 the new instance. Defaults to None.
-            exclude (Optional[Union[Sequence[Any], Any]]): item(s) to exclude in 
-                the new instance. Defaults to None.       
-        
+
         Raises:
-            ValueError: if 'include' and 'exclude' are both None.
-                              
+            ValueError: if `include` and `exclude` are both None.
+
         Returns:
-            Listing: with only items from 'include' and no items in 'exclude'.
+            Listing: with only items from `include` and no items in `exclude`.
 
         """
         if include is None and exclude is None:
             raise ValueError('include or exclude must not be None')
+        if include is None:
+            contents = copy.deepcopy(self.contents)
         else:
-            if include is None:
-                contents = self.contents
-            else:
-                include = list(utilities.iterify(item = include))
-                contents = [i for i in self.contents if i in include]
-            if exclude is not None:
-                exclude = list(utilities.iterify(item = exclude))
-                contents = [i for i in contents if i not in exclude]
-            new_listing = copy.deepcopy(self)
-            new_listing.contents = contents
+            include = list(utilities._iterify(include))
+            contents = [i for i in self.contents if i in include]
+        if exclude is not None:
+            exclude = list(utilities._iterify(exclude))
+            contents = [i for i in contents if i not in exclude]
+        new_listing = copy.deepcopy(self)
+        new_listing.contents = contents
         return new_listing
-                       
+
     """ Dunder Methods """
 
     def __getitem__(self, index: Any) -> Any:
-        """Returns value(s) for 'key' in 'contents'.
+        """Returns value(s) for `key` in `contents`.
 
         Args:
-            index (Any): index to search for in 'contents'.
+            index (Any): index to search for in `contents`.
 
         Returns:
-            Any: item stored in 'contents' at key.
+            Any: item stored in `contents` at key.
 
         """
         return self.contents[index]
-            
+
     def __setitem__(self, index: Any, value: Any) -> None:
-        """sets 'key' in 'contents' to 'value'.
+        """Sets `key` in `contents` to `value`.
 
         Args:
-            index (Any): index to set 'value' to in 'contents'.
-            value (Any): value to be set at 'key' in 'contents'.
+            index (Any): index to set `value` to in `contents`.
+            value (Any): value to be set at `key` in `contents`.
 
         """
         self.contents[index] = value
         return
 
-    def __delitem__(self, index: Any) -> None:
-        """Deletes item at 'key' index in 'contents'.
-
-        Args:
-            index (Any): index in 'contents' to delete.
 
-        """
-        del self.contents[index]
-        return
-
-
-@dataclasses.dataclass # type: ignore
-class Hybrid(Listing):
+@dataclasses.dataclass
+class DictList(Listing):
     """Iterable that has both a dict and list interfaces.
-    
-    Hybrid combines the functionality and interfaces of python dicts and lists.
+
+    DictList combines the functionality and interfaces of python dicts and lists.
     It allows duplicate keys and list-like iteration while supporting the easier
     access methods of dictionaries. In order to support this hybrid approach to
-    iterables, Hybrid can only store items that are hashable or have a 'name' 
+    iterables, DictList can only store items that are hashable or have a `name`
     attribute or property that contains or returns a hashable value.
 
-    A Hybrid inherits the differences between a Listing and an ordinary python 
+    A DictList inherits the differences between a Listing and an ordinary python
     list.
-    
-    A Hybrid differs from a Listing in 3 significant ways:
+
+    A DictList differs from a Listing in 3 significant ways:
         1) It only stores hashable items or objects for which a str name can be
-            derived (using the get_name function).
-        2) Hybrid has an interface of both a dict and a list, but stores a list. 
-            Hybrid does this by taking advantage of the 'name' attribute or
-            hashability of stored items. A 'name' or hash acts as a key to 
-            create the facade of a dict with the items in the stored list 
-            serving as values. This allows for duplicate keys for storing items, 
-            simpler iteration than a dict, and support for returning multiple 
-            matching items. This design comes at the expense of lookup speed. As 
-            a result, Hybrid should only be used if a high volume of access 
-            calls is not anticipated. Ordinarily, the loss of lookup speed 
+            derived (using the namify function).
+        2) DictList has an interface of both a dict and a list, but stores a list.
+            DictList does this by taking advantage of the `name` attribute or
+            hashability of stored items. A `name` or hash acts as a key to
+            create the facade of a dict with the items in the stored list
+            serving as values. This allows for duplicate keys for storing items,
+            simpler iteration than a dict, and support for returning multiple
+            matching items. This design comes at the expense of lookup speed. As
+            a result, DictList should only be used if a high volume of access
+            calls is not anticipated. Ordinarily, the loss of lookup speed
             should have negligible effect on overall performance.
-        3) Hybrids should not store int types. This ensures that when, for 
-            example, a 'hybrid[3]' is called, the item at that index is 
-            returned. If int types are stored, that call would create 
+        3) DictLists should not store int types. This ensures that when, for
+            example, a `dictlist_instance[3]` is called, the item at that index is
+            returned. If int types are stored, that call would create
             uncertainty as to whether an index or item should be returned. By
             design, int types are assumed to be calls to return the item at that
             index.
         4) When using dict access methods, a list of matches may be returned
-            because a Hybrid allows duplicate pseudo-keys to be used.
+            because a DictList allows duplicate pseudo-keys to be used.
 
     Args:
         contents (MutableSequence[Hashable]): items to store that are hashable
-            or have a 'name' attribute. Defaults to an empty list.
-        default_factory (Optional[Any]): default value to return or default 
-            function to call when the 'get' method is used. Defaults to None. 
-                          
+            or have a `name` attribute. Defaults to an empty list.
+        default_factory (Optional[Any]): default value to return or default
+            function to call when the `get` method is used. Defaults to None.
+
     """
+
     contents: MutableSequence[Hashable] = dataclasses.field(
         default_factory = list)
-    default_factory: Optional[Any] = None
-        
-    """ Public Methods """
-
-    def get(self, key: Hashable, default: Optional[Any] = None) -> Any: # type: ignore
-        """Returns value in 'contents' or default options.
-        
-        Args:
-            key (Hashable): key for value in 'contents'.
-            default (Optional[Any]): default value to return if 'key' is not 
-                found in 'contents'.
-        
+    default_factory: Any | None = None
+
+    """ Instance Methods """
+
+    def delete(self, item: Any | int) -> None:
+        """Deletes item in `contents`.
+
+        If `item` is not an int type, this method looks for a matching `name`
+        attribute in the stored instances and deletes all such items. If `key`
+        is an int type, only the item at that index is deleted.
+
+        Args:
+            item (Any, int): name or index in `contents` to delete.
+
+        """
+        if isinstance(item, int):
+            del self.contents[item]
+        else:
+            self.contents = [
+                c for c in self.contents if utilities._namify(c) != item]
+        return
+
+    def get(self, key: Hashable, default: Any | None = None) -> Any:
+        """Returns value in `contents` or default options.
+
+        Args:
+            key (Hashable): key for value in `contents`.
+            default (Optional[Any]): default value to return if `key` is not
+                found in `contents`.
+
         Raises:
-            KeyError: if 'key' is not in the Hybrid and 'default' and the
-                'default_factory' attribute are both None.
-        
+            KeyError: if `key` is not in the DictList and `default` and the
+                `default_factory` attribute are both None.
+
         Returns:
-            Any: value matching key in 'contents' or 'default_factory' value. 
-            
+            Any: value matching key in `contents` or `default_factory` value.
+
         """
         try:
             return self[key]
-        except (KeyError, TypeError):
-            if default is None:
-                if self.default_factory is None:
-                    raise KeyError(f'{key} is not in the Hybrid')
-                else:
-                    try:
-                        return self.default_factory()
-                    except TypeError:
-                        return self.default_factory
-            else:
+        except (KeyError, TypeError) as error:
+            if default is not None:
                 return default
+            if self.default_factory is None:
+                raise KeyError(f'{key} is not in the DictList') from error
+            try:
+                return self.default_factory()
+            except TypeError:
+                return self.default_factory
 
     def items(self) -> tuple[tuple[Hashable, ...], tuple[Any, ...]]:
-        """Emulates python dict 'items' method.
-        
+        """Emulates python dict `items` method.
+
         Returns:
-            tuple[tuple[Hashable, ...], tuple[Any, ...]]: a tuple equivalent to 
-                dict.items(). A Hybrid cannot actually create an ItemsView 
-                because that would eliminate any duplicate keys, which are 
-                permitted by Hybrid.
-            
+            tuple[tuple[Hashable, ...], tuple[Any, ...]]: a tuple equivalent to
+                dict.items(). A DictList cannot actually create an ItemsView
+                because that would eliminate any duplicate keys, which are
+                permitted by DictList.
+
         """
-        return tuple(zip(self.keys(), self.values()))
+        return tuple(zip(self.keys(), self.values(), strict = True))
 
     def keys(self) -> tuple[Hashable, ...]:
-        """Emulates python dict 'keys' method.
-        
+        """Emulates python dict `keys` method.
+
         Returns:
-            tuple[Hashable, ...]: a tuple equivalent to dict.keys(). A Hybrid 
-                cannot actually create an KeysView because that would eliminate 
-                any duplicate keys, which are permitted by Hybrid.
-            
-        """
-        return tuple([utilities.get_name(item = c) for c in self.contents])
-
-    def setdefault(self, value: Any) -> None: # type: ignore
-        """sets default value to return when 'get' method is used.
-        
+            tuple[Hashable, ...]: a tuple equivalent to dict.keys(). A DictList
+                cannot actually create an KeysView because that would eliminate
+                any duplicate keys, which are permitted by DictList.
+
+        """
+        return tuple(utilities._namify(c) for c in self.contents)
+
+    def setdefault(self, value: Any) -> None:
+        """Sets default value to return when `get` method is used.
+
         Args:
             value (Any): default value to return.
-            
+
         """
-        self.default_factory = value 
+        self.default_factory = value
         return
 
     def update(self, items: Mapping[Any, Any]) -> None:
-        """Mimics the dict 'update' method by extending 'contents' with 'items'.
-        
+        """Mimics the dict `update` method by extending `contents` with `items`.
+
         Args:
-            items (Mapping[Any, Any]): items to add to the 'contents' attribute. 
-                The values of 'items' are added to 'contents' and the keys 
-                become the 'name' attributes of those values. As a result, the 
-                keys of 'items' are discarded. To mimic dict' update', the 
-                passed 'items' values are added to 'contents' by the 'extend' 
-                method which adds the values to the end of 'contents'.           
-        
+            items (Mapping[Any, Any]): items to add to the `contents` attribute.
+                The values of `items` are added to `contents` and the keys
+                become the `name` attributes of those values. As a result, the
+                keys of `items` are discarded. To mimic `dict.update`, the
+                passed `items` values are added to `contents` by the `extend`
+                method which adds the values to the end of `contents`.
+
         """
         self.extend(list(items.values()))
         return
 
     def values(self) -> tuple[Any, ...]:
-        """Emulates python dict 'values' method.
-        
+        """Emulates python dict `values` method.
+
         Returns:
-            tuple[Any, ...]: a tuple equivalent to dict.values(). A Hybrid 
-                cannot actually create an ValuesView because that would 
-                eliminate any duplicate keys, which are permitted by Hybrid.
-            
+            tuple[Any, ...]: a tuple equivalent to dict.values(). A DictList
+                cannot actually create an ValuesView because that would
+                eliminate any duplicate keys, which are permitted by DictList.
+
         """
         return tuple(self.contents)
 
     """ Dunder Methods """
 
-    def __getitem__(self, key: Union[Hashable, int]) -> Any: # type: ignore
-        """Returns value(s) for 'key' in 'contents'.
-        
-        If 'key' is not an int type, this method looks for a matching 'name'
+    def __getitem__(self, key: Hashable | int) -> Any:
+        """Returns value(s) for `key` in `contents`.
+
+        If `key` is not an int type, this method looks for a matching `name`
         attribute in the stored instances.
-        
-        If 'key' is an int type, this method returns the stored item at the
+
+        If `key` is an int type, this method returns the stored item at the
         corresponding index.
-        
-        If only one match is found, a single item is returned. If more are 
-        found, a Hybrid or Hybrid subclass with the matching 'name' attributes 
-        is returned.
+
+        If only one match is found, a single item is returned. If more are
+        found, a `DictList` or `DictList` subclass with the matching `name`
+        attributes is returned.
 
         Args:
-            key (Union[Hashable, int]): name of an item or index to search for 
-                in 'contents'.
+            key (Hashable, int): name of an item or index to search for
+                in `contents`.
 
         Returns:
-            Any: value(s) stored in 'contents' that correspond to 'key'. If 
-                there is more than one match, the return is a Hybrid or Hybrid 
+            Any: value(s) stored in `contents` that correspond to `key`. If
+                there is more than one match, the return is a DictList or DictList
                 subclass with that matching stored items.
 
         """
         if isinstance(key, int):
             return self.contents[key]
+        matches = [
+            c for c in self.contents if utilities._namify(c) == key]
+        if not matches:
+            raise KeyError(f'{key} is not in {self.__class__.__name__}')
+        if len(matches) == 1:
+            return matches[0]
         else:
-            
-            matches = [
-                c for c in self.contents if utilities.get_name(item = c) == key]
-            # matches = []
-            # for value in self.contents:
-            #     if (
-            #         hash(value) == key 
-            #         or utilities.get_name(item = value) == key):
-            #         matches.append(value)
-            # matches = [
-            #     i for i, c in enumerate(self.contents)
-            #     if utilities.get_name(c) == key]
-            if len(matches) == 0:
-                raise KeyError(f'{key} is not in {self.__class__.__name__}')
-            elif len(matches) == 1:
-                return matches[0]
-            else:
-                return matches
-            
-    def __setitem__(self, key: Union[Any, int], value: Any) -> None:
-        """sets 'key' in 'contents' to 'value'.
-
-        Args:
-            key (Union[Any, int]): if key isn't an int, it is ignored (since the
-                'name' attribute of the value will be acting as the key). In
-                such a case, the 'value' is added to the end of 'contents'. If
-                key is an int, 'value' is assigned at the that index number in
-                'contents'.
-            value (Any): value to be paired with 'key' in 'contents'.
+            return matches
 
-        """
-        if isinstance(key, int):
-            self.contents[key] = value
-        else:
-            self.add(value)
-        return
-
-    def __delitem__(self, key: Union[Any, int]) -> None:
-        """Deletes item matching 'key' in 'contents'.
-
-        If 'key' is not an int type, this method looks for a matching 'name'
-        attribute in the stored instances and deletes all such items. If 'key'
-        is an int type, only the item at that index is deleted.
+    def __setitem__(self, key: Any | int, value: Any) -> None:
+        """Sets `key` in `contents` to `value`.
 
         Args:
-            key (Union[Any, int]): name or index in 'contents' to delete.
+            key (Any | int): if key isn`t an int, it is ignored (since the
+                `name` attribute of the value will be acting as the key). In
+                such a case, the `value` is added to the end of `contents`. If
+                key is an int, `value` is assigned at the that index number in
+                `contents`.
+            value (Any): value to be paired with `key` in `contents`.
 
         """
         if isinstance(key, int):
-            del self.contents[key]
+            self.contents[key] = value
         else:
-            self.contents = [
-                c for c in self.contents if utilities.get_name(c) != key]
+            self.add(value)
         return
-
```

