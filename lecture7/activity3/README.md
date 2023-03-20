# Activities

## Task 1

- Refer to te following link. Explain the Dijkstra's Shortest Path Algorithm.
  https://www.freecodecamp.org/news/dijkstras-shortest-path-algorithm-visual-introduction/

Dijkstra's algorithm is a shortest path algorithm that helps find the shortest path between two nodes in a graph. The algorithm works by starting at the source node and finding the shortest path to all other nodes in the graph.

The algorithm uses a priority queue to keep track of the nodes that need to be visited. The priority queue is initialized with the source node and its distance is set to 0. The distance to all other nodes is set to infinity.

The algorithm then selects the node with the smallest distance from the priority queue and visits all its neighbors. For each neighbor, the algorithm calculates the distance to the neighbor through the current node and updates its distance if it is smaller than the current distance.

The algorithm then adds the neighbor to the priority queue if it has not been visited before. This process is repeated until all nodes have been visited or the destination node is reached.

Once the algorithm has visited all nodes, it returns the shortest path to the destination node. The shortest path is found by tracing back from the destination node to the source node using the parent node of each visited node.

Dijkstra's algorithm is an efficient algorithm with a time complexity of O(E log V) where E is the number of edges and V is the number of vertices in the graph. The algorithm can be used to solve many problems such as finding the shortest path in a road network, the fastest way to travel between two cities, or the least expensive way to route a package through a network.

## Task 2

- Explain how the code in `./src/dspa.cpp` works. Refer to the following link:
  https://www.geeksforgeeks.org/c-program-for-dijkstras-shortest-path-algorithm-greedy-algo-7/

 Dijkstra's algorithm, a shortest-path algorithm that finds the shortest path between a source node and all other nodes in a weighted graph. The program uses an adjacency matrix to represent the graph.

The program first defines the number of vertices in the graph using the preprocessor directive #define V 9.

Next, there are three functions defined:

minDistance - this function takes in two arrays, dist and sptSet, and returns the index of the vertex with the minimum distance value from the set of vertices not yet included in the shortest path tree. It does this by iterating through all vertices and checking if the vertex has not been included in the shortest path tree and its distance value is less than or equal to the current minimum. If it is, it updates the minimum value and the index of the minimum value.

printSolution - this function takes in the array dist and the number of vertices n and prints the shortest distance from the source vertex to each vertex. It simply iterates through all vertices and prints the vertex index and its distance from the source vertex.

dijkstra - this is the main function that implements Dijkstra's algorithm. It takes in the adjacency matrix graph and the source vertex src. It first initializes two arrays, dist and sptSet. dist is used to store the minimum distance from the source vertex to each vertex, and sptSet is used to keep track of whether each vertex has been included in the shortest path tree or not.

The program then initializes all distances in dist to INT_MAX and all values in sptSet to false. The distance from the source vertex to itself is set to 0.

The main loop of the algorithm runs V-1 times, where V is the number of vertices in the graph. In each iteration, it finds the vertex with the minimum distance value that has not yet been included in the shortest path tree using the minDistance function. It then marks this vertex as processed by setting its corresponding value in sptSet to true.

The program then updates the distance values of all adjacent vertices of the current vertex by checking if the current vertex provides a shorter path to them than their current distance value. If it does, their distance value is updated accordingly.

After the loop completes, the printSolution function is called to print the shortest distance from the source vertex to each vertex in the graph.

Finally, the main function creates an example graph using the adjacency matrix and calls the dijkstra function with the source vertex 0.

## Task 3

- Explain how the code in `./src/mspt.cpp` works. Refer to the following link:
  https://www.tutorialspoint.com/kruskal-s-minimum-spanning-tree-algorithm-greedy-algorithm-in-cplusplus#

This is a C++ program to find the Minimum Spanning Tree (MST) of a given graph using Kruskal's algorithm.

The program defines three data structures: Edge, Graph, and subset. The Edge structure defines the source and destination vertices and the weight of an edge. The Graph structure defines the number of vertices and edges in the graph, as well as an array of Edge structures to store the edges. The subset structure is used to represent a subset of the vertices in the graph.

The program then defines several functions. The createGraph function creates a new graph with the specified number of vertices and edges and returns a pointer to it. The find function finds the parent of a given vertex in a subset, and the Union function performs the union of two subsets by rank. The myComp function is a comparison function used by the qsort function to sort the edges in the graph by weight.

The KruskalMST function takes a pointer to a graph as input and uses Kruskal's algorithm to find its MST. It first initializes an empty array result to store the edges in the MST, sets the edge counter e to 0, and sorts the edges in the graph by weight using qsort. It then initializes an array of subset structures and sets each vertex to its own subset.

It then iterates over the sorted edges, and for each edge, it finds the parents of its source and destination vertices using the find function. If the parents are not the same, it adds the edge to the result array and merges the subsets using the Union function. It continues this process until it has added V-1 edges to result or it has processed all the edges in the graph. It then prints out the edges in the MST and the minimum cost of the MST.

The main function of the program creates a new graph with 24 vertices and 25 edges, initializes the edges with their source, destination, and weight, and then calls the KruskalMST function to find the MST of the graph. The MST is printed out along with its minimum cost.

## Task 4: Individual (at home)

- Refer to te following link. Explain when to use the greedy methods and when to avoid them.
  https://www.freecodecamp.org/news/when-to-use-greedy-algorithms/

Greedy algorithms are used when the optimal solution to a problem can be obtained by making a locally optimal choice at each step. They are simple to implement and often produce good solutions in a reasonable amount of time. However, there are situations where greedy algorithms may not produce the optimal solution, and in such cases, it is better to use other algorithms.

  Here are some situations where it is appropriate to use greedy algorithms:

      When the problem can be broken down into smaller subproblems, and the optimal solution to the overall problem can be obtained by solving the subproblems independently.

      When the problem exhibits the "matroid property," which means that the optimal solution to the problem can be obtained by iteratively adding elements to a "greedy" solution in a certain order.

      When the problem satisfies the "optimal substructure" property, which means that the optimal solution to the problem can be obtained by combining the optimal solutions to smaller subproblems.

      When the problem has a natural ordering of elements, and the optimal solution can be obtained by selecting elements in that order.

  On the other hand, there are situations where greedy algorithms may not produce the optimal solution, and other algorithms should be used instead. Here are some examples:

      When the problem does not exhibit the matroid property or the optimal substructure property.

      When the problem has multiple objectives, and it is not clear how to optimize them all simultaneously.

      When the problem has constraints that are difficult to satisfy, and a greedy algorithm may violate them.

      When the problem has cycles or other structures that make it difficult to choose a locally optimal solution.

  In summary, greedy algorithms are useful when the problem exhibits certain properties, such as matroid property or optimal substructure, and when the solution can be obtained by making a locally optimal choice at each step. However, in some cases, greedy algorithms may not produce the optimal solution, and other algorithms should be used instead.

## Link(s)

- https://cpp.sh/
