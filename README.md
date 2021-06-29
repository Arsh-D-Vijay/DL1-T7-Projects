# Sudoku Solver
Project Description:

This project aim is to solve sudoku puzzles, taken from an image. 

Approach:

- Find Sudoku Puzzle Contours inside the image.
- Warp out the Sudoku Puzzle.
- Divide Whole Puzzle into seprate boxes.
- Run my model on each box and generate a Grid (array) recognisible to Solver File.
- Run Solver Function.
- Output the Solved Sudoku.

This Project uses OpenCV library for Image Processing.
For the ML model, I have chosen the simillar architecture as of LeNet (developed by Yann Lecunn).
The Solver function works on simple backtracking and recursion approach to solve a given (9,9) grid.

Files:

- Sudoku_Solver : This file contains functions to solve a sudoku puzzle

- Sudoku_Solver_Main_v2 : This is the main file where I have done Image processing to process the Sudoku Image which then is 
		              feeded to my ML model for genration of grid recognisable by my Sudoku_Solver File.

- Utility_Functions : This contain all the utility functions used in my Sudoku_Solver_Main_v2 file.

- digit_recog_main.h5 : ML model


Libraries Used:

TensorFlow version -- 2.5
OpenCV version -- 4.5.2
Numpy verison -- 1.19.5
Matplotlib verison -- 3.4.2
