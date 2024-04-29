# Comparing `tmp/yaconfiglib-0.2.0.tar.gz` & `tmp/yaconfiglib-0.3.0.tar.gz`

## Comparing `yaconfiglib-0.2.0.tar` & `yaconfiglib-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/examples/config.toml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/examples/hiera.yaml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/examples/includeme.yaml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/examples/jinja.yaml.j2
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/__init__.py
--rw-r--r--   0        0        0     6307 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/hiera.py
--rw-r--r--   0        0        0     7135 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/backends/__init__.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/backends/base.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/backends/jinja2.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/backends/toml.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/backends/yaml.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/utils/__init__.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/utils/enum.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/utils/jinja2.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/utils/log.py
--rw-r--r--   0        0        0    16694 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/src/yaconfiglib/utils/merge.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/LICENSE
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/README.md
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 yaconfiglib-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/examples/config.toml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/examples/hiera.yaml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/examples/includeme.yaml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/examples/jinja.yaml.j2
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/example.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/__init__.py
+-rw-r--r--   0        0        0     9234 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/loader.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/backends/__init__.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/backends/base.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/backends/jinja2.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/backends/toml.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/backends/yaml.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/utils/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/utils/enum.py
+-rw-r--r--   0        0        0     2591 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/utils/jinja2.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/utils/log.py
+-rw-r--r--   0        0        0    16694 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/utils/merge.py
+-rw-r--r--   0        0        0     3345 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/src/yaconfiglib/utils/source.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/LICENSE
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/README.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 yaconfiglib-0.3.0/PKG-INFO
```

### Comparing `yaconfiglib-0.2.0/src/example.py` & `yaconfiglib-0.3.0/src/example.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import logging
 import sys
 from dataclasses import dataclass
 
 import yaml
 
-from yaconfiglib import hiera
-from yaconfiglib.backends.jinja2 import Jinja2ConfigLoader
-from yaconfiglib.backends.toml import TomlConfigLoader
-from yaconfiglib.backends.yaml import YamlConfigLoader
-from yaconfiglib.hiera import LogLevel, MergeMethod
+from yaconfiglib import YamlConfig
 from yaconfiglib.loader import ConfigLoader
+from yaconfiglib.loader import ConfigLoaderMergeMethod as MergeMethod
+from yaconfiglib.utils.log import LogLevel
 from yaconfiglib.utils.merge import typed_merge
 
 
 @dataclass
 class Test:
     field_1: str
     field_2: int
@@ -31,35 +29,36 @@
     dict(field_1=1, field_2=2),
     init=True,
 )
 
 
 logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
 
-loader = YamlConfigLoader()
+loader = YamlConfig()
 
 yaml.SafeLoader.add_constructor("!load", loader)
 
+configloader = ConfigLoader()
 
-hieraconf = hiera.load(
+hieraconf = configloader.load(
     """#!test.yaml
 pathname:
   stem: root
 """,
     "examples/hiera.yaml",
     interpolate=True,
+    merge=MergeMethod.Deep,
 )
 print(yaml.dump(hieraconf, indent=2))
 
 config = yaml.safe_load(
     "test: !load {pathname: examples/includeme.yaml, transform: '{ pathname.name: value.include }', key_factory: '%pathname.as_posix()', type: map }"
 )
 print(yaml.dump(config, indent=2))
 
-configloader = ConfigLoader()
 
 jinjaconfig = loader.load("examples/jinja.yaml.j2", configloader=configloader)
 print(yaml.dump(jinjaconfig, indent=2))
 
 pyproject = configloader.load("pyproject.toml")
 print(yaml.dump(pyproject, indent=2))
```

### Comparing `yaconfiglib-0.2.0/src/yaconfiglib/backends/base.py` & `yaconfiglib-0.3.0/src/yaconfiglib/backends/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,17 @@
         )
 
     @classmethod
     def get_class_by_name(cls, name: str) -> type[_ty.Self]:
         for scls in cls.__subclasses__(recursive=True):
             _name = getattr(scls, "NAME", None)
             if not _name:
-                _name = scls.__name__.lower().removesuffix("configloader")
+                _name = (
+                    scls.__name__.lower().removesuffix("loader").removesuffix("config")
+                )
             if _name == name:
                 return scls
 
     @classmethod
     def can_load_path(cls, path: _Path) -> bool:
         return (
             cls.PATHNAME_REGEX.match(path.name) != None if cls.PATHNAME_REGEX else False
```

### Comparing `yaconfiglib-0.2.0/src/yaconfiglib/backends/jinja2.py` & `yaconfiglib-0.3.0/src/yaconfiglib/backends/jinja2.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.2.0/src/yaconfiglib/backends/yaml.py` & `yaconfiglib-0.3.0/src/yaconfiglib/backends/yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import typing
 
 import yaml
 from pathlib_next import Path, Pathname
 
 from yaconfiglib.backends.base import ConfigBackend
 
-__all__ = ["YamlConfigLoader"]
+__all__ = ["YamlConfig"]
 
 
-class YamlConfigLoader(ConfigBackend):
+class YamlConfig(ConfigBackend):
     PATHNAME_REGEX = re.compile(r".*\.((yaml)|(yml))$", re.IGNORECASE)
     DEFAULT_LOADER_CLS = yaml.SafeLoader
     PATH_FACTORY = Path
 
     def __call__(self, loader: yaml.Loader, node: yaml.Node):
         args = ()
         kwargs = {}
```

### Comparing `yaconfiglib-0.2.0/src/yaconfiglib/utils/log.py` & `yaconfiglib-0.3.0/src/yaconfiglib/utils/log.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.2.0/src/yaconfiglib/utils/merge.py` & `yaconfiglib-0.3.0/src/yaconfiglib/utils/merge.py`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.2.0/LICENSE` & `yaconfiglib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yaconfiglib-0.2.0/pyproject.toml` & `yaconfiglib-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "yaconfiglib"
-version = "0.2.0"
+version = "0.3.0"
 authors = [{ name = "Jose A" }]
 description = "Another Config lib for python, basically load config/yaml/toml/... files and add some features like relative import and templating."
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `yaconfiglib-0.2.0/PKG-INFO` & `yaconfiglib-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: yaconfiglib
-Version: 0.2.0
+Version: 0.3.0
 Summary: Another Config lib for python, basically load config/yaml/toml/... files and add some features like relative import and templating.
 Project-URL: Homepage, https://github.com/jose-pr/yaconfiglib/
 Project-URL: Issues, https://github.com/jose-pr/yaconfiglib/issues
 Author: Jose A
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

