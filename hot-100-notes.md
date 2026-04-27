#### 1 两数和
**idea:** 先排序，从两边往中间靠

排序过程保持前后位置映射：
`sorted_nums = sorted(enumerate(nums), key=lambda x: x[1])`
