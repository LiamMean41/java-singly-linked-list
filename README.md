# Java Singly Linked List

A singly linked list (SLL) implemented from scratch in Java using a custom `Node` class and a `LinearListInterface` contract. Built as a week 2 data structures and algorithms exercise to explore pointer-based list traversal and manual memory management.

## How it works

Each node stores a data element and a reference (`next`) to the following node. The list tracks a `head` pointer and manually maintains a `size` counter. Traversal uses `curr` and `prev` pointers that walk the chain node by node.

| Method | Behaviour |
|---|---|
| `add(Object)` | Appends an element to the end of the list |
| `add(int, Object)` | Inserts an element at a given index |
| `remove(int)` | Removes the node at a given index |
| `get(int)` | Returns the node at a given index |
| `size()` | Returns the number of nodes |
| `isEmpty()` | Returns true if the list has no nodes |
| `print()` | Prints all nodes from head to tail |

## Requirements

- Java 8 or higher
- NetBeans IDE (recommended — project includes `nbproject/` config)

## Getting started

Open in NetBeans via `File → Open Project` and run, or build manually:

```bash
javac -sourcepath src -d out src/week2/SLLApp.java
java -cp out week2.SLLApp
```

The app runs a console self-test on launch — adding three nodes, printing the list, checking size, then inserting a wildcard node at index 1 and printing again.

## Notes

Indices in this implementation are **1-based**, not 0-based. Index `1` refers to the head node.
