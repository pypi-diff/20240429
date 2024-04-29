# Comparing `tmp/nestipy_ioc-0.1.30.tar.gz` & `tmp/nestipy_ioc-0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_ioc-0.1.30.tar", max compression
+gzip compressed data, was "nestipy_ioc-0.1.31.tar", max compression
```

## Comparing `nestipy_ioc-0.1.30.tar` & `nestipy_ioc-0.1.31.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2024-04-22 13:24:07.751008 nestipy_ioc-0.1.30/README.md
--rw-r--r--   0        0        0      374 2024-04-24 07:46:50.671389 nestipy_ioc-0.1.30/pyproject.toml
--rw-r--r--   0        0        0      774 2024-04-24 06:53:58.268550 nestipy_ioc-0.1.30/src/nestipy_ioc/__init__.py
--rw-r--r--   0        0        0      122 2024-04-22 14:21:10.410610 nestipy_ioc-0.1.30/src/nestipy_ioc/annotation.py
--rw-r--r--   0        0        0    12449 2024-04-23 11:57:44.650683 nestipy_ioc-0.1.30/src/nestipy_ioc/container.py
--rw-r--r--   0        0        0     1440 2024-04-22 13:59:48.684851 nestipy_ioc-0.1.30/src/nestipy_ioc/context_container.py
--rw-r--r--   0        0        0     1701 2024-04-23 15:29:10.758786 nestipy_ioc-0.1.30/src/nestipy_ioc/dependency.py
--rw-r--r--   0        0        0      885 2024-04-22 14:30:34.353131 nestipy_ioc-0.1.30/src/nestipy_ioc/meta.py
--rw-r--r--   0        0        0     3013 2024-04-24 07:40:20.664817 nestipy_ioc-0.1.30/src/nestipy_ioc/middleware.py
--rw-r--r--   0        0        0      877 2024-04-22 14:22:54.695299 nestipy_ioc-0.1.30/src/nestipy_ioc/provider.py
--rw-r--r--   0        0        0       56 2024-04-22 13:59:03.116828 nestipy_ioc-0.1.30/src/nestipy_ioc/utils.py
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 nestipy_ioc-0.1.30/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-22 13:24:07.751008 nestipy_ioc-0.1.31/README.md
+-rw-r--r--   0        0        0      373 2024-04-29 13:15:27.470532 nestipy_ioc-0.1.31/pyproject.toml
+-rw-r--r--   0        0        0      774 2024-04-24 06:53:58.268550 nestipy_ioc-0.1.31/src/nestipy_ioc/__init__.py
+-rw-r--r--   0        0        0      122 2024-04-22 14:21:10.410610 nestipy_ioc-0.1.31/src/nestipy_ioc/annotation.py
+-rw-r--r--   0        0        0    12493 2024-04-29 13:12:56.485255 nestipy_ioc-0.1.31/src/nestipy_ioc/container.py
+-rw-r--r--   0        0        0     1440 2024-04-22 13:59:48.684851 nestipy_ioc-0.1.31/src/nestipy_ioc/context_container.py
+-rw-r--r--   0        0        0     1701 2024-04-23 15:29:10.758786 nestipy_ioc-0.1.31/src/nestipy_ioc/dependency.py
+-rw-r--r--   0        0        0      885 2024-04-22 14:30:34.353131 nestipy_ioc-0.1.31/src/nestipy_ioc/meta.py
+-rw-r--r--   0        0        0     3013 2024-04-24 07:40:20.664817 nestipy_ioc-0.1.31/src/nestipy_ioc/middleware.py
+-rw-r--r--   0        0        0      877 2024-04-22 14:22:54.695299 nestipy_ioc-0.1.31/src/nestipy_ioc/provider.py
+-rw-r--r--   0        0        0       56 2024-04-22 13:59:03.116828 nestipy_ioc-0.1.31/src/nestipy_ioc/utils.py
+-rw-r--r--   0        0        0      477 1970-01-01 00:00:00.000000 nestipy_ioc-0.1.31/PKG-INFO
```

### Comparing `nestipy_ioc-0.1.30/src/nestipy_ioc/__init__.py` & `nestipy_ioc-0.1.31/src/nestipy_ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.30/src/nestipy_ioc/container.py` & `nestipy_ioc-0.1.31/src/nestipy_ioc/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 
     async def _get_method_dependency(self, method_to_resolve: Callable, search_scope: list, origin: list):
         params = inspect.signature(method_to_resolve).parameters
         args = {}
         for name, param in params.items():
             if name != 'self' and param.annotation is not inspect.Parameter.empty:
                 annotation, dep_key = self.helper.get_type_from_annotation(param.annotation)
-                if dep_key.metadata is not CtxDepKey.Service:
+                if dep_key.metadata in CtxDepKey.to_list() and dep_key.metadata is not CtxDepKey.Service:
                     dependency = self._resolve_context_service(name, dep_key.metadata, annotation)
                     args[name] = dependency
                 elif annotation in search_scope:
                     dependency = await self.get(annotation, origin=origin)
                     args[name] = dependency
                 else:
                     _name: str = annotation.__name__ if not isinstance(annotation, str) else annotation
```

### Comparing `nestipy_ioc-0.1.30/src/nestipy_ioc/context_container.py` & `nestipy_ioc-0.1.31/src/nestipy_ioc/context_container.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.30/src/nestipy_ioc/dependency.py` & `nestipy_ioc-0.1.31/src/nestipy_ioc/dependency.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.30/src/nestipy_ioc/meta.py` & `nestipy_ioc-0.1.31/src/nestipy_ioc/meta.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.30/src/nestipy_ioc/middleware.py` & `nestipy_ioc-0.1.31/src/nestipy_ioc/middleware.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.30/src/nestipy_ioc/provider.py` & `nestipy_ioc-0.1.31/src/nestipy_ioc/provider.py`

 * *Files identical despite different names*

