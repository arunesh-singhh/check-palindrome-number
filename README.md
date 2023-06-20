# check-palindrome-number
A number is defined as a Palindrome number if it reads the exact same from both forward and backward. And the crazy thing is that it is not only valid to numbers. Even if a string reads the same forwards and backward, then it is a Palindrome as well! 

To check if a number is a Palindrome number or not, we first take the input of the number and create a copy of the number taken as an input.

We then create a new variable to store the reversed number and initialize it with 0.

Traverse through the number using mod 10 and division by 10 operations and in each loop make sure to add the digit in the reversed number variable*10.
