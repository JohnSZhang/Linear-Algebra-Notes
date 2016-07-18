* Permutation Matrix P
    The Permutation Matrix P executes row exchanges.

    With row exchanges, A = LU becomes PA = LU where P is the identity matrix with some reordered rows. The total possible count of reordering (permutations) of an n by n permutation matrix is n! And P^-1 = P ^ T or that P * P^t = I.

    Transpose (A^t)ij = Aji. R^t * R is always symmetric, where a symmetric matrix is one whose transpose equals itself.

* Vector Spaces
    What is a vector space? for example R^2 is the space of all 2 dimensional real vectors, such as [2, 3], [pi, e], [0, 0] etc.

    R^n Space is the space of all vectors with n components where each component belongs to the group R.

    Vector Spaces have to be closed under all linear combination of vectors, so the positive x, y section of the x y plane is a real vector space (not closed under multiplication).

    However, the the subspace of a line through the origin of the x y plane would be a valid closed vector space, and a subspace of R^2 vector space.

    Subspaces of the vector space R^2 includes:
        1. All of R^2
        2. Any line through [0, 0]
        3. The 0 vector (Z)

    Given a matrix in a subspace (say 2 columns in R^3), if we take all the linear combinations of columns then we will get a column space C which is a subspace of the total vector space R^3. And those linear combinations will form a plane. This is an interesting conclusion, that 2 columns in R ^3 will be 2 lines that form a plane of vector subspace.

* From Book
    If A = LDU then A^t = L^t D^t U^t, and the pivot matrix has D = D^t (of course)

    Using Transpose of Matrix for calculations: we can see X^t * Y (1xn)(nx1) has the inner product of the two (or dot product). While X * Y ^ t is the outer product (nx1)(1xn) which produces a matrix.

    Inner product of A * x with y = Inner product of x with A^t * y

    When A is symmetric, A = LDU becomes A = LDL^t

    P and P^-1 are both transpose and inverse of each other, quite useful. 
