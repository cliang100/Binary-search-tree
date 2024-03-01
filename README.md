**Binary Search Tree (BST) Implementation in Python**

This Python script demonstrates the implementation of a Binary Search Tree (BST) along with various operations such as insertion, search, and deletion.

### Classes:

1. **TreeNode:**
   - Represents a single node in the binary search tree.
   - Each node contains a `key` (value), `left` child pointer, and `right` child pointer.
   - The `__str__` method allows printing the key of a node.

2. **BinarySearchTree:**
   - Represents the binary search tree data structure.
   - Provides methods for inserting, searching, deleting nodes, and performing an inorder traversal.
   - The `_insert`, `_search`, `_delete`, and `_inorder_traversal` methods are helper methods used internally.
   - The `insert` method inserts a new key into the BST.
   - The `search` method searches for a key in the BST.
   - The `delete` method removes a key from the BST.
   - The `inorder_traversal` method returns the keys of the BST in sorted order.

### Usage Example:

```python
bst = BinarySearchTree()
nodes = [50, 30, 20, 40, 70, 60, 80]

# Insert nodes into the BST
for node in nodes:
    bst.insert(node)

# Perform inorder traversal to display keys in sorted order
print("Inorder traversal:", bst.inorder_traversal())

# Search for a key in the BST
print("Search for 40:", bst.search(40))

# Delete a key from the BST
bst.delete(40)
print("Inorder traversal after deleting 40:", bst.inorder_traversal())

# Attempt to search for the deleted key
print("Search for 40:", bst.search(40))
```

### Output:
```
Inorder traversal: [20, 30, 40, 50, 60, 70, 80]
Search for 40: 40
Inorder traversal after deleting 40: [20, 30, 50, 60, 70, 80]
Search for 40: None
```

This script demonstrates the basic functionality of a binary search tree, including insertion, search, and deletion operations. Users can easily modify the `nodes` list to create different BST configurations and observe the behavior of the tree.
