#CrackYourPlacement

# Problem Solving

- ## Container with Most Water
    https://leetcode.com/problems/container-with-most-water/description/ \
    ```I had used two pointer approach in this problem. I assign two pointers at the start and end of the array and and loop it until they don't collide each other, In loop I find the minimum height from the array values pointing to that pointer [mini = min(arr[i], arr[j]) i.e., i - Initial Pointer & j - Final Pointer] and then calculate the area of the container [mini*(j-i)] then move the pointer which has less height. If arr[i] < arr[j] then move i [i++] else move j [j--] and go for the next itiration, meanwhile I only change the area value when the current calculated area is greater than the previous area. So that's how we get the max. area of the container to store water in it.```

- ## 3 Sum Problem
    https://leetcode.com/problems/3sum/description/ \
    ```I first sort the array and use two pointer array inside a loop [where i loop through the array with variable 'i'] and then I assign two pointers named j=i+1 & k=n-1 [where n is the size of the array] and then loop it until j < k. In loop I calculate the sum of the three values [arr[i] + arr[j] + arr[k]] and then check if the sum is less than 0 then move j [j++](As array is sorted so to make sum=0 we have to move j position by 1) else if sum is greater than 0 then move k [k--] (As array is sorted so to make sum=0 we have to move k position by 1) else if sum is equal to 0 then store the values in a vector and then move j and k until they are not equal to the previous values [that's how we ignore the repeating pairs] and start with the next iteration.```

- ## 4 Sum Problem
    https://leetcode.com/problems/4sum/description/ \
    ```I applied the same logic as '3 Sum Problem' but here I used one more nested loop to loop through the array.```

- ## Spiral Matrix
    https://leetcode.com/problems/spiral-matrix/description/ \
    ```I initialized four variables, top, bottom, left & right and then I looped through the matrix until top <= bottom and left <= right. In loop I first looped through the top row and then incremented top by 1, then looped through the right column and then decremented right by 1, then looped through the bottom row and then decremented bottom by 1 and then looped through the left column and then incremented left by 1 [matrix can have only one row too so for that matrix we have to put condition for bottom two loops i.e., top<=bottom & left<=right respectively], that's how i traverse through the outer part of the matrix in a spiral form so I kept on doing this until top <= bottom and left <= right.```

- ## Jump Game - I
    https://leetcode.com/problems/jump-game/description/ \
    ```I initialized a variable maxIndex=0 [To calculate the maximum index we can reach] and then loop through the array, if current index is greater than maxIndex then return false else update the maxIndex with the maximum value of maxIndex and i+arr[i] [i.e., the maximum index we can reach from the current index] and then return true if we reach the end of the array.```