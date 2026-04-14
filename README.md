# Project-Sudoku-Puzzle-Generator-50-points-Angelina-Wang

Project Description:
In this project, the main objective is to design a Java program that generates a solved Sudoku puzzle and print it in a readable format. Sudoku puzzles must contain the numbers 1-9 only once in each row, column, and 3x3 box. The Java program must have at least one 2D array, which represents the Sudoku board, as well as at least one ArrayList, whihc must be used in a meaningful way. 

Code Overview:
In the main method, the sudoku board is first created by declaring a 2D array of the size 9x9. Then, the method fillBoard is called. The method fillBoard utilizes a nested for loop to look through each position of the sudoku board. If it finds that a certain position’s value is zero, the method creates an ArrayList named moves that uses another method, valdidMoves.
ValidMoves declares an empty ArrayList, result, and uses a for loop to look through each number 1-9. It calls on the method, check.
Check uses a for loop to check every position of the current row and column, and the 3x3 box the current position is in, to see if the current number already exists. If the number exists, the method returns the false. If the number doesn't exist, the method returns true.
ValidMoves adds the current number to the temporary ArrayList if the value of the method check is true. In order to create a unique solution, it generates a random index to insert the verified number into. 
In fillBoard, the method now iterates through the randomized ArrayList moves. It inserts a random number into the position and uses recursion to solve the rest of the board. If the board can be solved, the value returned is true. If the number choice cannot solve the solution, the method resets the position as zero, forcing the program to try a different solution. 
The main method calls on the method printBoard to neatly print out the solution. It iterates through each column and row, printing out the value at the position. If the row number is divisible by 3, the method prints a horizontal line. If the column number is divisible by 3, the method prints a vertical line. 


Running the Code:
To run the code, make a copy of the code in the file named "main". Use an online Java compiler, such as CodeHS's Java Sandbox, and paste the code into the editor.

List of Files:
1. README.md
2. main
