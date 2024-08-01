#CrackYourPlacement

# Problem Solving

- ## Set Matrix Zeroes
    https://leetcode.com/problems/set-matrix-zeroes/description/ \
    [Brute] \
    ```In this i loop through the matrix and find zeros, if zero found then i mark it's row & column values as -1 (where value!=0) and at last i convert all -1 as 0```
    [Better] \
    ```I used external array of row & column to mark which row & column at last i have to make zero, and at last i convert all the marked element to zero```
    [Optimal] \
    ```In Set Matrix Zeroes problem, we have to set the entire row and column to 0 if we encounter 0 at any cell in the matrix. So my approach is, I'll choose the first row and first column as a flag to store the information about the row and column that needs to be set to 0, but there might be a conflict between the arr[0][0] as it'll store flag of row or column, so I'll use a separate flag for the row called [col0=1] and put column in arr[0][0].```
    
    ```I'll loop through the matrix and find the cell with 0 and set it's row & column flag to 0, if it's first row then I'll set col0=0. That's how we mark the matrix. Now we loop through the non-flagged part of matrix and check if and cell is non-zeros or not, if it is then we check whether it's row or column is flagged to 0 or not, if it is then we set the cell to 0. Now we check the flag column first with arr[0][0]=0 and if it is then we set the entire column to 0. Then we check the flag row with col0=0 and if it is then we set the entire row to 0. That's how our Set Matrix Zeroes problem is solved.```
    ```
- ## Best Time to Buy and Sell Stock
    https://leetcode.com/problems/best-time-to-buy-and-sell-stock/description/ \
    ```I assume the first element as the minimum price and set the maxProfit to 0. Then I loop through the rest of the array and find the cost of stock [selling - buying] i.e., prices[i] - minimum price. If the cost is greater than maxProfit then I update the maxProfit. If the prices[i] is less than minimum price then I update the minimum price. That's how we solve the Best Time to Buy and Sell Stock problem.```
    ```
- ## Move Zeros to End of Array
    https://leetcode.com/problems/move-zeroes/description/ \
    [Brute] \
    ```I used temp array to store all non-zeros elements and then store it in the real array, at last i set rest of the values to zero.```
    [Optimal] \
    ```I first assign the index to -1 and find the first zero in the array while looping through it and break when i finds the first zero. Then I loop through the rest of the array and use 'i' as a pointer i = index+1, if arr[i] is non-zero then I swap arr[i] with arr[index] and increment the i & index by 1 if not we increase only i index by 1. That's how we solve the Move Zeros to End of Array problem.```
    ```
- ## Chocolate Distribution Problem
    https://www.geeksforgeeks.org/problems/chocolate-distribution-problem3825/1 \
    ```I sort the Array and then adjust the window according to the number of student, and find the minimum diffenrence between the maximum and minimum element of the window[difference first and last element of the window] by looping through the array. That's how we solve the Chocolate Distribution Problem.```
    ```
- ## Rotate Array to Right by K Steps
    https://leetcode.com/problems/rotate-array/description/ \
    [Brute] \
    ```I store from 0th to Kth element in an temp array and then re-build the array, where i put the k+1th element at 0th position and so on, and fill the rest of the position with temp array values.```
    [Optimal] \
    ```I divide the array into two parts, first part is from 0 to n-k-1 and second part is from n-k to n-1. Then I reverse the first part and reverse the second part and then reverse the entire array. That's how we solve the Rotate Array to Right by K Steps problem.```