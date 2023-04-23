---
title: Selection in Python
author: Nikky Leone
date: 2022-08-09 20:55:00 +0800
categories: [Year 8, Python]
tags: [selection]
---

**Programs are designed using common building blocks, known as programming constructs.** These programming constructs form the basis for all programs.

# Selection

**Selection is a programming construct where a section of code is run only if a condition is met. In programming, there are occasions when a decision needs to be made.** Selection is the process of making a decision. The result of the decision determines which path the program will take next.

For example, **a program could tell a user whether they are old enough to learn how to drive a car. If the user's age meets the required driving age, the program would follow one path and execute one set of statements. Otherwise, it would follow a different path and execute a different set of statements.**

Selection works by testing a condition. The test gives a Boolean result - **TRUE or FALSE.**

In programming, selection is implemented using **IF THEN ELSE** statements:

'''pseudocode
OUTPUT “How old are you?”
age ← USERINPUT
IF age > 16 THEN
     OUTPUT "You are old enough to drive a car"
ELSE
     OUTPUT "Come back when you are older!"
ENDIF'''


In the above pseudo-code program, the path the program takes depends on the condition. A variable, in this case age, is used to test the condition.

**If the value of age is greater than 16, the result of the tested condition is TRUE and the program follows the first path, which follows the statement THEN. This path outputs to the user that they are old enough to drive.**

If the value of age is less than 16, the result is FALSE and the program follows the second path, **which follows the statement ELSE.** This path outputs to the user that they are not yet old enough to drive.

The statement 'ENDIF' ends the selection block.
