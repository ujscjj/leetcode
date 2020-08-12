# 剑指offer

### 面试的基本流程

共享桌面远程面试：

> 思考清楚再开始编码：因为在没有形成清晰的思路之前写出的代码通常会漏洞百出，且会越改越乱；
>
> 能够进行单元测试：**测试在前、开发在后**的程序员太稀缺了；面试官最关心的是应聘者的编程习惯及调试能力。

行为面试：

> 在介绍到项目经验时，应聘者不必详述项目的背景，而要突出介绍自己完成的工作及取得的成绩。

技术面试：

> 遇到复杂的问题，可以通过**画图、举例子分析和分解复杂问题先理清思路再动手编程**；
>
> 还应该不断优化时间效率和空间效率；
>
> 尽量把解决前面问题的思路迁移到后面的问题中去，展示自己良好的学习能力。
>
> 
>
> 1.扎实的基础知识：包括编程语言、数据结构和算法；面试官喜欢问链表和二叉树相关问题，大部分公司注重查找和排序算法(**二分查找、快速排序、归并排序**)。
>
> 2.高质量的代码：**面试官总会关注边界条件、特殊输入等看似细枝末节但实则至关重要的地方**。
>
> 3.清晰的思路：首先，先举几个例子让自己理解问题；其次，可以试着用图形表示抽象的数据结构；最后，可以试着把复杂的问题分解为若干简单的子问题，再一一解决。如很多基于递归的思路，包括分治和动态规划。

应聘者提问：

> 不要问薪水，不要立即打听面试结果；可以问问部门的具体业务、新人培养计划、工作环境等。

### 面试需要的基础知识

数据结构：

> 数组和字符串是两种最基本的数据结构，链表应该是面试题中使用频率最高的一中数据结构。如果面试官想要加大难度，那么他很欧可能会选用与树（尤其是二叉树）相关的面试题。
>
> 栈是一个与递归紧密相关的数据结构，队列在图（包括树）的宽度优先遍历中需要用到，因此也要掌握这两种数据结构。

09.[ 用两个栈实现队列](https://leetcode-cn.com/problems/yong-liang-ge-zhan-shi-xian-dui-lie-lcof) 的拓展—》两个队列实现栈

算法和数据操作：

> 常考算法面试题，很多算法题都可以使用**递归和循环**两种不同的方式实现；基于递归的实现方法代码会比较简洁，但性能不如基于循环的实现方法。
>
> 重点应该掌握**二分查找、快速排序、递归排序**，做到随时正确、完整地写出他们的代码。对插入排序、冒泡排序、快速排序、归并排序等不同算法的优劣要烂熟于胸。（平均时间复杂度、最差时间复杂度、额外空间消耗）
>
> 面试题要求在二维数组上搜索路径，那么应该用**回溯法**；只要当不可以使用递归的时候，再考虑用**栈**来模拟递归的过程。
>
> 如果面试题是求某个问题的最优解，并且该问题可以分为多个子问题，那么应该尝试使用**动态**规划；使用数组保存子问题的最优解。如果分解子问题的时候存在某个最特优的选择，那么该题可能适用于贪婪算法。
>
> 位运算主要包括：与、或、异或、左移、右移。（正数右移前面补0；负数右移前面补1)

11.[旋转数组的最小数字](https://leetcode-cn.com/problems/xuan-zhuan-shu-zu-de-zui-xiao-shu-zi-lcof) 

12.[矩阵中的路径](https://leetcode-cn.com/problems/ju-zhen-zhong-de-lu-jing-lcof) 

13.[机器人的运动范围](https://leetcode-cn.com/problems/ji-qi-ren-de-yun-dong-fan-wei-lcof) 

14-I.[剪绳子](https://leetcode-cn.com/problems/jian-sheng-zi-lcof) 

14-II.[剪绳子 II](https://leetcode-cn.com/problems/jian-sheng-zi-ii-lcof)

15.[二进制中1的个数](https://leetcode-cn.com/problems/er-jin-zhi-zhong-1de-ge-shu-lcof) (x&(x-1)表示将最右边的1变为0；x&(-x)表示只保留最右边的1）

### 高质量的代码

代码的完整性：

> **实现基本功能、边界值、无效的输入**：整数溢出、递归的基线情况要确保能够取到边界值、无效输入;
>
> 处理错误的3中方法：返回0/False、设置全局变量、异常。

**17.**[打印从1到最大的n位数](https://leetcode-cn.com/problems/da-yin-cong-1dao-zui-da-de-nwei-shu-lcof)

**18.**[删除链表的节点](https://leetcode-cn.com/problems/shan-chu-lian-biao-de-jie-dian-lcof/) 

> 原著中附加了待删除结点的指针，要求时间复杂度O(1)：将下一个节点的值赋值给该节点，并把下一个节点删除，需考虑待删除节点是否为尾节点以及该链表是否只有一个节点。
>
> 删除重复节点：输入为空指针、待删除节点位于链表头部/中间/尾部、链表中无重复节点/都是重复节点。

**19.**[正则表达式匹配](https://leetcode-cn.com/problems/zheng-ze-biao-da-shi-pi-pei-lcof/)

**20.**[表示数值的字符串](https://leetcode-cn.com/problems/biao-shi-shu-zhi-de-zi-fu-chuan-lcof/)

**21.**[调整数组顺序使奇数位于偶数前面](https://leetcode-cn.com/problems/diao-zheng-shu-zu-shun-xu-shi-qi-shu-wei-yu-ou-shu-qian-mian-lcof) 

代码的鲁棒性：

> 最好在编程之前考虑所有可能的输入，确保写出的代码在完成了基本功能之外，还考虑了边界条件，并做好了错误处理。
>
> 平时在写代码的时候，应聘者最好养成防御性编程的习惯，在函数入口判断输入是否有效，并对各种无效输入做好相应的处理。

26.[树的子结构](https://leetcode-cn.com/problems/shu-de-zi-jie-gou-lcof) 

### 解决面试题的思路

画图让抽象问题具体化：

> 图形能使抽象的问题具体化、形象化，应聘者说不定通过几幅图形就能找到规律，从而找到问题的解决方案。特别是面试题涉及到链表、二叉树等数据结构时。
>
> 可以画出几幅图形，一边看着图行一遍讲解，面试官就能更加轻松地理解应聘者的思路。这对应聘者是有益的，因为面试官会觉得他具有很好的沟通交流能力。

28.[对称的二叉树](https://leetcode-cn.com/problems/dui-cheng-de-er-cha-shu-lcof) 

29.[顺时针打印矩阵](https://leetcode-cn.com/problems/shun-shi-zhen-da-yin-ju-zhen-lcof) 

举例让抽象问题具体化：

> 当一眼看不出问题中隐藏的规律的时候，我们可以试着用一两个具体的例子模拟操作的过程，这样说不定就能通过具体的例子找到抽象的规律。
>
> 具体的例子有有可以帮助我们向面试官解释算法思路。

31.[栈的压入、弹出序列](https://leetcode-cn.com/problems/zhan-de-ya-ru-dan-chu-xu-lie-lcof) 

**33.**[二叉搜索树的后序遍历序列](https://leetcode-cn.com/problems/er-cha-sou-suo-shu-de-hou-xu-bian-li-xu-lie-lcof) 

分解让复杂问题简单化：

> 当我们遇到复杂的大问题的时候，如果能够先把大问题分解成若干个简单的小问题，然后再逐个解决这些小问题，则可能也会容易很多。分治法、动态规划法等方法的应用都是分解复杂问题的思路。

35.[复杂链表的复制](https://leetcode-cn.com/problems/fu-za-lian-biao-de-fu-zhi-lcof) 

**36.**[二叉搜索树与双向链表](https://leetcode-cn.com/problems/er-cha-sou-suo-shu-yu-shuang-xiang-lian-biao-lcof) 

**37.**[ 序列化二叉树](https://leetcode-cn.com/problems/xu-lie-hua-er-cha-shu-lcof) 

### 优化时间和空间效率

时间效率：

> 面试官除了考查应聘者的编程能力，还关注应聘者有没有不断优化效率、追求完美的态度和能力。
>
> 首先，我们的编码习惯对代码的时间效率有很大的影响。如函数中的值传递，从形参到实参会产生一次复制操作，应尽量避免。
>
> 其次，递归和循环两种思路实现的时间效率可能会大不一样。可以用递归的思路分析问题，写代码的时候用数组来保存中间结果。
>
> 再次，代码的时间效率还体现应聘者对数据结构和算法功底的掌握程度。同样是查找，顺序数组的二分查找时间效率就更低。
>
> 最后，应聘者再面试的时候要展示敏捷的思维能力和追求完美的激情。听到题目的时候，我们一般想到最直观的算法，可能不是最优的，但也不妨在第一时间告诉面试官，这样至少面试官会觉得我们思想比较敏捷；然后思考的时候一定不能轻言放弃，而要表现出积极思考的态度，努力从不同的角度思考问题。面试官希望应聘者能够有激情、有耐心地尝试新思路，而不是碰到难题就退缩。

39.[数组中出现次数超过一半的数字](https://leetcode-cn.com/problems/shu-zu-zhong-chu-xian-ci-shu-chao-guo-yi-ban-de-shu-zi-lcof) 

40.[最小的k个数](https://leetcode-cn.com/problems/zui-xiao-de-kge-shu-lcof) 

**41.**[数据流中的中位数](https://leetcode-cn.com/problems/shu-ju-liu-zhong-de-zhong-wei-shu-lcof) 

43.[1～n整数中1出现的次数](https://leetcode-cn.com/problems/1nzheng-shu-zhong-1chu-xian-de-ci-shu-lcof) 

**44.**[数字序列中某一位的数字](https://leetcode-cn.com/problems/shu-zi-xu-lie-zhong-mou-yi-wei-de-shu-zi-lcof) 

45.[把数组排成最小的数](https://leetcode-cn.com/problems/ba-shu-zu-pai-cheng-zui-xiao-de-shu-lcof) 

**48.**[最长不含重复字符的子字符串](https://leetcode-cn.com/problems/zui-chang-bu-han-zhong-fu-zi-fu-de-zi-zi-fu-chuan-lcof/)

时间效率和空间效率的平衡：

> 以空间换时间，值得注意的是，“以空间换时间”的策略并不一定都是可行的，在面试的时候要具体问题具体分析。

**49.**[丑数](https://leetcode-cn.com/problems/chou-shu-lcof) 

**51.**[数组中的逆序对](https://leetcode-cn.com/problems/shu-zu-zhong-de-ni-xu-dui-lcof) 

### 面试中的各项能力

沟通能力和学习能力:

> 在面试的时候，知之为知之，不知为不知，对于不清楚的知识点，要勇于承认，千万别不懂装懂。

知识迁移能力：

> 知识迁移能力的一种通俗的说法是“举一反三”的能力。我们在去面试之前，通常都会看一些经典的面试题，然而题目总是看不完的，我们不可能把所有的面试题都准备一遍。因此，更重要的是每做一道面试题的时候，都要总结这道题的解法有什么特点，有哪些思路是可以应用到同类型的题目中去的。

**55-II.**[平衡二叉树](https://leetcode-cn.com/problems/ping-heng-er-cha-shu-lcof) 

**56-II.**[数组中数字出现的次数 II](https://leetcode-cn.com/problems/shu-zu-zhong-shu-zi-chu-xian-de-ci-shu-ii-lcof) 

57-II.[和为s的连续正数序列](https://leetcode-cn.com/problems/he-wei-sde-lian-xu-zheng-shu-xu-lie-lcof) 

**58-I.**[翻转单词顺序](https://leetcode-cn.com/problems/fan-zhuan-dan-ci-shun-xu-lcof) 

59-II.[ 队列的最大值](https://leetcode-cn.com/problems/dui-lie-de-zui-da-zhi-lcof) 

**59-I.**[滑动窗口的最大值](https://leetcode-cn.com/problems/hua-dong-chuang-kou-de-zui-da-zhi-lcof) 

抽象建模能力：

> 有些面试官喜欢从日常生活中抽取提炼问题来考察应聘者是否能够建立数学模型并解决问题。要想解决这类问题，应聘者除了需要具备扎实的数学基础和编程能力，还需要具有敏锐的洞察力和丰富的想象力。
>
> 建模的第一步是选择合理的数据结构来表述问题；
>
> 建模的第二部是分析模型中的内在规律，并用编程语言表述这种规律。

60.[ n个骰子的点数](https://leetcode-cn.com/problems/nge-tou-zi-de-dian-shu-lcof) 

61.[ 扑克牌中的顺子](https://leetcode-cn.com/problems/bu-ke-pai-zhong-de-shun-zi-lcof) 

**62.**[圆圈中最后剩下的数字](https://leetcode-cn.com/problems/yuan-quan-zhong-zui-hou-sheng-xia-de-shu-zi-lcof) 

63.[股票的最大利润](https://leetcode-cn.com/problems/gu-piao-de-zui-da-li-run-lcof) 

发散思维能力：

> 在难题面前，应聘者是轻言放弃，还是充满激情地寻找新思路、新方法，具有不同心态的应聘者在面试中的表现是大不一样的。

**64.**[ 求1+2+…+n](https://leetcode-cn.com/problems/qiu-12n-lcof) 

**65.**[不用加减乘除做加法](https://leetcode-cn.com/problems/bu-yong-jia-jian-cheng-chu-zuo-jia-fa-lcof) 

**66.**[构建乘积数组](https://leetcode-cn.com/problems/gou-jian-cheng-ji-shu-zu-lcof) 

两个面试案例：

> 要考虑全面，从基本功能、边界条件和无效处理等方面确保代码的完整性和鲁棒性。
>
> 我把题目说得模棱两可是希望应聘者能够主动向我提出问题，一步一步弄清我的意图。
>
> 如果面试官逐渐加大难度，那么通常是一件好事，这说明应聘者一开始表现得很好，面试官想看看他的水平有多深；如果一开始答得不好，面试官已经判断出他的能力有限，心里已经默默地给出了NO，为了照顾应聘者的情面，也会问几个简单的问题，虽然这些简单的问题应聘者可能都答对，但是前面的结果已经不会改变。

**67.**[把字符串转换成整数](https://leetcode-cn.com/problems/ba-zi-fu-chuan-zhuan-huan-cheng-zheng-shu-lcof/)

**68-I.[**二叉搜索树的最近公共祖先](https://leetcode-cn.com/problems/er-cha-sou-suo-shu-de-zui-jin-gong-gong-zu-xian-lcof) 

68-II.[二叉树的最近公共祖先](https://leetcode-cn.com/problems/er-cha-shu-de-zui-jin-gong-gong-zu-xian-lcof/)











