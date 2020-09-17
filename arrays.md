# Arrays
+ [Two Sum](#two-sum)
+ [3Sum](#3Sum)
+ [Subarray Sum Equals K](#subarray-sum-equals-k)

## Two Sum
https://leetcode.com/problems/two-sum/

```python
def twoSum(self, nums, target):
    result=[]
    for i in range(len(nums)-1):
        if nums[i]+nums[i+1]==target:
            result=[i,i+1]
    return result 

```

## 3Sum
https://leetcode.com/problems/3sum/

```python
def threeSum(self, nums):
    result=[]
    for i in range(len(nums)-3):
        for g in range(1,len(nums)-2):
            for l in range (2, len(nums)-1):
                if nums[i]+nums[g]+nums[l]==0:
                    result=[i,g,l]
                    return result
```
```python
def threeSum(self, nums):
        if len(nums) < 3:
            return []
        nums.sort()
        res = set()
        for i, v in enumerate(nums[:-2]):
            if i >= 1 and v == nums[i-1]:
                continue
            d = {}
            for x in nums[i+1:]:
                if x not in d:
                    d[-v-x] = 1
                else:
                    res.add((v, -v-x, x))
        return map(list, res)
```     
## Subarray Sum Equals K
https://leetcode.com/problems/subarray-sum-equals-k/
```python


```
