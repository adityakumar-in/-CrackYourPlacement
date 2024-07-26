#CrackYourPlacement

# Problem Solving

- ## Valid Parenthesis String
    https://leetcode.com/problems/valid-parenthesis-string/description/ \
    ```In this I used two pointer approach (min, max) and loop through the string and check if the current character is '(' then increment max & min by 1 else if it's ')' then decrement max & min by 1 and if it's '*' then increment max & decrement min by 1. In the end check if min<0 then set min to 0 (As we have to check the third condition for * also) & if max<0 then return false (as parenthesis itself is invalid so no need to check for *). After loop end return [min==0].```

- ## Valid Parenthesis
    https://leetcode.com/problems/valid-parentheses/description/ \
    ```I use Stack in this, I loop through the string and check if the current character is '(' or '{' or '[' then push it in the stack and if ')' or '}' or ']' is found then i check if the top of stack is '(' or '{' or '[' respectively then i pop() from the stack, in between if stack is empty then it's invalid parenthesis, and at last if stack is empty then it's valid parenthesis.```

- ## Find the Index of the First Occurrence in a String
    https://leetcode.com/problems/find-the-index-of-the-first-occurrence-in-a-string/description/ \ 
    ```In this I used sliding window technique, I loop through the string and by substring function I check if the current substring is equal to the given string then return the index, if not return -1.```

- ## Valid Palindrome II
    https://leetcode.com/problems/valid-palindrome-ii/description/ \
    ```In this I used palindrome technique but for one delete operation, I used a outer function to check if it's palindrome or not, i check for the both the ends [delete right & delete left] and if it's palindrome then return true else return false.```

- ## Integer to Roman
    https://leetcode.com/problems/integer-to-roman/description/ \
    ```I used vector to store notations with it's values and loop until number is not equal to 0 and check if current number is greater than the notation value, if yes then i divide the value and add the notation to result accordingly. if not i decrement to next notation value and check the same condition again, that's how i got the roman number.```