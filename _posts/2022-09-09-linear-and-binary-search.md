---
title: Linear and Binary search
author: Nikky Leone
date: 2022-09-09 20:55:00 +0800
categories: [Year 8, Algorithms]
tags: [linear and binary search]
---

An example of a computer searching algorithm is linear search. This is a simple algorithm used to find a value in a list of data. The algorithm runs as follows:

- Identify a search term.
- Look at the first item in the list.
- Compare the item with the search term.
- Is the current item the same as the search term? If so, the item has been found. If not, move to the next item.
- Repeat from step two until the last item in the list has been reached.
- If the end of the list has been reached and the search term has not been found, then the search term is not in the list and the algorithm can stop.

# Linear search example

This algorithm could be used to search the following list for the number 1:

3, 2, 4, 1, 5

The algorithm would produce:

- 3, 2, 4, 1, 5 (1 compared to 3 - not found)

- 3, 2, 4, 1, 5 (1 compared to 2 - not found)

- 3, 2, 4, 1, 5 (1 compared to 4 - not found)

- 3, 2, 4, 1, 5 (1 compared to 1- found)

Because the linear search algorithm simply moves up the list and checks each item, the data in the list does not need to be in order. However, as the list gets longer the algorithm takes longer to run, making it inefficient for large lists.

In [**pseudo-code**](https://www.bbc.co.uk/bitesize/guides/z3bq7ty/revision/2), this may look like:

```pseudocode
find <-- 1
found <-- False
length <-- length(list)
counter <-- 0


WHILE found = False AND counter <= length
     IF list[counter] = find THEN
          found <-- True
          OUTPUT 'Found at position', counter
        ELSE
          counter <-- counter + 1
        ENDIF
ENDWHILE
IF found = False THEN
   OUTPUT 'Item not found'
ENDIF
```


# Binary search

Binary search is a 'divide and conquer' algorithm which requires the initial array to be sorted before searching.

It is called binary because it splits the array into two halves as part of the algorithm. Initially, a binary search will look at the item in the middle of the array and compare it to the search terms.

This leads to three possible scenarios:

- Search criteria = middle item: Item Found
- Search criteria is less than middle item: Search the first half of the array
- Search criteria is larger than middle item: Search the upper half of the array

The process of dividing the array continues until the middle item meets the search criteria.

The binary search algorithm can be expressed by the following [**pseudo-code**](https://www.bbc.co.uk/bitesize/guides/z3bq7ty/revision/2):

```
OUTPUT "Which customer do you want to find?"
INPUT user inputs John Smith
STORE the user's input in the customer_name variable
customer_found = False
(a flag that identifies if the customer is found)

WHILE customer_found = False:
  Find midpoint of list
  IF customer_name = record at midpoint of list THEN
    customer_found = True
  ELSE IF customer comes before the midpoint THEN
    throw away the second half of the list
  ELSE 
    throw away the first part of the list
    OUTPUT customer details
array = [3, 14, 15, 29, 31, 35, 40, 66, 68, 98]
length = list.length                                     
number = input("What number would you like to find?")
lowerBoundry = 0
upperBoundry = length – 1
match = false
while match == false AND lowerBoundry != upperBoundry
  midPoint = round((lowerBoundry + upperBoundry)/2)
  if array[midPoint] == number then
    print("We have found your number!")
    match = true
  elseif array[midPoint] - < number then
    lowerBoundry = midPoint + 1
  else
    upperBoundry = midPoint – 1
  endif
endwhile
```

This can be simplified as:

- Let n = length of the array, let min = 0 and max = n-1
Calculate guess as the average of max and min, rounded down (so it is an integer)
- If array[guess] equals target, then stop. You found it. Return guess
- If the guess was too low, that is, array[guess] - < target, then set min = guess + 1
- Otherwise, the guess was too high. Set max = guess - 1
- Go back to step 2
- Evaluating linear and binary searches
- 
Although a binary search is a little harder to program, it is far more efficient than a linear search.

Example: For an array with 16 elements, the best case scenario is that a binary search will find the element on the first go and, in the worst case, on the fourth go (24 = 16).

For an array with 1 million elements, this would mean a worst case scenario of 20 goes, while the worst case for a linear search of 1 million items would be 1 million probes.

When should you use a binary search?
- If the list is large and changing often, with items constantly being added or deleted, then the time it takes to constantly re-order the list to allow for a binary search might be longer than a simple serial search in the first place
- If the list is large and static (e.g., a database of telephone numbers), then a binary search is very fast compared to a linear search (in maths terms it takes 2log2(n) for a binary search over n items)
- If the list is small, then it might be simpler to use a linear search
- If the list is random, then a linear search is the only way to search
- If the list is skewed so that the most often searched items are placed at the beginning then, on average, a linear search is likely to be better


