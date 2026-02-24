# Data Structure Problems

## Hashing

1. Given a hash function of $f(x)=x+31$ mod 11, determine *if* there is a collision for items inserted with the keys 60, 9, 45, 3, 70, 5, 90, 93, 39, 77, 70  in that order. At which item does the first collision occur?
	1. Draw the resultant array if we inserted using the **linear/sequential probing** method of collision resolution. Use arrows/different colors to demonstrate when probing occurs.
	2. What is the result of the array when resolving collisions using **chaining**? Draw a picture.
2. Given a hash function of $f(x) = x^6 - 23x^5 + 6x^3 + 3 \text{ mod } 22$, determine if there is a collision for items inserted with the keys in the following order. At which item does the first collision occur? (*scroll down for more problems*)
	- 68
	- 57
	- 22
	- 37
	- 30
	- 18
	- 2
	- 99
	- 10
	- 6
	- 40
	- 69
	- 65
	- 72
	 - 41
	 - 48
	 - 13
	 - 95
	 - 75
	 - 59
	 - 28
	- 100
	1. Draw the resultant array if we inserted using the **linear/sequential probing** method of collision resolution. Use arrows/different colors to demonstrate when probing occurs.
	2. What is the result of the array when resolving collisions using **chaining**? Draw a picture.

------

## Binary Search Trees


1. Draw the binary search tree according to the numbers inserted in the following order:
	- 43
	- 27
	- 54
	- 46
	- 35
	- 24
	- 82
	- 76
	- 97
	- 91
	- 73
	- 11
	- 60
	- 74
2. Using that BST, list its traversals:
	1. Pre-order
	2. In-order 
	3. Post-order
3. Draw the binary search tree according to the numbers inserted in the following order:
	- 58
	- 47
	- 84
	- 39
	- 55
	- 14
	- 98
	- 53
	- 79
	- 42
	- 87
	 - 3
	- 90
	 - 1
	- 51
	- 44
	- 83
	- 62
4. Using that BST, list its traversals:
	1. Pre-order
	2. In-order 
	3. Post-order
-----
## Easy

1. Suppose you seek to maintain the contents of a refrigerator so as to minimize food spoilage. What data structure should you use, and how should you use it?
2. Imagine you have a closet full of shirts. What can you do to organize your shirts for easy retrieval?

---

## Medium

1. Design a stack $S$ that supports `S.push(x)`, `S.pop()`, `S.findmin()`, which returns the minimum element of $S$. All operations should run **in constant time**.
2. Design a data structure to support the following operations:
	1. `Insert(x,T)` – insert the item `x` into the set `T`.
	2. `Delete(k,T)` – delete the `k`th smallest element from `T`.
	3. `Member(x,T)` – return true iff `x` is in `T`.  
   All operations must take $O(log n)$ time on an n-element set. Prove or reason that it does so.

-----
## Hard
3. What is the best data structure for maintaining URLs that have been visited by a web crawler? Describe an algorithm to test whether a given URL has already been visited, optimizing both space and time.
4. Tic-tac-toe is a game played on an n x n board (typically n=3) where two players take consecutive turns placing “O” and “X” marks onto the board cells. The game is won if n consecutive “O” or “X” marks are placed in a row, column, or diagonal. Create a data structure with O(n) space that accepts a sequence of moves, and reports in constant time whether the last move won the game.
5. Your friends in the SMC nursing program need to keep track of their clinical hours. Your friends in the SMC education program need to keep track of their teaching hours, as well. When you talk to the faculty, you realize that the students submit their hours to a central spreadsheet. They get flagged if they have not yet completed enough hours compared to their peers (there is a sample, "standard" peer, who has the exemplary number of hours so that the faculty have a benchmark). 
   Describe a data structure that, given a new student's submission, adequately computes the amount of time. You should generally describe the following operations: Insert (student adds the course), Search, Delete (student drops clinical course). Provide worst-case complexity of each operation.
   Your answer should involve no actual code, only a high-level description of the algorithm(s).
6. The library, in its course of moving to the Power Plant, has stored 1 million video games in a room in Ageno East. Develop a short proposal that addresses the following questions: On what metrics should the items be accessed? If we design a data structure to help the library search function report the current catalog, what is best way to store the items in the computer? How should they be accessed, what does insertion or retrieval of a video game look like in code? Use technical terms you have learned wherever possible.