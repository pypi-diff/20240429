# Comparing `tmp/typing-protocol-intersection-0.4.0.tar.gz` & `tmp/typing_protocol_intersection-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typing-protocol-intersection-0.4.0.tar", last modified: Sun Mar 10 21:51:08 2024, max compression
+gzip compressed data, was "typing_protocol_intersection-0.4.1.tar", last modified: Mon Apr 29 20:40:20 2024, max compression
```

## Comparing `typing-protocol-intersection-0.4.0.tar` & `typing_protocol_intersection-0.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2024-03-10 21:51:08.791359 typing-protocol-intersection-0.4.0/
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)     1067 2022-03-12 15:38:10.000000 typing-protocol-intersection-0.4.0/LICENSE
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)     5886 2024-03-10 21:51:08.791359 typing-protocol-intersection-0.4.0/PKG-INFO
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)     5099 2024-03-10 21:42:10.000000 typing-protocol-intersection-0.4.0/README.md
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)     2000 2024-02-14 19:24:20.000000 typing-protocol-intersection-0.4.0/pyproject.toml
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)      884 2024-03-10 21:51:08.791359 typing-protocol-intersection-0.4.0/setup.cfg
-drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2024-03-10 21:51:08.791359 typing-protocol-intersection-0.4.0/tests/
--rw-------   0 mbiel     (1000) mbiel     (1000)     5281 2024-03-10 21:42:10.000000 typing-protocol-intersection-0.4.0/tests/test_mypy_plugin.py
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)      649 2022-03-12 12:10:18.000000 typing-protocol-intersection-0.4.0/tests/test_python_module.py
-drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2024-03-10 21:51:08.788025 typing-protocol-intersection-0.4.0/typing_protocol_intersection/
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)       76 2022-03-11 17:16:39.000000 typing-protocol-intersection-0.4.0/typing_protocol_intersection/__init__.py
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)    10234 2024-03-10 21:42:10.000000 typing-protocol-intersection-0.4.0/typing_protocol_intersection/mypy_plugin.py
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)        0 2022-03-09 10:02:04.000000 typing-protocol-intersection-0.4.0/typing_protocol_intersection/py.typed
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)      865 2023-05-24 20:17:27.000000 typing-protocol-intersection-0.4.0/typing_protocol_intersection/types.py
-drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2024-03-10 21:51:08.791359 typing-protocol-intersection-0.4.0/typing_protocol_intersection.egg-info/
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)     5886 2024-03-10 21:51:08.000000 typing-protocol-intersection-0.4.0/typing_protocol_intersection.egg-info/PKG-INFO
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)      473 2024-03-10 21:51:08.000000 typing-protocol-intersection-0.4.0/typing_protocol_intersection.egg-info/SOURCES.txt
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)        1 2024-03-10 21:51:08.000000 typing-protocol-intersection-0.4.0/typing_protocol_intersection.egg-info/dependency_links.txt
--rw-r--r--   0 mbiel     (1000) mbiel     (1000)       29 2024-03-10 21:51:08.000000 typing-protocol-intersection-0.4.0/typing_protocol_intersection.egg-info/top_level.txt
+drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2024-04-29 20:40:20.397634 typing_protocol_intersection-0.4.1/
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)     1067 2022-03-12 15:38:10.000000 typing_protocol_intersection-0.4.1/LICENSE
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)     5887 2024-04-29 20:40:20.397634 typing_protocol_intersection-0.4.1/PKG-INFO
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)     5100 2024-04-29 20:31:36.000000 typing_protocol_intersection-0.4.1/README.md
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)     2000 2024-02-14 19:24:20.000000 typing_protocol_intersection-0.4.1/pyproject.toml
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)      884 2024-04-29 20:40:20.397634 typing_protocol_intersection-0.4.1/setup.cfg
+drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2024-04-29 20:40:20.394301 typing_protocol_intersection-0.4.1/tests/
+-rw-------   0 mbiel     (1000) mbiel     (1000)     5349 2024-04-29 20:31:36.000000 typing_protocol_intersection-0.4.1/tests/test_mypy_plugin.py
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)      649 2022-03-12 12:10:18.000000 typing_protocol_intersection-0.4.1/tests/test_python_module.py
+drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2024-04-29 20:40:20.394301 typing_protocol_intersection-0.4.1/typing_protocol_intersection/
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)       76 2022-03-11 17:16:39.000000 typing_protocol_intersection-0.4.1/typing_protocol_intersection/__init__.py
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)    10234 2024-04-29 20:31:36.000000 typing_protocol_intersection-0.4.1/typing_protocol_intersection/mypy_plugin.py
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)        0 2022-03-09 10:02:04.000000 typing_protocol_intersection-0.4.1/typing_protocol_intersection/py.typed
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)      865 2023-05-24 20:17:27.000000 typing_protocol_intersection-0.4.1/typing_protocol_intersection/types.py
+drwxr-xr-x   0 mbiel     (1000) mbiel     (1000)        0 2024-04-29 20:40:20.397634 typing_protocol_intersection-0.4.1/typing_protocol_intersection.egg-info/
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)     5887 2024-04-29 20:40:20.000000 typing_protocol_intersection-0.4.1/typing_protocol_intersection.egg-info/PKG-INFO
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)      473 2024-04-29 20:40:20.000000 typing_protocol_intersection-0.4.1/typing_protocol_intersection.egg-info/SOURCES.txt
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)        1 2024-04-29 20:40:20.000000 typing_protocol_intersection-0.4.1/typing_protocol_intersection.egg-info/dependency_links.txt
+-rw-r--r--   0 mbiel     (1000) mbiel     (1000)       29 2024-04-29 20:40:20.000000 typing_protocol_intersection-0.4.1/typing_protocol_intersection.egg-info/top_level.txt
```

### Comparing `typing-protocol-intersection-0.4.0/LICENSE` & `typing_protocol_intersection-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typing-protocol-intersection-0.4.0/PKG-INFO` & `typing_protocol_intersection-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing-protocol-intersection
-Version: 0.4.0
+Version: 0.4.1
 Summary: Protocol intersection for mypy
 Home-page: https://github.com/klausweiss/typing-protocol-intersection
 Project-URL: Bug Tracker, https://github.com/klausweiss/typing-protocol-intersection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -27,15 +27,15 @@
 The `ProtocolIntersection` type tells mypy that an object implements multiple protocols.
 It can be used either as a function parameter or as a return value.
 A mypy plugin that ships with the package is required for this to work.
 See the [examples](#examples) section below.
 
 ## Supported versions
 
-The plugin supports python 3.8 up to 3.12 and mypy >= 0.920 and <= 1.9.x.
+The plugin supports python 3.8 up to 3.12 and mypy >= 0.920 and <= 1.10.x.
 
 ## Installation
 
 The `typing-protocol-intersection` package is pip-installable:
 
 ```shell
 pip install typing-protocol-intersection
```

### Comparing `typing-protocol-intersection-0.4.0/README.md` & `typing_protocol_intersection-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 The `ProtocolIntersection` type tells mypy that an object implements multiple protocols.
 It can be used either as a function parameter or as a return value.
 A mypy plugin that ships with the package is required for this to work.
 See the [examples](#examples) section below.
 
 ## Supported versions
 
-The plugin supports python 3.8 up to 3.12 and mypy >= 0.920 and <= 1.9.x.
+The plugin supports python 3.8 up to 3.12 and mypy >= 0.920 and <= 1.10.x.
 
 ## Installation
 
 The `typing-protocol-intersection` package is pip-installable:
 
 ```shell
 pip install typing-protocol-intersection
```

### Comparing `typing-protocol-intersection-0.4.0/pyproject.toml` & `typing_protocol_intersection-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `typing-protocol-intersection-0.4.0/setup.cfg` & `typing_protocol_intersection-0.4.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = typing-protocol-intersection
-version = 0.4.0
+version = 0.4.1
 description = Protocol intersection for mypy
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/klausweiss/typing-protocol-intersection
 project_urls = 
 	Bug Tracker = https://github.com/klausweiss/typing-protocol-intersection/issues
 classifiers =
```

### Comparing `typing-protocol-intersection-0.4.0/tests/test_mypy_plugin.py` & `typing_protocol_intersection-0.4.1/tests/test_mypy_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
 
 @pytest.mark.parametrize(
     "version",
     [
         pytest.param("0.910", id="0.910 - before the first supported 0.920"),
         pytest.param("0.992", id="0.992 - non-existent version greater than the last tested 0.x"),
-        pytest.param("1.10.0", id="1.10.0 - first greater than 1.9.x with breaking changes"),
+        pytest.param("1.11.0", id="1.11.0 - first greater than 1.10.x with breaking changes"),
     ],
 )
 def test_raises_for_unsupported_mypy_versions(version: str) -> None:
     with pytest.raises(NotImplementedError):
         typing_protocol_intersection.mypy_plugin.plugin(version)
 
 
@@ -124,13 +124,14 @@
         pytest.param("1.3.0", id="1.3.0 - some 1.3.x version"),
         pytest.param("1.4.0", id="1.4.0 - some 1.4.x version"),
         pytest.param("1.5.0", id="1.5.0 - some 1.5.x version"),
         pytest.param("1.6.0", id="1.6.0 - some 1.6.x version"),
         pytest.param("1.7.0", id="1.7.0 - some 1.7.x version"),
         pytest.param("1.8.0", id="1.8.0 - some 1.8.x version"),
         pytest.param("1.9.0", id="1.9.0 - some 1.9.x version"),
+        pytest.param("1.10.0", id="1.10.0 - some 1.10.x version"),
     ],
 )
 def test_initializes_for_supported_mypy_versions(version: str) -> None:
     # when
     _plugin = typing_protocol_intersection.mypy_plugin.plugin(version)
     # then no exception
```

### Comparing `typing-protocol-intersection-0.4.0/tests/test_python_module.py` & `typing_protocol_intersection-0.4.1/tests/test_python_module.py`

 * *Files identical despite different names*

### Comparing `typing-protocol-intersection-0.4.0/typing_protocol_intersection/mypy_plugin.py` & `typing_protocol_intersection-0.4.1/typing_protocol_intersection/mypy_plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
 
 
 def plugin(version: str) -> typing.Type[mypy.plugin.Plugin]:
     version_prefix, *_ = version.split("dev.", maxsplit=1)  # stripping +dev.f6a8037cc... suffix if applicable
     numeric_prefixes = (_numeric_prefix(x) for x in version_prefix.split("."))
     parted_version = tuple(int(prefix) if prefix else None for prefix in numeric_prefixes)
     if (len(parted_version) == 2 and (0, 920) <= parted_version <= (0, 991)) or (
-        len(parted_version) == 3 and (1, 0, 0) <= parted_version < (1, 10, 0)
+        len(parted_version) == 3 and (1, 0, 0) <= parted_version < (1, 11, 0)
     ):
         return ProtocolIntersectionPlugin
 
     raise NotImplementedError(f"typing-protocol-intersection does not support mypy=={version}")
 
 
 def _numeric_prefix(string: str) -> Optional[str]:
```

### Comparing `typing-protocol-intersection-0.4.0/typing_protocol_intersection/types.py` & `typing_protocol_intersection-0.4.1/typing_protocol_intersection/types.py`

 * *Files identical despite different names*

### Comparing `typing-protocol-intersection-0.4.0/typing_protocol_intersection.egg-info/PKG-INFO` & `typing_protocol_intersection-0.4.1/typing_protocol_intersection.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typing-protocol-intersection
-Version: 0.4.0
+Version: 0.4.1
 Summary: Protocol intersection for mypy
 Home-page: https://github.com/klausweiss/typing-protocol-intersection
 Project-URL: Bug Tracker, https://github.com/klausweiss/typing-protocol-intersection/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -27,15 +27,15 @@
 The `ProtocolIntersection` type tells mypy that an object implements multiple protocols.
 It can be used either as a function parameter or as a return value.
 A mypy plugin that ships with the package is required for this to work.
 See the [examples](#examples) section below.
 
 ## Supported versions
 
-The plugin supports python 3.8 up to 3.12 and mypy >= 0.920 and <= 1.9.x.
+The plugin supports python 3.8 up to 3.12 and mypy >= 0.920 and <= 1.10.x.
 
 ## Installation
 
 The `typing-protocol-intersection` package is pip-installable:
 
 ```shell
 pip install typing-protocol-intersection
```

