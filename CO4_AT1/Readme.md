#  – Minimum Falling Path Sum

## Course
Design and Analysis of Algorithms (DAA)

## Topic
Minimum Falling Path Sum using Dynamic Programming

## Objective

To find the minimum sum of a falling path from the top row to the bottom row of a square matrix.

At each step, movement is allowed:
- Directly below
- Diagonally left
- Diagonally right

## Sample Input

3

2 1 3
6 5 4
7 8 9

## Expected Output

Min Sum = 13

## Approach

Dynamic Programming is used to store the minimum path sum reaching each cell.

For every cell, the minimum value from the three possible cells in the previous row is selected.

## Recurrence

dp[i][j] = matrix[i][j] + min(
    dp[i-1][j-1],
    dp[i-1][j],
    dp[i-1][j+1]
)

Only valid neighboring positions are considered at the boundaries.

## Complexity

### Time Complexity
O(n²)

### Space Complexity
O(n²)

## Files

- `source code.c` – C source code
- `_Report.pdf` – Complete report
- `README.md` – Project documentation

## Result

For the sample matrix, the minimum falling path is:

1 → 4 → 8

Minimum Sum:

13

## Conclusion

Dynamic Programming efficiently solves the Minimum Falling Path Sum problem by storing previously calculated minimum path values and avoiding repeated computation.
