# Comparing `tmp/pluginmgr-1.1.0.tar.gz` & `tmp/pluginmgr-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluginmgr-1.1.0.tar", max compression
+gzip compressed data, was "pluginmgr-1.2.0.tar", max compression
```

## Comparing `pluginmgr-1.1.0.tar` & `pluginmgr-1.2.0.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0    11358 2022-03-21 15:09:20.259428 pluginmgr-1.1.0/LICENSE
--rw-r--r--   0        0        0     1803 2022-03-21 15:09:20.259428 pluginmgr-1.1.0/README.md
--rw-r--r--   0        0        0     1348 2022-03-21 15:09:58.479459 pluginmgr-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6403 2022-03-21 15:09:20.262761 pluginmgr-1.1.0/src/pluginmgr/__init__.py
--rw-r--r--   0        0        0     3764 2022-03-21 15:09:20.262761 pluginmgr-1.1.0/src/pluginmgr/config.py
--rw-r--r--   0        0        0     2584 2022-03-21 15:09:59.616166 pluginmgr-1.1.0/setup.py
--rw-r--r--   0        0        0     2651 2022-03-21 15:09:59.616651 pluginmgr-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2020-10-31 17:02:01.566928 pluginmgr-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1803 2022-03-21 18:54:04.048965 pluginmgr-1.2.0/README.md
+-rw-r--r--   0        0        0     1290 2024-04-29 00:25:57.024882 pluginmgr-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7536 2024-04-29 00:23:05.022326 pluginmgr-1.2.0/src/pluginmgr/__init__.py
+-rw-r--r--   0        0        0     3764 2022-03-21 18:54:04.051965 pluginmgr-1.2.0/src/pluginmgr/config.py
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 pluginmgr-1.2.0/PKG-INFO
```

### Comparing `pluginmgr-1.1.0/LICENSE` & `pluginmgr-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pluginmgr-1.1.0/README.md` & `pluginmgr-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pluginmgr-1.1.0/src/pluginmgr/__init__.py` & `pluginmgr-1.2.0/src/pluginmgr/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import imp
 import importlib
+import importlib.util
+import types
+import importlib_metadata
 import logging
 import os
 import re
 import sys
 
-import pkg_resources
 
-
-class SearchPathImporter:
+class SearchPathImporter(importlib.abc.MetaPathFinder, importlib.abc.Loader):
     """
     import hook to dynamically load modules from a search path
 
     """
 
     def __init__(self, namespace, searchpath, create_loader):
         self._searchpath = []
@@ -20,14 +20,17 @@
         self.namespace = namespace
         self.log = logging.getLogger(__name__)
         self.re_ns = re.compile(r"^%s\.(.*)$" % re.escape(self.namespace))
         self.log.debug(f"hook.compile({self.namespace})")
         self.searchpath = searchpath
         self.create_loader = create_loader
 
+    def install(self):
+        sys.meta_path.append(self)
+
     @property
     def searchpath(self):
         return getattr(self, "_searchpath")
 
     @searchpath.setter
     def searchpath(self, value):
         if not value:
@@ -55,34 +58,56 @@
             return
 
         name = match.group(1)
         self.log.debug(f"hook match {name}")
         if self.find_file(name):
             return self
 
+    def find_spec(self, fullname, path=None, target=None):
+        self.log.debug(f"hook.find_spec({self}, {fullname}, {path}, {target})")
+        if self.create_loader:
+            if fullname == self.package or fullname == self.namespace:
+                return importlib.machinery.ModuleSpec(fullname, self)
+
+        match = self.re_ns.match(fullname)
+        if match:
+            if fq_path := self.find_file(match.group(1)):
+                return importlib.machinery.ModuleSpec(fullname, self, origin=fq_path)
+        return None
+
     def find_file(self, name):
         for each in self.searchpath:
             fq_path = os.path.join(each, name + ".py")
             self.log.debug(f"checking {fq_path}")
             if os.path.isfile(fq_path):
                 return fq_path
 
     def load_module(self, fullname):
         self.log.debug(f"hook.load({fullname})")
+        # For backward compatibility, delegate to exec_module.
+        module = types.ModuleType(fullname)
+        return self.exec_module(module)
+
+    def exec_module(self, module):
+        fullname = module.__name__
+        self.log.debug(f"hook.load({module}) {fullname}")
 
         # build package for loader if it doesn't exist
         # don't need to check for create_loader here, checks in find_module
         if fullname == self.package or fullname == self.namespace:
             self.log.debug(f"hook.create_loader({fullname})")
             # make a new loader module
-            mod = imp.new_module(fullname)
+            # spec = importlib.util.spec_from_loader(fullname, loader=self)
+            # mod = importlib.util.module_from_spec(spec)
+            mod = types.ModuleType(fullname)
 
             # set a few properties required by PEP 302
             mod.__file__ = self.namespace
             mod.__name__ = fullname
+            # this is the only one needed for py3.11
             mod.__path__ = self.searchpath
             mod.__loader__ = self
             mod.__package__ = ".".join(fullname.split(".")[:-1])
             sys.modules[fullname] = mod
             return mod
 
         match = self.re_ns.match(fullname)
@@ -143,32 +168,33 @@
             self._imphook.searchpath = value
             return
 
         if not value:
             return
 
         self._imphook = SearchPathImporter(self.namespace, value, self.create_loader)
-        sys.meta_path.append(self._imphook)
+        self._imphook.install()
 
     def import_external(self, namespace=None):
         if not namespace:
             namespace = self.namespace
-        for entry_point in pkg_resources.iter_entry_points(namespace):
+        for entry_point in importlib_metadata.entry_points()[namespace]:
             module = entry_point.load()
             self.searchpath = (self.searchpath or []) + [
                 os.path.dirname(module.__file__)
             ]
             # need to mark new searchpath as already imported
             # to avoid re-import from new namespace
             sys.modules[f"{namespace}{entry_point.name}"] = sys.modules[
                 entry_point.module_name
             ]
 
     def register(self, typ):
         """register a plugin"""
+
         # should be able to combine class/instance namespace, and inherit from either
         # would need to store meta or rely on copy ctor
         def _func(cls):
             if typ in self._class:
                 raise ValueError("duplicated type name '%s'" % typ)
             cls.plugin_type = typ
             self._class[typ] = cls
```

### Comparing `pluginmgr-1.1.0/src/pluginmgr/config.py` & `pluginmgr-1.2.0/src/pluginmgr/config.py`

 * *Files identical despite different names*

### Comparing `pluginmgr-1.1.0/PKG-INFO` & `pluginmgr-1.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: pluginmgr
-Version: 1.1.0
+Version: 1.2.0
 Summary: lightweight python plugin system supporting config inheritance
 Home-page: https://github.com/20c/pluginmgr
 License: Apache-2.0
 Author: 20C
 Author-email: code@20c.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development
-Requires-Dist: munge (>=1.0.0,<2.0.0)
+Requires-Dist: importlib-metadata (>=1)
+Requires-Dist: munge (>=1)
 Project-URL: Repository, https://github.com/20c/pluginmgr
 Description-Content-Type: text/markdown
 
 
 # pluginmgr
```

