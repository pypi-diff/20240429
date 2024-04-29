# Comparing `tmp/issx-0.5.2.tar.gz` & `tmp/issx-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issx-0.5.2.tar", max compression
+gzip compressed data, was "issx-0.5.3.tar", max compression
```

## Comparing `issx-0.5.2.tar` & `issx-0.5.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1101 2024-04-29 13:08:17.527934 issx-0.5.2/LICENCE
--rw-r--r--   0        0        0     6557 2024-04-29 13:08:17.527934 issx-0.5.2/README.md
--rw-r--r--   0        0        0     3535 2024-04-29 13:08:17.527934 issx-0.5.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-29 13:08:17.527934 issx-0.5.2/src/issx/__init__.py
--rw-r--r--   0        0        0     6722 2024-04-29 13:08:17.527934 issx-0.5.2/src/issx/cli.py
--rw-r--r--   0        0        0     1126 2024-04-29 13:08:17.527934 issx-0.5.2/src/issx/cli_utils.py
--rw-r--r--   0        0        0      137 2024-04-29 13:08:17.527934 issx-0.5.2/src/issx/clients/__init__.py
--rw-r--r--   0        0        0      317 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/clients/exceptions.py
--rw-r--r--   0        0        0     4008 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/clients/gitlab.py
--rw-r--r--   0        0        0     3258 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/clients/interfaces.py
--rw-r--r--   0        0        0     3857 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/clients/redmine.py
--rw-r--r--   0        0        0      106 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/domain/__init__.py
--rw-r--r--   0        0        0     1707 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/domain/config.py
--rw-r--r--   0        0        0      205 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/domain/issues.py
--rw-r--r--   0        0        0        0 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/instance_managers/__init__.py
--rw-r--r--   0        0        0     2420 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/instance_managers/config_parser.py
--rw-r--r--   0        0        0     2557 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/instance_managers/managers.py
--rw-r--r--   0        0        0        0 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/py.typed
--rw-r--r--   0        0        0     2360 2024-04-29 13:08:17.531934 issx-0.5.2/src/issx/services.py
--rw-r--r--   0        0        0     7617 1970-01-01 00:00:00.000000 issx-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1101 2024-04-29 13:19:18.531575 issx-0.5.3/LICENCE
+-rw-r--r--   0        0        0     6557 2024-04-29 13:19:18.531575 issx-0.5.3/README.md
+-rw-r--r--   0        0        0     3535 2024-04-29 13:19:18.531575 issx-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-29 13:19:18.531575 issx-0.5.3/src/issx/__init__.py
+-rw-r--r--   0        0        0     6680 2024-04-29 13:19:18.531575 issx-0.5.3/src/issx/cli.py
+-rw-r--r--   0        0        0     1126 2024-04-29 13:19:18.531575 issx-0.5.3/src/issx/cli_utils.py
+-rw-r--r--   0        0        0      137 2024-04-29 13:19:18.531575 issx-0.5.3/src/issx/clients/__init__.py
+-rw-r--r--   0        0        0      317 2024-04-29 13:19:18.531575 issx-0.5.3/src/issx/clients/exceptions.py
+-rw-r--r--   0        0        0     4008 2024-04-29 13:19:18.535575 issx-0.5.3/src/issx/clients/gitlab.py
+-rw-r--r--   0        0        0     3258 2024-04-29 13:19:18.535575 issx-0.5.3/src/issx/clients/interfaces.py
+-rw-r--r--   0        0        0     3857 2024-04-29 13:19:18.535575 issx-0.5.3/src/issx/clients/redmine.py
+-rw-r--r--   0        0        0      106 2024-04-29 13:19:18.535575 issx-0.5.3/src/issx/domain/__init__.py
+-rw-r--r--   0        0        0     1707 2024-04-29 13:19:18.535575 issx-0.5.3/src/issx/domain/config.py
+-rw-r--r--   0        0        0      205 2024-04-29 13:19:18.535575 issx-0.5.3/src/issx/domain/issues.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:19:18.535575 issx-0.5.3/src/issx/instance_managers/__init__.py
+-rw-r--r--   0        0        0     2420 2024-04-29 13:19:18.535575 issx-0.5.3/src/issx/instance_managers/config_parser.py
+-rw-r--r--   0        0        0     2557 2024-04-29 13:19:18.535575 issx-0.5.3/src/issx/instance_managers/managers.py
+-rw-r--r--   0        0        0        0 2024-04-29 13:19:18.535575 issx-0.5.3/src/issx/py.typed
+-rw-r--r--   0        0        0     2360 2024-04-29 13:19:18.535575 issx-0.5.3/src/issx/services.py
+-rw-r--r--   0        0        0     7617 1970-01-01 00:00:00.000000 issx-0.5.3/PKG-INFO
```

### Comparing `issx-0.5.2/LICENCE` & `issx-0.5.3/LICENCE`

 * *Files identical despite different names*

### Comparing `issx-0.5.2/README.md` & `issx-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `issx-0.5.2/pyproject.toml` & `issx-0.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "issx"
-version = "0.5.2"
+version = "0.5.3"
 description = "Tool for synchronizing issues between different services"
 authors = [
     "nekeal <szymon.sc.cader@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `issx-0.5.2/src/issx/cli.py` & `issx-0.5.3/src/issx/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 from typing import Annotated
 
 import typer
 from rich.console import Console
-from rich.syntax import Syntax
 from rich.text import Text
 
 from issx.cli_utils import RichConfigReader
 from issx.clients.gitlab import GitlabClient, GitlabInstanceClient
 from issx.clients.redmine import RedmineClient, RedmineInstanceClient
 from issx.domain import SupportedBackend
 from issx.domain.config import InstanceConfig, ProjectFlatConfig
@@ -161,15 +160,15 @@
         ),
     ],
 ) -> None:
     """Generate instance's new_config string"""
 
     new_config = RichConfigReader().read(InstanceConfig)
     console.print()
-    console.print(Syntax(new_config.as_toml(f"instances.{instance_name}"), "toml"))
+    console.print(Text(new_config.as_toml(f"projects.{instance_name}")))
 
     console.print(
         "\nSuccess!\nCopy the above config to your config file", style="green"
     )
 
 
 @config_app.command()
```

### Comparing `issx-0.5.2/src/issx/cli_utils.py` & `issx-0.5.3/src/issx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.2/src/issx/clients/gitlab.py` & `issx-0.5.3/src/issx/clients/gitlab.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.2/src/issx/clients/interfaces.py` & `issx-0.5.3/src/issx/clients/interfaces.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.2/src/issx/clients/redmine.py` & `issx-0.5.3/src/issx/clients/redmine.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.2/src/issx/domain/config.py` & `issx-0.5.3/src/issx/domain/config.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.2/src/issx/instance_managers/config_parser.py` & `issx-0.5.3/src/issx/instance_managers/config_parser.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.2/src/issx/instance_managers/managers.py` & `issx-0.5.3/src/issx/instance_managers/managers.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.2/src/issx/services.py` & `issx-0.5.3/src/issx/services.py`

 * *Files identical despite different names*

### Comparing `issx-0.5.2/PKG-INFO` & `issx-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issx
-Version: 0.5.2
+Version: 0.5.3
 Summary: Tool for synchronizing issues between different services
 Home-page: https://nekeal.github.io/issx
 License: MIT
 Author: nekeal
 Author-email: szymon.sc.cader@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

