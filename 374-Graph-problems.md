
# 1. Easy

**Required for all EASY problems:** Draw the graph described by the following vertices and edges. Your graph should have 8 vertices and 11 edges.

$V = \{a,b,c,d,e,f,g,h\}$

$E = \{(a,b),(a,c),(b,c),(b,d),(c,d),(d,e),(e,f),(e,g),(e,h),(f,g),(g,h)\}$

1.1. Demonstrate a BFS traversal of the graph, starting with vertex $a$.

1.2. Demonstrate a DFS traversal of the graph, starting with vertex $a$.

**Required for problems 1.3 and 1.4**: Modify the graph by adding the following weights to the edges.
$E_{weighted} = \{(a,b,9),(a,c,1),(b,c,7),(b,d,6),(c,d,5),(d,e,5),(e,f,4),(e,g,3),(e,h,10),(f,g,8),(g,h,1)\}$
1.3. Show the minimum spanning tree constructed using first **Prim's** algorithm (begin at vertex $d$), then **Kruskal's** algorithm. What is the weight of the MST produced by each algorithm?

1.4. (must complete 1.3 first) Are the two MSTs different? If so, describe how and why they differ. If not, reason why both algorithms produce the same result.

1.5. What is the shortest path between $a$ and $g$ using Dijkstra's algorithm? What about between $a$ and $h$?

-----
# 2. Medium

2.1. Suppose that two radio stations need to be assigned different frequencies if their broadcasting locations are within 120 miles of each other. How many different frequencies must be used for the seven stations whose distances from each other are shown in the following table?


|     | A   | B   | C   | D   | E   | F   | G   | H   |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| A   | 0   | 75  | 160 | 100 | 175 | 90  | 135 | 230 |
| B   | 75  | 0   | 100 | 50  | 130 | 110 | 120 | 200 |
| C   | 160 | 100 | 0   | 70  | 50  | 130 | 180 | 140 |
| D   | 100 | 50  | 70  | 0   | 80  | 80  | 65  | 150 |
| E   | 175 | 130 | 50  | 80  | 0   | 115 | 50  | 85  |
| F   | 90  | 110 | 130 | 80  | 115 | 0   | 60  | 135 |
| G   | 135 | 120 | 80  | 65  | 50  | 60  | 0   | 90  |
| H   | 230 | 200 | 140 | 150 | 85  | 135 | 90  | 0   |


2.2. A particular academic program has $n$ required courses, certain pairs of which have prerequisite relations so that $(x,y)$ means you must take course $x$ before $y$. How would you analyze the prerequisite pairs to make sure it is possible for people to complete the program?


2.3. Your job is to arrange $n$ ill-behaved children in a single-file line, with everyone facing front. You are given a list of statements of the form “$i$ hates $j$.” If child $i$ hates child $j$, then you do not want to put $i$ somewhere behind $j$, because then $i$ is capable of throwing something at $j$.

a. Give an algorithm that orders the line (or says that it is not possible) in $O(n+m)$ time.

b. Suppose instead you want to arrange the children in rows such that if i hates j, then i must be in a lower numbered row than j. Give an efficient algorithm to find the minimum number of rows needed, if it is possible.


2.4. A *matching* in a graph is a set of disjoint edges: that is, edges that do not have common vertices. Give a linear-time algorithm to find a maximum matching in a tree.

2.5. Describe a specific, real-world situation not yet mentioned in class or in this problem set, in which graph coloring solves a useful issue. Describe and draw a specific graph that applies to this situation. Then determine the graph's coloring, and state your conclusion to the situation.

2.6. Describe a specific, real-world situation not yet mentioned in class or in this problem set, in which the minimum spanning tree solves a useful issue. Describe and draw a specific graph that applies to this situation. Then determine the graph's MST, and state your conclusion to the situation.

2.7. Describe a specific, real-world situation not yet mentioned in class or in this problem set, in which shortest path or network flow (choose one) solves a useful issue. Describe and draw a specific graph that applies to this situation. Then determine the graph's shortest path/maximum flow, and state your conclusion to the situation.


-----

# 3. Hard

3.1. The popular Sudoku game can be represented as a graph coloring problem. The standard version of the game is a 9x9 grid, and the solver must place digits from 1 through 9 in each of the 81 squares in such a way that each row, column, and 3x3 subgrid (9 nonoverlapping squares) contains exactly each digit exactly once. Let the 81 vertices of the graph represent the squares of the 

a. Describe in words, *without drawing the graph*: What do the vertices represent? What rule is used to assign edges to the graph?

b. If we represent this game as a coloring problem, what does each color represent? How many colors should be used to color the vertices?

c. In a typical puzzle, enough of the squares are initially filled in with digits in such a way that there is a unique way to complete the puzzle. What is the analog for the graph coloring in such an instance?


3.2. You got a job at the Rheem Theater. You are reconstructing their movie schedule for this weekend, based on your regular customers' preferences. Each customer (for a total of $n$) has filled out a survey indicating the two movies they would like to see this weekend. Consider your set of movies to be $M_1, M_2, …, M_k$. You will show movies in only one time slot on Saturday evening and one time slot on Sunday evening. However, multiple movies may be screened at the same time. Assume we have $s$ possible screens (i.e. assume we have as many screens as we need).

You must decide which movies should be shown on Saturday and which on Sunday, so that every customer gets to see the two movies they desire. Is there a schedule where each movie is shown at most once? Design an efficient algorithm to find such a schedule if one exists. Argue its complexity.


3.3. You are planning the seating arrangement for a wedding, and are given a list of guests, $V$. For each guest $g$, you have a list of all other guests who are on bad terms with them.

Feelings are reciprocal: if $h$ is on bad terms with $g$, then $g$ is on bad terms with $h$.

Your goal is to arrange the seating such that no pair of guests sitting at the same table are on bad terms with each other. There will be *only two* (perhaps very large) tables at the wedding. Give an efficient algorithm to find an acceptable seating arrangement, if one exists. Provide a reasoning about its complexity.


3.4. Given pre-order and in-order traversals of a rooted binary tree, is it possible to reconstruct the tree? If so, sketch an algorithm to do it. If not, give a counterexample. Repeat the problem if, instead, you are given the pre-order and post-order traversals.

