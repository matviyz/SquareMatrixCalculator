# SquareMatrixCalculator
Includes various calculator functions for Square Matrices. Built on Google Colab with a python notebook for CS102.

## How it works
### Inputiting the Matrix
The user first inputs how many rows/columns they want for their matrix.
Then the user inputs their entries.
The function `omat(n)` appends a list of n size with n lists inside into `omatrix`, then uses a numpy function to print out the results in text, and a matplotlib function to show the matrix graphically.
### Usecases
Then the user is asked what they would like to do with their matrix.
There is an option to show the tranpose, find the determinant, show the inverse, or show the eigenvalues.
The user makes a selection by using the `input()` function followed by a series of corresponding `elif` statements.
### Transpose
If the user selects the transpose, it is given using the numpy function, and then printed the same way the inputed matrix was.
### Determinant
The determinant is calculated using another numpy function and then rounded to an accuracy of 4 digits.
The value is then printed.
### Inverse
The inverse of a matrix can only exist if the determinant is not 0, so in order to calculate the inverse, the `detm()` function is ran and checked if it's not equal to 0.
If it returns true, a numpy function is used to find the inverse and then displayed the same way the original matrix was. 
If it returns false, A message is printed saying that the matrix is uninvertible.
### Eigenvalues
Yet another numpy function is used to find the eigenvalues and eigenvectors of the matrix, the same way the original matrix was.
