The Palindrome Challenge

1.

Pseudocode:

a) get the word
b) set left pointer at index 0 (start)
c) set right pointer at last index (end)
d) while left pointer < right pointer: compare character at left with character at right, if they are different, return "not a palindrome", if they are the same - move left pointer forward and right pointer backward
e) if the loop completes - return "it's a palindrome"

2.

# Creating the function with a word parameter
def palindrome_func(word):
    
    # Setting the left and right pointers
    leftpointer = 0    
    rightpointer = len(word) - 1

    # As long as the left (0) is smaller than right

    while leftpointer < rightpointer :
       # If characters are not the same, stop and return that it's not
       if word[leftpointer] != word[rightpointer]:
         return "Not a palindrome"
       # If are the same, add one to the left, remove 1 from the right
       leftpointer += 1
       rightpointer -= 1

    # If all checks have been done, return that it is
    return "It's a palindrome"

# Test cases
print(palindrome_func("racecar"))
print(palindrome_func("hello"))
print(palindrome_func("A man a plan a canal Panama"))


Used claude for this one. As for the time complexity, my approach was the most efficient one, as it can stop right after the first check compared with the approach claude suggested. The other was "reserve the words, check the characters and when you finish all the checks, give the result". The edge cases that are included in test, are the empty string, single character. The last test has spaces, capitals, and if you run it, it says it's not a palindrome. In real life though, this sentence is a palindrome. If my approach wasn't so strict, this would be a palindrome too. The approach with the reserved words is simpler, as claude says, but mine is more efficient.

3.

Honest Reflection on AI Use

I really liked the fact that i took time to think the problem. Used ai for understanding deeper the core of palindrome effect and how it works with code/words. I believe i analyse the problem more than before, which probably means that i practised my thinking approach? something like that. Not without making syntax mistakes for sure. Rewriting it would be possible if i practise python on a daily basis.