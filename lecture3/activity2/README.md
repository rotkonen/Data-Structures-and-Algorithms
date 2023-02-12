# Activities

## Task 1

- Refer to the following link. Discuss how bubble Insertion works:
  https://opendsa-server.cs.vt.edu/ODSA/AV/Sorting/insertionsortAV.html

Insertion starts sorting from left and compares to all variables that are already handled

## Task 2

- The following snippet is from `./src/insertion.cpp` lines 12-22. Discuss in groups how the code works:

```cpp
    for (int k = 1; k < 10; k++)
    {
        int temp = myarray[k];
        int j = k - 1;
        while (j >= 0 && temp <= myarray[j])
        {
            myarray[j + 1] = myarray[j];
            j = j - 1;
        }
        myarray[j + 1] = temp;
    }
```
This is example of insertion sort, it sorts from small-->large by comparing all previous cases

## Task 3

- Discuss the complexity analysis of insertion sort. Refer to the link below:
  https://www.softwaretestinghelp.com/insertion-sort/

  Insertion sort is O(n^2), but will perform better on average than bubble or selection sort.

## Links

- https://cpp.sh/
