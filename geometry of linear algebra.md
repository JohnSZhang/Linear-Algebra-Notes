* Example
    2x + y = 3 => y = 3 - 2x => y + 2 = 3 => y = 1
    x - 2y = -1 => x - 6 + 4x = -1 => 5x = 5 => x = 1

* Row Picture:
    Looking at the rows as series of linear equations and solve by drawing out the lines as represented by the row variables.
        In this cases they are the lines 2x + y = 3 and x -2y = -1

* Column Picture:
    Look at the columns of the equations as vectors and take the linear combination of the two vectors. (ie v1 * X + v2 * y)
        In this case we have the vectors [2, 1] for x and [1, -2] for y and they sum to be [3, -1]. We want a certain multiplier of x and y so that the vectors multiplied will result in the sum vector.

    Each linear system can be seen both row and column wise.

    Matrix Form:
    Matrix A (coefficient matrix) has the form of [V1, V2] = [2,  1]
                                        [1, -2]
    [2,  1][x] = [ 3]
    [1, -2][y]   [-1]

    In the form AX = B, X = B/A => A^-1B

    We are really looking for the A Inverse Matrix (A^-1), such that A*A^-1 = the identity matrix of [1 0]
       [0 1]
    In our case, [X] = A^-1[ 3]
                 [Y]       [-1]

    We can think of Ax as a combination of the columns of the matrix A (ie A(c1)x + A(c2)y + A(c3)z +...) This combination of columns instead of dot product of rows and the Xs can sometimes be more efficient.

* Linear Independence:
    Question: For a given A, can I solve Ax = b for all values of b? Do the linear combinations of the columns fill the entire plane / space?

    A matrix is said to be singular if its linear combinations cannot fit the entire plane that it is in. A invertible matrix is one which can fill the entire solution space. This is because the individual column vectors are linearly dependent (they are all on the same line/plane, etc).

    A matrix's vectors are also dependent if there is a combination of the vectors which gives the zero vector. (think about two vectors in 2D plane, only way they can be combined to reach 0 is if they are on the same line)

* Additional Notes From Book:
    It is important to think about the 'space' of all combination of vectors of a particular size (this always include the 0 vector, and is a plane in 2d, a space in 3d, etc etc)

    A column vector of [1, 2] can also be written in its row form as (1, 2)

    A dot product of two vectors V * W = V1W1 + V2W2

    Any vector V divided by its length ||V|| gives you the unit vector in the same direction as the original V vector.

    Dot product of two vectors V * W = 0 when the two vectors are perpendicular to each other.

    Unit Vectors u and U at angle Theta have u * U = cos Theta. Therefore, when v and w are nonzero vectors then V * W / ||V|| * ||W|| gives you the cosine angle between them.

    Matrix notation takes the form of A(row, col), so A(5, 7) is the 5th row and 7th column.

    
