# Binary Trees
This repository contains C functions and structures related to binary trees. Here, we explore the fundamentals of binary trees, their properties, traversal methods, and distinctions between different types of binary trees.

## Table of Contents
- [General Overview](#general-overview)
- [Key Concepts](#key-concepts)
- [Requirements](#requirements)
- [Data Structures](#data-structures)
- [Functionality](#functionality)
- [Print Function](#print-function)
- [Usage](#usage)
- [Authors](#authors)
- [License](#license)

## General Overview

### What is a Binary Tree?
A binary tree is a hierarchical data structure consisting of nodes where each node has at most two children, referred to as the left child and the right child. Each node contains data and pointers to its children.

### Difference between a Binary Tree and a Binary Search Tree (BST)
A binary search tree is a type of binary tree that follows a specific ordering property. In a BST, for each node, all elements in its left subtree are lesser than the node's value, and all elements in its right subtree are greater.

### Time Complexity Gain Compared to Linked Lists
Binary trees can offer improved time complexity over linked lists for certain operations. While linked lists have O(n) time complexity for searching, binary trees, especially BSTs, can achieve O(log n) time complexity for search operations in a balanced tree.

### Properties of a Binary Tree
- **Depth:** The depth of a node in a tree is the number of edges from the root node to that node.
- **Height:** The height of a tree is the maximum depth among all nodes in the tree.
- **Size:** The size of a binary tree is the total number of nodes in the tree.

### Traversal Methods in Binary Trees
Different traversal methods to navigate through a binary tree include:
- **In-order traversal:** Visit left subtree, current node, right subtree.
- **Pre-order traversal:** Visit current node, left subtree, right subtree.
- **Post-order traversal:** Visit left subtree, right subtree, current node.

### Types of Binary Trees
- **Complete Binary Tree:** A binary tree in which every level, except possibly the last, is completely filled, and all nodes are as left as possible.
- **Full Binary Tree:** A binary tree in which every node other than the leaves has two children.
- **Perfect Binary Tree:** A binary tree that is both full and complete, having all levels filled.
- **Balanced Binary Tree:** A binary tree is balanced if the height of the left and right subtrees of any node differ by no more than one.

## Requirements
- Code files should adhere to specific guidelines including compiling on Ubuntu 20.04 LTS using specified flags and allowed editors.
- Follow the Betty style for code formatting.
- Limit the number of functions per file to five and avoid using global variables.

## Data Structures
The following data structures are used for different types of binary trees:
```c
/**
 * struct binary_tree_s - Binary tree node
 *
 * @n: Integer stored in the node
 * @parent: Pointer to the parent node
 * @left: Pointer to the left child node
 * @right: Pointer to the right child node
 */
struct binary_tree_s
{
    int n;
    struct binary_tree_s *parent;
    struct binary_tree_s *left;
    struct binary_tree_s *right;
};

typedef struct binary_tree_s binary_tree_t;
```

Additionally, specific typedefs are used for Binary Search Trees (bst_t), AVL Trees (avl_t), and Max Binary Heaps (heap_t).

## Functionality
The functionality provided in this repository includes various operations and algorithms related to binary trees. The functions are designed to handle basic binary trees that do not necessarily follow any specific rules.

## Print Function
The print function provided in the repository is used solely for visualization purposes and is not required to be pushed to the repository. It aids in visualizing the binary tree structure.

## Usage
To use the functions and structures provided in this repository, include the necessary header file `binary_trees.h` and implement the required functionality in your C programs.

## Authors
This project is authored by FAITH WARIMA NG'ENDO AKA PHARIUM WARIMA.
