### 最大公约数

辗转相除法是计算最大公约数的比较好的方法：

```python
def gcd(a, b):
	return a if b == 0 else gcd(b, a%b)

recude()函数：用传给 reduce 中的函数 function（有两参数）先对集合中的第1、2个元素进行操作，得到的结果再与第三个数据用 function函数 运算，最后得到一个结果。

备足定理：ax+by=z有整数解(a,b),那么z必定是(x,y)的最大公约数的整数倍。
```



#### 相关题目

[914. 卡牌分组](https://leetcode-cn.com/problems/x-of-a-kind-in-a-deck-of-cards/)

[365. 水壶问题](https://leetcode-cn.com/problems/water-and-jug-problem/)

[1071. 字符串的最大公因子](https://leetcode-cn.com/problems/greatest-common-divisor-of-strings/)



