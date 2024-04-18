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
- [算法:灵茶山艾府](https://space.bilibili.com/206214/channel/collectiondetail?sid=842776&ctype=0)

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

### [34.在排序数组中查找元素的第一个和最后一个位置](https://leetcode.cn/problems/find-first-and-last-position-of-element-in-sorted-array/solution/er-fen-cha-zhao-zong-shi-xie-bu-dui-yi-g-t9l9/)
### [162.寻找峰值](https://leetcode.cn/problems/find-peak-element/solution/by-endlesscheng-9ass/)
### [153.寻找旋转排序数组中的最小值](https://leetcode.cn/problems/find-minimum-in-rotated-sorted-array/solution/by-endlesscheng-owgd/)
### [33.搜索旋转排序数组](https://leetcode.cn/problems/search-in-rotated-sorted-array/solution/by-endlesscheng-auuh/)
