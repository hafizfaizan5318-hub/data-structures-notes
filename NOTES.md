# DSA Quick Revision Cheat Sheet

## Big-O — how fast an algorithm grows
| Notation | Name | Example |
|---|---|---|
| O(1) | Constant | Accessing an array element by index |
| O(log n) | Logarithmic | Binary search |
| O(n) | Linear | Traversing an array or linked list |
| O(n log n) | Linearithmic | Merge sort, quick sort (average) |
| O(n²) | Quadratic | Bubble sort, nested loops |

- **Omega (Ω)** = best case. **Theta (Θ)** = average/tight bound. **Big-O** = worst case.

## Stack (LIFO — Last In, First Out)
- `push(x)` add on top · `pop()` remove top · `peek()` see top without removing
- Used in: undo buttons, function calls, bracket matching, backtracking.

## Queue (FIFO — First In, First Out)
- `enqueue(x)` add at rear · `dequeue()` remove from front
- Circular queue reuses empty front spaces so memory is not wasted.
- Used in: print jobs, task scheduling, BFS.

## Linked List
- Nodes hold **data + next pointer**. No fixed size, but no direct index access — finding an item is O(n).
- Insert/delete at the **start** is O(1). At the **end**: trace to the last node, link the new node, done.
- Always keep a `head` pointer safe — lose it and the whole list is lost.

## Trees
- Traversals of a binary tree: **Inorder** (left, root, right), **Preorder** (root, left, right), **Postorder** (left, right, root).
- Inorder traversal of a BST gives values in **sorted order**.

## Graphs
- **BFS** explores level by level (uses a queue). **DFS** goes deep first (uses a stack / recursion).

## Searching & Sorting
- Binary search: array must be **sorted**; halves the search space each step → O(log n).
- Bubble sort: swap neighbours repeatedly; the largest value "bubbles" to the end each pass.

## Hashing
- A hash function turns a key into an index. Two keys landing on the same index = **collision**; handled by chaining (linked list at that index) or open addressing (probe for the next free slot).

---
*Personal study notes — written while learning, may simplify some details.*
