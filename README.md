Matrix Computer

Matrix computer simply reads a file consisting of all the matrices given by the user.
Sample file format is given below:

1,2,3
4,5,6
7,5,8

2,2
3,3

This implies that each element of matrix’s each row must be separated by “,” and each row must be written in a new line.
Moreover a blank line separates two matrices.

readFile(filename, num_matrices) 

This function reads a file and then parses it, file is read line by line, each line is trimmed which removes extra characters and empty spaces and then elements are separated on the basis of “,”. These elements are then stored on list, where single list represents a row and list of lists represent a matrix. Then another linked list is created to list all the matrices in a file. 

Filename and number of matrices to be read should be passed as function arguments.

matrixAdd(matrixA , matrixB) 

This function simply takes two matrices which are extracted from list of matrices and then checks if there order is same or not, if it is same matrices are added element by element and sum is returned as a matrix, otherwise operation is not performed.

matrixSub(matrixA , matrixB) 

This function simply takes two matrices which are extracted from list of matrices and then checks if there order is same or not, if it is same matrices are subtracted element by element and difference is returned as a matrix, otherwise operation is not performed.

matrixMultiply(matrixA , matrixB)

This function simply takes two matrices, which are extracted from list of matrices and then checks if the number of columns of matrixA is equal to the number of rows of matrixB then multiplication is performed. In multiplication each row is multiplied by each column and then added together which makes a single element. Similarly all elements are calculated like this and matrix of respected order is performed.


Moreover few more functions are also implemented for debugging purposes:
matrixPrint(matrix)
matrixPrintList(matrixList)
Unit Tests
 
All unit tests are implemented in a single “MatrixTest” class. Each test is a function, which tests a required functionality. Brief descriptions of three functions are given below.
testMatrixAdd()

This test adds three matrices and then compares the calculated result with the original result; an exception is raised if result does not match. Matrices are fetched from a file created by a user.
testMatrixMultiply()

This test simply reads a file, fetches two matrices from a file and then performs multiplication on them. Calculated result is then compared with the actual result; an exception is raised if result does not match.
testMatrixMulThenAdd()

This test reads a file and fetches three matrices. First two matrices are multiplied if their multiplication is possible and then adds a third matrix to a result if their order is same. Calculated result is then compared with the actual result; an exception is raised if result does not match.

Note
Sample matrix file, documentation, source code and unit tests are uploaded on lms as  well as github.

