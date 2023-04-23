---
title: String manipulation
author: Nikky Leone
date: 2022-08-09 20:55:00 +0000
categories: [Year 8, Python]
tags: [string manipulation]
mermaid: true
---

**A string is a variable that holds a sequence of one or more alphanumeric characters.** It is usually possible to manipulate a string to provide information or to alter the contents of a string. The examples below use Python to demonstrate string manipulation:

```python
wordOne = "Computer"

wordTwo = "Science"
```

## Length

**The length of a string can usually be determined using the built-in len function.** This gives the length as an integer.

`len(wordOne)` would give the answer 8 as there are eight characters in the word "*Computer*".

## Character position

**It is possible to determine which character features at a position within a string:**

`wordOne[2]` would give the answer "m" as "m" is the third character in the word “*Computer*” - remember computers generally start counting at zero.

`wordOne[0:2]` would give "*Com*", the first three characters in the string.

`wordOne[3:6]` would give "*put*", the three characters starting from position three.

## Upper and lowercase

**It is possible to change all letters in a string to either upper- or lowercase.** This can be very useful, for example when checking possible inputs.

`topic = "Computer Science".topic = topic.lower()` would give a value for topic of "*computer science*"

`topic = topic.upper()` would give a value for topic of "*COMPUTER SCIENCE*".

## Concatenation

**To concatenate strings means to join them to form another string, eg:**

`sentence = wordOne + " " + wordTwo` would give "*Computer Science*".

Alternatively, a string can be *lengthened* by adding more characters, for example:

`wordOne = wordOne + " Science"` would result in the value of wordOne becoming "*Computer Science*".
