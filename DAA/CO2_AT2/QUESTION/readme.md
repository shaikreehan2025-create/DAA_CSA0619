
# CO1 Assignment – Brute Force Pattern Matching

## Course
Design and Analysis of Algorithms (DAA)

## Title
Brute Force Pattern Matching in a Document Editor

## Problem Statement

Implement the Brute Force Pattern Matching algorithm to locate keywords in a document. Explain the working process, analyze its time complexity, and justify the need for more efficient algorithms.

## Files Included

- Pattern_Matching.c
-_Report.pdf
- README.md

## Algorithm

1. Read the text.
2. Read the pattern.
3. Compare the pattern with every possible position in the text.
4. If all characters match, display the starting position.
5. If no match exists, display "Pattern not found."

## Time Complexity

- Best Case: O(m)
- Average Case: O(nm)
- Worst Case: O(nm)

## Space Complexity

O(1)

## Result

The Brute Force Pattern Matching algorithm successfully searches for a keyword in the given text. Although it is simple and easy to implement, its O(nm) worst-case time complexity makes it less efficient than algorithms such as KMP, Boyer-Moore, and Rabin-Karp for large documents.
