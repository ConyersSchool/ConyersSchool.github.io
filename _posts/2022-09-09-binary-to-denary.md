---
title: Binary to Denary 
author: Nikky Leone
date: 2022-09-09 20:55:00 +0000
categories: [Year 8, Computer Mathematics]
tags: [binary to denary]
math: true
---

**Humans tend to use the denary number system. This is the base 10 system that you are familiar with.** However, computers work in the binary number system, which is base 2. **Denary numbers must be converted into their binary equivalent before a computer can use them.**

**The denary system has ten symbols - 0, 1, 2, 3, 4, 5, 6, 7, 8 and 9.** The value of each denary place value is calculated by multiplying the previous place value by ten. For example:

10,000, 	1,000, 	100, 	10, 	1

**So, the value of the number 124 in denary place values is actually:**


10000 = 0,  1000 = 0,  100 = 1,  10 = 2,  1 = 4


This gives (1 × 100) + (2 × 10) + (4 × 1) = 124.

**Binary to denary**
**The value of each binary place value is calculated by multiplying the previous place value by two. The first eight binary place values are:**

128, 	64,  32, 	16,  8,  4, 	2, 	1


In binary, each place value can only be represented by 1 or a 0.

**To convert binary to denary, simply take each place value that has a 1, and add them together.**

For example, the binary number 1111100 in binary place values is:

128 = 0,  64 = 1,  32 = 1,  16 = 1,  8 = 1,  4 = 1,  2 = 0,  1 = 0

**Result: (0 × 128) + (1 × 64) + (1 × 32) + (1 × 16) + (1 × 8) + (1 × 4) + (0 × 2) + (0 × 1) = 124**

# Denary to binary

**To convert from denary to binary, start by subtracting the biggest place value you can from the denary number, then place a 1 in that place value column. Next, subtract the second biggest place value you can, and place a 1 in the column. Repeat this process until you reach zero.** Finally, place a 0 in any empty place value columns.

**Example: convert denary number 84**

- **First set up the columns of binary place values.**

128, 64, 32, 16, 8, 4,	2, 1

- **64 is the biggest place value that can be subtracted from 84. Place a 1 in the 64 place value column and subtract 64 from 84, which gives 20.**

64 = 1

- **16 is the biggest place value that can be subtracted from 20. Place a 1 in the 16 place value column and subtract 16 from 20, which gives 4.**

64 = 1, 16 = 1 

- **4 is the biggest place value that can be subtracted from 4. Place a 1 in the 4 place value column and subtract 4 from 4, which gives 0.**

64 = 1, 16 = 1, 4 = 1

- **Place a 0 in each remaining empty place value column.**

128 = 0,  64 = 1,  32 = 0,  16 = 1,  8 = 0,  4 = 1,  2 = 0,  1 = 0

- **Result: 84 in denary is 01010100 in binary.**

To check that this is right, convert the binary back to denary:

**(0 × 128) + (1 × 64) + (0 × 32) + (1 × 16) + (0 × 8) + (1 × 4) + (0 × 2) + (0 × 1) = 84**

**Another way to convert a denary number to binary is to divide the starting number by two. If it divides evenly, the binary digit is 0.** If it does not and there is a remainder, the binary digit is 1. Finally, reverse the digits and you have the correct number.

> **Remember**, when coverting binary numbers, try to create a table based on the binary values.
{: .prompt-warning }
