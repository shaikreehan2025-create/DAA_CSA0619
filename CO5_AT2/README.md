# Permutation Generation with Position Restrictions

## Course

Design and Analysis of Algorithms (DAA)

## Topic

Permutation Generation with Position Restrictions using Backtracking

---

## Objective

To generate all valid permutations of a set of distinct elements while ensuring that restricted elements are not placed in their prohibited positions.

The solution uses Backtracking to build permutations one position at a time and prunes invalid assignments before deeper recursion.

---

## Problem Statement

Given:

- A set of distinct elements.
- A list of position restrictions.

Generate all permutations that satisfy every position restriction.

For example:

Elements:

A B C D

Restrictions:

- A cannot be placed at position 1.
- C cannot be placed at position 3.

Only permutations satisfying these restrictions are printed.

---

## Approach

The algorithm uses Backtracking.

For each position:

1. Try every unused element.
2. Check whether the element is allowed at the current position.
3. If the element is restricted, reject it immediately.
4. If allowed, place the element.
5. Recursively generate the remaining positions.
6. Remove the element after returning from recursion.
7. Try the next available element.

---

## Pruning

Pruning is performed before making a recursive call.

If an element is not allowed at the current position, the branch is immediately rejected.

This prevents invalid partial permutations from being generated further.

---

## Duplicate Prevention

The `used[]` array keeps track of elements already placed in the current permutation.

Therefore, every element is used exactly once.

The program assumes that the input elements are distinct.

---

## Input Format

```text
Number of elements
Elements
Number of restrictions
Position Element
