# Graphs 

### What are graphs, and what are their common terminologies ?
- A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges

- common terminologies used in graphs are:

* **Vertex:** A vertex (or node) is a point in a graph.
* **Edge:** An edge (or link) is a connection between two vertices in a graph.
* **Degree:** The degree of a vertex is the number of edges connected to it.
* **Path:** A path is a sequence of vertices connected by edges.
* **Cycle:** A cycle is a path that starts and ends at the same vertex.
* **Tree:** A tree is a connected graph with no cycles.

### What are the types of graphs ?
- Directed and Undirected
- Depends on how connected the graphs are to other node/vertices, There are three different types are completed, connected, and disconnected.


### What are the different ways of representing graphs ?
- Adjacency Matrix
- Adjacency List

### what is the weighted graph ?
- A weighted graph is a graph with numbers assigned to its edges. These numbers are called weights


### How to traverse the graph ?
1. Breadth First : BFS starts at a single vertex and explores all of its adjacent vertices before moving on to the next level of vertices. This process continues until all vertices in the graph have been visited.

- Here is what the algorithm breadth first traversal looks like:

- Enqueue the declared start node into the Queue.
- Create a loop that will run while the node still has nodes present.
- Dequeue the first node from the queue
- if the Dequeue‘d node has unvisited child nodes, add the unvisited children to visited set and insert them into the queue.

- The implementation :
```
ALGORITHM BreadthFirst(vertex)
    DECLARE nodes <-- new List()
    DECLARE breadth <-- new Queue()
    DECLARE visited <-- new Set()

    breadth.Enqueue(vertex)
    visited.Add(vertex)

    while (breadth is not empty)
        DECLARE front <-- breadth.Dequeue()
        nodes.Add(front)

        for each child in front.Children
            if(child is not visited)
                visited.Add(child)
                breadth.Enqueue(child)

    return nodes;
```

2. depth first 
- The depth first traversal uses a stack (last in, first out) to traverse the nodes of the graph. The algorithm will start at a given node, push it into the stack and mark it as visited. Then, it will visit all the adjacent nodes and for each adjacent node, it will repeat the same process. If there are no more adjacent nodes to explore, the top element of the stack is popped off and the process repeats itself until the stack is empty.
- The algorithm for a depth first traversal is as follows:

- Push the root node into the Stack and mark as visited.
- Start a while loop that runs as long as the stack is not empty.
= Pop the top node off of the stack and check its neighbors.
- If a neighbor hasn’t been visited, push it onto the stack and mark as visited.
- Repeat until the stack is empty.