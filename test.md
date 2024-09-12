## 2024-09-01

**题目：Two Sum**

**解题思路：**
- 使用哈希表，遍历数组，寻找目标值和当前元素的差值。x

**代码：**
```python
def twoSum(nums, target):
    hash_map = {}
    for i, num in enumerate(nums):
        if target - num in hash_map:
            return [hash_map[target - num], i]
        hash_map[num] = i