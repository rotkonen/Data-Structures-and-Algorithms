# Activities

## Task 1

- Refer to the following link. Discuss the characteristics of Greedy approach:
  https://www.geeksforgeeks.org/greedy-approach-vs-dynamic-programming/

The Greedy approach is a technique used in algorithms to solve optimization problems. It works by making locally optimal choices at each step in the hope of finding a global optimum.

The key characteristic of the Greedy approach is that it focuses on the immediate benefit of each decision rather than considering the long-term consequences. This can lead to suboptimal solutions, as a locally optimal choice may not be globally optimal. However, the Greedy approach is often used because it is computationally efficient and can be used to solve many problems quickly.

Another characteristic of the Greedy approach is that it does not always guarantee an optimal solution. For some problems, there may not be a Greedy algorithm that always produces the best solution. In these cases, Dynamic Programming is a better approach.

Dynamic Programming is a technique that works by breaking a problem into smaller subproblems and solving each subproblem only once. It uses a memoization technique to avoid redundant calculations and can solve complex problems efficiently. The key characteristic of Dynamic Programming is that it optimizes a problem by considering all possible choices and selecting the best one.

In summary, the Greedy approach is a simple and efficient technique that can be used to solve many optimization problems. However, it is not always guaranteed to produce the best solution, and for complex problems, Dynamic Programming is often a better approach.

## Task 2

- Explain how the code in `./src/fkp.cp`p works. Refer to the following link:
  https://www.geeksforgeeks.org/fractional-knapsack-problem/

Code is Fractional Knapsack Problem, which is a classic optimization problem. The problem statement is as follows:

Given a set of items, each with a weight and a value, and a knapsack with a weight capacity, find the maximum value subset of the items that can fit into the knapsack.

The algorithm used to solve the problem in the given code is a greedy algorithm, which works by choosing the item with the maximum value-to-weight ratio at each step.

The code defines a struct Item which has two attributes, value and weight, to represent the value and weight of each item. The cmp function is a comparison function that sorts the items in decreasing order of their value-to-weight ratio, which is calculated as value/weight.

The main function, fractionalKnapsack, takes in the weight capacity of the knapsack, an array of items, and the number of items. It first sorts the items using the comparison function defined earlier. It then loops through each item and checks if it can be added completely to the knapsack. If it can, the item is added and its weight is subtracted from the remaining capacity of the knapsack. If it can't, then a fractional part of the item is added, which is calculated using the remaining capacity of the knapsack and the item's value-to-weight ratio.

Finally, the function returns the total value of the items in the knapsack.

The main function initializes the knapsack weight capacity to 50 and defines an array of items with their values and weights. It then calls the fractionalKnapsack function with these parameters and prints the result.

Overall, the code works by using a greedy algorithm to iteratively add items with the highest value-to-weight ratio to the knapsack until it is full. The algorithm provides a solution that is not guaranteed to be optimal, but is often good enough in practice.

## Task 3

- Explain how the code in `./src/asp.cpp` works. Refer to the following link:
  https://www.geeksforgeeks.org/activity-selection-problem-greedy-algo-1/

This code solves the activity selection problem, which involves selecting a maximum set of non-overlapping activities that can be done by a single person, given their start and finish times.

The function printMaxActivities takes in three parameters:

    s[]: an array containing the start times of the activities
    f[]: an array containing the finish times of the activities
    n: the total number of activities

The function first prints a message indicating that it will print the selected activities, then initializes a variable i to 0 and prints the index of the first activity (i.e., 0).

Then, the function loops through the rest of the activities starting from index 1. For each activity, it checks if its start time is greater than or equal to the finish time of the previously selected activity (which is represented by the index i). If so, it prints the index of the current activity and updates the value of i to the index of the current activity.

At the end, the function has printed the indices of the maximum set of non-overlapping activities that can be done by a single person. The driver code initializes arrays s[] and f[] with some sample start and finish times, computes the size of the arrays, and calls the printMaxActivities function with these inputs. The output shows the selected activities.

## Task 4: Individual (at home)

- Refer to te following link. Explain the differences between Greedy Algorithm and Dynamic Programming
  https://www.geeksforgeeks.org/greedy-approach-vs-dynamic-programming/

Greedy algorithms and dynamic programming are two popular techniques for solving optimization problems, but they differ in their approaches.

Greedy algorithms work by making locally optimal choices at each step to reach a globally optimal solution. In other words, the algorithm selects the best available option at each step without considering the long-term impact of that decision. Greedy algorithms are usually faster and require less memory than dynamic programming, but they do not guarantee an optimal solution in all cases.

On the other hand, dynamic programming breaks down the problem into smaller subproblems and solves each subproblem only once, storing the result in a table to avoid redundant computations. The algorithm then uses the results of the subproblems to build the solution to the original problem. Dynamic programming requires more time and memory than a greedy approach but guarantees an optimal solution in all cases.

In summary, greedy algorithms are faster but may not always give optimal solutions, while dynamic programming guarantees optimal solutions but requires more time and memory. Choosing between the two approaches depends on the specific problem and the trade-off between efficiency and optimality.

## Link(s)

- https://cpp.sh/
