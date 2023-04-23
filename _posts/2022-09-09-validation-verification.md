---
title: Validation and Verification 
author: Nikky Leone
date: 2022-08-09 20:55:00 +0800
categories: [Year 7, Database]
tags: [validation and verification]
---

Lesson Objectives:

- Explain what verification is and why it is used. 
 - Create a database that is fully validated.
  - Discuss what validation is and how it helps to reduce human error. 


Validation and verification are two ways to check that the data entered into a computer is correct. Data entered incorrectly is of little use.

# Validation

**Validation is an automatic computer check to ensure that the data entered is sensible and reasonable. It does not check the accuracy of data.
For example, a secondary school student is likely to be aged between 11 and 16. The computer can be programmed only to accept numbers between 11 and 16. This is a range check.** 

However, this does not guarantee that the number typed in is correct. For example, a student's age might be 14, but if 11 is entered it will be valid but incorrect.

# Types of validation

There are a number of validation types that can be used to check the data that is being entered.



|Validation type | How it works                                      | Example usage                                                                                  |
|:---------------|:--------------------------------------------------|-----------------------------------------------------------------------------------------------:|
| Check digit    | The last one or two digits are correct            |Bar code readers in supermarkets use check digits                                               |
| Format check   | Checks the data is in the right format            |A National Insurance number is in the form LL 99 99 L where L is any letter and 9 is any number |
| Length check   | Checks the data isn't too short or too long       |A password which needs to be six letters long                                                   |
| Lookup table   | Looks up acceptable values in a table             |There are only seven possible days of the week                                                  |
| Presence check | Checks that data has been entered into a field    |In most databases a key field cannot be left blank                                              |
| Range check    | Checks if a value falls within the specified range|Number of hours worked must be less than 50 and more than 0                                     |
| Spell check    | Looks up words in a dictionary	                   |When word processing                                                                            |










