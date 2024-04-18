# iOS基础
## OC Runtime
[OC之Runtime](https://juejin.cn/post/6914203330277769230)
## OC Runloop
[深入理解RunLoop](https://blog.ibireme.com/2015/05/18/runloop/)
## OC Block

## OC 内存管理

# 面试知识点
iOS：
- [iOS RoadMap](https://roadmap.isylar.com/)
- [Swift Programming Language](https://docs.swift.org/swift-book/documentation/the-swift-programming-language)
- [Programming with Objective-C](https://developer.apple.com/library/archive/documentation/Cocoa/Conceptual/ProgrammingWithObjectiveC/Introduction/Introduction.html#//apple_ref/doc/uid/TP40011210-CH1-SW1)

计算机基础：
- [CS自学指南](https://csdiy.wiki/)
- [编程指北](https://csguide.cn/)
- [算法:OI Wiki](https://oi-wiki.org/basic/)
- [算法:灵茶山艾府-基础算法精讲](https://space.bilibili.com/206214/channel/collectiondetail?sid=842776&ctype=0)

# 算法
> 算法的***正确性***是前提，不能盲目套模版。如果没有思路，先考虑暴力求解，找到特点/规律后逐步优化。

## 1. 相向双指针
> 对应`灵茶山艾府-基础算法精讲`的第1、2集。

使用数组头尾的2个指针，***相向***移动双指针，遍历数组来求解。
可用双指针算法求解的题目，需要满足指针移动的正确性，例如***单调性***。
### [167.两数之和 II - 输入有序数组](https://leetcode.cn/problems/two-sum-ii-input-array-is-sorted/solution/san-shu-zhi-he-bu-hui-xie-xiang-xiang-sh-6wbq/)
### [15.三数之和](https://leetcode.cn/problems/3sum/solution/shuang-zhi-zhen-xiang-bu-ming-bai-yi-ge-pno55/)
### [11.盛最多水的容器](https://leetcode.cn/problems/container-with-most-water/solution/by-endlesscheng-f0xz/)
### [42.接雨水](https://leetcode.cn/problems/trapping-rain-water/solution/zuo-liao-nbian-huan-bu-hui-yi-ge-shi-pin-ukwm/)

## 2. 滑动窗口
> 对应`灵茶山艾府-基础算法精讲`的第3集。

窗口是由窗口头尾2个指针包含的一个***连续***区间，在数组中***滑动***这个窗口来求解。属于同向双指针。
### [209.长度最小的子数组](https://leetcode.cn/problems/minimum-size-subarray-sum/solution/biao-ti-xia-biao-zong-suan-cuo-qing-kan-k81nh/)
### [3.乘积小于 K 的子数组](https://leetcode.cn/problems/subarray-product-less-than-k/solution/xia-biao-zong-suan-cuo-qing-kan-zhe-by-e-jebq/)
### [713.无重复字符的最长子串](https://leetcode.cn/problems/longest-substring-without-repeating-characters/solution/xia-biao-zong-suan-cuo-qing-kan-zhe-by-e-iaks/)

## 3. 二分查找
> 对应`灵茶山艾府-基础算法精讲`的第4、5集。

二分查找和相向双指针类似，使用数组头尾的2个指针，且相向移动指针：在2个指针的中间值将区间分为红色区间、蓝色区间（***红蓝染色法***），不断减半直到找到目标值。所以时间复杂度是O(LogN)。
头尾两个指针各自有开区间、闭区间的写法(一共4种写法)，不同写法需要对应的判断和移动指针。
### [34.在排序数组中查找元素的第一个和最后一个位置](https://leetcode.cn/problems/find-first-and-last-position-of-element-in-sorted-array/solution/er-fen-cha-zhao-zong-shi-xie-bu-dui-yi-g-t9l9/)
### [162.寻找峰值](https://leetcode.cn/problems/find-peak-element/solution/by-endlesscheng-9ass/)
### [153.寻找旋转排序数组中的最小值](https://leetcode.cn/problems/find-minimum-in-rotated-sorted-array/solution/by-endlesscheng-owgd/)
### [33.搜索旋转排序数组](https://leetcode.cn/problems/search-in-rotated-sorted-array/solution/by-endlesscheng-auuh/)

## 4. 链表：反转链表
> 对应`灵茶山艾府-基础算法精讲`的第6集。

遍历链表：模拟每个节点需要的操作。
### [206.反转链表](https://leetcode.cn/problems/reverse-linked-list/solution/you-xie-cuo-liao-yi-ge-shi-pin-jiang-tou-o5zy/)
### [92.反转链表 II](https://leetcode.cn/problems/reverse-linked-list-ii/solution/you-xie-cuo-liao-yi-ge-shi-pin-jiang-tou-teqq/)
### [25.K 个一组翻转链表](https://leetcode.cn/problems/reverse-nodes-in-k-group/solution/you-xie-cuo-liao-yi-ge-shi-pin-jiang-tou-plfs/)

## 5. 链表：快慢指针
> 对应`灵茶山艾府-基础算法精讲`的第7集。

### [876.链表的中间结点](https://leetcode.cn/problems/middle-of-the-linked-list/solution/mei-xiang-ming-bai-yi-ge-shi-pin-jiang-t-wzwm/)
### [141.环形链表](https://leetcode.cn/problems/linked-list-cycle/solution/mei-xiang-ming-bai-yi-ge-shi-pin-jiang-t-c4sw/)
### [142.环形链表 II](https://leetcode.cn/problems/linked-list-cycle-ii/solution/mei-xiang-ming-bai-yi-ge-shi-pin-jiang-t-nvsq/)
### [143.重排链表](https://leetcode.cn/problems/reorder-list/solution/mei-xiang-ming-bai-yi-ge-shi-pin-jiang-t-u66q/)

## 5. 链表：删除节点题
> 对应`灵茶山艾府-基础算法精讲`的第8集。

遍历链表。
### [237.删除链表中的节点](https://leetcode.cn/problems/delete-node-in-a-linked-list/solutions/2004056/ru-he-shan-chu-jie-dian-liu-fen-zhong-ga-x3kn/)
### [19.删除链表的倒数第 N 个结点](https://leetcode.cn/problems/remove-nth-node-from-end-of-list/solutions/2004057/ru-he-shan-chu-jie-dian-liu-fen-zhong-ga-xpfs/)
### [83.删除排序链表中的重复元素](https://leetcode.cn/problems/remove-duplicates-from-sorted-list/solutions/2004062/ru-he-qu-zhong-yi-ge-shi-pin-jiang-tou-p-98g7/)
### [82.删除排序链表中的重复元素 II](https://leetcode.cn/problems/remove-duplicates-from-sorted-list-ii/solutions/2004067/ru-he-qu-zhong-yi-ge-shi-pin-jiang-tou-p-2ddn/)

## 6. 二叉树 & 递归
> 对应`灵茶山艾府-基础算法精讲`的第9、10、11、12集。

递归原理：***数学归纳法***，像多米诺骨牌一样 传递的推倒相同的牌，直到终止条件。  
递归模版：递归函数=多米诺骨牌，重复的调用自己；终止条件：牌堆末尾，判断推导是否结束。
```
递归函数() {
  满足终止条件：return
  否则：递归函数()
}
```
### [104.二叉树的最大深度](https://leetcode.cn/problems/maximum-depth-of-binary-tree/solution/kan-wan-zhe-ge-shi-pin-rang-ni-dui-di-gu-44uz/)
### [100.相同的树](https://leetcode.cn/problems/same-tree/solution/ru-he-ling-huo-yun-yong-di-gui-lai-kan-s-empk/)
### [101.对称二叉树](https://leetcode.cn/problems/symmetric-tree/solution/ru-he-ling-huo-yun-yong-di-gui-lai-kan-s-6dq5/)
### [110.平衡二叉树](https://leetcode.cn/problems/balanced-binary-tree/solution/ru-he-ling-huo-yun-yong-di-gui-lai-kan-s-c3wj/)
### [199.二叉树的右视图](https://leetcode.cn/problems/binary-tree-right-side-view/solution/ru-he-ling-huo-yun-yong-di-gui-lai-kan-s-r1nc/)
### [98.验证二叉搜索树](https://leetcode.cn/problems/validate-binary-search-tree/solution/qian-xu-zhong-xu-hou-xu-san-chong-fang-f-yxvh/)
### [236.二叉树的最近公共祖先](https://leetcode.cn/problems/lowest-common-ancestor-of-a-binary-tree/solutions/2023872/fen-lei-tao-lun-luan-ru-ma-yi-ge-shi-pin-2r95/)
### [235.二叉搜索树的最近公共祖先](https://leetcode.cn/problems/lowest-common-ancestor-of-a-binary-search-tree/solutions/2023873/zui-jin-gong-gong-zu-xian-yi-ge-shi-pin-8h2zc/)

## 7. 二叉树：层序遍历
> 对应`灵茶山艾府-基础算法精讲`的第13集。

层序遍历属于***广度优先搜索***(BFS,Breadth First Search)，用***队列***保存节点。另外，***深度优先搜索***(DFS,Depth First Search)，用***栈***保存节点。
### [102.二叉树的层序遍历](https://leetcode.cn/problems/binary-tree-level-order-traversal/solution/bfs-wei-shi-yao-yao-yong-dui-lie-yi-ge-s-xlpz/)
### [103.二叉树的锯齿形层序遍历](https://leetcode.cn/problems/binary-tree-zigzag-level-order-traversal/solution/bfs-wei-shi-yao-yao-yong-dui-lie-yi-ge-s-xlv3/)
### [513.找树左下角的值](https://leetcode.cn/problems/find-bottom-left-tree-value/solution/bfs-wei-shi-yao-yao-yong-dui-lie-yi-ge-s-f34y/)

