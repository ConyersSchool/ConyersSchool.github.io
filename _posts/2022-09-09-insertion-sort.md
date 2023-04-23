---
title: Insertion sort
author: Nikky Leone
date: 2022-09-09 20:55:00 +0800
categories: [Year 8, Algorithms]
tags: [bubble sort]
---

**An insertion sort is less complex and efficient than a merge sort, but more efficient than a bubble sort.**

**An insertion sort compares values in turn, starting with the second value in the list. If this value is greater than the value to the left of it, no changes are made. Otherwise this value is repeatedly moved left until it meets a value that is less than it. The sort process then starts again with the next value. This continues until the end of the list is reached.**

Consider this unsorted list:

<img src="https://bam.files.bbci.co.uk/bam/live/content/znxhgwx/large" >

12 is the first value in the list. No other values are before it, so the sort moves on to the next value, 14. 14 is greater than the value to the left, 12, so the sort moves on again to the next value, 13. 13 is less than 14, so the two elements are swapped:

<img src="https://bam.files.bbci.co.uk/bam/live/content/zkr9mfr/large" >

13 is greater than 12, so the sort moves onto the next value, 14. 14 is greater than 13, so again the sort moves on.

11 is less than 14, so the two values swap:

<img src="https://bam.files.bbci.co.uk/bam/live/content/z67xvk7/large" >

11 is less than 13, so the two values swap:

<img src="https://bam.files.bbci.co.uk/bam/live/content/zn6prj6/large">

The process repeats:

<img src="https://bam.files.bbci.co.uk/bam/live/content/z626382/large" >

The list is now sorted into order.

Although more efficient than a bubble sort, insertion sorts work best when used with smaller **data** sets. Large data sets are more efficiently handled by merge sorts.

