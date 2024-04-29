# Comparing `tmp/dataclasses_json-0.6.3.tar.gz` & `tmp/dataclasses_json-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclasses_json-0.6.3.tar", max compression
+gzip compressed data, was "dataclasses_json-0.6.4.tar", max compression
```

## Comparing `dataclasses_json-0.6.3.tar` & `dataclasses_json-0.6.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1084 2023-11-27 19:47:58.516156 dataclasses_json-0.6.3/LICENSE
--rw-r--r--   0        0        0    23874 2023-11-27 19:47:58.516156 dataclasses_json-0.6.3/README.md
--rw-r--r--   0        0        0      495 2023-11-27 19:47:58.516156 dataclasses_json-0.6.3/dataclasses_json/__init__.py
--rw-r--r--   0        0        0      154 2023-11-27 19:48:14.628069 dataclasses_json-0.6.3/dataclasses_json/__version__.py
--rw-r--r--   0        0        0     5990 2023-11-27 19:47:58.516156 dataclasses_json-0.6.3/dataclasses_json/api.py
--rw-r--r--   0        0        0     3527 2023-11-27 19:47:58.516156 dataclasses_json-0.6.3/dataclasses_json/cfg.py
--rw-r--r--   0        0        0    17871 2023-11-27 19:47:58.516156 dataclasses_json-0.6.3/dataclasses_json/core.py
--rw-r--r--   0        0        0    15997 2023-11-27 19:47:58.516156 dataclasses_json-0.6.3/dataclasses_json/mm.py
--rw-r--r--   0        0        0        0 2023-11-27 19:47:58.516156 dataclasses_json-0.6.3/dataclasses_json/py.typed
--rw-r--r--   0        0        0     3313 2023-11-27 19:47:58.516156 dataclasses_json-0.6.3/dataclasses_json/stringcase.py
--rw-r--r--   0        0        0    10452 2023-11-27 19:47:58.516156 dataclasses_json-0.6.3/dataclasses_json/undefined.py
--rw-r--r--   0        0        0     5714 2023-11-27 19:47:58.516156 dataclasses_json-0.6.3/dataclasses_json/utils.py
--rw-r--r--   0        0        0     1147 2023-11-27 19:48:14.628069 dataclasses_json-0.6.3/pyproject.toml
--rw-r--r--   0        0        0    25035 1970-01-01 00:00:00.000000 dataclasses_json-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-02-01 20:31:14.479021 dataclasses_json-0.6.4/LICENSE
+-rw-r--r--   0        0        0    23874 2024-02-01 20:31:14.483021 dataclasses_json-0.6.4/README.md
+-rw-r--r--   0        0        0      495 2024-02-01 20:31:14.483021 dataclasses_json-0.6.4/dataclasses_json/__init__.py
+-rw-r--r--   0        0        0      154 2024-02-01 20:31:31.823006 dataclasses_json-0.6.4/dataclasses_json/__version__.py
+-rw-r--r--   0        0        0     5990 2024-02-01 20:31:14.483021 dataclasses_json-0.6.4/dataclasses_json/api.py
+-rw-r--r--   0        0        0     3527 2024-02-01 20:31:14.483021 dataclasses_json-0.6.4/dataclasses_json/cfg.py
+-rw-r--r--   0        0        0    17887 2024-02-01 20:31:14.483021 dataclasses_json-0.6.4/dataclasses_json/core.py
+-rw-r--r--   0        0        0    15997 2024-02-01 20:31:14.483021 dataclasses_json-0.6.4/dataclasses_json/mm.py
+-rw-r--r--   0        0        0        0 2024-02-01 20:31:14.483021 dataclasses_json-0.6.4/dataclasses_json/py.typed
+-rw-r--r--   0        0        0     3313 2024-02-01 20:31:14.483021 dataclasses_json-0.6.4/dataclasses_json/stringcase.py
+-rw-r--r--   0        0        0    10452 2024-02-01 20:31:14.483021 dataclasses_json-0.6.4/dataclasses_json/undefined.py
+-rw-r--r--   0        0        0     5714 2024-02-01 20:31:14.483021 dataclasses_json-0.6.4/dataclasses_json/utils.py
+-rw-r--r--   0        0        0     1147 2024-02-01 20:31:31.823006 dataclasses_json-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0    25035 1970-01-01 00:00:00.000000 dataclasses_json-0.6.4/PKG-INFO
```

### Comparing `dataclasses_json-0.6.3/LICENSE` & `dataclasses_json-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.3/README.md` & `dataclasses_json-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.3/dataclasses_json/api.py` & `dataclasses_json-0.6.4/dataclasses_json/api.py`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.3/dataclasses_json/cfg.py` & `dataclasses_json-0.6.4/dataclasses_json/cfg.py`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.3/dataclasses_json/core.py` & `dataclasses_json-0.6.4/dataclasses_json/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
             res = value  # assume already decoded
             if type(value) is dict and dict not in type_options:
                 for type_option in type_options:
                     if is_dataclass(type_option):
                         try:
                             res = _decode_dataclass(type_option, value, infer_missing)
                             break
-                        except (KeyError, ValueError):
+                        except (KeyError, ValueError, AttributeError):
                             continue
                 if res == value:
                     warnings.warn(
                         f"Failed to decode {value} Union dataclasses."
                         f"Expected Union to include a matching dataclass and it didn't."
                     )
     return res
```

### Comparing `dataclasses_json-0.6.3/dataclasses_json/mm.py` & `dataclasses_json-0.6.4/dataclasses_json/mm.py`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.3/dataclasses_json/stringcase.py` & `dataclasses_json-0.6.4/dataclasses_json/stringcase.py`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.3/dataclasses_json/undefined.py` & `dataclasses_json-0.6.4/dataclasses_json/undefined.py`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.3/dataclasses_json/utils.py` & `dataclasses_json-0.6.4/dataclasses_json/utils.py`

 * *Files identical despite different names*

### Comparing `dataclasses_json-0.6.3/pyproject.toml` & `dataclasses_json-0.6.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclasses-json"
-version = "0.6.3"
+version = "0.6.4"
 description = "Easily serialize dataclasses to and from JSON."
 authors = ["Charles Li <charles.dt.li@gmail.com>"]
 maintainers = ['Charles Li <charles.dt.li@gmail.com>', 'Georgiy Zubrienko <gzu@ecco.com>', 'Vitaliy Savitskiy <visa@ecco.com>', 'Matthias Als <mata@ecco.com>']
 license = 'MIT'
 readme = "README.md"
 repository = 'https://github.com/lidatong/dataclasses-json'
```

### Comparing `dataclasses_json-0.6.3/PKG-INFO` & `dataclasses_json-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclasses-json
-Version: 0.6.3
+Version: 0.6.4
 Summary: Easily serialize dataclasses to and from JSON.
 Home-page: https://github.com/lidatong/dataclasses-json
 License: MIT
 Author: Charles Li
 Author-email: charles.dt.li@gmail.com
 Maintainer: Charles Li
 Maintainer-email: charles.dt.li@gmail.com
```

