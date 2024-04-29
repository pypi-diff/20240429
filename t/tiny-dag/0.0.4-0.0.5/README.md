# Comparing `tmp/tiny_dag-0.0.4.tar.gz` & `tmp/tiny_dag-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiny_dag-0.0.4.tar", last modified: Sun Apr 28 07:11:23 2024, max compression
+gzip compressed data, was "tiny_dag-0.0.5.tar", last modified: Mon Apr 29 14:49:54 2024, max compression
```

## Comparing `tiny_dag-0.0.4.tar` & `tiny_dag-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-28 07:11:23.941379 tiny_dag-0.0.4/
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     1072 2024-04-27 07:53:55.000000 tiny_dag-0.0.4/LICENSE
--rw-r--r--   0 ossi      (1000) ossi      (1000)     1373 2024-04-28 07:11:23.941379 tiny_dag-0.0.4/PKG-INFO
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      835 2024-04-27 14:12:21.000000 tiny_dag-0.0.4/README.md
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      104 2024-04-27 09:26:48.000000 tiny_dag-0.0.4/pyproject.toml
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      668 2024-04-28 07:11:23.941379 tiny_dag-0.0.4/setup.cfg
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-28 07:11:23.937379 tiny_dag-0.0.4/src/
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-28 07:11:23.941379 tiny_dag-0.0.4/src/tiny_dag.egg-info/
--rw-r--r--   0 ossi      (1000) ossi      (1000)     1373 2024-04-28 07:11:23.000000 tiny_dag-0.0.4/src/tiny_dag.egg-info/PKG-INFO
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      286 2024-04-28 07:11:23.000000 tiny_dag-0.0.4/src/tiny_dag.egg-info/SOURCES.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        1 2024-04-28 07:11:23.000000 tiny_dag-0.0.4/src/tiny_dag.egg-info/dependency_links.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        9 2024-04-28 07:11:23.000000 tiny_dag-0.0.4/src/tiny_dag.egg-info/requires.txt
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        8 2024-04-28 07:11:23.000000 tiny_dag-0.0.4/src/tiny_dag.egg-info/top_level.txt
-drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-28 07:11:23.941379 tiny_dag-0.0.4/src/tinydag/
--rw-rw-r--   0 ossi      (1000) ossi      (1000)        0 2024-04-27 07:53:55.000000 tiny_dag-0.0.4/src/tinydag/__init__.py
--rw-rw-r--   0 ossi      (1000) ossi      (1000)     6340 2024-04-28 07:07:16.000000 tiny_dag-0.0.4/src/tinydag/graph.py
--rw-rw-r--   0 ossi      (1000) ossi      (1000)      711 2024-04-27 07:53:55.000000 tiny_dag-0.0.4/src/tinydag/node.py
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-29 14:49:54.770158 tiny_dag-0.0.5/
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     1072 2024-04-27 07:53:55.000000 tiny_dag-0.0.5/LICENSE
+-rw-r--r--   0 ossi      (1000) ossi      (1000)     1638 2024-04-29 14:49:54.770158 tiny_dag-0.0.5/PKG-INFO
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     1100 2024-04-29 14:48:03.000000 tiny_dag-0.0.5/README.md
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      104 2024-04-27 09:26:48.000000 tiny_dag-0.0.5/pyproject.toml
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      668 2024-04-29 14:49:54.774158 tiny_dag-0.0.5/setup.cfg
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-29 14:49:54.766158 tiny_dag-0.0.5/src/
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-29 14:49:54.770158 tiny_dag-0.0.5/src/tiny_dag.egg-info/
+-rw-r--r--   0 ossi      (1000) ossi      (1000)     1638 2024-04-29 14:49:54.000000 tiny_dag-0.0.5/src/tiny_dag.egg-info/PKG-INFO
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      286 2024-04-29 14:49:54.000000 tiny_dag-0.0.5/src/tiny_dag.egg-info/SOURCES.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        1 2024-04-29 14:49:54.000000 tiny_dag-0.0.5/src/tiny_dag.egg-info/dependency_links.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        9 2024-04-29 14:49:54.000000 tiny_dag-0.0.5/src/tiny_dag.egg-info/requires.txt
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        8 2024-04-29 14:49:54.000000 tiny_dag-0.0.5/src/tiny_dag.egg-info/top_level.txt
+drwxrwxr-x   0 ossi      (1000) ossi      (1000)        0 2024-04-29 14:49:54.770158 tiny_dag-0.0.5/src/tinydag/
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)        0 2024-04-27 07:53:55.000000 tiny_dag-0.0.5/src/tinydag/__init__.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)     6500 2024-04-29 14:42:23.000000 tiny_dag-0.0.5/src/tinydag/graph.py
+-rw-rw-r--   0 ossi      (1000) ossi      (1000)      711 2024-04-27 07:53:55.000000 tiny_dag-0.0.5/src/tinydag/node.py
```

### Comparing `tiny_dag-0.0.4/LICENSE` & `tiny_dag-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tiny_dag-0.0.4/PKG-INFO` & `tiny_dag-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny-dag
-Version: 0.0.4
+Version: 0.0.5
 Summary: Minimal DAG implementation with Python
 Home-page: https://github.com/omyllymaki/tiny-dag
 Author: Ossi Myllymäki
 Author-email: omyllymaki@gmail.com
 Project-URL: Bug Tracker, https://github.com/omyllymaki/tiny-dag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,17 @@
 License-File: LICENSE
 Requires-Dist: graphviz
 
 # Tiny DAG
 
 Bare bones implementation of computation (directed, acyclic) graph for Python.
 
+User provides graph structure (nodes) and input data for graph. Graph executes every node in graph and returns output 
+of every node as the result.
+
 # Requirements
 
 - Python >= 3.6
 - graphviz (optional)
 
 # Installation
 
@@ -53,11 +56,15 @@
 ]
 graph = Graph(nodes)
 graph.render()
 data = {"x": 5, "y": 3, "z": 3}
 results = graph.calculate(data)
 ```
 
+The results is dict of node outputs, in this case:
+
+{'add1': 8, 'add2': 13, 'mul': 104, 'div': 34.666666666666664}
+
 render method produces following figure:
 <p align="center">
 <img src="sample_graph.jpg" width="800px" />
 </p>
```

### Comparing `tiny_dag-0.0.4/README.md` & `tiny_dag-0.0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Tiny DAG
 
 Bare bones implementation of computation (directed, acyclic) graph for Python.
 
+User provides graph structure (nodes) and input data for graph. Graph executes every node in graph and returns output 
+of every node as the result.
+
 # Requirements
 
 - Python >= 3.6
 - graphviz (optional)
 
 # Installation
 
@@ -37,11 +40,15 @@
 ]
 graph = Graph(nodes)
 graph.render()
 data = {"x": 5, "y": 3, "z": 3}
 results = graph.calculate(data)
 ```
 
+The results is dict of node outputs, in this case:
+
+{'add1': 8, 'add2': 13, 'mul': 104, 'div': 34.666666666666664}
+
 render method produces following figure:
 <p align="center">
 <img src="sample_graph.jpg" width="800px" />
 </p>
```

### Comparing `tiny_dag-0.0.4/setup.cfg` & `tiny_dag-0.0.5/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tiny-dag
-version = 0.0.4
+version = 0.0.5
 author = Ossi Myllymäki
 author_email = omyllymaki@gmail.com
 description = Minimal DAG implementation with Python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/omyllymaki/tiny-dag
 project_urls =
```

### Comparing `tiny_dag-0.0.4/src/tiny_dag.egg-info/PKG-INFO` & `tiny_dag-0.0.5/src/tiny_dag.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiny-dag
-Version: 0.0.4
+Version: 0.0.5
 Summary: Minimal DAG implementation with Python
 Home-page: https://github.com/omyllymaki/tiny-dag
 Author: Ossi Myllymäki
 Author-email: omyllymaki@gmail.com
 Project-URL: Bug Tracker, https://github.com/omyllymaki/tiny-dag/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,17 @@
 License-File: LICENSE
 Requires-Dist: graphviz
 
 # Tiny DAG
 
 Bare bones implementation of computation (directed, acyclic) graph for Python.
 
+User provides graph structure (nodes) and input data for graph. Graph executes every node in graph and returns output 
+of every node as the result.
+
 # Requirements
 
 - Python >= 3.6
 - graphviz (optional)
 
 # Installation
 
@@ -53,11 +56,15 @@
 ]
 graph = Graph(nodes)
 graph.render()
 data = {"x": 5, "y": 3, "z": 3}
 results = graph.calculate(data)
 ```
 
+The results is dict of node outputs, in this case:
+
+{'add1': 8, 'add2': 13, 'mul': 104, 'div': 34.666666666666664}
+
 render method produces following figure:
 <p align="center">
 <img src="sample_graph.jpg" width="800px" />
 </p>
```

### Comparing `tiny_dag-0.0.4/src/tinydag/graph.py` & `tiny_dag-0.0.5/src/tinydag/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import time
 from copy import copy
-from typing import List, Callable, Union
+from typing import List, Callable, Union, Optional, Any
 
 from tinydag.node import Node
 
 logger = logging.getLogger(__name__)
 
 try:
     import graphviz as graphviz
@@ -24,15 +24,15 @@
 
     User provides graph structure (nodes) and input data for graph. Every node waits until input data for that node
     is ready. Eventually, graph executes every node in graph and returns output of every node as result.
     """
 
     def __init__(self,
                  nodes: List[Node],
-                 wrappers: List[Callable] = None):
+                 wrappers: Optional[List[Callable]] = None) -> None:
         """
         :param nodes: List of nodes.
         :param wrappers: Optional wrapper functions that will be used to wrap all functions in nodes.
 
         User needs to specify inputs, function and name for every node.
 
         Example:
@@ -60,15 +60,15 @@
 
         self._check_nodes(nodes)
         self.nodes = nodes
         self.wrappers = wrappers
 
     def render(self,
                path: str = "graph.gv",
-               view: bool = True) -> "Digraph":
+               view: bool = True) -> Optional["Digraph"]:
         """
         Render graph. This will only work if graphviz is available.
         :param path: Path to save fig.
         :param view: Show graph fig.
         :return: graphviz Digraph is graphviz is available, otherwise None.
         """
 
@@ -81,31 +81,31 @@
                     dot.edge(node_input, node.name)
             dot.render(path, view=view)
             return dot
         except Exception as e:
             logger.warning(f"Graph cannot be rendered, caught error: {e}")
             return None
 
-    def check(self, input_data: dict = None) -> None:
+    def check(self, input_data: Optional[dict] = None) -> None:
         """
         Check if graph can be executed. Raises Exception if graph is not valid.
 
         :param input_data: Input data for graph, where keys are names used in graph definition.
         """
         self._execute(input_data, False)
 
-    def calculate(self, input_data: dict = None) -> dict:
+    def calculate(self, input_data: Optional[dict] = None) -> dict:
         """
         Execute every node in graph.
         :param input_data: Input data for graph, where keys are names used in graph definition.
         :return: Output of every node, with node names as keys.
         """
         return self._execute(input_data)
 
-    def _execute(self, input_data: dict = None, run: bool = True) -> dict:
+    def _execute(self, input_data: Optional[dict] = None, run: Optional[bool] = True) -> dict:
         # Container where all the node outputs will be stored
         results = copy(input_data) if input_data is not None else {}
 
         nodes_to_execute = [i for i in range(len(self.nodes))]
         t_graph_start = time.time()
 
         # Loop until all nodes are executed
@@ -140,43 +140,43 @@
         # Remove inputs
         if input_data is not None:
             for key in input_data.keys():
                 results.pop(key)
 
         return results
 
-    def _run_node(self, node, data):
+    def _run_node(self, node: Node, data: list) -> Any:
         f = node.function
         if self.wrappers is not None:
             for wrapper in self.wrappers:
                 f = wrapper(f)
         t_node_start = time.time()
         output = f(*data)
         t_node_end = time.time()
         logger.debug(f"Node {node} execution took {1000 * (t_node_end - t_node_start): 0.3f} ms")
         return output
 
-    def __add__(self, nodes: Union[List[Node], Node]):
+    def __add__(self, nodes: Union[List[Node], Node]) -> "Graph":
         if isinstance(nodes, list):
             nodes = self.nodes + nodes
         else:
             nodes = self.nodes + [nodes]
         return Graph(nodes, self.wrappers)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return str([n.name for n in self.nodes])
 
     @staticmethod
-    def _check_nodes(nodes):
+    def _check_nodes(nodes: List[Node]) -> None:
         node_names = [n.name for n in nodes]
         if len(set(node_names)) < len(node_names):
             raise GraphError("All the nodes need to have unique name!")
 
     @staticmethod
-    def _get_input_data(node, results):
+    def _get_input_data(node: Node, results: dict) -> list:
         input_data = []
         for i in node.inputs:
             val = results.get(i, None)
             if val is None:
                 logger.debug(f"Cannot find input {i} for node {node}.")
                 break
             else:
```

### Comparing `tiny_dag-0.0.4/src/tinydag/node.py` & `tiny_dag-0.0.5/src/tinydag/node.py`

 * *Files identical despite different names*

