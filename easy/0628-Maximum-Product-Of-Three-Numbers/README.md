# [628. Maximum Product of Three Numbers](https://leetcode.com/problems/maximum-product-of-three-numbers/submissions/2089239268/?envType=daily-question&envId=2026-07-31)

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-success)
![Language](https://img.shields.io/badge/Language-python3-blue)
![Runtime](https://img.shields.io/badge/Runtime-Accepted-lightgrey)
![Memory](https://img.shields.io/badge/Memory-Accepted%0A93%20%2F%2093%20testcases%20passed-lightgrey)

## Problem Statement
<p>Given an integer array <code>nums</code>, <em>find three numbers whose product is maximum and return the maximum product</em>.</p>

<p>&nbsp;</p>
<p><strong class="example">Example 1:</strong></p>
<pre><strong>Input:</strong> nums = [1,2,3]
<strong>Output:</strong> 6
</pre><p><strong class="example">Example 2:</strong></p>
<pre><strong>Input:</strong> nums = [1,2,3,4]
<strong>Output:</strong> 24
</pre><p><strong class="example">Example 3:</strong></p>
<pre><strong>Input:</strong> nums = [-1,-2,-3]
<strong>Output:</strong> -6
</pre>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>3 &lt;= nums.length &lt;=&nbsp;10<sup>4</sup></code></li>
	<li><code>-1000 &lt;= nums[i] &lt;= 1000</code></li>
</ul>


## Constraints
N/A

## Topics
Array, Math, Sorting

## Approach & Complexity
- **Time Complexity**: O(?)
- **Space Complexity**: O(?)

## Solution
```python3
class Solution:
  def maximumProduct(self, nums: list[int]) -> int:
    nums.sort()
    return max(nums[-1] * nums[0] * nums[1],
               nums[-1] * nums[-2] * nums[-3])

```

> *Generated on 2026-07-31 by [LeetCode Auto Sync](https://github.com/)*
