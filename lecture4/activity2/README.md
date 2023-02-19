# Activities

> The [modulo-calculator](#links) might be handy in these exercises.

## Task 1

- Refer to the following link. Discuss how open hashing works.
  https://www.cs.usfca.edu/~galles/visualization/OpenHash.html
  - Open hashing takes integer, counts selected modulo and inserts to hash value modulo calculation gives. Example in this link uses modulo 13.  (x modulo 13)
- Open Hashing Practice. Refer to the following link. Move each record on the left to the appropriate bin on the right.
  https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Hashing/OpenHashPRO.html
- Given the following input (`4322, 1334, 1471, 9679, 1989, 6171, 6173, 4199`) and the hash function `x mod 10`, which of the following statements are true?
- [x] `9679, 1989, 4199` hash to the same value
- [x] `1471, 6171` hash to the same value
- [] All elements hash to the same value
- [] Each element hashes to a different value

## Task 2

- Bucket Hashing Practice. Refer to the following [link](https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Hashing/HashBucketPRO.html).
- The keys `12, 18, 13, 2, 3, 23, 5 and 15` are inserted into an initially empty hash table of length `10` using open addressing with hash function `h(k) = k mod 10` and **linear probing**. What is the resultant hash table?
  - 12 is index 2
    18 is index 8
    13 is index 3
    2 is index 4
    3 is index 5
    23 is index 6
    5 is index 7
    15 is index 9

## Task 3:

- What is the [Birthday Paradox](http://en.wikipedia.org/wiki/Birthday_problem)?
  - States that in a random group of 23 people, there is about a 50 percent chance that two people have the same birthday.
- Why is it generally discussed with hashing?
- In a hash table of 9658 slots, what is the smallest number of records that must be inserted for the probability of a collision to be 61% or more? Use the calculator at this [link](https://opendsa-server.cs.vt.edu/ODSA/AV/Hashing/Birthday.html)
  - 136
- Discuss in groups how the following program works `./src/birthday.cpp`?

## Task 4: Individual (at home)

- Difference between `Separate Chaining` and `Open Addressing` collision handling techniques?
  - Separate chaining hash table never fills up, we can always add more elements to chain.
    Chaining is Less sensitive to the hash function or load factors.
    Chaining is Simpler to implement.
    Chaining is mostly used when it is unknown how many and how frequently keys may be inserted or deleted.
    Cache performance of chaining is not good as keys are stored using linked list.
    Wastage of Space (Some Parts of hash table in chaining are never used).
    Chaining uses extra space for links.
  - Open Addressing requires more computation.
    In open addressing, table may become full.
    Open addressing requires extra care to avoid clustering and load factor.
    Open addressing is used when the frequency and number of keys is known.
    Open addressing provides better cache performance as everything is stored in the same table.
    In Open addressing, a slot can be used even if an input doesn’t map to it.
    No links in Open addressing
    
  https://www.geeksforgeeks.org/open-addressing-collision-handling-technique-in-hashing/

  https://www.geeksforgeeks.org/separate-chaining-collision-handling-technique-in-hashing/

- (Bonus) Run the following program and comment on the code `./src/hashtable.cpp`

## Link(s)

- [modulo-calculator](https://www.calculators.org/math/modulo.php)
- [Practice Problems on Hashing](https://www.geeksforgeeks.org/practice-problems-on-hashing/)
