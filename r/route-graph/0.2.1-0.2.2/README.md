# Comparing `tmp/route_graph-0.2.1.tar.gz` & `tmp/route_graph-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "route_graph-0.2.1.tar", max compression
+gzip compressed data, was "route_graph-0.2.2.tar", max compression
```

## Comparing `route_graph-0.2.1.tar` & `route_graph-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1068 2024-03-13 19:42:03.922331 route_graph-0.2.1/LICENSE
--rw-r--r--   0        0        0     3691 2024-03-13 19:42:03.922331 route_graph-0.2.1/README.md
--rw-r--r--   0        0        0      638 2024-03-13 19:42:22.353130 route_graph-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       50 2024-03-12 18:08:17.700914 route_graph-0.2.1/route_graph/__init__.py
--rw-r--r--   0        0        0       89 2024-03-12 22:17:46.081869 route_graph-0.2.1/route_graph/exceptions.py
--rw-r--r--   0        0        0     1425 2024-03-13 20:03:45.193194 route_graph-0.2.1/route_graph/main.py
--rw-r--r--   0        0        0     4475 1970-01-01 00:00:00.000000 route_graph-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-13 19:42:03.922331 route_graph-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3691 2024-03-13 19:42:03.922331 route_graph-0.2.2/README.md
+-rw-r--r--   0        0        0      671 2024-04-29 06:52:29.019401 route_graph-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       50 2024-03-12 18:08:17.700914 route_graph-0.2.2/route_graph/__init__.py
+-rw-r--r--   0        0        0       89 2024-03-12 22:17:46.081869 route_graph-0.2.2/route_graph/exceptions.py
+-rw-r--r--   0        0        0     1425 2024-03-13 20:03:45.193194 route_graph-0.2.2/route_graph/main.py
+-rw-r--r--   0        0        0     4467 1970-01-01 00:00:00.000000 route_graph-0.2.2/PKG-INFO
```

### Comparing `route_graph-0.2.1/LICENSE` & `route_graph-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `route_graph-0.2.1/README.md` & `route_graph-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `route_graph-0.2.1/pyproject.toml` & `route_graph-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [tool.poetry]
 name = "route-graph"
-version = "0.2.1"
+version = "0.2.2"
 description = "Tool for creating graphs of routes"
 authors = ["Fabian Affolter <mail@fabian-affolter.ch>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["traceroute", "graph", "routes"]
 homepage = "https://github.com/audiusGmbH/route-graph"
 repository = "https://github.com/audiusGmbH/route-graph"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-typer = {extras = ["all"], version = "^0.9.0"}
+typer = "^0.12"
 scapy = "^2.5.0"
 typing-extensions = "^4.10.0"
 
+[tool.poetry.dev-dependencies]
+black = "^24.3"
+isort = "^5.13"
+
 [tool.poetry.scripts]
 route-graph = "route_graph.main:app"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `route_graph-0.2.1/route_graph/main.py` & `route_graph-0.2.2/route_graph/main.py`

 * *Files identical despite different names*

### Comparing `route_graph-0.2.1/PKG-INFO` & `route_graph-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: route-graph
-Version: 0.2.1
+Version: 0.2.2
 Summary: Tool for creating graphs of routes
 Home-page: https://github.com/audiusGmbH/route-graph
 License: MIT
 Keywords: traceroute,graph,routes
 Author: Fabian Affolter
 Author-email: mail@fabian-affolter.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: scapy (>=2.5.0,<3.0.0)
-Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.12,<0.13)
 Requires-Dist: typing-extensions (>=4.10.0,<5.0.0)
 Project-URL: Repository, https://github.com/audiusGmbH/route-graph
 Description-Content-Type: text/markdown
 
 # route-graph
 
 CLI tool for creating graphs of routes.
```

