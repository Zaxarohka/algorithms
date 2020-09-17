# Arrays
+ [Two Sum](#two-sum)
+ [3Sum](#3Sum)
+ [Subarray Sum Equals K](#subarray-sum-equals-k)

## Two Sum
https://leetcode.com/problems/two-sum/



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
## Subarray Sum Equals K
https://leetcode.com/problems/subarray-sum-equals-k/
```python


```
