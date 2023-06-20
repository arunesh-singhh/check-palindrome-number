A number is defined as a Palindrome number if it reads the exact same from both forward and backward. And the crazy thing is that it is not only valid to numbers. Even if a string reads the same forwards and backward, then it is a Palindrome as well!

To check if a number is a Palindrome number or not, we first take the input of the number and create a copy of the number taken as an input.
We then create a new variable to store the reversed number and initialize it with 0.
Traverse through the number using mod 10 and division by 10 operations and in each loop make sure to add the digit in the reversed number variable*10.

Example 1:

Input: x = 121
Output: true
Explanation: 121 reads as 121 from left to right and from right to left.
Example 2:

Input: x = -121
Output: false
Explanation: From left to right, it reads -121. From right to left, it becomes 121-. Therefore it is not a palindrome.
Example 3:

Input: x = 10
Output: false
Explanation: Reads 01 from right to left. Therefore it is not a palindrome.

    def isPalindrome(x):
        if x < 0:
            return False
            
        c = x
        b = 0
        while c: 
            b = b * 10 + c % 10
            c //= 10
        return b == x
    
    a = int(input("enter number: "))
    print(isPalindrome(a))
