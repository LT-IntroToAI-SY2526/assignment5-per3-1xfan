# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. What are some things that you learned through this assignment? Think about the concepts of backtracking, constraint satisfaction, and search algorithms. Were there any particular challenges you faced while implementing the Board class methods or the DFS/BFS functions? How did you overcome them?

I learned about stacking and how to implement it in the code. I also learned about different search methods such as breadth-first and depth-first, and how to apply them. I faced some challenges when implementing the board class methods, as I was a little confused by concepts such as the least constraining cells. The more we went over it as a class, the more I was able to grasp this concept and overcome this challenge.


2. How can you apply what you learned in this assignment to future programs or projects? Consider other types of problems that involve searching through possibilities, making decisions, and backtracking when those decisions don't work out. Can you think of real-world scenarios where DFS or BFS might be useful? What about other constraint satisfaction problems?

I can apply what I learned in this assignment to future programs or projects by utilizing the same/similar search algorithms or similar ones for other projects, possibly even for solving other games. Some types of problems that involve searching through possibilities and making decisions are games that contain certain restrictions that require rigorous checking to see if an action is allowed, and if not all of the requirement are met, the program will not work. This is somewhat similar to the questions that you (Mr. Berg) gave us before this project in the word puzzle questions where we had to figure out what floor a certain person lived on, given certain information.

3. Explain how the Stack and Queue classes work and why they are important for DFS and BFS algorithms. Describe the difference between LIFO (Last In First Out) and FIFO (First In First Out) data structures. How does using a Stack versus a Queue change the way the search algorithm explores possible solutions? Why is one data structure better suited for depth-first search and the other for breadth-first search?

Stack uses LIFO which means the last item added is the first taken out. That item is then used in DFS to explore one path thoroughly before backtracking. Queue uses FIFO where the first item added is the first taken out. That item is then used to explore all neighbors before moving lower. Using Stack makes the search go as deep as possible first, while Queue makes it move level by level. One data structure is better suited for one type of search over the other because one takes time in order to find the exact solution of a cell while the other goes through every cell and simply narrows down what the solution could be.
