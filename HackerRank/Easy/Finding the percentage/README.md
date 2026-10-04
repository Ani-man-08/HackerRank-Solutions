# Finding the percentage

**Difficulty:** Easy  
**Topics:** N/A  
**HackerRank URL:** [Finding the percentage](https://www.hackerrank.com/challenges/finding-the-percentage/problem)

## Problem Description

The provided code stub will read in a dictionary containing key/value pairs of name:[marks] for a list of students.  Print the average of the marks array for the student name provided, showing 2 places after the decimal.

**Example** **

The query_name** is 'beta'.  beta's average score is .

**Input Format**

The first line contains the integer , the number of students' records. The next  lines contain the names and marks obtained by a student, each value separated by a space. The final line contains **query_name**, the name of a student to query.

**Constraints**

*

*

*

**Output Format**

Print one line: The average of the marks obtained by the particular student correct to 2 decimal places.

**Sample Input 0**

```
3
Krishna 67 68 69
Arjun 70 98 63
Malika 52 56 60
Malika

```

**Sample Output 0**

```
56.00

```

**Explanation 0**

Marks for Malika are  whose average is

**Sample Input 1**

```
2
Harsh 25 26.5 28
Anurag 26 28 30
Harsh

```

**Sample Output 1**

```
26.50

```

## Examples



## Constraints



## Solution

```pypy3
// HackerRank Problem: Finding the percentage
// Link: https://www.hackerrank.com/challenges/finding-the-percentage/problem
// Difficulty: Easy
// Language: pypy3

n = int(input())
student_marks = {}
for i in range(n):
    name, *scores = input().split()
    scores = list(map(float, scores))
    student_marks[name] = scores
query_name = input()

scores = student_marks[query_name]

total = 0
count = 0
for i in scores:
    total = total + i
    count = count + 1
result = total/count

print(f"{result:.2f}")

```

---
<div align="center">

**🔄 Synced with [CommitSync](https://www.google.com/search?q=CommitSync+extension)**

*Automatically organized and synced by CommitSync.*

</div>
