* Linear Algebra
    Vectors -> Matrices -> Subspaces
    Vectors U, V, W with a linear combination with x1, x2, x3 (scalars) to get answer b.

    Taking a combination of Vectors is akin to filling out the columns of a matrix.

    If Ax = b, then the A^-1 (Inverse Matrix) gives you x for a given B. Ie x = A^-1b (Hence inverse is super important for transforming between solutions).

    Because a invertible matrix will be able to provide a solution for x with any given b, the original A that A^-1 came from contains 5 independent vectors that together gives a basis for the current space. (Any b can be reached from a particular x).

    A Subspace is a vector space inside a larger space (the whole space), think a plane inside a 3d space, a subspace an also be the same as the whole space.

* From Notes
    With not invertible matrix we have a solution x for which Ax = 0 (and x is not a zero vector). We cannot multiply both sides by A inverse to find a non-zero solution of x.

    Since Cx is the combination of all vectors, it is the solution subspace, which can be a plane for R3 in case of dependent vectors and the whole space if the vectors are independent.

    Vector Space is a collection of vectors closed under linear combination while subspace is a victor space in another vector space. The smallest subspace is the zero vector.

* From Book
   A matrix is invertible if from b we can get x, and because of that we can fill the entire vector space b from some combination of x.

   A Vector is said to be not independent if it's a linear combination of other vectors.

   If columns are independent, Ax = 0 has only one solution and the matrix is invertible, else the columns are dependent and Ax = 0 has many solutions and the matrix is a singular matrix.
