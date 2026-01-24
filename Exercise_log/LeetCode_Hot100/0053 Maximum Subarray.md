# [0053.Maximum Subarray](https://leetcode.cn/problems/maximum-subarray/?envType=study-plan-v2&envId=top-100-liked](https://leetcode.cn/problems/maximum-subarray/description/?envType=study-plan-v2&envId=top-100-liked)



## 题目



Given an integer array `nums`, find the subarray with the largest sum, and return _its sum_.



Example:



```

Input: nums = [-2,1,-3,4,-1,2,1,-5,4]
Output: 6
Explanation:The subarray [4,-1,2,1] has the largest sum 6.



Input: nums = [1]
Output: 1
Explanation:The subarray [1] has the largest sum 1.



Input: nums = [5,4,-1,7,8]
Output: 23
Explanation:The subarray [5,4,-1,7,8] has the largest sum 23.
```







## 题目大意



给定一个整数数组，找到带有最大和的zi'shu'zu

## 解题思路



最大的容量=最大的面积



左右两个双指针，不断比较两元素所代表的高度，移动较小的那一个（左指针右移，右指针左移），以寻求最大面积
