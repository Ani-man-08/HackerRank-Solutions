# Set .add() 

**Difficulty:** Easy  
**Topics:** N/A  
**HackerRank URL:** [Set .add() ](https://www.hackerrank.com/challenges/py-set-add/problem)

## Problem Description

If we want to add a single element to an existing set, we can use the *.add()* operation. **
It adds the element to the set and returns '`None`**'.

**Example**

```
>>> s = set('HackerRank')
>>> s.add('H')
>>> print s
set(['a', 'c', 'e', 'H', 'k', 'n', 'r', 'R'])
>>> print s.add('HackerRank')
None
>>> print s
set(['a', 'c', 'e', 'HackerRank', 'H', 'k', 'n', 'r', 'R'])

```

**
Task**

Apply your knowledge of the *.add()* operation to help your friend Rupal.**

Rupal has a huge collection of country stamps. She decided to count the total number of distinct country stamps in her collection. She asked for your help. You pick the stamps one by one from a stack of  country stamps.

Find the total number of distinct country stamps.

Input Format**

The first line contains an integer , the total number of country stamps.**
The next  lines contains the name of the country where the stamp is from.

Constraints**

**Output Format**

Output the total number of distinct country stamps on a single line.

**Sample Input**

```
7
UK
China
USA
France
New Zealand
UK
France

```

**Sample Output**

```
5

```

**Explanation**

UK and France repeat twice. Hence, the total number of distinct country stamps is  (five).

## Examples



## Constraints



## Solution

```pypy3
// HackerRank Problem: Set .add() 
// Link: https://www.hackerrank.com/challenges/py-set-add/problem
// Difficulty: Easy
// Language: pypy3

N = int(input())
country_list = set()
for i in range(N):
    country = input()
    country_list.add(country)
print(len(country_list))    
    
    

```

---
<div align="center">

**🔄 Synced with [CommitSync](https://www.google.com/search?q=CommitSync+extension)**

*Automatically organized and synced by CommitSync.*

</div>
