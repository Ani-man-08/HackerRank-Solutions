# The Minion Game

**Difficulty:** Medium  
**Topics:** N/A  
**HackerRank URL:** [The Minion Game](https://www.hackerrank.com/challenges/the-minion-game/problem)

## Problem Description

Kevin and Stuart want to play the '**The Minion Game**'.**

Game Rules****

Both players are given the same string, .

Both players have to make substrings using the letters of the string .

Stuart has to make words starting with *consonants*.

Kevin has to make words starting with *vowels*.

The game ends when both players have made all possible substrings.

Scoring****
A player gets `+1` point for each occurrence of the substring in the string .

For Example**:**
String  = *BANANA*

Kevin's vowel beginning word = *ANA*

Here, *ANA* occurs twice in *BANANA*. Hence, Kevin will get `2` Points.

For better understanding, see the image below:

*

Your task is to determine the winner of the game and their score.

Function Description**

Complete the minion_game* in the editor below.

*minion_game* has the following parameters:

* *string string:* the string to analyze

**Prints**

* *string:* the winner's name and score, separated by a space on one line, or `Draw` if there is no winner

**Input Format**

A single line of input containing the string . **
Note**: The string  will contain only uppercase letters: .

**Constraints**

**

Sample Input**

```
BANANA

```

**Sample Output**

```
Stuart 12

```

**Note :

Vowels are only defined as . In this problem,  is not considered a vowel.**

## Examples



## Constraints



## Solution

```pypy3
// HackerRank Problem: The Minion Game
// Link: https://www.hackerrank.com/challenges/the-minion-game/problem
// Difficulty: Medium
// Language: pypy3

def minion_game(string):
  vowels = "AEIOU"
  kevin = 0
  stuart = 0
  for i in range(len(string)):
    points = len(string) - i
    if string[i] in vowels:
        kevin += points
    else:
        stuart += points

  if stuart > kevin:
    print("Stuart", stuart)
  elif kevin > stuart:
    print("Kevin", kevin)
  else:
    print("Draw")
            


```

---
<div align="center">

**🔄 Synced with [CommitSync](https://www.google.com/search?q=CommitSync+extension)**

*Automatically organized and synced by CommitSync.*

</div>
