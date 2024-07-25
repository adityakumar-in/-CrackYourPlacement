#CrackYourPlacement

# Problem Solving

- ## Max. Value of Equation
    https://leetcode.com/problems/max-value-of-equation/description/ \
    ```In this I have to put values(from array) in equation and return the max. value it'll generate. So equation is yi + yj + |xi - xj| where i < j & |xi-xj| <=k. So I modified the equation like this yi + yj + xj - xi -> (xj + yj) + (yi - xi). I used priority queue to store the max value of (yi - xi) [As in the end the max. value of equation depend on these values], priority queue will store values like this {{yi-xi, xi(for checking the condition <=k)}} and Firstly I initialized the priority queue and set ans = INT_MIN and loop through the array and pop the values from the priority queue if it's not empty and xj-xi>k (as we only want to put the values which obeys the condition), then i calculate the ans [max(ans, xj+yj+priority_queue.top().first)] and push the values in the priority queue. In the end return the ans.```

- ## Largest Rectangle in Histogram [Two Pointer Logic - Idle for Mid. Range Values]
    https://leetcode.com/problems/largest-rectangle-in-histogram/ \
    ```In this I have to find the largest rectangle area in histogram. So I used two pointer technique and loop through the array and find the left and right boundary of the rectangle i.e., > current height. Then calculate the area and update the max. area. [area = max(area, height[i]*(right-left-1))]. That's how i got the max area i.e., rectangle```

- ## Insert Delete GetRandom O(1)
    https://leetcode.com/problems/insert-delete-getrandom-o1/description/

- ## Game of Life
    https://leetcode.com/problems/game-of-life/description/ \
    ```In this i loop through the matrix and find all the live neighbours of each cell and update the cell according to the rules. [1 -> -1 if cell dies & 0 -> 2 if cell becomes live] and in the end update the cell values according to the rules.```

- ## Missing Number
    https://leetcode.com/problems/missing-number/description/
