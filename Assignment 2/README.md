# Assignment 2 : Specifying Programs

All resulting methods need to verify. Additional lemmas might be included.

## Question 1

Create a program that prints out the days of 2020 using a recursive method. Three data types are supplied (Day, Month, Date) which must be used.

## Question 2

Write a program that prints a simple timer. A Timer data type is supplied (contains the time). The *tick* method returns a new *Timer* one second shorter than its argument. The countdown method is recursive and counts down to zero.

## Question 3

Complete a file of specify and implement following functions using a Linked List:
- *foot* which returns the last element if the list has at least one element
- *footOpt* which returns either the last element or (if there isn't any elements) nothing
- *minMaxOpt* which returns either nothing if the list is empty; otherwise the min and max values in the list. Requires a list of integers.
- *sorted* which returns true if the list is sorted. Requires a list of integers.
- *merge* which merges two sorted lists.

## Question 4

Specify and implement a "dictionary" data structure which holds keys and values. The structure should be built using a linked list with the following methods:
- *toMap* which converts the Dictionary to the equivalent map
- *insert* which adds a new key-value pair to the dictionary (doesn't care about duplicate keys)
- *lookup* which returns the associated value given a key
- *contains* which returns true if a key is in the dictionary
- *noDupKeys* which returns true if there are not duplicate keys
- *cull* which returns a new Dictionary without the duplicates of the contained keys (removes all the duplicated keys, keeping one)
