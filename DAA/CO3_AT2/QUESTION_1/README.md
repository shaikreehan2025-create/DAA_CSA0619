# File System Search Optimization Using Binary Search

## Course
Design and Analysis of Algorithms (DAA)

## Title
File System Search Optimization (Binary Search)

## Objective

To analyze how Binary Search improves file retrieval efficiency in a sorted file directory using the divide-and-conquer approach.

## Problem

An operating system maintains sorted file directories for quick access. Binary Search is applied to efficiently locate a requested file.

## Requirements

- File names must be sorted.
- File names must be comparable.
- Efficient access to the middle element is required.

## Algorithm

1. Set the lower and upper search boundaries.
2. Find the middle element.
3. Compare the target file with the middle file.
4. If they match, return the file position.
5. If the target is greater, search the right half.
6. Otherwise, search the left half.
7. Continue until the file is found or the search range becomes empty.

## Divide and Conquer

Binary Search divides the search space into two halves at every step and continues searching only in the relevant half.

## Complexity

### Best Case
O(1)

### Average Case
O(log n)

### Worst Case
O(log n)

### Space Complexity
O(1)

## Files

- `source code .c` – C source code
- `_Report.pdf` – Detailed report

- `README.md` – Project documentation

## Result

Binary Search provides efficient file retrieval from sorted directories. By eliminating half of the remaining files after each comparison, it achieves O(log n) search time and is significantly faster than Linear Search for large sorted datasets.

## Conclusion

Binary Search is an effective file retrieval technique when a directory is maintained in sorted order. Its divide-and-conquer strategy makes it highly suitable for large indexed datasets.
