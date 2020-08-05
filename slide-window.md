### 滑动窗口（Sliding Window）

滑动窗口是一种解决问题的思路，通常用来解决一些连续问题。一般遇到连续子数组/连续子序列等，要有这样的敏感性。

从类型上来说主要有：

- 固定滑动窗口大小
- 滑动窗口大小不固定，即可变窗口，求最小的满足条件的窗口
- 滑动窗口大小不固定，即可变窗口，求最大的满足条件的窗口

相应的模板为：

```python
for 右指针 in 可迭代对象:
    更新窗口内信息
    判断左指针是否要收缩(窗口内信息满足条件):
        更新最优解
        收缩左指针(更新窗口内信息，移动左指针)
返回最优解

for 右指针 in 可迭代对象:
    更新窗口内信息
    判断左指针是否要收缩(窗口内信息不满足条件):
        收缩左指针(更新窗口内信息，移动左指针)
    更新最优解
返回最优解
```



经典变形：

> 窗口内信息不好统计—>统计窗口外信息，如1234题；
>
> 求解固定数目(K)条件的选择数—>最多K个的选择数-最多K-1个条件的选择数，如930、992、1248题。



#### 相关题目

[209. 长度最小的子数组](https://leetcode-cn.com/problems/minimum-size-subarray-sum/)

[3. 无重复字符的最长子串](https://leetcode-cn.com/problems/longest-substring-without-repeating-characters/)

[76. 最小覆盖子串](https://leetcode-cn.com/problems/minimum-window-substring/)

[438. 找到字符串中所有字母异位词](https://leetcode-cn.com/problems/find-all-anagrams-in-a-string/)

[904. 水果成篮](https://leetcode-cn.com/problems/fruit-into-baskets/)

[930. 和相同的二元子数组](https://leetcode-cn.com/problems/binary-subarrays-with-sum/)

[992. K 个不同整数的子数组](https://leetcode-cn.com/problems/subarrays-with-k-different-integers/)

[1004. 最大连续1的个数 III](https://leetcode-cn.com/problems/max-consecutive-ones-iii/)

[1234. 替换子串得到平衡字符串](https://leetcode-cn.com/problems/replace-the-substring-for-balanced-string/)

[1248. 统计「优美子数组」](https://leetcode-cn.com/problems/count-number-of-nice-subarrays/)