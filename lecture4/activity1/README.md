# Activities

## Task 1

- Refer to the following link. Discuss how Merge-sort works:
  https://opendsa-server.cs.vt.edu/OpenDSA/AV/Sorting/mergesortAV.html
  It works by recursively breaking down a problem into two or more sub-problems of the same or related type, until these become simple enough to be solved directly.

- Merge-sort Practice. Refer to the following link. Merge the two sub-arrays into the larger array.
  https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Sorting/MergesortMergePRO.html

## Task 2

- Refer to the following link. Discuss how Quick-sort works:  
  https://opendsa-server.cs.vt.edu/OpenDSA/AV/Sorting/quicksortAV.html
- Quick-sort Practice. Refer to the following link. Partition the array using quicksort.
  https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Sorting/QuicksortPartitPRO.html
  It works by splitting a large array of data into smaller sub-arrays. 

## Task 3

- The following snippet is from `./src/quicksort.cpp` lines 32-43. Discuss in groups how the code works:

```cpp
void quickSort(int arr[], int low, int high)
{
    if (low < high)
    {
        //partition the array
        int pivot = partition(arr, low, high);

        //sort the sub arrays independently
        quickSort(arr, low, pivot - 1);
        quickSort(arr, pivot + 1, high);
    }
}
```
Recursively sorting the two partitioned arrays around the pivot element

- The following snippet is from `./src/quicksort.cpp` line 27. Discuss in groups how ìt works:

```cpp
swap(&arr[i + 1], &arr[high]);
```
Pivot element change

## Task 4: Individual (at home)

1. Merge-sort has better worst case performance than quicksort. So why Quick-sort is considered better than Merge-sort? Refer to the following article
   https://www.geeksforgeeks.org/quicksort-better-mergesort/
2. Refer to the following article. Analyze the complexity of the Merge-sort algorithm.
   https://www.softwaretestinghelp.com/merge-sort/
3. Refer to the following article. Analyze the complexity of the Quick-sort algorithm.
   https://www.softwaretestinghelp.com/quick-sort/
