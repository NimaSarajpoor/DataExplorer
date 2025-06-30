---
title: "leet code 1"
description: "Digging into the leet code probelem 1"
date: "2025-06-27"
categories:
  - python
  - programming
# image: system-design.png
---

Link: https://leetcode.com/problems/two-sum/description/


With the arrival of LLM such as ChatGPT that are capable of answering simple-to-medium questions, getting the code that works for us may not be that hard. However, I still think it is important to understand the problem and the solution. We would like to think about "why". We let LLM handle the "how" part. In this post, we will try to understand the problem and the solution for the first leet code problem: Two Sum.


## Problem Statement
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target. You may assume that each input would have exactly one solution, and you may not use the same element twice. You can return the answer in any order. Example: `nums=[5, 1, 2, 10]`, `target = 15`, the answer is `[0, 3]` because `5 + 10 = 15`.

## Solution
First of all, we need to traverse the whole array. Why? Because the two elements that add up to the target can be anywhere in the array. Second of all, we need to have a way to keep track of the indices. Let's start with a simple solution that uses a nested loop. 

```python
def two_sum(nums, target):
    for i in range(len(nums)):
        for j in range(i + 1, len(nums)):
            if nums[i] + nums[j] == target:
                return [i, j]
    
```

This solution has a time complexity of O(n^2) because we are using a nested loop to traverse the array. This is not efficient for large arrays. Let's see if we can reduce the time complexity to O(n).

```python
def two_sum(nums, target):
    num_to_index = {}
    for i, num in enumerate(nums):
        complement = target - num
        if complement in num_to_index:
            return [num_to_index[complement], i]
        
        num_to_index[num] = i
```

How does this work if we have two elements that are equal, and their sum is equal to the target? Example: `[3, 1, 3, 10]`, `target = 6`. The answer is `[0, 2]` because `3 + 3 = 6`. As we traverse the array, we will add the first `3` to the dictionary with its index `0`. When we reach the second `3`, we will find that the complement `3` is already in the dictionary, and we can return the indices `[0, 2]`.

Note that this solution has the time complexity of O(n) because we are only traversing the array once. The space complexity is also O(n) because we are using a dictionary to store the indices of the elements!

## Think about other stuff
* What if the array is sorted?
* What if the problem does not guarantee that there is exactly one solution? How does the provided solution behave in that case?
    + There is at most one solution.
    + There is at least one solution.

* What if the target is sum of three elements?

