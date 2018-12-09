A program which checks whether a certain input is a valid nxn sudoku or not.

Use input.txt for an example of sodoku

Run project with make from a terminal:

make clean  
make all  
make run  


For our purposes, an nxn sudoku is a collection of numbers organised in rows, columns and subsquares.

We consider each of the rows, columns, and subsquares to have n elements, with n being a square number greater than 1 (in other words, n can be 4, 9, 16 and so on).

So for example if n is 4, we have a 4×4 sudoku with 16 elements, if n is 9 we have a 9×9 one with 81 elements, and so on.

For instance the following is a 4×4 sudoku that we could expect in input for our program:

1 2 3 4  
4 1 2 76  
4 4 4 1  
9 4 1 -7  
The rows are:

1 2 3 4; 4 1 2 76; 4 4 4 1; 9 4 1 -7

The columns are:

1 4 4 9; 2 1 4 4; 3 2 4 1; 4 76 1 -7

The subsquares are:

1 2 4 1; 3 4 2 76; 4 4 9 4; 4 1 1 -7

We say that an nxn sudoku is valid if each of the rows, columns and subsquares contains all the numbers from 1 to n.

The sudoku above is clearly not a valid one.

The following 9×9 sudoku is a valid one:

8 4 2 5 7 1 9 3 6   
3 5 1 8 6 9 7 4 2  
7 6 9 2 4 3 1 8 5  
5 9 7 6 2 8 3 1 4  
6 2 3 1 9 4 5 7 8  
4 1 8 3 5 7 2 6 9  
9 8 6 7 3 2 4 5 1  
1 7 4 9 8 5 6 2 3  
2 3 5 4 1 6 8 9 7   
The program reads from the user the name of an input text file containing a sudoku, reads the input from the file and prints the sudoku on the screen. It determines whether the sudoku is a valid one or not and prints the outcome on the screen.


