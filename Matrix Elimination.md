* Elimination Example
    1 2 1
    3 8 1
    0 4 1

    With a given set of equations, we would like to eliminate a particular variable by using pivots (they cannot be 0).

    A(1, 1) is our first pivot that we will use to try and eliminate the variable.

    We multiply row one by 3 to get
    3, 6, 3 and subtracts it from row 2 to get ride of A(2, 1) and get:

    1 2  1
    0 2 -2
    0 4  1

    Now we have the 2nd pivot at A(2, 2) and use it to eliminate A(3, 2) by multiply it by 2 and subtract from row 3 to get:

    1 2  1
    0 2 -2
    0 0  5

    This transforms our A matrix to the U (stands for upper triangular form) matrix with pivots at 1, 2, and 5

    When there are temporary zeros in the pivot position, we do row exchange. When the pivot position zero is not exchangeable, then the matrix is not invertible.

    the right hand side (b) will receive the same kind of elimination sets (multiplication and subtraction) to preserve the equation on both sides. Once the elimination is complete, b becomes the vector c

* Backwards Substitution
    we take our U and C, and go backwards from the last row up to the first row. Since the last row has only zeros except for the last pivot, we can easily work out way up from row M to row 0.

* Matrix Elimination Steps
    As our examples above, we can use a matrix to create the same steps of (multiply row n by a number, then subtract it from another using a negative number).

    Since the identity matrix preserve the original matrix, we can simply change the 0 of one of the identify rows with the change we wish to make for that row. This way we can see the elimination process as a series of multiplication on the original matrix A. ie. E32(E21 * A) = U, if E stands for the elementary single step matrix for each row elimination.

    We can also use a permutation matrix to switch rows of a matrix, which is simply an identity matrix with it's rows swapped. To do a column operation, multiple the same modified identity matrix to the right of the matrix whose columns you want to swap.

    We can in in fact combine these single elimination steps around A but switching the () and create a single matrix to transform A to U according to the associative law of matrices. ie, E32(E21 * A) = (E32 * E21) * A. However, we would first like to get the E^-1 inverse matrices for these elementary matrices.

* From Book
    The key thing about a single elimination matrix is to take the row you want to subtract from (a) and the row to subtract is from (b), multiply by negative l (their ratio) and put that in the ab position of the identity matrix.

    Likewise we multiply the result B with the same elimination matrix to preserve the equality. And remember, associative law holds for matrix multiplication while commutative law does not. 

    The matrix for row exchange exchanges that changes the location of 1s in the identity matrix is called the permutation matrix.

    The idea of combining A with the result B to do elimination has a whole is called using an augmented matrix.
