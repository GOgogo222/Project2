# [0189 Rotate Array](https://leetcode.cn/problems/rotate-array/description/?envType=study-plan-v2&envId=top-100-liked)



## 题目



Given an integer array `nums`, rotate the array to the right by `k` steps, where `k` is non-negative.



Example:



```

Input: nums = [1,2,3,4,5,6,7], k = 3
Output: [5,6,7,1,2,3,4]
Explanation:rotate 1 steps to the right: [7,1,2,3,4,5,6]
rotate 2 steps to the right: [6,7,1,2,3,4,5]
rotate 3 steps to the right: [5,6,7,1,2,3,4]


Input: nums = [-1,-100,3,99], k = 2
Output: [3,99,-1,-100]
Explanation:rotate 1 steps to the right: [99,-1,-100,3]
rotate 2 steps to the right: [3,99,-1,-100]
```




## 题目大意



给定一个整数数组，找到带有最大和的子数组，并返回这个值



子数组是一个数组中连续的非空元素序列


## 解题思路



若当前指针所指元素之前的和小于0，则丢弃**当前元素之前**的序列