# DoThreeSumSolution.cpp 三数求和，解题思路
* 思路：数组需要做基础排序，遍历数组，双指针滑动匹配
* 解题过程
  * 排序数组：使用 std::sort 对数组进行排序。
  * 遍历数组：
    * 使用一个 for 循环固定第一个数。
    * 在固定第一个数之后，使用两个指针，一个指向当前数的下一个位置，另一个指向数组末尾。
  * 双指针法：
    * 计算三个数的和，如果和为零，则记录这个三元组。
    * 如果和小于零，则将左指针右移以增加和。
    * 如果和大于零，则将右指针左移以减小和。
  * 去重：
    * 在固定第一个数时，如果当前数和前一个数相同，则跳过。
    * 在找到一个和为零的三元组后，跳过重复的元素。