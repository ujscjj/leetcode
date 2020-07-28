### 前缀树问题

前缀树用来解决公共前缀/公共后缀等问题，api主要有以下几个：

> insert(word)：插入一个单词
>
> search(word)：查找一个单词是否存在
>
> startWith(word)：查找是否存在以 word 为前缀的单词

```python
def insert(self, word: str) -> None:
        node = self.root
        for s in word:
            if s not in node:
                node[s] = {}
            node = node[s]
        node['end'] = 1

def search(self, word: str) -> bool:
        node = self.root
        for s in word:
            if s in node:
                node = node[s]
            else:
                return False
        return 'end' in node

def startsWith(self, prefix: str) -> bool:
        node = self.root
        for s in prefix:
            if s in node:
                node = node[s]
            else:
                return False
        return True
```



#### 相关题目

[208. 实现 Trie (前缀树)](https://leetcode-cn.com/problems/implement-trie-prefix-tree/)

[211. 添加与搜索单词 - 数据结构设计](https://leetcode-cn.com/problems/add-and-search-word-data-structure-design/)

[472. 连接词](https://leetcode-cn.com/problems/concatenated-words/)

[212. 单词搜索 II](https://leetcode-cn.com/problems/word-search-ii/)

[1032. 字符流](https://leetcode-cn.com/problems/stream-of-characters/)

[820. 单词的压缩编码](https://leetcode-cn.com/problems/short-encoding-of-words/)