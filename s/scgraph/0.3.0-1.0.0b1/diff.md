# Comparing `tmp/scgraph-0.3.0.tar.gz` & `tmp/scgraph-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scgraph-0.3.0.tar", last modified: Fri Jul 14 16:05:01 2023, max compression
+gzip compressed data, was "scgraph-1.0.0b1.tar", last modified: Thu Jul 20 20:19:22 2023, max compression
```

## Comparing `scgraph-0.3.0.tar` & `scgraph-1.0.0b1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-14 16:05:00.993639 scgraph-0.3.0/
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-0.3.0/LICENSE
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     4057 2023-07-14 16:05:00.993639 scgraph-0.3.0/PKG-INFO
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)     3396 2023-07-13 13:09:33.000000 scgraph-0.3.0/README.md
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      104 2023-07-11 14:07:00.000000 scgraph-0.3.0/pyproject.toml
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-14 16:05:00.993639 scgraph-0.3.0/scgraph/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)       81 2023-07-11 14:58:32.000000 scgraph-0.3.0/scgraph/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)    24358 2023-07-14 16:04:53.000000 scgraph-0.3.0/scgraph/core.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-14 16:05:00.993639 scgraph-0.3.0/scgraph/data/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      100 2023-07-11 12:57:30.000000 scgraph-0.3.0/scgraph/data/__init__.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      403 2023-07-11 12:57:30.000000 scgraph-0.3.0/scgraph/data/example.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)  1257473 2023-07-11 14:04:45.000000 scgraph-0.3.0/scgraph/data/marnet.py
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     2420 2023-07-11 15:18:13.000000 scgraph-0.3.0/scgraph/utils.py
-drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-14 16:05:00.993639 scgraph-0.3.0/scgraph.egg-info/
--rw-rw-r--   0 conmak    (1000) conmak    (1000)     4057 2023-07-14 16:05:00.000000 scgraph-0.3.0/scgraph.egg-info/PKG-INFO
--rw-rw-r--   0 conmak    (1000) conmak    (1000)      300 2023-07-14 16:05:00.000000 scgraph-0.3.0/scgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-07-14 16:05:00.000000 scgraph-0.3.0/scgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2023-07-14 16:05:00.000000 scgraph-0.3.0/scgraph.egg-info/top_level.txt
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-07-14 16:05:00.993639 scgraph-0.3.0/setup.cfg
--rwxrwxr-x   0 conmak    (1000) conmak    (1000)      969 2023-07-14 16:04:41.000000 scgraph-0.3.0/setup.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:19:22.089457 scgraph-1.0.0b1/
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     1072 2023-04-14 17:06:21.000000 scgraph-1.0.0b1/LICENSE
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     6749 2023-07-20 20:19:22.089457 scgraph-1.0.0b1/PKG-INFO
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)     6084 2023-07-20 20:14:59.000000 scgraph-1.0.0b1/README.md
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      109 2023-07-20 20:16:30.000000 scgraph-1.0.0b1/pyproject.toml
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:19:22.089457 scgraph-1.0.0b1/scgraph/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)       96 2023-07-20 20:10:57.000000 scgraph-1.0.0b1/scgraph/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)    20565 2023-07-20 19:09:42.000000 scgraph-1.0.0b1/scgraph/core.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:19:22.089457 scgraph-1.0.0b1/scgraph/geographs/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:10:31.000000 scgraph-1.0.0b1/scgraph/geographs/__init__.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)  1143458 2023-07-20 20:16:35.000000 scgraph-1.0.0b1/scgraph/geographs/marnet.py
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     2150 2023-07-20 18:43:41.000000 scgraph-1.0.0b1/scgraph/utils.py
+drwxrwxr-x   0 conmak    (1000) conmak    (1000)        0 2023-07-20 20:19:22.089457 scgraph-1.0.0b1/scgraph.egg-info/
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)     6749 2023-07-20 20:19:22.000000 scgraph-1.0.0b1/scgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)      286 2023-07-20 20:19:22.000000 scgraph-1.0.0b1/scgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        1 2023-07-20 20:19:22.000000 scgraph-1.0.0b1/scgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 conmak    (1000) conmak    (1000)        8 2023-07-20 20:19:22.000000 scgraph-1.0.0b1/scgraph.egg-info/top_level.txt
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)       79 2023-07-20 20:19:22.089457 scgraph-1.0.0b1/setup.cfg
+-rwxrwxr-x   0 conmak    (1000) conmak    (1000)      973 2023-07-20 20:19:15.000000 scgraph-1.0.0b1/setup.py
```

### Comparing `scgraph-0.3.0/LICENSE` & `scgraph-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `scgraph-0.3.0/scgraph/core.py` & `scgraph-1.0.0b1/scgraph/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,346 +1,279 @@
-import copy
-from .utils import Distance
+from .utils import haversine, hard_round
 
 
 class Graph:
-    def __init__(self, data: dict):
+    @staticmethod
+    def validate_graph(graph: dict):
         """
         Function:
 
-        - Initialize a Graph object
-        - Returns `None`
+        - Validate that a graph is properly formatted
 
         Required Arguments:
 
-        - None
-
-        Optional Arguments:
-
-        - `data`:
+        - `graph`
             - Type: dict
-            - What: A dictionary of dictionaries
-            - Structure:
-                - `graph`
-                    - Type: dict of dicts of ints or floats
-                    - What: A dictionary of dictionaries of integers or floats
-                        - The first level of keys are the origin nodes
-                        - The second level of keys are the destination nodes
-                        - The values are the distances between the origin and destination nodes
-                        - Note: The graph is assumed to be directed
-                - `nodes`
-                    - Type: dict of dicts of ints or floats
-                    - What: A dictionary of dictionaries of integers or floats
-                        - The first level of keys are the node ids
-                        - The second level of keys are the attributes:
-                            - `latitude`
-                                - Type: float
-                                - What: The latitude of the node
-                            - `longitude`
-                                - Type: float
-                                - What: The longitude of the node
-                        - The values are the attributes for the nodes
-            - EG: {
-                "graph": {
-                        "0": {"1": 5, "2": 1},
-                        "1": {"0": 5, "2": 2, "3": 1},
-                        "2": {"0": 1, "1": 2, "3": 4, "4": 8},
-                        "3": {"1": 1, "2": 4, "4": 3, "5": 6},
-                        "4": {"2": 8, "3": 3},
-                        "5": {"3": 6}
-                    }
-                "nodes": {
-                        "0": {"latitude": 0, "longitude": 0},
-                        "1": {"latitude": 0, "longitude": 1},
-                        "2": {"latitude": 1, "longitude": 0},
-                        "3": {"latitude": 1, "longitude": 1},
-                        "4": {"latitude": 2, "longitude": 0},
-                        "5": {"latitude": 2, "longitude": 1}
-                    }
-                }
-            - Note: In the example:
-                - The distance to travel from node "0" to node "1" is 5
-                - The distance to travel from node "0" to node "2" is 1
-                - Node "0" is at latitude 0 and longitude 0
-        """
-        self.graph = copy.deepcopy(data.get("graph", {}))
-        self.nodes = copy.deepcopy(data.get("nodes", {}))
-
-    def validate_nodes(self):
-        """
-        Function:
-
-        - Validate that the nodes are a dictionary of dictionaries of floats or integers
-        - Returns `None`
-
-        Required Arguments:
-
-        - None
+            - What: A dictionary of dictionaries where the keys are origin node ids and the values are dictionaries of destination node ids and distances
+            - Note: Ids must be integers starting at 0 and increasing sequentially to the number of nodes in the graph
+            - Note: All nodes must be included as origins in the graph regardless of if they have any connected destinations
 
         Optional Arguments:
 
         - None
         """
-        assert isinstance(self.nodes, dict), "Your nodes must be a dictionary"
-        # Check that the nodes are a dictionary of dictionaries of floats
-        for node, node_dict in self.nodes.items():
+        ids = []
+        assert isinstance(graph, dict), "Your graph must be a dictionary"
+        for origin_id, origin_dict in graph.items():
             assert isinstance(
-                node_dict, dict
-            ), f"Your nodes must be a dictionary of dictionaries but the value for node {node} is not a dictionary"
-            for key, value in node_dict.items():
-                assert key in [
-                    "latitude",
-                    "longitude",
-                ], f"Your nodes must be a dictionary of dictionaries where the keys are 'latitude' and 'longitude' but the key ({key}) for node ({node}) is not 'latitude' or 'longitude'"
+                origin_id, int
+            ), f"Origin and destination ids must be integers but {origin_id} is not an integer"
+            assert isinstance(
+                origin_dict, dict
+            ), f"Your graph must be a dictionary of dictionaries but the value for origin {origin_id} is not a dictionary"
+            ids.append(origin_id)
+            for destination_id, distance in origin_dict.items():
                 assert isinstance(
-                    value,
-                    (
-                        float,
-                        int,
-                    ),
-                ), f"Your nodes must be a dictionary of dictionaries where the values are floats or ints but the value for node ({node}) and key ({key}) is not a float"
+                    destination_id, int
+                ), f"Origin and destination ids must be integers but {destination_id} is not an integer"
+                assert isinstance(
+                    distance, (int, float)
+                ), f"Distances must be integers or floats but {distance} is not an integer or float"
+                ids.append(destination_id)
+        ids = set(ids)
+        assert (
+            min(ids) == 0
+        ), f"Your graph must have ids starting at 0 but the minimum id is {min(ids)}"
+        assert (
+            max(ids) == len(ids) - 1
+        ), f"Your graph must have ids that are sequential starting at 0 but the maximum id is {max(ids)}"
+        assert len(graph) == len(
+            ids
+        ), f"Your graph must have origin ids for all nodes regardless of if they have any connected destinations"
 
-    def validate_graph(self, check_symmetry: bool = True):
+    @staticmethod
+    def dijkstra(graph: dict, origin_id: int, destination_id: int):
         """
         Function:
 
-        - Validate that the graph is a dictionary of dictionaries of integers or floats
-        - If `check_symmetry` is True, also validate that the graph is symmetric
-        - Returns `None`
+        - Identify the shortest path between two nodes in a sparse network graph using a modified dijkstra algorithm
+            - Modifications allow for a sparse distance matrix to be used instead of a dense distance matrix
+            - This can dramatically reduce the memory and compute requirements of the algorithm
+            - This algorithm runs in O(n^2) time where n is the number of nodes in the graph
+        - Return a dictionary of various path information including:
+            - `id_path`: A list of node ids in the order they are visited
+            - `path`: A list of node dictionaries (lat + long) in the order they are visited
 
         Required Arguments:
 
-        - None
+        - `graph`
+            - Type: dict
+            - What: A dictionary of dictionaries where the keys are origin node ids and the values are dictionaries of destination node ids and distances
+        - `origin_id`
+            - Type: int
+            - What: The id of the origin node from the graph dictionary to start the shortest path from
+        - `destination_id`
+            - Type: int
+            - What: The id of the destination node from the graph dictionary to end the shortest path at
 
         Optional Arguments:
 
-        - `check_symmetry`
-            - Type: bool
-            - What: Whether to validate that the graph is symmetric
-            - Default: True
-        """
-        assert isinstance(self.graph, dict), "Your graph must be a dictionary"
-        # Check that the graph is a dictionary of dictionaries of integers or floats
-        for origin, destination_dict in self.graph.items():
-            assert isinstance(
-                destination_dict, dict
-            ), f"Your graph must be a dictionary of dictionaries but the value for origin ({origin}) is not a dictionary"
-            for destination, distance in destination_dict.items():
-                # Assert distance is number
-                assert isinstance(
-                    distance,
-                    (
-                        int,
-                        float,
-                    ),
-                ), f"Your graph must be a dictionary of dictionaries where the keys are integers or floats but the key for origin ({origin}) and destination ({destination}) is not an integer or a float"
-                # Assert distance is positive
-                assert (
-                    distance >= 0
-                ), f"Your graph must be a dictionary of dictionaries where the values are positive but the value for origin ({origin}) and destination ({destination}) is not positive"
-                # Assert origin and destination are in nodes if nodes is provided
-                if self.nodes != {}:
-                    # Assert id is in nodes
-                    assert (
-                        origin in self.nodes
-                    ), f"Your graph must be a dictionary of dictionaries where the origin node is in the nodes but the origin node ({origin}) is not in the nodes dictionary"
-                    assert (
-                        destination in self.nodes
-                    ), f"Your graph must be a dictionary of dictionaries where the destination node is in the nodes but the destination node ({destination}) for origin ({origin}) is not in the nodes dictionary"
-        # Check that the graph is symmetric
-        if check_symmetry:
-            for origin, destination_dict in self.graph.items():
-                for destination, distance in destination_dict.items():
-                    if distance != self.graph.get(destination, {}).get(
-                        origin, None
-                    ):
-                        raise ValueError(
-                            f"Graph is not symmetric for origin ({origin}) and destination ({destination})"
-                        )
-
-    def dijkstra(self, origin: str, destination: str):
+        - None
         """
-        Function:
+        distance_matrix = [float("inf") for i in graph]
+        branch_tip_distances = [float("inf") for i in graph]
+        predecessor = [None for i in graph]
+
+        distance_matrix[origin_id] = 0
+        branch_tip_distances[origin_id] = 0
 
-        - Identify the minimum length route between two nodes in a sparse network graph
-        - Return that route as a list of node keys in the order they are visited as well as the total distance traveled
+        while True:
+            current_distance = min(branch_tip_distances)
+            if current_distance == float("inf"):
+                return None
+            current_id = branch_tip_distances.index(current_distance)
+            branch_tip_distances[current_id] = float("inf")
+            if current_id == destination_id:
+                break
+            for connected_id, connected_distance in graph[current_id].items():
+                possible_distance = current_distance + connected_distance
+                if possible_distance < distance_matrix[connected_id]:
+                    distance_matrix[connected_id] = possible_distance
+                    predecessor[connected_id] = current_id
+                    branch_tip_distances[connected_id] = possible_distance
+
+        output_path = [current_id]
+        while predecessor[current_id] is not None:
+            current_id = predecessor[current_id]
+            output_path.append(current_id)
+
+        output_path.reverse()
+
+        return {
+            "path": output_path,
+            "length": hard_round(4, distance_matrix[destination_id]),
+        }
 
-        Algorithm Notes:
+    @staticmethod
+    def dijkstra_makowski(graph: dict, origin_id: int, destination_id: int):
+        """
+        Function:
 
-        - Runs in O(n^2) time
+        - Identify the shortest path between two nodes in a sparse network graph using Makowski's modified Dijkstra algorithm
+            - Modifications allow for a sparse distance matrix to be used instead of a dense distance matrix
+            - Improvements include only computing future potential nodes based on the open leaves for each branch
+                - Open leaves are nodes that have not been visited yet but are adjacent to other visited nodes
+            - This can dramatically reduce the memory and compute requirements of the algorithm
+            - For particularly sparse graphs, this algorithm runs close to O(n) time
+                - Where n is the number of nodes in the graph
+            - For dense graphs, this algorithm runs in O(n^2) time
+                - Where n is the number of nodes in the graph
+        - Return a dictionary of various path information including:
+            - `id_path`: A list of node ids in the order they are visited
+            - `path`: A list of node dictionaries (lat + long) in the order they are visited
 
         Required Arguments:
 
-        - `origin`
-            - Type: str
-            - What: The origin node key
-        - `destination`
-            - Type: str
-            - What: The destination node key
+        - `graph`
+            - Type: dict
+            - What: A dictionary of dictionaries where the keys are origin node ids and the values are dictionaries of destination node ids and distances
+        - `origin_id`
+            - Type: int
+            - What: The id of the origin node from the graph dictionary to start the shortest path from
+        - `destination_id`
+            - Type: int
+            - What: The id of the destination node from the graph dictionary to end the shortest path at
 
         Optional Arguments:
 
         - None
         """
-        ids = list(
-            set(
-                [key for key in self.graph.keys()]
-                + [
-                    key
-                    for subdict in self.graph.values()
-                    for key in subdict.keys()
-                ]
-            )
-        )
-        id_map = {key: idx for idx, key in enumerate(ids)}
-        id_map_inv = {v: k for k, v in id_map.items()}
-
-        origin_id = id_map[origin]
-        destination_id = id_map[destination]
-
-        id_graph = {
-            id_map[origin]: {
-                id_map[destination]: distance
-                for destination, distance in self.graph[origin].items()
-            }
-            for origin in self.graph.keys()
-        }
-
-        distance_matrix = [float("inf") for i in id_map]
-        branch_tip_distances = [float("inf") for i in id_map]
-        predecessor = [None for i in id_map]
+        distance_matrix = [float("inf") for i in graph]
+        open_leaves = {}
+        predecessor = [None for i in graph]
 
         distance_matrix[origin_id] = 0
-        branch_tip_distances[origin_id] = 0
+        open_leaves[origin_id] = 0
 
         while True:
-            current_distance = min(branch_tip_distances)
-            if current_distance == float("inf"):
+            if len(open_leaves) == 0:
                 return None
-            current = branch_tip_distances.index(current_distance)
-            if current == destination_id:
+            current_id = min(open_leaves, key=open_leaves.get)
+            open_leaves.pop(current_id)
+            if current_id == destination_id:
                 break
-            for destination, distance in id_graph[current].items():
-                new_distance = current_distance + distance
-                if new_distance < distance_matrix[destination]:
-                    distance_matrix[destination] = new_distance
-                    predecessor[destination] = current
-                    branch_tip_distances[destination] = new_distance
-            branch_tip_distances[current] = float("inf")
-
-        id_path = [current]
-        while predecessor[current] is not None:
-            current = predecessor[current]
-            id_path.append(current)
-
-        output = {
-            "path_ids": [id_map_inv[id] for id in id_path[::-1]],
-            "length": distance_matrix[destination_id],
+            current_distance = distance_matrix[current_id]
+            for connected_id, connected_distance in graph[current_id].items():
+                possible_distance = current_distance + connected_distance
+                if possible_distance < distance_matrix[connected_id]:
+                    distance_matrix[connected_id] = possible_distance
+                    predecessor[connected_id] = current_id
+                    open_leaves[connected_id] = possible_distance
+
+        output_path = [current_id]
+        while predecessor[current_id] is not None:
+            current_id = predecessor[current_id]
+            output_path.append(current_id)
+
+        output_path.reverse()
+
+        return {
+            "path": output_path,
+            "length": hard_round(4, distance_matrix[destination_id]),
         }
-        if len(self.nodes) > 0:
-            output["path"] = [self.nodes[id] for id in output["path_ids"]]
-        return output
 
-    def dijkstra_v2(
-        self,
-        origin: str,
-        destination: str,
-        return_length: bool = True,
-        return_id_path: bool = True,
-        return_node_path: bool = True,
-    ):
+
+class GeoGraph:
+    def __init__(self, graph: dict, nodes: dict):
         """
         Function:
 
-        - Identify the minimum length route between two nodes in a sparse network graph
-        - Return that route as a list of node keys in the order they are visited
+        - Create a GeoGraph object
+
+        Required Arguments:
+
+        - `graph`
+            - Type: dict
+            - What: A dictionary of dictionaries where the keys are origin node ids and the values are dictionaries of destination node ids and distances
+            - Note: Ids must be integers starting at 0 and increasing sequentially to the number of nodes in the graph
+            - Note: All nodes must be included as origins in the graph regardless of if they have any connected destinations
+        - `nodes`
+            - Type: dict
+            - What: A dictionary of dictionaries where the keys are node ids and the values are dictionaries of node coordinates (latitude and longitude)
+            - Note: Ids must be integers starting at 0 and increasing sequentially to the number of nodes in the graph
+            - Note: All nodes must be included in the nodes dictionary
+
+        Optional Arguments:
+
+        """
+        self.graph = graph
+        self.nodes = nodes
 
-        Algorithm Notes:
+    def validate_graph(self):
+        """
+        Function:
 
-        - Runs between O(n) time and O(n^2) time depending on the sparsity of the graph
-        - This algorithm is faster than `dijkstra` for graphs that terminate branches in dead ends
-        - In general, this applies to graphs that are more sparse
-        - For dense graphs, this algorithm will be slower than `dijkstra` because of the overhead of maintaining the open leaves as a dictionary
+        - Validate that self.graph is properly formatted (see Graph.validate_graph)
 
         Required Arguments:
 
-        - `origin`
-            - Type: str
-            - What: The origin node key
-        - `destination`
-            - Type: str
-            - What: The destination node key
+        - None
 
         Optional Arguments:
 
         - None
         """
-        ids = list(
-            set(
-                [key for key in self.graph.keys()]
-                + [
-                    key
-                    for subdict in self.graph.values()
-                    for key in subdict.keys()
-                ]
-            )
-        )
-        id_map = {key: idx for idx, key in enumerate(ids)}
-        id_map_inv = {v: k for k, v in id_map.items()}
+        Graph.validate_graph(self.graph)
 
-        origin_id = id_map[origin]
-        destination_id = id_map[destination]
+    def validate_nodes(self):
+        """
 
-        id_graph = {
-            id_map[origin]: {
-                id_map[destination]: distance
-                for destination, distance in self.graph[origin].items()
-            }
-            for origin in self.graph.keys()
-        }
+        Function:
 
-        distance_matrix = [float("inf") for i in id_map]
-        open_leaves = {}
-        predecessor = [None for i in id_map]
+        - Validate that self.nodes is properly formatted (see GeoGraph.__init__ docs for more details)
 
-        distance_matrix[origin_id] = 0
-        open_leaves[origin_id] = 0
+        Required Arguments:
 
-        while True:
-            if len(open_leaves) == 0:
-                return None
-            current = min(open_leaves, key=open_leaves.get)
-            open_leaves.pop(current)
-            if current == destination_id:
-                break
-            current_distance = distance_matrix[current]
-            for destination, distance in id_graph[current].items():
-                if current_distance + distance < distance_matrix[destination]:
-                    distance_matrix[destination] = current_distance + distance
-                    predecessor[destination] = current
-                    open_leaves[destination] = current_distance + distance
-
-        id_path = [current]
-        while predecessor[current] is not None:
-            current = predecessor[current]
-            id_path.append(current)
-
-        output = {
-            "path_ids": [id_map_inv[id] for id in id_path[::-1]],
-            "length": distance_matrix[destination_id],
-        }
-        if len(self.nodes) > 0:
-            output["path"] = [self.nodes[id] for id in output["path_ids"]]
-        return output
+        - None
+
+        Optional Arguments:
+
+        - None
+        """
+        assert isinstance(self.nodes, dict), "Your nodes must be a dictionary"
+        for node, node_dict in self.nodes.items():
+            assert isinstance(
+                node_dict, dict
+            ), f"Your nodes must be a dictionary of dictionaries but the value for node {node} is not a dictionary"
+            for key, value in node_dict.items():
+                assert key in [
+                    "latitude",
+                    "longitude",
+                ], f"Your nodes must be a dictionary of dictionaries where the keys are 'latitude' and 'longitude' but the key ({key}) for node ({node}) is not 'latitude' or 'longitude'"
+                assert isinstance(
+                    value,
+                    (
+                        float,
+                        int,
+                    ),
+                ), f"Your nodes must be a dictionary of dictionaries where the values are floats or ints but the value for node ({node}) and key ({key}) is not a float"
+            assert (
+                node_dict.get("latitude") >= -90
+                and node_dict.get("latitude") <= 90
+            ), f"Your latitude values must be between -90 and 90 but the latitude value for node {node} is {node_dict.get('latitude')}"
+            assert (
+                node_dict.get("longitude") >= -180
+                and node_dict.get("longitude") <= 180
+            ), f"Your longitude values must be between -180 and 180 but the longitude value for node {node} is {node_dict.get('longitude')}"
 
     def get_shortest_path(
         self,
-        origin,
-        destination,
-        algorithm: str = "dijkstra_v2",
+        origin_node,
+        destination_node,
+        algorithm_fn=Graph.dijkstra_makowski,
         node_addition_type: str = "quadrant",
         **kwargs,
     ):
         """
         Function:
 
         - Identify the shortest path between two nodes in a sparse network graph
@@ -348,275 +281,218 @@
         - Return a dictionary of various path information including:
             - `id_path`: A list of node ids in the order they are visited
             - `path`: A list of node dictionaries (lat + long) in the order they are visited
             - `length`: The length of the path
 
          Required Arguments:
 
-        - `origin`
+        - `origin_node`
             - Type: dict
             - What: A dictionary with the keys 'latitude' and 'longitude'
-        - `destination`
+        - `destination_node`
             - Type: dict
             - What: A dictionary with the keys 'latitude' and 'longitude'
 
         Optional Arguments:
 
-        - `algorithm`
-            - Type: str
-            - What: The algorithm to use to identify the shortest path
-            - Default: 'dijkstra'
+        - `algorithm_fn`
+            - Type: function | method
+            - What: The algorithm function to identify the shortest path
+            - Default: 'Graph.dijkstra_makowski'
             - Options:
-                - 'dijkstra': A modified dijkstra algorithm that uses a sparse distance matrix to identify the shortest path
-                - 'dijkstra_v2': A modified dijkstra algorithm that uses a sparse distance matrix to identify the shortest path
+                - 'Graph.dijkstra': A modified dijkstra algorithm that uses a sparse distance matrix to identify the shortest path
+                - 'Graph.dijkstra_makowski': A modified dijkstra algorithm that uses a sparse distance matrix to identify the shortest path
+                - Any user defined algorithm that takes the arguments:
+                    - `graph`: A dictionary of dictionaries where the keys are origin node ids and the values are dictionaries of destination node ids and distances
+                    - `origin`: The id of the origin node from the graph dictionary to start the shortest path from
+                    - `destination`: The id of the destination node from the graph dictionary to end the shortest path at
         - `node_addition_type`
             - Type: str
             - What: The type of node addition to use when adding your origin and destination nodes to the distance matrix
             - Default: 'quadrant'
             - Options:
                 - 'quadrant': Add the closest node in each quadrant (ne, nw, se, sw) to the distance matrix for this node
                 - 'closest': Add only the closest node to the distance matrix for this node
                 - 'all': Add all nodes to the distance matrix for this node
             - Notes:
-                - `dijkstra_v2` will operate substantially faster if the `node_addition_type` is set to 'quadrant' or 'closest'
+                - `dijkstra_makowski` will operate substantially faster if the `node_addition_type` is set to 'quadrant' or 'closest'
                 - `dijkstra` will operate at the similar speeds regardless of the `node_addition_type`
-                - When using `all`, you should consider using `dijkstra` instead of `dijkstra_v2` as it will be faster
+                - When using `all`, you should consider using `dijkstra` instead of `dijkstra_makowski` as it will be faster
         - `**kwargs`
             - Any additional keyword arguments to pass to the algorithm
         """
         # Add the origin and destination nodes to the graph
-        self.add_node(
-            node=origin, name="origin", node_addition_type=node_addition_type
+        origin_id = self.add_node(
+            node=origin_node, node_addition_type=node_addition_type
         )
-        self.add_node(
-            node=destination,
-            name="destination",
+        destination_id = self.add_node(
+            node=destination_node,
             node_addition_type=node_addition_type,
         )
 
         try:
-            output = self.run_algorithm(
-                algorithm=algorithm, origin="origin", destination="destination"
+            output = algorithm_fn(
+                graph=self.graph,
+                origin_id=origin_id,
+                destination_id=destination_id,
             )
-            self.remove_node(name="origin")
-            self.remove_node(name="destination")
+            output["coordinate_path"] = self.get_coordinate_path(output["path"])
+            self.remove_added_node(node_id=origin_id)
+            self.remove_added_node(node_id=destination_id)
             return output
         except Exception as e:
-            self.remove_node(name="origin")
-            self.remove_node(name="destination")
+            self.remove_added_node(node_id=origin_id)
+            self.remove_added_node(node_id=destination_id)
             raise e
 
-    def run_algorithm(
-        self,
-        origin: str,
-        destination: str,
-        algorithm: str = "dijkstra_v2",
-        **kwargs,
-    ):
+    def get_coordinate_path(self, path):
         """
         Function:
 
-        - Identify the shortest path between two nodes in a sparse network graph
-
-        - Return a dictionary of various path information including:
-            - `id_path`: A list of node ids in the order they are visited
-            - `path`: A list of node dictionaries (lat + long) in the order they are visited
-            - `length`: The length of the path
+        - Return a list of node dictionaries (lat + long) in the order they are visited
 
-         Required Arguments:
+        Required Arguments:
 
-        - `algorithm`
-            - Type: str
-            - What: The algorithm to use to identify the shortest path
-            - Default: 'dijkstra'
-            - Options:
-                - 'dijkstra': A modified dijkstra algorithm that uses a sparse distance matrix to identify the shortest path
-                - 'dijkstra_v2': A modified dijkstra algorithm that uses a sparse distance matrix to identify the shortest path
-        - `origin`
-            - Type: str
-            - What: The name of the origin node in the network data
-        - `destination`
-            - Type: str
-            - What: The name of the destination node in the network data
+        - `path`
+            - Type: list
+            - What: A list of node ids in the order they are visited
 
         Optional Arguments:
 
-        - **kwargs:
-            - Any additional keyword arguments to pass to the algorithm
+        - None
         """
-        # Assert that the algorithm is valid
-        assert algorithm in [
-            "dijkstra",
-            "dijkstra_v2",
-        ], f"Invalid algorithm provided ({algorithm}), valid options are: dijkstra or dijkstra_v2"
-        if algorithm == "dijkstra":
-            return self.dijkstra(origin, destination, **kwargs)
-        elif algorithm == "dijkstra_v2":
-            return self.dijkstra_v2(origin, destination, **kwargs)
+        return [self.nodes[node_id] for node_id in path]
 
-    def remove_node(self, name: str):
+    def remove_added_node(self, node_id: int):
         """
         Function:
 
-        - Remove a node from the network
+        - Remove a node that has been added to the network from the network
+        - Assumes that this node has symmetric flows
+            - EG: If node A has a distance of 10 to node B, then node B has a distance of 10 to node A
         - Return None
 
         Required Arguments:
 
-        - `name`
+        - `node_id`
             - Type: str
             - What: The name of the node to remove
 
         Optional Arguments:
 
         - None
         """
         # Assert that the node exists
         assert (
-            name in self.nodes.keys()
-        ), f"Node {name} does not exist in the network"
-
-        # Remove the node from the nodes dictionary
-        del self.nodes[name]
-
-        # Remove the node from the graph
-        del self.graph[name]
-        for node in self.graph.keys():
-            if name in self.graph[node].keys():
-                del self.graph[node][name]
+            node_id in self.nodes
+        ), f"Node {node_id} does not exist in the network"
+        reverse_connections = [i for i in self.graph[node_id].keys()]
+        for reverse_connection in [i for i in self.graph[node_id].keys()]:
+            del self.graph[reverse_connection][node_id]
+        del self.graph[node_id]
+        del self.nodes[node_id]
 
     def add_node(
         self,
         node: dict,
-        name: str,
         circuity: [float, int] = 4,
-        distance_calculation: str = "haversine",
         node_addition_type: str = "quadrant",
     ):
         """
         Function:
 
         - Add a node to the network
-        - Return None
+        - Returns the id of the new node
 
         Required Arguments:
 
         - `node`
             - Type: dict
             - What: A dictionary with the keys 'latitude' and 'longitude'
-        - `name`
-            - Type: str
-            - What: The name of the node
 
         Optional Arguments:
 
         - `circuity`
             - Type: float | int
-            - What: The circuity of the network
-            - Default: 2
-        - `distance_calculation`
-            - Type: str
-            - What: The distance calculation to use
-            - Default: 'haversine'
-            - Options: 'haversine'
+            - What: The circuity to apply to any distance calculations
+            - Default: 4
+            - Note: This defaults to 4 to prevent the algorithm from taking a direct route in direction of the destination over some impassible terrain (EG: a maritime network that goes through land)
         - `node_addition_type`
             - Type: str
             - What: The type of node addition to use
             - Default: 'quadrant'
             - Options:
                 - 'quadrant': Add the closest node in each quadrant (ne, nw, se, sw) to the distance matrix for this node
                 - 'closest': Add only the closest node to the distance matrix for this node
                 - 'all': Add all nodes to the distance matrix for this node
             - Notes:
-                - `dijkstra_v2` will operate substantially faster if the `node_addition_type` is set to 'quadrant' or 'closest'
+                - `dijkstra_makowski` will operate substantially faster if the `node_addition_type` is set to 'quadrant' or 'closest'
                 - `dijkstra` will operate at the similar speeds regardless of the `node_addition_type`
-                - When using `all`, you should consider using `dijkstra` instead of `dijkstra_v2` as it will be faster
+                - When using `all`, you should consider using `dijkstra` instead of `dijkstra_makowski` as it will be faster
 
         """
-        # Validate the node
-        assert isinstance(name, str), f"Your node name ({name}) is not a string"
-        assert isinstance(
-            node, dict
-        ), f"Your node ({name}) must be a dictionary"
-        assert (
-            "latitude" in node.keys()
-        ), f'Your node must ({name}) have a key called "latitude"'
+        # Validate the inputs
+        assert isinstance(node, dict), "Node must be a dictionary"
+        assert "latitude" in node.keys(), "Node must have a latitude"
+        assert "longitude" in node.keys(), "Node must have a longitude"
         assert (
-            "longitude" in node.keys()
-        ), 'Your node ({name}) must have a key called "longitude"'
-        assert isinstance(
-            node["latitude"], (int, float)
-        ), f"Your node ({name}) latitude must be an integer or a float"
-        assert isinstance(
-            node["longitude"], (int, float)
-        ), f"Your node ({name}) longitude must be an integer or a float"
-        # Validate the circuity
-        assert isinstance(
-            circuity, (int, float)
-        ), f"Your circuity for node ({name}) must be an integer or a float"
+            node["latitude"] >= -90 and node["latitude"] <= 90
+        ), "Latitude must be between -90 and 90"
         assert (
-            circuity >= 1
-        ), f"Your circuity for node  ({name}) must be greater than or equal to 1"
-        # Validate the distance calculation
-        assert distance_calculation in [
-            "haversine"
-        ], f"Invalid distance calculation provided for node ({name}) with option ({distance_calculation}), valid options are: haversine"
+            node["longitude"] >= -180 and node["longitude"] <= 180
+        ), "Longitude must be between -180 and 180"
+        assert circuity > 0, "Circuity must be greater than 0"
         assert node_addition_type in [
             "quadrant",
             "all",
             "closest",
-        ], f"Invalid node addition type provided for node ({name}) with option ({node_addition_type}), valid options are: quadrant, all, closest"
-        if node_addition_type == "quadrant":
-            # Calculate the distance from the new node to all other nodes and add
-            # only the closest node in each directional quadrant (ne, nw, se, sw) to the graph
-            quadrant_distances = {}
-            for node_i_id, node_i in self.nodes.items():
-                direction = (
+        ], f"Invalid node addition type provided ({node_addition_type}), valid options are: ['quadrant', 'all', 'closest']"
+
+        # Create the node
+        new_node_id = max(self.graph) + 1
+        self.nodes[new_node_id] = node
+        self.graph[new_node_id] = {}
+
+        distances = {
+            node_i_id: {
+                "distance": round(
+                    haversine(node, node_i, circuity=circuity), 4
+                ),
+                "quadrant": (
                     "n" if node["latitude"] > node_i["latitude"] else "s"
                 )
-                direction += (
-                    "e" if node["longitude"] > node_i["longitude"] else "w"
-                )
-                lowest_distance = quadrant_distances.get(direction, {}).get(
-                    "distance", float("inf")
-                )
-                node_i_distance = Distance.haversine(
-                    node, node_i, circuity=circuity
-                )
-                if node_i_distance < lowest_distance:
-                    quadrant_distances[direction] = {
-                        "distance": node_i_distance,
-                        "node": node_i_id,
-                    }
-            self.graph[name] = {}
-            for quadrant in quadrant_distances.values():
-                self.graph[quadrant["node"]][name] = quadrant["distance"]
-                self.graph[name][quadrant["node"]] = quadrant["distance"]
-            # Add the node to the nodes dictionary
-            self.nodes[name] = node
-        elif node_addition_type == "all":
-            # Calculate the distance from the new node to all other nodes
-            self.graph[name] = {}
+                + ("e" if node["longitude"] > node_i["longitude"] else "w"),
+            }
+            for node_i_id, node_i in self.nodes.items()
+        }
+
+        if node_addition_type == "all":
             for node_i_id, node_i in self.nodes.items():
-                distance = Distance.haversine(node, node_i, circuity=circuity)
-                self.graph[node_i_id][name] = distance
-                self.graph[name][node_i_id] = distance
-            # Add the node to the nodes dictionary
-            self.nodes[name] = node
+                self.graph[new_node_id][node_i_id] = distances[node_i_id][
+                    "distance"
+                ]
+                self.graph[node_i_id][new_node_id] = distances[node_i_id][
+                    "distance"
+                ]
         elif node_addition_type == "closest":
-            # Calculate the distance from the new node to all other nodes and add
-            # only the closest node to the graph
-            closest_node = None
-            closest_distance = float("inf")
-            for node_i_id, node_i in self.nodes.items():
-                distance = Distance.haversine(node, node_i, circuity=circuity)
-                if distance < closest_distance:
-                    closest_node = node_i_id
-                    closest_distance = distance
-            self.graph[name] = {closest_node: closest_distance}
-            self.graph[closest_node][name] = closest_distance
-            # Add the node to the nodes dictionary
-            self.nodes[name] = node
-        else:
-            raise ValueError(
-                f"Invalid node addition type: {node_addition_type}"
-            )
+            min_node_id = min(distances, key=lambda x: distances[x]["distance"])
+            self.graph[new_node_id][min_node_id] = distances[min_node_id][
+                "distance"
+            ]
+            self.graph[min_node_id][new_node_id] = distances[min_node_id][
+                "distance"
+            ]
+        elif node_addition_type == "quadrant":
+            for quadrant in ["ne", "nw", "se", "sw"]:
+                min_node_id = min(
+                    distances,
+                    key=lambda x: distances[x]["distance"]
+                    if distances[x]["quadrant"] == quadrant
+                    else float("inf"),
+                )
+                self.graph[new_node_id][min_node_id] = distances[min_node_id][
+                    "distance"
+                ]
+                self.graph[min_node_id][new_node_id] = distances[min_node_id][
+                    "distance"
+                ]
+        return new_node_id
```

### Comparing `scgraph-0.3.0/scgraph/utils.py` & `scgraph-1.0.0b1/scgraph/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,78 +1,75 @@
 import math
 
 
-class Distance:
-    @classmethod
-    def haversine(
-        self,
-        origin: dict,
-        destination: dict,
-        units: str = "km",
-        circuity: [float, int] = 1,
-    ):
-        """
-        Function:
-
-        - Calculate the great circle distance in kilometers between two points on the earth (specified in decimal degrees)
-
-        Required Arguments:
-
-        - `origin`:
-            - Type: dict
-            - What: is the origin point? (dict with keys "longitude" and "latitude")
-        - `destination`:
-            - Type: dict
-            - What: is the destination point? (dict with keys "longitude" and "latitude")
-
-        Optional Arguments:
-
-        - `units`:
-            - Type: str
-            - What: units to return the distance in? (one of "km", "m", "mi", or "ft")
-            - Default: "km"
-        - `circuity`:
-            - Type: float | int
-            - What: Multiplier to increase the calculated distance (to account for circuity)
-            - Default: 1
-
-        """
-        # convert decimal degrees to radians
-        lon1, lat1, lon2, lat2 = map(
-            math.radians,
-            [
-                origin["longitude"],
-                origin["latitude"],
-                destination["longitude"],
-                destination["latitude"],
-            ],
-        )
-        # haversine formula
-        dlon = lon2 - lon1
-        dlat = lat2 - lat1
-        a = (
-            math.sin(dlat / 2) ** 2
-            + math.cos(lat1) * math.cos(lat2) * math.sin(dlon / 2) ** 2
-        )
-        c = 2 * math.asin(a**0.5)
-        # Set the radius of earth based on the units specified
-        if units == "km":
-            radius = 6371
-        elif units == "m":
-            radius = 6371000
-        elif units == "mi":
-            radius = 3959
-        elif units == "ft":
-            radius = 3959 * 5280
-        else:
-            raise ValueError('Units must be one of "km", "m", "mi", or "ft"')
-        return c * radius * circuity
+def haversine(
+    origin: dict,
+    destination: dict,
+    units: str = "km",
+    circuity: [float, int] = 1,
+):
+    """
+    Function:
+
+    - Calculate the great circle distance in kilometers between two points on the earth (specified in decimal degrees)
+
+    Required Arguments:
+
+    - `origin`:
+        - Type: dict
+        - What: is the origin point? (dict with keys "longitude" and "latitude")
+    - `destination`:
+        - Type: dict
+        - What: is the destination point? (dict with keys "longitude" and "latitude")
+
+    Optional Arguments:
+
+    - `units`:
+        - Type: str
+        - What: units to return the distance in? (one of "km", "m", "mi", or "ft")
+        - Default: "km"
+    - `circuity`:
+        - Type: float | int
+        - What: Multiplier to increase the calculated distance (to account for circuity)
+        - Default: 1
+
+    """
+    # convert decimal degrees to radians
+    lon1, lat1, lon2, lat2 = map(
+        math.radians,
+        [
+            origin["longitude"],
+            origin["latitude"],
+            destination["longitude"],
+            destination["latitude"],
+        ],
+    )
+    # haversine formula
+    dlon = lon2 - lon1
+    dlat = lat2 - lat1
+    a = (
+        math.sin(dlat / 2) ** 2
+        + math.cos(lat1) * math.cos(lat2) * math.sin(dlon / 2) ** 2
+    )
+    c = 2 * math.asin(a**0.5)
+    # Set the radius of earth based on the units specified
+    if units == "km":
+        radius = 6371
+    elif units == "m":
+        radius = 6371000
+    elif units == "mi":
+        radius = 3959
+    elif units == "ft":
+        radius = 3959 * 5280
+    else:
+        raise ValueError('Units must be one of "km", "m", "mi", or "ft"')
+    return c * radius * circuity
 
 
-def hardRound(decimal_places, a):
+def hard_round(decimal_places, a):
     """
     Function:
 
     - Round a number to a specified number of decimal places
 
     Required Arguments:
```

### Comparing `scgraph-0.3.0/setup.py` & `scgraph-1.0.0b1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
   name = 'scgraph',
   packages = find_packages(),
-  version = '0.3.0',
+  version = '1.0.0b1',
   license='MIT',
   description = 'Determine an approximate route between two points on earth',
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'Connor Makowski',
   author_email = 'connor.m.makowski@gmail.com',
   url = 'https://github.com/connor-makowski/scgraph',
-  download_url = 'https://github.com/connor-makowski/scgraph/dist/scgraph-0.3.0.tar.gz',
+  download_url = 'https://github.com/connor-makowski/scgraph/dist/scgraph-1.0.0b1.tar.gz',
   keywords = ['scgraph'],
   install_requires=[],
   classifiers=[
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',
```

