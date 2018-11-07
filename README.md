# leetcode
数据结构和算法的学习

## 学习数据结构和算法的好处
提升编程能力，理解当红技术
1. 区块链的结构就是一个链表（linked list），每一个区块的指针指向前一个区块。
2. 每一个区块内的结构是`二叉树`（Binary Tree），Merkle Tree。

## 如何有效学习算法和数据结构
《异类-不一样的成功启示录》

>一万小时定律

### 三个方法
* Chunk it up（切碎知识点）
* Deliberate practicing（刻意练习）
* Feedback（反馈）

### 常见的数据结构

|-- Data Structure --|-- Algorithm --|
|----|----|
|Array 数组           |Greedy 贪婪算法       |
|Stack 栈/Queue 队列    |Recursion 循环/Backtrace 回溯|
|Priority Queue 优先队列|In/Pre/Post-order Traversal 中序/前序/后续遍历|
|Linked List 链表|Breadth-first/Depth-first search 广度优先/深度优先搜索|
|Tree 树/Binary Search Tree 二叉搜索树|Divide and Conquer 分治法|
|Hash Table 哈希表|Dynamic Programming 动态规划|
|Disjoint Set 并查集|Binary Search 二分查找|
|Trie 字典树|Graph 图形算法|
|Bloom Filter 布鲁姆过滤||
|LRU Cache 本地缓存类||

### 切题四件套
* Clarification
* Possible solutions
    - compare(time/space)
    - optimal（加强）
* Coding（多写）
* Test cases

## Big O notation
O(1): Constant Complexity 常数复杂度
O(log n): logarithmic Complexity 对数复杂度   
    二分查找时间复杂度即为O(log n)
O(n): Linear Complexity 线性复杂度   
    二叉树的遍历为O(n)，每个节点遍历一次
    排序的二维矩阵查找为O(n)，一维O(log n)
O(n^2): N square Complexity 平方
O(n^3): N cube Complexity 立方
O(2^n): Exponential Growth 指数
O(n!): Factorial 阶乘
    快排、归并排序 O(n*log n)

### Array数组
内存里一段连续的存储区域
时间复杂度：
Access 查询O(1)
Insert 插入、Delete 删除操作O(n)，链式复杂度

### Linked List 链表
与数组对比，改善了插入O(1)和删除O(1)操作
查询操作挪指针，O(n)

### Doubly Linked List 双链表
既有前驱，也有后继指针
时间复杂度同上

### Stack - First in Last out(FILO)
    Array or Linked List
### Queue - First in First out(FIFO)
    Array or Doubly Linked List

### Priority Queue 优先队列
    正常入，按照优先级出
#### 实现机制（面试需了解，不需代码实现）
1. Heap 堆（Binary 二叉堆，Binomial 多项式堆， Fibonacci 斐波那契堆）
2. Binary Search Tree 二叉搜索树（也称有序二叉树ordered，排序二叉树sorted），是指一棵空树或者具有下列性质的二叉树：
   * 左子树上所有结点的值均小于它的根节点的值
   * 右子树上所有结点的值均大于它的根节点的值
   * Recursively，递归的，左、右子树也分别为二叉搜索树

Mini Heap 小顶堆（越小的越靠上）
>父亲节点比左右孩子小，最小元素在堆顶

Max Heap 大顶堆
堆的维基百科：需要了解不同堆的复杂度即可，严格斐波拉契堆是效率最好的。
https://en.wikipedia.org/wiki/Heap_(data_structure)

哈希函数映射到哈希表
哈希碰撞常见的解决做法是拉链法

哈希表 时间复杂度O(1) 但是乱序
二叉搜索树 时间复杂度O(log n) 但是有序

链表Linked List是特殊化的树Tree
树Tree是特殊化的图Graph

前序遍历：根左右
中序遍历：左根右
后序遍历：左右根
