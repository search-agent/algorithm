* 题目：排序数组
* 思路： 归并排序（Merge Sort）是基于分治思想的排序算法。它将数组分成两半，分别对两半进行排序，然后将排序好的两半合并成一个有序的数组
* 解题过程： 
  1. 拆分（mergeSortArray）：
     1. 递归地将数组分成两部分，直到每个部分只有一个元素（自然有序）。
     2. 然后合并这些有序的子数组。
  2. 合并（merge）：
     1. 合并两个有序的子数组 nums[left..mid] 和 nums[mid+1..right]。
     2. 使用两个临时数组 L 和 R 分别存储两个子数组的元素。
     3. 将 L 和 R 中的元素按顺序合并回 nums。

