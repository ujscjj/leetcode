### 滑动窗口（Sliding Window）

滑动窗口是一种解决问题的思路，通常用来解决一些连续问题。一般遇到连续子数组/连续子序列等，要有这样的敏感性。

从类型上来说主要有：

- 固定滑动窗口大小
- 滑动窗口大小不固定，即可变窗口，求最小的满足条件的窗口
- 滑动窗口大小不固定，即可变窗口，求最小的满足条件的窗口

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


