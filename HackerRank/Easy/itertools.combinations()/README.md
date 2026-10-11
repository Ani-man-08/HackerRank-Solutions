# itertools.combinations()

**Difficulty:** Easy  
**Topics:** N/A  
**HackerRank URL:** [itertools.combinations()](https://www.hackerrank.com/challenges/itertools-combinations/problem)

## Problem Description

**[itertools.combinations(iterable, r)](https://docs.python.org/2/library/itertools.html#itertools.combinations)** **
This tool returns the  length subsequences of elements from the input iterable.

Combinations are emitted in lexicographic sorted order. So, if the input iterable is sorted, the combination tuples will be produced in sorted order.

 Sample Code**

```
>>> from itertools import combinations
>>>
>>> print list(combinations('12345',2))
[('1', '2'), ('1', '3'), ('1', '4'), ('1', '5'), ('2', '3'), ('2', '4'), ('2', '5'), ('3', '4'), ('3', '5'), ('4', '5')]
>>>
>>> A = [1,1,3,3,3]
>>> print list(combinations(A,4))
[(1, 1, 3, 3), (1, 1, 3, 3), (1, 1, 3, 3), (1, 3, 3, 3), (1, 3, 3, 3)]

```

**Task**

You are given a string . **
Your task is to print all possible combinations, up to size , of the string in lexicographic sorted order.

Input Format**

A single line containing the string  and integer value  separated by a space.

**Constraints**

 **
The string contains only *UPPERCASE* characters.

Output Format**

Print the different combinations of string  on separate lines.

**Sample Input**

```
HACK 2

```

**Sample Output**

```
A
C
H
K
AC
AH
AK
CH
CK
HK

```

## Examples



## Constraints



## Solution

```pypy3
// HackerRank Problem: itertools.combinations()
// Link: https://www.hackerrank.com/challenges/itertools-combinations/problem
// Difficulty: Easy
// Language: pypy3

# Enter your code here. Read input from STDIN. Print output to STDOUT
from itertools import combinations

s, k = input().split()
s = sorted(s)
k = int(k)

for i in range(1, k + 1):
    for j in combinations(s, i):
        print(''.join(j))

```

---
<div align="center">

**🔄 Synced with [CommitSync](https://www.google.com/search?q=CommitSync+extension)**

*Automatically organized and synced by CommitSync.*

</div>
