# Graphs

A graph is a fundamental data structure in computer science that represents a collection of nodes (also called vertices) connected by edges. Graphs are used to model various real-world scenarios, such as social networks, transportation systems, computer networks, and more. They are a versatile tool for solving problems involving relationships and connections between entities.

**Graphs can be classified into two main categories: directed and undirected.**

**1. Directed Graph (Digraph):** In a directed graph, edges have a direction associated with them. This means that an edge from node A to node B does not necessarily imply that there is an edge from B to A. These types of graphs are often used to model scenarios where relationships have a specific direction, like following relationships in a social network.

**2. Undirected Graph:** In an undirected graph, edges do not have a direction. An edge between nodes A and B implies a mutual relationship between them; if there's an edge from A to B, there's also an edge from B to A. Undirected graphs are suitable for modeling symmetric relationships, such as friendships in a social network.

- Graphs can also be categorized based on whether they allow self-loops (an edge from a node to itself) and whether they have weighted edges (edges with associated numerical values, indicating distances, costs, etc.).

**Graphs can be represented using various data structures. The two most common representations are:**

**1. Adjacency Matrix:** An adjacency matrix is a 2D array where each cell (i, j) represents whether there is an edge between nodes i and j. For weighted graphs, the cell value can represent the weight of the edge.

**2. Adjacency List:** An adjacency list represents a graph as a collection of lists. Each node has a list of its adjacent nodes (neighbors). For weighted graphs, each entry in the list can contain not only the adjacent node's identifier but also the weight of the connecting edge.

**Graphs can also have different properties and characteristics:**

- **Degree:** The degree of a node in an undirected graph is the number of edges connected to it. In a directed graph, nodes have both an incoming and an outgoing degree.

- **Path:** A path in a graph is a sequence of nodes where each adjacent pair is connected by an edge. The length of a path is the number of edges it contains.

- **Cycle:** A cycle is a path that starts and ends at the same node.

- **Connected Graph:** A graph is connected if there is a path between every pair of nodes.

- **Acyclic Graph:** A graph without any cycles is called an acyclic graph.

- **Weighted Graph:** A graph where edges have associated weights.

- **Sparse Graph:** A graph with relatively few edges compared to the total number of possible edges.

- **Dense Graph:** A graph with many edges, close to the maximum possible edges.