# Assignment 3 : Verifying Programs

[Explaination of Dafny](/Dafny.md).

This assignment is about verifying programs.

## Question 1

                          *          row=1 printed=1
                         * *         row=2 printed=3
                        * * *        row=3 printed=6
                       * * * *       row=4 printed=10
                      * * * * *      row=5 printed=15
                     * * * * * *     row=6 printed=21
                    * * * * * * *    row=7 printed=28
                   * * * * * * * *   row=8 printed=36
                  * * * * * * * * *  row=9 printed=45
                 * * * * * * * * * * row=10 printed=55

Complete the file to embody a formal mathematical and graphical proof of the closed form of triangular numbers. Use the provided functions instead of printing anything directly. Ensure that the complier can prove that the code printed is correct (conditions).

## Question 2

Complete the files to find the largest absolute difference between successive elements in an array of integers. Each step should be verified by the Dafny compiler:
- Compute the sequences of differences between sequence elements
- Prove it is correct
- Write an iterative implementation of the first step
- Write a fuction that computes the maximum absolute value of a sequence of integers so, when given the result of the first step, will give the maximum absolute difference.

## Question 3

Complete the files to specify and implement a binary search Tree (linked list version). Includes the following methods:
- Returning the size of the Tree
- Converting the Tree into a Set
- Checking if the Tree is a valid binary search Tree (all subtrees are valid, all values in left are smaller than the node's value, and all value on right are larger)
- Checking if the Tree contains a value
- Checking if the Tree contains a value using an iterative approach
- Converting the Tree into a Set using an iteractive approach

## Question 4 : Addition

Complete the files to add two [arbitrary precision natural numbers](https://en.wikipedia.org/wiki/Arbitrary-precision_arithmetic). Includes the following methods:
- Returns the value of a Number
- Returns the value of a Number using an iterative approach
- Adds two Numbers
