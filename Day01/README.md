# Day 1 — Shortest Path in Binary Matrix

**LeetCode 1091 — Medium**

### Problem

Given an `n × n` binary matrix, find the shortest clear path from `(0,0)` to `(n-1,n-1)`.

A clear path can move in **8 directions**: horizontal, vertical, and diagonal.

Return the length of the shortest path, or `-1` if no path exists.

### Approach

* Use **BFS** since we need the shortest path in an unweighted grid.
* Store `{distance, {row, col}}` in the queue.
* Check all **8 possible directions** from each cell.
* Mark visited cells as `1` to avoid revisiting them.
* Start with distance `1`.
* Return the distance when the destination is reached.

### Time Complexity

**O(n²)**

### Space Complexity

**O(n²)**

### Learned

BFS can find the shortest path in an unweighted grid, and marking cells visited while adding them to the queue prevents duplicate processing.
