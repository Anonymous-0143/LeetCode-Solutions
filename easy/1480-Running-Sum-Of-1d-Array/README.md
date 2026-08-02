# [1480. Running Sum of 1d Array](https://leetcode.com/problems/running-sum-of-1d-array/submissions/2091871185/)

![Difficulty](https://img.shields.io/badge/Difficulty-Easy-success)
![Language](https://img.shields.io/badge/Language-python3-blue)
![Runtime](https://img.shields.io/badge/Runtime-Accepted-lightgrey)
![Memory](https://img.shields.io/badge/Memory-Accepted%0A54%20%2F%2054%20testcases%20passed-lightgrey)

## Problem Statement
<p>Given an array <code>nums</code>. We define a running sum of an array as&nbsp;<code>runningSum[i] = sum(nums[0]&hellip;nums[i])</code>.</p>

<p>Return the running sum of <code>nums</code>.</p>

<p>&nbsp;</p>
<p><strong class="example">Example 1:</strong></p>

<pre>
<strong>Input:</strong> nums = [1,2,3,4]
<strong>Output:</strong> [1,3,6,10]
<strong>Explanation:</strong> Running sum is obtained as follows: [1, 1+2, 1+2+3, 1+2+3+4].</pre>

<p><strong class="example">Example 2:</strong></p>

<pre>
<strong>Input:</strong> nums = [1,1,1,1,1]
<strong>Output:</strong> [1,2,3,4,5]
<strong>Explanation:</strong> Running sum is obtained as follows: [1, 1+1, 1+1+1, 1+1+1+1, 1+1+1+1+1].</pre>

<p><strong class="example">Example 3:</strong></p>

<pre>
<strong>Input:</strong> nums = [3,1,2,10,1]
<strong>Output:</strong> [3,4,6,16,17]
</pre>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>1 &lt;= nums.length &lt;= 1000</code></li>
	<li><code>-10^6&nbsp;&lt;= nums[i] &lt;=&nbsp;10^6</code></li>
</ul>


## Constraints
N/A

## Topics
Array, Prefix Sum

## Approach & Complexity
- **Time Complexity**: O(?)
- **Space Complexity**: O(?)

## Solution
```python3
class Solution:
    def runningSum(self, nums: List[int]) -> List[int]:
        result = [nums[0]] if nums else []
      
        for i in range(1, len(nums)):
            result.append(result[-1] + nums[i])
          
        return result

```

> *Generated on 2026-08-02 by [LeetCode Auto Sync](https://github.com/)*
