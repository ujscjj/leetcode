### 递归和动态规划

- #### 递归

  定义：是一种直接或间接调用自身函数或方法的算法。

  是从问题的结果倒推，直到问题的规模缩小到寻常；所以要有递归函数和基线情况。

- #### 动态规划

  从寻常入手，逐步扩大规模到最优子结构；所以要有临界条件和状态转移方程。

递归在缩小规模的同时可能会重复计算，比如说爬楼梯问题：

```javascript
function climbStairs(n) {
  if (n === 1) return 1;
  if (n === 2) return 2;
  return climbStairs(n - 1) + climbStairs(n - 2);
}
```

而且每次执行一个函数都有一定的开销，拿JS引擎来说，每次函数执行都会进行入栈操作，执行过程中很容易爆栈。

动态规划则不会出现这些问题：

```javascript
function climbStairs(n) {
  if (n === 1) return 1;
  if (n === 2) return 2;
  let a = 1;
  let b = 2;
  let temp;
  for (let i = 3; i <= n; i++) {
    temp = a + b;
    a = b;
    b = temp;
  }
  return temp;
}
```

因为只涉及到单个因素，只需要一个一维数组即可；对于涉及到多个因素，则需要二维数组等更高维度了，比如说经典的背包问题。

> 爬楼梯没有使用一维数组，而是借助两个变量实现，这样空间复杂度就会比较下，为O(1)。因为爬楼梯问题的状态转移方程之和前两个有关，只需要存储这两个即可。很多时候都可以这样讨巧，但并不是所有的。



#### 动态规划问题需要画表格

动态规划是一种类似查表的问题来缩短时间复杂度和空间复杂度。

画表格的目的就是去不断推导，完成状态转移，表格中的每一个cell都是一个小问题，我们填表的过程其实就是解决问题的过程。我们先解决规模为寻常的问题，然后根据这个结果推导下去，通常情况下，表格右下角是问题的最大规模，也就是我们需要求解的规模。

其实，大部分的动态规划问题套路都是“选择”或者“不选择”。



#### 动态规划问题Tips

- 确定转移方程时，应该考虑是否需要padding来对边界进行处理，以及考虑添加虚拟首部来对边界进行处理；
- 二维dp数组中，内层循环中，要根据i状态下此值可选的次数为无限/1，判断______，决定是顺序循环/还是逆序循环(如322题和416题)；
- 若状态转移方程的i的状态只涉及i-1的状态，那么可以将dp数组减少一个维度；
- 当i状态下存在多种情况时，那么为这多种情况增加一个dp数组的维度即可。



#### 相关题目

[198. 打家劫舍](https://leetcode-cn.com/problems/house-robber/)

[322. 零钱兑换](https://leetcode-cn.com/problems/coin-change/)

[518. 零钱兑换 II](https://leetcode-cn.com/problems/coin-change-2/)

[416. 分割等和子集](https://leetcode-cn.com/problems/partition-equal-subset-sum/)

[139. 单词拆分](https://leetcode-cn.com/problems/word-break/)

[91. 解码方法](https://leetcode-cn.com/problems/decode-ways/)

[309. 最佳买卖股票时机含冷冻期](https://leetcode-cn.com/problems/best-time-to-buy-and-sell-stock-with-cooldown/)









