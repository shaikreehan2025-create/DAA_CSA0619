# Edge Coloring Problem Using Backtracking

## Course

Design and Analysis of Algorithms (DAA)

## Topic

Edge Coloring Problem – Backtracking

## Objective

To assign colors to the edges of a graph such that no two adjacent edges share the same color.

## Problem

Two edges are adjacent when they share a common vertex.

Adjacent edges must have different colors.

The program determines whether a valid edge coloring exists using a specified number of colors.

## Approach

Backtracking is used to construct the coloring.

For each edge:

1. Try every available color.
2. Check whether the color conflicts with an adjacent edge.
3. If safe, assign the color.
4. Recursively process the next edge.
5. If the assignment fails, backtrack and try another color.

## Constraints

- Every edge must receive a color.
- Adjacent edges cannot have the same color.
- Only the specified number of colors may be used.

## Complexity

### Time Complexity

Approximately:

O(E × K^E)

where:

- E = number of edges
- K = number of available colors

The algorithm has exponential worst-case behavior.

### Space Complexity

O(E)

## Sample Graph

Edges:

(1,2)
(1,3)
(2,3)
(2,4)
(3,4)

Colors:

3

## Sample Result

A valid coloring can be obtained such as:

(1,2) → Color 1
(1,3) → Color 2
(2,3) → Color 3
(2,4) → Color 2
(3,4) → Color 1

## Files

- `.c_soucecode` – C source code
- `_Report_at1.pdf` – Detailed report
- `README.md` – Project documentation

## Result

The program successfully applies backtracking and constraint checking to find a valid edge coloring when one exists within the specified color limit.

## Conclusion

Backtracking is an effective method for solving small and medium-sized edge-coloring instances. However, its exponential worst-case complexity limits its scalability for very large graphs.
