# Question 38 – Quick Sort Performance Using Sampling

## Course
Design and Analysis of Algorithms (DAA)

## Title
Evaluate Quick Sort Performance on Extremely Large Datasets Using Sampling Techniques for Pivot Selection

---

## Objective

To evaluate the performance of Quick Sort on a large dataset by comparing:

1. Standard Quick Sort using a fixed pivot.
2. Quick Sort using median-of-three sampling for pivot selection.

The execution time of both approaches is measured and compared.

---

## Problem Statement

Evaluate Quick Sort performance on extremely large datasets using sampling techniques for pivot selection. Record execution time and compare the results. Analyze how sampling improves pivot quality and interpret the findings to justify its effectiveness.

---

## Approach

### Standard Quick Sort

The last element of the current partition is selected as the pivot.

### Sampling-Based Quick Sort

Three elements are sampled:

- First element
- Middle element
- Last element

The median of these three elements is selected as the pivot.

This technique is called **Median-of-Three Pivot Selection**.

---

## Dataset

The program generates:

**1,000,000 random integer elements**

The same dataset is used for both algorithms to ensure a fair comparison.

---

## Performance Measurement

Execution time is measured using the C `clock()` function.

The program reports:

- Standard Quick Sort execution time
- Sampling Quick Sort execution time
- Whether the resulting arrays are correctly sorted
- Performance comparison

--
## Complexity Analysis

### Average Case

Both approaches have:

**O(n log n)**

### Worst Case

Both can still have:

**O(n²)**

Sampling does not remove the theoretical worst case, but it can improve the probability of selecting a better pivot.

---

## Why Sampling Helps

A pivot close to the middle of the data generally produces more balanced partitions.

Better partitions reduce unnecessary recursive depth and can improve practical performance on large datasets.

Median-of-three sampling adds a small amount of overhead but can make Quick Sort more robust against unfavorable pivot choices.

---

## Files

```text
QUESTION_38/
│
├── source code.c
├──_Report.pdf
├─
└── README.md
```

### File Description

- `source code.c` – C implementation of both Quick Sort approaches.
- `Report.pdf` – Detailed explanation, methodology, complexity analysis, results, and conclusion.

- `README.md` – Project overview and documentation.

---

## Result

The experiment compares standard Quick Sort with sampling-based Quick Sort on a large dataset.

Sampling improves pivot selection by choosing the median of three sampled elements, increasing the likelihood of balanced partitions. Although sampling introduces a small additional overhead, it can improve practical performance and reduce the likelihood of poor partitions.

The average-case complexity remains:

**O(n log n)**

while the theoretical worst-case complexity remains:

**O(n²)**.

---

## Conclusion

Sampling-based pivot selection is an effective practical optimization for Quick Sort when processing large datasets. It improves pivot quality without significantly increasing the algorithm's overall complexity.
