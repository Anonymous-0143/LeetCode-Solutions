# [3345. Smallest Divisible Digit Product I](https://leetcode.com/problems/smallest-divisible-digit-product-i/submissions/2096990924/?envType=daily-question&envId=2026-08-06)

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-success)
![Language](https://img.shields.io/badge/Language-python3-blue)
![Runtime](https://img.shields.io/badge/Runtime-Accepted%0A1000%20%2F%201000%20testcases%20passed-lightgrey)
![Memory](https://img.shields.io/badge/Memory-MB-lightgrey)

## Problem Statement
<p>You are given two integers <code>n</code> and <code>t</code>. Return the <strong>smallest</strong> number greater than or equal to <code>n</code> such that the <strong>product of its digits</strong> is divisible by <code>t</code>.</p>

<p>&nbsp;</p>
<p><strong class="example">Example 1:</strong></p>

<div class="example-block">
<p><strong>Input:</strong> <span class="example-io">n = 10, t = 2</span></p>

<p><strong>Output:</strong> <span class="example-io">10</span></p>

<p><strong>Explanation:</strong></p>

<p>The digit product of 10 is 0, which is divisible by 2, making it the smallest number greater than or equal to 10 that satisfies the condition.</p>
</div>

<p><strong class="example">Example 2:</strong></p>

<div class="example-block">
<p><strong>Input:</strong> <span class="example-io">n = 15, t = 3</span></p>

<p><strong>Output:</strong> <span class="example-io">16</span></p>

<p><strong>Explanation:</strong></p>

<p>The digit product of 16 is 6, which is divisible by 3, making it the smallest number greater than or equal to 15 that satisfies the condition.</p>
</div>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>1 &lt;= n &lt;= 100</code></li>
	<li><code>1 &lt;= t &lt;= 10</code></li>
</ul>


## Constraints
N/A

## Topics
Math, Enumeration

## Approach & Complexity
- **Time Complexity**: O(?)
- **Space Complexity**: O(?)

## Solution
```python3
class Solution:
  def smallestNumber(self, n: int, t: int) -> int:
    return next(num for num in range(n, n + 10)
                if self._getDigitProd(num) % t == 0)

  def _getDigitProd(self, num: int) -> int:
    digitProd = 1
    while num > 0:
      digitProd *= num % 10
      num //= 10
    return digitProd

```

> *Generated on 2026-08-06 by [LeetCode Auto Sync](https://github.com/)*
