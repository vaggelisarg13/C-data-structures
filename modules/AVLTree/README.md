# AVL Tree

The [AVL Tree](https://en.wikipedia.org/wiki/AVL_tree) is a self-balancing binary search tree that maintains its height balance to ensure efficient operations for insertion, deletion, and search. This data structure is particularly useful when dealing with dynamic datasets that require frequent updates while maintaining a logarithmic height, ensuring O(log n) time complexity for most operations.
To be more specific, in the AVL tree the difference in height between the left and right subtrees of every node is at most 1. This property ensures that the tree is always balanced and prevents it from becoming skewed, which guarantees efficient search, insertion, and deletion operations.

For each node: 
$$∣height(left-subtree) − height(right-subtree)∣ ≤ 1$$


## Features
- Automatic balancing: The AVL tree maintains its balance during insertions and deletions, ensuring a balanced structure at all times.
- Generic implementation: The tree is implemented using void pointers and macros, making it adaptable to different data types.
- Efficient operations: Most operations, such as search, insertion, and deletion, have an average time complexity of O(log n).

<img align="right" width=380 alt="AVL Tree picture" src="https://en.wikipedia.org/wiki/File:AVL-tree-wBalance_K.svg">

### Complexity of the implemented functions

| Function                   | Time Complexity          | Space Complexity        |
|----------------------------|--------------------------|-------------------------|
| AVLTree_insert             | O(log n)                | O(log n) (recursive)    |
| AVLTree_delete             | O(log n)                | O(log n) (recursive)    |
| AVLTree_search             | O(log n)                | O(log n) (recursive)    |
| AVLTree_inorder_traversal  | O(n)                    | O(log n) (recursive)    |
| AVLTree_preorder_traversal | O(n)                    | O(log n) (recursive)    |
| AVLTree_postorder_traversal| O(n)                    | O(log n) (recursive)    |
| AVLTree_select_k_th_item   | O(log n)                | O(log n) (recursive)    |
| AVLTree_empty              | O(1)                    | O(1)                    |
| AVL_count_items            | O(n)                    | O(logn) (recursive)     |
| AVLTree_min_value          | O(log n)                | O(log n) (recursive)    |
| AVLTree_max_value          | O(log n)                | O(log n) (recursive)    |
| AVLTree_destroy            | O(n)                    | O(log n) (recursive)    |