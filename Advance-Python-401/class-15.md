# class-15

## Trees

### Binary Trees, Binary Search Trees, and K-ary Trees

**1. Binary Trees**

A binary tree is a hierarchical data structure where each node has at most two children: a left child and a right child. The structure of a binary tree resembles a tree, with the topmost node being the root and the nodes below it forming branches. The nodes at the bottom of the tree are called leaf nodes and have no children. In a binary tree, each node can have either zero, one, or two children.
Binary trees can be classified further into full binary trees, complete binary trees, and perfect binary trees, depending on specific conditions:

- **Full Binary Tree:** A binary tree is considered full if every node has either zero or two children.
- **Complete Binary Tree:** A binary tree is considered complete if all levels, except possibly the last one, are completely filled, and all nodes are as left as possible.
- **Perfect Binary Tree:** A binary tree is considered perfect if all levels are completely filled with nodes.
Binary trees can be traversed using various algorithms, including pre-order traversal, in-order traversal, and post-order traversal.

**2. Binary Search Trees (BSTs)**

A binary search tree (BST) is a type of binary tree that satisfies an ordering property. In a BST, for any given node, all the values in its left subtree are less than the node's value, and all the values in its right subtree are greater than the node's value. This ordering property allows for efficient searching, insertion, and deletion operations.
BSTs are commonly used to store data in a way that facilitates efficient searching. The ordering property enables a binary search algorithm, where comparisons are made at each node to determine the next step of the search. In balanced BSTs, such as AVL trees or Red-Black trees, the height of the tree is kept balanced, ensuring efficient search operations with an average time complexity of O(log n).

**3. K-ary Trees**

A K-ary tree is a generalization of a binary tree where each node can have up to K children. The value of K determines the degree of the tree. In a K-ary tree, each node can have at most K children, and each child is labeled as a specific position or index, such as the first child, second child, and so on.
K-ary trees are commonly used to represent hierarchical data structures, such as file systems, organization charts, or multiway search trees. They can efficiently model scenarios where each node may have a variable number of children.

K-ary trees can be traversed using various algorithms, including depth-first traversal (pre-order, in-order, post-order) and breadth-first traversal (level-order).

