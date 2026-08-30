# Assembly Line Scheduling vs Word Break – Dynamic Programming

## Course

Design and Analysis of Algorithms (DAA)

## Topic

Assembly Line Scheduling vs Word Break (DP Comparison)

## Objective

To solve Assembly Line Scheduling and Word Break using Dynamic Programming and compare their recurrence relations, decision-making, constraints, complexity, and scalability.

## Problems Covered

### 1. Assembly Line Scheduling

Finds the minimum time required to process a product through two assembly lines.

The algorithm decides whether to:

- Stay on the current line
- Switch to the other line

Time Complexity:

O(n)

Space Complexity:

O(n)

### 2. Word Break

Determines whether a string can be divided into valid words from a given dictionary.

Example:

applepie = apple + pie

Basic DP complexity:

O(n²) position checks

Space Complexity:

O(n)

## Dynamic Programming

Both problems use previously calculated results to avoid repeated computation.

Assembly Line Scheduling uses a minimum-cost decision:

min(stay, switch)

Word Break uses a Boolean decision:

possible valid segmentation

## Comparison

| Feature | Assembly Line | Word Break |
|---|---|---|
| Type | Optimization | Decision |
| DP Value | Minimum cost | Boolean |
| Complexity | O(n) | O(n²) basic DP |
| Main Decision | Stay/Switch | Word boundary |
| Input | Station times | String + dictionary |

## Files

- `.c_sourceccode` – C source code
- `_Report.pdf` – Complete report
- `README.md` – Project documentation

## Result

Both problems were successfully solved using Dynamic Programming.

Assembly Line Scheduling has O(n) time complexity, while Word Break requires O(n²) position checks in its basic DP formulation.

## Conclusion

The comparison demonstrates the versatility of Dynamic Programming. It can be used for optimization problems such as Assembly Line Scheduling and decision problems such as Word Break.
