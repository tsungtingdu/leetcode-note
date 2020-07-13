# Array

### [54. Spiral Matrix](https://leetcode.com/problems/spiral-matrix/)
> Given a matrix of m x n elements (m rows, n columns), return all elements of the matrix in spiral order.

* simulation (what I did), but using "direction matrix"
* layer-by-layer
* transpose array (!)

***
### [88. Merge Sorted Array](https://leetcode.com/problems/merge-sorted-array/)

> Given two sorted integer arrays nums1 and nums2, merge nums2 into nums1 as one sorted array.

> Note: The number of elements initialized in nums1 and nums2 are m and n respectively.
You may assume that nums1 has enough space (size that is equal to m + n) to hold additional elements from nums2.

* start from the end of final array
***

### [118. Pascal's Triangle](https://leetcode.com/problems/pascals-triangle/)
> Given a non-negative integer numRows, generate the first numRows of Pascal's triangle.

***
### [283. Move Zeroes](https://leetcode.com/problems/move-zeroes/)

> Given an array nums, write a function to move all 0's to the end of it while maintaining the relative order of the non-zero elements.

> Note:
> 1. You must do this in-place without making a copy of the array.
> 2. Minimize the total number of operations.

* append non-zero number, then create zeros at the end
***
### [414. Third Maximum Number](https://leetcode.com/problems/third-maximum-number/)

> Given a non-empty array of integers, return the third maximum number in this array. If it does not exist, return the maximum number. The time complexity must be in O(n).

***
### [448. Find All Numbers Disappeared in an Array](https://leetcode.com/problems/find-all-numbers-disappeared-in-an-array/)

> Given an array of integers where 1 ≤ a[i] ≤ n (n = size of array), some elements appear twice and others appear once.

> Find all the elements of [1, n] inclusive that do not appear in this array.

> Could you do it without extra space and in O(n) runtime? You may assume the returned list does not count as extra space.

* create "tag" on current value! (so no need to create another array for comparision)

***
### [498. Diagonal Traverse](https://leetcode.com/problems/diagonal-traverse/)

> Given a matrix of M x N elements (M rows, N columns), return all elements of the matrix in diagonal order as shown in the below image.

* diagonal Iteration first, then reverse
* simulation (like what I did)

***
### [905. Sort Array By Parity](https://leetcode.com/problems/sort-array-by-parity/)

> Given an array A of non-negative integers, return an array consisting of all the even elements of A, followed by all the odd elements of A. You may return any answer array that satisfies this condition.

* write even numbers first, then odd numbers (two for loops)
* quick sort (two pointer, from start and back)

***
### [941. Valid Mountain Array](https://leetcode.com/problems/valid-mountain-array/)

> Given an array A of integers, return true if and only if it is a valid mountain array...

* there is only one peak
* count steps of first walking up then first walking down
***
### [1051. Height Checker](https://leetcode.com/problems/height-checker/)

> Students are asked to stand in non-decreasing order of heights for an annual photo.

> Return the minimum number of students that must move in order for all students to be standing in non-decreasing order of height.

> Notice that when a group of students is selected they can reorder in any possible way between themselves and the non selected students remain on their seats.

```js
const heightChecker = (heights) => {
    return [...heights].sort((a,b) => a - b).reduce((a,c,i) => c != heights[i] ? a+1 : a,0)
}
```
* without sorting (but counting sort?)

***
