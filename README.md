# Graphs
A _graph_ is simply a collection of nodes with edges between (some of) them.  <br>
* Graphs can be either directed (like the following graph) or undirected. While directed edges are like a 
one-way street, undirected edges are like a two-way street. <br>
* The graph might consist of multiple isolated subgraphs. <br>
* lf there is a path between every pair of vertices, it is called a "connected graph" <br>
* The graph can also have cycles (or not). An "acyclic graph" is one without cycles. <br>

## Graph Traversals 

The two most common ways to search a graph are _depth-first search(DFS)_ and _breadth-first search(BFS)._ 
* In *depth-first search (DFS)*, we start at the root (or another arbitrarily selected node) and explore each branch completely before moving on to the next branch. That is, we go deep first (hence the name depth first search) before we go wide. 
* In *breadth-first search (BFS)*, we start at the root (or another arbitrarily selected node) and explore each neighbor before going on to any of their children. That is, we go wide (hence breadth-first search) before we go deep.

![dfs-vs-bfs](https://user-images.githubusercontent.com/85002425/147876026-81b5dfe7-6aae-4fd5-9222-30afd43ef7c5.gif)


# Kruskal's Algorithm

* Kruskal's algorithm finds a *minimum spanning forest* of an undirected edge-weighted graph. 
* If the graph is connected, it finds a *minimum spanning tree.* (A minimum spanning tree of a connected graph is a subset of the edges that forms a tree that includes every vertex, where the sum of the weights of all the edges in the tree is minimized.
* For a disconnected graph, a *minimum spanning forest* is composed of a minimum spanning tree for each connected component.
* It is a *greedy algorithm* in graph theory as in each step it adds the next lowest-weight edge that will not form a cycle to the minimum spanning forest.

![kruskals](https://user-images.githubusercontent.com/85002425/147876375-622147ba-55da-44f7-96f0-f71424bd71d3.gif)

# Dijkstra's Algorithm

* Dijkstra’s algorithm is very similar to Prim’s algorithm for minimum spanning tree. Like Prim’s MST, we generate a SPT (shortest path tree) with a given source as a root.
* We maintain two sets, one set contains vertices included in the shortest-path tree, other set includes vertices not yet included in the shortest-path tree.
* At every step of the algorithm, we find a vertex that is in the other set (set of not yet included) and has a minimum distance from the source.
* Dijkstra’s algorithm is used to find the shortest path from a single source vertex to all other vertices in the given graph. 

![dijkstra](https://user-images.githubusercontent.com/85002425/147876617-f2d5cc6c-0e16-468b-a0e5-e500b31b46eb.gif)









