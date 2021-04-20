# leedcode-liwang
Study note for leetcode.

---
### Easy
* 001 Two Sum  
Using hash map. 

* 020 Valid Parentheses  
Using stack can achieve O(n) space and O(n) time.  
Using Regular match, the complexity depends on the regular algorithm.

* 021 Merge Two Sorted Lists  
Traverse the linked list. O(m+n) time, O(m+n) sapce.  

*0026  Remove Duplicates from Sorted Array  
使用双指针，一个快指针，一个慢指针。开始时，两个指针都指向首元素。当两指针元素值相同时，快指针+1；当两指针元素不同时，慢指针跳到快指针位置，计数器+1。循环，直到快指针遍历完数组。


### Medium 
* 0008 字符串转换整数 (atoi)  
我还是在理解题目的前提下，使用的条件判断来解决，用时不理想，用了53分钟，通过测试，这是不可接受的。  
看了答案，使用的是自动状态机。将字符串抽象成一个类，内部各种状态。这是更高级的玩法，但是第一次看到题目，如果是面试，很难考虑全面，反而容易出错。

* 0078 子集  
我还是使用了循环，试图找到所有可能的子集，然后逐个加入到集合中。方法就是使用循环，显得非常复杂。  
答案使用的是迭代法，巧妙利用python中的列表合并符号 + ，逐个添加元素， 和已存在的列表做加法，然后再合并，效果非常好。参看：https://leetcode-cn.com/problems/subsets/solution/hui-su-suan-fa-by-powcai-5/ 思路二

* 0046 全排列  
我感觉我有点进步，使用了递归来解决这个问题。 递归还是蛮考思维逻辑能力的全面性的。我的问题是，对定义闭包用的不熟悉，python传递参数是形参还是实参理解不透，如果是list要传递形参，必须要重新复制一个新变量。至此。用时1小时。  
题解：可以使用DFS(深度优先遍历)，BFS（广度优先遍历），在这里DFS是更优的解法，即回溯算法，它更节约空间。参看：https://leetcode-cn.com/problems/permutations/solution/quan-pai-lie-by-leetcode-solution-2/  空间复杂度：O(n * n!), 时间复杂度：O(n!) 

* 0022 括号生成 见：https://leetcode-cn.com/problems/generate-parentheses/    
这题我开始过于追求细节， 试图在递归中，将验证规则也加上，导致逻辑有bug,始终得出的答案不完整。 看了解析后，还是原则上使用DFS算法，但是把验证规则剥离开来，逻辑就清晰很多。

* 0094 二叉树的中序遍历  
这个使用递归是比较简单的，我大概10分钟就调通了。 迭代的话，是一个挑战，需要模拟递归的过程，建立一个栈，在实现的过程中有诸多细节需要考虑。

* 0289 生命游戏  
这题相对简单，但是细节要把握好，我由于疲劳，一些边界条件写错了。导致浪费了很多时间。

* 0230 二叉搜索树中第K小的元素  
这题如果采用递归，遍历出所有元素的话，时间复杂度偏高。最好是采用迭代法，遍历的时候到第k个元素即停止。 但是我的疑惑是，为什么在递归算法中，加入了k这个参数，却无法达到要求。

* 0341 扁平化嵌套列表迭代器  
这个题非常的tricky, 它的本质是要让你在初始化的时候，就将嵌套结构的列表，转化为单一整数的列表。 还是考的是对python类的理解和列表的知识，还有就是递归算法。  





* 


