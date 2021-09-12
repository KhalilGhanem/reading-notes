# Graphs

A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

* Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
* Edge - An edge is a connection between two nodes.
* Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
* Degree - The degree of a vertex is the number of edges connected to that vertex.

## Directed vs Undirected

* Undirected Graph: is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.
* Directed Graph (Digraph): is a graph where every edge is directed.

## Graphs types

* Complete Graph: is when all nodes are connected to all other nodes.
* Connected Graph: is graph that has all of vertices/nodes have at least one edge.
* Disconnected Graph: is a graph where some vertices may not have edges.

## Acyclic vs Cyclic

* Acyclic Graph: is a directed graph without cycles.
  
  A cycle is when a node can be traversed through and potentially end up back at itself.

* Cyclic Graph: is a graph that has cycles.

  A cycle is defined as a path of a positive length that starts and ends at the same vertex.

## Weighted Graphs

A weighted graph is a graph with numbers assigned to its edges. These numbers are called weights.

## Traversals

* Breadth First
* Depth First

## Real World Uses of Graphs

1. GPS and Mapping
2. Driving Directions
3. Social Networks
4. Airline Traffic
5. Netflix uses graphs for suggestions of products
