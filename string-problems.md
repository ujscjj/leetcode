### 字符串问题

字符串问题有很多，从简单的实现substr，识别回文，到复杂一点的公共子串/子序列。

专门处理字符串的方法有很多，如 Huffman 树、游程编码、马拉车算法、Trie(前缀树)等等。



#### 回文问题

回文串就是一个正着读和反着读都一样的字符串。判断回文串的通用方法是首尾指针(如题125)；判断最长回文子串的主要方法是“中心扩展法”，如果可以充分利用回文的特点，则可以减少很多重复的计算，典型的是“马拉车算法”。

[125. 验证回文串](https://leetcode-cn.com/problems/valid-palindrome/) 判断一个字符是字母或数字：x.isalpha() or x.isdigit()      x.isalnum()

[131. 分割回文串](https://leetcode-cn.com/problems/palindrome-partitioning/)

[5. 最长回文子串](https://leetcode-cn.com/problems/longest-palindromic-substring/) “中心扩展法”、“马拉车法”

[516. 最长回文子序列](https://leetcode-cn.com/problems/longest-palindromic-subsequence/)

[214. 最短回文串](https://leetcode-cn.com/problems/shortest-palindrome/)



#### 前缀问题

前缀树用来处理这类问题是最符直觉的。但是它也有缺点。比如公共前缀很少的情况下，比较费内存。

[14. 最长公共前缀](https://leetcode-cn.com/problems/longest-common-prefix/)

[208. 实现 Trie (前缀树)](https://leetcode-cn.com/problems/implement-trie-prefix-tree/)





