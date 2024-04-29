# Comparing `tmp/coredumpy-0.0.1.tar.gz` & `tmp/coredumpy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coredumpy-0.0.1.tar", last modified: Sun Apr 21 23:25:19 2024, max compression
+gzip compressed data, was "coredumpy-0.1.0.tar", last modified: Mon Apr 29 03:23:03 2024, max compression
```

## Comparing `coredumpy-0.0.1.tar` & `coredumpy-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,33 @@
-drwxr-xr-x   0 gaogaotiantian  (1000) gaogaotiantian  (1000)        0 2024-04-21 23:25:19.601571 coredumpy-0.0.1/
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)    11357 2024-04-21 19:19:52.000000 coredumpy-0.0.1/LICENSE
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)    14628 2024-04-21 23:25:19.601571 coredumpy-0.0.1/PKG-INFO
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)      647 2024-04-21 23:24:15.000000 coredumpy-0.0.1/README.md
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)     1171 2024-04-21 23:04:16.000000 coredumpy-0.0.1/pyproject.toml
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)       38 2024-04-21 23:25:19.601571 coredumpy-0.0.1/setup.cfg
-drwxr-xr-x   0 gaogaotiantian  (1000) gaogaotiantian  (1000)        0 2024-04-21 23:25:19.601571 coredumpy-0.0.1/src/
-drwxr-xr-x   0 gaogaotiantian  (1000) gaogaotiantian  (1000)        0 2024-04-21 23:25:19.601571 coredumpy-0.0.1/src/coredumpy/
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)      444 2024-04-21 23:05:37.000000 coredumpy-0.0.1/src/coredumpy/__init__.py
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)      227 2024-04-21 22:18:20.000000 coredumpy-0.0.1/src/coredumpy/__main__.py
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)     1522 2024-04-21 23:01:14.000000 coredumpy-0.0.1/src/coredumpy/coredumpy.py
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)      679 2024-04-21 23:25:16.000000 coredumpy-0.0.1/src/coredumpy/except_hook.py
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)      682 2024-04-21 23:08:47.000000 coredumpy-0.0.1/src/coredumpy/main.py
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)      498 2024-04-21 22:17:16.000000 coredumpy-0.0.1/src/coredumpy/patch.py
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)     4206 2024-04-21 23:03:03.000000 coredumpy-0.0.1/src/coredumpy/py_object_proxy.py
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)      500 2024-04-21 22:17:24.000000 coredumpy-0.0.1/src/coredumpy/type_support.py
-drwxr-xr-x   0 gaogaotiantian  (1000) gaogaotiantian  (1000)        0 2024-04-21 23:25:19.601571 coredumpy-0.0.1/src/coredumpy.egg-info/
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)    14628 2024-04-21 23:25:19.000000 coredumpy-0.0.1/src/coredumpy.egg-info/PKG-INFO
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)      436 2024-04-21 23:25:19.000000 coredumpy-0.0.1/src/coredumpy.egg-info/SOURCES.txt
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)        1 2024-04-21 23:25:19.000000 coredumpy-0.0.1/src/coredumpy.egg-info/dependency_links.txt
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)       45 2024-04-21 23:25:19.000000 coredumpy-0.0.1/src/coredumpy.egg-info/entry_points.txt
--rw-r--r--   0 gaogaotiantian  (1000) gaogaotiantian  (1000)       10 2024-04-21 23:25:19.000000 coredumpy-0.0.1/src/coredumpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:23:03.898373 coredumpy-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 03:22:50.000000 coredumpy-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-29 03:22:50.000000 coredumpy-0.1.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17306 2024-04-29 03:23:03.898373 coredumpy-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-29 03:22:50.000000 coredumpy-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-29 03:22:50.000000 coredumpy-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 03:23:03.898373 coredumpy-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:23:03.894373 coredumpy-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:23:03.894373 coredumpy-0.1.0/src/coredumpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-29 03:22:50.000000 coredumpy-0.1.0/src/coredumpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-29 03:22:50.000000 coredumpy-0.1.0/src/coredumpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-04-29 03:22:50.000000 coredumpy-0.1.0/src/coredumpy/coredumpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-29 03:22:50.000000 coredumpy-0.1.0/src/coredumpy/except_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-29 03:22:50.000000 coredumpy-0.1.0/src/coredumpy/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-29 03:22:50.000000 coredumpy-0.1.0/src/coredumpy/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-29 03:22:50.000000 coredumpy-0.1.0/src/coredumpy/py_object_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-29 03:22:50.000000 coredumpy-0.1.0/src/coredumpy/pytest_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-29 03:22:50.000000 coredumpy-0.1.0/src/coredumpy/type_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-29 03:22:50.000000 coredumpy-0.1.0/src/coredumpy/unittest_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-29 03:22:50.000000 coredumpy-0.1.0/src/coredumpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:23:03.898373 coredumpy-0.1.0/src/coredumpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17306 2024-04-29 03:23:03.000000 coredumpy-0.1.0/src/coredumpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-29 03:23:03.000000 coredumpy-0.1.0/src/coredumpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 03:23:03.000000 coredumpy-0.1.0/src/coredumpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-29 03:23:03.000000 coredumpy-0.1.0/src/coredumpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-29 03:23:03.000000 coredumpy-0.1.0/src/coredumpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 03:23:03.898373 coredumpy-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-29 03:22:50.000000 coredumpy-0.1.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-29 03:22:50.000000 coredumpy-0.1.0/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-29 03:22:50.000000 coredumpy-0.1.0/tests/test_py_object_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-29 03:22:50.000000 coredumpy-0.1.0/tests/test_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-29 03:22:50.000000 coredumpy-0.1.0/tests/test_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-29 03:22:50.000000 coredumpy-0.1.0/tests/test_utils.py
```

### Comparing `coredumpy-0.0.1/LICENSE` & `coredumpy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coredumpy-0.0.1/PKG-INFO` & `coredumpy-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: coredumpy
-Version: 0.0.1
-Summary: A utility tool to dump python stacks
+Version: 0.1.0
+Summary: coredumpy saves your crash site for post-mortem debugging
 Author-email: Tian Gao <gaogaotiantian@hotmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -203,58 +203,125 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/gaogaotiantian/coredumpy
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: System :: Logging
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: NOTICE.txt
 
 # coredumpy
 
-coredumpy saves your crash site so you can better debug your python program.
+[![build](https://github.com/gaogaotiantian/coredumpy/actions/workflows/build_test.yaml/badge.svg)](https://github.com/gaogaotiantian/coredumpy/actions/workflows/build_test.yaml)  [![coverage](https://img.shields.io/codecov/c/github/gaogaotiantian/coredumpy)](https://codecov.io/gh/gaogaotiantian/coredumpy)  [![pypi](https://img.shields.io/pypi/v/coredumpy.svg)](https://pypi.org/project/coredumpy/)  [![support-version](https://img.shields.io/pypi/pyversions/coredumpy)](https://img.shields.io/pypi/pyversions/coredumpy)  [![sponsor](https://img.shields.io/badge/%E2%9D%A4-Sponsor%20me-%23c96198?style=flat&logo=GitHub)](https://github.com/sponsors/gaogaotiantian)
+
+coredumpy saves your crash site for post-mortem debugging.
 
 ## Highlights
 
 * Easy to use
-* Supports pdb interface
-* Does not rely on pickle
-* Dump file is independent of environment
+* Native support for unittest, pytest and run-time exceptions
+* Portable and safe dump
+* Utilizes pdb interface
 
 ## Usage
 
 ### dump
 
-You can dump any frame (and its parent frames) manually by
+In most cases, you only need to hook `coredumpy` to some triggers
+
+For `Exception` and `unittest`, patch with a simple line
 
 ```python
-from coredumpy import dump
+import coredumpy
+# Create a dump in "./dumps" when there's an unhandled exception
+coredumpy.patch_except(directory='./dumps')
+# Create a dump in "./dumps" when there's a unittest failure/error
+coredumpy.patch_unittest(directory='./dumps')
+```
 
-dump("coredumpy_dump", frame)
+For `pytest`, you can use `coredumpy` as a plugin
 
-# without frame argument, it will dump the current frame stack
-dump("coredumpy_dump")
 ```
+# Create a dump in "./dumps" when there's a pytest failure/error
+pytest --enable-coredumpy --coredumpy-dir ./dumps
+```
+
+<details>
 
-You can hook the exception so a dump will be automatically created if your program crashes due to an exception
+<summary>
+Or you can dump the current frame stack manually
+</summary>
 
 ```python
-from coredumpy import patch_excepthook
-patch_excepthook()
+import coredumpy
+
+# Without frame argument, top frame will be the caller of coredumpy.dump()
+coredumpy.dump()
+# Specify a specific frame as the top frame to dump
+coredumpy.dump(frame)
+# Specify a filename to save the dump, without it a unique name will be generated
+coredumpy.dump(path='coredumpy.dump')
+# You can use a function for path
+coredumpy.dump(path=lambda: f"coredumpy_{time.time()}.dump")
+# Specify a directory to keep the dump
+coredumpy.dump(directory='./dumps')
+# Specify the description of the dump for peek
+coredumpy.dump(description="a random dump")
 ```
 
+</details>
+
 ### load
+
+Load your dump with
+
+```
+coredumpy load <your_dump_file>
+```
+
+A [pdb](https://docs.python.org/3/library/pdb.html) debugger will be brought up
+and of course not everything is supported.
+
+### peek
+
+If you only need some very basic information of the dump (to figure out which dump
+you actually need), you can use `peek` command.
+
+```
+coredumpy peek <your_dump_directory>
+coredumpy peek <your_dump_file1> <your_dump_file2>
+```
+
+## About the data
+
+Besides a couple of builtin types, coredumpy treats almost every object as an
+Python object with attributes, and that's what it records in the dump.
+
+It does not use `pickle` so you don't need to have the same run-time environment
+when you load the dump. It's also safer to open an arbitrary dump without the
+unsafe pickling process.
+
+That being said, most of the objects will not be "restored" as they were when
+being dumped. You are in an observer mode where you can inspect attributes of
+all objects. None of the methods of the objects would work, nor would any
+dymanic features.
+
+## License
+
+Copyright 2024 Tian Gao.
+
+Distributed under the terms of the  [Apache 2.0 license](https://github.com/gaogaotiantian/coredumpy/blob/master/LICENSE).
```

### Comparing `coredumpy-0.0.1/pyproject.toml` & `coredumpy-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "coredumpy"
 authors = [{name = "Tian Gao", email = "gaogaotiantian@hotmail.com"}]
-description = "A utility tool to dump python stacks"
+description = "coredumpy saves your crash site for post-mortem debugging"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 license = {file = "LICENSE"}
 dynamic = ["version"]
 classifiers = [
     "Development Status :: 4 - Beta",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: MacOS",
@@ -29,9 +28,12 @@
 
 [project.urls]
 Homepage = "https://github.com/gaogaotiantian/coredumpy"
 
 [project.scripts]
 coredumpy = "coredumpy:main"
 
+[project.entry-points.pytest11]
+coredumpy = "coredumpy:pytest_hook"
+
 [tool.setuptools.dynamic]
-version = {attr = "coredumpy.__version__"}
+version = {attr = "coredumpy.__version__"}
```

### Comparing `coredumpy-0.0.1/src/coredumpy/py_object_proxy.py` & `coredumpy-0.1.0/src/coredumpy/py_object_proxy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,102 @@
 # Licensed under the Apache License: http://www.apache.org/licenses/LICENSE-2.0
 # For details: https://github.com/gaogaotiantian/coredumpy/blob/master/NOTICE.txt
 
 
 import inspect
+import queue
 import types
 from typing import Callable
 
 
+class _Unknown:
+    def __repr__(self):
+        return "<Unknown Object>"
+
+
+_unknown = _Unknown()
+
+
 class PyObjectProxy:
     _objects: dict[str, dict] = {}
     _proxies: dict[str, object] = {}
     _encoders: dict[str, Callable] = {}
     _decoders: dict[str, Callable] = {}
+    _pending_objects: queue.Queue = queue.Queue()
+    _current_recursion_depth = 0
+    _max_recursion_depth = 100
 
     def __init__(self):
         self._coredumpy_attrs = {}
 
     @classmethod
     def clear(cls):
         cls._objects.clear()
         cls._proxies.clear()
 
     @classmethod
     def add_object(cls, obj):
-        if id(obj) not in cls._objects:
-            cls._objects[str(id(obj))] = cls.dump_object(obj)
+        if str(id(obj)) not in cls._objects:
+            cls._current_recursion_depth = 0
+            cls._add_object(obj)
+            while not cls._pending_objects.empty():
+                depth, o = cls._pending_objects.get()
+                cls._current_recursion_depth = depth
+                cls._objects[str(id(o))] = cls.dump_object(o)
+            cls._current_recursion_depth = 0
+            cls._pending_objects = queue.Queue()
+        return cls._objects[str(id(obj))]
+
+    @classmethod
+    def _add_object(cls, obj):
+        if cls._current_recursion_depth > cls._max_recursion_depth:
+            return
+        id_str = str(id(obj))
+        if id_str not in cls._objects:
+            cls._objects[id_str] = {"type": "_coredumpy_unknown"}
+            cls._pending_objects.put((cls._current_recursion_depth + 1, obj))
 
     @classmethod
     def dump_object(cls, obj):
         if obj is None:
             return {"type": "None"}
-        elif isinstance(obj, (int, float, str)):
+        elif isinstance(obj, (int, float, str, bool)):
             return {"type": type(obj).__name__, "value": obj}
-        elif isinstance(obj, (list, tuple)):
+        elif isinstance(obj, (list, tuple, set)):
             for item in obj:
-                cls.add_object(item)
+                cls._add_object(item)
             return {"type": type(obj).__name__, "value": [str(id(item)) for item in obj]}
         elif isinstance(obj, dict):
             for key, value in obj.items():
-                cls.add_object(key)
-                cls.add_object(value)
+                cls._add_object(key)
+                cls._add_object(value)
             return {"type": type(obj).__name__, "value": {str(id(key)): str(id(value)) for key, value in obj.items()}}
         elif type(obj) in cls._encoders:
             return cls._encoders[type(obj)](obj)
         return cls.default_encode(obj)
 
     @classmethod
     def load_object(cls, id, data=None):
         if id in cls._proxies:
             return cls._proxies[id]
         if data is None:
-            raise ValueError("Object not found")
-        if data["type"] == "None":
+            proxy = _unknown
+        elif data["type"] == "None":
             proxy = None
-        elif data["type"] in ("int", "float", "str"):
+        elif data["type"] in ("int", "float", "str", "bool"):
             proxy = data["value"]
-        elif data["type"] in ("list", "tuple"):
-            proxy = [cls.load_object(item_id, cls._objects[item_id]) for item_id in data["value"]]
+        elif data["type"] == "list":
+            proxy = [cls.load_object(item_id, cls._objects.get(item_id)) for item_id in data["value"]]
+        elif data["type"] == "tuple":
+            proxy = tuple(cls.load_object(item_id, cls._objects.get(item_id)) for item_id in data["value"])
+        elif data["type"] == "set":
+            proxy = set(cls.load_object(item_id, cls._objects.get(item_id)) for item_id in data["value"])
         elif data["type"] == "dict":
-            proxy = {cls.load_object(key_id, cls._objects[key_id]):
-                     cls.load_object(value_id, cls._objects[value_id])
+            proxy = {cls.load_object(key_id, cls._objects.get(key_id)):
+                     cls.load_object(value_id, cls._objects.get(value_id))
                      for key_id, value_id in data["value"].items()}
         elif data["type"] in cls._decoders:
             proxy = cls._decoders[data["type"]](id, data)
         else:
             proxy = cls.default_decode(id, data)
         cls._proxies[id] = proxy
         return proxy
@@ -72,21 +105,36 @@
     def load_objects(cls, data):
         cls._objects = data
         for id, obj in data.items():
             cls.load_object(id, obj)
 
     @classmethod
     def default_encode(cls, obj):
-        data = {"type": type(obj).__name__, "attrs": {}}
-        if isinstance(obj, (types.ModuleType, types.FunctionType, types.BuiltinFunctionType)):
+        obj_type = type(obj)
+        if obj_type.__module__ in ("builtins", "__main__"):
+            typename = obj_type.__qualname__
+        else:
+            typename = f"{obj_type.__module__}.{obj_type.__qualname__}"
+
+        data = {"type": typename, "attrs": {}}
+        if isinstance(obj, (types.ModuleType,
+                            types.FunctionType,
+                            types.BuiltinFunctionType,
+                            types.LambdaType,
+                            types.MethodType,
+                            )):
             return data
-        for attr, value in inspect.getmembers(obj):
-            if not attr.startswith("__") and not callable(value):
-                cls.add_object(value)
-                data["attrs"][attr] = str(id(value))
+        try:
+            for attr, value in inspect.getmembers(obj):
+                if not attr.startswith("__") and not callable(value):
+                    cls._add_object(value)
+                    data["attrs"][attr] = str(id(value))
+        except Exception:  # pragma: no cover
+            # inspect.getmembers may fail on some objects
+            pass
         return data
 
     @classmethod
     def default_decode(cls, id, data):
         obj = cls()
         obj._coredumpy_id = id
         obj._coredumpy_type = data["type"]
@@ -102,16 +150,14 @@
     def __setattr__(self, key, value):
         if key.startswith("_coredumpy_"):
             self.__dict__[key] = value
         else:
             self._coredumpy_attrs[key] = value
 
     def __getattr__(self, item):
-        if item.startswith("_coredumpy_"):
-            return self.__dict__[item]
         if item in self._coredumpy_attrs:
             return type(self)._proxies[self._coredumpy_attrs[item]]
         raise AttributeError(f"'{self._coredumpy_type}' object has no attribute '{item}'")
 
     def __repr__(self):
         return f"<{self._coredumpy_type} object at 0x{int(self._coredumpy_id):x}>"
```

### Comparing `coredumpy-0.0.1/src/coredumpy.egg-info/PKG-INFO` & `coredumpy-0.1.0/src/coredumpy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: coredumpy
-Version: 0.0.1
-Summary: A utility tool to dump python stacks
+Version: 0.1.0
+Summary: coredumpy saves your crash site for post-mortem debugging
 Author-email: Tian Gao <gaogaotiantian@hotmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -203,58 +203,125 @@
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: Homepage, https://github.com/gaogaotiantian/coredumpy
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: System :: Logging
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: NOTICE.txt
 
 # coredumpy
 
-coredumpy saves your crash site so you can better debug your python program.
+[![build](https://github.com/gaogaotiantian/coredumpy/actions/workflows/build_test.yaml/badge.svg)](https://github.com/gaogaotiantian/coredumpy/actions/workflows/build_test.yaml)  [![coverage](https://img.shields.io/codecov/c/github/gaogaotiantian/coredumpy)](https://codecov.io/gh/gaogaotiantian/coredumpy)  [![pypi](https://img.shields.io/pypi/v/coredumpy.svg)](https://pypi.org/project/coredumpy/)  [![support-version](https://img.shields.io/pypi/pyversions/coredumpy)](https://img.shields.io/pypi/pyversions/coredumpy)  [![sponsor](https://img.shields.io/badge/%E2%9D%A4-Sponsor%20me-%23c96198?style=flat&logo=GitHub)](https://github.com/sponsors/gaogaotiantian)
+
+coredumpy saves your crash site for post-mortem debugging.
 
 ## Highlights
 
 * Easy to use
-* Supports pdb interface
-* Does not rely on pickle
-* Dump file is independent of environment
+* Native support for unittest, pytest and run-time exceptions
+* Portable and safe dump
+* Utilizes pdb interface
 
 ## Usage
 
 ### dump
 
-You can dump any frame (and its parent frames) manually by
+In most cases, you only need to hook `coredumpy` to some triggers
+
+For `Exception` and `unittest`, patch with a simple line
 
 ```python
-from coredumpy import dump
+import coredumpy
+# Create a dump in "./dumps" when there's an unhandled exception
+coredumpy.patch_except(directory='./dumps')
+# Create a dump in "./dumps" when there's a unittest failure/error
+coredumpy.patch_unittest(directory='./dumps')
+```
 
-dump("coredumpy_dump", frame)
+For `pytest`, you can use `coredumpy` as a plugin
 
-# without frame argument, it will dump the current frame stack
-dump("coredumpy_dump")
 ```
+# Create a dump in "./dumps" when there's a pytest failure/error
+pytest --enable-coredumpy --coredumpy-dir ./dumps
+```
+
+<details>
 
-You can hook the exception so a dump will be automatically created if your program crashes due to an exception
+<summary>
+Or you can dump the current frame stack manually
+</summary>
 
 ```python
-from coredumpy import patch_excepthook
-patch_excepthook()
+import coredumpy
+
+# Without frame argument, top frame will be the caller of coredumpy.dump()
+coredumpy.dump()
+# Specify a specific frame as the top frame to dump
+coredumpy.dump(frame)
+# Specify a filename to save the dump, without it a unique name will be generated
+coredumpy.dump(path='coredumpy.dump')
+# You can use a function for path
+coredumpy.dump(path=lambda: f"coredumpy_{time.time()}.dump")
+# Specify a directory to keep the dump
+coredumpy.dump(directory='./dumps')
+# Specify the description of the dump for peek
+coredumpy.dump(description="a random dump")
 ```
 
+</details>
+
 ### load
+
+Load your dump with
+
+```
+coredumpy load <your_dump_file>
+```
+
+A [pdb](https://docs.python.org/3/library/pdb.html) debugger will be brought up
+and of course not everything is supported.
+
+### peek
+
+If you only need some very basic information of the dump (to figure out which dump
+you actually need), you can use `peek` command.
+
+```
+coredumpy peek <your_dump_directory>
+coredumpy peek <your_dump_file1> <your_dump_file2>
+```
+
+## About the data
+
+Besides a couple of builtin types, coredumpy treats almost every object as an
+Python object with attributes, and that's what it records in the dump.
+
+It does not use `pickle` so you don't need to have the same run-time environment
+when you load the dump. It's also safer to open an arbitrary dump without the
+unsafe pickling process.
+
+That being said, most of the objects will not be "restored" as they were when
+being dumped. You are in an observer mode where you can inspect attributes of
+all objects. None of the methods of the objects would work, nor would any
+dymanic features.
+
+## License
+
+Copyright 2024 Tian Gao.
+
+Distributed under the terms of the  [Apache 2.0 license](https://github.com/gaogaotiantian/coredumpy/blob/master/LICENSE).
```

