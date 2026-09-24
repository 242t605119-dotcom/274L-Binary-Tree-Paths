# Binary Tree Paths

LeetCode 257

## Problem Statement

Given the root of a binary tree, return all root-to-leaf paths in any order.

A leaf is a node with no children.

Each path should be represented as a string where the node values are connected using `"->"`.

## Solution

This solution uses Depth-First Search (DFS) to explore every path from the root to a leaf node.

While traversing the tree, the current node value is added to the path. When a leaf node is reached, the complete path is added to the result list.

## Example

### Input

```text
root = [1,2,3,null,5]
```

### Output

```text
["1->2->5","1->3"]
```

### Explanation

There are two root-to-leaf paths:

```text
1 -> 2 -> 5
1 -> 3
```

Therefore, the output is:

```text
["1->2->5","1->3"]
```

## Approach

1. Start from the root of the binary tree.
2. Use DFS to traverse the tree.
3. Add each node value to the current path.
4. When a leaf node is reached, store the complete path.
5. Continue until all root-to-leaf paths are visited.
6. Return the list of paths.

## Algorithm

1. Create an empty result list.
2. Define a DFS function that receives a node and the current path.
3. If the node is empty, return.
4. Add the node value to the current path.
5. If the node is a leaf, add the path to the result.
6. Otherwise, add `"->"` and recursively visit the left and right children.
7. Return the result list.

## Complexity

* Time Complexity: O(n)
* Space Complexity: O(n)

## Author

T. Nandhini
