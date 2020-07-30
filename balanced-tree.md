### 平衡二叉树

平衡二叉树的定义:

> 一个二叉树每个节点的左右两个子树的高度差的绝对值不超过1.



如果要判断一棵树是否为平衡二叉树，只需要死扣定义，然后用递归即可轻松解决。

```python
def height(root):
	if root == None:
		return 0
	return max(height(root.left), height(root.right)) + 1
def dfs(root):
	if root == None:
		return True
	return dfs(root.left) and dfs(root.right) and abs(height(root.left) - height(root.right)) <= 1
	
return dfs(root)
```

如果需要将一个数组或者链表（逻辑上都是线性的数据结构）转化为平衡二叉树，则可以选择排序数组(或链表)的中点，左边的元素为左子树， 右边的元素为右子树即可。



#### 相关题目

[110. 平衡二叉树](https://leetcode-cn.com/problems/balanced-binary-tree/)

[108. 将有序数组转换为二叉搜索树](https://leetcode-cn.com/problems/convert-sorted-array-to-binary-search-tree/)

[109. 有序链表转换二叉搜索树](https://leetcode-cn.com/problems/convert-sorted-list-to-binary-search-tree/)

[1382. 将二叉搜索树变平衡](https://leetcode-cn.com/problems/balance-a-binary-search-tree/)





