# The Value of Friendship

A Java 8 implementation using **Disjoint Set Union (DSU)** and a **Greedy approach** to maximize cumulative friendship values in a network.

## Problem Summary
For every edge added to a network, calculate the total number of friendships ($S \times (S-1)$ for each group of size $S$). The goal is to maximize the sum of these totals over all edge additions.

## Solution Logic
1.  **DSU:** Identify final component sizes and count redundant edges.
2.  **Greedy Sort:** Sort final component sizes in descending order to prioritize larger groups.
3.  **Accumulation:** Build components step-by-step, adding the current total friendship to the cumulative sum at each step.
4.  **Redundant Edges:** Add the final maximum friendship value for all remaining extra edges.

## Usage
```bash
javac Solution.java
java Solution < input.txt
