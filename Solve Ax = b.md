* Solving for Ax = b
    Ax = b is solvable when b is in the column space of A. If a combination of A gives zero row, then the same combination of the entries of b must also give 0.

    To find solution for Ax = b.
        1. We can set all free variables to zero, then we can solve Ax = b for the pivot variables. Then you have the particular solution where there are no free variables.

        2. Add on null space, x = xp + xn. This is because Axp = b, and Axn = 0, so Axp + Axn = b. So we can have the particular solution in the form of xcomplete = xp + c1xn1 + c2xn2 (where xns are special vectors of the null space of the matrix a). This will not be a subspace as xp will not be the origin, so whatever the null space will be will be shifted away from the origin by xp.

* Rank
    For a m by n matrix, the rank r will be <= m and r <= n. (because r cannot be more than the row length and each column can only have one pivot).

    Full column rand means r = n. This means there are no free variables and the N(A) = Z, and the solution of Ax = b is equal to Xp, there is only one particular solution.

    In case of r = m = n, R = I, 1 solution to Ax = b

    In case of r = n < m R = (I, 0), with 0 or one solution

    In case r = m < n, R = [I F] and there are always an infinite number of solutions because we have an infinite number combination of the null space

    In case r < m, r < n, R = (IF, 00). In this case either there's 0 solution or there will be an infinite number of solution.

    Because of the above cases, the rank is a crucial number that tells you a lot about the number of solutions to the problem of Ax = b.

* From the Book
    The definition of rank is the number of pivots that a matrix A has. Because often times rows are multiplies of each other it can be less than the number of rows that a matrix contains.

    We can also think of rank as the number of independent rows that A and U have, and that happens to also be the same rank number of independent columns.

    Lastly, the number of rank r is the dimension of the column space of the matrix, so even though a row have 6 columns, if only 2 of them are independent then its column space is just a line in 6 dimension space.

    Because the matrix A has r pivot columns and n - r number of free variables, there are exactly n - r special solutions in the null space matrix N(A).

    We can really think of it to mean that Ax = 0 has r independent equations only, which leaves us with n - r number of free variable independent solutions.

    Follow that logic, when A is square the invertible then it's reduced echelon form has to be the matrix I. 
