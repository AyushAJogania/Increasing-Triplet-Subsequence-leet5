# Increasing-Triplet-Subsequence-leet5

_**Problem Description**_
You are given an integer array nums. Your task is to determine if there exists a triplet (i, j, k) in the array such that i < j < k and nums[i] < nums[j] < nums[k]. If such a triplet exists, return true; otherwise, return false.

**Example**
INPUT nums = [1, 2, 3, 4, 5]
OUTPUT true


**Explanation:**
In this case, the array nums contains the triplet (1, 2, 3), where nums[1] < nums[2] < nums[3]. Therefore, the output is true.


**Approach**
To solve this problem with O(n) time complexity and O(1) space complexity, we can use the concept of maintaining two variables to keep track of the smallest and second smallest elements encountered so far. The steps of the approach are as follows:


Initialize two variables, small and big, with maximum integer values.
Iterate through the elements of the array.
If an element is smaller than or equal to small, update small with that element.
If an element is greater than small but smaller than or equal to big, update big with that element.
If an element is greater than both small and big, we have found a valid increasing triplet subsequence, and we can return true.
If we complete the loop without finding a valid triplet, return false.


**Time Complexity Analysis**
The time complexity of this solution is O(n), where n is the length of the input array nums. This is because we iterate through the array only once.

 
**Space Complexity Analysis**
The space complexity of this solution is O(1) as we are using a constant amount of space to store the small and big variables.

  
**Summary**
The "Increasing Triplet Subsequence" problem asks us to determine if there exists a triplet in the given array such that the elements form an increasing subsequence. By maintaining two variables to keep track of the smallest and second smallest elements encountered, we can efficiently solve this problem with O(n) time complexity and O(1) space complexity.
