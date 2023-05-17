# Trees 

### What is a Tree Data Structure ?
- A Tree is a Data structure in which data items are connected using references in a hierarchical manner. Each Tree consists of a root node from which we can access each element of the tree. Starting from the root node, each node contains zero or more nodes connected to it as children

### Parts of a Tree
![](Treedatastructure.png)


### Common Terminology:

- Node: A component of a tree that contains its own values and references to other nodes.
Root: The starting node of the tree.
- K: A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
- Left: A reference to the left child node in a binary tree.
- Right: A reference to the right child node in a binary tree.
- Edge: The link between a parent and child node.
- Leaf: A node that does not have any children.
- Height: The number of edges from the root to the furthest leaf in a tree

### Traversals:
- Tree traversals allow us to search for nodes, print tree contents, and perform other operations on trees. There are two categories of traversals: depth-first and breadth-first.

  - Depth-First Traversals:

     - Pre-order: Visit the root node, then recursively traverse the left subtree, followed by the right subtree.
     - In-order: Recursively traverse the left subtree, visit the root node, and then traverse the right subtree.
     - Post-order: Recursively traverse the left subtree, then the right subtree, and finally visit the root node.
     
   - Breadth-First Traversal:

     - Iterates through the tree level by level, visiting nodes from left to right
### Big O Complexity:

- The time complexity for inserting a node or searching in a binary tree is O(n) in the worst case, where n is the number of nodes.
The space complexity for inserting a node using breadth-first insertion is O(w), where w is the largest width of the tree.
The time complexity for searching in a binary search tree is O(h), where h is the height of the tree.
In a balanced tree, the height is log(n), while in an unbalanced tree, the height can be n