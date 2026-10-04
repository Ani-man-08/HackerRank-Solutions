# Lists

**Difficulty:** Easy  
**Topics:** N/A  
**HackerRank URL:** [Lists](https://www.hackerrank.com/challenges/python-lists/problem)

## Problem Description

Consider a list (`list = []`). You can perform the following commands:

* `insert i e`: Insert integer  at position .

* `print`: Print the list.

* `remove e`: Delete the first occurrence of integer .

* `append e`: Insert integer  at the end of the list.

* `sort`: Sort the list.

* `pop`: Pop the last element from the list.

* `reverse`: Reverse the list.

Initialize your list and read in the value of  followed by  lines of commands where each command will be of the  types listed above. Iterate through each command in order and perform the corresponding operation on your list.

**Example** **

* : Append  to the list, .

* : Append  to the list, .

* : Insert  at index , .

* : Print the array.
 Output:

```
[1, 3, 2]

```

Input Format**

The first line contains an integer, , denoting the number of commands. **
Each line  of the  subsequent lines contains one of the commands described above.

Constraints**

* The elements added to the list must be *integers*.

**Output Format**

For each command of type `print`, print the list on a new line.

**Sample Input 0**

```
12
insert 0 5
insert 1 10
insert 0 6
print
remove 6
append 9
append 1
sort
print
pop
reverse
print

```

**Sample Output 0**

```
[6, 5, 10]
[1, 5, 9, 10]
[9, 5, 1]

```

## Examples



## Constraints



## Solution

```pypy3
// HackerRank Problem: Lists
// Link: https://www.hackerrank.com/challenges/python-lists/problem
// Difficulty: Easy
// Language: pypy3

N = int(input())
result = []
for i in range(N):
    command, *value = input().split()
    value = list(map(int,value))
    if command == 'insert':
        result.insert(value[0], value[1])
    elif command == 'print':
        print(result)   
    elif command == 'append':
        result.append(value[0])
    elif command == 'sort':
        result.sort()
    elif command == 'pop':
        result.pop()
    elif command == 'reverse':
        result.reverse()     
    elif command == 'remove':
        result.remove(value[0])      
                 
    
    

```

---
<div align="center">

**🔄 Synced with [CommitSync](https://www.google.com/search?q=CommitSync+extension)**

*Automatically organized and synced by CommitSync.*

</div>
