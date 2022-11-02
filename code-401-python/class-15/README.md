# Binary tree
**Trees** are non-linear data structures that represent nodes connected by edges. Each tree consists of a root node as the Parent node, and the left node and right node as Child nodes.

**Binary tree** tree whose elements have at most two children is called a binary tree. Each element in a binary tree can have only two children. A node’s left child must have a value less than its parent’s value, and the node’s right child must have a value greater than its parent value.
![tree](https://cdn.programiz.com/sites/tutorial2program/files/tree_0.png)


## Implementation
```
class Node:

    def __init__(self, data):
        # left child
        self.left = None
        # right child
        self.right = None
        # node's value
        self.data = data

    # print function
    def PrintTree(self):
        print(self.data)

root = Node(27)

root.PrintTree()

```

## Types of Tree
1. Binary Tree
2. Binary Search Tree
3. AVL Tree
4. B-Tree

### Node
A node is an entity that contains a key or value and pointers to its child nodes.

The last nodes of each path are called leaf nodes or external nodes that do not contain a link/pointer to child nodes.

The node having at least a child node is called an internal node.

### Edge
It is the link between any two nodes.
### Refrences :
1. https://www.programiz.com/dsa/trees
2. https://www.educative.io/answers/binary-trees-in-python
