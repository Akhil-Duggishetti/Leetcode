# Leetcode
Leet code solutions
class Solution:
    def twoSum(self, nums: List[int], target: int):
        a={}
        for i,num in enumerate(nums):
            if target-num in a:
                return [a[target-num],i]
            else:
                a[num]=i
