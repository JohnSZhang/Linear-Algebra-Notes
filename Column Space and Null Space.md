* More Subspaces
    Vector Space requirements: V + W and CV are in the subspace if all combinations of CV + DW are in the Space

    Give Subspaces P and L, is P union L (all vectors in P or L or both) a subspace? No, because you cannot add vectors from the two subspaces and still expect it to be in the subspace.

    Now given subspaces P and L, is P intersect L a subspace? Yes,

* Column Space
    Example A = [1 1 2]C(A) is a subspace of of R4
                [2 1 3]
                [3 1 4]
                [4 1 5]
    if we take all linear combination of those columns.

    Now for this particular A, which bs can we reach via some x for Ax = b? If and only if b is in the column space of the matrix A.

* Null Space
    The null space is all solutions of X (x1, x2, x3) for which Ax = 0. So instead looking for all b values, we instead only look for one particular b value (that of the zero vector)

    The zero vector will always be in the null space. In our example above, the null space is the space of c * (1, 1, -1). And is it always going to be a space because if AV = 0 and AW = 0 then A(V+W) = 0

    After reducing the matrix A to the reduced echelon form, we plug in numbers (usually 0, 1) for all the free variables and backwards substitute to get its 'special solutions' that will then combine to generate the entire null space.

    We can always find the null space matrix [-F]
                                             [ I]
    Assuming that the reduced echelon matrix is in [I F] form (F stands for free).
* From Book
    Why do we care about the column space? Imagine a matrix A, if A is not invertible then we know it is not possible to solve A for all values of b. But then which values of b can we solve for? This is the column space.

    S, the set of vectors in vector space V, SS all combinations of vectors in S. SS = all c1 * v1 + ... + cn * vn and is equal to the subspace of V 'spanned' by s. When S is the set of columns then SS is the column space.

    The null space of A, all solutions of x for which Ax = 0, is denoted by N(A) and can be found by elimination. Only none invertible matrices have null space other than the 0 value (because invertible ones do not have free variables after elimination).

    To solve for null space, we do a few more steps to the elimination process to produce the reduced system Rx = 0.

    The basic idea is to do forward elimination then back substitute in Rx = 0 to produce x. For such matrices, there are Columns which contain pivot variables, and Columns that do not (the free variable columns).

    Finding the special solutions to those pivot columns gives us Ux = 0 which is also Ax = 0, and they together generate the null space via linear combination.

    For a m by n matrix, the column space will be in the R ^ m space while the null space will be a subspace of R  ^ n. In the case that n > m, we will have nonzero solutions as there will be free variables left over after all pivots are resolved.

    Taking the Upper Echelon form one step further, we can subtract rows above pivots and multiple all rows by the inverse of the pivot to reach the reduced row echelon form (R). For any invertible matrix R = I.

    The ones and zeros of the reduced echelon form makes it easy to find special solutions of the matrix A, which will then linearly combine into the null space.
