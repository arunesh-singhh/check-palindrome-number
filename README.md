# check-palindrome-number
check palindrome number

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
