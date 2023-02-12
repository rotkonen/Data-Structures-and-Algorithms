# Activities

## Task 1:

- Refer to the following link. Discuss how Queues based on linked lists works:
  https://www.cs.usfca.edu/~galles/visualization/QueueLL.html

  It's just basic queue, like waiting in shopping line. Everytime element is added, new node is created and when takin out from queue it takes the last added one out (FIFO)

## Task 2:

- The following snippet is from `./src/queue.cpp` lines 8-10. What happens if `front`, `rear` and `temp` were not global variables?

```cpp
struct node *front = NULL;
struct node *rear = NULL;
struct node *temp;
```
If they are not global variables, we could't modify them. There would have to a be pointer or some other system implemented.

## Task 3:

- The following snippet is from `./src/queue.cpp` lines 11-28. Discuss in groups how the code works:

```cpp
void Insert(int val)
{
    if (rear == NULL)
    {
        rear = new node;
        rear->next = NULL;
        rear->data = val;
        front = rear;
    }
    else
    {
        temp = new node;
        rear->next = temp;
        temp->data = val;
        temp->next = NULL;
        rear = temp;
    }
}
```

## Task 4: Individual, at home

- Discuss the various operations that can be performed on a linked list. Refer to the following link:
  https://www.softwaretestinghelp.com/linked-list/

  Insertion - add new elements to the list at the beginning, end, or specific position.

    Deletion - remove elements from the list based on certain conditions.

    Traversal - visiting and processing each node in the list.

    Search - find the location of a specific element in the list.

    Reversal - reverse the order of the elements in the list.

    Sorting - arrange the elements in the list in a particular order.

    Merge - combine two or more linked lists into one.

    Split - divide a linked list into two or more smaller lists.

These are some of the basic operations that can be performed on a linked list, but the exact set of operations that can be performed may vary depending on the specific use case.

## Links

- https://cpp.sh/
