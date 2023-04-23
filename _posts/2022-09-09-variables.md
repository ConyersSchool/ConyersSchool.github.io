---
title:  Working with variables
author: Nikky Leone
date: 2022-08-09 20:55:00 +0000
categories: [Year 8, Python]
tags: [variables]
---

You can use variables to store numbers.

```python
pocket_money = 20
```

The variable ‘pocket_money’ is used to store how much pocket money you have. Right now you have £20.

As well as using fixed numbers in calculations and storing the answer in a variable, we can also use variables within the calculations themselves. In this example, the instruction uses the variable ‘money_in_bank’ to calculate the answer and then stores the answer in a variable called ‘total_money’.

total_money = money_in_bank + 10
The variables represent any value we choose to assign to them.

Consider this Python (3.x) program:

```python
>>> money_in_bank = 20
>>> total_money = money_in_bank + 10
>>> print(total_money)
30
```

The first line stores the value 20 to the variable ‘money_in_bank’. Since the computer knows that ‘money_in_bank’ has the value 20, it can calculate the value of ‘total_money’ and store it. Once calculated, the value of ‘total_money’ can be printed to the screen.

Once a value is stored, all sorts of mathematical operations can be performed on the variables:

```python
>>> money_in_bank = 20
>>> total_money = money_in_bank + 10
>>> print(total_money)
30
>>> cost_of_holiday = 150
>>> left_to_pay = cost_of_holiday - total_money
>>> print(left_to_pay)
120
```

> Using variables means the exact amounts that are being used don’t have to be remembered - the computer stores the numbers for us.
Working with text
{: .prompt-tip }

A variable can hold a number, but it can also hold a piece of text. Just one letter is called a character. More than one character is called a string.

A text variable works in the same way as a number variable, with a couple of differences:

text variables hold characters (letters, digits, punctuation)
the data in text variables is placed in quotes
arithmetic calculations cannot be performed on text variables
Consider the following Python (3.x) program that uses strings:

```python
>>> message = "Hooray! It's my birthday!"
>>> print(message)
Hooray! It's my birthday!
```
> Data in a character or string has quotes placed around it. This tells the computer that we are using text and not a number.
{: .prompt-tip }
