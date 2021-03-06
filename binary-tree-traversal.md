### 二叉树的遍历

- #### 前中后序遍历的递归/迭代算法

  - 前中后序列遍历递归算法比较简单；
  - 前序遍历迭代算法稍难，需要借助栈(出栈时再做输出，先进后出)；
  - 中序遍历迭代算法再加些难度，关键点在于：针对每一个结点，出栈时判断结点是否有右子节点，若有，则重复上述步骤；
  - 后序遍历迭代算法则于前序遍历相同，最后逆序即可。

  题目：[144. 二叉树的前序遍历](https://leetcode-cn.com/problems/binary-tree-preorder-traversal/) [94. 二叉树的中序遍历](https://leetcode-cn.com/problems/binary-tree-inorder-traversal/) [145. 二叉树的后序遍历](https://leetcode-cn.com/problems/binary-tree-postorder-traversal/)

- #### 层次遍历的迭代算法

  层序遍历遍历需要借助队列，关键点在于，外循环之内需要一个queue长的内循环来输出这一层的结点值。

  题目：[102. 二叉树的层序遍历](https://leetcode-cn.com/problems/binary-tree-level-order-traversal/)

  

#### 相关题目

[230. 二叉搜索树中第K小的元素](https://leetcode-cn.com/problems/kth-smallest-element-in-a-bst/)

[104. 二叉树的最大深度](https://leetcode-cn.com/problems/maximum-depth-of-binary-tree/)

[701. 二叉搜索树中的插入操作](https://leetcode-cn.com/problems/insert-into-a-binary-search-tree/)

[110. 平衡二叉树](https://leetcode-cn.com/problems/balanced-binary-tree/)

[98. 验证二叉搜索树](https://leetcode-cn.com/problems/validate-binary-search-tree/)

[236. 二叉树的最近公共祖先](https://leetcode-cn.com/problems/lowest-common-ancestor-of-a-binary-tree/)

[124. 二叉树中的最大路径和](https://leetcode-cn.com/problems/binary-tree-maximum-path-sum/)









