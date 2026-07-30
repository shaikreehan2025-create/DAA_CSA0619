# CO1 Assignment – Debugging Pair Sum Code

## Student Details

- **Course:** Design and Analysis of Algorithms (DAA)
- **Assignment:** CO1
- **Topic:** Debugging Pair Sum Code (Brute Force)

---

## Repository Structure

```
Question_3/
│
├── Pair_Sum.c
├── Pair_Sum_Report.pdf
├── Output_Screenshot.png
└── README.md
```

---

## Problem Statement

The given Pair Sum algorithm contains a logical error because the `return None` statement is placed inside the outer loop. This causes the function to terminate before checking all possible pairs.

The objective is to:

- Identify the error.
- Debug the algorithm.
- Ensure every valid pair is checked.
- Avoid redundant mirror comparisons.
- Analyze the time complexity.
- Implement the corrected algorithm in C.

---

## Algorithm

1. Read the array elements.
2. Read the target sum.
3. Use the outer loop to select the first element.
4. Use the inner loop starting from `i + 1` to compare the remaining elements.
5. If a pair whose sum equals the target is found, display the indices and values.
6. If no pair exists after checking all combinations, display "No pair found."

---

## Time Complexity

**O(n²)**

The algorithm uses two nested loops to examine all unique element pairs.

---

## Space Complexity

**O(1)**

Only a constant amount of extra memory is used.

---

## Files Included

- **Pair_Sum.c** – C source code
- **Pair_Sum_Report.pdf** – Report containing theory, algorithm, analysis, screenshots, and result
- **Output_Screenshot.png** – Program execution output
- **README.md** – Project description

---

## Result

The Pair Sum algorithm was successfully debugged by moving the `return None` statement outside the outer loop. The corrected program checks all possible pairs before concluding fail
