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

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

When I configured the DFS algorithm and BFS algorithm to see how many computations each algorithm ran when updating the sodoku board, I found that the DFS algorithm was more efficent, as the DFS algoirthm had less update computations compared to BFS, meaning it completed the same task but with less memory and time. In the case that the sodoku board were signifcantly easier, I think that the BFS algorithm would be more efficent as it's more perferrable for trees where the solution node is close to the origin node. 

2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

The implementation of different data structures for DFS and BFS made them more specialized for certain situations when it came to their functionallity. The stack and quene functions in DFS and BFS could possibly be intergrated into an array system.

3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

The Sodoku solver could switch between DFS or BFS depending on the percieved difficulty of the inital sodoku board in order to create a more efficent algorithm. The lessons of this assignment could be applied to situations where the next state after doing an action is not exactly known, but can at least be predicted. 