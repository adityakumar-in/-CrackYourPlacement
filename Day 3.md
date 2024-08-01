#CrackYourPlacement

# Problem Solving

- ## Union of Two Sorted Array
    https://www.geeksforgeeks.org/problems/union-of-two-sorted-arrays-1587115621/1 \
    [Brute] \
    ```I used set and insert both array in that set, and then appended that values in a array.```
    [Optimal] \
    ```I had used two pointer approach in this problem. I had taken two pointers i and j and initialized them to 0. Then I looped through the both array and checked if the element at i is less than the element at j then I store the element at i in a seperate array and incremented i by 1. If the element at i is greater than the element at j then I printed the element at j in a seperate array and incremented j by 1 but at same time I check if the last element stored is not as same as the current checked element, if TRUE then I insert the element only. At some point one of the array iteration will be completed and then I loop through the rest part and apply the same condition on it again.```

- ## Intersection of Two Sorted Array
    https://www.naukri.com/code360/problems/intersection-of-2-arrays_1082149 \
    [Brute] \
    ```I used loop through two arrays (using nested loop), and also maintain visited array for second array to be intersected, if the values of first and second array equals and it's not visited than we put that array in a intersected array and mark it visited and do i++ & j++. If arr[j]>arr[i] break from the inner loop (as it's not a good idea to traverse the full array then).```
    [Optimal] \
    ```I had used two pointer approach in this problem. I had taken two pointers i and j and initialized them to 0. Then I looped through the both array and checked if a[i] < b[j] if YES do i++, if a[i] > b[j] do j++ else [if equals] store it in seperate array and increment both i and j by 1 and At last you got your intersected array.```

- ## 2 Sum Problem
    https://leetcode.com/problems/two-sum/description/ \
    [Brute] \
    ```I used nested loop for traverse through the array, and find if the sum of two elements is equals to target value or not, if it's  YES then i return that position.```
    [Better] \
    ```I had used hashmap in this problem. I looped through the array and store the current element, and calculate the left value to get the target value[target - current] and check if the left value is present in the hashmap or not. If YES then return the index, If NOT then store the current element in the hashmap and continue the loop process. At last if no such pair found then return [-1, -1].```
    [Optimal] \
    ```I sort the array and then apply the two pointer approach (i - start of array, j - end of array), if i+j greater than target than do j--, if i+j less than target than do i++ else return the pair```

- ## Find All Duplicates in Array
    https://leetcode.com/problems/find-all-duplicates-in-an-array/description/ \
    ```I used two pointer logic where I set one pointer to 0 and use another to loop through the array from 1 to end, I checked if arr[i]==arr[j] if YES then I store the element in a seperate array and continue the loop till last, meanwhile I increment the value of both pointers by 1 on each iteration. At last I get the array of all duplicates.```

- ## Find the Duplicate Number
    https://leetcode.com/problems/find-the-duplicate-number/description/ \
    ```I used two pointer logic where I set one pointer to 0 and use another to loop through the array from 1 to end, I checked if arr[i]==arr[j] if YES then I return the element, If NOT then I continue the loop till last, meanwhile I increment the value of both pointers by 1 on each iteration. At last I return -1 if no such element found.```