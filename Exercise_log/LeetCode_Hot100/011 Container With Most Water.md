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


Explanation:The above vertical lines are represented by array [1,8,6,2,5,4,8,3,7]. In this case, the max area of water (blue section) the container can contain is 49.


Input: nums = height = [1,1]
Output:       1

```







## 题目大意



给定一个长度为n的整数(integer)数组，数组元素的大小同时代表圆柱的高度，试着用两个圆柱组成一个有最大容量的容器

不能倾斜(s)容器！

## 解题思路



最大的容量=最大的面积



顺序扫描数组，对每一个元素，在 map 中找能组合给定值的另一半数字，如果找到了，直接返回 2 个数字的下标即可。如果找不到，就把这个数字存入 map 中，等待扫到“另一半”数字的时候，再取出来返回结果。

