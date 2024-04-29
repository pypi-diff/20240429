# Comparing `tmp/modgeosys_graph_algorithms-0.3.9.tar.gz` & `tmp/modgeosys_graph_algorithms-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modgeosys_graph_algorithms-0.3.9.tar", max compression
+gzip compressed data, was "modgeosys_graph_algorithms-0.4.0.tar", max compression
```

## Comparing `modgeosys_graph_algorithms-0.3.9.tar` & `modgeosys_graph_algorithms-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4224 2024-04-28 17:48:48.450848 modgeosys_graph_algorithms-0.3.9/README.md
--rw-r--r--   0        0        0      489 2024-04-28 17:51:56.303357 modgeosys_graph_algorithms-0.3.9/pyproject.toml
--rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.3.9/src/modgeosys/__init__.py
--rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/__init__.py
--rw-r--r--   0        0        0     3229 2024-04-28 04:37:43.782725 modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/a_star.py
--rw-r--r--   0        0        0      625 2024-04-28 04:54:23.937487 modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/distance.py
--rw-r--r--   0        0        0      177 2024-04-28 17:43:46.457872 modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/edge_validation.py
--rw-r--r--   0        0        0      418 2024-04-28 05:11:58.328061 modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/edge_weight.py
--rw-r--r--   0        0        0     1696 2024-04-06 19:04:49.983022 modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/prim.py
--rw-r--r--   0        0        0     7804 2024-04-28 17:47:33.322604 modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/types.py
--rw-r--r--   0        0        0     4767 2024-04-28 16:28:12.634644 modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/conftest.py
--rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/generate_a_star_test_data.py
--rw-r--r--   0        0        0     8358 2024-04-27 21:40:29.497540 modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_a_star.py
--rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_distance.py
--rw-r--r--   0        0        0    24076 2024-04-27 21:40:29.505540 modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_prim.py
--rw-r--r--   0        0        0     3795 2024-04-28 04:46:03.711552 modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_types.py
--rw-r--r--   0        0        0     4609 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     4214 2024-04-29 04:40:54.037521 modgeosys_graph_algorithms-0.4.0/README.md
+-rw-r--r--   0        0        0      489 2024-04-29 21:38:44.805145 modgeosys_graph_algorithms-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.4.0/src/modgeosys/__init__.py
+-rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/__init__.py
+-rw-r--r--   0        0        0     3219 2024-04-29 04:36:13.020391 modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/a_star.py
+-rw-r--r--   0        0        0      625 2024-04-28 18:02:46.684609 modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/distance.py
+-rw-r--r--   0        0        0      177 2024-04-28 18:02:46.684609 modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/edge_validation.py
+-rw-r--r--   0        0        0      408 2024-04-29 04:36:13.064391 modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/edge_weight.py
+-rw-r--r--   0        0        0     1696 2024-04-06 19:04:49.983022 modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/prim.py
+-rw-r--r--   0        0        0     7744 2024-04-29 04:44:15.842283 modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/types.py
+-rw-r--r--   0        0        0     4727 2024-04-29 04:44:15.878284 modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/conftest.py
+-rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/generate_a_star_test_data.py
+-rw-r--r--   0        0        0     8338 2024-04-29 04:44:15.866284 modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_a_star.py
+-rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_distance.py
+-rw-r--r--   0        0        0    24076 2024-04-27 21:40:29.505540 modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_prim.py
+-rw-r--r--   0        0        0     3775 2024-04-29 04:36:13.028391 modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_types.py
+-rw-r--r--   0        0        0     4599 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.4.0/PKG-INFO
```

### Comparing `modgeosys_graph_algorithms-0.3.9/README.md` & `modgeosys_graph_algorithms-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                                                           (((0.0, 2.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 3}),
                                                           (((2.0, 1.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1})),
                                         distance_function=manhattan_distance, edge_weight_function=length_cost_per_unit)
 
 # Load a bigger graph from a pickle file.
 with open('python/data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
   larger_graph = pickle.load(pickled_sample_larger_graph_file)
-  larger_graph.heuristic_distance_function = manhattan_distance
+  larger_graph.distance_function = manhattan_distance
   larger_graph.edge_weight_function = length_cost_per_unit
 
 # Call the A* function.
 toy_a_star_path = a_star(graph=toy_graph, start_node_index=0, goal_node_index=4)
 print('Toy A* Path:')
 pprint(toy_a_star_path)
 print()
```

### Comparing `modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/a_star.py` & `modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/a_star.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 def a_star(graph: Graph, start_node_index: int, goal_node_index: int) -> list[Hop]:
     """Implement the A* algorithm for finding the shortest path between two nodes in a graph."""
 
     # Grab the nodes and adjacency map from the graph.
     nodes         = graph.nodes
     adjacency_map = graph.adjacency_map()
-    heuristic_distance = graph.heuristic_distance_function
+    heuristic_distance = graph.distance_function
     if not heuristic_distance:
         raise AttributeError('The graph must have a heuristic_distance property to use the A* algorithm.')
 
     # Initialize the edge hop lists.
     unhopped   = list(graph.edges)
     hops       = []
```

### Comparing `modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/distance.py` & `modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/prim.py` & `modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.9/src/modgeosys/graph/types.py` & `modgeosys_graph_algorithms-0.4.0/src/modgeosys/graph/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
 class Graph:
     """A graph."""
     nodes: NodeSequence = field(default_factory=list)
     edges: EdgeSequence = field(default_factory=tuple)
     properties: dict = field(default_factory=dict)
     edge_weight_function: EdgeWeightCallable | None
-    heuristic_distance_function: DistanceCallable | None
+    distance_function: DistanceCallable | None
 
     @classmethod
     def from_edge_definitions(cls, edge_definitions: EdgeDefinitionSequence, properties: dict | None = None, distance_function: DistanceCallable | None = None, edge_weight_function: EdgeWeightCallable | None = None) -> 'Graph':
         """Create a graph from a sequence of edge definitions."""
         coordinates_of_all_nodes = []
 
         for edge_definition in edge_definitions:
@@ -140,22 +140,22 @@
                 nodes[index] = Node(coordinates=edge_node_coordinates)
             node_indices = frozenset(indices)
             edge = Edge(weight=edge_definition[1], node_indices=node_indices, properties=edge_definition[2])
             edges.append(edge)
 
         nodes = [nodes[index] for index in sorted(nodes)]
 
-        return cls(nodes=nodes, edges=edges, properties=properties, edge_weight_function=edge_weight_function, heuristic_distance_function=distance_function)
+        return cls(nodes=nodes, edges=edges, properties=properties, edge_weight_function=edge_weight_function, distance_function=distance_function)
 
-    def __init__(self, nodes: NodeSequence, edges: EdgeSequence, properties: dict | None = None, edge_weight_function: EdgeWeightCallable | None = None, heuristic_distance_function: DistanceCallable | None = None):
+    def __init__(self, nodes: NodeSequence, edges: EdgeSequence, properties: dict | None = None, edge_weight_function: EdgeWeightCallable | None = None, distance_function: DistanceCallable | None = None):
         """Initialize a graph."""
         self.nodes = deepcopy(nodes)
         self.edges = tuple(deepcopy(edge) for edge in edges)
         self.properties = {} if properties is None else (deepcopy(properties) if isinstance(properties, dict) else dict(properties))
-        self.heuristic_distance_function = heuristic_distance_function if heuristic_distance_function else None
+        self.distance_function = distance_function if distance_function else None
         if edge_weight_function:
             self.edge_weight_function = edge_weight_function
             for edge in self.edges:
                 edge.weight = self.edge_weight_function(self, edge)
         else:
             self.edge_weight_function = specified_edge_weight
```

### Comparing `modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/conftest.py` & `modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,25 +54,25 @@
             Edge(properties={'cost_per_unit': 1}, weight=2.0, node_indices=frozenset((2, 3))),
             Edge(properties={'cost_per_unit': 3}, weight=9.0, node_indices=frozenset((1, 4))),
             Edge(properties={'cost_per_unit': 1}, weight=2.0, node_indices=frozenset((3, 4))))
 
 
 @pytest.fixture
 def valid_graph1(valid_nodes, valid_edges1):
-    return Graph(properties={}, nodes=valid_nodes, edges=valid_edges1, heuristic_distance_function=manhattan_distance)
+    return Graph(properties={}, nodes=valid_nodes, edges=valid_edges1, distance_function=manhattan_distance)
 
 
 @pytest.fixture
 def valid_graph2(valid_nodes, valid_edges2):
-    return Graph(properties={}, nodes=valid_nodes, edges=valid_edges2, heuristic_distance_function=manhattan_distance)
+    return Graph(properties={}, nodes=valid_nodes, edges=valid_edges2, distance_function=manhattan_distance)
 
 
 @pytest.fixture
 def valid_graph3(valid_nodes, valid_edges3):
-    return Graph(properties={}, nodes=valid_nodes, edges=valid_edges3, heuristic_distance_function=manhattan_distance, edge_weight_function=length_cost_per_unit)
+    return Graph(properties={}, nodes=valid_nodes, edges=valid_edges3, distance_function=manhattan_distance, edge_weight_function=length_cost_per_unit)
 
 
 @pytest.fixture
 def valid_graph_from_edge_definitions():
     return Graph.from_edge_definitions(edge_definitions=((((0.0, 0.0), (0.0, 2.0)), COMPUTED_WEIGHT, {'cost_per_unit': 2}),
                                                          (((0.0, 0.0), (1.0, 0.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1}),
                                                          (((1.0, 0.0), (2.0, 1.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1}),
@@ -81,15 +81,15 @@
                                        distance_function=manhattan_distance, edge_weight_function=length_cost_per_unit)
 
 
 @pytest.fixture
 def valid_graph_larger():
     with open('data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
         graph = pickle.load(pickled_sample_larger_graph_file)
-        graph.heuristic_distance_function = manhattan_distance
+        graph.distance_function = manhattan_distance
         graph.edge_weight_function = length_cost_per_unit
         return graph
 
 
 @pytest.fixture
 def valid_graph_larger_with_string_edge_weights(valid_graph_larger):
     graph = valid_graph_larger
```

### Comparing `modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/generate_a_star_test_data.py` & `modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/generate_a_star_test_data.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_a_star.py` & `modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_a_star.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,19 +58,19 @@
     assert result == [Hop(edge=Edge(weight=1.0, node_indices=frozenset({0, 2}), properties={'cost_per_unit': 1}), cached_f=5.0, g=1.0, h=4.0),
                       Hop(edge=Edge(weight=2.0, node_indices=frozenset({2, 3}), properties={'cost_per_unit': 1}), cached_f=5.0, g=3.0, h=2.0),
                       Hop(edge=Edge(weight=2.0, node_indices=frozenset({3, 4}), properties={'cost_per_unit': 1}), cached_f=5.0, g=5.0, h=0.0)]
 
 
 def test_a_star_with_no_path_manhattan(valid_nodes):
     with pytest.raises(NoNavigablePathError):
-        a_star(graph=Graph(nodes=valid_nodes, edges=(), heuristic_distance_function=manhattan_distance), start_node_index=0, goal_node_index=3)
+        a_star(graph=Graph(nodes=valid_nodes, edges=(), distance_function=manhattan_distance), start_node_index=0, goal_node_index=3)
 
 
 def test_a_star_with_single_node_path_manhattan():
-    assert len(a_star(graph=Graph(nodes=[(0.0, 0.0)], edges=(), heuristic_distance_function=manhattan_distance), start_node_index=0, goal_node_index=0)) == 0.0
+    assert len(a_star(graph=Graph(nodes=[(0.0, 0.0)], edges=(), distance_function=manhattan_distance), start_node_index=0, goal_node_index=0)) == 0.0
 
 
 def test_a_star_finds_shortest_path_manhattan_larger_graph(valid_graph_larger):
     result = a_star(graph=valid_graph_larger, start_node_index=0, goal_node_index=4)
 
     assert len(result) == 12
     assert result == [Hop(edge=Edge(weight=122.70985671734266, node_indices=frozenset({0, 15})), cached_f=1177.683043473936, g=122.70985671734266, h=1054.9731867565933),
```

### Comparing `modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_distance.py` & `modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_prim.py` & `modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.3.9/tests/modgeosys/graph/test_types.py` & `modgeosys_graph_algorithms-0.4.0/tests/modgeosys/graph/test_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,23 +54,23 @@
     assert edge1 != edge2
 
 
 def test_graph_creation(valid_nodes, valid_edges1, valid_graph1):
     assert valid_graph1.nodes == valid_nodes
     assert valid_graph1.edges == valid_edges1
     assert valid_graph1.properties == {}
-    assert valid_graph1.heuristic_distance_function is not None
+    assert valid_graph1.distance_function is not None
     assert valid_graph1.edge_weight_function is not None
 
 
 def test_graph_creation_with_edge_weight_function(valid_nodes, valid_edges3_with_computed_weights, valid_graph3):
     assert valid_graph3.nodes == valid_nodes
     assert valid_graph3.edges == valid_edges3_with_computed_weights
     assert valid_graph3.properties == {}
-    assert valid_graph3.heuristic_distance_function is not None
+    assert valid_graph3.distance_function is not None
     assert valid_graph3.edge_weight_function is not None
 
 
 def test_graph_creation_from_edge_definitions(valid_graph_from_edge_definitions, valid_nodes, valid_edges1_with_computed_weights):
     assert valid_graph_from_edge_definitions.nodes == valid_nodes
     assert valid_graph_from_edge_definitions.edges == valid_edges1_with_computed_weights
```

### Comparing `modgeosys_graph_algorithms-0.3.9/PKG-INFO` & `modgeosys_graph_algorithms-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modgeosys-graph-algorithms
-Version: 0.3.9
+Version: 0.4.0
 Summary: 
 Author: Kevin Weller
 Author-email: klweller@icloud.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: heapdict (>=1.0.1,<2.0.0)
@@ -48,15 +48,15 @@
                                                           (((0.0, 2.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 3}),
                                                           (((2.0, 1.0), (2.0, 3.0)), COMPUTED_WEIGHT, {'cost_per_unit': 1})),
                                         distance_function=manhattan_distance, edge_weight_function=length_cost_per_unit)
 
 # Load a bigger graph from a pickle file.
 with open('python/data/graph.pickle', 'rb') as pickled_sample_larger_graph_file:
   larger_graph = pickle.load(pickled_sample_larger_graph_file)
-  larger_graph.heuristic_distance_function = manhattan_distance
+  larger_graph.distance_function = manhattan_distance
   larger_graph.edge_weight_function = length_cost_per_unit
 
 # Call the A* function.
 toy_a_star_path = a_star(graph=toy_graph, start_node_index=0, goal_node_index=4)
 print('Toy A* Path:')
 pprint(toy_a_star_path)
 print()
```

