# Arrays
+ [Two Sum](#two-sum)
+ [3Sum](#3Sum)
+ [Subarray Sum Equals K](#subarray-sum-equals-k)

## Two Sum
https://leetcode.com/problems/two-sum/



## 3Sum
https://leetcode.com/problems/3sum/

```python

```
```python

```     
## Subarray Sum Equals K
https://leetcode.com/problems/subarray-sum-equals-k/
```python
def subarraySum(self, nums, k):
    left = 0
    right = 0
    result = 0
    sum = 0
    while(left < len(nums)):
        sum +=nums[right]
        right +=1
        if sum == k:
            result +=1
        if right == len(nums):
            left +=1
            right = left
            sum = 0            
    return result
```
