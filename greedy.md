### 贪婪策略

贪婪策略是一种常见的算法思想，具体是指，在对问题求解时，总是做出在当前看来是最好的选择。也就是说，不从整体最优加以考虑，它所做出的是在某种意义上的局部最优解。贪心算法不是对所有问题都能得到整体最优解，关键在于贪心策略的选择，选择的贪心策略必须具备无后效性，即某个状态以前的过程不会影响以后的状态。这点和动态规划类似，大多数情况下也是用来处理极值问题。



#### 相关题目

[55. 跳跃游戏](https://leetcode-cn.com/problems/jump-game/)

[45. 跳跃游戏 II](https://leetcode-cn.com/problems/jump-game-ii/) 实现方式较为巧妙，借助 i 、end。 

[1024. 视频拼接](https://leetcode-cn.com/problems/video-stitching/) 实现方式较为巧妙，借助 left、right。

[1326. 灌溉花园的最少水龙头数目](https://leetcode-cn.com/problems/minimum-number-of-taps-to-open-to-water-a-garden/)

