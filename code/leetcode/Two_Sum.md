## QUESTION
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.
You may assume that each input would have exactly one solution, and you may not use the same element twice.
You can return the answer in any order.

### SOLUTION 1
```{python}
class Solution(object):
    def twoSum(self, nums, target):
        for i, num_one in enumerate(nums):
            for j, num_two in enumerate(nums):
                total = num_one + num_two 
                if i == j:
                    continue
                elif total == target:
                    return [i,j]

        """
        :type nums: List[int]
        :type target: int
        :rtype: List[int]
        """
```   
