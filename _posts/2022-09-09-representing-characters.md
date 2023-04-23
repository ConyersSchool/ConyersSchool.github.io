---
title: Representing characters 
author: Nikky Leone
date: 2022-08-09 20:55:00 +0000
categories: [Year 8, Computer Mathematics]
tags: [representing characters]
---

**Binary data can represent numbers, graphics, sound and characters. It is then organised and manipulated differently. Data can also be stored in arrays, records or external files and go through validation or verification checks to ensure accuracy.**

# Representation of characters

**Computers work in binary. As a result, all characters, whether they are letters, punctuation or digits, are stored as binary numbers. All of the characters that a computer can use are called a character set.**

Two standards are in common use:

- **American Standard Code for Information Interchange (ASCII)**
- **Unicode**

**ASCII uses seven bits, giving a character set of 128 characters. The characters are represented in a table called the ASCII table. The 128 characters include:**

- **32 control codes (mainly to do with printing)**
- **32 punctuation codes, symbols, and space**
- **26 upper-case letters**
- **26 lower-case letters**
- **numeric digits 0-9**

**We tend to say that the letter ‘A’ is the first letter of the alphabet, ‘B’ is the second and so on, all the way up to ‘Z’, which is the 26th letter. In ASCII, each character has its own assigned number.**

# Denary, binary and hexadecimal representations of ASCII characters

**‘A’ is represented by the denary number 65 (binary 1000001,hexadecimal 41), ‘B’ by 66 (binary 1000010, hexadecimal 42) and so on up to ‘Z’, which is represented by the denary number 90 (binary 1011010, hexadecimal 5A).** Similarly, lower-case letters start at denary 97 (binary 1100001, hexadecimal 61) and end at denary 122 (binary 1111010, hexadecimal 7A).

**When data is stored or transmitted, its ASCII or Unicode number is used, not the character itself.**

For example, the word "Computer" would be represented as:

1000011 1101111 1101101 1110000 1110101 1110100 1100101 1110010


## Extended ASCII

**Extended ASCII uses eight bits, giving a character set of 256 characters. This allows for special characters such as those with accents in languages such as French and Spanish.**

## Unicode

**While suitable for representing English characters, 256 characters is far too small to hold every character in other languages, such as Chinese or Arabic. Unicode uses 16 bits, giving a range of 65,536 characters.** It more suitable for languages with a large number of characters, **but it requires more memory.**
