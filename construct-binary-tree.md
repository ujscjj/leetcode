### 构造二叉树系列

无限递归即可：

```python
def buildTree(self, preorder: List[int], inorder: List[int]) -> TreeNode:
	if preorder == []:
		return None
	value = preorder[0]
    root = TreeNode(value)
    index = inorder.index(value)
	root.left = self.buildTree(preorder[1:index+1], inorder[:index])
	root.right = self.buildTree(preorder[index+1:], inorder[index+1:])
	return root
```



#### 相关题目

[105. 从前序与中序遍历序列构造二叉树](https://leetcode-cn.com/problems/construct-binary-tree-from-preorder-and-inorder-traversal/)

[106. 从中序与后序遍历序列构造二叉树](https://leetcode-cn.com/problems/construct-binary-tree-from-inorder-and-postorder-traversal/)

[889. 根据前序和后序遍历构造二叉树](https://leetcode-cn.com/problems/construct-binary-tree-from-preorder-and-postorder-traversal/)

