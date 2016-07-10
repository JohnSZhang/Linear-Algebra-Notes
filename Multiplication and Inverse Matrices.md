* Multiplication
    We can think of a matrix A(m,n) multiply by another matrix B(n, p) for the result C(m, p). The most traditional way to think of the result as individual cells of the matrix C as the dot product of a row of matrix A with a Column of Matrix B.

    We can also think of the multiplication as a series of matrix A multiply by columns of column B. So C col 1 is A multiply by B column 1, each column being the linear combination of matrix A with a particular column of Matrix B.

    Likewise, we can think of individual rows of Matrix C as a linear combination of the individual rows of Matrix A with the Matrix B.

    Lastly, we can multiply a column of Matrix A by the row of a column of Matrix B to get a full matrix. And summing the resulting Matrices.

    We can in fact this this one step further by taking subsections of matrix A , multiply them with matching blocks of matrix B, and then recombining the sum of the blocks (good for parallel computing)

* Inverse Matrix
    A ^ -1 * A = I and A * A ^ -1 = I also in cases that A is a square matrix (not intuitive)

    A matrix A is singular and not invertible if there is some x for which Ax = 0 (where x is not 0). This is because we now have multiple mapping from B = 0 back to A (no single inverse can give us more than one solutions for a given input B).

* Gauss - Jordan
    A * column j of A ^ -1 = column j of I

    Looking at the multiplication A * A ^ -1 in a column based way, see each column of Ij as the product of A with A ^ -1j.

    If we combine the matrix A and A ^ -1 in a 2n by n matrix, then if we repeat the steps of elimination on the left to create the identity matrix then the right hand side will become the inverse matrix. First get upper elimination form, then remove the remaining none identity numbers.

* From Book
    Total number of multiplications needed for the multiplication of a m * n and n * p matrix is n * m * p

    When looking at a column times a row case of matrix multiplication (n x 1)(1 x n) we get a n x n matrix. This is allowed because the number of columns of the first matrix is the same as the number of rows of the 2nd. This is called the 'outer' product.

    Block matrix multiplication follows the same order as regular matrix multiplication. (we treat the blocks like numbers)

    Block elimination produces the schur complement D-CA^-1B

    A^-1A = AA^-1 = I (note order of multiplication)

    a 2 by 2 matrix is invertible if ad - bc is not zero. This ad - bc number is the determinant.

    A diagonal matrix has an inverse if no diagonal entry is zero.

    If A and B are both invertible then AB is also invertible. The inverse of AB is (AB)^-1 = B^-1 * A^-1. Likewise for products of more matrices, we always reverse the order.

    The Gauss Jordan Idea is really to multiply [AI] by A^-1 to get [IA^-1]

    An invertible matrix cannot have a zero determinant because to calculate its inverse we have to divide by its determinant
