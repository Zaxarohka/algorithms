# Intervals
+ [non-overlapping-intervals](#non-overlapping-intervals)
+ [merge-intervals](#merge-intervals)
+ [insert-interval](#insert-interval)

## Non-overlapping-intervals
https://leetcode.com/problems/non-overlapping-intervals/
```python
def eraseOverlapIntervals(self, intervals):
        if not intervals:
            return 0
        intervals.sort(key = lambda x: x[0])
        cur_end = intervals[0][1]
        result = 0
        for start, end in intervals[1:]:
            if start < cur_end:
                cur_end = min(cur_end, end)
                result += 1
            else:
                cur_end = end
        return result
        

```

## Merge-intervals
https://leetcode.com/problems/merge-intervals/
```python


```

## Insert-interval
https://leetcode.com/problems/insert-interval/
