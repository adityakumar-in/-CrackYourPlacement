#DsaPractice

# Learning
- ## Euclidean Algorithm
- ## Singly Linked List
    - ### Insertion
    - ### Deletion
- ## Doubly Linked List Introduction

# Problem Solving

- ## Check for Perfect Number
    https://takeuforward.org/plus/data-structures-and-algorithm/beginner-problems/basic-maths/check-for-perfect-number/ \
    [Optimal] \
    ```I loop through the half of the number (because other half was just (n/i) where i is the looping var. of the first half) and then check if the number is divisible by i then add i to the sum and aslo check if (n/i)!=i && (n/i)!=n then also add (n/i) added to sum (As we have to sum up other half too) then check if the sum is equal to the number then return true else return false.```

- ## GCD of Two Numbers
    https://takeuforward.org/plus/data-structures-and-algorithm/beginner-problems/basic-maths/gcd-of-two-numbers/ \
    [Optimal] - Euclidean Algorithm \
    ```I keep on subtracting the smaller number from the larger number until one becomes zero and returned the other one.```

- ## LCM of Two Numbers
    https://takeuforward.org/plus/data-structures-and-algorithm/beginner-problems/basic-maths/lcm-of-two-numbers/ \
    [Optimal] \
    ```I calculated the GCD and then divided the product of the two numbers by the GCD to get the LCM.```

- ## Divisors of a Number
    https://takeuforward.org/plus/data-structures-and-algorithm/beginner-problems/basic-maths/divisors-of-a-number/ \
    [Optimal] \
    ```I used the same approach as the PERFECT NUMBER problem but instead of checking if [(n/i)!=i && (n/i)!=n], i check only [(n/i)!=i] just stored the divisors in an array and later returned it in sorted order.```

