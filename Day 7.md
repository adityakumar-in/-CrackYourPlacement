#CrackYourPlacement

# Problem Solving

- ## Simplify Path
    https://leetcode.com/problems/simplify-path/description/ \
    ```I loop through the string & find the words inside two '/' & then check if the word is '.' or '' then i do nothing, if the word is '..' (if stack is not empty) then i pop the last element from the stack, else i push the word into the stack. Finally i join the stack with '/' and return the result.```

- ## Reverse Words in a String
    https://leetcode.com/problems/reverse-words-in-a-string/description/ \
    ```I loop through the string & find the words inside two ' ' & then i push the word into the stack (if the word is not empty i.e., '') and finally i join the stack with ' ' and return the result.```

- ## Basic Calculator II
    https://leetcode.com/problems/basic-calculator-ii/description/ \
    ```I loop through the string & check if digit, if YES then i simply add digit to a number, if NO (then it's operator) then i check the last operator [+ (i initialized it with '+')] and then i perform the operation result+=lastNumber, now i update the last number according to the current operator (lastNumber or -lastNumber) and continue the loop, same i do for * & /, i * and / with lastNumber & currentNumber  and at last i make currentNumber=0 and sin = currentChar when loop one iteration is done. at last i do result+=lastNumber (if last operation was * or / then the result is stored in lastNumber) and return the result.```

- ## Valid Number
    https://leetcode.com/problems/valid-number/description/ \
    ```A number can be valid only on four condition - 1. Digit (it should contain digits) 2. Dot (it should contain only one dot & dot is not at begining [if digitSeen then dot can be at the last]) 3. E (it should contain only one e but not at beinning or last) 4. Sign (it should contain only one sign, but not at last, if sign is in middle after e/E then it's valid) - I check all the conditions and return the result.```

- ## Score of a String
    https://leetcode.com/problems/score-of-a-string/description/ \
    ```I loop through the string and add the absolute difference of current and next character and store it in varaible called result. And finally return the result.```