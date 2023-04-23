---
title:  Spreadsheet applications
author: Nikky Leone
date: 2022-08-09 20:55:00 +0000
categories: [Year 8, Spreadsheet design]
tags: [spreadsheets applications]
---

**There are many different features available within spreadsheet applications. Six of the most common, and most important, are listed below:**

## Conditional formatting

**You can apply formats to individual cells or a range of cells. The formatting will change depending on the value of the cell. For example, you can have a cell appear with a red background and the data itself coloured red when the value of the cell is greater than 10.**

<img src="https://bam.files.bbci.co.uk/bam/live/content/zwx8rwx/medium" alt="picture 1">

## Importing data

**When an application is able to read a file created by another application, this is called 'importing'. Spreadsheets will allow you to import data from databases, text files and websites.**

## Headers and footers

**A header is an area set aside at the top of each sheet. Within this area you can include information that you want repeated on each sheet in the workbook. A footer is an area set aside at the bottom of each sheet. Within this area you will often find page numbering, file names and dates.** This is often only visible when printed.

## IF statements

**An IF statement checks to see if a statement is true or false and then does one of two things depending on the result. It can be represented as:**

`=IF(Evaluate Condition, Do this if true, Do this if false)`

**For example, if daily sales for a company are greater than £30 then there has been a profit, if they are less than £30 there has been a loss.**

`=IF(D6>30,"Profit","Loss")` can be entered into an empty cell to show whether a profit or a loss has been made.

<img src="https://bam.files.bbci.co.uk/bam/live/content/zqhj97h/medium" alt="picture 2">

## VLOOKUP

**Short for 'Vertical Lookup'. In spreadsheets it is very common to want to 'look up' one thing and compare against another.**

For example, you may want to look up the price of a certain product. VLOOKUP allows you to find a value within a table. You will need the following information in your VLOOKUP formula:

`=VLOOKUP(lookup value, range containing the lookup value, column number in the range containing the return value)`

**The formula in cell F1 needs to look up the value 'Pear' in the column labelled 'Product' and return the relevant value from the second column - 'Price'. This can be achieved using the formula:**

`=VLOOKUP("pear",A2:B5,2)`

<img src="https://bam.files.bbci.co.uk/bam/live/content/zxfmw6f/medium" alt="Picture 3">
