# Activities

## Task 1:

- Answer at least 5 questions from the following link. Make sure you write the question as well as the answer.
  https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Graph/GraphIntroSumm.html
 
What is the out degree of Vertex 3?
1

Two vertices of a graph are ADJACENT if there is an edge joining them.
True

How many connected components does this graph have?
It had 3

A complete graph is a clique of size:
|V|

Two vertices can be adjacent even if they are not neighbors.
False

> You can refer to [link #2](#links) below for more info.

## Task 2

- Discuss how depth-first search works by experimenting with the following link. Try both directed and undirected graphs and write a short summary.
  https://opendsa-server.cs.vt.edu/OpenDSA/AV/Graph/DFSAV.html

Depth-first search (DFS) is a graph traversal algorithm that visits all the vertices in a graph by exploring as far as possible along each branch before backtracking. It can be used to detect cycles in a graph, to determine whether a graph is connected, and to find a path between two vertices.

Undirected will go through all nodes, but sometimes directed graph will not go through all nodes.

> You can refer to [link #3](#links) below for more info.

## Task 3

- Discuss how breadth-first search works by experimenting with the following link. Try both directed and undirected graphs and write a short summary.
  https://opendsa-server.cs.vt.edu/OpenDSA/AV/Graph/BFSAV.html

Breadth-first search (BFS) is another graph traversal algorithm that visits all the vertices in a graph by exploring all the vertices at a given distance from the starting vertex before moving on to vertices at the next distance. It can be used to find the shortest path between two vertices, among other applications.

> You can refer to [link #4](#links) below for more info.

## Task 4:

- Reproduce the behavior of the BFS algorithm for the following graph:
  https://opendsa-server.cs.vt.edu/OpenDSA/AV/Graph/BFSPE.html

Done. Take all connected to A in alph order, then go to next letter and connect all.

> You can refer to [link #4](#links) below.

## Task 5: Individual (at home)

- There are two traditional approaches to representing graphs: The adjacency matrix and the adjacency list. What are the main differences in term of space/time complexity. You can refer to following link:
  https://www.baeldung.com/cs/adjacency-matrix-list-complexity

An adjacency matrix is a two-dimensional array of size n x n, where n is the number of vertices in the graph. The entry in row i and column j of the matrix represents the edge between vertex i and vertex j. If the graph is undirected, the matrix is symmetric, and only the upper or lower triangular part of the matrix needs to be stored. If the graph is sparse (i.e., has relatively few edges compared to the maximum possible number of edges), the adjacency matrix can be implemented using a sparse matrix representation to save space.

The main advantage of the adjacency matrix is that checking whether there is an edge between two vertices takes constant time O(1). However, the space complexity of the adjacency matrix is O(n^2), which can be a problem for large graphs, especially if the graph is sparse.

An adjacency list is a list of lists, where each list corresponds to a vertex and contains the vertices that are adjacent to it. If the graph is weighted, the lists can also contain the weights of the edges. The space complexity of the adjacency list is O(n + m), where n is the number of vertices and m is the number of edges.

The main advantage of the adjacency list is that it can represent both directed and undirected graphs efficiently and can handle sparse graphs well. However, checking whether there is an edge between two vertices takes time proportional to the number of adjacent vertices, which can be O(n) in the worst case.

In summary, the adjacency matrix is efficient for dense graphs but can be wasteful for sparse graphs, whereas the adjacency list is efficient for sparse graphs but can be inefficient for dense graphs. The choice of representation depends on the characteristics of the graph and the specific application.

## Links

1. https://cpp.sh/
2. https://opendsa-server.cs.vt.edu/OpenDSA/Books/Everything/html/GraphIntro.html
3. https://opendsa-server.cs.vt.edu/OpenDSA/Books/Everything/html/GraphTraversal.html#depth-first-search
4. https://opendsa-server.cs.vt.edu/OpenDSA/Books/Everything/html/GraphTraversal.html#breadth-first-search
