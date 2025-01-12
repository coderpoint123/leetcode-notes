## Python Cheat Sheet 🐍

DAY 1
1. **Concatenation of Array**:
Link: https://leetcode.com/problems/concatenation-of-array/description/

Code: class Solution:
    def getConcatenation(self, nums: List[int]) -> List[int]:
        a=nums+nums
        return a

2.**Contains Duplicate**
Link: https://leetcode.com/problems/contains-duplicate/description/

Code: class Solution:
    def containsDuplicate(self, nums: List[int]) -> bool:
        nums.sort()
        for i in range(1,len(nums)):
            if nums[i]==nums[i-1]:
                return True
        return False

3. **Valid Anagram**
Link : https://leetcode.com/problems/valid-anagram/description/
Code : class Solution:
    def isAnagram(self, s: str, t: str) -> bool:
        return sorted(s)==sorted(t)

4. **Replace Elements With Greatest Element On Right Side**
Link : https://leetcode.com/problems/replace-elements-with-greatest-element-on-right-side/submissions/849338516/
Code : class Solution:
    def replaceElements(self, arr: List[int]) -> List[int]:
        maxNum = -1
        for i in range(len(arr) - 1, -1, -1):
            last = maxNum
            maxNum = max(maxNum, arr[i])
            arr[i] = last
        return arr

  
