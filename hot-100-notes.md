#### 1 两数和
**idea:** 先排序，从两边往中间靠

排序过程保持前后位置映射：
`sorted_nums = sorted(enumerate(nums), key=lambda x: x[1])`

#### 49 字母异位词分组
**idea:** 使用字典记录

set可变，不可哈希，因此不可作为字典的key。

可使用：frozenset（元素不重复），tuple(sorted(target))（仅无序，可重复）

#### 128 最长连续序列
**idea:** 使用哈希表

set()转换数组为哈希表时间O(n)， in my_set, my_set.add .remove .discord（删除元素，可以不存在）时间复杂度均为平均O(1)，最坏O(n)，因此做题时可默认为O(1)

#### 283 移动零
**idea:** 使用双指针，进行交换。注意不能改变顺序，因此需要左右指针一起往右走。

list操作除pop() append()外，时间复杂度都是O(n)

#### 11 盛最多水的容器
**idea:** 双指针，递归分析应该移动哪边的指针。
