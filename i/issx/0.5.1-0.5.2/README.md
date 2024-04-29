# Comparing `tmp/issx-0.5.1.tar.gz` & `tmp/issx-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issx-0.5.1.tar", max compression
+gzip compressed data, was "issx-0.5.2.tar", max compression
```

## Comparing `issx-0.5.1.tar` & `issx-0.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1101 2024-04-29 12:54:24.334131 issx-0.5.1/LICENCE
--rw-r--r--   0        0        0     6557 2024-04-29 12:54:24.334131 issx-0.5.1/README.md
--rw-r--r--   0        0        0     3535 2024-04-29 12:54:24.338131 issx-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/__init__.py
--rw-r--r--   0        0        0     6722 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/cli.py
--rw-r--r--   0        0        0      994 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/cli_utils.py
--rw-r--r--   0        0        0      137 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/clients/__init__.py
--rw-r--r--   0        0        0      317 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/clients/exceptions.py
--rw-r--r--   0        0        0     4008 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/clients/gitlab.py
--rw-r--r--   0        0        0     3258 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/clients/interfaces.py
--rw-r--r--   0        0        0     3857 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/clients/redmine.py
--rw-r--r--   0        0        0      106 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/domain/__init__.py
--rw-r--r--   0        0        0     1707 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/domain/config.py
--rw-r--r--   0        0        0      205 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/domain/issues.py
--rw-r--r--   0        0        0        0 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/instance_managers/__init__.py
--rw-r--r--   0        0        0     2420 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/instance_managers/config_parser.py
--rw-r--r--   0        0        0     2557 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/instance_managers/managers.py
--rw-r--r--   0        0        0        0 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/py.typed
--rw-r--r--   0        0        0     2360 2024-04-29 12:54:24.338131 issx-0.5.1/src/issx/services.py
--rw-r--r--   0        0        0     7617 1970-01-01 00:00:00.000000 issx-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-29 13:08:17.527934 issx-0.5.2/LICENCE
+-rw-r--r--   0        0        0     6557 2024-04-29 13:08:17.527934 issx-0.5.2/README.md
+-rw-r--r--   0        0        0     3535 2024-04-29 13:08:17.527934 issx-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 13:08:17.527934 issx-0.5.2/src/issx/__init__.py
+-rw-r--r--   0        0        0     6722 2024-04-29 13:08:17.527934 issx-0.5.2/src/issx/cli.py
+-rw-r--r--   0        0        0     1126 2024-04-29 13:08:17.527934 issx-0.5.2/src/issx/cli_utils.py
+-rw-r--r--   0        0        0      137 2024-04-29 13:08:17.527934 issx-0.5.2/src/issx/clients/__init__.py
+-rw-r--r--   0        0        0      317 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/clients/exceptions.py
+-rw-r--r--   0        0        0     4008 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/clients/gitlab.py
+-rw-r--r--   0        0        0     3258 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/clients/interfaces.py
+-rw-r--r--   0        0        0     3857 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/clients/redmine.py
+-rw-r--r--   0        0        0      106 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/domain/__init__.py
+-rw-r--r--   0        0        0     1707 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/domain/config.py
+-rw-r--r--   0        0        0      205 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/domain/issues.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/instance_managers/__init__.py
+-rw-r--r--   0        0        0     2420 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/instance_managers/config_parser.py
+-rw-r--r--   0        0        0     2557 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/instance_managers/managers.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/py.typed
+-rw-r--r--   0        0        0     2360 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/services.py
+-rw-r--r--   0        0        0     7617 1970-01-01 00:00:00.000000 issx-0.5.2/PKG-INFO
```

### Comparing `issx-0.5.1/LICENCE` & `issx-0.5.2/LICENCE`

 * *Files identical despite different names*

### Comparing `issx-0.5.1/README.md` & `issx-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `issx-0.5.1/pyproject.toml` & `issx-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "issx"
-version = "0.5.1"
+version = "0.5.2"
 description = "Tool for synchronizing issues between different services"
 authors = [
     "nekeal <szymon.sc.cader@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `issx-0.5.1/src/issx/cli.py` & `issx-0.5.2/src/issx/cli.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.1/src/issx/cli_utils.py` & `issx-0.5.2/src/issx/cli_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,12 +24,15 @@
                 [str(v) for v in field.type.__members__.values()]
                 if issubclass(field.type, Enum)
                 else None
             )
             if field.type
             else None
         )
+        ask_kwargs = {}
+        if field.default:
+            ask_kwargs["default"] = str(field.default)
         return Prompt.ask(
             f"Enter [bold]{field.name}[/bold]",
-            default=str(field.default) if field.default else "",
+            default=str(field.default) if field.default else ...,  # type: ignore[arg-type]
             choices=choices,
         )
```

### Comparing `issx-0.5.1/src/issx/clients/gitlab.py` & `issx-0.5.2/src/issx/clients/gitlab.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.1/src/issx/clients/interfaces.py` & `issx-0.5.2/src/issx/clients/interfaces.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.1/src/issx/clients/redmine.py` & `issx-0.5.2/src/issx/clients/redmine.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.1/src/issx/domain/config.py` & `issx-0.5.2/src/issx/domain/config.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.1/src/issx/instance_managers/config_parser.py` & `issx-0.5.2/src/issx/instance_managers/config_parser.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.1/src/issx/instance_managers/managers.py` & `issx-0.5.2/src/issx/instance_managers/managers.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.1/src/issx/services.py` & `issx-0.5.2/src/issx/services.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.1/PKG-INFO` & `issx-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issx
-Version: 0.5.1
+Version: 0.5.2
 Summary: Tool for synchronizing issues between different services
 Home-page: https://nekeal.github.io/issx
 License: MIT
 Author: nekeal
 Author-email: szymon.sc.cader@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

