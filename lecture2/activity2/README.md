# Activities

## Task 1

Refer to the first [link](#links).

- Why is Algorithm Analysis Important?
    The accidental or unintentional use of an inefficient algorithm can significantly impact system performance
- Explain the Big $O$ notation
    Big O Notation is a tool used to describe the time complexity of algorithms.
- Compare `Linear`, `Logarithmic`, `Quadratic` and `Constant` complexities.
    	O(n), O(log(n)), O(n²), O(c)

## Task2

Refer to the first [link](#links).

- Write a simple algorithm in C++ that finds the square of the first item in a list and then prints it on the screen.
    #include <iostream>
    #include <vector>

    int main() {
    std::vector<int> list = {10, 2, 3, 4, 5, 6, 7, 8, 9, 10};
    int result = list[0] * list[0];
    std::cout << result << std::endl;
    return 0;
    }
- What is the complexity of the algorithm?
    The complexity of the previous algorithm is O(1).

## Task 3

Refer to the first [link](#links).

- Write a simple program that displays all items in a list to the console.
    #include <iostream>
    #include <vector>

    int main() {
    std::vector<int> numbers = {1, 2, 3, 4, 5};
    for (int number : numbers) {
        std::cout << number << std::endl;
    }
    return 0;
    }


- What is the complexity of the algorithm?

## Task 4: : Individual, at home

Refer to this [pdf](./big_o.pdf):

- What is the difference between complexity and performance:
    Performance how much time/memory/disk/... is actually used when a program is run. This depends on the machine, compiler, etc. as well as the code.
    Complexity how do the resource requirements of a program or algorithm scale, i.e., what happens as the size of the problem being solved gets larger?
- Does complexity affects performance or is it the other way around?
    It affects the performance
- Restate the formal definition of big $O$ in plain English
    Big O notation is a mathematical notation that describes the limiting behavior of a function when the argument tends towards a particular value or infinity, and is usually written as 'O'. It is an Asymptotic Notation for the worst case, which is also the ceiling of growth for a given function.
## Links

- [Big O Notation and Algorithm Analysis ](https://stackabuse.com/big-o-notation-and-algorithm-analysis-with-python-examples/)
- [Visualization](https://www.cs.usfca.edu/~galles/visualization/Search.html)
- [Big-O notation explained by a self-taught programmer](https://justin.abrah.ms/computer-science/big-o-notation-explained.html)
- [Big-O is easy to calculate, if you know how](https://justin.abrah.ms/computer-science/how-to-calculate-big-o.html)
- https://cpp.sh/
