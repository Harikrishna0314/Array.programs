# Trapping Rain Water — Java

A Java implementation of the **Trapping Rain Water** problem using the **two-pointer technique**. The program calculates the total amount of rainwater that can be trapped between bars of different heights. This is a common Data Structures and Algorithms problem that focuses on arrays, two pointers, and optimization.

## Problem Statement

Given an array of non-negative integers where each element represents the height of a bar and the width of every bar is `1`, calculate how much rainwater can be trapped between the bars after rainfall.

### Example

```text
Input:
[0,1,0,2,1,0,1,3,2,1,2,1]

Output:
6
```

The amount of water trapped depends on the tallest boundaries on the left and right of each position.

## Approach

This solution uses the **two-pointer approach** to solve the problem efficiently.

Two pointers are initialized:

* `left` — starts from the beginning of the array.
* `right` — starts from the end of the array.
* `leftMax` — stores the maximum height encountered from the left.
* `rightMax` — stores the maximum height encountered from the right.

At every step, the pointer on the side with the smaller height is processed. If the current height is lower than the maximum boundary on that side, water can be trapped at that position.

## Algorithm

1. Initialize `left` and `right` pointers.
2. Initialize `leftMax`, `rightMax`, and `totalWater`.
3. Compare the heights at the two pointers.
4. Process the side with the smaller height.
5. Update the corresponding maximum height.
6. Calculate and add trapped water when the current bar is lower than the maximum.
7. Continue until the two pointers meet.
8. Return the total trapped water.

## Complexity

| Complexity | Value    |
| ---------- | -------- |
| Time       | **O(n)** |
| Space      | **O(1)** |

The two-pointer method achieves linear time while using constant extra space, making it more memory-efficient than approaches that store left/right maximum arrays.

## Technologies

* Java
* Arrays
* Two-Pointer Technique
* Data Structures & Algorithms

## Learning Outcomes

Through this problem, I practiced:

* Array traversal
* Two-pointer technique
* Maintaining running maximum values
* Optimizing time and space complexity
* Solving an array-based DSA problem efficiently
