# Dynamic Programming

### [1155. Number of Dice Rolls With Target Sum](https://leetcode.com/problems/number-of-dice-rolls-with-target-sum)

> You have d dice, and each die has f faces numbered 1, 2, ..., f.
>
> Return the number of possible ways (out of fd total ways) modulo 10^9 + 7 to roll the dice so the sum of the face up numbers equals target.

* 二維陣列，橫軸為 target 值，縱軸為 dice 數量
* 從 d = 1 開始計算可以達到的 target 位置
* d = 2 開始，累積 target 前面 f 數量的值。那些位置只要加上 1~f 即可達到 target 值

***