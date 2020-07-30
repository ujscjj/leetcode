### 字典序列删除

移掉K位数字，使得剩下的数字最小，模板：

```python
stack = []
for digit in num:
	while k > 0 and stack and stack[-1] > digit:
		stack.pop()
		k -= 1
	stack.append(digit)
stack = stack[:-k] if k else stack
return ''.join(stack).lstrip('0') or '0'
```



#### 相关题目

[402. 移掉K位数字](https://leetcode-cn.com/problems/remove-k-digits/)

[316. 去除重复字母](https://leetcode-cn.com/problems/remove-duplicate-letters/)

[1081. 不同字符的最小子序列](https://leetcode-cn.com/problems/smallest-subsequence-of-distinct-characters/)

[321. 拼接最大数](https://leetcode-cn.com/problems/create-maximum-number/)

