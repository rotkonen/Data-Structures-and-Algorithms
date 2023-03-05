# Activities

## Task 1

- Refer to the following link. Discuss how the
  Recursive Factorial works:
  https://www.cs.usfca.edu/~galles/visualization/RecFact.html

  Recursive factorial is a function that calculates the factorial of a given number using a recursive approach. The factorial of a positive integer n is defined as the product of all positive integers up to and including n.

- Refer to the following link. Discuss how the Recursive Fibonacci works:
  https://www.cs.usfca.edu/~galles/visualization/DPFib.html
  
  Recursive Fibonacci is a function that calculates the nth Fibonacci number using a recursive approach. The Fibonacci sequence is a series of numbers in which each number is the sum of the two preceding numbers. The first two numbers in the sequence are 0 and 1.

## Task 2

There are `n` stairs, a person standing at the bottom wants to reach the top. The person can climb either 1 stair or 2 stairs at a time. There is a simple implementations in `./src/` folder. Discuss how the code works.

  Code counts the steps taken and also considers if 1 or 2 steps taken at a time.

## Task 3

- There are `n` stairs, a person standing at the bottom wants to reach the top. The person can climb either 1 stair or 2 stairs or **3 stairs** at a time. Write a program that counts the number of ways, the person can reach the top. You can use the following program as a starter `./src/staircase1.cpp`. Also the link below might useful:
  https://www.includehelp.com/cpp-programs/stair-case-program-to-solve-the-staircase-problem.aspx

```cpp
#include <iostream>
        using namespace std;

        int number_of_paths(int n)
        {
            if (n <= 0)
                return 0;
            if (n == 1)
                return 1;
            if (n == 2)
                return 2;
            if (n == 3)
                return 4;

            return number_of_paths(n - 1) + number_of_paths(n - 2) + number_of_paths(n - 3);
        }

        int main()
        {

            cout << "number of paths =  " << number_of_paths(4);
            return 0;
        }
```

## Task 4: Individual (at home)

- What are the pros/cons of recursive over iterative Programming?
Pros
 - Cleaner code
 - It's more intuitive
Cons
 - Takes up a lot more stack space
 - Slows down processing time
 - Can lead to potential stack overflow
 - Often harder to debug

- Difference between recursion and induction.
  Recursion is a process in which a function gets repeated again and again until some base function is satisfied.
  Induction is the branch of mathematics that is used to prove a result, or a formula, or a statement, or a theorem.
> Refer to the [links](#links) section below.

## Links

- https://cpp.sh/
- [Difference Between Recursion and Induction](https://www.geeksforgeeks.org/difference-between-recursion-and-induction/)
- [Recursion vs Iterative Programming](https://www.softwaretestinghelp.com/recursion-in-cpp/)
