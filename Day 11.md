#CrackYourPlacement

# Problem Solving

- ## Perfect Sum Problem
    https://www.naukri.com/code360/problems/subset-sum_630213 \
    ```In this you have to count all the subsequences whose sum is equal to the given sum. So I used recursion, in which i used take & don't take technique, I used recursive call to find the sum of all the subsequences and then checked if the sum is equal to the given sum or not, if yes return true else false, also while doing recursive call, i used to check if call is equal to true or not, if yes then return true, if both the call is not equal to true then i simply return false & i also handled the situation where sum>target, in that case i return false.```

- ## Merge Sort
    https://www.geeksforgeeks.org/problems/merge-sort/1 \
    ```I used recursion to divide the array into two parts and then merge the two parts, i used two recursive call i.e., from low to mid & mid+1 to high to divide the array into smaller smaller part, and write the base case as if low==high (At that time it'll backtrack and start merging and sorting the array).```

- ## Quick Sort
    https://www.geeksforgeeks.org/problems/quick-sort/1 \
    [Quick Sort Logic] \
    ```I used recursion to divide an array from pivot into two parts and call it recusively when low<high, but before calling i have to find the pivot value too, so for that i used an external function called 'partition' for doing pivot``` \
    [Partition Logic] \
    ```I used partition function to find the pivot value and then used that pivot value to divide the array into two parts and then call the quicksort function recursively, The logic in partion function is that place the values less than pivot to left and greater than pivot to right & then return the current pivot value.```

- ## Combination Sum 
    https://leetcode.com/problems/combination-sum/description/ \
    ```I used recursion to find the combination sum, in which i used take (but in take i don't increase the index by 1 as i have to recheck for the sum) & don't take (i used index+1 as if sum!=target then i should start the next recursion process) technique, so in take i used to call the function recursively with target-arr[i] and i used to add to the list if target==0 and then backtrack for the other possible combination.```

