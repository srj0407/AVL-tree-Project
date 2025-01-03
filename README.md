# AVL-tree-Project

# AVL Tree Implementation in C

This project implements an AVL tree, a self-balancing binary search tree, in C. The repository contains code to create, manipulate, and test AVL trees, with functionalities including insertion, deletion, and tree traversal.

## Features

- **Self-Balancing**: The tree remains balanced after each insertion or deletion using AVL rotations.
- **Efficient Operations**: Ensures \(O(\log n)\) complexity for search, insertion, and deletion.
- **Preorder Traversal**: Displays tree structure for verification and debugging.
- **Memory Management**: Implements safe memory allocation and deallocation.

## File Overview

### Core Files
- **`avl.c`**:
  - Implements AVL tree operations, including insertion, deletion, balancing, and traversal.
  - Contains helper functions for tree rotations and height calculations.

- **`avl.h`**:
  - Header file defining the structures and function prototypes for the AVL tree.

### Test and Utility
- **`test_avl.c`**:
  - A comprehensive test suite for validating the AVL tree implementation.
  - Includes multiple test cases with expected and actual output for preorder traversal.

- **`Makefile`**:
  - Simplifies compilation of the project.
  - Contains targets for building and cleaning the project.

## Compilation and Usage

1. **Compile the Project**:
   Use the `Makefile` to compile the AVL tree code and the test suite:
   ```bash
   make
   ```

2. **Run the Tests**:
   Execute the compiled test program:
   ```bash
   ./test_avl
   ```

3. **Clean Up**:
   To remove generated files, use:
   ```bash
   make clean
   ```

## Example Usage

### Test Case 1
Input:
```c
avl_insert(avl1, 10);
avl_insert(avl1, 20);
avl_insert(avl1, 30);
avl_insert(avl1, 40);
avl_insert(avl1, 50);
avl_insert(avl1, 25);
```

Expected Preorder Traversal:
```
30 20 10 25 40 50
```

### Test Case 2
Input:
```c
avl_insert(avl2, 64);
avl_insert(avl2, 96);
avl_insert(avl2, 32);
avl_insert(avl2, 16);
```

Expected Preorder Traversal:
```
64 24 16 8 40 32 48 88 80 96
```

## Future Enhancements

- Implement a visualizer for AVL tree operations.
- Add more test cases for edge scenarios.
- Optimize rotation logic for improved readability.
