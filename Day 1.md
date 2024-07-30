#CrackYourPlacement

# Learning

- ## C++ STL (Standard Template Library)

# Problem Solving

- ## Largest Element in Array
    https://bit.ly/3Pld280 \
    [Brute] \
    ```I had stored first element in a variable, then Loop through the array and compare each element with the variable. If the element is greater than the variable, then store the element in the variable. and at the end, the variable will have the largest element.``` \
    [Better] \
    ```I used two pointer approach, in which i traverse the array from the both end and find the maxNum from them.```

- ## Second Largest Element in Array
    https://bit.ly/3pFvBcN \
    [Brute] \
    ```I sort the array and then store the last element, and started the loop from the second last element and break when element is not equals to the last element. (As that element is our Second Largest element)``` \
    [Better] \
    ```I find the largest element and then start the loop (initialize second largest element = -1), if element is greater than second largest element & element is not equal to the largest element then update second largest element with current element and continue the next iteration, at end you'll find the secondLargest element.``` \
    [Optimal] \
    ```I had stored the largest element in an variable, and put the second largest -1. Then I loop through the array, if the element is greater than the largest element, then store the largest element in second largest [As Largest now become the Second Largest] and store the element in largest. There's also a condition when element is less than largest but greater than second largest so in this case we store the element in second largest. At the end, the second largest will have the second largest element.```

- ## Check if Array Is Sorted and Rotated
    https://leetcode.com/problems/check-if-array-is-sorted-and-rotated/description/ \
    ### For Sorted
    ```I had loop through the array and check if the current element is less than the next element, if it is TRUE for all case then element is sorted. if it's not then I'll return FALSE```
    ### For Rotated
    ```In Rotated Case, As mentioned in the question that if the array is sorted from a particular point then it's called sorted too, eg - 5, 1, 3, 4 is sorted if we rotate it from '1' then it becomes 1, 3, 4, 5. So to solve this problem i found out the position from where the Sorted logic return False, so my position will be current + 1, so i loop through the array from position + 1 in a circular way [using % operator] and check if the current element is less than the next element, if it is TRUE for all case then element is sorted. if it's not then I'll return FALSE, at last I'll return TRUE if all the cases of Sorted and Rotated Logic is TRUE.```

- ## Remove Duplicates from Sorted Array
    https://leetcode.com/problems/remove-duplicates-from-sorted-array/description/ \
    [Brute] \
    ```I used set to store the unique elements and then copy the set to the array from starting point``` \
    [Optimal] \
    ```I set index = 0, and loop through the array from 1 to n [where n - size of array] and check if the index element is not equals to the looped current element, if it's TRUE then i replace the index + 1 element with the looped current element and increment the index. [As in sorted array if the values are repeating then to find the next non-repeating value you have to find the element which is not equal to the current element] At last, the index will have the size of the array without duplicates & And we return 'index+1'```

- ## Sort an array of 0's 1's and 2's (Sort Colors)
    https://leetcode.com/problems/sort-colors/description/ \
    [Brute] \
    ```I used linear sort to sort the array``` \
    [Better] \
    ```I used three variables to store the count of 0's, 1's and 2's and then i again loop through those counts and store it in array in sequencial manner``` \
    [Optimal] \
    ```I applied the Dutch National Flag Algorithm, where i took 3 variables low = 0, mid = 0, high = n-1 [where n - size of array]. I loop through the array and check if the mid element is 0 then i swap the mid element with the low element and increment the low and mid by 1. If the mid element is 1 then i increment the mid by 1. If the mid element is 2 then i swap the mid element with the high element and decrement the high by 1. At last, the array will be sorted.```

