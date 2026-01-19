# [011.Container With Most Water](https://leetcode.cn/problems/container-with-most-water/description/?envType=study-plan-v2&envId=top-100-liked)


## 题目



You are given an integer array `height` of length `n`. There are `n` vertical lines drawn such that the two endpoints of the `ith` line are `(i, 0)` and `(i, height[i])`.

Find two lines that together with the x-axis form a container, such that the container contains the most water.

Return _the maximum amount of water a container can store_.

**Notice** that you may not slant the container.



Example:



```

Input: height = [1,8,6,2,5,4,8,3,7]
Output: 49


Input: nums = [0]
Output:       [0]

```







## 题目大意



给定一个整数数组，把数组中的0元素都移到数组的后面并保持其他元素的位置



~~注意，不可复制该数组~~



## 解题思路



这道题最优的做法时间复杂度是 O(n)。



顺序扫描数组，对每一个元素，在 map 中找能组合给定值的另一半数字，如果找到了，直接返回 2 个数字的下标即可。如果找不到，就把这个数字存入 map 中，等待扫到“另一半”数字的时候，再取出来返回结果。

