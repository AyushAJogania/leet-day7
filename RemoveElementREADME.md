# leet-day7


**LeetCode Problem: Remove Element**


You are given an integer array nums and an integer val. Your task is to remove all occurrences of val in nums in-place and return the number of elements in nums that are not equal to val.

Input

nums: A vector of integers representing the input array.

val: An integer representing the value to be removed from nums.

Output

Return an integer representing the new size of the array without occurrences of val.

Input: nums = [3, 2, 2, 3], val = 3

Output: 2

Explanation: The function should return `k = 2`, with the first two elements of `nums` being 2.

**Constraints**

0 <= nums.length <= 100

0 <= nums[i] <= 50

0 <= val <= 100


_**Approach and Solution**_

The solution uses the two-pointer technique to remove all occurrences of val in-place. It keeps track of the new size of the array without occurrences of val using a variable k. The function iterates through the array using a for loop and if the current element is not equal to val, it moves the element to the position indicated by k and increments k. The function finally returns k, which represents the new size of the array without occurrences of val.

