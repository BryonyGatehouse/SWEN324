# Assignment 4 : Reasoning about Systems

[Explanation of Dafny](/Dafny.md)

This assignment focuses on demonstrating and reasoning about the verification of systems in Dafny.

## Question 1

A palindrome is a word whose spelling is the same forwards and backwards.

Complete the files:
- Write *forallPalin* which uses only one forall statement to checks if a string is a palindrome.
- Write *recPalin* which is primatively recursive (without using quantifiers, etc) and checks if a string is a palindrome.
- Write and verify a lemma that proves that, if *forallPalin* returns true, *recPalin* returns true.
- Write and verify a lemma that proves that, if *recPalin* returns true, *forallPalin* returns true.
- Write and verify a non-recursive method that uses while to check if a string is a palindrome.
- Write and verify a lemma that proves that if *a* and *b* are palindromes (according to *recPalin*) then *a + b + a* is also a palindrome (according to *recPalin*).

## Question 2

A [Trie](https://en.wikipedia.org/wiki/Trie) is a prefix (diverging) n-ary tree.

Complete the following steps:
- Complete the predicate specification that is true if the Trie contains the given string.
- Write a method (using the previous predicate for proof) that creates a Trie with only the given string.
- Write a lemma that proves that the Trie built in the previous method contains only the given string.
- Write a method that checks if a Trie contains the given string using an iterative implementation.
- Complete the function to add a string to the Trie.
- Write a lemma that proves that the string has been added to the Trie.
- Write a lemma that proves a string is still in the Trie when a new string is added.
- Write a function that returns the set of strings in a Trie.

## Question 3

Implement a key-value store using parallel arrays.

## Question 4

In propositional logic, a well formed formula (WFF) is a simple Boolean expression made up from Boolean variables and logical connectives: ¬ (neg), ∧ (and/conjunction, con), ∨ (or/disjunction, dis), => (implies) and ≡ (equivalence, equiv). A WFF is said to be satisfiable if it evaluates to true for some assignment of truth values (true or false) to its variables, and unsatisfiable otherwise. Lots of practical problems can be formulated as Boolean satisfiability problems so that a satisfying assignment for the variables provides a solution to the problem.

Given a WFF (well formed formula) data type, complete the following steps:
- Write a function that returns a set of all variables defined in the WFF.
- Write a recursive function to evaluate a WFF given an environment (the values of the variables).
- Write a function that returns a set of all possible environments in a WFF.
- Write a function that either returns all satisfying assignments (that would make the WFF true), or an empty set if the WFF is unsatisfiable.
- Write an iterative version that evaluate a WFF and verify the returns the same value as the other evaluate method.
